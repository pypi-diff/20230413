# Comparing `tmp/joulescope-1.1.2.tar.gz` & `tmp/joulescope-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joulescope-1.1.2.tar", last modified: Mon Mar 20 19:45:57 2023, max compression
+gzip compressed data, was "joulescope-1.1.3.tar", last modified: Thu Apr 13 20:58:40 2023, max compression
```

## Comparing `joulescope-1.1.2.tar` & `joulescope-1.1.3.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxrwxrwx   0        0        0        0 2023-03-20 19:45:57.860389 joulescope-1.1.2/
--rw-rw-rw-   0        0        0    21482 2023-03-20 19:31:59.000000 joulescope-1.1.2/CHANGELOG.md
--rw-rw-rw-   0        0        0     6771 2020-08-11 21:29:57.000000 joulescope-1.1.2/CREDITS.html
--rw-rw-rw-   0        0        0    11558 2020-05-30 15:27:09.000000 joulescope-1.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0      132 2022-11-07 18:35:15.000000 joulescope-1.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3628 2023-03-20 19:45:57.860389 joulescope-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1762 2020-11-25 13:12:14.000000 joulescope-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-20 19:45:57.820861 joulescope-1.1.2/joulescope/
--rw-rw-rw-   0        0        0     2291 2023-03-20 19:38:30.000000 joulescope-1.1.2/joulescope/__init__.py
--rw-rw-rw-   0        0        0      730 2020-05-30 15:27:09.000000 joulescope-1.1.2/joulescope/__main__.py
--rw-rw-rw-   0        0        0    54968 2023-03-11 15:21:25.000000 joulescope-1.1.2/joulescope/data_recorder.py
--rw-rw-rw-   0        0        0    26397 2022-09-09 13:37:25.000000 joulescope-1.1.2/joulescope/datafile.py
-drwxrwxrwx   0        0        0        0 2023-03-20 19:45:57.835867 joulescope-1.1.2/joulescope/entry_points/
--rw-rw-rw-   0        0        0        0 2020-05-30 15:27:09.000000 joulescope-1.1.2/joulescope/entry_points/__init__.py
--rw-rw-rw-   0        0        0     1325 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/entry_points/bootloader_go.py
--rw-rw-rw-   0        0        0     4040 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/entry_points/capture.py
--rw-rw-rw-   0        0        0     1530 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/entry_points/gpo_demo.py
--rw-rw-rw-   0        0        0     2103 2022-09-09 18:57:06.000000 joulescope-1.1.2/joulescope/entry_points/info.py
--rw-rw-rw-   0        0        0     2110 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/entry_points/parameter_set.py
--rw-rw-rw-   0        0        0     5043 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/entry_points/program.py
--rw-rw-rw-   0        0        0     6546 2022-09-10 13:15:16.000000 joulescope-1.1.2/joulescope/entry_points/recording.py
--rw-rw-rw-   0        0        0     3609 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/entry_points/runner.py
--rw-rw-rw-   0        0        0      865 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/entry_points/scan.py
--rw-rw-rw-   0        0        0     2883 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/entry_points/statistics.py
--rw-rw-rw-   0        0        0     2814 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/entry_points/stream_test.py
--rw-rw-rw-   0        0        0     3000 2020-05-30 15:27:09.000000 joulescope-1.1.2/joulescope/file_replace.py
--rw-rw-rw-   0        0        0     5532 2023-02-22 12:49:19.000000 joulescope-1.1.2/joulescope/jls_v2_writer.py
--rw-rw-rw-   0        0        0     3056 2022-09-09 13:37:25.000000 joulescope-1.1.2/joulescope/parameter.py
--rw-rw-rw-   0        0        0    11070 2022-11-07 22:01:01.000000 joulescope-1.1.2/joulescope/parameters_v1.py
--rw-rw-rw-   0        0        0     8797 2022-12-20 13:24:03.000000 joulescope-1.1.2/joulescope/span.py
--rw-rw-rw-   0        0        0      653 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/stream_buffer.py
-drwxrwxrwx   0        0        0        0 2023-03-20 19:45:57.839879 joulescope-1.1.2/joulescope/test/
--rw-rw-rw-   0        0        0        0 2020-05-30 15:27:09.000000 joulescope-1.1.2/joulescope/test/__init__.py
--rw-rw-rw-   0        0        0    16330 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/test/test_data_recorder.py
--rw-rw-rw-   0        0        0     5407 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/test/test_data_recorder_downsampled.py
--rw-rw-rw-   0        0        0     2484 2020-05-30 15:27:09.000000 joulescope-1.1.2/joulescope/test/test_file_replace.py
--rw-rw-rw-   0        0        0     4237 2022-11-21 18:21:24.000000 joulescope-1.1.2/joulescope/test/test_jls_v2_writer.py
--rw-rw-rw-   0        0        0     2902 2021-03-09 14:36:24.000000 joulescope-1.1.2/joulescope/test/test_span.py
--rw-rw-rw-   0        0        0     1179 2020-05-30 15:27:09.000000 joulescope-1.1.2/joulescope/test/test_time.py
--rw-rw-rw-   0        0        0     4631 2021-11-19 14:35:42.000000 joulescope-1.1.2/joulescope/test/test_units.py
--rw-rw-rw-   0        0        0    10876 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/test_datafile.py
--rw-rw-rw-   0        0        0     2189 2020-05-30 15:27:09.000000 joulescope-1.1.2/joulescope/time.py
--rw-rw-rw-   0        0        0     4736 2021-11-19 14:35:42.000000 joulescope-1.1.2/joulescope/units.py
-drwxrwxrwx   0        0        0        0 2023-03-20 19:45:57.843878 joulescope-1.1.2/joulescope/v0/
--rw-rw-rw-   0        0        0        0 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/__init__.py
--rw-rw-rw-   0        0        0     6362 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/array_storage.py
--rw-rw-rw-   0        0        0    12568 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/bootloader.py
--rw-rw-rw-   0        0        0     9922 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/calibration.py
--rw-rw-rw-   0        0        0    85576 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/decimators.py
--rw-rw-rw-   0        0        0    58006 2023-03-20 19:36:21.000000 joulescope-1.1.2/joulescope/v0/driver.py
--rw-rw-rw-   0        0        0   955367 2023-03-09 19:27:11.000000 joulescope-1.1.2/joulescope/v0/filter_fir.c
--rw-rw-rw-   0        0        0     6132 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/firmware_manager.py
-drwxrwxrwx   0        0        0        0 2023-03-20 19:45:57.845378 joulescope-1.1.2/joulescope/v0/native/
--rw-rw-rw-   0        0        0     3763 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/native/filter_fir.c
--rw-rw-rw-   0        0        0     2904 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/native/filter_fir.h
--rw-rw-rw-   0        0        0     2647 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/native/running_statistics.c
--rw-rw-rw-   0        0        0     2891 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/native/running_statistics.h
-drwxrwxrwx   0        0        0        0 2023-03-20 19:45:57.846378 joulescope-1.1.2/joulescope/v0/native/test/
--rw-rw-rw-   0        0        0    57119 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/native/test/acutest.h
--rw-rw-rw-   0        0        0     2942 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/native/test/test_filter_fir.c
--rw-rw-rw-   0        0        0     1913 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/notification_handler.py
--rw-rw-rw-   0        0        0   432133 2023-03-10 18:01:01.000000 joulescope-1.1.2/joulescope/v0/pattern_buffer.c
--rw-rw-rw-   0        0        0     1245 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/public_keys.py
--rw-rw-rw-   0        0        0  2673525 2023-03-09 19:27:12.000000 joulescope-1.1.2/joulescope/v0/stream_buffer.c
-drwxrwxrwx   0        0        0        0 2023-03-20 19:45:57.850384 joulescope-1.1.2/joulescope/v0/test/
--rw-rw-rw-   0        0        0        0 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/test/__init__.py
--rw-rw-rw-   0        0        0     2999 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/test/test_array_storage.py
--rw-rw-rw-   0        0        0     3717 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/test/test_calibration.py
--rw-rw-rw-   0        0        0     4551 2023-03-10 18:03:29.000000 joulescope-1.1.2/joulescope/v0/test/test_device.py
--rw-rw-rw-   0        0        0     2308 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/test/test_filter_fir.py
--rw-rw-rw-   0        0        0     1418 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/test/test_parameter.py
--rw-rw-rw-   0        0        0     3379 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/test/test_pattern_buffer.py
--rw-rw-rw-   0        0        0     3670 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/test/test_stats.py
--rw-rw-rw-   0        0        0    24677 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/test/test_stream_buffer.py
--rw-rw-rw-   0        0        0     1793 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/test/test_view.py
-drwxrwxrwx   0        0        0        0 2023-03-20 19:45:57.853384 joulescope-1.1.2/joulescope/v0/usb/
--rw-rw-rw-   0        0        0      758 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/usb/__init__.py
--rw-rw-rw-   0        0        0     8886 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/usb/api.py
--rw-rw-rw-   0        0        0     5114 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/usb/core.py
--rw-rw-rw-   0        0        0     8111 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/usb/device_thread.py
--rw-rw-rw-   0        0        0     4046 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/usb/hw_tests.py
--rw-rw-rw-   0        0        0     1542 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/usb/impl_tools.py
-drwxrwxrwx   0        0        0        0 2023-03-20 19:45:57.854384 joulescope-1.1.2/joulescope/v0/usb/libusb/
--rw-rw-rw-   0        0        0        0 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/usb/libusb/__init__.py
--rw-rw-rw-   0        0        0    40907 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/usb/libusb/device.py
--rw-rw-rw-   0        0        0     2406 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/usb/scan_info.py
-drwxrwxrwx   0        0        0        0 2023-03-20 19:45:57.856384 joulescope-1.1.2/joulescope/v0/usb/winusb/
--rw-rw-rw-   0        0        0        0 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/usb/winusb/__init__.py
--rw-rw-rw-   0        0        0    35453 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/usb/winusb/device.py
--rw-rw-rw-   0        0        0     8061 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/usb/winusb/kernel32.py
--rw-rw-rw-   0        0        0     6017 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/usb/winusb/setupapi.py
--rw-rw-rw-   0        0        0     5280 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v0/usb/winusb/win32_device_notify.py
-drwxrwxrwx   0        0        0        0 2023-03-20 19:45:57.859389 joulescope-1.1.2/joulescope/v1/
--rw-rw-rw-   0        0        0      690 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v1/__init__.py
--rw-rw-rw-   0        0        0    28152 2023-01-25 15:17:35.000000 joulescope-1.1.2/joulescope/v1/device.py
--rw-rw-rw-   0        0        0     7317 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v1/driver.py
--rw-rw-rw-   0        0        0     5627 2023-01-25 15:11:23.000000 joulescope-1.1.2/joulescope/v1/js110.py
--rw-rw-rw-   0        0        0     7534 2023-01-25 15:11:30.000000 joulescope-1.1.2/joulescope/v1/js220.py
--rw-rw-rw-   0        0        0     6630 2023-02-15 17:15:30.000000 joulescope-1.1.2/joulescope/v1/sample_buffer.py
--rw-rw-rw-   0        0        0   887106 2023-03-09 19:27:13.000000 joulescope-1.1.2/joulescope/v1/stats.c
--rw-rw-rw-   0        0        0    16097 2022-11-11 18:39:12.000000 joulescope-1.1.2/joulescope/v1/stream_buffer.py
-drwxrwxrwx   0        0        0        0 2023-03-20 19:45:57.859889 joulescope-1.1.2/joulescope/v1/test/
--rw-rw-rw-   0        0        0        0 2022-10-30 18:42:53.000000 joulescope-1.1.2/joulescope/v1/test/__init__.py
--rw-rw-rw-   0        0        0     3047 2022-11-10 15:29:05.000000 joulescope-1.1.2/joulescope/v1/test/test_sample_buffer.py
--rw-rw-rw-   0        0        0      470 2023-03-20 19:33:51.000000 joulescope-1.1.2/joulescope/version.py
--rw-rw-rw-   0        0        0    21187 2022-11-11 15:21:00.000000 joulescope-1.1.2/joulescope/view.py
-drwxrwxrwx   0        0        0        0 2023-03-20 19:45:57.824362 joulescope-1.1.2/joulescope.egg-info/
--rw-rw-rw-   0        0        0     3628 2023-03-20 19:45:57.000000 joulescope-1.1.2/joulescope.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3265 2023-03-20 19:45:57.000000 joulescope-1.1.2/joulescope.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-20 19:45:57.000000 joulescope-1.1.2/joulescope.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-03-20 19:45:57.000000 joulescope-1.1.2/joulescope.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      200 2023-03-20 19:45:57.000000 joulescope-1.1.2/joulescope.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-03-20 19:45:57.000000 joulescope-1.1.2/joulescope.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      851 2022-11-30 15:24:46.000000 joulescope-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0      117 2023-03-20 19:45:57.863889 joulescope-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     6882 2023-03-16 19:48:12.000000 joulescope-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:40.121279 joulescope-1.1.3/
+-rw-rw-rw-   0        0        0    21564 2023-04-13 20:52:18.000000 joulescope-1.1.3/CHANGELOG.md
+-rw-rw-rw-   0        0        0     6771 2020-08-11 21:29:57.000000 joulescope-1.1.3/CREDITS.html
+-rw-rw-rw-   0        0        0    11558 2020-05-30 15:27:09.000000 joulescope-1.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      132 2022-11-07 18:35:15.000000 joulescope-1.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3628 2023-04-13 20:58:40.121279 joulescope-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1762 2020-11-25 13:12:14.000000 joulescope-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:40.048838 joulescope-1.1.3/joulescope/
+-rw-rw-rw-   0        0        0     2291 2023-03-20 19:38:30.000000 joulescope-1.1.3/joulescope/__init__.py
+-rw-rw-rw-   0        0        0      730 2020-05-30 15:27:09.000000 joulescope-1.1.3/joulescope/__main__.py
+-rw-rw-rw-   0        0        0    54968 2023-03-11 15:21:25.000000 joulescope-1.1.3/joulescope/data_recorder.py
+-rw-rw-rw-   0        0        0    26397 2022-09-09 13:37:25.000000 joulescope-1.1.3/joulescope/datafile.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:40.086705 joulescope-1.1.3/joulescope/entry_points/
+-rw-rw-rw-   0        0        0        0 2020-05-30 15:27:09.000000 joulescope-1.1.3/joulescope/entry_points/__init__.py
+-rw-rw-rw-   0        0        0     1325 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/entry_points/bootloader_go.py
+-rw-rw-rw-   0        0        0     4040 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/entry_points/capture.py
+-rw-rw-rw-   0        0        0     1530 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/entry_points/gpo_demo.py
+-rw-rw-rw-   0        0        0     2103 2022-09-09 18:57:06.000000 joulescope-1.1.3/joulescope/entry_points/info.py
+-rw-rw-rw-   0        0        0     2110 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/entry_points/parameter_set.py
+-rw-rw-rw-   0        0        0     5043 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/entry_points/program.py
+-rw-rw-rw-   0        0        0     6546 2022-09-10 13:15:16.000000 joulescope-1.1.3/joulescope/entry_points/recording.py
+-rw-rw-rw-   0        0        0     3609 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/entry_points/runner.py
+-rw-rw-rw-   0        0        0      865 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/entry_points/scan.py
+-rw-rw-rw-   0        0        0     2883 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/entry_points/statistics.py
+-rw-rw-rw-   0        0        0     2814 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/entry_points/stream_test.py
+-rw-rw-rw-   0        0        0     3000 2020-05-30 15:27:09.000000 joulescope-1.1.3/joulescope/file_replace.py
+-rw-rw-rw-   0        0        0     5532 2023-02-22 12:49:19.000000 joulescope-1.1.3/joulescope/jls_v2_writer.py
+-rw-rw-rw-   0        0        0     3056 2022-09-09 13:37:25.000000 joulescope-1.1.3/joulescope/parameter.py
+-rw-rw-rw-   0        0        0    11070 2022-11-07 22:01:01.000000 joulescope-1.1.3/joulescope/parameters_v1.py
+-rw-rw-rw-   0        0        0     8797 2022-12-20 13:24:03.000000 joulescope-1.1.3/joulescope/span.py
+-rw-rw-rw-   0        0        0      653 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/stream_buffer.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:40.090213 joulescope-1.1.3/joulescope/test/
+-rw-rw-rw-   0        0        0        0 2020-05-30 15:27:09.000000 joulescope-1.1.3/joulescope/test/__init__.py
+-rw-rw-rw-   0        0        0    16330 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/test/test_data_recorder.py
+-rw-rw-rw-   0        0        0     5407 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/test/test_data_recorder_downsampled.py
+-rw-rw-rw-   0        0        0     2484 2020-05-30 15:27:09.000000 joulescope-1.1.3/joulescope/test/test_file_replace.py
+-rw-rw-rw-   0        0        0     4237 2022-11-21 18:21:24.000000 joulescope-1.1.3/joulescope/test/test_jls_v2_writer.py
+-rw-rw-rw-   0        0        0     2902 2021-03-09 14:36:24.000000 joulescope-1.1.3/joulescope/test/test_span.py
+-rw-rw-rw-   0        0        0     1179 2020-05-30 15:27:09.000000 joulescope-1.1.3/joulescope/test/test_time.py
+-rw-rw-rw-   0        0        0     4631 2021-11-19 14:35:42.000000 joulescope-1.1.3/joulescope/test/test_units.py
+-rw-rw-rw-   0        0        0    10876 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/test_datafile.py
+-rw-rw-rw-   0        0        0     2189 2020-05-30 15:27:09.000000 joulescope-1.1.3/joulescope/time.py
+-rw-rw-rw-   0        0        0     4736 2021-11-19 14:35:42.000000 joulescope-1.1.3/joulescope/units.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:40.093721 joulescope-1.1.3/joulescope/v0/
+-rw-rw-rw-   0        0        0        0 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/__init__.py
+-rw-rw-rw-   0        0        0     6362 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/array_storage.py
+-rw-rw-rw-   0        0        0    12568 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/bootloader.py
+-rw-rw-rw-   0        0        0     9922 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/calibration.py
+-rw-rw-rw-   0        0        0    85576 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/decimators.py
+-rw-rw-rw-   0        0        0    58006 2023-03-20 19:36:21.000000 joulescope-1.1.3/joulescope/v0/driver.py
+-rw-rw-rw-   0        0        0   957021 2023-04-04 17:52:34.000000 joulescope-1.1.3/joulescope/v0/filter_fir.c
+-rw-rw-rw-   0        0        0     6132 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/firmware_manager.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:40.100737 joulescope-1.1.3/joulescope/v0/native/
+-rw-rw-rw-   0        0        0     3763 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/native/filter_fir.c
+-rw-rw-rw-   0        0        0     2904 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/native/filter_fir.h
+-rw-rw-rw-   0        0        0     2647 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/native/running_statistics.c
+-rw-rw-rw-   0        0        0     2891 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/native/running_statistics.h
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:40.107252 joulescope-1.1.3/joulescope/v0/native/test/
+-rw-rw-rw-   0        0        0    57119 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/native/test/acutest.h
+-rw-rw-rw-   0        0        0     2942 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/native/test/test_filter_fir.c
+-rw-rw-rw-   0        0        0     1913 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/notification_handler.py
+-rw-rw-rw-   0        0        0   433682 2023-04-04 17:52:35.000000 joulescope-1.1.3/joulescope/v0/pattern_buffer.c
+-rw-rw-rw-   0        0        0     1245 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/public_keys.py
+-rw-rw-rw-   0        0        0  2675267 2023-04-04 17:52:35.000000 joulescope-1.1.3/joulescope/v0/stream_buffer.c
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:40.111261 joulescope-1.1.3/joulescope/v0/test/
+-rw-rw-rw-   0        0        0        0 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/test/__init__.py
+-rw-rw-rw-   0        0        0     2999 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/test/test_array_storage.py
+-rw-rw-rw-   0        0        0     3717 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/test/test_calibration.py
+-rw-rw-rw-   0        0        0     4551 2023-03-10 18:03:29.000000 joulescope-1.1.3/joulescope/v0/test/test_device.py
+-rw-rw-rw-   0        0        0     2308 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/test/test_filter_fir.py
+-rw-rw-rw-   0        0        0     1418 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/test/test_parameter.py
+-rw-rw-rw-   0        0        0     3379 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/test/test_pattern_buffer.py
+-rw-rw-rw-   0        0        0     3670 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/test/test_stats.py
+-rw-rw-rw-   0        0        0    24677 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/test/test_stream_buffer.py
+-rw-rw-rw-   0        0        0     1793 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/test/test_view.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:40.113765 joulescope-1.1.3/joulescope/v0/usb/
+-rw-rw-rw-   0        0        0      758 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/usb/__init__.py
+-rw-rw-rw-   0        0        0     8886 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/usb/api.py
+-rw-rw-rw-   0        0        0     5114 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/usb/core.py
+-rw-rw-rw-   0        0        0     8111 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/usb/device_thread.py
+-rw-rw-rw-   0        0        0     4046 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/usb/hw_tests.py
+-rw-rw-rw-   0        0        0     1542 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/usb/impl_tools.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:40.114768 joulescope-1.1.3/joulescope/v0/usb/libusb/
+-rw-rw-rw-   0        0        0        0 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/usb/libusb/__init__.py
+-rw-rw-rw-   0        0        0    40907 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/usb/libusb/device.py
+-rw-rw-rw-   0        0        0     2406 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/usb/scan_info.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:40.116773 joulescope-1.1.3/joulescope/v0/usb/winusb/
+-rw-rw-rw-   0        0        0        0 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/usb/winusb/__init__.py
+-rw-rw-rw-   0        0        0    35453 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/usb/winusb/device.py
+-rw-rw-rw-   0        0        0     8061 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/usb/winusb/kernel32.py
+-rw-rw-rw-   0        0        0     6017 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/usb/winusb/setupapi.py
+-rw-rw-rw-   0        0        0     5280 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v0/usb/winusb/win32_device_notify.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:40.120276 joulescope-1.1.3/joulescope/v1/
+-rw-rw-rw-   0        0        0      690 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v1/__init__.py
+-rw-rw-rw-   0        0        0    28152 2023-01-25 15:17:35.000000 joulescope-1.1.3/joulescope/v1/device.py
+-rw-rw-rw-   0        0        0     7317 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v1/driver.py
+-rw-rw-rw-   0        0        0     5627 2023-01-25 15:11:23.000000 joulescope-1.1.3/joulescope/v1/js110.py
+-rw-rw-rw-   0        0        0     7534 2023-01-25 15:11:30.000000 joulescope-1.1.3/joulescope/v1/js220.py
+-rw-rw-rw-   0        0        0     6630 2023-02-15 17:15:30.000000 joulescope-1.1.3/joulescope/v1/sample_buffer.py
+-rw-rw-rw-   0        0        0   888760 2023-04-04 17:52:36.000000 joulescope-1.1.3/joulescope/v1/stats.c
+-rw-rw-rw-   0        0        0    16328 2023-04-12 13:39:59.000000 joulescope-1.1.3/joulescope/v1/stream_buffer.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:40.120779 joulescope-1.1.3/joulescope/v1/test/
+-rw-rw-rw-   0        0        0        0 2022-10-30 18:42:53.000000 joulescope-1.1.3/joulescope/v1/test/__init__.py
+-rw-rw-rw-   0        0        0     3047 2022-11-10 15:29:05.000000 joulescope-1.1.3/joulescope/v1/test/test_sample_buffer.py
+-rw-rw-rw-   0        0        0      470 2023-04-11 14:30:33.000000 joulescope-1.1.3/joulescope/version.py
+-rw-rw-rw-   0        0        0    21187 2022-11-11 15:21:00.000000 joulescope-1.1.3/joulescope/view.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:40.052350 joulescope-1.1.3/joulescope.egg-info/
+-rw-rw-rw-   0        0        0     3628 2023-04-13 20:58:39.000000 joulescope-1.1.3/joulescope.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3265 2023-04-13 20:58:40.000000 joulescope-1.1.3/joulescope.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 20:58:39.000000 joulescope-1.1.3/joulescope.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-04-13 20:58:39.000000 joulescope-1.1.3/joulescope.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      200 2023-04-13 20:58:39.000000 joulescope-1.1.3/joulescope.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-13 20:58:39.000000 joulescope-1.1.3/joulescope.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      851 2022-11-30 15:24:46.000000 joulescope-1.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0      117 2023-04-13 20:58:40.122279 joulescope-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     6882 2023-03-16 19:48:12.000000 joulescope-1.1.3/setup.py
```

### Comparing `joulescope-1.1.2/CHANGELOG.md` & `joulescope-1.1.3/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 
 # CHANGELOG
 
 This file contains the list of changes made to pyjoulescope.
 
 
