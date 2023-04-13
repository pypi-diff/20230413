# Comparing `tmp/byteblower-test-framework-1.0.0b8.tar.gz` & `tmp/byteblower-test-framework-1.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byteblower-test-framework-1.0.0b8.tar", last modified: Fri Feb  3 11:29:24 2023, max compression
+gzip compressed data, was "byteblower-test-framework-1.0.0b9.tar", last modified: Fri Feb  3 14:53:16 2023, max compression
```

## Comparing `byteblower-test-framework-1.0.0b8.tar` & `byteblower-test-framework-1.0.0b9.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0     7652 2022-12-15 08:52:49.386525 byteblower-test-framework-1.0.0b8/LICENSE
--rw-r--r--   0        0        0     8474 2023-02-02 10:21:00.465525 byteblower-test-framework-1.0.0b8/README.pypi.rst
--rw-r--r--   0        0        0      202 2023-02-02 10:21:00.465525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/__init__.py
--rw-r--r--   0        0        0        0 2023-02-02 10:21:00.465525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/__init__.py
--rw-r--r--   0        0        0    19816 2023-02-02 10:21:00.465525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/analyseraggregator.py
--rw-r--r--   0        0        0     9354 2023-02-02 10:21:00.465525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/bufferanalyser.py
--rw-r--r--   0        0        0       40 2023-02-02 10:21:00.465525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/data_analysis/__init__.py
--rw-r--r--   0        0        0      867 2023-02-02 10:21:00.465525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/data_analysis/data_analyser.py
--rw-r--r--   0        0        0    24483 2023-02-02 10:21:00.465525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/data_analysis/frameblasting.py
--rw-r--r--   0        0        0     1266 2023-02-02 10:21:00.465525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/data_analysis/tcp.py
--rw-r--r--   0        0        0       40 2023-02-02 10:21:00.465525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/data_gathering/__init__.py
--rw-r--r--   0        0        0      841 2023-02-02 10:21:00.465525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/data_gathering/data_gatherer.py
--rw-r--r--   0        0        0     4978 2023-02-02 10:21:00.465525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/data_gathering/tcp.py
--rw-r--r--   0        0        0    20380 2023-02-02 10:21:00.465525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/data_gathering/trigger.py
--rw-r--r--   0        0        0     3890 2023-02-02 10:21:00.465525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/flow_analyser.py
--rw-r--r--   0        0        0     8643 2023-02-02 10:21:00.465525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/framelossanalyser.py
--rw-r--r--   0        0        0     2733 2023-02-02 10:21:00.465525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/httpanalyser.py
--rw-r--r--   0        0        0    25376 2023-02-02 10:21:00.465525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/latencyanalyser.py
--rw-r--r--   0        0        0       40 2023-02-02 10:21:00.465525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/plotting/__init__.py
--rw-r--r--   0        0        0     4605 2023-02-02 10:21:00.465525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/plotting/generic_chart.py
--rw-r--r--   0        0        0       31 2023-02-02 10:21:00.465525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/render/__init__.py
--rw-r--r--   0        0        0    14952 2023-02-02 10:21:00.465525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/render/frameblasting.py
--rw-r--r--   0        0        0      868 2023-02-02 10:21:00.465525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/render/renderer.py
--rw-r--r--   0        0        0     1294 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/render/tcp.py
--rw-r--r--   0        0        0       34 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/storage/__init__.py
--rw-r--r--   0        0        0       44 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/storage/data_store.py
--rw-r--r--   0        0        0      619 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/storage/tcp.py
--rw-r--r--   0        0        0     4816 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/storage/trigger.py
--rw-r--r--   0        0        0     3518 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/voiceanalyser.py
--rw-r--r--   0        0        0        0 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_endpoint/__init__.py
--rw-r--r--   0        0        0        0 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_endpoint/ipv4/__init__.py
--rw-r--r--   0        0        0     7766 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_endpoint/ipv4/nat.py
--rw-r--r--   0        0        0     4441 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_endpoint/ipv4/port.py
--rw-r--r--   0        0        0        0 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_endpoint/ipv6/__init__.py
--rw-r--r--   0        0        0     3223 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_endpoint/ipv6/port.py
--rw-r--r--   0        0        0    11205 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_endpoint/port.py
--rw-r--r--   0        0        0        0 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_factory/__init__.py
--rw-r--r--   0        0        0     1477 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_factory/frame.py
--rw-r--r--   0        0        0        0 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_host/__init__.py
--rw-r--r--   0        0        0     1474 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_host/server.py
--rw-r--r--   0        0        0        0 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_report/__init__.py
--rw-r--r--   0        0        0     7751 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_report/byteblowerhtmlreport.py
--rw-r--r--   0        0        0     7339 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_report/byteblowerjsonreport.py
--rw-r--r--   0        0        0     3902 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_report/byteblowerreport.py
--rw-r--r--   0        0        0     2821 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_report/byteblowerunittestreport.py
--rw-r--r--   0        0        0      327 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_report/helper.py
--rw-r--r--   0        0        0     2039 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_report/options.py
--rw-r--r--   0        0        0      302 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_report/templates/flow_section.html
--rw-r--r--   0        0        0     1527 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_report/templates/report.html
--rw-r--r--   0        0        0      180 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_report/templates/test_section.html
--rw-r--r--   0        0        0     3194 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_report/unittestreport.py
--rw-r--r--   0        0        0     5770 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_scenario.py
--rw-r--r--   0        0        0        0 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_traffic/__init__.py
--rw-r--r--   0        0        0     4770 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_traffic/flow.py
--rw-r--r--   0        0        0     4104 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_traffic/frame.py
--rw-r--r--   0        0        0     5909 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_traffic/frameblastingflow.py
--rw-r--r--   0        0        0     5723 2023-02-02 11:12:59.487414 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_traffic/gamingflow.py
--rw-r--r--   0        0        0     4798 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_traffic/httpflow.py
--rw-r--r--   0        0        0     2748 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_traffic/imix.py
--rw-r--r--   0        0        0        0 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_traffic/ipv4/__init__.py
--rw-r--r--   0        0        0     3131 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_traffic/ipv4/frame.py
--rw-r--r--   0        0        0        0 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_traffic/ipv6/__init__.py
--rw-r--r--   0        0        0     2539 2023-02-03 11:28:16.307047 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_traffic/ipv6/frame.py
--rw-r--r--   0        0        0    13737 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_traffic/tcpflow.py
--rw-r--r--   0        0        0     6552 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_traffic/videoflow.py
--rw-r--r--   0        0        0     4809 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_traffic/voiceflow.py
--rw-r--r--   0        0        0      162 2023-02-03 11:29:23.878650 byteblower-test-framework-1.0.0b8/byteblower_test_framework/_version.py
--rw-r--r--   0        0        0      585 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/all.py
--rw-r--r--   0        0        0     1490 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/analysis.py
--rw-r--r--   0        0        0      983 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/endpoint.py
--rw-r--r--   0        0        0      773 2022-12-15 08:52:49.390526 byteblower-test-framework-1.0.0b8/byteblower_test_framework/exceptions.py
--rw-r--r--   0        0        0      320 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/factory.py
--rw-r--r--   0        0        0      338 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/host.py
--rw-r--r--   0        0        0      356 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/logging.py
--rw-r--r--   0        0        0     1125 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/report.py
--rw-r--r--   0        0        0     2898 2023-02-02 10:21:00.493525 byteblower-test-framework-1.0.0b8/byteblower_test_framework/traffic.py
--rw-r--r--   0        0        0     9058 2023-01-11 12:54:46.158901 byteblower-test-framework-1.0.0b8/pyproject.toml
--rw-r--r--   0        0        0    11180 1970-01-01 00:00:00.000000 byteblower-test-framework-1.0.0b8/PKG-INFO
+-rw-r--r--   0        0        0     7652 2022-10-20 08:28:27.544900 byteblower-test-framework-1.0.0b9/LICENSE
+-rw-r--r--   0        0        0     8474 2023-02-02 10:20:12.265718 byteblower-test-framework-1.0.0b9/README.pypi.rst
+-rw-r--r--   0        0        0      202 2023-02-02 10:20:12.265718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-02 10:20:12.265718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/__init__.py
+-rw-r--r--   0        0        0    19816 2023-02-02 10:20:12.265718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/analyseraggregator.py
+-rw-r--r--   0        0        0     9354 2023-02-02 10:20:12.265718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/bufferanalyser.py
+-rw-r--r--   0        0        0       40 2023-02-02 10:20:12.265718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/data_analysis/__init__.py
+-rw-r--r--   0        0        0      867 2023-02-02 10:20:12.265718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/data_analysis/data_analyser.py
+-rw-r--r--   0        0        0    24474 2023-02-03 14:39:47.959392 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/data_analysis/frameblasting.py
+-rw-r--r--   0        0        0     1266 2023-02-02 10:20:12.265718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/data_analysis/tcp.py
+-rw-r--r--   0        0        0       40 2023-02-02 10:20:12.265718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/data_gathering/__init__.py
+-rw-r--r--   0        0        0      841 2023-02-02 10:20:12.265718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/data_gathering/data_gatherer.py
+-rw-r--r--   0        0        0     4978 2023-02-02 10:20:12.265718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/data_gathering/tcp.py
+-rw-r--r--   0        0        0    20380 2023-02-02 10:20:12.265718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/data_gathering/trigger.py
+-rw-r--r--   0        0        0     3890 2023-02-02 10:20:12.265718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/flow_analyser.py
+-rw-r--r--   0        0        0     8643 2023-02-02 10:20:12.269718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/framelossanalyser.py
+-rw-r--r--   0        0        0     2733 2023-02-02 10:20:12.269718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/httpanalyser.py
+-rw-r--r--   0        0        0    25376 2023-02-02 10:20:12.269718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/latencyanalyser.py
+-rw-r--r--   0        0        0       40 2023-02-02 10:20:12.269718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/plotting/__init__.py
+-rw-r--r--   0        0        0     4605 2023-02-02 10:20:12.269718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/plotting/generic_chart.py
+-rw-r--r--   0        0        0       31 2023-02-02 10:20:12.269718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/render/__init__.py
+-rw-r--r--   0        0        0    14952 2023-02-02 10:20:12.269718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/render/frameblasting.py
+-rw-r--r--   0        0        0      868 2023-02-02 10:20:12.269718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/render/renderer.py
+-rw-r--r--   0        0        0     1294 2023-02-02 10:20:12.269718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/render/tcp.py
+-rw-r--r--   0        0        0       34 2023-02-02 10:20:12.269718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/storage/__init__.py
+-rw-r--r--   0        0        0       44 2023-02-02 10:20:12.269718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/storage/data_store.py
+-rw-r--r--   0        0        0      619 2023-02-02 10:20:12.269718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/storage/tcp.py
+-rw-r--r--   0        0        0     4816 2023-02-02 10:20:12.269718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/storage/trigger.py
+-rw-r--r--   0        0        0     3518 2023-02-02 10:20:12.269718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/voiceanalyser.py
+-rw-r--r--   0        0        0        0 2023-02-02 10:20:12.269718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_endpoint/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-02 10:20:12.269718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_endpoint/ipv4/__init__.py
+-rw-r--r--   0        0        0     7766 2023-02-02 10:20:12.269718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_endpoint/ipv4/nat.py
+-rw-r--r--   0        0        0     4441 2023-02-02 10:20:12.269718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_endpoint/ipv4/port.py
+-rw-r--r--   0        0        0        0 2023-02-02 10:20:12.269718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_endpoint/ipv6/__init__.py
+-rw-r--r--   0        0        0     3223 2023-02-02 10:20:12.269718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_endpoint/ipv6/port.py
+-rw-r--r--   0        0        0    11205 2023-02-02 10:20:12.269718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_endpoint/port.py
+-rw-r--r--   0        0        0        0 2023-02-02 10:20:12.269718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_factory/__init__.py
+-rw-r--r--   0        0        0     1477 2023-02-02 10:20:12.269718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_factory/frame.py
+-rw-r--r--   0        0        0        0 2023-02-02 10:20:12.269718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_host/__init__.py
+-rw-r--r--   0        0        0     1474 2023-02-02 10:20:12.269718 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_host/server.py
+-rw-r--r--   0        0        0        0 2023-02-02 10:20:12.273717 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_report/__init__.py
+-rw-r--r--   0        0        0     7751 2023-02-02 10:20:12.273717 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_report/byteblowerhtmlreport.py
+-rw-r--r--   0        0        0     7339 2023-02-02 10:20:12.273717 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_report/byteblowerjsonreport.py
+-rw-r--r--   0        0        0     3902 2023-02-02 10:20:12.273717 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_report/byteblowerreport.py
+-rw-r--r--   0        0        0     2821 2023-02-02 10:20:12.273717 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_report/byteblowerunittestreport.py
+-rw-r--r--   0        0        0      327 2023-02-02 10:20:12.273717 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_report/helper.py
+-rw-r--r--   0        0        0     2039 2023-02-02 10:20:12.273717 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_report/options.py
+-rw-r--r--   0        0        0      302 2023-02-02 10:20:12.273717 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_report/templates/flow_section.html
+-rw-r--r--   0        0        0     1527 2023-02-02 10:20:12.273717 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_report/templates/report.html
+-rw-r--r--   0        0        0      180 2023-02-02 10:20:12.273717 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_report/templates/test_section.html
+-rw-r--r--   0        0        0     3194 2023-02-02 10:20:12.273717 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_report/unittestreport.py
+-rw-r--r--   0        0        0     5770 2023-02-02 10:20:12.273717 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_scenario.py
+-rw-r--r--   0        0        0        0 2023-02-02 10:20:12.273717 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_traffic/__init__.py
+-rw-r--r--   0        0        0     4770 2023-02-02 10:20:12.273717 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_traffic/flow.py
+-rw-r--r--   0        0        0     4104 2023-02-02 10:20:12.273717 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_traffic/frame.py
+-rw-r--r--   0        0        0     5909 2023-02-02 10:20:12.273717 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_traffic/frameblastingflow.py
+-rw-r--r--   0        0        0     5723 2023-02-02 11:11:53.254310 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_traffic/gamingflow.py
+-rw-r--r--   0        0        0     4798 2023-02-02 10:20:12.273717 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_traffic/httpflow.py
+-rw-r--r--   0        0        0     2748 2023-02-02 10:20:12.273717 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_traffic/imix.py
+-rw-r--r--   0        0        0        0 2023-02-02 10:20:12.273717 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_traffic/ipv4/__init__.py
+-rw-r--r--   0        0        0     3131 2023-02-02 10:20:12.273717 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_traffic/ipv4/frame.py
+-rw-r--r--   0        0        0        0 2023-02-02 10:20:12.273717 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_traffic/ipv6/__init__.py
+-rw-r--r--   0        0        0     2539 2023-02-03 08:56:53.382112 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_traffic/ipv6/frame.py
+-rw-r--r--   0        0        0    13737 2023-02-02 10:20:12.273717 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_traffic/tcpflow.py
+-rw-r--r--   0        0        0     6552 2023-02-02 10:20:12.273717 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_traffic/videoflow.py
+-rw-r--r--   0        0        0     4809 2023-02-02 10:20:12.273717 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_traffic/voiceflow.py
+-rw-r--r--   0        0        0      162 2023-02-03 14:53:15.178245 byteblower-test-framework-1.0.0b9/byteblower_test_framework/_version.py
+-rw-r--r--   0        0        0      585 2023-02-02 10:20:12.273717 byteblower-test-framework-1.0.0b9/byteblower_test_framework/all.py
+-rw-r--r--   0        0        0     1490 2023-02-02 10:20:12.273717 byteblower-test-framework-1.0.0b9/byteblower_test_framework/analysis.py
+-rw-r--r--   0        0        0      983 2023-02-02 10:20:12.273717 byteblower-test-framework-1.0.0b9/byteblower_test_framework/endpoint.py
+-rw-r--r--   0        0        0      773 2022-10-26 14:02:37.222102 byteblower-test-framework-1.0.0b9/byteblower_test_framework/exceptions.py
+-rw-r--r--   0        0        0      320 2023-02-02 10:20:12.277717 byteblower-test-framework-1.0.0b9/byteblower_test_framework/factory.py
+-rw-r--r--   0        0        0      338 2023-02-02 10:20:12.277717 byteblower-test-framework-1.0.0b9/byteblower_test_framework/host.py
+-rw-r--r--   0        0        0      356 2023-02-02 10:20:12.277717 byteblower-test-framework-1.0.0b9/byteblower_test_framework/logging.py
+-rw-r--r--   0        0        0     1125 2023-02-02 10:20:12.277717 byteblower-test-framework-1.0.0b9/byteblower_test_framework/report.py
+-rw-r--r--   0        0        0     2898 2023-02-02 10:20:12.277717 byteblower-test-framework-1.0.0b9/byteblower_test_framework/traffic.py
+-rw-r--r--   0        0        0     9058 2023-01-11 12:52:35.905819 byteblower-test-framework-1.0.0b9/pyproject.toml
+-rw-r--r--   0        0        0    11180 1970-01-01 00:00:00.000000 byteblower-test-framework-1.0.0b9/PKG-INFO
```

### Comparing `byteblower-test-framework-1.0.0b8/LICENSE` & `byteblower-test-framework-1.0.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/README.pypi.rst` & `byteblower-test-framework-1.0.0b9/README.pypi.rst`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/analyseraggregator.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/analyseraggregator.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/bufferanalyser.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/bufferanalyser.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/data_analysis/data_analyser.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/data_analysis/data_analyser.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/data_analysis/frameblasting.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/data_analysis/frameblasting.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,15 +396,15 @@
             cumul = 0
             for x in range(0, len(packet_count_buckets)):
                 cumul += packet_count_buckets[x]
                 if cumul > threshold:
                     df_latency_update = DataFrame(
                         {
                             'latency': [(x + 1) * bucket_width],
-                            'percentile': [100.0 - percentile]
+                            'percentile': percentile,
                         }
                     )
 
                     self._df_latency = concat(
                         [self._df_latency, df_latency_update],
                         ignore_index=True
                     )
```

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/data_analysis/tcp.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/data_analysis/tcp.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/data_gathering/data_gatherer.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/data_gathering/data_gatherer.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/data_gathering/tcp.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/data_gathering/tcp.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/data_gathering/trigger.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/data_gathering/trigger.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/flow_analyser.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/flow_analyser.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/framelossanalyser.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/framelossanalyser.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/httpanalyser.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/httpanalyser.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/latencyanalyser.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/latencyanalyser.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/plotting/generic_chart.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/plotting/generic_chart.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/render/frameblasting.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/render/frameblasting.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/render/renderer.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/render/renderer.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/render/tcp.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/render/tcp.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/storage/tcp.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/storage/tcp.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/storage/trigger.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/storage/trigger.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_analysis/voiceanalyser.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_analysis/voiceanalyser.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_endpoint/ipv4/nat.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_endpoint/ipv4/nat.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_endpoint/ipv4/port.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_endpoint/ipv4/port.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_endpoint/ipv6/port.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_endpoint/ipv6/port.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_endpoint/port.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_endpoint/port.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_factory/frame.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_factory/frame.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_host/server.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_host/server.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_report/byteblowerhtmlreport.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_report/byteblowerhtmlreport.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_report/byteblowerjsonreport.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_report/byteblowerjsonreport.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_report/byteblowerreport.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_report/byteblowerreport.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_report/byteblowerunittestreport.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_report/byteblowerunittestreport.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_report/options.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_report/options.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_report/templates/report.html` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_report/templates/report.html`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_report/unittestreport.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_report/unittestreport.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_scenario.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_scenario.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_traffic/flow.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_traffic/flow.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_traffic/frame.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_traffic/frame.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_traffic/frameblastingflow.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_traffic/frameblastingflow.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_traffic/gamingflow.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_traffic/gamingflow.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_traffic/httpflow.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_traffic/httpflow.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_traffic/imix.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_traffic/imix.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_traffic/ipv4/frame.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_traffic/ipv4/frame.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_traffic/ipv6/frame.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_traffic/ipv6/frame.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_traffic/tcpflow.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_traffic/tcpflow.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_traffic/videoflow.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_traffic/videoflow.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/_traffic/voiceflow.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/_traffic/voiceflow.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/all.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/all.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/analysis.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/analysis.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/endpoint.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/endpoint.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/exceptions.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/exceptions.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/report.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/report.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/byteblower_test_framework/traffic.py` & `byteblower-test-framework-1.0.0b9/byteblower_test_framework/traffic.py`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/pyproject.toml` & `byteblower-test-framework-1.0.0b9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `byteblower-test-framework-1.0.0b8/PKG-INFO` & `byteblower-test-framework-1.0.0b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byteblower-test-framework
-Version: 1.0.0b8
+Version: 1.0.0b9
 Summary: Test Framework for the ByteBlower Traffic Generator.
 Keywords: ByteBlower,Test Framework
 Author-email: ByteBlower Development Team <support.byteblower@excentis.com>
 Maintainer-email: Tom Ghyselinck <tom.ghyselinck@excentis.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
```

