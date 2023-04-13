# Comparing `tmp/joulescope_ui-1.0.7.tar.gz` & `tmp/joulescope_ui-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joulescope_ui-1.0.7.tar", last modified: Tue Apr  4 18:06:32 2023, max compression
+gzip compressed data, was "joulescope_ui-1.0.8.tar", last modified: Thu Apr 13 20:58:46 2023, max compression
```

## Comparing `joulescope_ui-1.0.7.tar` & `joulescope_ui-1.0.8.tar`

### file list

```diff
@@ -1,272 +1,282 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.835945 joulescope_ui-1.0.7/
--rw-rw-rw-   0        0        0    36310 2023-04-04 17:47:06.000000 joulescope_ui-1.0.7/CHANGELOG.md
--rw-rw-rw-   0        0        0    13225 2023-04-04 17:19:13.000000 joulescope_ui-1.0.7/CREDITS.html
--rw-rw-rw-   0        0        0    11558 2018-07-03 17:53:12.000000 joulescope_ui-1.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0      160 2023-03-10 02:18:44.000000 joulescope_ui-1.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     6885 2023-04-04 18:06:32.835945 joulescope_ui-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     5309 2023-03-10 14:30:22.000000 joulescope_ui-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.744818 joulescope_ui-1.0.7/joulescope_ui/
--rw-rw-rw-   0        0        0     2976 2023-03-29 15:40:51.000000 joulescope_ui-1.0.7/joulescope_ui/__init__.py
--rw-rw-rw-   0        0        0      902 2023-03-09 20:16:57.000000 joulescope_ui-1.0.7/joulescope_ui/__main__.py
--rw-rw-rw-   0        0        0     1886 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/about.py
--rw-rw-rw-   0        0        0     3935 2023-03-12 15:18:01.000000 joulescope_ui-1.0.7/joulescope_ui/api.py
--rw-rw-rw-   0        0        0     6921 2023-03-09 20:21:39.000000 joulescope_ui-1.0.7/joulescope_ui/app.py
--rw-rw-rw-   0        0        0     7516 2023-03-20 12:38:29.000000 joulescope_ui-1.0.7/joulescope_ui/capabilities.py
--rw-rw-rw-   0        0        0     6226 2023-03-29 15:41:11.000000 joulescope_ui-1.0.7/joulescope_ui/dev_signal_buffer_source.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.757341 joulescope_ui-1.0.7/joulescope_ui/devices/
--rw-rw-rw-   0        0        0        0 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/devices/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.760341 joulescope_ui-1.0.7/joulescope_ui/devices/jsdrv/
--rw-rw-rw-   0        0        0        0 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/devices/jsdrv/__init__.py
--rw-rw-rw-   0        0        0     3917 2023-03-19 13:46:25.000000 joulescope_ui-1.0.7/joulescope_ui/devices/jsdrv/device.py
--rw-rw-rw-   0        0        0    24218 2023-03-17 12:19:24.000000 joulescope_ui-1.0.7/joulescope_ui/devices/jsdrv/js110.py
--rw-rw-rw-   0        0        0    24425 2023-03-19 15:12:33.000000 joulescope_ui-1.0.7/joulescope_ui/devices/jsdrv/js220.py
--rw-rw-rw-   0        0        0    14136 2023-03-17 12:38:08.000000 joulescope_ui-1.0.7/joulescope_ui/devices/jsdrv/jsdrv_stream_buffer.py
--rw-rw-rw-   0        0        0     7170 2023-03-17 12:14:59.000000 joulescope_ui-1.0.7/joulescope_ui/devices/jsdrv/jsdrv_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.761341 joulescope_ui-1.0.7/joulescope_ui/entry_points/
--rw-rw-rw-   0        0        0        0 2020-04-07 21:08:41.000000 joulescope_ui-1.0.7/joulescope_ui/entry_points/__init__.py
--rw-rw-rw-   0        0        0     2318 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/entry_points/ui.py
--rw-rw-rw-   0        0        0     3168 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/error_window.py
--rw-rw-rw-   0        0        0     4917 2023-03-15 21:06:26.000000 joulescope_ui-1.0.7/joulescope_ui/expanding_widget.py
--rw-rw-rw-   0        0        0    11849 2023-03-31 21:30:44.000000 joulescope_ui-1.0.7/joulescope_ui/exporter.py
--rw-rw-rw-   0        0        0     3179 2023-01-24 22:12:47.000000 joulescope_ui-1.0.7/joulescope_ui/file_dialog.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.712224 joulescope_ui-1.0.7/joulescope_ui/fonts/
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.761841 joulescope_ui-1.0.7/joulescope_ui/fonts/DSEG14-Modern/
--rw-rw-rw-   0        0        0     4487 2020-03-14 16:24:02.000000 joulescope_ui-1.0.7/joulescope_ui/fonts/DSEG14-Modern/DSEG-LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.762340 joulescope_ui-1.0.7/joulescope_ui/fonts/Hack/
--rw-rw-rw-   0        0        0     3744 2023-04-04 17:09:37.000000 joulescope_ui-1.0.7/joulescope_ui/fonts/Hack/LICENSE.md
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.762840 joulescope_ui-1.0.7/joulescope_ui/fonts/Lato/
--rw-rw-rw-   0        0        0     4500 2010-12-15 04:00:00.000000 joulescope_ui-1.0.7/joulescope_ui/fonts/Lato/OFL.txt
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.763341 joulescope_ui-1.0.7/joulescope_ui/fonts/SourceCodePro/
--rw-rw-rw-   0        0        0     4566 2023-04-04 17:17:39.000000 joulescope_ui-1.0.7/joulescope_ui/fonts/SourceCodePro/LICENSE.md
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.763841 joulescope_ui-1.0.7/joulescope_ui/fonts/SourceSerifPro/
--rw-rw-rw-   0        0        0     4615 2014-05-30 04:00:00.000000 joulescope_ui-1.0.7/joulescope_ui/fonts/SourceSerifPro/OFL.txt
--rw-rw-rw-   0        0        0  3411435 2023-04-04 18:06:32.000000 joulescope_ui-1.0.7/joulescope_ui/fonts.rcc
--rw-rw-rw-   0        0        0     2642 2023-01-24 22:12:47.000000 joulescope_ui-1.0.7/joulescope_ui/getting_started.html
--rw-rw-rw-   0        0        0     4994 2023-03-18 21:45:09.000000 joulescope_ui-1.0.7/joulescope_ui/help_ui.py
--rw-rw-rw-   0        0        0     6488 2023-03-18 13:34:03.000000 joulescope_ui-1.0.7/joulescope_ui/jls_source.py
--rw-rw-rw-   0        0        0     9069 2023-03-29 15:41:27.000000 joulescope_ui-1.0.7/joulescope_ui/jls_v1.py
--rw-rw-rw-   0        0        0     8262 2023-03-29 22:24:39.000000 joulescope_ui-1.0.7/joulescope_ui/jls_v2.py
--rw-rw-rw-   0        0        0     3109 2023-03-20 14:51:40.000000 joulescope_ui-1.0.7/joulescope_ui/json.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.764341 joulescope_ui-1.0.7/joulescope_ui/locale/
--rw-rw-rw-   0        0        0      965 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/locale/__init__.py
--rw-rw-rw-   0        0        0     5629 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/logging_util.py
--rw-rw-rw-   0        0        0    24876 2023-04-04 17:32:11.000000 joulescope_ui-1.0.7/joulescope_ui/main.py
--rw-rw-rw-   0        0        0     2171 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/mem_leak_debugger.py
--rw-rw-rw-   0        0        0     9118 2023-03-18 18:14:25.000000 joulescope_ui-1.0.7/joulescope_ui/metadata.py
--rw-rw-rw-   0        0        0     5812 2023-03-18 14:11:03.000000 joulescope_ui-1.0.7/joulescope_ui/paths.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.766855 joulescope_ui-1.0.7/joulescope_ui/plugins/
--rw-rw-rw-   0        0        0      792 2023-03-20 13:23:46.000000 joulescope_ui-1.0.7/joulescope_ui/plugins/__init__.py
--rw-rw-rw-   0        0        0     8664 2023-03-20 14:22:30.000000 joulescope_ui-1.0.7/joulescope_ui/plugins/cdf.py
--rw-rw-rw-   0        0        0    10908 2023-03-20 13:34:44.000000 joulescope_ui-1.0.7/joulescope_ui/plugins/frequency.py
--rw-rw-rw-   0        0        0     9176 2023-03-20 13:34:59.000000 joulescope_ui-1.0.7/joulescope_ui/plugins/histogram.py
--rw-rw-rw-   0        0        0     6270 2023-03-29 15:41:27.000000 joulescope_ui-1.0.7/joulescope_ui/plugins/max_window.py
--rw-rw-rw-   0        0        0     2219 2023-03-20 13:10:43.000000 joulescope_ui-1.0.7/joulescope_ui/plugins/plugin_helpers.py
--rw-rw-rw-   0        0        0     4247 2023-03-13 18:49:46.000000 joulescope_ui-1.0.7/joulescope_ui/plugins/usb_inrush.py
--rw-rw-rw-   0        0        0     2130 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/process_monitor.py
--rw-rw-rw-   0        0        0     1008 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/profile.py
--rw-rw-rw-   0        0        0    63807 2023-03-31 19:42:47.000000 joulescope_ui-1.0.7/joulescope_ui/pubsub.py
--rw-rw-rw-   0        0        0    12868 2023-03-19 18:14:07.000000 joulescope_ui-1.0.7/joulescope_ui/range_tool.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.768355 joulescope_ui-1.0.7/joulescope_ui/resources/
--rw-rw-rw-   0        0        0    11509 2019-07-27 15:33:28.000000 joulescope_ui-1.0.7/joulescope_ui/resources/dmg_background.svg
--rw-rw-rw-   0        0        0     3357 2020-11-05 22:48:01.000000 joulescope_ui-1.0.7/joulescope_ui/resources/icons.svg
--rw-rw-rw-   0        0        0    11282 2020-08-12 18:43:24.000000 joulescope_ui-1.0.7/joulescope_ui/resources/zoom.svg
--rw-rw-rw-   0        0        0     1989 2023-04-04 16:57:10.000000 joulescope_ui-1.0.7/joulescope_ui/resources.py
--rw-rw-rw-   0        0        0    22839 2023-04-04 18:06:32.000000 joulescope_ui-1.0.7/joulescope_ui/resources.rcc
--rw-rw-rw-   0        0        0     1840 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/sanitize.py
--rw-rw-rw-   0        0        0    10890 2023-03-20 18:55:58.000000 joulescope_ui-1.0.7/joulescope_ui/software_update.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.773854 joulescope_ui-1.0.7/joulescope_ui/styles/
--rw-rw-rw-   0        0        0     3239 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/README.md
--rw-rw-rw-   0        0        0      834 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/__init__.py
--rw-rw-rw-   0        0        0     4354 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/color_editor.py
--rw-rw-rw-   0        0        0     4369 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/color_file.py
--rw-rw-rw-   0        0        0     6822 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/color_picker.py
--rw-rw-rw-   0        0        0      944 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/color_scheme.py
--rw-rw-rw-   0        0        0     1383 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/color_scheme_dark.txt
--rw-rw-rw-   0        0        0     2346 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/color_scheme_light.txt
--rw-rw-rw-   0        0        0      778 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/font_scheme.py
--rw-rw-rw-   0        0        0       30 2023-03-31 19:50:28.000000 joulescope_ui-1.0.7/joulescope_ui/styles/font_scheme_js1.txt
--rw-rw-rw-   0        0        0     3405 2023-04-04 16:50:03.000000 joulescope_ui-1.0.7/joulescope_ui/styles/fonts.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.785369 joulescope_ui-1.0.7/joulescope_ui/styles/js1/
--rw-rw-rw-   0        0        0      179 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/js1/arrow_down.svg
--rw-rw-rw-   0        0        0      179 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/js1/arrow_left.svg
--rw-rw-rw-   0        0        0      179 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/js1/arrow_right.svg
--rw-rw-rw-   0        0        0      179 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/js1/arrow_up.svg
--rw-rw-rw-   0        0        0       86 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/js1/branch_closed.svg
--rw-rw-rw-   0        0        0      177 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/js1/branch_end.svg
--rw-rw-rw-   0        0        0      177 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/js1/branch_end_open.svg
--rw-rw-rw-   0        0        0      177 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/js1/branch_more.svg
--rw-rw-rw-   0        0        0       86 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/js1/branch_open.svg
--rw-rw-rw-   0        0        0       93 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/js1/branch_vline.svg
--rw-rw-rw-   0        0        0      335 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/js1/checkbox_checked.svg
--rw-rw-rw-   0        0        0      499 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/js1/checkbox_indeterminate.svg
--rw-rw-rw-   0        0        0      264 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/js1/checkbox_unchecked.svg
--rw-rw-rw-   0        0        0      234 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/js1/close.svg
--rw-rw-rw-   0        0        0     1907 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/js1/detach.svg
--rw-rw-rw-   0        0        0      259 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/js1/hmovetoolbar.svg
--rw-rw-rw-   0        0        0      191 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/js1/hsepartoolbar.svg
--rw-rw-rw-   0        0        0     2382 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/js1/index.json
--rw-rw-rw-   0        0        0      432 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/js1/radio_checked.svg
--rw-rw-rw-   0        0        0      345 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/js1/radio_unchecked.svg
--rw-rw-rw-   0        0        0      263 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/js1/sizegrip.svg
--rw-rw-rw-   0        0        0      419 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/js1/style.html
--rw-rw-rw-   0        0        0    19524 2023-04-04 14:57:41.000000 joulescope_ui-1.0.7/joulescope_ui/styles/js1/style.qss
--rw-rw-rw-   0        0        0      526 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/js1/tabs_menu.svg
--rw-rw-rw-   0        0        0       31 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/js1/transparent.svg
--rw-rw-rw-   0        0        0      760 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/js1/vmovetoolbar.svg
--rw-rw-rw-   0        0        0      653 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/js1/vsepartoolbars.svg
--rw-rw-rw-   0        0        0    15079 2023-03-18 21:39:13.000000 joulescope_ui-1.0.7/joulescope_ui/styles/manager.py
--rw-rw-rw-   0        0        0     3635 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/parameter_file.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.787877 joulescope_ui-1.0.7/joulescope_ui/styles/system/
--rw-rw-rw-   0        0        0      350 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/system/index.json
--rw-rw-rw-   0        0        0       17 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/system/style.html
--rw-rw-rw-   0        0        0     3222 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/system/style.qss
--rw-rw-rw-   0        0        0      558 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/system/zoom_all.svg
--rw-rw-rw-   0        0        0      481 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/system/zoom_in.svg
--rw-rw-rw-   0        0        0      393 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/system/zoom_out.svg
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.789377 joulescope_ui-1.0.7/joulescope_ui/styles/test/
--rw-rw-rw-   0        0        0        0 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/test/__init__.py
--rw-rw-rw-   0        0        0     2816 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/test/test_color_file.py
--rw-rw-rw-   0        0        0     2156 2023-03-18 18:42:17.000000 joulescope_ui-1.0.7/joulescope_ui/styles/test/test_manager.py
--rw-rw-rw-   0        0        0     1959 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/styles/test/test_parameter_file.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.794377 joulescope_ui-1.0.7/joulescope_ui/test/
--rw-rw-rw-   0        0        0        0 2018-04-10 21:33:42.000000 joulescope_ui-1.0.7/joulescope_ui/test/__init__.py
--rw-rw-rw-   0        0        0     1139 2023-03-10 14:49:52.000000 joulescope_ui-1.0.7/joulescope_ui/test/test_capabilities.py
--rw-rw-rw-   0        0        0     6853 2023-03-10 14:56:31.000000 joulescope_ui-1.0.7/joulescope_ui/test/test_metadata.py
--rw-rw-rw-   0        0        0    10324 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/test/test_pubsub.py
--rw-rw-rw-   0        0        0    12814 2023-03-12 15:57:42.000000 joulescope_ui-1.0.7/joulescope_ui/test/test_pubsub_registry.py
--rw-rw-rw-   0        0        0     5147 2023-03-16 16:02:02.000000 joulescope_ui-1.0.7/joulescope_ui/test/test_range_tool.py
--rw-rw-rw-   0        0        0     2582 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/test/test_sanitize.py
--rw-rw-rw-   0        0        0     2034 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/test/test_software_update.py
--rw-rw-rw-   0        0        0     4055 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/test/test_time_map.py
--rw-rw-rw-   0        0        0     1601 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/test/test_tooltip.py
--rw-rw-rw-   0        0        0     5008 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/test/test_units.py
--rw-rw-rw-   0        0        0     3197 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/time_map.py
--rw-rw-rw-   0        0        0     2234 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/tooltip.py
--rw-rw-rw-   0        0        0     7060 2023-01-24 22:12:47.000000 joulescope_ui-1.0.7/joulescope_ui/ui_util.py
--rw-rw-rw-   0        0        0     5873 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/units.py
--rw-rw-rw-   0        0        0       23 2023-03-31 18:37:16.000000 joulescope_ui-1.0.7/joulescope_ui/version.py
--rw-rw-rw-   0        0        0    12735 2023-03-29 15:51:51.000000 joulescope_ui-1.0.7/joulescope_ui/view.py
--rw-rw-rw-   0        0        0     1042 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widget_tools.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.795377 joulescope_ui-1.0.7/joulescope_ui/widgets/
--rw-rw-rw-   0        0        0     1116 2023-03-10 13:54:56.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.796880 joulescope_ui-1.0.7/joulescope_ui/widgets/device_control/
--rw-rw-rw-   0        0        0      647 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/device_control/__init__.py
--rw-rw-rw-   0        0        0     3177 2023-03-15 21:07:03.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/device_control/device_control_widget.py
--rw-rw-rw-   0        0        0     3397 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/device_control/device_info_dialog.py
--rw-rw-rw-   0        0        0    20308 2023-03-16 12:50:43.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/device_control/js220_ctrl_widget.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.801917 joulescope_ui-1.0.7/joulescope_ui/widgets/device_control/styles/
--rw-rw-rw-   0        0        0      180 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/device_control/styles/active_checked.svg
--rw-rw-rw-   0        0        0      129 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/device_control/styles/active_unchecked.svg
--rw-rw-rw-   0        0        0      129 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/device_control/styles/closed.svg
--rw-rw-rw-   0        0        0       78 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/device_control/styles/color_scheme_dark.txt
--rw-rw-rw-   0        0        0      216 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/device_control/styles/color_scheme_light.txt
--rw-rw-rw-   0        0        0      240 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/device_control/styles/doc.svg
--rw-rw-rw-   0        0        0     1936 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/device_control/styles/index.json
--rw-rw-rw-   0        0        0     1749 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/device_control/styles/info.svg
--rw-rw-rw-   0        0        0      125 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/device_control/styles/open.svg
--rw-rw-rw-   0        0        0     4466 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/device_control/styles/style.qss
--rw-rw-rw-   0        0        0      240 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/device_control/styles/target_power.svg
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.802916 joulescope_ui-1.0.7/joulescope_ui/widgets/example/
--rw-rw-rw-   0        0        0      639 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/example/__init__.py
--rw-rw-rw-   0        0        0     2100 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/example/example_widget.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.804916 joulescope_ui-1.0.7/joulescope_ui/widgets/example/styles/
--rw-rw-rw-   0        0        0      100 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/example/styles/color_scheme_dark.txt
--rw-rw-rw-   0        0        0      100 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/example/styles/color_scheme_light.txt
--rw-rw-rw-   0        0        0       80 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/example/styles/font_scheme_js1.txt
--rw-rw-rw-   0        0        0      122 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/example/styles/index.json
--rw-rw-rw-   0        0        0      242 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/example/styles/style.qss
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.805416 joulescope_ui-1.0.7/joulescope_ui/widgets/flyout/
--rw-rw-rw-   0        0        0      630 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/flyout/__init__.py
--rw-rw-rw-   0        0        0     4010 2023-03-17 14:48:42.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/flyout/flyout_widget.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.807420 joulescope_ui-1.0.7/joulescope_ui/widgets/flyout/styles/
--rw-rw-rw-   0        0        0        0 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/flyout/styles/color_scheme_dark.txt
--rw-rw-rw-   0        0        0        0 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/flyout/styles/color_scheme_light.txt
--rw-rw-rw-   0        0        0      130 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/flyout/styles/index.json
--rw-rw-rw-   0        0        0      692 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/flyout/styles/style.qss
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.808424 joulescope_ui-1.0.7/joulescope_ui/widgets/hamburger/
--rw-rw-rw-   0        0        0      638 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/hamburger/__init__.py
--rw-rw-rw-   0        0        0     2164 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/hamburger/hamburger_widget.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.809424 joulescope_ui-1.0.7/joulescope_ui/widgets/help/
--rw-rw-rw-   0        0        0      628 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/help/__init__.py
--rw-rw-rw-   0        0        0     2350 2023-03-10 14:01:14.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/help/help_widget.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.809925 joulescope_ui-1.0.7/joulescope_ui/widgets/memory/
--rw-rw-rw-   0        0        0      632 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/memory/__init__.py
--rw-rw-rw-   0        0        0    10028 2023-03-18 20:18:20.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/memory/memory_widget.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.811929 joulescope_ui-1.0.7/joulescope_ui/widgets/memory/styles/
--rw-rw-rw-   0        0        0      105 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/memory/styles/color_scheme_dark.txt
--rw-rw-rw-   0        0        0      105 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/memory/styles/color_scheme_light.txt
--rw-rw-rw-   0        0        0      122 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/memory/styles/index.json
--rw-rw-rw-   0        0        0        0 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/memory/styles/style.qss
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.812929 joulescope_ui-1.0.7/joulescope_ui/widgets/progress_bar/
--rw-rw-rw-   0        0        0      643 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/progress_bar/__init__.py
--rw-rw-rw-   0        0        0     5816 2023-03-12 16:20:31.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/progress_bar/progress_bar_widget.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.813929 joulescope_ui-1.0.7/joulescope_ui/widgets/settings/
--rw-rw-rw-   0        0        0      641 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/settings/__init__.py
--rw-rw-rw-   0        0        0    18786 2023-03-31 20:53:10.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/settings/settings_widget.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.814928 joulescope_ui-1.0.7/joulescope_ui/widgets/sidebar/
--rw-rw-rw-   0        0        0      633 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/sidebar/__init__.py
--rw-rw-rw-   0        0        0     9518 2023-03-18 20:20:00.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/sidebar/sidebar_widget.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.821436 joulescope_ui-1.0.7/joulescope_ui/widgets/sidebar/styles/
--rw-rw-rw-   0        0        0      575 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/sidebar/styles/color_scheme_dark.txt
--rw-rw-rw-   0        0        0      216 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/sidebar/styles/color_scheme_light.txt
--rw-rw-rw-   0        0        0      358 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/sidebar/styles/device.svg
--rw-rw-rw-   0        0        0      345 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/sidebar/styles/help.svg
--rw-rw-rw-   0        0        0     4416 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/sidebar/styles/index.json
--rw-rw-rw-   0        0        0      421 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/sidebar/styles/memory.svg
--rw-rw-rw-   0        0        0      309 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/sidebar/styles/pause.svg
--rw-rw-rw-   0        0        0      241 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/sidebar/styles/play.svg
--rw-rw-rw-   0        0        0      205 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/sidebar/styles/record.svg
--rw-rw-rw-   0        0        0      274 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/sidebar/styles/settings.svg
--rw-rw-rw-   0        0        0      309 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/sidebar/styles/stop.svg
--rw-rw-rw-   0        0        0     5290 2023-03-15 21:49:27.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/sidebar/styles/style.qss
--rw-rw-rw-   0        0        0      207 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/sidebar/styles/target_power.svg
--rw-rw-rw-   0        0        0      511 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/sidebar/styles/widgets.svg
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.822436 joulescope_ui-1.0.7/joulescope_ui/widgets/signal_record/
--rw-rw-rw-   0        0        0      699 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/signal_record/__init__.py
--rw-rw-rw-   0        0        0     6727 2023-03-29 19:41:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/signal_record/signal_record.py
--rw-rw-rw-   0        0        0     7983 2023-03-18 13:24:49.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/signal_record/signal_record_config_widget.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.823936 joulescope_ui-1.0.7/joulescope_ui/widgets/statistics_record/
--rw-rw-rw-   0        0        0      715 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/statistics_record/__init__.py
--rw-rw-rw-   0        0        0     3942 2023-03-18 13:36:54.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/statistics_record/statistics_record.py
--rw-rw-rw-   0        0        0     6501 2023-03-18 13:25:13.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/statistics_record/statistics_record_config_widget.py
--rw-rw-rw-   0        0        0     6078 2023-01-24 22:12:47.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/switch.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.824936 joulescope_ui-1.0.7/joulescope_ui/widgets/value/
--rw-rw-rw-   0        0        0      630 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/value/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.826936 joulescope_ui-1.0.7/joulescope_ui/widgets/value/styles/
--rw-rw-rw-   0        0        0      152 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/value/styles/color_scheme_dark.txt
--rw-rw-rw-   0        0        0      100 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/value/styles/color_scheme_light.txt
--rw-rw-rw-   0        0        0      106 2023-04-04 15:40:17.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/value/styles/font_scheme_js1.txt
--rw-rw-rw-   0        0        0      122 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/value/styles/index.json
--rw-rw-rw-   0        0        0        0 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/value/styles/style.qss
--rw-rw-rw-   0        0        0    26745 2023-03-20 16:06:00.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/value/value_widget.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.828944 joulescope_ui-1.0.7/joulescope_ui/widgets/waveform/
--rw-rw-rw-   0        0        0      636 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/waveform/__init__.py
--rw-rw-rw-   0        0        0     8426 2023-03-30 13:55:55.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/waveform/line_segments.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.834944 joulescope_ui-1.0.7/joulescope_ui/widgets/waveform/styles/
--rw-rw-rw-   0        0        0      841 2023-03-17 14:15:26.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/waveform/styles/color_scheme_dark.txt
--rw-rw-rw-   0        0        0        0 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/waveform/styles/color_scheme_light.txt
--rw-rw-rw-   0        0        0       34 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/waveform/styles/font_scheme_js1.txt
--rw-rw-rw-   0        0        0      754 2023-03-18 15:01:04.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/waveform/styles/index.json
--rw-rw-rw-   0        0        0      121 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/waveform/styles/marker_add1.svg
--rw-rw-rw-   0        0        0      198 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/waveform/styles/marker_add2.svg
--rw-rw-rw-   0        0        0      228 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/waveform/styles/marker_clear.svg
--rw-rw-rw-   0        0        0      237 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/waveform/styles/pin_left.svg
--rw-rw-rw-   0        0        0      237 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/waveform/styles/pin_right.svg
--rw-rw-rw-   0        0        0     3520 2023-03-18 15:02:05.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/waveform/styles/style.qss
--rw-rw-rw-   0        0        0      597 2023-03-18 15:06:21.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/waveform/styles/y_zoom_all.svg
--rw-rw-rw-   0        0        0      558 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/waveform/styles/zoom_all.svg
--rw-rw-rw-   0        0        0      471 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/waveform/styles/zoom_in.svg
--rw-rw-rw-   0        0        0      388 2023-03-09 18:33:57.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/waveform/styles/zoom_out.svg
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.835445 joulescope_ui-1.0.7/joulescope_ui/widgets/waveform/test/
--rw-rw-rw-   0        0        0        0 2023-03-08 16:08:46.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/waveform/test/__init__.py
--rw-rw-rw-   0        0        0    13485 2023-03-18 15:03:45.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/waveform/waveform_control.py
--rw-rw-rw-   0        0        0   120519 2023-04-04 14:04:09.000000 joulescope_ui-1.0.7/joulescope_ui/widgets/waveform/waveform_widget.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:32.756842 joulescope_ui-1.0.7/joulescope_ui.egg-info/
--rw-rw-rw-   0        0        0     6885 2023-04-04 18:06:32.000000 joulescope_ui-1.0.7/joulescope_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9424 2023-04-04 18:06:32.000000 joulescope_ui-1.0.7/joulescope_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 18:06:32.000000 joulescope_ui-1.0.7/joulescope_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-04-04 18:06:32.000000 joulescope_ui-1.0.7/joulescope_ui.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      363 2023-04-04 18:06:32.000000 joulescope_ui-1.0.7/joulescope_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-04 18:06:32.000000 joulescope_ui-1.0.7/joulescope_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      117 2023-04-04 18:06:32.836945 joulescope_ui-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     8932 2023-04-04 13:54:40.000000 joulescope_ui-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.384179 joulescope_ui-1.0.8/
+-rw-rw-rw-   0        0        0    37019 2023-04-13 20:54:02.000000 joulescope_ui-1.0.8/CHANGELOG.md
+-rw-rw-rw-   0        0        0    13225 2023-04-04 17:19:13.000000 joulescope_ui-1.0.8/CREDITS.html
+-rw-rw-rw-   0        0        0    11558 2018-07-03 17:53:12.000000 joulescope_ui-1.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      160 2023-03-10 02:18:44.000000 joulescope_ui-1.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     6885 2023-04-13 20:58:46.384179 joulescope_ui-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     5309 2023-03-10 14:30:22.000000 joulescope_ui-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.157685 joulescope_ui-1.0.8/joulescope_ui/
+-rw-rw-rw-   0        0        0     2976 2023-03-29 15:40:51.000000 joulescope_ui-1.0.8/joulescope_ui/__init__.py
+-rw-rw-rw-   0        0        0      902 2023-03-09 20:16:57.000000 joulescope_ui-1.0.8/joulescope_ui/__main__.py
+-rw-rw-rw-   0        0        0     1886 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/about.py
+-rw-rw-rw-   0        0        0     3935 2023-03-12 15:18:01.000000 joulescope_ui-1.0.8/joulescope_ui/api.py
+-rw-rw-rw-   0        0        0     7197 2023-04-12 21:24:46.000000 joulescope_ui-1.0.8/joulescope_ui/app.py
+-rw-rw-rw-   0        0        0     7516 2023-03-20 12:38:29.000000 joulescope_ui-1.0.8/joulescope_ui/capabilities.py
+-rw-rw-rw-   0        0        0     6226 2023-03-29 15:41:11.000000 joulescope_ui-1.0.8/joulescope_ui/dev_signal_buffer_source.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.169204 joulescope_ui-1.0.8/joulescope_ui/devices/
+-rw-rw-rw-   0        0        0        0 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/devices/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.171204 joulescope_ui-1.0.8/joulescope_ui/devices/jsdrv/
+-rw-rw-rw-   0        0        0        0 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/devices/jsdrv/__init__.py
+-rw-rw-rw-   0        0        0     3917 2023-03-19 13:46:25.000000 joulescope_ui-1.0.8/joulescope_ui/devices/jsdrv/device.py
+-rw-rw-rw-   0        0        0    24570 2023-04-13 14:57:50.000000 joulescope_ui-1.0.8/joulescope_ui/devices/jsdrv/js110.py
+-rw-rw-rw-   0        0        0    28183 2023-04-13 14:57:31.000000 joulescope_ui-1.0.8/joulescope_ui/devices/jsdrv/js220.py
+-rw-rw-rw-   0        0        0    14980 2023-04-12 18:27:36.000000 joulescope_ui-1.0.8/joulescope_ui/devices/jsdrv/jsdrv_stream_buffer.py
+-rw-rw-rw-   0        0        0     7170 2023-03-17 12:14:59.000000 joulescope_ui-1.0.8/joulescope_ui/devices/jsdrv/jsdrv_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.177219 joulescope_ui-1.0.8/joulescope_ui/entry_points/
+-rw-rw-rw-   0        0        0        0 2020-04-07 21:08:41.000000 joulescope_ui-1.0.8/joulescope_ui/entry_points/__init__.py
+-rw-rw-rw-   0        0        0     2318 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/entry_points/ui.py
+-rw-rw-rw-   0        0        0     3168 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/error_window.py
+-rw-rw-rw-   0        0        0     4917 2023-03-15 21:06:26.000000 joulescope_ui-1.0.8/joulescope_ui/expanding_widget.py
+-rw-rw-rw-   0        0        0    11849 2023-03-31 21:30:44.000000 joulescope_ui-1.0.8/joulescope_ui/exporter.py
+-rw-rw-rw-   0        0        0     3179 2023-01-24 22:12:47.000000 joulescope_ui-1.0.8/joulescope_ui/file_dialog.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.088346 joulescope_ui-1.0.8/joulescope_ui/fonts/
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.181226 joulescope_ui-1.0.8/joulescope_ui/fonts/DSEG14-Modern/
+-rw-rw-rw-   0        0        0     4487 2020-03-14 16:24:02.000000 joulescope_ui-1.0.8/joulescope_ui/fonts/DSEG14-Modern/DSEG-LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.190247 joulescope_ui-1.0.8/joulescope_ui/fonts/Hack/
+-rw-rw-rw-   0        0        0     3744 2023-04-04 17:09:37.000000 joulescope_ui-1.0.8/joulescope_ui/fonts/Hack/LICENSE.md
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.193250 joulescope_ui-1.0.8/joulescope_ui/fonts/Lato/
+-rw-rw-rw-   0        0        0     4500 2010-12-15 04:00:00.000000 joulescope_ui-1.0.8/joulescope_ui/fonts/Lato/OFL.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.197263 joulescope_ui-1.0.8/joulescope_ui/fonts/SourceCodePro/
+-rw-rw-rw-   0        0        0     4566 2023-04-04 17:17:39.000000 joulescope_ui-1.0.8/joulescope_ui/fonts/SourceCodePro/LICENSE.md
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.201270 joulescope_ui-1.0.8/joulescope_ui/fonts/SourceSerifPro/
+-rw-rw-rw-   0        0        0     4615 2014-05-30 04:00:00.000000 joulescope_ui-1.0.8/joulescope_ui/fonts/SourceSerifPro/OFL.txt
+-rw-rw-rw-   0        0        0  3411435 2023-04-13 20:58:45.000000 joulescope_ui-1.0.8/joulescope_ui/fonts.rcc
+-rw-rw-rw-   0        0        0     2642 2023-01-24 22:12:47.000000 joulescope_ui-1.0.8/joulescope_ui/getting_started.html
+-rw-rw-rw-   0        0        0     4994 2023-03-18 21:45:09.000000 joulescope_ui-1.0.8/joulescope_ui/help_ui.py
+-rw-rw-rw-   0        0        0     6488 2023-03-18 13:34:03.000000 joulescope_ui-1.0.8/joulescope_ui/jls_source.py
+-rw-rw-rw-   0        0        0     9069 2023-03-29 15:41:27.000000 joulescope_ui-1.0.8/joulescope_ui/jls_v1.py
+-rw-rw-rw-   0        0        0     8262 2023-03-29 22:24:39.000000 joulescope_ui-1.0.8/joulescope_ui/jls_v2.py
+-rw-rw-rw-   0        0        0     3109 2023-03-20 14:51:40.000000 joulescope_ui-1.0.8/joulescope_ui/json.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.201769 joulescope_ui-1.0.8/joulescope_ui/locale/
+-rw-rw-rw-   0        0        0      965 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/locale/__init__.py
+-rw-rw-rw-   0        0        0     5629 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/logging_util.py
+-rw-rw-rw-   0        0        0    25310 2023-04-13 20:24:51.000000 joulescope_ui-1.0.8/joulescope_ui/main.py
+-rw-rw-rw-   0        0        0     2171 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/mem_leak_debugger.py
+-rw-rw-rw-   0        0        0     9118 2023-03-18 18:14:25.000000 joulescope_ui-1.0.8/joulescope_ui/metadata.py
+-rw-rw-rw-   0        0        0     5808 2023-04-12 17:49:24.000000 joulescope_ui-1.0.8/joulescope_ui/paths.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.208789 joulescope_ui-1.0.8/joulescope_ui/plugins/
+-rw-rw-rw-   0        0        0      792 2023-03-20 13:23:46.000000 joulescope_ui-1.0.8/joulescope_ui/plugins/__init__.py
+-rw-rw-rw-   0        0        0     8662 2023-04-12 17:48:45.000000 joulescope_ui-1.0.8/joulescope_ui/plugins/cdf.py
+-rw-rw-rw-   0        0        0    10906 2023-04-12 17:49:28.000000 joulescope_ui-1.0.8/joulescope_ui/plugins/frequency.py
+-rw-rw-rw-   0        0        0     9174 2023-04-12 17:49:32.000000 joulescope_ui-1.0.8/joulescope_ui/plugins/histogram.py
+-rw-rw-rw-   0        0        0     6270 2023-03-29 15:41:27.000000 joulescope_ui-1.0.8/joulescope_ui/plugins/max_window.py
+-rw-rw-rw-   0        0        0     2219 2023-03-20 13:10:43.000000 joulescope_ui-1.0.8/joulescope_ui/plugins/plugin_helpers.py
+-rw-rw-rw-   0        0        0     4247 2023-03-13 18:49:46.000000 joulescope_ui-1.0.8/joulescope_ui/plugins/usb_inrush.py
+-rw-rw-rw-   0        0        0     2130 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/process_monitor.py
+-rw-rw-rw-   0        0        0     1008 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/profile.py
+-rw-rw-rw-   0        0        0    63957 2023-04-13 20:12:00.000000 joulescope_ui-1.0.8/joulescope_ui/pubsub.py
+-rw-rw-rw-   0        0        0    12868 2023-03-19 18:14:07.000000 joulescope_ui-1.0.8/joulescope_ui/range_tool.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.211293 joulescope_ui-1.0.8/joulescope_ui/resources/
+-rw-rw-rw-   0        0        0    11509 2019-07-27 15:33:28.000000 joulescope_ui-1.0.8/joulescope_ui/resources/dmg_background.svg
+-rw-rw-rw-   0        0        0     3357 2020-11-05 22:48:01.000000 joulescope_ui-1.0.8/joulescope_ui/resources/icons.svg
+-rw-rw-rw-   0        0        0    11282 2020-08-12 18:43:24.000000 joulescope_ui-1.0.8/joulescope_ui/resources/zoom.svg
+-rw-rw-rw-   0        0        0     1989 2023-04-04 16:57:10.000000 joulescope_ui-1.0.8/joulescope_ui/resources.py
+-rw-rw-rw-   0        0        0    22839 2023-04-13 20:58:45.000000 joulescope_ui-1.0.8/joulescope_ui/resources.rcc
+-rw-rw-rw-   0        0        0     1840 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/sanitize.py
+-rw-rw-rw-   0        0        0     1304 2023-04-13 20:26:58.000000 joulescope_ui-1.0.8/joulescope_ui/shortcuts.py
+-rw-rw-rw-   0        0        0    10890 2023-03-20 18:55:58.000000 joulescope_ui-1.0.8/joulescope_ui/software_update.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.233838 joulescope_ui-1.0.8/joulescope_ui/styles/
+-rw-rw-rw-   0        0        0     3239 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/README.md
+-rw-rw-rw-   0        0        0      834 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/__init__.py
+-rw-rw-rw-   0        0        0     4354 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/color_editor.py
+-rw-rw-rw-   0        0        0     4369 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/color_file.py
+-rw-rw-rw-   0        0        0     6822 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/color_picker.py
+-rw-rw-rw-   0        0        0      944 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/color_scheme.py
+-rw-rw-rw-   0        0        0     1383 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/color_scheme_dark.txt
+-rw-rw-rw-   0        0        0     2346 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/color_scheme_light.txt
+-rw-rw-rw-   0        0        0      778 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/font_scheme.py
+-rw-rw-rw-   0        0        0       30 2023-03-31 19:50:28.000000 joulescope_ui-1.0.8/joulescope_ui/styles/font_scheme_js1.txt
+-rw-rw-rw-   0        0        0     3405 2023-04-04 16:50:03.000000 joulescope_ui-1.0.8/joulescope_ui/styles/fonts.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.250384 joulescope_ui-1.0.8/joulescope_ui/styles/js1/
+-rw-rw-rw-   0        0        0      179 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/arrow_down.svg
+-rw-rw-rw-   0        0        0      179 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/arrow_left.svg
+-rw-rw-rw-   0        0        0      179 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/arrow_right.svg
+-rw-rw-rw-   0        0        0      179 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/arrow_up.svg
+-rw-rw-rw-   0        0        0       86 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/branch_closed.svg
+-rw-rw-rw-   0        0        0      177 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/branch_end.svg
+-rw-rw-rw-   0        0        0      177 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/branch_end_open.svg
+-rw-rw-rw-   0        0        0      177 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/branch_more.svg
+-rw-rw-rw-   0        0        0       86 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/branch_open.svg
+-rw-rw-rw-   0        0        0       93 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/branch_vline.svg
+-rw-rw-rw-   0        0        0      335 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/checkbox_checked.svg
+-rw-rw-rw-   0        0        0      499 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/checkbox_indeterminate.svg
+-rw-rw-rw-   0        0        0      264 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/checkbox_unchecked.svg
+-rw-rw-rw-   0        0        0      234 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/close.svg
+-rw-rw-rw-   0        0        0     1907 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/detach.svg
+-rw-rw-rw-   0        0        0      259 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/hmovetoolbar.svg
+-rw-rw-rw-   0        0        0      191 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/hsepartoolbar.svg
+-rw-rw-rw-   0        0        0     2382 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/index.json
+-rw-rw-rw-   0        0        0      432 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/radio_checked.svg
+-rw-rw-rw-   0        0        0      345 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/radio_unchecked.svg
+-rw-rw-rw-   0        0        0      263 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/sizegrip.svg
+-rw-rw-rw-   0        0        0      419 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/style.html
+-rw-rw-rw-   0        0        0    19524 2023-04-04 14:57:41.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/style.qss
+-rw-rw-rw-   0        0        0      526 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/tabs_menu.svg
+-rw-rw-rw-   0        0        0       31 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/transparent.svg
+-rw-rw-rw-   0        0        0      760 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/vmovetoolbar.svg
+-rw-rw-rw-   0        0        0      653 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/vsepartoolbars.svg
+-rw-rw-rw-   0        0        0    15079 2023-03-18 21:39:13.000000 joulescope_ui-1.0.8/joulescope_ui/styles/manager.py
+-rw-rw-rw-   0        0        0     3635 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/parameter_file.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.274408 joulescope_ui-1.0.8/joulescope_ui/styles/system/
+-rw-rw-rw-   0        0        0      350 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/system/index.json
+-rw-rw-rw-   0        0        0       17 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/system/style.html
+-rw-rw-rw-   0        0        0     3222 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/system/style.qss
+-rw-rw-rw-   0        0        0      558 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/system/zoom_all.svg
+-rw-rw-rw-   0        0        0      481 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/system/zoom_in.svg
+-rw-rw-rw-   0        0        0      393 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/system/zoom_out.svg
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.285919 joulescope_ui-1.0.8/joulescope_ui/styles/test/
+-rw-rw-rw-   0        0        0        0 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/test/__init__.py
+-rw-rw-rw-   0        0        0     2816 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/test/test_color_file.py
+-rw-rw-rw-   0        0        0     2156 2023-03-18 18:42:17.000000 joulescope_ui-1.0.8/joulescope_ui/styles/test/test_manager.py
+-rw-rw-rw-   0        0        0     1959 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/test/test_parameter_file.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.315480 joulescope_ui-1.0.8/joulescope_ui/test/
+-rw-rw-rw-   0        0        0        0 2018-04-10 21:33:42.000000 joulescope_ui-1.0.8/joulescope_ui/test/__init__.py
+-rw-rw-rw-   0        0        0     1139 2023-03-10 14:49:52.000000 joulescope_ui-1.0.8/joulescope_ui/test/test_capabilities.py
+-rw-rw-rw-   0        0        0     6851 2023-04-12 17:49:35.000000 joulescope_ui-1.0.8/joulescope_ui/test/test_metadata.py
+-rw-rw-rw-   0        0        0    10861 2023-04-13 20:09:56.000000 joulescope_ui-1.0.8/joulescope_ui/test/test_pubsub.py
+-rw-rw-rw-   0        0        0    12814 2023-03-12 15:57:42.000000 joulescope_ui-1.0.8/joulescope_ui/test/test_pubsub_registry.py
+-rw-rw-rw-   0        0        0     5147 2023-03-16 16:02:02.000000 joulescope_ui-1.0.8/joulescope_ui/test/test_range_tool.py
+-rw-rw-rw-   0        0        0     2582 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/test/test_sanitize.py
+-rw-rw-rw-   0        0        0     2034 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/test/test_software_update.py
+-rw-rw-rw-   0        0        0     4055 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/test/test_time_map.py
+-rw-rw-rw-   0        0        0     1601 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/test/test_tooltip.py
+-rw-rw-rw-   0        0        0     5229 2023-04-12 21:57:44.000000 joulescope_ui-1.0.8/joulescope_ui/test/test_units.py
+-rw-rw-rw-   0        0        0     3197 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/time_map.py
+-rw-rw-rw-   0        0        0     2234 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/tooltip.py
+-rw-rw-rw-   0        0        0     7060 2023-01-24 22:12:47.000000 joulescope_ui-1.0.8/joulescope_ui/ui_util.py
+-rw-rw-rw-   0        0        0     7261 2023-04-12 21:56:15.000000 joulescope_ui-1.0.8/joulescope_ui/units.py
+-rw-rw-rw-   0        0        0       23 2023-04-04 19:20:04.000000 joulescope_ui-1.0.8/joulescope_ui/version.py
+-rw-rw-rw-   0        0        0    12791 2023-04-13 12:57:34.000000 joulescope_ui-1.0.8/joulescope_ui/view.py
+-rw-rw-rw-   0        0        0     1042 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widget_tools.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.318493 joulescope_ui-1.0.8/joulescope_ui/widgets/
+-rw-rw-rw-   0        0        0     1160 2023-04-12 20:18:29.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.320001 joulescope_ui-1.0.8/joulescope_ui/widgets/accumulator/
+-rw-rw-rw-   0        0        0      642 2023-04-12 20:02:06.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/accumulator/__init__.py
+-rw-rw-rw-   0        0        0     6954 2023-04-12 21:59:19.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/accumulator/accumulator_widget.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.330516 joulescope_ui-1.0.8/joulescope_ui/widgets/accumulator/styles/
+-rw-rw-rw-   0        0        0      109 2023-04-12 20:03:25.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/accumulator/styles/color_scheme_dark.txt
+-rw-rw-rw-   0        0        0      109 2023-04-12 20:03:47.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/accumulator/styles/color_scheme_light.txt
+-rw-rw-rw-   0        0        0       37 2023-04-12 20:36:04.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/accumulator/styles/font_scheme_js1.txt
+-rw-rw-rw-   0        0        0      122 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/accumulator/styles/index.json
+-rw-rw-rw-   0        0        0      762 2023-04-12 20:35:40.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/accumulator/styles/style.qss
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.333017 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/
+-rw-rw-rw-   0        0        0      647 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/__init__.py
+-rw-rw-rw-   0        0        0     3177 2023-03-15 21:07:03.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/device_control_widget.py
+-rw-rw-rw-   0        0        0     3397 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/device_info_dialog.py
+-rw-rw-rw-   0        0        0    20306 2023-04-12 17:47:44.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/js220_ctrl_widget.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.337021 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/styles/
+-rw-rw-rw-   0        0        0      180 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/styles/active_checked.svg
+-rw-rw-rw-   0        0        0      129 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/styles/active_unchecked.svg
+-rw-rw-rw-   0        0        0      129 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/styles/closed.svg
+-rw-rw-rw-   0        0        0       78 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/styles/color_scheme_dark.txt
+-rw-rw-rw-   0        0        0      216 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/styles/color_scheme_light.txt
+-rw-rw-rw-   0        0        0      240 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/styles/doc.svg
+-rw-rw-rw-   0        0        0     1936 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/styles/index.json
+-rw-rw-rw-   0        0        0     1749 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/styles/info.svg
+-rw-rw-rw-   0        0        0      125 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/styles/open.svg
+-rw-rw-rw-   0        0        0     4466 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/styles/style.qss
+-rw-rw-rw-   0        0        0      240 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/styles/target_power.svg
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.344052 joulescope_ui-1.0.8/joulescope_ui/widgets/example/
+-rw-rw-rw-   0        0        0      639 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/example/__init__.py
+-rw-rw-rw-   0        0        0     2100 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/example/example_widget.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.353611 joulescope_ui-1.0.8/joulescope_ui/widgets/example/styles/
+-rw-rw-rw-   0        0        0      100 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/example/styles/color_scheme_dark.txt
+-rw-rw-rw-   0        0        0      100 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/example/styles/color_scheme_light.txt
+-rw-rw-rw-   0        0        0       80 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/example/styles/font_scheme_js1.txt
+-rw-rw-rw-   0        0        0      122 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/example/styles/index.json
+-rw-rw-rw-   0        0        0      242 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/example/styles/style.qss
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.354611 joulescope_ui-1.0.8/joulescope_ui/widgets/flyout/
+-rw-rw-rw-   0        0        0      630 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/flyout/__init__.py
+-rw-rw-rw-   0        0        0     4010 2023-03-17 14:48:42.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/flyout/flyout_widget.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.356112 joulescope_ui-1.0.8/joulescope_ui/widgets/flyout/styles/
+-rw-rw-rw-   0        0        0        0 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/flyout/styles/color_scheme_dark.txt
+-rw-rw-rw-   0        0        0        0 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/flyout/styles/color_scheme_light.txt
+-rw-rw-rw-   0        0        0      130 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/flyout/styles/index.json
+-rw-rw-rw-   0        0        0      692 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/flyout/styles/style.qss
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.357116 joulescope_ui-1.0.8/joulescope_ui/widgets/hamburger/
+-rw-rw-rw-   0        0        0      638 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/hamburger/__init__.py
+-rw-rw-rw-   0        0        0     2164 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/hamburger/hamburger_widget.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.358125 joulescope_ui-1.0.8/joulescope_ui/widgets/help/
+-rw-rw-rw-   0        0        0      628 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/help/__init__.py
+-rw-rw-rw-   0        0        0     2350 2023-03-10 14:01:14.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/help/help_widget.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.358630 joulescope_ui-1.0.8/joulescope_ui/widgets/memory/
+-rw-rw-rw-   0        0        0      632 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/memory/__init__.py
+-rw-rw-rw-   0        0        0    10815 2023-04-12 19:57:12.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/memory/memory_widget.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.360633 joulescope_ui-1.0.8/joulescope_ui/widgets/memory/styles/
+-rw-rw-rw-   0        0        0      105 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/memory/styles/color_scheme_dark.txt
+-rw-rw-rw-   0        0        0      105 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/memory/styles/color_scheme_light.txt
+-rw-rw-rw-   0        0        0      122 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/memory/styles/index.json
+-rw-rw-rw-   0        0        0        0 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/memory/styles/style.qss
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.361637 joulescope_ui-1.0.8/joulescope_ui/widgets/progress_bar/
+-rw-rw-rw-   0        0        0      643 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/progress_bar/__init__.py
+-rw-rw-rw-   0        0        0     5816 2023-04-05 17:16:31.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/progress_bar/progress_bar_widget.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.362137 joulescope_ui-1.0.8/joulescope_ui/widgets/settings/
+-rw-rw-rw-   0        0        0      641 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/settings/__init__.py
+-rw-rw-rw-   0        0        0    21759 2023-04-13 19:27:43.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/settings/settings_widget.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.363137 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/
+-rw-rw-rw-   0        0        0      633 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/__init__.py
+-rw-rw-rw-   0        0        0     9819 2023-04-13 18:54:20.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/sidebar_widget.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.369645 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/
+-rw-rw-rw-   0        0        0      575 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/color_scheme_dark.txt
+-rw-rw-rw-   0        0        0      216 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/color_scheme_light.txt
+-rw-rw-rw-   0        0        0      358 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/device.svg
+-rw-rw-rw-   0        0        0      345 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/help.svg
+-rw-rw-rw-   0        0        0     4413 2023-04-13 15:29:15.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/index.json
+-rw-rw-rw-   0        0        0      421 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/memory.svg
+-rw-rw-rw-   0        0        0      274 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/misc.svg
+-rw-rw-rw-   0        0        0      309 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/pause.svg
+-rw-rw-rw-   0        0        0      241 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/play.svg
+-rw-rw-rw-   0        0        0      205 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/record.svg
+-rw-rw-rw-   0        0        0      511 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/settings.svg
+-rw-rw-rw-   0        0        0      309 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/stop.svg
+-rw-rw-rw-   0        0        0     5528 2023-04-13 15:30:01.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/style.qss
+-rw-rw-rw-   0        0        0      207 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/target_power.svg
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.371148 joulescope_ui-1.0.8/joulescope_ui/widgets/signal_record/
+-rw-rw-rw-   0        0        0      699 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/signal_record/__init__.py
+-rw-rw-rw-   0        0        0     6727 2023-03-29 19:41:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/signal_record/signal_record.py
+-rw-rw-rw-   0        0        0     7983 2023-03-18 13:24:49.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/signal_record/signal_record_config_widget.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.372652 joulescope_ui-1.0.8/joulescope_ui/widgets/statistics_record/
+-rw-rw-rw-   0        0        0      715 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/statistics_record/__init__.py
+-rw-rw-rw-   0        0        0     3942 2023-03-18 13:36:54.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/statistics_record/statistics_record.py
+-rw-rw-rw-   0        0        0     6501 2023-03-18 13:25:13.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/statistics_record/statistics_record_config_widget.py
+-rw-rw-rw-   0        0        0     6078 2023-01-24 22:12:47.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/switch.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.373652 joulescope_ui-1.0.8/joulescope_ui/widgets/value/
+-rw-rw-rw-   0        0        0      630 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/value/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.375652 joulescope_ui-1.0.8/joulescope_ui/widgets/value/styles/
+-rw-rw-rw-   0        0        0      152 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/value/styles/color_scheme_dark.txt
+-rw-rw-rw-   0        0        0      100 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/value/styles/color_scheme_light.txt
+-rw-rw-rw-   0        0        0      106 2023-04-04 15:40:17.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/value/styles/font_scheme_js1.txt
+-rw-rw-rw-   0        0        0      122 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/value/styles/index.json
+-rw-rw-rw-   0        0        0        0 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/value/styles/style.qss
+-rw-rw-rw-   0        0        0    26822 2023-04-12 21:58:36.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/value/value_widget.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.377156 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/
+-rw-rw-rw-   0        0        0      636 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/__init__.py
+-rw-rw-rw-   0        0        0     8426 2023-03-30 13:55:55.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/line_segments.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.383679 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/
+-rw-rw-rw-   0        0        0      841 2023-03-17 14:15:26.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/color_scheme_dark.txt
+-rw-rw-rw-   0        0        0        0 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/color_scheme_light.txt
+-rw-rw-rw-   0        0        0       34 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/font_scheme_js1.txt
+-rw-rw-rw-   0        0        0      754 2023-03-18 15:01:04.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/index.json
+-rw-rw-rw-   0        0        0      121 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/marker_add1.svg
+-rw-rw-rw-   0        0        0      198 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/marker_add2.svg
+-rw-rw-rw-   0        0        0      228 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/marker_clear.svg
+-rw-rw-rw-   0        0        0      237 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/pin_left.svg
+-rw-rw-rw-   0        0        0      237 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/pin_right.svg
+-rw-rw-rw-   0        0        0     3520 2023-03-18 15:02:05.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/style.qss
+-rw-rw-rw-   0        0        0      597 2023-03-18 15:06:21.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/y_zoom_all.svg
+-rw-rw-rw-   0        0        0      558 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/zoom_all.svg
+-rw-rw-rw-   0        0        0      471 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/zoom_in.svg
+-rw-rw-rw-   0        0        0      388 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/zoom_out.svg
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.383679 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/test/
+-rw-rw-rw-   0        0        0        0 2023-03-08 16:08:46.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/test/__init__.py
+-rw-rw-rw-   0        0        0    13485 2023-03-18 15:03:45.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/waveform_control.py
+-rw-rw-rw-   0        0        0   122898 2023-04-13 20:41:07.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/waveform_widget.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.168703 joulescope_ui-1.0.8/joulescope_ui.egg-info/
+-rw-rw-rw-   0        0        0     6885 2023-04-13 20:58:45.000000 joulescope_ui-1.0.8/joulescope_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9841 2023-04-13 20:58:45.000000 joulescope_ui-1.0.8/joulescope_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 20:58:45.000000 joulescope_ui-1.0.8/joulescope_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-04-13 20:58:45.000000 joulescope_ui-1.0.8/joulescope_ui.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      363 2023-04-13 20:58:45.000000 joulescope_ui-1.0.8/joulescope_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-13 20:58:45.000000 joulescope_ui-1.0.8/joulescope_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      117 2023-04-13 20:58:46.387683 joulescope_ui-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     8932 2023-04-13 20:52:43.000000 joulescope_ui-1.0.8/setup.py
```

### Comparing `joulescope_ui-1.0.7/CHANGELOG.md` & `joulescope_ui-1.0.8/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,35 @@
 
 # CHANGELOG
 
 This file contains the list of changes made to pyjoulescope_ui.
 
 