+## 1.1.3
+
+2023 Apr 13
+
+* Fixed single field output for stream_buffer v1.
+
+
 ## 1.1.2
 
 2023 Mar 20
 
 * Modified JOULESCOPE_BACKEND to skip backend autoimport if 'None' specified.
```

### Comparing `joulescope-1.1.2/CREDITS.html` & `joulescope-1.1.3/CREDITS.html`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/LICENSE.txt` & `joulescope-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/PKG-INFO` & `joulescope-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joulescope
-Version: 1.1.2
+Version: 1.1.3
 Summary: Joulescope™ host driver and utilities
 Home-page: https://joulescope.readthedocs.io
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/pyjoulescope/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `joulescope-1.1.2/README.md` & `joulescope-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/__init__.py` & `joulescope-1.1.3/joulescope/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/__main__.py` & `joulescope-1.1.3/joulescope/__main__.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/data_recorder.py` & `joulescope-1.1.3/joulescope/data_recorder.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/datafile.py` & `joulescope-1.1.3/joulescope/datafile.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/entry_points/bootloader_go.py` & `joulescope-1.1.3/joulescope/entry_points/bootloader_go.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/entry_points/capture.py` & `joulescope-1.1.3/joulescope/entry_points/capture.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/entry_points/gpo_demo.py` & `joulescope-1.1.3/joulescope/entry_points/gpo_demo.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/entry_points/info.py` & `joulescope-1.1.3/joulescope/entry_points/info.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/entry_points/parameter_set.py` & `joulescope-1.1.3/joulescope/entry_points/parameter_set.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/entry_points/program.py` & `joulescope-1.1.3/joulescope/entry_points/program.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/entry_points/recording.py` & `joulescope-1.1.3/joulescope/entry_points/recording.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/entry_points/runner.py` & `joulescope-1.1.3/joulescope/entry_points/runner.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/entry_points/scan.py` & `joulescope-1.1.3/joulescope/entry_points/scan.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/entry_points/statistics.py` & `joulescope-1.1.3/joulescope/entry_points/statistics.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/entry_points/stream_test.py` & `joulescope-1.1.3/joulescope/entry_points/stream_test.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/file_replace.py` & `joulescope-1.1.3/joulescope/file_replace.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/jls_v2_writer.py` & `joulescope-1.1.3/joulescope/jls_v2_writer.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/parameter.py` & `joulescope-1.1.3/joulescope/parameter.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/parameters_v1.py` & `joulescope-1.1.3/joulescope/parameters_v1.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/span.py` & `joulescope-1.1.3/joulescope/span.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/stream_buffer.py` & `joulescope-1.1.3/joulescope/stream_buffer.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/test/test_data_recorder.py` & `joulescope-1.1.3/joulescope/test/test_data_recorder.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/test/test_data_recorder_downsampled.py` & `joulescope-1.1.3/joulescope/test/test_data_recorder_downsampled.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/test/test_file_replace.py` & `joulescope-1.1.3/joulescope/test/test_file_replace.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/test/test_jls_v2_writer.py` & `joulescope-1.1.3/joulescope/test/test_jls_v2_writer.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/test/test_span.py` & `joulescope-1.1.3/joulescope/test/test_span.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/test/test_time.py` & `joulescope-1.1.3/joulescope/test/test_time.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/test/test_units.py` & `joulescope-1.1.3/joulescope/test/test_units.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/test_datafile.py` & `joulescope-1.1.3/joulescope/test_datafile.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/time.py` & `joulescope-1.1.3/joulescope/time.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/units.py` & `joulescope-1.1.3/joulescope/units.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/array_storage.py` & `joulescope-1.1.3/joulescope/v0/array_storage.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/bootloader.py` & `joulescope-1.1.3/joulescope/v0/bootloader.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/calibration.py` & `joulescope-1.1.3/joulescope/v0/calibration.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/decimators.py` & `joulescope-1.1.3/joulescope/v0/decimators.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/driver.py` & `joulescope-1.1.3/joulescope/v0/driver.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/filter_fir.c` & `joulescope-1.1.3/joulescope/v0/filter_fir.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "C:\\bin\\Python3_11_2\\Lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
             "C:\\bin\\Python3_11_2\\Lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
@@ -30,16 +30,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -224,15 +224,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -263,15 +263,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -2122,20 +2122,28 @@
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
@@ -19969,52 +19977,67 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -21888,28 +21911,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -22881,44 +22904,62 @@
     return ret;
 }
 
 /* TypeImport */
 #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
```

### Comparing `joulescope-1.1.2/joulescope/v0/firmware_manager.py` & `joulescope-1.1.3/joulescope/v0/firmware_manager.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/native/filter_fir.c` & `joulescope-1.1.3/joulescope/v0/native/filter_fir.c`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/native/filter_fir.h` & `joulescope-1.1.3/joulescope/v0/native/filter_fir.h`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/native/running_statistics.c` & `joulescope-1.1.3/joulescope/v0/native/running_statistics.c`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/native/running_statistics.h` & `joulescope-1.1.3/joulescope/v0/native/running_statistics.h`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/native/test/acutest.h` & `joulescope-1.1.3/joulescope/v0/native/test/acutest.h`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/native/test/test_filter_fir.c` & `joulescope-1.1.3/joulescope/v0/native/test/test_filter_fir.c`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/notification_handler.py` & `joulescope-1.1.3/joulescope/v0/notification_handler.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/pattern_buffer.c` & `joulescope-1.1.3/joulescope/v0/pattern_buffer.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "C:\\bin\\Python3_10_10\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
-            "C:\\bin\\Python3_10_10\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
-            "C:\\bin\\Python3_10_10\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarrayobject.h",
-            "C:\\bin\\Python3_10_10\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarraytypes.h",
-            "C:\\bin\\Python3_10_10\\lib\\site-packages\\numpy\\core\\include\\numpy\\ufuncobject.h"
+            "C:\\bin\\Python3_11_2\\Lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
+            "C:\\bin\\Python3_11_2\\Lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
+            "C:\\bin\\Python3_11_2\\Lib\\site-packages\\numpy\\core\\include\\numpy\\ndarrayobject.h",
+            "C:\\bin\\Python3_11_2\\Lib\\site-packages\\numpy\\core\\include\\numpy\\ndarraytypes.h",
+            "C:\\bin\\Python3_11_2\\Lib\\site-packages\\numpy\\core\\include\\numpy\\ufuncobject.h"
         ],
         "include_dirs": [
-            "C:\\bin\\Python3_10_10\\lib\\site-packages\\numpy\\core\\include"
+            "C:\\bin\\Python3_11_2\\Lib\\site-packages\\numpy\\core\\include"
         ],
         "name": "joulescope.v0.pattern_buffer",
         "sources": [
             "joulescope/v0/pattern_buffer.pyx"
         ]
     },
     "module_name": "joulescope.v0.pattern_buffer"