+## 1.0.8
+
+<span style="color:yellow">⚠ ALPHA RELEASE - USE WITH CAUTION ⚠</span> 
+
+Improves upon 1.0.7 but still alpha quality.  See the 1.0.0 release
+notes below for additional usage guidelines.
+
+2023 Apr 13
+
+* Fixed unplug/replug creating duplicate sample stream buffers.
+* Added JS220 firmware update.
+* Fixed metadata flag 'hidden' -> 'hide'.
+* Added duration to memory widget.
+* Increased default sidebar flyout width from 250 to 300. 
+* Added accumulator widget.
+* Added support for customary Ah & Wh units.
+* Added global settings support.
+  * Added sidebar direct link. 
+  * Added Settings Widget to Widget menu bar.
+* Added keyboard shortcuts to main and waveform widget.
+
+
 ## 1.0.7
 
 <span style="color:yellow">⚠ ALPHA RELEASE - USE WITH CAUTION ⚠</span> 
 
 Improves upon 1.0.6 but still alpha quality.  See the 1.0.0 release
 notes below for additional usage guidelines.
```

### Comparing `joulescope_ui-1.0.7/CREDITS.html` & `joulescope_ui-1.0.8/CREDITS.html`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/LICENSE.txt` & `joulescope_ui-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/PKG-INFO` & `joulescope_ui-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joulescope_ui
-Version: 1.0.7
+Version: 1.0.8
 Summary: Joulescope™ graphical user interface
 Home-page: https://www.joulescope.com
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/pyjoulescope_ui/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `joulescope_ui-1.0.7/README.md` & `joulescope_ui-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/__init__.py` & `joulescope_ui-1.0.8/joulescope_ui/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/__main__.py` & `joulescope_ui-1.0.8/joulescope_ui/__main__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/about.py` & `joulescope_ui-1.0.8/joulescope_ui/about.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/api.py` & `joulescope_ui-1.0.8/joulescope_ui/api.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/app.py` & `joulescope_ui-1.0.8/joulescope_ui/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,24 @@
         'brief': N_('The software update channel.'),
         'default': 'alpha',  #  todo change to stable for first stable release
         'options': [
             ['alpha', N_('alpha')],
             ['beta', N_('beta')],
             ['stable', N_('stable')],
         ]