@@ -27,16 +27,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -221,15 +221,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -260,15 +260,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -1043,195 +1043,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":689
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":690
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":691
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":692
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":696
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":697
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":698
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":699
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":703
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":704
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":713
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":714
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":715
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":717
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":718
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":719
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":721
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":722
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":724
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":725
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":726
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1259,42 +1259,42 @@
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 struct __pyx_obj_10joulescope_2v0_14pattern_buffer_PatternBuffer;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":728
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":729
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":730
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":732
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1694,20 +1694,28 @@
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
@@ -4908,15 +4916,15 @@
   __Pyx_AddTraceback("joulescope.v0.pattern_buffer.PatternBuffer.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":734
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4925,29 +4933,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":735
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":734
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4958,15 +4966,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":737
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4975,29 +4983,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":738
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":737
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5008,15 +5016,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":740
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5025,29 +5033,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":741
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":740
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5058,15 +5066,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":743
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5075,29 +5083,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":744
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":743
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5108,15 +5116,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":746
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5125,29 +5133,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":747
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":746
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5158,212 +5166,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":749
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":750
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":751
+    /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":750
+    /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":753
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":749
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":928
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":929
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":930
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":928
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":932
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":933
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":934
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":935
+    /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":934
+    /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":936
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":932
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":940
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5379,15 +5387,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":941
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -5395,53 +5403,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":942
+      /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 942, __pyx_L3_error)
 
-      /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":941
+      /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":943
+    /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":944
+      /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 944, __pyx_L5_except_error)
@@ -5449,30 +5457,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":941
+    /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":940
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5487,15 +5495,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":946
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5511,15 +5519,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":947
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5527,53 +5535,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":948
+      /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 948, __pyx_L3_error)
 
-      /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":947
+      /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":949
+    /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":950
+      /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 950, __pyx_L5_except_error)
@@ -5581,30 +5589,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":947
+    /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":946
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5619,15 +5627,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":952
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5643,15 +5651,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":953
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5659,53 +5667,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":954
+      /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 954, __pyx_L3_error)
 
-      /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":953
+      /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":955
+    /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":956
+      /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 956, __pyx_L5_except_error)
@@ -5713,30 +5721,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":953
+    /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":952
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5751,176 +5759,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":966
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":978
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":966
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":981
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":993
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":981
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":996
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":1003
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":996
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":1006
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":1010
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":1006
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":1013
+/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":1017
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":1013
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -6269,26 +6277,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":944
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(2, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":950
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(2, 950, __pyx_L1_error)
@@ -6381,52 +6389,67 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -6712,15 +6735,15 @@
  * # Licensed under the Apache License, Version 2.0 (the "License");
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "../../../bin/Python3_10_10/lib/site-packages/numpy/__init__.pxd":1013
+  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -7471,28 +7494,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -8698,44 +8721,62 @@
     return ret;
 }
 
 /* TypeImport */
   #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