-    }
+    },
+    'units': {
+        'dtype': 'str',
+        'brief': N_('The units to display.'),
+        'options': [
+            ['SI', N_('International System of Units (SI)')],
+            ['Xh', N_('Customary units (Ah and Wh)')],
+        ],
+        'default': 'SI',
+    },
 }
 
 
 _SETTINGS_VALUES_AT_START = {
     'statistics_stream_enable': True,
     'statistics_stream_record': False,
     'signal_stream_enable': True,
```

### Comparing `joulescope_ui-1.0.7/joulescope_ui/capabilities.py` & `joulescope_ui-1.0.8/joulescope_ui/capabilities.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/dev_signal_buffer_source.py` & `joulescope_ui-1.0.8/joulescope_ui/dev_signal_buffer_source.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/devices/jsdrv/device.py` & `joulescope_ui-1.0.8/joulescope_ui/devices/jsdrv/device.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/devices/jsdrv/js110.py` & `joulescope_ui-1.0.8/joulescope_ui/devices/jsdrv/js110.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,68 +20,72 @@
 import threading
 
 
 EVENTS = {
     'statistics/!data': Metadata('obj', 'Periodic statistics data for each signal.'),
 }
 
-SETTINGS = {
+_SETTINGS_OBJ_ONLY = {
     'name': {
         'dtype': 'str',
         'brief': N_('Device name'),
         'detail': N_("""\
-        The Joulescope UI automatically populates the device name
-        with the device type and serial number.
-
-        This setting allows you to change the default, if you wish, to better
-        reflect how you are using your JS110.  This setting is
-        most useful when you are instrumenting a system using 
-        multiple Joulescopes."""),
+            The Joulescope UI automatically populates the device name
+            with the device type and serial number.
+    
+            This setting allows you to change the default, if you wish, to better
+            reflect how you are using your JS110.  This setting is
+            most useful when you are instrumenting a system using 
+            multiple Joulescopes."""),
         'default': None,
     },
     'info': {
         'dtype': 'obj',
         'brief': N_('Device information'),
         'default': None,
-        'flags': ['ro', 'hidden'],
+        'flags': ['ro', 'hide'],
     },
     'state': {
         'dtype': 'int',
         'brief': N_('Device state indicator'),
         'options': [
             [0, 'closed'],
             [1, 'opening'],
             [2, 'open'],
             [3, 'closing'],
         ],
         'default': 0,
-        'flags': ['ro', 'hidden'],
+        'flags': ['ro', 'hide'],
     },
     'state_req': {
         'dtype': 'int',
         'brief': N_('Requested device state'),
         'options': [
             [0, 'closed'],
             [1, 'open'],
         ],
         'default': 1,
-        'flags': ['ro', 'hidden'],
+        'flags': ['ro', 'hide'],
     },
     'sources/1/name': {
         'dtype': 'str',
         'brief': N_('Device name'),
         'default': None,
-        'flags': ['ro', 'hidden'],  # duplicated from settings/name
+        'flags': ['ro', 'hide'],  # duplicated from settings/name
     },
     'sources/1/info': {
         'dtype': 'obj',
         'brief': N_('Device information'),
         'default': None,
-        'flags': ['ro', 'hidden'],  # duplicated from settings/info['device']
+        'flags': ['ro', 'hide'],  # duplicated from settings/info['device']
     },
+}
+
+
+_SETTINGS_CLASS = {
     'signal_frequency': {
         'dtype': 'int',
         'brief': N_('Signal frequency'),
         'detail': N_("""\
         This setting controls the output sampling frequency for the 
         measurement signals current, voltage, and power.  Use this
         setting to reduce the data storage requirements for long
@@ -141,15 +145,15 @@
             Toggle the connection between the current terminals.
 
             When enabled, current flows between the current terminals.
             When disabled, current cannot flow between the current terminals.
             In common system setups, this inhibits target power, which can
             be used to power cycle reset the target device."""),
         'default': True,
-        'flags': ['hidden'],  # Display in ExpandingWidget's header_ex_widget
+        'flags': ['hide'],  # Display in ExpandingWidget's header_ex_widget
     },
     'current_range': {
         'dtype': 'int',
         'brief': N_('Current range'),
         'detail': N_("""\
             Configure the J110's current range.  Most applications should
             use the default, "auto".
@@ -338,43 +342,48 @@
         'default': True,
         'topics': ('s/gpi/1/ctrl', 's/gpi/1/!data'),
     },
 }
 
 
 def _populate():
-    global SETTINGS, EVENTS
+    global _SETTINGS_OBJ_ONLY, EVENTS
     for signal_id, value in _SIGNALS.items():
-        SETTINGS[f'signals/{signal_id}/name'] = {
+        _SETTINGS_OBJ_ONLY[f'signals/{signal_id}/name'] = {
             'dtype': 'str',
             'brief': N_('Signal name'),
-            'flags': ['hidden'],
+            'flags': ['hide'],
             'default': value['brief'],
         }
-        SETTINGS[f'signals/{signal_id}/enable'] = {
+        _SETTINGS_OBJ_ONLY[f'signals/{signal_id}/enable'] = {
             'dtype': 'bool',
             'brief': value['brief'],
             'detail': value['detail'],
-            'flags': ['hidden'],
+            'flags': ['hide'],
             'default': value['default'],
         }
         EVENTS[f'signals/{signal_id}/!data'] = Metadata('obj', 'Signal data')
 
 
 _populate()
 
 
-@register
 class Js110(Device):
 
+    SETTINGS = _SETTINGS_CLASS
+
     def __init__(self, driver, device_path):
         super().__init__(driver, device_path)
+        _, model, serial_number = device_path.split('/')
+        name = f'{model.upper()}-{serial_number}'
         self.EVENTS = copy.deepcopy(EVENTS)
-        self.SETTINGS = copy.deepcopy(SETTINGS)
-        self.SETTINGS['name']['default'] = device_path
+        self.SETTINGS = copy.deepcopy(_SETTINGS_CLASS)
+        for key, value in _SETTINGS_OBJ_ONLY.items():
+            self.SETTINGS[key] = copy.deepcopy(value)
+        self.SETTINGS['name']['default'] = name
         self.SETTINGS['sources/1/name']['default'] = device_path
         self._info = {
             'vendor': 'Jetperch LLC',
             'model': 'JS110',
             'version': {
                 'hw': '1',
                 'fw': '0.0.0',
@@ -651,7 +660,10 @@
     def on_action_accum_clear(self, topic, value):
         prev_value = self._statistics_offsets
         if value is None:
             self._statistics_offsets = None
         else:
             self._statistics_offsets = list(value)
         return topic, prev_value
+
+
+register(Js110, 'JS110')
```

### Comparing `joulescope_ui-1.0.7/joulescope_ui/devices/jsdrv/js220.py` & `joulescope_ui-1.0.8/joulescope_ui/devices/jsdrv/js220.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,99 +12,102 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from joulescope_ui.capabilities import CAPABILITIES
 from .device import Device
 from joulescope_ui import N_, get_topic_name, register
 from joulescope_ui.metadata import Metadata
+from pyjoulescope_driver import release, program
 import copy
 import queue
 import threading
 
 
 def _version_u32_to_str(v):
     major = (v >> 24) & 0xff
     minor = (v >> 16) & 0xff
     patch = (v & 0xffff)
     return '.'.join(str(x) for x in [major, minor, patch])
 
 
+_PROGRESS_TOPIC = 'registry/progress/actions/!update'
+
 EVENTS = {
     'statistics/!data': Metadata('obj', 'Periodic statistics data for each signal.'),
 }
 
 _SETTINGS_OBJ_ONLY = {
     'name': {
         'dtype': 'str',
         'brief': N_('Device name'),
         'detail': N_("""\
-    The Joulescope UI automatically populates the device name
-    with the device type and serial number.
-
-    This setting allows you to change the default, if you wish, to better
-    reflect how you are using your JS220.  This setting is
-    most useful when you are instrumenting a system using 
-    multiple Joulescopes."""),
+            The Joulescope UI automatically populates the device name
+            with the device type and serial number.
+        
+            This setting allows you to change the default, if you wish, to better
+            reflect how you are using your JS220.  This setting is
+            most useful when you are instrumenting a system using 
+            multiple Joulescopes."""),
         'default': None,
     },
     'info': {
         'dtype': 'obj',
         'brief': N_('Device information'),
         'default': None,
-        'flags': ['ro', 'hidden'],
+        'flags': ['ro', 'hide'],
     },
     'state': {
         'dtype': 'int',
         'brief': N_('Device state indicator'),
         'options': [
             [0, 'closed'],
             [1, 'opening'],
             [2, 'open'],
             [3, 'closing'],
         ],
         'default': 0,
-        'flags': ['ro', 'hidden'],
+        'flags': ['ro', 'hide'],
     },
     'state_req': {
         'dtype': 'int',
         'brief': N_('Requested device state'),
         'options': [
             [0, 'closed'],
             [1, 'open'],
         ],
         'default': 1,
-        'flags': ['ro', 'hidden'],
+        'flags': ['ro', 'hide'],
     },
     'sources/1/name': {
         'dtype': 'str',
         'brief': N_('Device name'),
         'default': None,
-        'flags': ['ro', 'hidden'],  # duplicated from settings/name
+        'flags': ['ro', 'hide'],  # duplicated from settings/name
     },
     'sources/1/info': {
         'dtype': 'obj',
         'brief': N_('Device information'),
         'default': None,
-        'flags': ['ro', 'hidden'],  # duplicated from settings/info['device']
+        'flags': ['ro', 'hide'],  # duplicated from settings/info['device']
     },
 }
 
 _SETTINGS_CLASS = {
     'signal_frequency': {
         'dtype': 'int',
         'brief': N_('Signal frequency'),
         'detail': N_("""\
-        This setting controls the output sampling frequency for the 
-        measurement signals current, voltage, and power.  Use this
-        setting to reduce the data storage requirements for long
-        captures where lower temporal accuracy is sufficient. 
-        
-        The JS220 instrument always samples at 2 MHz and 
-        then downsamples to 1 MHz.  This setting controls 
-        additional optional downsampling."""),
+            This setting controls the output sampling frequency for the 
+            measurement signals current, voltage, and power.  Use this
+            setting to reduce the data storage requirements for long
+            captures where lower temporal accuracy is sufficient. 
+            
+            The JS220 instrument always samples at 2 MHz and 
+            then downsamples to 1 MHz.  This setting controls 
+            additional optional downsampling."""),
         'options': [
             [1000000, "1 MHz"],
             [500000, "500 kHz"],
             [200000, "200 kHz"],
             [100000, "100 kHz"],
             [50000, "50 kHz"],
             [20000, "20 kHz"],
@@ -150,15 +153,15 @@
             Toggle the connection between the current terminals.
             
             When enabled, current flows between the current terminals.
             When disabled, current cannot flow between the current terminals.
             In common system setups, this inhibits target power, which can
             be used to power cycle reset the target device."""),
         'default': True,
-        'flags': ['hidden'],   # Display in ExpandingWidget's header_ex_widget
+        'flags': ['hide'],   # Display in ExpandingWidget's header_ex_widget
     },
     'current_range': {
         'dtype': 'int',
         'brief': N_('Current range'),
         'detail': N_("""\
             Configure the JS220's current range.  Most applications should
             use the default, "auto".
@@ -250,14 +253,35 @@
         'brief': N_('Trigger output value'),
         'detail': N_("""Turn the trigger output on or off.
         
             The trigger must also be configured for output for this
             setting to have any effect."""),
         'default': False,
     },
+    'firmware_channel': {
+        'dtype': 'str',
+        'brief': 'FW channel',
+        'detail': """The maturity level channel for firmware updates.
+        
+            We strongly recommend keeping the default "stable"
+            unless you are a Joulescope developer.""",
+        'options': [['alpha', 'alpha'], ['beta', 'beta'], ['stable', 'stable']],
+        'default': 'stable',
+        'flags': ['hide', 'dev'],
+    },
+    'firmware_available': {
+        'dtype': 'obj',
+        'brief': 'FW available',
+        'detail': '''Firmware update availability.
+        
+            None when no firmware update is available.
+            Map of subname: [current, available] when available.''',
+        'default': None,  # or dict of name: [current, available]
+        'flags': ['hide', 'tmp', 'ro'],
+    },
 }
 
 
 _SETTINGS_MAP = {
     'signal_frequency': 'h/fs',
 
 }
@@ -364,31 +388,30 @@
 
 def _populate():
     global _SETTINGS_CLASS, EVENTS
     for signal_id, value in _SIGNALS.items():
         _SETTINGS_CLASS[f'signals/{signal_id}/name'] = {
             'dtype': 'str',
             'brief': N_('Signal name'),
-            'flags': ['hidden'],
+            'flags': ['hide'],
             'default': value['brief'],
         }
         _SETTINGS_CLASS[f'signals/{signal_id}/enable'] = {
             'dtype': 'bool',
             'brief': value['brief'],
             'detail': value['detail'],
-            'flags': ['hidden'],
+            'flags': ['hide'],
             'default': value['default'],
         }
         EVENTS[f'signals/{signal_id}/!data'] = Metadata('obj', 'Signal data')
 
 
 _populate()
 
 
-@register
 class Js220(Device):
 
     SETTINGS = _SETTINGS_CLASS
 
     def __init__(self, driver, device_path):
         super().__init__(driver, device_path)
         _, model, serial_number = device_path.split('/')
@@ -405,14 +428,15 @@
             'serial_number': serial_number,
         }
         self.SETTINGS['info']['default'] = self._info
         self.SETTINGS['sources/1/name']['default'] = name
         self.SETTINGS['sources/1/info']['default'] = self._info
 
         self._on_stats_fn = self._on_stats  # for unsub
+        self._driver_device_open = False
         self._thread = None
         self._quit = False
         self._target_power_app = False
         self._queue = queue.Queue()
 
         self._statistics_offsets = None
         self._on_settings_fn = self._on_settings
@@ -491,22 +515,22 @@
             self._ui_publish('settings/state', 'opening')
             self._quit = False
             self._thread = threading.Thread(target=self._run)
             self._thread.start()
             self._log.info('open req done')
 
     def _close_req(self):
+        t, self._thread = self._thread, None
         # must be called from UI pubsub thread
-        if self._thread is not None:
+        if t is not None:
             self._log.info('closing')
             self._ui_publish('settings/state', 'closing')
             self._send_to_thread('close')
             self._quit = True
-            self._thread.join()
-            self._thread = None
+            t.join()
             self._ui_publish('settings/state', 'closed')
             self._log.info('closed')
 
     def on_action_finalize(self):
         self._log.info('finalize')
         self._close_req()
 
@@ -542,15 +566,16 @@
             self._driver_publish('c/trigger/dir', value)
         elif topic == 'gpio_voltage':
             self._driver_publish('c/gpio/vref', value)
         elif topic == 'name':
             self._ui_publish('settings/sources/1/name', value)
         elif topic in ['info', 'state', 'state_req', 'out', 'enable',
                        'sources', 'sources/1', 'sources/1/info', 'sources/1/name',
-                       'signals']:
+                       'signals',
+                       'firmware_available', 'firmware_channel']:
             pass
         elif topic.startswith('signals/'):
             pass
         else:
             self._log.warning('Unsupported topic %s', f'{get_topic_name(self)}/settings/{topic}')
 
     def _current_range_update(self):
@@ -572,21 +597,80 @@
         elif cmd == 'current_range_update':
             self._current_range_update()
         elif cmd == 'close':
             pass  # handled in outer wrapper
         else:
             self._log.warning('Unhandled cmd: %s', cmd)
 
+    def _is_firmware_update_available(self):
+        try:
+            image = release.release_get(self.firmware_channel)
+            segments = release.release_to_segments(image)
+            ctrl_app = segments[release.SUBTYPE_CTRL_APP]
+            fpga = segments[release.SUBTYPE_SENSOR_FPGA]
+        except Exception:
+            self._log.info('firmware_update_available: Could not parse firmware image')
+            return None
+        ctrl_app_now = self._driver_query('c/fw/version')
+        fpga_now = self._driver_query('s/fpga/version')
+        if ctrl_app_now >= ctrl_app['version'] and fpga_now >= fpga['version']:
+            self._log.info('firmware_update_available %s: up to date', self.unique_id)
+            return None
+        v = program.version_to_str
+        rv = {
+            'ctrl_app': [v(ctrl_app_now), v(ctrl_app['version'])],
+            'fpga': [v(fpga_now), v(fpga['version'])]
+        }
+        self._log.info('firmware_update_available %s: %s', self.unique_id, rv)
+        return rv
+
+    def _firmware_update(self):
+        if self.firmware_available is None:
+            return False
+        try:
+            image = release.release_get(self.firmware_channel)
+        except Exception:
+            self._log.info('Could not parse firmware image')
+            return False
+        self._close()
+        self._log.info('firmware_update: start')
+        self.firmware_available = None
+        self._driver.open(self._path, 'restore')
+
+        def on_progress(completion, msg):
+            value = {
+                'id': f'{self.unique_id}.firmware_update',
+                'progress': completion,
+                'name': N_('Update') + ' ' + self.unique_id,
+                'brief': msg,
+            }
+            self._pubsub.publish(_PROGRESS_TOPIC, value)
+
+        rv = program.release_program(self._driver, self.device_path, image,
+                                     progress=on_progress)
+        versions_before = dict(rv[0])
+        result = ['firmware_update: complete']
+        for key, value in rv[1]:
+            v = versions_before.get(key, '?.?.?')
+            result.append(f'    {key:10s}  {v} => {value}')
+        self._log.info('\n'.join(result))
+        self._ui_publish('')
+        return True
+
     def _run(self):
         self._log.info('thread start')
         if self._open():
             self._log.info('thread exit due to open fail')
             return 1
         self._ui_publish('settings/state', 'open')
         self._log.info('thread open complete')
+        self.firmware_available = self._is_firmware_update_available()
+        if self.firmware_available is not None:
+            self._quit |= self._firmware_update()
+
         while not self._quit:
             try:
                 cmd, args = self._queue.get(timeout=0.1)
             except queue.Empty:
                 continue
             if cmd == 'close':
                 break
@@ -614,31 +698,34 @@
             self._driver_publish('s/stats/ctrl', 1)
             self._driver_subscribe('s/stats/value', 'pub', self._on_stats_fn)
             self._ui_subscribe('settings', self._on_settings_fn, ['pub', 'retain'])
         except Exception:
             self._log.exception('driver config failed')
             self._ui_publish('settings/state', 'closing')
             return 1
+        self._driver_device_open = True
         self._log.info('open %s done', self.unique_id)
         return 0
 
     def _close(self):
-        if self.state == 0:  # already closed
+        if not self._driver_device_open:
+            self._log.info('close %s when already closed', self.unique_id)
             return
         self._log.info('close %s start', self.unique_id)
         self._ui_unsubscribe('settings', self._on_settings_fn)
         self._ui_publish('settings/state', 'closing')
         self._driver_unsubscribe('s/stats/value', self._on_stats_fn)
         try:
             for t in _SIGNALS.values():
                 self._driver_publish(t['topics'][0], 0)
             self._driver_publish('s/stats/ctrl', 0)
         except RuntimeError as ex:
             self._log.info('Exception during close cleanup: %s', ex)
         self._driver.close(self._path)
+        self._driver_device_open = False
         self._log.info('close %s done', self.unique_id)
 
     def _on_stats(self, topic, value):
         if self._statistics_offsets is None:
             accum_sample_start = value['time']['accum_samples']['value'][-1]
             charge = value['accumulators']['charge']['value']
             energy = value['accumulators']['energy']['value']
@@ -676,7 +763,10 @@
     def on_action_accum_clear(self, topic, value):
         prev_value = self._statistics_offsets
         if value is None:
             self._statistics_offsets = None
         else:
             self._statistics_offsets = list(value)
         return topic, prev_value
+
+
+register(Js220, 'JS220')
```

### Comparing `joulescope_ui-1.0.7/joulescope_ui/devices/jsdrv/jsdrv_stream_buffer.py` & `joulescope_ui-1.0.8/joulescope_ui/devices/jsdrv/jsdrv_stream_buffer.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from joulescope_ui import CAPABILITIES, N_, Metadata, get_topic_name
+from pyjoulescope_driver import time64
 from .device import Device
 import copy
 import logging
 import time
 
 
 _MEM_CLEANUP_PERIOD_S = 1.0   # process memory cleanup with this period (seconds)
@@ -44,25 +45,31 @@
         'default': N_('Joulescope stream buffer'),
     },
     'size': {
         'dtype': 'int',
         'brief': N_('Buffer memory size in bytes'),
         'default': int(0.5 * 1024 ** 3),
     },
+    'duration': {
+        'dtype': 'float',
+        'brief': N_('Buffer memory duration in seconds'),
+        'default': 0.0,
+        'flags': ['ro', 'tmp'],
+    },
     'sources': {
         'dtype': 'node',
         'brief': 'Hold source settings',
         'default': None,
-        'flags': ['hidden'],
+        'flags': ['hide'],
     },
     'signals': {
         'dtype': 'node',
         'brief': 'Hold signal settings',
         'default': None,
-        'flags': ['hidden'],
+        'flags': ['hide'],
     },
     'clear_on_play': {
         'dtype': 'bool',
         'brief': 'Clear on play',
         'detail': """\
             When signal sample streaming is paused, the stream buffer pauses
             sample accumulation.  This setting controls what happens on play
@@ -86,35 +93,35 @@
         'brief': N_('Name'),
         'default': N_('Source name'),
     }),
     'info': Metadata({
         'dtype': 'obj',
         'brief': N_('Source information'),
         'default': None,
-        'flags': ['ro', 'hidden', 'skip_undo'],
+        'flags': ['ro', 'hide', 'skip_undo'],
     }),
 }
 
 _SETTINGS_PER_SIGNAL = {
     'name': Metadata({
         'dtype': 'str',
         'brief': N_('Name'),
         'default': N_('Signal name'),
     }),
     'meta': Metadata({
         'dtype': 'obj',
         'brief': N_('Signal metadata'),
         'default': None,
-        'flags': ['ro', 'hidden', 'skip_undo'],
+        'flags': ['ro', 'hide', 'skip_undo'],
     }),
     'range': Metadata({
         'dtype': 'obj',
         'brief': N_('Signal time range'),
         'default': None,
-        'flags': ['ro', 'hidden', 'skip_undo'],
+        'flags': ['ro', 'hide', 'skip_undo'],
     }),
 }
 
 
 def defer_until_registered(f):
     def wrapper(self, value):
         if self._initialize_cache is not None:
@@ -157,29 +164,35 @@
         self._req_time = {}  # device_rsp_id: time_last_used
         self._collect_time = time.time()
 
     def __str__(self):
         return f'JsdrvStreamBuffer({self._id})'
 
     def on_action_device_add(self, device: Device):
+        self._log.info('device_add %s', device.unique_id)
         self._sources[device.unique_id] = device
         topic = get_topic_name(self.unique_id)
         source_topic = f'{topic}/settings/sources/{device.unique_id}'
         for name, meta in _SETTINGS_PER_SOURCE.items():
             self.pubsub.topic_add(f'{source_topic}/{name}', meta, exists_ok=True)
         self.pubsub.publish(f'{source_topic}/name', device.name)
         self.pubsub.publish(f'{source_topic}/info', device.info)
         device_topic = get_topic_name(device)
         for signal in self.pubsub.enumerate(f'{device_topic}/settings/signals'):
             self.pubsub.subscribe(f'{device_topic}/settings/signals/{signal}/enable',
                                   self._on_signal_enable, ['pub', 'retain'])
         self.pubsub.publish(f'{topic}/events/sources/!add', device.unique_id)
 
     def on_action_device_remove(self, device):
+        self._log.info('device_remove %s', device.unique_id)
         topic = get_topic_name(self.unique_id)
+        signals = list(self._signals.keys())
+        for signal_id in signals:
+            if signal_id.split('.')[0] == device.unique_id:
+                self.on_action_remove(signal_id)
         source_topic = f'{topic}/settings/{device.unique_id}'
         self.pubsub.publish(f'{topic}/events/sources/!remove', device.unique_id)
         for name, meta in _SETTINGS_PER_SOURCE.items():
             self.pubsub.topic_remove(f'{source_topic}/{name}')
         for topic in list(self._device_subscriptions.keys()):
             if topic.startswith(device.device_path):
                 fn = self._device_subscriptions.pop(topic)
@@ -218,16 +231,18 @@
         self._driver_publish('m/@/!remove', int(self._id))
         self.pubsub.topic_remove(f'{get_topic_name(self)}/settings/signals')
 
     def _on_device_signal_info(self, topic, value):
         # device_signal_info m/001/s/001/info {'version': 1, 'field_id': 1, 'index': 0, 'element_type': 4, 'element_size_bits': 32, 'topic': b'u/js220/000415/s/i/!data', 'size_in_utc': 8725724278, 'size_in_samples': 8126464, 'time_range_utc': {'start': 911549982937, 'end': 914237683277, 'length': 2503116}, 'time_range_samples': {'start': 848947077, 'end': 851450193, 'length': 2503116}, 'sample_rate': 1000000.0}
         buf_id = int(topic.split('/')[-2])
         signal_id = self._signals_reverse.get(buf_id)
+        duration = value['size_in_utc'] / time64.SECOND
+        t = get_topic_name(self)
+        self.pubsub.publish(f'{t}/settings/duration', duration)
         if signal_id is not None:
-            t = get_topic_name(self)
             utc = value['time_range_utc']
             r = {
                 'utc': [utc['start'], utc['end']],
                 'samples': value['time_range_samples'],
                 'sample_rate': value['time_map']['counter_rate'],
             }
             self.pubsub.publish(f'{t}/settings/signals/{signal_id}/range', r)
@@ -253,14 +268,18 @@
         self._driver_publish(f'm/{self._id}/g/hold', value)
 
     @defer_until_registered
     def on_setting_mode(self, value):
         self._driver_publish(f'm/{self._id}/g/mode', int(value))
 
     def on_action_add(self, signal_id):
+        if signal_id in self._signals:
+            self._log.info('add duplicate %s', signal_id)
+            return
+        self._log.info('add %s', signal_id)
         buf_id = self._signals_free.pop(0)
         unique_id, signal = signal_id.split('.')
         device = self._sources[unique_id]
         signal_meta = copy.deepcopy(device.info)
         self._signals[signal_id] = [buf_id, signal_meta]
         self._signals_reverse[buf_id] = signal_id
         device_path = device.device_path
@@ -278,14 +297,15 @@
         device_source = f'{device_path}/{subtopic}'
         buf_prefix = f'm/{self._id}/s/{buf_id:03d}'
         self._driver_publish(f'{buf_prefix}/topic', device_source)
         self._device_subscribe(f'{buf_prefix}/info', ['pub', 'pub_retain'], self._on_device_signal_info)
         self.pubsub.publish(f'{ui_prefix}/events/signals/!add', signal_id)
 
     def on_action_remove(self, signal_id):
+        self._log.info('remove %s', signal_id)
         buf_id, _ = self._signals.pop(signal_id)
         self._signals_reverse.pop(buf_id)
         self._signals_free.append(buf_id)
         self._driver_publish(f'm/{self._id}/a/!remove', buf_id)
         ui_prefix = get_topic_name(self)
         self.pubsub.publish(f'{ui_prefix}/events/signals/!remove', signal_id)
         self.pubsub.topic_remove(f'{ui_prefix}/settings/signals/{signal_id}')
```

### Comparing `joulescope_ui-1.0.7/joulescope_ui/devices/jsdrv/jsdrv_wrapper.py` & `joulescope_ui-1.0.8/joulescope_ui/devices/jsdrv/jsdrv_wrapper.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/entry_points/ui.py` & `joulescope_ui-1.0.8/joulescope_ui/entry_points/ui.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/error_window.py` & `joulescope_ui-1.0.8/joulescope_ui/error_window.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/expanding_widget.py` & `joulescope_ui-1.0.8/joulescope_ui/expanding_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/exporter.py` & `joulescope_ui-1.0.8/joulescope_ui/exporter.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/file_dialog.py` & `joulescope_ui-1.0.8/joulescope_ui/file_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/fonts/DSEG14-Modern/DSEG-LICENSE.txt` & `joulescope_ui-1.0.8/joulescope_ui/fonts/DSEG14-Modern/DSEG-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/fonts/Hack/LICENSE.md` & `joulescope_ui-1.0.8/joulescope_ui/fonts/Hack/LICENSE.md`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/fonts/Lato/OFL.txt` & `joulescope_ui-1.0.8/joulescope_ui/fonts/Lato/OFL.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/fonts/SourceCodePro/LICENSE.md` & `joulescope_ui-1.0.8/joulescope_ui/fonts/SourceCodePro/LICENSE.md`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/fonts/SourceSerifPro/OFL.txt` & `joulescope_ui-1.0.8/joulescope_ui/fonts/SourceSerifPro/OFL.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/fonts.rcc` & `joulescope_ui-1.0.8/joulescope_ui/fonts.rcc`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/getting_started.html` & `joulescope_ui-1.0.8/joulescope_ui/getting_started.html`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/help_ui.py` & `joulescope_ui-1.0.8/joulescope_ui/help_ui.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/jls_source.py` & `joulescope_ui-1.0.8/joulescope_ui/jls_source.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/jls_v1.py` & `joulescope_ui-1.0.8/joulescope_ui/jls_v1.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/jls_v2.py` & `joulescope_ui-1.0.8/joulescope_ui/jls_v2.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/json.py` & `joulescope_ui-1.0.8/joulescope_ui/json.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/locale/__init__.py` & `joulescope_ui-1.0.8/joulescope_ui/locale/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/logging_util.py` & `joulescope_ui-1.0.8/joulescope_ui/logging_util.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/main.py` & `joulescope_ui-1.0.8/joulescope_ui/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # https://stackoverflow.com/questions/11874767/real-time-plotting-in-while-loop-with-matplotlib
 # https://wiki.qt.io/Gallery_of_Qt_CSS_Based_Styles
 
 from joulescope_ui import pubsub_singleton, N_, get_topic_name, tooltip_format, CAPABILITIES, Metadata, __version__
+from joulescope_ui.pubsub import UNDO_TOPIC, REDO_TOPIC
+from joulescope_ui.shortcuts import Shortcuts
 from joulescope_ui.widgets import *   # registers all built-in widgets
 from joulescope_ui.logging_util import logging_preconfig, logging_config
 from joulescope_ui.styles.manager import style_settings
 from joulescope_ui.process_monitor import ProcessMonitor
 from joulescope_ui import software_update
 from joulescope_ui.ui_util import show_in_folder
 from joulescope_ui.dev_signal_buffer_source import DevSignalBufferSource
@@ -136,14 +138,15 @@
     def __init__(self, filename=None, is_config_load=False):
         self._log = logging.getLogger(__name__)
         super(MainWindow, self).__init__()
         self.setWindowTitle('Joulescope')
         self._dialog = None
         self._pubsub = pubsub_singleton
         self._pubsub_process_count_last = self._pubsub.process_count
+        self._shortcuts = Shortcuts(self)
         self.SETTINGS = style_settings(N_('UI'))
         self.SETTINGS['changelog_version_show'] = {
             'dtype': 'str',
             'brief': 'The version for the last changelog show',
             'default': '__default__',
         }
         self._pubsub.register(self, 'ui', parent=None)
@@ -254,15 +257,14 @@
             ]],
         ])
         self._view_menu_group = QtGui.QActionGroup(self._menu_items['view_menu'][0])
         self._view_menu_group.setExclusive(True)
         self.setMenuBar(self._menu_bar)
         self._pubsub.subscribe('registry/paths/settings/mru_files', self._on_mru, flags=['pub', 'retain'])
 
-        _device_factory_add()
         self._pubsub.subscribe('registry_manager/capabilities/view.object/list',
                                self._on_change_views, flags=['pub', 'retain'])
         self._pubsub.subscribe('registry/view/settings/active', self._on_change_views, flags=['pub'])
         self._pubsub.subscribe('registry_manager/capabilities/widget.class/list',
                                self._on_change_widgets, flags=['pub', 'retain'])
 
         if not is_config_load:
@@ -299,28 +301,33 @@
         self._cpu_utilization = QtWidgets.QLabel(self._status_bar)
         self._cpu_utilization.setToolTip(_CPU_UTILIZATION_TOOLTIP)
         self._status_bar.addPermanentWidget(self._cpu_utilization)
         self._mem_utilization = QtWidgets.QLabel(self._status_bar)
         self._mem_utilization.setToolTip(_MEMORY_UTILIZATION_TOOLTIP)
         self._status_bar.addPermanentWidget(self._mem_utilization)
 
+        self._shortcuts.add(QtGui.QKeySequence.Undo, UNDO_TOPIC, None)
+        self._shortcuts.add(QtGui.QKeySequence.Redo, REDO_TOPIC, None)
+        self._shortcuts.add(QtCore.Qt.Key_Space, 'registry/app/settings/signal_stream_enable', '__toggle__')
+
         self.show()
         # self._mem_leak_debugger = MemLeakDebugger(self)
         # self._side_bar.on_cmd_show(1)
         if self._pubsub.query('registry/app/settings/software_update_check'):
             self._software_update_thread = software_update.check(
                 callback=self._do_cbk,
                 path=self._pubsub.query('common/settings/paths/update'),
                 channel=self._pubsub.query('registry/app/settings/software_update_channel'))
 
         # display changelog on version change
         topic = f'{self.topic}/settings/changelog_version_show'
         if __version__ != self._pubsub.query(topic, default=None):
             self._pubsub.publish(topic, __version__)
             self._pubsub.publish('registry/help_html/actions/!show', 'changelog')
+        self.resync_request()
 
     def _center(self, resize=None):
         screen = self.screen()
         sz = screen.size()
         sw, sh = sz.width(), sz.height()
         if resize == True:
             w, h = int(sw * 0.8), int(sh * 0.8)
@@ -477,15 +484,14 @@
     def on_action_view_logs(self):
         path = pubsub_singleton.query('common/settings/paths/log')
         self._log.info('view logs: %s', path)
         show_in_folder(path)
 
     def closeEvent(self, event):
         self._log.info('closeEvent()')
-        _device_factory_finalize()
         self._pubsub.publish('registry/JlsSource/actions/!finalize', None)
         return super(MainWindow, self).closeEvent(event)
 
     def on_action_close(self, value):
         global _software_update, _config_clear
         if isinstance(value, dict):
             _software_update = value.get('software_update')
@@ -538,15 +544,17 @@
 
         app = QtWidgets.QApplication([])
         resources = load_resources()
         fonts = load_fonts()
         appnope.nope()
         ui = MainWindow(filename=filename, is_config_load=is_config_load)
         pubsub_singleton.notify_fn = ui.resync_request
+        _device_factory_add()
         rc = app.exec_()
+        _device_factory_finalize()
         _finalize()
         del ui
         if _software_update is not None:
             software_update.apply(_software_update)
         return rc
     except Exception:
         if app is None:
```

### Comparing `joulescope_ui-1.0.7/joulescope_ui/mem_leak_debugger.py` & `joulescope_ui-1.0.8/joulescope_ui/mem_leak_debugger.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/metadata.py` & `joulescope_ui-1.0.8/joulescope_ui/metadata.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/paths.py` & `joulescope_ui-1.0.8/joulescope_ui/paths.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         'brief': N_('The name for this widget.'),
         'default': N_('Paths'),
     },
     'path': {
         'dtype': 'str',
         'brief': N_('Default path'),
         'detail': N_('The default path for loading and saving files.'),
-        'flags': ['ro', 'hidden'],
+        'flags': ['ro', 'hide'],
         'default': None,
     },
     'fixed_path': {
         'dtype': 'str',
         'brief': N_('Fixed default path'),
         'detail': N_('The fixed default path for loading and saving files.'),
         'default': None,
@@ -72,15 +72,15 @@
             [3, N_('Most recently used path')],
         ],
         'default': 3,
     },
     'mru_files': {
         'dtype': 'obj',
         'brief': N_('Most recent file list'),
-        'flags': ['ro', 'hidden'],
+        'flags': ['ro', 'hide'],
         'default': [],
     },
     'mru_count': {
         'dtype': 'int',
         'brief': N_('Most recently used length'),
         'options': [
             [5, '5'],
```

### Comparing `joulescope_ui-1.0.7/joulescope_ui/plugins/__init__.py` & `joulescope_ui-1.0.8/joulescope_ui/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/plugins/cdf.py` & `joulescope_ui-1.0.8/joulescope_ui/plugins/cdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 class CdfRangeToolWidget(QtWidgets.QWidget):
 
     SETTINGS = {
         'data': {
             'dtype': 'obj',
             'brief': 'Hold the data',
             'default': None,
-            'flags': ['hidden'],
+            'flags': ['hide'],
         }
     }
 
     def __init__(self, data=None):
         self._data = data
         self._plot_item = None
         super().__init__()
```

### Comparing `joulescope_ui-1.0.7/joulescope_ui/plugins/frequency.py` & `joulescope_ui-1.0.8/joulescope_ui/plugins/frequency.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 class FrequencyRangeToolWidget(QtWidgets.QWidget):
 
     SETTINGS = {
         'data': {
             'dtype': 'obj',
             'brief': 'Hold the histogram data',
             'default': None,
-            'flags': ['hidden'],
+            'flags': ['hide'],
         }
     }
 
     def __init__(self, data=None):
         self._data = data
         self._bg = None
         self._f = None
```

### Comparing `joulescope_ui-1.0.7/joulescope_ui/plugins/histogram.py` & `joulescope_ui-1.0.8/joulescope_ui/plugins/histogram.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 class HistogramRangeToolWidget(QtWidgets.QWidget):
 
     SETTINGS = {
         'data': {
             'dtype': 'obj',
             'brief': 'Hold the histogram data',
             'default': None,
-            'flags': ['hidden'],
+            'flags': ['hide'],
         }
     }
 
     def __init__(self, data=None):
         self._data = data
         self._hist = None
         self._bin_edges = None
```

### Comparing `joulescope_ui-1.0.7/joulescope_ui/plugins/max_window.py` & `joulescope_ui-1.0.8/joulescope_ui/plugins/max_window.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/plugins/plugin_helpers.py` & `joulescope_ui-1.0.8/joulescope_ui/plugins/plugin_helpers.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/plugins/usb_inrush.py` & `joulescope_ui-1.0.8/joulescope_ui/plugins/usb_inrush.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/process_monitor.py` & `joulescope_ui-1.0.8/joulescope_ui/process_monitor.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/profile.py` & `joulescope_ui-1.0.8/joulescope_ui/profile.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/pubsub.py` & `joulescope_ui-1.0.8/joulescope_ui/pubsub.py`

 * *Files 0% similar despite different names*

```diff
@@ -939,15 +939,18 @@
         except KeyError:
             self._log.warning('Publish to unknown topic %s', topic)
             return None
         if flag == 'pub':
             if t.meta is None:
                 self._log.info('Missing metadata for %s', t.topic_name)
             else:
-                value = t.meta.validate(value)
+                if t.meta.dtype == 'bool' and value in ['!', '~', '__toggle__']:
+                    value = not t.value
+                else:
+                    value = t.meta.validate(value)
             if t.subtopic_name.startswith('!'):
                 cmds_update_fn = t.update_fn['command']
                 if len(cmds_update_fn):
                     rv = cmds_update_fn[0](self, topic, value)
                     self._undo_capture.cmd_add(topic, value, rv)
             elif t.value == value:
                 # self._log.debug('dedup %s: %s == %s', topic_name, t.value, value)
```

### Comparing `joulescope_ui-1.0.7/joulescope_ui/range_tool.py` & `joulescope_ui-1.0.8/joulescope_ui/range_tool.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/resources/dmg_background.svg` & `joulescope_ui-1.0.8/joulescope_ui/resources/dmg_background.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/resources/icons.svg` & `joulescope_ui-1.0.8/joulescope_ui/resources/icons.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/resources/zoom.svg` & `joulescope_ui-1.0.8/joulescope_ui/resources/zoom.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/resources.py` & `joulescope_ui-1.0.8/joulescope_ui/resources.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/resources.rcc` & `joulescope_ui-1.0.8/joulescope_ui/resources.rcc`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/sanitize.py` & `joulescope_ui-1.0.8/joulescope_ui/sanitize.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/software_update.py` & `joulescope_ui-1.0.8/joulescope_ui/software_update.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/styles/README.md` & `joulescope_ui-1.0.8/joulescope_ui/styles/README.md`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/styles/__init__.py` & `joulescope_ui-1.0.8/joulescope_ui/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/styles/color_editor.py` & `joulescope_ui-1.0.8/joulescope_ui/styles/color_editor.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/styles/color_file.py` & `joulescope_ui-1.0.8/joulescope_ui/styles/color_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/styles/color_picker.py` & `joulescope_ui-1.0.8/joulescope_ui/styles/color_picker.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/styles/color_scheme.py` & `joulescope_ui-1.0.8/joulescope_ui/styles/color_scheme.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/styles/color_scheme_dark.txt` & `joulescope_ui-1.0.8/joulescope_ui/styles/color_scheme_dark.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/styles/color_scheme_light.txt` & `joulescope_ui-1.0.8/joulescope_ui/styles/color_scheme_light.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/styles/font_scheme.py` & `joulescope_ui-1.0.8/joulescope_ui/styles/font_scheme.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/styles/fonts.py` & `joulescope_ui-1.0.8/joulescope_ui/styles/fonts.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/styles/js1/detach.svg` & `joulescope_ui-1.0.8/joulescope_ui/styles/js1/detach.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/styles/js1/index.json` & `joulescope_ui-1.0.8/joulescope_ui/styles/js1/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/styles/js1/style.qss` & `joulescope_ui-1.0.8/joulescope_ui/styles/js1/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/styles/js1/tabs_menu.svg` & `joulescope_ui-1.0.8/joulescope_ui/styles/js1/tabs_menu.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/styles/js1/vmovetoolbar.svg` & `joulescope_ui-1.0.8/joulescope_ui/styles/js1/vmovetoolbar.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/styles/js1/vsepartoolbars.svg` & `joulescope_ui-1.0.8/joulescope_ui/styles/js1/vsepartoolbars.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/styles/manager.py` & `joulescope_ui-1.0.8/joulescope_ui/styles/manager.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/styles/parameter_file.py` & `joulescope_ui-1.0.8/joulescope_ui/styles/parameter_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/styles/system/style.qss` & `joulescope_ui-1.0.8/joulescope_ui/styles/system/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/styles/system/zoom_all.svg` & `joulescope_ui-1.0.8/joulescope_ui/styles/system/zoom_all.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/styles/test/test_color_file.py` & `joulescope_ui-1.0.8/joulescope_ui/styles/test/test_color_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/styles/test/test_manager.py` & `joulescope_ui-1.0.8/joulescope_ui/styles/test/test_manager.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/styles/test/test_parameter_file.py` & `joulescope_ui-1.0.8/joulescope_ui/styles/test/test_parameter_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/test/test_capabilities.py` & `joulescope_ui-1.0.8/joulescope_ui/test/test_capabilities.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/test/test_metadata.py` & `joulescope_ui-1.0.8/joulescope_ui/test/test_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,15 @@
             'int',
             brief='My int',
             detail='My detail description.',
             default=42,
             options=[[1, 'one'], [42, 'answer']],
             range=[0, 100],
             format='%d',
-            flags=['hidden'],
+            flags=['hide'],
         )
         k = m.to_map()
         self.assertEqual(m.dtype, k['dtype'])
         for key in ['dtype', 'brief', 'detail', 'default', 'options', 'range', 'format', 'flags']:
             self.assertIn(key, k)
 
     def test_from_meta(self):
```

### Comparing `joulescope_ui-1.0.7/joulescope_ui/test/test_pubsub.py` & `joulescope_ui-1.0.8/joulescope_ui/test/test_pubsub.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,14 +231,15 @@
         p.redo()
         with self.assertRaises(KeyError):
             p.query(TOPIC1)
 
     def test_save(self):
         topic = 'registry/value/settings/my_topic'
         p1 = PubSub()
+        p1.topic_add('registry_manager/next_unique_id', dtype='int', brief='next_unique_id', default=1)
         p1.topic_add(topic, dtype='str', brief='my topic', default='hello')
         f = io.StringIO()
         p1.save(f)
         s = f.getvalue()
 
         p2 = PubSub()
         p2.registry_initialize()
@@ -266,10 +267,24 @@
         t.start()
         t.join()
         self.assertEqual(['notify'], self.pub)
         self.assertEqual('hello', p1.query(TOPIC1))
         p1.process()
         self.assertEqual('world', p1.query(TOPIC1))
 
+    def test_bool_toggle(self):
+        p1 = PubSub()
+        p1.topic_add(TOPIC1, dtype='bool', brief='my topic', default=False)
+        p1.process()
+        self.assertEqual(False, p1.query(TOPIC1))
+
+        p1.publish(TOPIC1, '!')
+        p1.process()
+        self.assertEqual(True, p1.query(TOPIC1))
+
+        p1.publish(TOPIC1, '__toggle__')
+        p1.process()
+        self.assertEqual(False, p1.query(TOPIC1))
+
     # todo complicated undo with stack usage
     # todo profiles
     # todo settings
```

### Comparing `joulescope_ui-1.0.7/joulescope_ui/test/test_pubsub_registry.py` & `joulescope_ui-1.0.8/joulescope_ui/test/test_pubsub_registry.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/test/test_range_tool.py` & `joulescope_ui-1.0.8/joulescope_ui/test/test_range_tool.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/test/test_sanitize.py` & `joulescope_ui-1.0.8/joulescope_ui/test/test_sanitize.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/test/test_software_update.py` & `joulescope_ui-1.0.8/joulescope_ui/test/test_software_update.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/test/test_time_map.py` & `joulescope_ui-1.0.8/joulescope_ui/test/test_time_map.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/test/test_tooltip.py` & `joulescope_ui-1.0.8/joulescope_ui/test/test_tooltip.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/test/test_units.py` & `joulescope_ui-1.0.8/joulescope_ui/test/test_units.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,32 +20,34 @@
 from joulescope_ui import units
 import numpy as np
 
 
 class TestUnits(unittest.TestCase):
 
     def test_charge(self):
-        self.assertEqual({'value': 1, 'units': 'C'}, units.convert_units(1, 'C', 'C'))
-        self.assertEqual({'value': 1 / 3600, 'units': 'Ah'}, units.convert_units(1, 'C', 'Ah'))
-        self.assertEqual({'value': 1, 'units': 'Ah'}, units.convert_units(1, 'Ah', 'Ah'))
-        self.assertEqual({'value': 3600, 'units': 'C'}, units.convert_units(1, 'Ah', 'C'))
+        self.assertEqual((1, 'C'), units.convert_units(1, 'C', 'SI'))
+        self.assertEqual((1 / 3600, 'Ah'), units.convert_units(1, 'C', 'Xh'))
 
     def test_energy(self):
-        self.assertEqual({'value': 1, 'units': 'J'}, units.convert_units(1, 'J', 'J'))
-        self.assertEqual({'value': 1 / 3600, 'units': 'Wh'}, units.convert_units(1, 'J', 'Wh'))
-        self.assertEqual({'value': 1, 'units': 'Wh'}, units.convert_units(1, 'Wh', 'Wh'))
-        self.assertEqual({'value': 3600, 'units': 'J'}, units.convert_units(1, 'Wh', 'J'))
+        self.assertEqual((1, 'J'), units.convert_units(1, 'J', 'J'))
+        self.assertEqual((1 / 3600, 'Wh'), units.convert_units(1, 'J', 'Xh'))
 
     def test_elapsed_time_formatter(self):
-        self.assertEqual('1 s', units.elapsed_time_formatter(1))
-        self.assertEqual('1000 s', units.elapsed_time_formatter(1000.1))
-        self.assertEqual('2:01', units.elapsed_time_formatter(121, fmt='standard'))
-        self.assertEqual('20:01', units.elapsed_time_formatter(1201, fmt='standard'))
-        self.assertEqual('1:02:03', units.elapsed_time_formatter(3723, fmt='standard'))
-        self.assertEqual('1:02:03:04', units.elapsed_time_formatter(93784, fmt='standard'))
+        self.assertEqual(('1.00000', 's'), units.elapsed_time_formatter(1))
+        self.assertEqual(('1', 's'), units.elapsed_time_formatter(1, trim_trailing_zeros=True))
+        self.assertEqual(('1.10000', 's'), units.elapsed_time_formatter(1.1))
+        self.assertEqual(('1.1', 's'), units.elapsed_time_formatter(1.1, trim_trailing_zeros=True))
+        self.assertEqual(('1.1', 's'), units.elapsed_time_formatter(1.11111111111111, precision=2))
+        self.assertEqual(('1.11111', 's'), units.elapsed_time_formatter(1.11111111111111))
+        self.assertEqual(('1000.10', 's'), units.elapsed_time_formatter(1000.1))
+        self.assertEqual(('2:01.000', 'm:ss'), units.elapsed_time_formatter(121, fmt='standard'))
+        self.assertEqual(('2:01', 'm:ss'), units.elapsed_time_formatter(121, fmt='standard', precision=0))
+        self.assertEqual(('20:01.00', 'mm:ss'), units.elapsed_time_formatter(1201, fmt='standard'))
+        self.assertEqual(('1:02:03.00', 'h:mm:ss'), units.elapsed_time_formatter(3723, fmt='standard'))
+        self.assertEqual(('2:05:49:44', 'D:hh:mm:ss'), units.elapsed_time_formatter(193784, fmt='standard'))
 
     def assertClose(self, expected, actual):
         np.testing.assert_almost_equal(expected[0], actual[0])
         self.assertEqual(expected[1], actual[1])
         np.testing.assert_almost_equal(expected[2], actual[2])
 
     def test_no_change(self):
```

### Comparing `joulescope_ui-1.0.7/joulescope_ui/time_map.py` & `joulescope_ui-1.0.8/joulescope_ui/time_map.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/tooltip.py` & `joulescope_ui-1.0.8/joulescope_ui/tooltip.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/ui_util.py` & `joulescope_ui-1.0.8/joulescope_ui/ui_util.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/units.py` & `joulescope_ui-1.0.8/joulescope_ui/units.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,18 +17,31 @@
 
 For full handling of units, see the excellent quantities module
 http://pythonhosted.org/quantities/.
 """
 
 
 import re
+import numpy as np
+from joulescope_ui import N_, pubsub_singleton
+
 
 # https://www.regular-expressions.info/floatingpoint.html
 #RE_IS_NUMBER = re.compile('^([-+]?[0-9]*\.?[0-9]+(?:[eE][-+]?[0-9]+))')
 RE_IS_NUMBER = re.compile('^\s*([-+]?[0-9]*\.?[0-9]+)\s*(.*)')
+UNITS_SETTING = {
+    'dtype': 'str',
+    'brief': N_('The units to display.'),
+    'options': [
+        ['default', N_('Use the application defaults')],
+        ['SI', N_('International System of Units (SI)')],
+        ['Xh', N_('Customary units (Ah and Wh)')],
+    ],
+    'default': 'default',
+}
 
 
 _UNIT_PREFIX = [
     (1e24, 'Y'),
     (1e21, 'Z'),
     (1e18, 'E'),
     (1e15, 'P'),
@@ -62,23 +75,14 @@
 
 FIELD_UNITS_INTEGRAL = {
     'current': 'charge',
     'power': 'energy',
 }
 
 
-UNIT_CONVERTER = {
-    # (from, to): conversion function
-    ('C', 'Ah'): lambda x: x / 3600.0,
-    ('Ah', 'C'): lambda x: x * 3600.0,
-    ('J', 'Wh'): lambda x: x / 3600.0,
-    ('Wh', 'J'): lambda x: x * 3600.0,
-}
-
-
 def unit_prefix(value):
     """Get the unit prefix and adjust value.
 
     :param value: The value to convert to a power of 1000.
     :return: The tuple of (adjusted_value, prefix, scale)
         where value = scale * adjust_value
         Scale is always a power of 10 (10**k).
@@ -146,57 +150,84 @@
         if v is not None:
             if v >= 1:
                 v = int(v)
             number *= v
     return number
 
 
-def convert_units(value, input_units, output_units):
-    key = (input_units, output_units)
-    fn = UNIT_CONVERTER.get(key)
-    if fn is not None:
-        return {
-            'value': fn(value),
-            'units': output_units}
-    return {
-        'value': value,
-        'units': input_units}
+def convert_units(x, x_units, unit_setting):
+    if x_units not in ['C', 'J']:
+        return x, x_units
+    if unit_setting == 'default':
+        unit_setting = pubsub_singleton.query('registry/app/settings/units', default='SI')
+    if unit_setting == 'Xh':
+        x /= 3600
+        y_units = 'Wh' if x_units == 'J' else 'Ah'
+    else:
+        y_units = x_units
+    return x, y_units
 
 
-def elapsed_time_formatter(seconds, cmdp=None, fmt=None):
+def elapsed_time_formatter(seconds, fmt=None, precision=None, trim_trailing_zeros=None):
     """Format time in seconds to a string.
 
     :param seconds: The elapsed time in seconds.
-    :param cmdp: The optional CommandProcessor containing the time formatting options.
     :param fmt: The optional format string containing:
         * 'seconds': Display time in seconds.
         * 'standard': Display time as D:hh:mm:ss.
-    :return: The elapsed time string.
+    :param precision: The integer precision to display given in
+        powers of 10.  This parameter determines the number of
+        fractional seconds digits.
+    :param trim_trailing_zeros: When True, trim any trailing fractional
+        zero digits.  When False (default), keep full precision.
+    :return: The tuple of elapsed time string and units string.
     """
-    seconds = int(seconds)  # drop fractions
+    precision = 6 if precision is None else int(precision)
+    x = float(seconds)
+    x_pow = int(np.ceil(np.log10(abs(x) + 1e-15)))
+    fract_digits = min(max(precision - x_pow, 0), precision)
+    fract_fmt = '{x:.' + str(fract_digits) + 'f}'
     fmt = 'seconds' if fmt is None else str(fmt)
-    if cmdp is not None:
-        if isinstance(cmdp, str):
-            fmt = cmdp
-        else:
-            fmt = cmdp['Units/elapsed_time']
     if seconds >= 60 and fmt in ['D:hh:mm:ss', 'conventional', 'standard']:
-        days = seconds // (24 * 60 * 60)
-        seconds -= days * (24 * 60 * 60)
-        hours = seconds // (60 * 60)
-        seconds -= hours * (60 * 60)
-        minutes = seconds // 60
-        seconds -= minutes * 60
-        time_parts = f'{days}:{hours:02d}:{minutes:02d}:{seconds:02d}'.split(':')
+        days = int(x / (24 * 60 * 60))
+        x -= days * (24 * 60 * 60)
+        hours = int(x / (60 * 60))
+        x -= hours * (60 * 60)
+        minutes = int(x / 60)
+        x -= minutes * 60
+        seconds_str = fract_fmt.format(x=x)
+        if '.' in seconds_str:
+            if seconds_str[1] == '.':
+                seconds_str = '0' + seconds_str
+        elif len(seconds_str) == 1:
+            seconds_str = '0' + seconds_str
+        time_parts = f'{days}:{hours:02d}:{minutes:02d}:{seconds_str}'.split(':')
+        units_parts = 'D:hh:mm:ss'.split(':')
         while True:
             p = time_parts[0]
             p_zero = '0' * len(p)
             if p == p_zero:
                 time_parts.pop(0)
+                units_parts.pop(0)
             else:
                 break
         time_str = ':'.join(time_parts)
+        units_str = ':'.join(units_parts)
         while time_str[0] == '0':
             time_str = time_str[1:]
-        return time_str
+            if len(units_str) >= 2 and units_str[1] != ':':
+                units_str = units_str[1:]
+        return time_str, units_str
     else:
-        return f'{seconds} s'
+        units_str = 's'
+        if fract_digits:
+            time_str = fract_fmt.format(x=x)
+        else:
+            time_str = str(int(x))
+
+    if bool(trim_trailing_zeros) and '.' in time_str:
+        while time_str[-1] == '0':
+            time_str = time_str[:-1]
+        if time_str[-1] == '.':
+            time_str = time_str[:-1]
+
+    return time_str, units_str
```

### Comparing `joulescope_ui-1.0.7/joulescope_ui/view.py` & `joulescope_ui-1.0.8/joulescope_ui/view.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,19 +77,21 @@
         'default': 'js1',
         'options': [['js1', N_('Joulescope standard font theme')]],
     },
     'ads_state': {
         'dtype': 'str',
         'brief': 'The Advanced Docking System state for restoring widget layout.',
         'default': '',
+        'flags': ['hide'],
     },
     'geometry': {
         'dtype': 'obj',
         'brief': 'The window size for restoring the view.',
         'default': None,
+        'flags': ['hide'],
     }
 }
 
 
 class View:
     CAPABILITIES = ['view@']
     SETTINGS = {**VIEW_SETTINGS, **style_settings(N_('View'))}
```

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widget_tools.py` & `joulescope_ui-1.0.8/joulescope_ui/widget_tools.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/__init__.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from .accumulator import AccumulatorWidget
 from .device_control import DeviceControlWidget
 # from .example import ExampleWidget
 from .memory import MemoryWidget
 from .hamburger import HamburgerWidget
 from .help import HelpWidget
 from .progress_bar import ProgressBarWidget
 from .sidebar import SideBar
```

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/device_control/__init__.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/device_control/device_control_widget.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/device_control_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/device_control/device_info_dialog.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/device_info_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/device_control/js220_ctrl_widget.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/js220_ctrl_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -383,15 +383,15 @@
         self._gpo['buttons'].append(b)
 
     def _add_settings(self):
         for name, value in self._DEVICE_SETTINGS.items():
             if name.startswith('out/') or name.endswith('/enable'):
                 continue
             meta = Metadata(value)
-            if 'hidden' in meta.flags:
+            if 'hide' in meta.flags:
                 continue
             if name == 'current_range' and self.is_js220:
                 pass  # todo add custom ranged slider for min/max selection
             self._add(name, meta)
 
     def _add_str(self, name):
         w = QtWidgets.QLineEdit(self)
```

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/device_control/styles/index.json` & `joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/styles/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/device_control/styles/info.svg` & `joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/styles/info.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/device_control/styles/style.qss` & `joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/example/__init__.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/example/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/example/example_widget.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/example/example_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/flyout/__init__.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/flyout/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/flyout/flyout_widget.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/flyout/flyout_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/flyout/styles/style.qss` & `joulescope_ui-1.0.8/joulescope_ui/widgets/flyout/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/hamburger/__init__.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/hamburger/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/hamburger/hamburger_widget.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/hamburger/hamburger_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/help/__init__.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/help/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/help/help_widget.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/help/help_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/memory/__init__.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/memory/memory_widget.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/memory/memory_widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,21 +12,23 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from PySide6 import QtWidgets, QtGui, QtCore
 from joulescope_ui import N_, register
 from joulescope_ui.tooltip import tooltip_format
 from joulescope_ui.styles import styled_widget, color_as_qcolor, font_as_qfont
+from joulescope_ui.units import elapsed_time_formatter
 import numpy as np
 import os
 import psutil
 
 _TOPIC = 'registry/JsdrvStreamBuffer:001'
 _TOPIC_CLEAR_ON_PLAY = f'{_TOPIC}/settings/clear_on_play'
 _TOPIC_SIZE = f'{_TOPIC}/settings/size'
+_TOPIC_DURATION = f'{_TOPIC}/settings/duration'
 _GB_FACTOR = 1024 ** 3
 _SZ_MIN = int(0.01 * _GB_FACTOR)
 
 
 def _mem_proc():
     return psutil.Process(os.getpid()).memory_info().rss
 
@@ -156,14 +158,15 @@
 @register
 @styled_widget(N_('Memory'))
 class MemoryWidget(QtWidgets.QWidget):
     CAPABILITIES = ['widget@']
 
     def __init__(self, parent=None):
         self._on_size_fn = self._on_size
+        self._on_duration_fn = self._on_duration
         self._base = 0
         self._size = 0  # in bytes
         self._used = 0
         super().__init__(parent=parent)
         self.setObjectName('memory_widget')
         self.setSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Preferred)
         self._layout = QtWidgets.QVBoxLayout()
@@ -189,17 +192,20 @@
             'total_units': QtWidgets.QLabel('GB', self._grid_widget),
             'available_label': QtWidgets.QLabel(N_('Available RAM size'), self._grid_widget),
             'available_value': QtWidgets.QLabel(f'0', self._grid_widget),
             'available_units': QtWidgets.QLabel('GB', self._grid_widget),
             'used_label': QtWidgets.QLabel(N_('Used RAM size'), self._grid_widget),
             'used_value': QtWidgets.QLabel(f'0', self._grid_widget),
             'used_units': QtWidgets.QLabel('GB', self._grid_widget),
+            'duration_label': QtWidgets.QLabel(N_('Duration'), self._grid_widget),
+            'duration_value': QtWidgets.QLabel('', self._grid_widget),
+            'duration_units': QtWidgets.QLabel('', self._grid_widget),
         }
 
-        for row, s in enumerate(['size', 'available', 'used', 'total']):
+        for row, s in enumerate(['size', 'available', 'used', 'total', 'duration']):
             self._grid_layout.addWidget(self._widgets[f'{s}_label'], row, 0)
             self._grid_layout.addWidget(self._widgets[f'{s}_value'], row, 1)
             self._grid_layout.addWidget(self._widgets[f'{s}_units'], row, 2)
 
         self._clear = QtWidgets.QPushButton(N_('Clear'), self)
         self._clear.pressed.connect(self._on_clear)
         self._layout.addWidget(self._clear)
@@ -241,14 +247,15 @@
             sz = self.pubsub.query(_TOPIC_SIZE)
             if mem > sz:
                 self._base = mem - sz
             else:
                 self._base = mem
             self.pubsub.subscribe(_TOPIC_CLEAR_ON_PLAY, self._clear_on_play_fn, ['pub', 'retain'])
             self.pubsub.subscribe(_TOPIC_SIZE, self._on_size_fn, ['pub', 'retain'])
+            self.pubsub.subscribe(_TOPIC_DURATION, self._on_duration_fn, ['pub', 'retain'])
             meta = self.pubsub.metadata(_TOPIC_CLEAR_ON_PLAY)
             self._clear_on_play.setToolTip(tooltip_format(meta.brief, meta.detail))
 
             self._timer.start(1000)
         if not self._memset.is_active:
             self._update()
 
@@ -273,7 +280,13 @@
 
     def _on_size(self, value):
         self._size = int(value)
         s = _format(self._size)
         self._widgets['size_value'].setText(s)
         self._memset.update_size(value)
         self._update(value)
+
+    def _on_duration(self, value):
+        dt = 0.0 if value is None else float(value)
+        time_str, units_str = elapsed_time_formatter(dt, fmt='standard', precision=3)
+        self._widgets[f'duration_value'].setText(time_str)
+        self._widgets[f'duration_units'].setText(units_str)
```

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/progress_bar/__init__.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/progress_bar/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/progress_bar/progress_bar_widget.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/progress_bar/progress_bar_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/settings/__init__.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/settings/settings_widget.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/settings/settings_widget.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,21 +15,22 @@
 
 from PySide6 import QtCore, QtGui, QtWidgets
 from joulescope_ui import pubsub_singleton, N_, register_decorator, \
     get_instance, get_unique_id, get_topic_name, Metadata, tooltip_format
 from joulescope_ui.ui_util import comboBoxConfig, comboBoxSelectItemByText
 from joulescope_ui.styles import styled_widget, font_as_qfont, font_as_qss
 from joulescope_ui.styles.color_picker import ColorItem
-from joulescope_ui.styles.color_scheme import COLOR_SCHEMES
-from joulescope_ui.styles.font_scheme import FONT_SCHEMES
 from joulescope_ui.styles.manager import style_settings
 import copy
 import logging
 
 
+_NAME = N_('Settings')
+
+
 class _GridWidget(QtWidgets.QWidget):
     """Base grid widget for all settings tabs.
 
     Subclasses use the _widgets and _grid attributes.
     """
 
     def __init__(self, parent=None):
@@ -77,20 +78,21 @@
 
     @property
     def object(self):
         return self._obj
 
     @object.setter
     def object(self, obj):
+        obj = get_instance(obj, default=None)
         if self._obj is not None:
             self.clear()
         if obj is None:
             self._obj = None
             return
-        self._obj = get_instance(obj)
+        self._obj = obj
         name_label = QtWidgets.QLabel(N_('Name'), self)
         self._grid.addWidget(name_label, 0, 0, 1, 1)
         self._widgets.append(name_label)
         value_label = QtWidgets.QLabel(N_('Value'), self)
         self._grid.addWidget(value_label, 0, 1, 1, 2)
         self._widgets.append(value_label)
 
@@ -100,25 +102,26 @@
         settings = pubsub_singleton.enumerate(topic, absolute=False, traverse=True)
         for setting in settings:
             if setting in styles:
                 continue
             self._insert(topic, setting)
 
     def _insert(self, topic, setting):
-        label = QtWidgets.QLabel(setting, self)
-        self._grid.addWidget(label, self._row, 0, 1, 1)
-        self._widgets.append(label)
-
         settings_topic = f'{topic}/{setting}'
         meta: Metadata = pubsub_singleton.metadata(settings_topic)
-        if meta is not None:
-            tooltip = tooltip_format(meta.brief, meta.detail)
-            label.setToolTip(tooltip)
+        if meta is None:
+            return
+        elif 'hide' in meta.flags:
+            return
         else:
-            tooltip = None
+            tooltip = tooltip_format(meta.brief, meta.detail)
+
+        label = QtWidgets.QLabel(setting, self)
+        self._grid.addWidget(label, self._row, 0, 1, 1)
+        self._widgets.append(label)
         w = None
         if meta.options is not None and len(meta.options):
             w = self._insert_combobox(settings_topic, meta)
         elif meta.dtype == 'bool':
             w = self._insert_bool(settings_topic)
         elif meta.dtype == 'str':
             w = self._insert_str(settings_topic, meta)
@@ -185,15 +188,15 @@
 
 class ColorEditorWidget(_GridWidget):
 
     def __init__(self, parent=None):
         self._colors = None
         self._obj = None
         self._topic = None
-        self._log = logging.getLogger(__name__)
+        self._log = logging.getLogger(__name__ + '.color')
         self._color_scheme = pubsub_singleton.query('registry/style/settings/color_scheme', default='dark')
         super().__init__(parent)
         self.setObjectName('color_editor_widget')
         self._color_widgets = []
 
     def _on_change(self, name, color):
         if len(color) == 7:
@@ -226,31 +229,32 @@
 
     @property
     def object(self):
         return self._obj
 
     @object.setter
     def object(self, obj):
+        obj = get_instance(obj, default=None)
         if self._obj is not None:
             self.clear()
             self._obj = None
         if obj is None:
             self._obj = None
             return
-        self._obj = get_instance(obj)
+        self._obj = obj
         if not hasattr(obj, 'style_obj') or obj.style_obj is None:
             return
-        self._topic = get_topic_name(self._obj)
+        self._topic = get_topic_name(obj)
         cls = obj.__class__
         colors = copy.deepcopy(cls._style_cls['load']['colors'][self._color_scheme])
         cls_colors = pubsub_singleton.query(f'{get_topic_name(obj.__class__)}/settings/colors')
         if cls_colors is not None:
             for color_name, color_value in cls_colors[self._color_scheme].items():
                 colors[color_name] = color_value
-        if not isinstance(self._obj, type):
+        if not isinstance(obj, type):
             if obj.colors is not None:
                 for key, value in obj.colors[self._color_scheme].items():
                     colors[key] = value
         self._colors = colors
 
         name_label = QtWidgets.QLabel(N_('Name'), self)
         self._grid.addWidget(name_label, 0, 0, 1, 1)
@@ -308,41 +312,42 @@
 
     def __init__(self, parent=None):
         super().__init__(parent)
         self._fonts = None
         self._obj = None
         self._topic = None
         self._font_scheme = pubsub_singleton.query('registry/style/settings/font_scheme', default='js1')
-        self._log = logging.getLogger(__name__)
+        self._log = logging.getLogger(__name__ + '.font')
         self.setObjectName('font_editor_widget')
 
     @property
     def object(self):
         return self._obj
 
     @object.setter
     def object(self, obj):
+        obj = get_instance(obj, default=None)
         if self._obj is not None:
             self.clear()
             self._obj = None
         if obj is None:
             self._obj = None
             return
-        self._obj = get_instance(obj)
-        self._topic = get_topic_name(self._obj)
+        self._obj = obj
+        self._topic = get_topic_name(obj)
         if not hasattr(obj, 'style_obj') or obj.style_obj is None:
             return
         cls = obj.__class__
 
         fonts = copy.deepcopy(cls._style_cls['load']['fonts'][self._font_scheme])
         cls_fonts = pubsub_singleton.query(f'{get_topic_name(obj.__class__)}/settings/fonts')
         if cls_fonts is not None:
             for font_name, font_value in cls_fonts[self._font_scheme].items():
                 fonts[font_name] = font_value
-        if not isinstance(self._obj, type):
+        if not isinstance(obj, type):
             if obj.fonts is not None:
                 for key, value in obj.fonts[self._font_scheme].items():
                     fonts[key] = value
         self._fonts = fonts
 
         name_label = QtWidgets.QLabel(N_('Name'), self)
         self._grid.addWidget(name_label, 0, 0, 1, 1)
@@ -377,35 +382,35 @@
 class StyleDefineEditorWidget(_GridWidget):
 
     def __init__(self, parent=None):
         super().__init__(parent)
         self._entries = {}
         self._obj = None
         self._topic = None
-        self._log = logging.getLogger(__name__)
+        self._log = logging.getLogger(__name__ + '.style')
         self.setObjectName('style_define_editor_widget')
 
     @property
     def object(self):
         return self._obj
 
     @object.setter
     def object(self, obj):
+        obj = get_instance(obj, default=None)
         if self._obj is not None:
             self.clear()
             self._obj = None
         if obj is None:
             self._obj = None
             return
         if not hasattr(obj, 'style_obj') or obj.style_obj is None:
             return
 
-        obj = get_instance(obj)
         self._obj = obj
-        self._topic = get_topic_name(self._obj)
+        self._topic = get_topic_name(obj)
         cls = obj.__class__
         entries = copy.deepcopy(cls._style_cls['load']['style_defines'])
         cls_entries = pubsub_singleton.query(f'{get_topic_name(obj.__class__)}/settings/style_defines')
         if cls_entries is not None:
             for e_name, e_value in cls_entries.items():
                 entries[e_name] = e_value
         if not isinstance(obj, type) and obj.style_defines is not None:
@@ -431,70 +436,136 @@
             self._widgets.append(w)
 
     def _on_change(self, name, value):
         self._entries[name] = value
         pubsub_singleton.publish(f'{self._topic}/settings/style_defines', dict(self._entries))
 
 
+def _class_items(capability):
+    entries = []
+    classes = pubsub_singleton.query(f'registry_manager/capabilities/{capability}/list')
+    for clz in classes:
+        instances = pubsub_singleton.query(f'{get_topic_name(clz)}/instances')
+        children = [[None, x, None] for x in instances if get_instance(x, default=None) is not None]
+        entries.append([None, clz, children])
+    return entries
+
+
+class SelectorWidget(QtWidgets.QTreeView):
+
+    def __init__(self, parent=None):
+        self._parent = parent
+        super().__init__(parent)
+        self.setSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
+        self.setSizeAdjustPolicy(QtWidgets.QAbstractScrollArea.SizeAdjustPolicy.AdjustToContents)
+        self.setHorizontalScrollBarPolicy(QtGui.Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
+        self._model = QtGui.QStandardItemModel(self)
+        self._model.setHorizontalHeaderLabels(['Name'])
+
+        self.setEditTriggers(QtWidgets.QAbstractItemView.NoEditTriggers)
+        self.setSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Preferred)
+        self.setSelectionBehavior(QtWidgets.QAbstractItemView.SelectRows)
+        self.setModel(self._model)
+        self.setHeaderHidden(True)
+        self.selectionModel().currentChanged.connect(self._on_changed)
+
+        items = [
+            # [name, unique_id, children]
+            [N_('Common'), 'app', None],
+            # [None, 'ui', None],
+            [None, 'paths', None],
+            [N_('View defaults'), 'view', None],
+            [N_('View'), pubsub_singleton.query('registry/view/settings/active'), None],
+            [N_('Devices'), '', _class_items('device.class')],
+            [N_('Widgets'), '', _class_items('widget.class')],
+        ]
+
+        self._populate(self._model.invisibleRootItem(), items)
+
+    @QtCore.Slot(object, object)
+    def _on_changed(self, model_index, model_index_old):
+        unique_id = self._model.data(model_index, QtCore.Qt.UserRole + 1)
+        if len(unique_id):
+            self._parent.object = unique_id
+        else:
+            self._parent.object = None
+
+    def _populate(self, parent, items):
+        for name, unique_id, children in items:
+            if name is None:
+                name = pubsub_singleton.query(f'{get_topic_name(unique_id)}/settings/name', default=unique_id)
+            child_item = QtGui.QStandardItem(name)
+            child_item.setData(unique_id, QtCore.Qt.UserRole + 1)
+            parent.appendRow(child_item)
+            if children is not None:
+                self._populate(child_item, children)
+
+
 @register_decorator(unique_id='settings')
-@styled_widget(N_('settings'))
-class SettingsWidget(QtWidgets.QWidget):
+@styled_widget(_NAME)
+class SettingsWidget(QtWidgets.QSplitter):
+    CAPABILITIES = ['widget@']
 
     SETTINGS = {
         'target': {
             'dtype': 'str',
             'brief': 'The unique_id for the target widget.',
-            'default': '',
+            'default': None,
         }
     }
 
     def __init__(self, parent=None):
+        self._log = logging.getLogger(__name__)
         super(SettingsWidget, self).__init__(parent)
         self._obj = None
         self.setObjectName(f'settings_widget')
-        self.setSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Preferred)
-        self._layout = QtWidgets.QVBoxLayout()
-        self._layout.setObjectName('settings_widget_layout')
-        self._layout.setSpacing(0)
-        self._layout.setContentsMargins(0, 0, 0, 0)
+        self.setSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
+
+        self._left = SelectorWidget(self)
 
         self._widgets = []
         widgets = [
             [SettingsEditorWidget(self), N_('Settings')],
             [ColorEditorWidget(self), N_('Colors')],
             [FontEditorWidget(self), N_('Fonts')],
             [StyleDefineEditorWidget(self), N_('Defines')],
         ]
 
         self._tabs = QtWidgets.QTabWidget(self)
+        self._tabs.setSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
         for widget, title in widgets:
+            widget.setSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
             scroll = QtWidgets.QScrollArea(self._tabs)
             scroll.setObjectName(widget.objectName() + '_scroll')
             scroll.setWidgetResizable(True)
             scroll.setWidget(widget)
             self._tabs.addTab(scroll, title)
             self._widgets.append([widget, scroll])
-        self._layout.addWidget(self._tabs)
-        self.setLayout(self._layout)
+
+        self.addWidget(self._left)
+        self.addWidget(self._tabs)
 
     def closeEvent(self, event):
         self.object = None
         return super().closeEvent(event)
 
     def on_setting_target(self, value):
         if isinstance(value, str) and not len(value):
             return  # default value, ignore
-        self.object = get_instance(value)
+        self._left.setVisible(value is None)
+        self.object = get_instance(value, default=None)
 
     @property
     def object(self):
         return self._obj
 
     @object.setter
     def object(self, obj):
+        obj_str = '[None]' if obj is None else get_unique_id(obj)
+        self._log.info('object <= %s', obj_str)
         for widget, _ in self._widgets:
             widget.object = obj
         self._obj = obj
 
     @staticmethod
     def on_cls_action_edit(pubsub, topic, value):
         w = SettingsWidget()
```

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/sidebar/__init__.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/sidebar/sidebar_widget.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/sidebar_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,58 +25,61 @@
 
 _DEVICE_TOOLTIP = tooltip_format(
     N_('Device control'),
     N_("""\
     Click to show the device control widget which displays
     the connected devices and their settings.  Use this
     widget to open and close devices and configure their
-    operation.
-    """))
-
-_WIDGETS_TOOLTIP = tooltip_format(
-    N_('Widget settings'),
-    N_("""\
-    Click to show the widget settings which allows you
-    to change the default settings for each widget type.
-    Future widgets you create will use the new defaults.
+    operation.\
     """))
 
 _MEMORY_TOOLTIP = tooltip_format(
     N_('Memory buffer settings'),
     N_("""\
     Streaming signal sample data is stored in your host
     computer's RAM.  Click this button to show the
     memory management widget which allows you to 
-    configure the memory used by this Joulescope UI instance.
+    configure the memory used by this Joulescope UI instance.\
+    """))
+
+_SETTINGS_TOOLTIP = tooltip_format(
+    N_('Settings'),
+    N_("""\
+    Click to show the settings which allows you
+    to change the global, default, and individual
+    instance settings for devices and widgets.
+    
+    Default changes may not affect existing instances,
+    and may only apply to future instances.\
     """))
 
 _HELP_TOOLTIP = tooltip_format(
     N_('Get help'),
     N_("""\
-    Click to display help options.
+    Click to display help options.\
     """))
 
-_SETTINGS_TOOLTIP = tooltip_format(
+_MISC_TOOLTIP = tooltip_format(
     N_('Additional settings and actions'),
     N_("""\
-    Click to display additional settings and actions.
+    Click to display additional settings and actions.\
     """))
 
 
 @register
 @styled_widget(N_('sidebar'))
 class SideBar(QtWidgets.QWidget):
 
     # Note: does NOT implement widget CAPABILITY, since not instantiable by user or available as a dock widget.
 
     SETTINGS = {
         'flyout_width': {
             'dtype': 'int',
             'brief': N_('The flyout width in pixels.'),
-            'default': 250,
+            'default': 300,
         },
     }
 
     def __init__(self, parent):
         self._parent = parent
         super().__init__(parent)
         self.setObjectName('side_bar_icons')
@@ -102,21 +105,22 @@
         b = self._add_blink_button('signal_record', 'signal_stream_record')
         b.toggled.connect(self._on_signal_stream_record_toggled)
         self._add_blink_button('statistics_play', 'statistics_stream_enable')
         b = self._add_blink_button('statistics_record', 'statistics_stream_record')
         b.toggled.connect(self._on_statistics_stream_record_toggled)
         self._add_button('device', _DEVICE_TOOLTIP)
         self._add_button('memory', _MEMORY_TOOLTIP)
-        # todo implement widget settings self._add_button('widgets', _WIDGETS_TOOLTIP)
+        b = self._add_button('settings', _SETTINGS_TOOLTIP)
+        b.clicked.connect(self._on_settings_pressed)
         self._spacer = QtWidgets.QSpacerItem(10, 0,
                                              QtWidgets.QSizePolicy.Minimum,
                                              QtWidgets.QSizePolicy.Expanding)
         self._layout.addItem(self._spacer)
         self._add_button('help', _HELP_TOOLTIP)
-        self._add_button('settings', _SETTINGS_TOOLTIP)
+        self._add_button('misc', _MISC_TOOLTIP)
 
         self.mousePressEvent = self._on_mousePressEvent
         pubsub_singleton.subscribe('registry/ui/events/blink_slow', self._on_blink, ['pub', 'retain'])
 
     def register(self):
         pubsub = pubsub_singleton
         pubsub.register(self, 'sidebar:0', parent='ui')
@@ -138,15 +142,15 @@
         m = HelpWidget()
         pubsub.register(m, 'help_widget:flyout', parent='flyout:0')
         self.widget_set('help', m)
 
         # Create the hamburger flyout widget for the sidebar
         m = HamburgerWidget()
         pubsub.register(m, 'hamburger_widget:flyout', parent='flyout:0')
-        self.widget_set('settings', m)
+        self.widget_set('misc', m)
 
     def _on_mousePressEvent(self, event):
         if event.button() == QtCore.Qt.LeftButton:
             self.on_cmd_show(-1)
             event.accept()
 
     def _on_signal_stream_record_toggled(self, checked):
@@ -157,14 +161,20 @@
 
     def _on_statistics_stream_record_toggled(self, checked):
         if bool(checked):
             pubsub_singleton.publish('registry/StatisticsRecord/actions/!start_request', None)
         else:
             pubsub_singleton.publish('registry/StatisticsRecord/actions/!stop', None)
 
+    def _on_settings_pressed(self, checked):
+        pubsub_singleton.publish('registry/view/actions/!widget_open', {
+            'value': 'registry/settings',
+            'floating': True,
+        })
+
     def _add_blink_button(self, name, app_setting):
         topic = f'registry/app/settings/{app_setting}'
         meta = pubsub_singleton.metadata(topic)
         tooltip = tooltip_format(meta.brief, meta.detail)
         button = self._add_button(name, tooltip)
         button.setProperty('blink', False)
         button.setCheckable(True)
```

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/sidebar/styles/color_scheme_dark.txt` & `joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/color_scheme_dark.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/sidebar/styles/index.json` & `joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/index.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9989795918367348%*

 * *Differences: {"'images'": "{'utilities': {'sources': {insert: [(2, 'memory.svg'), (3, 'misc.svg')], delete: [2, "*

 * *             '1]}}}'}*

```diff
@@ -206,17 +206,17 @@
                     }
                 ]
             ]
         },
         "utilities": {
             "sources": [
                 "device.svg",
-                "widgets.svg",
-                "memory.svg",
                 "help.svg",
+                "memory.svg",
+                "misc.svg",
                 "settings.svg"
             ],
             "targets": [
                 [
                     "{basename}_disabled{ext}",
                     {
                         "#000000": "sidebar.disabled",
```

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/sidebar/styles/style.qss` & `joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/style.qss`

 * *Files 2% similar despite different names*

```diff
@@ -56,21 +56,25 @@
 QPushButton#widgets:enabled       { image: url("{% path %}/widgets_enabled.svg"); }
 QPushButton#widgets:enabled:hover { image: url("{% path %}/widgets_hover.svg"); }
 
 QPushButton#memory:disabled      { image: url("{% path %}/memory_disabled.svg"); }
 QPushButton#memory:enabled       { image: url("{% path %}/memory_enabled.svg"); }
 QPushButton#memory:enabled:hover { image: url("{% path %}/memory_hover.svg"); }
 
+QPushButton#settings:disabled      { image: url("{% path %}/settings_disabled.svg"); }
+QPushButton#settings:enabled       { image: url("{% path %}/settings_enabled.svg"); }
+QPushButton#settings:enabled:hover { image: url("{% path %}/settings_hover.svg"); }
+
 QPushButton#help:disabled      { image: url("{% path %}/help_disabled.svg"); }
 QPushButton#help:enabled       { image: url("{% path %}/help_enabled.svg"); }
 QPushButton#help:enabled:hover { image: url("{% path %}/help_hover.svg"); }
 
-QPushButton#settings:disabled      { image: url("{% path %}/settings_disabled.svg"); }
-QPushButton#settings:enabled       { image: url("{% path %}/settings_enabled.svg"); }
-QPushButton#settings:enabled:hover { image: url("{% path %}/settings_hover.svg"); }
+QPushButton#misc:disabled      { image: url("{% path %}/misc_disabled.svg"); }
+QPushButton#misc:enabled       { image: url("{% path %}/misc_enabled.svg"); }
+QPushButton#misc:enabled:hover { image: url("{% path %}/misc_hover.svg"); }
 
 /****************************************************************************/
 /* Target Power toggle button                                               */
 /****************************************************************************/
 QPushButton#target_power[blink=false]:disabled     { image: url("{% path %}/target_power_disabled_0.svg"); }
 QPushButton#target_power[blink=true]:disabled      { image: url("{% path %}/target_power_disabled_1.svg"); }
 QPushButton#target_power[blink=false]:enabled      { image: url("{% path %}/target_power_off_0.svg"); }
```

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/signal_record/__init__.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/signal_record/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/signal_record/signal_record.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/signal_record/signal_record.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/signal_record/signal_record_config_widget.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/signal_record/signal_record_config_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/statistics_record/__init__.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/statistics_record/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/statistics_record/statistics_record.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/statistics_record/statistics_record.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/statistics_record/statistics_record_config_widget.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/statistics_record/statistics_record_config_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/switch.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/switch.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/value/__init__.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/value/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/value/value_widget.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/value/value_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from PySide6 import QtWidgets, QtGui, QtCore
 from joulescope_ui import CAPABILITIES, register, pubsub_singleton, N_, get_topic_name, tooltip_format
 from joulescope_ui.widget_tools import settings_action_create
 from joulescope_ui.styles import styled_widget, color_as_qcolor, font_as_qfont
-from joulescope_ui.units import unit_prefix, three_sig_figs
+from joulescope_ui.units import UNITS_SETTING, convert_units, unit_prefix, three_sig_figs
 from joulescope_ui.ui_util import comboBoxConfig
 import datetime
 import numpy as np
 import copy
 import logging
 
 
@@ -51,14 +51,15 @@
         'default': True,
     },
     'show_titles': {
         'dtype': 'bool',
         'brief': N_('Show the statistics section title for each signal.'),
         'default': True,
     },
+    'units': UNITS_SETTING,
 }
 
 def _settings_alter(**kwargs):
     d = copy.deepcopy(SETTINGS)
     for key, default in kwargs.items():
         d[key]['default'] = default
     return d
@@ -376,16 +377,15 @@
             painter.setPen(main_color)
             painter.setFont(main_font)
             y += main_font_metrics.ascent() + (y_signal - title_height - main_font_metrics.height()) // 2
 
             if signal_name in self._statistics['accumulators']:
                 signal = self._statistics['accumulators'][signal_name]
                 fields = ['accumulate_duration']
-                signal_value = signal['value']
-                signal_units = signal['units']
+                signal_value, signal_units = convert_units(signal['value'], signal['units'], self._parent.units)
                 _, prefix, scale = unit_prefix(signal_value)
             else:
                 signal = self._statistics['signals'][signal_name]
                 fields = fields if parent.show_fields else []
                 fields_all = [self._main] + fields
                 max_value = max([abs(signal[s]['value']) for s in fields_all])
                 _, prefix, scale = unit_prefix(max_value)
```

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/waveform/__init__.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/waveform/line_segments.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/line_segments.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/waveform/styles/color_scheme_dark.txt` & `joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/color_scheme_dark.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/waveform/styles/index.json` & `joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/waveform/styles/style.qss` & `joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/waveform/styles/y_zoom_all.svg` & `joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/y_zoom_all.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/waveform/styles/zoom_all.svg` & `joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/zoom_all.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/waveform/waveform_control.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/waveform_control.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.7/joulescope_ui/widgets/waveform/waveform_widget.py` & `joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/waveform_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,26 +11,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from PySide6 import QtWidgets, QtGui, QtCore, QtOpenGLWidgets, QtOpenGL
 from OpenGL import GL as gl
 from joulescope_ui import CAPABILITIES, register, pubsub_singleton, N_, get_topic_name, get_instance, time64
+from joulescope_ui.shortcuts import Shortcuts
 from joulescope_ui.styles import styled_widget, color_as_qcolor, font_as_qfont
 from joulescope_ui.widget_tools import settings_action_create
 from .line_segments import PointsF
 from .waveform_control import WaveformControlWidget
 from joulescope_ui.time_map import TimeMap
 import copy
 import logging
 import numpy as np
 import os
 import time
 from PySide6.QtGui import QPen, QBrush
-from joulescope_ui.units import unit_prefix
+from joulescope_ui.units import convert_units, UNITS_SETTING, unit_prefix
 from collections.abc import Iterable
 
 
 _NAME = N_('Waveform')
 _ZOOM_FACTOR = np.sqrt(2)
 _WHEEL_TO_DEGREES = 1.0 / 8.0  # https://doc.qt.io/qt-6/qwheelevent.html#angleDelta
 _WHEEL_TICK_DEGREES = 15.0   # Standard convention
@@ -390,15 +391,15 @@
             'brief': N_('The source filter string.'),
             'default': 'JsdrvStreamBuffer:001',
         },
         'on_widget_close_actions': {
             'dtype': 'obj',
             'brief': 'The list of [topic, value] to perform on widget close.',
             'default': [],
-            'flags': ['hidden', 'ro'],
+            'flags': ['hide', 'ro'],
         },
         'trace_width': {
             'dtype': 'int',
             'brief': N_('The trace width.'),
             'default': 1,
         },
         'fps': {
@@ -438,15 +439,15 @@
             'brief': N_('Show the plot statistics on the right.'),
             'default': True,
         },
         'x_range': {
             'dtype': 'obj',
             'brief': 'The x-axis range.',
             'default': [0, 0],
-            'flags': ['hidden', 'ro', 'skip_undo'],  # publish only
+            'flags': ['hide', 'ro', 'skip_undo'],  # publish only
         },
         'pin_left': {
             'dtype': 'bool',
             'brief': N_('Pin the left side (oldest) data so that it stays in view.'),
             'default': True,
         },
         'pin_right': {
@@ -454,15 +455,15 @@
             'brief': N_('Pin the right side (newest) data so that it stays in view.'),
             'default': True,
         },
         'state': {
             'dtype': 'obj',
             'brief': N_('The waveform state.'),
             'default': None,
-            'flags': ['hidden', 'ro'],
+            'flags': ['hide', 'ro'],
         },
         'control_location': {
             'dtype': 'str',
             'brief': N_('Control location'),
             'default': 'bottom',
             'options': [
                 ['off', N_('off')],
@@ -470,15 +471,16 @@
                 ['bottom', N_('bottom')],
             ],
         },
         'summary_signal': {
             'dtype': 'obj',
             'brief': N_('The signal to show in the summary.'),
             'default': None,
-        }
+        },
+        'units': UNITS_SETTING,
     }
 
     def __init__(self, parent=None, **kwargs):
         """Create a new instance.
 
         :param parent: The QtWidget parent.
         :param source_filter: The source filter string.
@@ -502,14 +504,15 @@
 
         self._on_source_list_fn = self._on_source_list
         self._on_signal_add_fn = self._on_signal_add
         self._on_signal_remove_fn = self._on_signal_remove
         self._on_signal_range_fn = self._on_signal_range
         self._menu = None
         self._dialog = None
+        self._shortcuts = Shortcuts(self)
         self._x_map = TimeMap()
         self._x_summary_map = TimeMap()
         self._mouse_pos = None
         self._mouse_pos_start = None
         self._wheel_accum_degrees = np.zeros(2, dtype=np.float64)
         self._margin = _MARGIN
 
@@ -534,16 +537,18 @@
 
         self._refresh_timer = QtCore.QTimer()
         self._refresh_timer.setTimerType(QtGui.Qt.PreciseTimer)
         self._refresh_timer.timeout.connect(self._on_refresh_timer)
         self._repaint_request = False
         self._fps = {
             'start': time.time(),
+            'thread_durations': [],
+            'time_durations': [],
             'times': [],
-            'str': '',
+            'str': [],
         }
 
     def on_setting_control_location(self, value):
         if value == 'off':
             self._control.setVisible(False)
             return
         self._layout.removeWidget(self._control)
@@ -646,20 +651,34 @@
                 plot['y_markers'] = []
         self.pubsub.subscribe('registry_manager/capabilities/signal_buffer.source/list',
                               self._on_source_list_fn, ['pub', 'retain'])
         topic = get_topic_name(self)
         self._control.on_pubsub_register(self.pubsub, topic, source_filter)
         for m in self.state['x_markers']:
             self._x_markers_by_id[m['id']] = m
+        self._shortcuts_add()
+
+    def _shortcuts_add(self):
+        topic = get_topic_name(self)
+        self._shortcuts.add(QtCore.Qt.Key_Asterisk, f'{topic}/actions/!x_zoom_all')
+        # self._shortcuts.add(QtCore.Qt.Key_Delete,  # clear annotations
+        # self._shortcuts.add(QtCore.Qt.Key_Backspace, # clear annotations
+        self._shortcuts.add(QtCore.Qt.Key_Left, f'{topic}/actions/!x_pan', -1)
+        self._shortcuts.add(QtCore.Qt.Key_Right, f'{topic}/actions/!x_pan', 1)
+        self._shortcuts.add(QtCore.Qt.Key_Up, f'{topic}/actions/!x_zoom', [1, None])
+        self._shortcuts.add(QtCore.Qt.Key_Down, f'{topic}/actions/!x_zoom', [-1, None])
+        self._shortcuts.add(QtCore.Qt.Key_Plus, f'{topic}/actions/!x_zoom', [1, None])
+        self._shortcuts.add(QtCore.Qt.Key_Minus, f'{topic}/actions/!x_zoom', [-1, None])
 
     def _cleanup(self):
         self.pubsub.unsubscribe_all(self._on_source_list_fn)
         self.pubsub.unsubscribe_all(self._on_signal_range_fn)
         self.pubsub.unsubscribe_all(self._on_signal_add)
         self.pubsub.unsubscribe_all(self._on_signal_remove)
+        self._shortcuts.clear()
         self._refresh_timer.stop()
 
     def on_pubsub_unregister(self):
         self._control.on_pubsub_unregister()
         self._cleanup()
 
     def closeEvent(self, event):
@@ -667,27 +686,37 @@
         return super().closeEvent(event)
 
     def on_widget_close(self):
         for topic, value in self.pubsub.query(f'{self.topic}/settings/on_widget_close_actions', default=[]):
             self._log.info('waveform close: %s %s', topic, value)
             self.pubsub.publish(topic, value)
 
-    def _update_fps(self):
+    def _update_fps(self, thread_duration, time_duration):
         t = time.time()
         self._fps['times'].append(t)
+        self._fps['thread_durations'].append(thread_duration)
+        self._fps['time_durations'].append(time_duration)
         if t - self._fps['start'] >= 1.0:
             x = np.array(self._fps['times'])
             x = np.diff(x)
+            d1 = np.array(self._fps['thread_durations'])
+            d2 = np.array(self._fps['time_durations'])
             self._fps['start'] = t
             self._fps['times'].clear()
+            self._fps['thread_durations'].clear()
+            self._fps['time_durations'].clear()
+            self._fps['str'].clear()
             if len(x):
-                t_avg = np.mean(x)
-                t_min = np.min(x)
-                t_max = np.max(x)
-                self._fps['str'] = f'{1/t_avg:.2f} Hz (min={t_min*1000:.2f}, max={t_max*1000:.2f} ms)'
+                self._fps['str'].append(f'{1 / np.mean(x):.2f} fps')
+            for name, v in [('interval', x), ('thread_duration', d1), ('time_duration', d2)]:
+                if not len(v):
+                    continue
+                v *= 1000  # convert from seconds to milliseconds
+                v_avg, v_min, v_max = np.mean(v), np.min(v), np.max(v)
+                self._fps['str'].append(f'{name} avg={v_avg:.2f}, min={v_min:.2f}, max={v_max:.2f} ms')
         return None
 
     def _on_signal_range(self, topic, value):
         # self._log.info('_on_signal_range(%s, %s)', topic, value)
         if value is None:
             return
         value = value['utc']
@@ -1201,14 +1230,16 @@
 
         :param p: The QPainter instance.
         :param size: The (width, height) for the plot area.
         """
         s = self._style
         if s is None:
             return
+        t_thread_start = time.thread_time_ns()
+        t_time_start = time.time_ns()
         self._repaint_request = False
 
         resize = not len(self._y_geometry_info)
         self._compute_geometry(size)
         if resize:
             self._plots_height_adjust()
         self._draw_background(p, size)
@@ -1220,18 +1251,22 @@
         # Draw each plot
         for plot in self.state['plots']:
             if plot['enabled']:
                 self._draw_plot(p, plot)
                 self._draw_plot_statistics(p, plot)
         self._draw_spacers(p)
         self._draw_markers(p, size)
-        self._draw_fps(p)
         self._draw_hover(p)
         self._set_cursor()
 
+        thread_duration = (time.thread_time_ns() - t_thread_start) / 1e9
+        time_duration = (time.time_ns() - t_time_start) / 1e9
+        self._update_fps(thread_duration, time_duration)
+        self._draw_fps(p, )
+
     def _draw_background(self, p, size):
         s = self._style
         widget_w, widget_h = size
         p.fillRect(0, 0, widget_w, widget_h, s['background_brush'])
 
     def _summary_geometry(self):
         _, _, x0 = self._x_geometry_info['margin.left']
@@ -1749,29 +1784,33 @@
             labels = ['avg', 'std', 'rms', 'min', 'max', 'p2p']
             v_rms = np.sqrt(v_avg * v_avg + v_std * v_std)
             values = [v_avg, v_std, v_rms, v_min, v_max, v_max - v_min]
             values = _statistics_format(labels, values, plot['units'])
 
             integral_units = plot.get('integral')
             if integral_units is not None:
-                integral_values = _statistics_format(['∫'], [v_avg * dt], integral_units)
+                integral_v, integral_units = convert_units(v_avg * dt, integral_units, self.units)
+                integral_values = _statistics_format(['∫'], [integral_v], integral_units)
                 values.extend(integral_values)
 
             pos_field = text_pos_key.split('_')[-1]
             p0 = np.rint(self._x_map.time64_to_counter(m[pos_field]))
             self._draw_statistics_text(p, (p0, y0), values, text_pos)
         p.setClipping(False)
 
     def _draw_fps(self, p):
         s = self._style
-        self._update_fps()
         if self.show_fps:
             p.setFont(s['axis_font'])
             p.setPen(s['text_pen'])
-            p.drawText(10, s['axis_font_metrics'].ascent(), self._fps['str'])
+            y = s['axis_font_metrics'].ascent()
+            y_incr = s['axis_font_metrics'].height()
+            for s in self._fps['str']:
+                p.drawText(10, y, s)
+                y += y_incr
 
     def _signal_data_get(self, plot):
         try:
             if isinstance(plot, str):
                 plot_idx = int(plot.split('.')[1])
                 plot = self.state['plots'][plot_idx]
             signals = plot['signals']
@@ -1878,15 +1917,16 @@
         q_names = ['avg', 'std', 'rms', 'min', 'max', 'p2p']
         q_value = [y_avg, y_std, y_rms, y_min, y_max, y_max - y_min]
         values = _statistics_format(q_names, q_value, plot['units'])
 
         dt = (z1 - z0) / time64.SECOND
         integral_units = plot.get('integral')
         if integral_units is not None:
-            integral_values = _statistics_format(['∫'], [y_avg * dt], integral_units)
+            integral_v, integral_units = convert_units(y_avg * dt, integral_units, self.units)
+            integral_values = _statistics_format(['∫'], [integral_v], integral_units)
             values.extend(integral_values)
         p.setClipRect(x0, y0, xd, yd)
         self._draw_statistics_text(p, (x0, y0), values)
         p.setClipping(False)
 
     def _target_lookup_by_pos(self, pos):
         """Get the target object.
@@ -2855,16 +2895,16 @@
     def on_action_x_zoom_all(self):
         """Perform a zoom action to the full extents.
         """
         self._log.info('x_zoom_all')
         self._plot_data_invalidate()
         self.x_range = self._extents()
 
-    def _on_x_pan(self, pan):
-        self._log.info(f'_on_x_pan {pan}')
+    def on_action_x_pan(self, pan):
+        self._log.info(f'on_action_x_pan {pan}')
         if self.pin_left or self.pin_right:
             return  # locked to extents
         e0, e1 = self._extents()
         x0, x1 = self.x_range
         d_x = x1 - x0
         p = int(d_x * 0.25 * pan)
         z0, z1 = x0 + p, x1 + p
@@ -2933,22 +2973,22 @@
         if x_delta and not y_delta:
             delta = x_delta
             is_pan = True
         is_y = QtCore.Qt.KeyboardModifier.ControlModifier & event.modifiers()
 
         if y_name == 'summary':
             if is_pan:
-                self._on_x_pan(delta)
+                self.on_action_x_pan(delta)
             else:
                 t = (self.x_range[0] + self.x_range[1]) / 2
                 topic = get_topic_name(self)
                 self.pubsub.publish(f'{topic}/actions/!x_zoom', [delta, t])
         if x_name == 'plot' and (y_name == 'x_axis' or not is_y):
             if is_pan:
-                self._on_x_pan(delta)
+                self.on_action_x_pan(delta)
             else:
                 t = self._x_map.counter_to_time64(self._mouse_pos[0])
                 topic = get_topic_name(self)
                 self.pubsub.publish(f'{topic}/actions/!x_zoom', [delta, t, self._mouse_pos[0]])
         elif y_name.startswith('plot.') and (is_y or x_name == 'y_axis'):
             plot_idx = int(y_name.split('.')[1])
             plot = self.state['plots'][plot_idx]
```

### Comparing `joulescope_ui-1.0.7/joulescope_ui.egg-info/PKG-INFO` & `joulescope_ui-1.0.8/joulescope_ui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joulescope-ui
-Version: 1.0.7
+Version: 1.0.8
 Summary: Joulescope™ graphical user interface
 Home-page: https://www.joulescope.com
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/pyjoulescope_ui/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `joulescope_ui-1.0.7/joulescope_ui.egg-info/SOURCES.txt` & `joulescope_ui-1.0.8/joulescope_ui.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 joulescope_ui/process_monitor.py
 joulescope_ui/profile.py
 joulescope_ui/pubsub.py
 joulescope_ui/range_tool.py
 joulescope_ui/resources.py
 joulescope_ui/resources.rcc
 joulescope_ui/sanitize.py
+joulescope_ui/shortcuts.py
 joulescope_ui/software_update.py
 joulescope_ui/time_map.py
 joulescope_ui/tooltip.py
 joulescope_ui/ui_util.py
 joulescope_ui/units.py
 joulescope_ui/version.py
 joulescope_ui/view.py
@@ -133,14 +134,21 @@
 joulescope_ui/test/test_sanitize.py
 joulescope_ui/test/test_software_update.py
 joulescope_ui/test/test_time_map.py
 joulescope_ui/test/test_tooltip.py
 joulescope_ui/test/test_units.py
 joulescope_ui/widgets/__init__.py
 joulescope_ui/widgets/switch.py
+joulescope_ui/widgets/accumulator/__init__.py
+joulescope_ui/widgets/accumulator/accumulator_widget.py
+joulescope_ui/widgets/accumulator/styles/color_scheme_dark.txt
+joulescope_ui/widgets/accumulator/styles/color_scheme_light.txt
+joulescope_ui/widgets/accumulator/styles/font_scheme_js1.txt
+joulescope_ui/widgets/accumulator/styles/index.json
+joulescope_ui/widgets/accumulator/styles/style.qss
 joulescope_ui/widgets/device_control/__init__.py
 joulescope_ui/widgets/device_control/device_control_widget.py
 joulescope_ui/widgets/device_control/device_info_dialog.py
 joulescope_ui/widgets/device_control/js220_ctrl_widget.py
 joulescope_ui/widgets/device_control/styles/active_checked.svg
 joulescope_ui/widgets/device_control/styles/active_unchecked.svg
 joulescope_ui/widgets/device_control/styles/closed.svg
@@ -183,22 +191,22 @@
 joulescope_ui/widgets/sidebar/sidebar_widget.py
 joulescope_ui/widgets/sidebar/styles/color_scheme_dark.txt
 joulescope_ui/widgets/sidebar/styles/color_scheme_light.txt
 joulescope_ui/widgets/sidebar/styles/device.svg
 joulescope_ui/widgets/sidebar/styles/help.svg
 joulescope_ui/widgets/sidebar/styles/index.json
 joulescope_ui/widgets/sidebar/styles/memory.svg
+joulescope_ui/widgets/sidebar/styles/misc.svg
 joulescope_ui/widgets/sidebar/styles/pause.svg
 joulescope_ui/widgets/sidebar/styles/play.svg
 joulescope_ui/widgets/sidebar/styles/record.svg
 joulescope_ui/widgets/sidebar/styles/settings.svg
 joulescope_ui/widgets/sidebar/styles/stop.svg
 joulescope_ui/widgets/sidebar/styles/style.qss
 joulescope_ui/widgets/sidebar/styles/target_power.svg
-joulescope_ui/widgets/sidebar/styles/widgets.svg
 joulescope_ui/widgets/signal_record/__init__.py
 joulescope_ui/widgets/signal_record/signal_record.py
 joulescope_ui/widgets/signal_record/signal_record_config_widget.py
 joulescope_ui/widgets/statistics_record/__init__.py
 joulescope_ui/widgets/statistics_record/statistics_record.py
 joulescope_ui/widgets/statistics_record/statistics_record_config_widget.py
 joulescope_ui/widgets/value/__init__.py
```

### Comparing `joulescope_ui-1.0.7/setup.py` & `joulescope_ui-1.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 import os
 import platform
 import sys
 import subprocess
 import shutil
 
 
-JOULESCOPE_DRIVER_VERSION_MIN = '1.3.1'  # also update requirements.txt
-JOULESCOPE_VERSION_MIN = '1.1.2'         # also update requirements.txt
+JOULESCOPE_DRIVER_VERSION_MIN = '1.3.2'  # also update requirements.txt
+JOULESCOPE_VERSION_MIN = '1.1.3'         # also update requirements.txt
 MYPATH = os.path.abspath(os.path.dirname(__file__))
 VERSION_PATH = os.path.join(MYPATH, 'joulescope_ui', 'version.py')
 
 
 def qt_rcc_path():
     # As of PySide 5.15.0, the pySide6-rcc executable ignores the --binary flag
     import PySide6
```