```

### Comparing `joulescope-1.1.2/joulescope/v0/public_keys.py` & `joulescope-1.1.3/joulescope/v0/public_keys.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/stream_buffer.c` & `joulescope-1.1.3/joulescope/v0/stream_buffer.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "C:\\bin\\Python3_11_2\\Lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
             "C:\\bin\\Python3_11_2\\Lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
@@ -30,16 +30,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -224,15 +224,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -263,15 +263,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -2691,20 +2691,28 @@
 
 /* SetVTable.proto */
 static int __Pyx_SetVtable(PyObject *dict, void *vtable);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
@@ -53879,57 +53887,73 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(6, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(5, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(5, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(5, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(5, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_generic) __PYX_ERR(5, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_number) __PYX_ERR(5, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_integer) __PYX_ERR(5, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(5, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(5, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(5, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_floating) __PYX_ERR(5, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(5, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(5, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_character) __PYX_ERR(5, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(5, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("joulescope.v0.filter_fir"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10joulescope_2v0_10filter_fir_FilterFir = __Pyx_ImportType(__pyx_t_1, "joulescope.v0.filter_fir", "FilterFir", sizeof(struct __pyx_obj_10joulescope_2v0_10filter_fir_FilterFir), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_10joulescope_2v0_10filter_fir_FilterFir = __Pyx_ImportType(__pyx_t_1, "joulescope.v0.filter_fir", "FilterFir", sizeof(struct __pyx_obj_10joulescope_2v0_10filter_fir_FilterFir), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10joulescope_2v0_10filter_fir_FilterFir),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_10joulescope_2v0_10filter_fir_FilterFir) __PYX_ERR(7, 20, __pyx_L1_error)
   __pyx_vtabptr_10joulescope_2v0_10filter_fir_FilterFir = (struct __pyx_vtabstruct_10joulescope_2v0_10filter_fir_FilterFir*)__Pyx_GetVtable(__pyx_ptype_10joulescope_2v0_10filter_fir_FilterFir->tp_dict); if (unlikely(!__pyx_vtabptr_10joulescope_2v0_10filter_fir_FilterFir)) __PYX_ERR(7, 20, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -55851,28 +55875,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -59965,44 +59989,62 @@
     return -1;
 }
 
 /* TypeImport */
   #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
```

### Comparing `joulescope-1.1.2/joulescope/v0/test/test_array_storage.py` & `joulescope-1.1.3/joulescope/v0/test/test_array_storage.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/test/test_calibration.py` & `joulescope-1.1.3/joulescope/v0/test/test_calibration.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/test/test_device.py` & `joulescope-1.1.3/joulescope/v0/test/test_device.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/test/test_filter_fir.py` & `joulescope-1.1.3/joulescope/v0/test/test_filter_fir.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/test/test_parameter.py` & `joulescope-1.1.3/joulescope/v0/test/test_parameter.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/test/test_pattern_buffer.py` & `joulescope-1.1.3/joulescope/v0/test/test_pattern_buffer.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/test/test_stats.py` & `joulescope-1.1.3/joulescope/v0/test/test_stats.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/test/test_stream_buffer.py` & `joulescope-1.1.3/joulescope/v0/test/test_stream_buffer.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/test/test_view.py` & `joulescope-1.1.3/joulescope/v0/test/test_view.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/usb/__init__.py` & `joulescope-1.1.3/joulescope/v0/usb/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/usb/api.py` & `joulescope-1.1.3/joulescope/v0/usb/api.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/usb/core.py` & `joulescope-1.1.3/joulescope/v0/usb/core.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/usb/device_thread.py` & `joulescope-1.1.3/joulescope/v0/usb/device_thread.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/usb/hw_tests.py` & `joulescope-1.1.3/joulescope/v0/usb/hw_tests.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/usb/impl_tools.py` & `joulescope-1.1.3/joulescope/v0/usb/impl_tools.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/usb/libusb/device.py` & `joulescope-1.1.3/joulescope/v0/usb/libusb/device.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/usb/scan_info.py` & `joulescope-1.1.3/joulescope/v0/usb/scan_info.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/usb/winusb/device.py` & `joulescope-1.1.3/joulescope/v0/usb/winusb/device.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/usb/winusb/kernel32.py` & `joulescope-1.1.3/joulescope/v0/usb/winusb/kernel32.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/usb/winusb/setupapi.py` & `joulescope-1.1.3/joulescope/v0/usb/winusb/setupapi.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v0/usb/winusb/win32_device_notify.py` & `joulescope-1.1.3/joulescope/v0/usb/winusb/win32_device_notify.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v1/__init__.py` & `joulescope-1.1.3/joulescope/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v1/device.py` & `joulescope-1.1.3/joulescope/v1/device.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v1/driver.py` & `joulescope-1.1.3/joulescope/v1/driver.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v1/js110.py` & `joulescope-1.1.3/joulescope/v1/js110.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v1/js220.py` & `joulescope-1.1.3/joulescope/v1/js220.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v1/sample_buffer.py` & `joulescope-1.1.3/joulescope/v1/sample_buffer.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/v1/stats.c` & `joulescope-1.1.3/joulescope/v1/stats.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "C:\\bin\\Python3_11_2\\Lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
             "C:\\bin\\Python3_11_2\\Lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
@@ -27,16 +27,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -221,15 +221,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -260,15 +260,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -2029,20 +2029,28 @@
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
@@ -19076,52 +19084,67 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -20332,28 +20355,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -21491,44 +21514,62 @@
     return ret;
 }
 
 /* TypeImport */
 #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
```

### Comparing `joulescope-1.1.2/joulescope/v1/stream_buffer.py` & `joulescope-1.1.3/joulescope/v1/stream_buffer.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,16 +350,21 @@
             The 'time' value is a dict contain the timing metadata for
             these samples.  The 'signals' value is a dict with one
             key for each field in fields.  Each field value is also
             a dict with entries 'value' and 'units'.
             However, if single field string is provided to fields, then just
             return that field's value.
         """
+        is_single_result = False
         if fields is None:
             fields = ['current', 'voltage', 'power', 'current_range', 'current_lsb', 'voltage_lsb']
+        elif isinstance(fields, str):
+            fields = [fields]
+            is_single_result = True
+
         self_start, self_stop = self.sample_id_range
         #self._log.debug(f'samples_get({start}, {stop}) in ({self_start}, {self_stop})')
         start = max(start, self_start)
         stop = min(stop, self_stop)
         t1 = self.sample_id_to_time(start)
         t2 = self.sample_id_to_time(stop)
         result = {
@@ -383,8 +388,10 @@
                     result['signals'][field] = {'value': out, 'units': units}
                 else:
                     d = np.empty(stop - start, dtype=np.float32)
                     d[:] = np.nan
                     result['signals'][field] = {'value': out, 'units': units}
             except KeyError:
                 pass  # cannot include this signal
+        if is_single_result:
+            return result['signals'][fields[0]]['value']
         return result
```

### Comparing `joulescope-1.1.2/joulescope/v1/test/test_sample_buffer.py` & `joulescope-1.1.3/joulescope/v1/test/test_sample_buffer.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope/view.py` & `joulescope-1.1.3/joulescope/view.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/joulescope.egg-info/PKG-INFO` & `joulescope-1.1.3/joulescope.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joulescope
-Version: 1.1.2
+Version: 1.1.3
 Summary: Joulescope™ host driver and utilities
 Home-page: https://joulescope.readthedocs.io
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/pyjoulescope/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `joulescope-1.1.2/joulescope.egg-info/SOURCES.txt` & `joulescope-1.1.3/joulescope.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/pyproject.toml` & `joulescope-1.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.2/setup.py` & `joulescope-1.1.3/setup.py`

 * *Files identical despite different names*

