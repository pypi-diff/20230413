# Comparing `tmp/srsgui-0.2.13.tar.gz` & `tmp/srsgui-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-mct1_sdo\srsgui-0.2.13.tar", last modified: Thu Apr 13 18:46:13 2023, max compression
+gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-ps3u1u8m\srsgui-0.2.9.tar", last modified: Tue Apr 11 21:39:00 2023, max compression
```

## Comparing `srsgui-0.2.13.tar` & `srsgui-0.2.9.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 18:46:13.365623 srsgui-0.2.13/
--rw-rw-rw-   0        0        0     1345 2022-08-02 00:19:43.000000 srsgui-0.2.13/.gitignore
--rw-rw-rw-   0        0        0     1107 2022-12-07 23:27:48.000000 srsgui-0.2.13/LICENSE.txt
--rw-rw-rw-   0        0        0     3331 2023-04-13 18:46:13.365623 srsgui-0.2.13/PKG-INFO
--rw-rw-rw-   0        0        0     2633 2023-02-13 17:17:13.000000 srsgui-0.2.13/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 18:46:13.265640 srsgui-0.2.13/docs/
--rw-rw-rw-   0        0        0      658 2023-01-30 16:55:49.000000 srsgui-0.2.13/docs/Makefile
--rwxrwxrwx   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.13/docs/autodoc.bat
--rwxrwxrwx   0        0        0      804 2023-01-30 16:55:49.000000 srsgui-0.2.13/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-04-13 18:46:13.285662 srsgui-0.2.13/docs/source/
-drwxrwxrwx   0        0        0        0 2023-04-13 18:46:13.295629 srsgui-0.2.13/docs/source/_static/
--rw-rw-rw-   0        0        0    31067 2023-01-30 16:55:49.000000 srsgui-0.2.13/docs/source/_static/cg-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    27242 2023-01-30 16:55:49.000000 srsgui-0.2.13/docs/source/_static/cg-terminal-screen-capture.png
--rw-rw-rw-   0        0        0     5762 2023-01-30 16:55:49.000000 srsgui-0.2.13/docs/source/_static/connect-dialog-box-capture.png
--rw-rw-rw-   0        0        0    71070 2023-01-30 16:55:49.000000 srsgui-0.2.13/docs/source/_static/example-screen-capture-1.png
--rw-rw-rw-   0        0        0    71011 2023-01-30 16:55:49.000000 srsgui-0.2.13/docs/source/_static/example-screen-capture-2.png
--rw-rw-rw-   0        0        0    56013 2023-01-30 16:55:49.000000 srsgui-0.2.13/docs/source/_static/initial-screen-capture.png
--rw-rw-rw-   0        0        0    29667 2023-01-30 16:55:49.000000 srsgui-0.2.13/docs/source/_static/osc-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    50740 2023-01-30 16:55:49.000000 srsgui-0.2.13/docs/source/_static/second-task-screen-capture.png
--rw-rw-rw-   0        0        0    39412 2023-01-30 16:55:49.000000 srsgui-0.2.13/docs/source/_static/terminal-with-example-2.png
--rw-rw-rw-   0        0        0    37573 2023-01-30 16:55:49.000000 srsgui-0.2.13/docs/source/_static/terminal-with-example.png
--rw-rw-rw-   0        0        0     1938 2023-01-30 16:55:49.000000 srsgui-0.2.13/docs/source/conf.py
--rw-rw-rw-   0        0        0     5998 2023-04-04 20:33:11.000000 srsgui-0.2.13/docs/source/create-project.rst
--rw-rw-rw-   0        0        0     6656 2023-04-04 20:33:11.000000 srsgui-0.2.13/docs/source/create-task.rst
--rw-rw-rw-   0        0        0     6110 2023-04-04 20:33:11.000000 srsgui-0.2.13/docs/source/define-instrument.rst
--rw-rw-rw-   0        0        0    15655 2023-04-04 20:33:11.000000 srsgui-0.2.13/docs/source/example.rst
--rw-rw-rw-   0        0        0     3684 2023-04-04 20:33:11.000000 srsgui-0.2.13/docs/source/index.rst
--rw-rw-rw-   0        0        0     4383 2023-04-04 20:33:11.000000 srsgui-0.2.13/docs/source/installation.rst
--rw-rw-rw-   0        0        0      936 2023-01-30 16:55:49.000000 srsgui-0.2.13/docs/source/srsgui.inst.communications.rst
--rw-rw-rw-   0        0        0      950 2023-01-30 16:55:49.000000 srsgui-0.2.13/docs/source/srsgui.inst.rst
--rw-rw-rw-   0        0        0      117 2023-01-30 16:55:49.000000 srsgui-0.2.13/docs/source/srsgui.rst
--rw-rw-rw-   0        0        0      989 2023-01-30 16:55:49.000000 srsgui-0.2.13/docs/source/srsgui.task.rst
--rw-rw-rw-   0        0        0      604 2023-01-30 16:55:49.000000 srsgui-0.2.13/docs/source/srsgui.ui.qt.rst
--rw-rw-rw-   0        0        0     1629 2023-01-30 16:55:49.000000 srsgui-0.2.13/docs/source/srsgui.ui.rst
--rw-rw-rw-   0        0        0     1193 2023-04-07 01:13:40.000000 srsgui-0.2.13/pyproject.toml
--rw-rw-rw-   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.13/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 18:46:13.365623 srsgui-0.2.13/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsgui-0.2.13/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:46:13.295629 srsgui-0.2.13/srsgui/
--rw-rw-rw-   0        0        0     1538 2023-04-13 18:42:42.000000 srsgui-0.2.13/srsgui/__init__.py
--rw-rw-rw-   0        0        0      314 2023-04-07 00:52:02.000000 srsgui-0.2.13/srsgui/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:46:13.251369 srsgui-0.2.13/srsgui/examples/
-drwxrwxrwx   0        0        0        0 2023-04-13 18:46:13.305623 srsgui-0.2.13/srsgui/examples/oscilloscope example/
-drwxrwxrwx   0        0        0        0 2023-04-13 18:46:13.305623 srsgui-0.2.13/srsgui/examples/oscilloscope example/instruments/
--rw-rw-rw-   0        0        0     1709 2023-01-30 16:55:49.000000 srsgui-0.2.13/srsgui/examples/oscilloscope example/instruments/cg635.py
--rw-rw-rw-   0        0        0     3025 2023-02-11 01:21:41.000000 srsgui-0.2.13/srsgui/examples/oscilloscope example/instruments/sds1202.py
--rw-rw-rw-   0        0        0     1977 2023-01-30 16:55:49.000000 srsgui-0.2.13/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
-drwxrwxrwx   0        0        0        0 2023-04-13 18:46:13.315618 srsgui-0.2.13/srsgui/examples/oscilloscope example/tasks/
--rw-rw-rw-   0        0        0     2401 2023-01-30 16:55:49.000000 srsgui-0.2.13/srsgui/examples/oscilloscope example/tasks/fifth.py
--rw-rw-rw-   0        0        0     1543 2023-01-30 16:55:49.000000 srsgui-0.2.13/srsgui/examples/oscilloscope example/tasks/first.py
--rw-rw-rw-   0        0        0     3978 2023-01-30 16:55:49.000000 srsgui-0.2.13/srsgui/examples/oscilloscope example/tasks/fourth.py
--rw-rw-rw-   0        0        0     2129 2023-01-30 16:55:49.000000 srsgui-0.2.13/srsgui/examples/oscilloscope example/tasks/second.py
--rw-rw-rw-   0        0        0     1893 2023-01-30 16:55:49.000000 srsgui-0.2.13/srsgui/examples/oscilloscope example/tasks/third.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:46:13.325639 srsgui-0.2.13/srsgui/inst/
--rw-rw-rw-   0        0        0     1074 2023-04-04 20:33:11.000000 srsgui-0.2.13/srsgui/inst/__init__.py
--rw-rw-rw-   0        0        0     9573 2023-04-13 16:02:21.000000 srsgui-0.2.13/srsgui/inst/commands.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:46:13.335636 srsgui-0.2.13/srsgui/inst/communications/
--rw-rw-rw-   0        0        0      126 2023-01-30 16:55:49.000000 srsgui-0.2.13/srsgui/inst/communications/__init__.py
--rw-rw-rw-   0        0        0     7903 2023-01-30 16:55:49.000000 srsgui-0.2.13/srsgui/inst/communications/interface.py
--rw-rw-rw-   0        0        0     1157 2023-01-30 16:55:49.000000 srsgui-0.2.13/srsgui/inst/communications/serial_ports.py
--rw-rw-rw-   0        0        0     8097 2023-01-30 16:55:49.000000 srsgui-0.2.13/srsgui/inst/communications/serialinterface.py
--rw-rw-rw-   0        0        0    10762 2023-01-30 16:55:49.000000 srsgui-0.2.13/srsgui/inst/communications/tcpipinterface.py
--rw-rw-rw-   0        0        0    14665 2023-04-11 20:13:55.000000 srsgui-0.2.13/srsgui/inst/component.py
--rw-rw-rw-   0        0        0      727 2023-01-30 16:55:49.000000 srsgui-0.2.13/srsgui/inst/exceptions.py
--rw-rw-rw-   0        0        0    10050 2023-04-13 16:23:13.000000 srsgui-0.2.13/srsgui/inst/indexcommands.py
--rw-rw-rw-   0        0        0     9647 2023-02-09 17:58:55.000000 srsgui-0.2.13/srsgui/inst/instrument.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:46:13.335636 srsgui-0.2.13/srsgui/task/
--rw-rw-rw-   0        0        0        2 2023-04-10 22:51:26.000000 srsgui-0.2.13/srsgui/task/__init__.py
--rw-rw-rw-   0        0        0      692 2023-01-30 16:55:49.000000 srsgui-0.2.13/srsgui/task/callbacks.py
--rw-rw-rw-   0        0        0     6485 2023-04-07 01:13:40.000000 srsgui-0.2.13/srsgui/task/config.py
--rw-rw-rw-   0        0        0     5203 2023-04-11 00:24:36.000000 srsgui-0.2.13/srsgui/task/inputs.py
--rw-rw-rw-   0        0        0     6865 2023-03-28 15:59:44.000000 srsgui-0.2.13/srsgui/task/sessionhandler.py
--rw-rw-rw-   0        0        0    22248 2023-04-12 21:42:04.000000 srsgui-0.2.13/srsgui/task/task.py
--rw-rw-rw-   0        0        0     4108 2023-01-30 16:55:49.000000 srsgui-0.2.13/srsgui/task/taskresult.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:46:13.355620 srsgui-0.2.13/srsgui/ui/
--rw-rw-rw-   0        0        0        0 2023-01-30 16:55:49.000000 srsgui-0.2.13/srsgui/ui/__init__.py
--rw-rw-rw-   0        0        0     3775 2023-04-04 20:33:12.000000 srsgui-0.2.13/srsgui/ui/commandhandler.py
--rw-rw-rw-   0        0        0     5918 2023-04-04 20:33:12.000000 srsgui-0.2.13/srsgui/ui/commandterminal.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:46:13.365623 srsgui-0.2.13/srsgui/ui/commandtree/
--rw-rw-rw-   0        0        0     2919 2023-04-07 19:57:55.000000 srsgui-0.2.13/srsgui/ui/commandtree/commandcapturewidget.py
--rw-rw-rw-   0        0        0     3362 2023-04-10 22:51:26.000000 srsgui-0.2.13/srsgui/ui/commandtree/commandcapturewidget.ui
--rw-rw-rw-   0        0        0     3633 2023-04-13 17:29:00.000000 srsgui-0.2.13/srsgui/ui/commandtree/commanddelegate.py
--rw-rw-rw-   0        0        0    10412 2023-04-13 16:31:48.000000 srsgui-0.2.13/srsgui/ui/commandtree/commanditem.py
--rw-rw-rw-   0        0        0     7255 2023-04-13 16:18:11.000000 srsgui-0.2.13/srsgui/ui/commandtree/commandmodel.py
--rw-rw-rw-   0        0        0     4790 2023-04-13 17:26:11.000000 srsgui-0.2.13/srsgui/ui/commandtree/commandspinbox.py
--rw-rw-rw-   0        0        0     3331 2023-04-12 19:07:11.000000 srsgui-0.2.13/srsgui/ui/commandtree/commandtreeview.py
--rw-rw-rw-   0        0        0     3837 2023-04-13 16:29:07.000000 srsgui-0.2.13/srsgui/ui/commandtree/commandtreewidget.py
--rw-rw-rw-   0        0        0     9296 2023-04-07 19:57:55.000000 srsgui-0.2.13/srsgui/ui/commandtree/jsonmodel.py
--rw-rw-rw-   0        0        0     4803 2023-04-10 22:51:26.000000 srsgui-0.2.13/srsgui/ui/commandtree/ui_commandcapturewidget.py
--rw-rw-rw-   0        0        0     4806 2023-04-11 17:35:42.000000 srsgui-0.2.13/srsgui/ui/commandtree/ui_commandtreewidget.py
--rw-rw-rw-   0        0        0     9679 2023-04-07 01:13:40.000000 srsgui-0.2.13/srsgui/ui/connectdlg.py
--rw-rw-rw-   0        0        0     3856 2023-04-04 20:33:12.000000 srsgui-0.2.13/srsgui/ui/deviceinfohandler.py
--rw-rw-rw-   0        0        0    14127 2023-04-07 19:57:55.000000 srsgui-0.2.13/srsgui/ui/dockhandler.py
--rw-rw-rw-   0        0        0    13671 2023-04-11 00:24:36.000000 srsgui-0.2.13/srsgui/ui/inputpanel.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:46:13.365623 srsgui-0.2.13/srsgui/ui/qt/
--rw-rw-rw-   0        0        0      678 2023-01-30 16:55:49.000000 srsgui-0.2.13/srsgui/ui/qt/QtCore.py
--rw-rw-rw-   0        0        0      556 2023-01-30 16:55:49.000000 srsgui-0.2.13/srsgui/ui/qt/QtGui.py
--rw-rw-rw-   0        0        0      656 2023-01-30 16:55:49.000000 srsgui-0.2.13/srsgui/ui/qt/QtWidgets.py
--rw-rw-rw-   0        0        0     1457 2023-03-08 01:32:20.000000 srsgui-0.2.13/srsgui/ui/qt/__init__.py
--rw-rw-rw-   0        0        0     1164 2023-01-30 16:55:49.000000 srsgui-0.2.13/srsgui/ui/qtloghandler.py
--rw-rw-rw-   0        0        0      268 2023-01-30 16:55:49.000000 srsgui-0.2.13/srsgui/ui/resource.qrc
--rw-rw-rw-   0        0        0    15358 2023-01-30 16:55:49.000000 srsgui-0.2.13/srsgui/ui/resource_rc.py
--rw-rw-rw-   0        0        0     2598 2023-01-30 16:55:49.000000 srsgui-0.2.13/srsgui/ui/signalhandler.py
--rw-rw-rw-   0        0        0    47891 2023-01-30 16:55:49.000000 srsgui-0.2.13/srsgui/ui/srslogo.jpg
--rw-rw-rw-   0        0        0      886 2023-01-30 16:55:49.000000 srsgui-0.2.13/srsgui/ui/stdout.py
--rw-rw-rw-   0        0        0    24758 2023-04-10 15:41:10.000000 srsgui-0.2.13/srsgui/ui/taskmain.py
--rw-rw-rw-   0        0        0    10403 2023-02-22 17:26:46.000000 srsgui-0.2.13/srsgui/ui/taskmain.ui
--rw-rw-rw-   0        0        0    11293 2023-02-22 17:26:46.000000 srsgui-0.2.13/srsgui/ui/ui_taskmain.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:46:13.305623 srsgui-0.2.13/srsgui.egg-info/
--rw-rw-rw-   0        0        0     3331 2023-04-13 18:46:13.000000 srsgui-0.2.13/srsgui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3162 2023-04-13 18:46:13.000000 srsgui-0.2.13/srsgui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 18:46:13.000000 srsgui-0.2.13/srsgui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-13 18:46:13.000000 srsgui-0.2.13/srsgui.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       53 2023-04-13 18:46:13.000000 srsgui-0.2.13/srsgui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-13 18:46:13.000000 srsgui-0.2.13/srsgui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.979862 srsgui-0.2.9/
+-rw-rw-rw-   0        0        0     1345 2022-08-02 00:19:43.000000 srsgui-0.2.9/.gitignore
+-rw-rw-rw-   0        0        0     1107 2022-12-07 23:27:48.000000 srsgui-0.2.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     3330 2023-04-11 21:39:00.979862 srsgui-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2633 2023-02-13 17:17:13.000000 srsgui-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.889910 srsgui-0.2.9/docs/
+-rw-rw-rw-   0        0        0      658 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/Makefile
+-rwxrwxrwx   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/autodoc.bat
+-rwxrwxrwx   0        0        0      804 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.899904 srsgui-0.2.9/docs/source/
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.919894 srsgui-0.2.9/docs/source/_static/
+-rw-rw-rw-   0        0        0    31067 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/cg-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    27242 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/cg-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0     5762 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/connect-dialog-box-capture.png
+-rw-rw-rw-   0        0        0    71070 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/example-screen-capture-1.png
+-rw-rw-rw-   0        0        0    71011 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/example-screen-capture-2.png
+-rw-rw-rw-   0        0        0    56013 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/initial-screen-capture.png
+-rw-rw-rw-   0        0        0    29667 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/osc-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    50740 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/second-task-screen-capture.png
+-rw-rw-rw-   0        0        0    39412 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/terminal-with-example-2.png
+-rw-rw-rw-   0        0        0    37573 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/terminal-with-example.png
+-rw-rw-rw-   0        0        0     1938 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/conf.py
+-rw-rw-rw-   0        0        0     5998 2023-04-04 20:33:11.000000 srsgui-0.2.9/docs/source/create-project.rst
+-rw-rw-rw-   0        0        0     6656 2023-04-04 20:33:11.000000 srsgui-0.2.9/docs/source/create-task.rst
+-rw-rw-rw-   0        0        0     6110 2023-04-04 20:33:11.000000 srsgui-0.2.9/docs/source/define-instrument.rst
+-rw-rw-rw-   0        0        0    15655 2023-04-04 20:33:11.000000 srsgui-0.2.9/docs/source/example.rst
+-rw-rw-rw-   0        0        0     3684 2023-04-04 20:33:11.000000 srsgui-0.2.9/docs/source/index.rst
+-rw-rw-rw-   0        0        0     4383 2023-04-04 20:33:11.000000 srsgui-0.2.9/docs/source/installation.rst
+-rw-rw-rw-   0        0        0      936 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/srsgui.inst.communications.rst
+-rw-rw-rw-   0        0        0      950 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/srsgui.inst.rst
+-rw-rw-rw-   0        0        0      117 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/srsgui.rst
+-rw-rw-rw-   0        0        0      989 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/srsgui.task.rst
+-rw-rw-rw-   0        0        0      604 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/srsgui.ui.qt.rst
+-rw-rw-rw-   0        0        0     1629 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/srsgui.ui.rst
+-rw-rw-rw-   0        0        0     1193 2023-04-07 01:13:40.000000 srsgui-0.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 21:39:00.979862 srsgui-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsgui-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.919894 srsgui-0.2.9/srsgui/
+-rw-rw-rw-   0        0        0     1537 2023-04-11 21:34:20.000000 srsgui-0.2.9/srsgui/__init__.py
+-rw-rw-rw-   0        0        0      314 2023-04-07 00:52:02.000000 srsgui-0.2.9/srsgui/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.879943 srsgui-0.2.9/srsgui/examples/
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.919894 srsgui-0.2.9/srsgui/examples/oscilloscope example/
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.919894 srsgui-0.2.9/srsgui/examples/oscilloscope example/instruments/
+-rw-rw-rw-   0        0        0     1709 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/instruments/cg635.py
+-rw-rw-rw-   0        0        0     3025 2023-02-11 01:21:41.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/instruments/sds1202.py
+-rw-rw-rw-   0        0        0     1977 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.929916 srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/
+-rw-rw-rw-   0        0        0     2401 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/fifth.py
+-rw-rw-rw-   0        0        0     1543 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/first.py
+-rw-rw-rw-   0        0        0     3978 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/fourth.py
+-rw-rw-rw-   0        0        0     2129 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/second.py
+-rw-rw-rw-   0        0        0     1893 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/third.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.939882 srsgui-0.2.9/srsgui/inst/
+-rw-rw-rw-   0        0        0     1074 2023-04-04 20:33:11.000000 srsgui-0.2.9/srsgui/inst/__init__.py
+-rw-rw-rw-   0        0        0     9578 2023-04-10 22:51:26.000000 srsgui-0.2.9/srsgui/inst/commands.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.939882 srsgui-0.2.9/srsgui/inst/communications/
+-rw-rw-rw-   0        0        0      126 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/inst/communications/__init__.py
+-rw-rw-rw-   0        0        0     7903 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/inst/communications/interface.py
+-rw-rw-rw-   0        0        0     1157 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/inst/communications/serial_ports.py
+-rw-rw-rw-   0        0        0     8097 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/inst/communications/serialinterface.py
+-rw-rw-rw-   0        0        0    10762 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/inst/communications/tcpipinterface.py
+-rw-rw-rw-   0        0        0    14665 2023-04-11 20:13:55.000000 srsgui-0.2.9/srsgui/inst/component.py
+-rw-rw-rw-   0        0        0      727 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/inst/exceptions.py
+-rw-rw-rw-   0        0        0    10049 2023-04-11 18:04:43.000000 srsgui-0.2.9/srsgui/inst/indexcommands.py
+-rw-rw-rw-   0        0        0     9647 2023-02-09 17:58:55.000000 srsgui-0.2.9/srsgui/inst/instrument.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.949878 srsgui-0.2.9/srsgui/task/
+-rw-rw-rw-   0        0        0        2 2023-04-10 22:51:26.000000 srsgui-0.2.9/srsgui/task/__init__.py
+-rw-rw-rw-   0        0        0      692 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/task/callbacks.py
+-rw-rw-rw-   0        0        0     6485 2023-04-07 01:13:40.000000 srsgui-0.2.9/srsgui/task/config.py
+-rw-rw-rw-   0        0        0     5203 2023-04-11 00:24:36.000000 srsgui-0.2.9/srsgui/task/inputs.py
+-rw-rw-rw-   0        0        0     6865 2023-03-28 15:59:44.000000 srsgui-0.2.9/srsgui/task/sessionhandler.py
+-rw-rw-rw-   0        0        0    22234 2023-04-10 22:51:26.000000 srsgui-0.2.9/srsgui/task/task.py
+-rw-rw-rw-   0        0        0     4108 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/task/taskresult.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.959872 srsgui-0.2.9/srsgui/ui/
+-rw-rw-rw-   0        0        0        0 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/__init__.py
+-rw-rw-rw-   0        0        0     3775 2023-04-04 20:33:12.000000 srsgui-0.2.9/srsgui/ui/commandhandler.py
+-rw-rw-rw-   0        0        0     5918 2023-04-04 20:33:12.000000 srsgui-0.2.9/srsgui/ui/commandterminal.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.969903 srsgui-0.2.9/srsgui/ui/commandtree/
+-rw-rw-rw-   0        0        0     2919 2023-04-07 19:57:55.000000 srsgui-0.2.9/srsgui/ui/commandtree/commandcapturewidget.py
+-rw-rw-rw-   0        0        0     3362 2023-04-10 22:51:26.000000 srsgui-0.2.9/srsgui/ui/commandtree/commandcapturewidget.ui
+-rw-rw-rw-   0        0        0     3489 2023-04-11 17:28:55.000000 srsgui-0.2.9/srsgui/ui/commandtree/commanddelegate.py
+-rw-rw-rw-   0        0        0    10180 2023-04-10 18:03:49.000000 srsgui-0.2.9/srsgui/ui/commandtree/commanditem.py
+-rw-rw-rw-   0        0        0     7833 2023-04-11 17:29:16.000000 srsgui-0.2.9/srsgui/ui/commandtree/commandmodel.py
+-rw-rw-rw-   0        0        0     4755 2023-04-11 17:22:27.000000 srsgui-0.2.9/srsgui/ui/commandtree/commandspinbox.py
+-rw-rw-rw-   0        0        0     3127 2023-04-11 21:33:12.000000 srsgui-0.2.9/srsgui/ui/commandtree/commandtreeview.py
+-rw-rw-rw-   0        0        0     3844 2023-04-11 17:33:14.000000 srsgui-0.2.9/srsgui/ui/commandtree/commandtreewidget.py
+-rw-rw-rw-   0        0        0     9296 2023-04-07 19:57:55.000000 srsgui-0.2.9/srsgui/ui/commandtree/jsonmodel.py
+-rw-rw-rw-   0        0        0     4803 2023-04-10 22:51:26.000000 srsgui-0.2.9/srsgui/ui/commandtree/ui_commandcapturewidget.py
+-rw-rw-rw-   0        0        0     4806 2023-04-11 17:35:42.000000 srsgui-0.2.9/srsgui/ui/commandtree/ui_commandtreewidget.py
+-rw-rw-rw-   0        0        0     9679 2023-04-07 01:13:40.000000 srsgui-0.2.9/srsgui/ui/connectdlg.py
+-rw-rw-rw-   0        0        0     3856 2023-04-04 20:33:12.000000 srsgui-0.2.9/srsgui/ui/deviceinfohandler.py
+-rw-rw-rw-   0        0        0    14127 2023-04-07 19:57:55.000000 srsgui-0.2.9/srsgui/ui/dockhandler.py
+-rw-rw-rw-   0        0        0    13671 2023-04-11 00:24:36.000000 srsgui-0.2.9/srsgui/ui/inputpanel.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.979862 srsgui-0.2.9/srsgui/ui/qt/
+-rw-rw-rw-   0        0        0      678 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/qt/QtCore.py
+-rw-rw-rw-   0        0        0      556 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/qt/QtGui.py
+-rw-rw-rw-   0        0        0      656 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/qt/QtWidgets.py
+-rw-rw-rw-   0        0        0     1457 2023-03-08 01:32:20.000000 srsgui-0.2.9/srsgui/ui/qt/__init__.py
+-rw-rw-rw-   0        0        0     1164 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/qtloghandler.py
+-rw-rw-rw-   0        0        0      268 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/resource.qrc
+-rw-rw-rw-   0        0        0    15358 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/resource_rc.py
+-rw-rw-rw-   0        0        0     2598 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/signalhandler.py
+-rw-rw-rw-   0        0        0    47891 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/srslogo.jpg
+-rw-rw-rw-   0        0        0      886 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/stdout.py
+-rw-rw-rw-   0        0        0    24758 2023-04-10 15:41:10.000000 srsgui-0.2.9/srsgui/ui/taskmain.py
+-rw-rw-rw-   0        0        0    10403 2023-02-22 17:26:46.000000 srsgui-0.2.9/srsgui/ui/taskmain.ui
+-rw-rw-rw-   0        0        0    11293 2023-02-22 17:26:46.000000 srsgui-0.2.9/srsgui/ui/ui_taskmain.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.919894 srsgui-0.2.9/srsgui.egg-info/
+-rw-rw-rw-   0        0        0     3330 2023-04-11 21:39:00.000000 srsgui-0.2.9/srsgui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3162 2023-04-11 21:39:00.000000 srsgui-0.2.9/srsgui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 21:39:00.000000 srsgui-0.2.9/srsgui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-11 21:39:00.000000 srsgui-0.2.9/srsgui.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       53 2023-04-11 21:39:00.000000 srsgui-0.2.9/srsgui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-11 21:39:00.000000 srsgui-0.2.9/srsgui.egg-info/top_level.txt
```

### Comparing `srsgui-0.2.13/.gitignore` & `srsgui-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/LICENSE.txt` & `srsgui-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/PKG-INFO` & `srsgui-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.2.13
+Version: 0.2.9
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Keywords: instrument control,data acquisition,data visualization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `srsgui-0.2.13/README.md` & `srsgui-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/docs/Makefile` & `srsgui-0.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/docs/make.bat` & `srsgui-0.2.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/docs/source/_static/cg-dir-terminal-screen-capture.png` & `srsgui-0.2.9/docs/source/_static/cg-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/docs/source/_static/cg-terminal-screen-capture.png` & `srsgui-0.2.9/docs/source/_static/cg-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/docs/source/_static/connect-dialog-box-capture.png` & `srsgui-0.2.9/docs/source/_static/connect-dialog-box-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/docs/source/_static/example-screen-capture-1.png` & `srsgui-0.2.9/docs/source/_static/example-screen-capture-1.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/docs/source/_static/example-screen-capture-2.png` & `srsgui-0.2.9/docs/source/_static/example-screen-capture-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/docs/source/_static/initial-screen-capture.png` & `srsgui-0.2.9/docs/source/_static/initial-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/docs/source/_static/osc-dir-terminal-screen-capture.png` & `srsgui-0.2.9/docs/source/_static/osc-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/docs/source/_static/second-task-screen-capture.png` & `srsgui-0.2.9/docs/source/_static/second-task-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/docs/source/_static/terminal-with-example-2.png` & `srsgui-0.2.9/docs/source/_static/terminal-with-example-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/docs/source/_static/terminal-with-example.png` & `srsgui-0.2.9/docs/source/_static/terminal-with-example.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/docs/source/conf.py` & `srsgui-0.2.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/docs/source/create-project.rst` & `srsgui-0.2.9/docs/source/create-project.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/docs/source/create-task.rst` & `srsgui-0.2.9/docs/source/create-task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/docs/source/define-instrument.rst` & `srsgui-0.2.9/docs/source/define-instrument.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/docs/source/example.rst` & `srsgui-0.2.9/docs/source/example.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/docs/source/index.rst` & `srsgui-0.2.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/docs/source/installation.rst` & `srsgui-0.2.9/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/docs/source/srsgui.inst.communications.rst` & `srsgui-0.2.9/docs/source/srsgui.inst.communications.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/docs/source/srsgui.inst.rst` & `srsgui-0.2.9/docs/source/srsgui.inst.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/docs/source/srsgui.task.rst` & `srsgui-0.2.9/docs/source/srsgui.task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/docs/source/srsgui.ui.qt.rst` & `srsgui-0.2.9/docs/source/srsgui.ui.qt.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/docs/source/srsgui.ui.rst` & `srsgui-0.2.9/docs/source/srsgui.ui.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/pyproject.toml` & `srsgui-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/__init__.py` & `srsgui-0.2.9/srsgui/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
                         InstLoginFailureError, InstIdError, \
                         InstSetError, InstQueryError, InstIndexError
 
 from srsgui.inst import Interface, SerialInterface, TcpipInterface
 from srsgui.inst.instrument import Instrument
 from srsgui.inst.component import Component
 
-__version__ = "0.2.13"  # Global version number
+__version__ = "0.2.9"  # Global version number
```

### Comparing `srsgui-0.2.13/srsgui/examples/oscilloscope example/instruments/cg635.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/instruments/cg635.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/examples/oscilloscope example/instruments/sds1202.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/instruments/sds1202.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/examples/oscilloscope example/tasks/fifth.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/fifth.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/examples/oscilloscope example/tasks/first.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/first.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/examples/oscilloscope example/tasks/fourth.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/fourth.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/examples/oscilloscope example/tasks/second.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/second.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/examples/oscilloscope example/tasks/third.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/third.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/inst/__init__.py` & `srsgui-0.2.9/srsgui/inst/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/inst/commands.py` & `srsgui-0.2.9/srsgui/inst/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,15 +212,15 @@
 
 class FloatCommand(Command):
     """
     Descriptor for a remote command to
     **set** and **query** a **float** value
     """
 
-    def __init__(self, remote_command_name, unit='', min=-1e6, max=1e6, step=1e-9,
+    def __init__(self, remote_command_name, unit='', min=-1000.0, max=1000.0, step=0.1,
                  significant_figures=4, default_value=None):
         super().__init__(remote_command_name, default_value)
         self._get_convert_function = float
 
         self.unit = unit
         self.maximum = max
         self.minimum = min
```

### Comparing `srsgui-0.2.13/srsgui/inst/communications/interface.py` & `srsgui-0.2.9/srsgui/inst/communications/interface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/inst/communications/serial_ports.py` & `srsgui-0.2.9/srsgui/inst/communications/serial_ports.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/inst/communications/serialinterface.py` & `srsgui-0.2.9/srsgui/inst/communications/serialinterface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/inst/communications/tcpipinterface.py` & `srsgui-0.2.9/srsgui/inst/communications/tcpipinterface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/inst/component.py` & `srsgui-0.2.9/srsgui/inst/component.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/inst/exceptions.py` & `srsgui-0.2.9/srsgui/inst/exceptions.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/inst/indexcommands.py` & `srsgui-0.2.9/srsgui/inst/indexcommands.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
 class FloatIndexCommand(IndexCommand):
     """
     Command class for a remote command with index
     using **set** and **query** returning an **float**
     """
 
     def __init__(self, remote_command_name, index_max, index_min=0, index_dict=None,
-                 unit='', value_min=-1e6, value_max=1e6, step=1e-9, significant_figures=4, default_valaue=0.0 ):
+                 unit='', value_min=-1e6, value_max=1e6, step=0.1, significant_figures=4, default_valaue=0.0 ):
         super().__init__(remote_command_name, index_max, index_min, index_dict)
         self._get_convert_function = float
 
         self.unit = unit
         self.maximum = value_max
         self.minimum = value_min
         self.step = step
```

### Comparing `srsgui-0.2.13/srsgui/inst/instrument.py` & `srsgui-0.2.9/srsgui/inst/instrument.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/task/callbacks.py` & `srsgui-0.2.9/srsgui/task/callbacks.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/task/config.py` & `srsgui-0.2.9/srsgui/task/config.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/task/inputs.py` & `srsgui-0.2.9/srsgui/task/inputs.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/task/sessionhandler.py` & `srsgui-0.2.9/srsgui/task/sessionhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/task/task.py` & `srsgui-0.2.9/srsgui/task/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,15 +276,15 @@
             self._keep_running = False
 
     def delay(self, seconds):
         """
         Check if the task is stopped and wait for the given seconds.
         """
         if not self._keep_running:
-            raise Task.TaskException('Task is requested to stop')
+            raise KeyboardInterrupt('Task is stopped')
         else:
             time.sleep(seconds)
 
     def set_session_handler(self, session_handler):
         """
         Parent should set a session handler for Task to use file output.
         """
@@ -350,15 +350,15 @@
     def clear_figures(self):
         """
         Clear all the figures in figure_dict
         """
         for fig in self.figure_dict.values():
             if hasattr(fig, 'canvas'):
                 fig.clear()
-                self.request_figure_update(fig)
+                self.request_figure_update()
 
     def is_running(self):
         """
         Task should check is_running() is True.
         If it returns False, Task should stop ASAP.
         """
         return self._keep_running
```

### Comparing `srsgui-0.2.13/srsgui/task/taskresult.py` & `srsgui-0.2.9/srsgui/task/taskresult.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/ui/commandhandler.py` & `srsgui-0.2.9/srsgui/ui/commandhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/ui/commandterminal.py` & `srsgui-0.2.9/srsgui/ui/commandterminal.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/ui/commandtree/commandcapturewidget.py` & `srsgui-0.2.9/srsgui/ui/commandtree/commandcapturewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/ui/commandtree/commandcapturewidget.ui` & `srsgui-0.2.9/srsgui/ui/commandtree/commandcapturewidget.ui`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/ui/commandtree/commanddelegate.py` & `srsgui-0.2.9/srsgui/ui/commandtree/commanddelegate.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,30 +19,30 @@
         if item.comp_type == Index:
             comp = item.parent().comp
             comp_type = item.parent().comp_type
         else:
             comp = item.comp
             comp_type = item.comp_type
 
-        if issubclass(comp_type, FloatCommand) or issubclass(comp_type, FloatIndexCommand):
+        if comp_type in (FloatCommand, FloatIndexCommand):
             editor = FloatSpinBox(parent)
             editor.setDecimals(10)
             editor.setSingleStep(0.1)
             editor.setMinimum(comp.minimum)
             editor.setMaximum(comp.maximum)
-            editor.setSuffix(' ' + comp.unit)
+            editor.setSuffix(comp.unit)
             editor.set_significant_figures(comp.significant_figures)
             editor.set_minimum_step(comp.step)
             return editor
 
-        elif issubclass(comp_type, IntCommand) or issubclass(comp_type, IntIndexCommand):
+        elif comp_type in (IntCommand, IntIndexCommand):
             editor = IntegerSpinBox(parent)
             editor.setMinimum(comp.minimum)
             editor.setMaximum(comp.maximum)
-            editor.setSuffix(' ' + comp.unit)
+            editor.setSuffix(comp.unit)
             return editor
 
         elif comp_type in (DictCommand, DictIndexCommand):
             editor = QComboBox(parent)
             for key in comp.set_dict.keys():
                 editor.addItem(str(key))
             return editor
@@ -67,20 +67,20 @@
         if item.comp_type == Index:
             comp = item.parent().comp
             comp_type = item.parent().comp_type
         else:
             comp = item.comp
             comp_type = item.comp_type
 
-        if issubclass(comp_type, FloatCommand) or issubclass(comp_type, FloatIndexCommand):
+        if comp_type in (FloatCommand, FloatIndexCommand):
             value = editor.value()
             model.setData(index, value, Qt.EditRole)
             item.precision = editor.precision
             return True
-        elif issubclass(comp_type, IntCommand) or issubclass(comp_type, IntIndexCommand):
+        elif comp_type in (IntCommand, IntIndexCommand):
             value = editor.value()
             model.setData(index, value, Qt.EditRole)
             return True
         elif comp_type in (DictCommand, DictIndexCommand):
             val = editor.currentText()
             convert = type(list(comp.get_dict.keys())[0])
             value = convert(val)
```

### Comparing `srsgui-0.2.13/srsgui/ui/commandtree/commanditem.py` & `srsgui-0.2.9/srsgui/ui/commandtree/commanditem.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,651 +1,637 @@
-00000000: 0d0a 696d 706f 7274 2074 696d 650d 0a69  ..import time..i
-00000010: 6d70 6f72 7420 6d61 7468 0d0a 0d0a 6672  mport math....fr
-00000020: 6f6d 2073 7273 6775 6920 696d 706f 7274  om srsgui import
-00000030: 2043 6f6d 706f 6e65 6e74 0d0a 6672 6f6d   Component..from
-00000040: 2073 7273 6775 692e 696e 7374 2069 6d70   srsgui.inst imp
-00000050: 6f72 7420 436f 6d6d 616e 642c 2049 6e64  ort Command, Ind
-00000060: 6578 436f 6d6d 616e 642c 205c 0d0a 2020  exCommand, \..  
-00000070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000080: 2020 2020 2020 466c 6f61 7443 6f6d 6d61        FloatComma
-00000090: 6e64 2c20 466c 6f61 7449 6e64 6578 436f  nd, FloatIndexCo
-000000a0: 6d6d 616e 640d 0a0d 0a0d 0a63 6c61 7373  mmand......class
-000000b0: 2049 6e64 6578 3a0d 0a20 2020 2070 6173   Index:..    pas
-000000c0: 730d 0a0d 0a0d 0a63 6c61 7373 2043 6f6d  s......class Com
-000000d0: 6d61 6e64 4974 656d 3a0d 0a20 2020 2022  mandItem:..    "
-000000e0: 2222 4120 436f 6d6d 616e 6420 6974 656d  ""A Command item
-000000f0: 2063 6f72 7265 7370 6f6e 6469 6e67 2074   corresponding t
-00000100: 6f20 6120 6c69 6e65 2069 6e20 5154 7265  o a line in QTre
-00000110: 6556 6965 7722 2222 0d0a 0d0a 2020 2020  eView"""....    
-00000120: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00000130: 662c 2070 6172 656e 743a 2022 436f 6d6d  f, parent: "Comm
-00000140: 616e 6449 7465 6d22 203d 204e 6f6e 6529  andItem" = None)
-00000150: 3a0d 0a20 2020 2020 2020 2073 656c 662e  :..        self.
-00000160: 5f70 6172 656e 7420 3d20 7061 7265 6e74  _parent = parent
-00000170: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-00000180: 6368 696c 6472 656e 203d 205b 5d0d 0a20  children = [].. 
-00000190: 2020 2020 2020 2073 656c 662e 5f76 616c         self._val
-000001a0: 7565 203d 204e 6f6e 650d 0a20 2020 2020  ue = None..     
-000001b0: 2020 200d 0a20 2020 2020 2020 2073 656c     ..        sel
-000001c0: 662e 6e61 6d65 203d 2022 220d 0a20 2020  f.name = ""..   
-000001d0: 2020 2020 2073 656c 662e 7661 6c75 655f       self.value_
-000001e0: 7479 7065 203d 204e 6f6e 6520 2023 2054  type = None  # T
-000001f0: 6865 7265 2061 7265 2033 2074 7970 6573  here are 3 types
-00000200: 206f 6620 7661 6c75 6573 3a20 7374 722c   of values: str,
-00000210: 2069 6e74 2c20 616e 6420 666c 6f61 740d   int, and float.
-00000220: 0a0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
-00000230: 636f 6d70 203d 204e 6f6e 650d 0a20 2020  comp = None..   
-00000240: 2020 2020 2073 656c 662e 636f 6d70 5f74       self.comp_t
-00000250: 7970 6520 3d20 4e6f 6e65 2020 2023 2054  ype = None   # T
-00000260: 6865 7265 2061 7265 2035 2074 7970 6573  here are 5 types
-00000270: 206f 6620 636f 6d70 6f6e 656e 7473 3a20   of components: 
-00000280: 436f 6d70 6f6e 656e 742c 2043 6f6d 6d61  Component, Comma
-00000290: 6e64 732c 2049 6e64 6578 436f 6d6d 616e  nds, IndexComman
-000002a0: 6473 2c20 6d65 7468 6f64 2061 6e64 2049  ds, method and I
-000002b0: 6e64 6578 0d0a 2020 2020 2020 2020 7365  ndex..        se
-000002c0: 6c66 2e73 6574 5f65 6e61 626c 6520 3d20  lf.set_enable = 
-000002d0: 4661 6c73 650d 0a20 2020 2020 2020 2073  False..        s
-000002e0: 656c 662e 6765 745f 656e 6162 6c65 203d  elf.get_enable =
-000002f0: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
-00000300: 7365 6c66 2e69 735f 6d65 7468 6f64 203d  self.is_method =
-00000310: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
-00000320: 7365 6c66 2e65 7863 6c75 6465 6420 3d20  self.excluded = 
-00000330: 4661 6c73 650d 0a20 2020 2020 2020 2073  False..        s
-00000340: 656c 662e 7261 775f 7265 6d6f 7465 5f63  elf.raw_remote_c
-00000350: 6f6d 6d61 6e64 203d 2022 220d 0a20 2020  ommand = ""..   
-00000360: 2020 2020 2073 656c 662e 7469 6d65 7374       self.timest
-00000370: 616d 7020 3d20 302e 300d 0a0d 0a20 2020  amp = 0.0....   
-00000380: 2064 6566 2061 7070 656e 6443 6869 6c64   def appendChild
-00000390: 2873 656c 662c 2069 7465 6d3a 2022 436f  (self, item: "Co
-000003a0: 6d6d 616e 6449 7465 6d22 293a 0d0a 2020  mmandItem"):..  
-000003b0: 2020 2020 2020 2222 2241 6464 2069 7465        """Add ite
-000003c0: 6d20 6173 2061 2063 6869 6c64 2222 220d  m as a child""".
-000003d0: 0a20 2020 2020 2020 2073 656c 662e 5f63  .        self._c
-000003e0: 6869 6c64 7265 6e2e 6170 7065 6e64 2869  hildren.append(i
-000003f0: 7465 6d29 0d0a 0d0a 2020 2020 6465 6620  tem)....    def 
-00000400: 6368 696c 6428 7365 6c66 2c20 726f 773a  child(self, row:
-00000410: 2069 6e74 2920 2d3e 2022 436f 6d6d 616e   int) -> "Comman
-00000420: 6449 7465 6d22 3a0d 0a20 2020 2020 2020  dItem":..       
-00000430: 2022 2222 5265 7475 726e 2074 6865 2063   """Return the c
-00000440: 6869 6c64 206f 6620 7468 6520 6375 7272  hild of the curr
-00000450: 656e 7420 6974 656d 2066 726f 6d20 7468  ent item from th
-00000460: 6520 6769 7665 6e20 726f 7722 2222 0d0a  e given row"""..
-00000470: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00000480: 656c 662e 5f63 6869 6c64 7265 6e5b 726f  elf._children[ro
-00000490: 775d 0d0a 0d0a 2020 2020 6465 6620 7061  w]....    def pa
-000004a0: 7265 6e74 2873 656c 6629 202d 3e20 2243  rent(self) -> "C
-000004b0: 6f6d 6d61 6e64 4974 656d 223a 0d0a 2020  ommandItem":..  
-000004c0: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
-000004d0: 7468 6520 7061 7265 6e74 206f 6620 7468  the parent of th
-000004e0: 6520 6375 7272 656e 7420 6974 656d 2222  e current item""
-000004f0: 220d 0a20 2020 2020 2020 2072 6574 7572  "..        retur
-00000500: 6e20 7365 6c66 2e5f 7061 7265 6e74 0d0a  n self._parent..
-00000510: 0d0a 2020 2020 6465 6620 6368 696c 6443  ..    def childC
-00000520: 6f75 6e74 2873 656c 6629 202d 3e20 696e  ount(self) -> in
-00000530: 743a 0d0a 2020 2020 2020 2020 2222 2252  t:..        """R
-00000540: 6574 7572 6e20 7468 6520 6e75 6d62 6572  eturn the number
-00000550: 206f 6620 6368 696c 6472 656e 206f 6620   of children of 
-00000560: 7468 6520 6375 7272 656e 7420 6974 656d  the current item
-00000570: 2222 220d 0a20 2020 2020 2020 2072 6574  """..        ret
-00000580: 7572 6e20 6c65 6e28 7365 6c66 2e5f 6368  urn len(self._ch
-00000590: 696c 6472 656e 290d 0a0d 0a20 2020 2064  ildren)....    d
-000005a0: 6566 2072 6f77 2873 656c 6629 202d 3e20  ef row(self) -> 
-000005b0: 696e 743a 0d0a 2020 2020 2020 2020 2222  int:..        ""
-000005c0: 2252 6574 7572 6e20 7468 6520 726f 7720  "Return the row 
-000005d0: 7768 6572 6520 7468 6520 6375 7272 656e  where the curren
-000005e0: 7420 6974 656d 206f 6363 7570 6965 7320  t item occupies 
-000005f0: 696e 2074 6865 2070 6172 656e 7422 2222  in the parent"""
-00000600: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00000610: 2073 656c 662e 5f70 6172 656e 742e 5f63   self._parent._c
-00000620: 6869 6c64 7265 6e2e 696e 6465 7828 7365  hildren.index(se
-00000630: 6c66 2920 6966 2073 656c 662e 5f70 6172  lf) if self._par
-00000640: 656e 7420 656c 7365 2030 0d0a 0d0a 2020  ent else 0....  
-00000650: 2020 4070 726f 7065 7274 790d 0a20 2020    @property..   
-00000660: 2064 6566 2076 616c 7565 2873 656c 6629   def value(self)
-00000670: 3a0d 0a20 2020 2020 2020 2022 2222 5265  :..        """Re
-00000680: 7475 726e 2074 6865 2076 616c 7565 206f  turn the value o
-00000690: 6620 7468 6520 6375 7272 656e 7420 6974  f the current it
-000006a0: 656d 2222 220d 0a20 2020 2020 2020 2074  em"""..        t
-000006b0: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
-000006c0: 2074 7320 3d20 7469 6d65 2e74 696d 6528   ts = time.time(
-000006d0: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
-000006e0: 6620 7473 202d 2073 656c 662e 7469 6d65  f ts - self.time
-000006f0: 7374 616d 7020 3c20 302e 313a 2020 2320  stamp < 0.1:  # 
-00000700: 5570 6461 7465 2076 616c 7565 206c 6174  Update value lat
-00000710: 6572 2074 6861 6e20 302e 3120 730d 0a20  er than 0.1 s.. 
-00000720: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00000730: 6574 7572 6e20 7365 6c66 2e5f 7661 6c75  eturn self._valu
-00000740: 650d 0a0d 0a20 2020 2020 2020 2020 2020  e....           
-00000750: 2069 6620 7365 6c66 2e63 6f6d 705f 7479   if self.comp_ty
-00000760: 7065 203d 3d20 496e 6465 7820 616e 6420  pe == Index and 
-00000770: 7365 6c66 2e67 6574 5f65 6e61 626c 6520  self.get_enable 
-00000780: 616e 6420 6e6f 7420 7365 6c66 2e65 7863  and not self.exc
-00000790: 6c75 6465 643a 0d0a 2020 2020 2020 2020  luded:..        
-000007a0: 2020 2020 2020 2020 7365 6c66 2e5f 7661          self._va
-000007b0: 6c75 6520 3d20 7365 6c66 2e5f 7061 7265  lue = self._pare
-000007c0: 6e74 2e63 6f6d 702e 5f5f 6765 7469 7465  nt.comp.__getite
-000007d0: 6d5f 5f28 7365 6c66 2e63 6f6d 7029 0d0a  m__(self.comp)..
-000007e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007f0: 7365 6c66 2e76 616c 7565 5f74 7970 6520  self.value_type 
-00000800: 3d20 7479 7065 2873 656c 662e 5f76 616c  = type(self._val
-00000810: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
-00000820: 2020 2020 2073 656c 662e 7469 6d65 7374       self.timest
-00000830: 616d 7020 3d20 7473 0d0a 2020 2020 2020  amp = ts..      
-00000840: 2020 2020 2020 656c 6966 2069 7373 7562        elif issub
-00000850: 636c 6173 7328 7479 7065 2873 656c 662e  class(type(self.
-00000860: 636f 6d70 292c 2043 6f6d 6d61 6e64 2920  comp), Command) 
-00000870: 616e 6420 7365 6c66 2e67 6574 5f65 6e61  and self.get_ena
-00000880: 626c 6520 616e 6420 6e6f 7420 7365 6c66  ble and not self
-00000890: 2e65 7863 6c75 6465 643a 0d0a 2020 2020  .excluded:..    
-000008a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000008b0: 2e5f 7661 6c75 6520 3d20 7365 6c66 2e63  ._value = self.c
-000008c0: 6f6d 702e 5f5f 6765 745f 5f28 7365 6c66  omp.__get__(self
-000008d0: 2e5f 7061 7265 6e74 2e63 6f6d 702c 2073  ._parent.comp, s
-000008e0: 656c 662e 5f70 6172 656e 742e 636f 6d70  elf._parent.comp
-000008f0: 2e5f 5f63 6c61 7373 5f5f 290d 0a20 2020  .__class__)..   
-00000900: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00000910: 662e 7661 6c75 655f 7479 7065 203d 2074  f.value_type = t
-00000920: 7970 6528 7365 6c66 2e5f 7661 6c75 6529  ype(self._value)
-00000930: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000940: 2020 7365 6c66 2e74 696d 6573 7461 6d70    self.timestamp
-00000950: 203d 2074 730d 0a20 2020 2020 2020 2065   = ts..        e
-00000960: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
-00000970: 6173 2065 3a0d 0a20 2020 2020 2020 2020  as e:..         
-00000980: 2020 2070 7269 6e74 2827 4572 726f 723a     print('Error:
-00000990: 207b 7d20 7b7d 272e 666f 726d 6174 2865   {} {}'.format(e
-000009a0: 2c20 7365 6c66 2e6e 616d 6529 290d 0a20  , self.name)).. 
-000009b0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-000009c0: 6c66 2e5f 7661 6c75 650d 0a0d 0a20 2020  lf._value....   
-000009d0: 2040 7661 6c75 652e 7365 7474 6572 0d0a   @value.setter..
-000009e0: 2020 2020 6465 6620 7661 6c75 6528 7365      def value(se
-000009f0: 6c66 2c20 7661 6c75 6529 3a0d 0a20 2020  lf, value):..   
-00000a00: 2020 2020 2073 656c 662e 5f76 616c 7565       self._value
-00000a10: 203d 2076 616c 7565 0d0a 0d0a 2020 2020   = value....    
-00000a20: 6465 6620 7365 745f 7661 6c75 6528 7365  def set_value(se
-00000a30: 6c66 2c20 7661 6c75 6529 3a0d 0a20 2020  lf, value):..   
-00000a40: 2020 2020 2022 2222 5365 7420 7661 6c75       """Set valu
-00000a50: 6520 746f 2074 6865 2069 6e73 7472 756d  e to the instrum
-00000a60: 656e 7420 616e 6420 7570 6461 7465 2074  ent and update t
-00000a70: 6865 2076 616c 7565 206f 6620 7468 6520  he value of the 
-00000a80: 6974 656d 2222 220d 0a20 2020 2020 2020  item"""..       
-00000a90: 2069 6620 7365 6c66 2e63 6f6d 705f 7479   if self.comp_ty
-00000aa0: 7065 203d 3d20 496e 6465 783a 0d0a 2020  pe == Index:..  
-00000ab0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00000ac0: 7061 7265 6e74 2e63 6f6d 702e 5f5f 7365  parent.comp.__se
-00000ad0: 7469 7465 6d5f 5f28 7365 6c66 2e63 6f6d  titem__(self.com
-00000ae0: 702c 2076 616c 7565 290d 0a20 2020 2020  p, value)..     
-00000af0: 2020 2020 2020 2073 656c 662e 5f76 616c         self._val
-00000b00: 7565 203d 2073 656c 662e 5f70 6172 656e  ue = self._paren
-00000b10: 742e 636f 6d70 2e5f 5f67 6574 6974 656d  t.comp.__getitem
-00000b20: 5f5f 2873 656c 662e 636f 6d70 290d 0a20  __(self.comp).. 
-00000b30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00000b40: 7469 6d65 7374 616d 7020 3d20 7469 6d65  timestamp = time
-00000b50: 2e74 696d 6528 290d 0a20 2020 2020 2020  .time()..       
-00000b60: 2065 6c69 6620 6973 7375 6263 6c61 7373   elif issubclass
-00000b70: 2874 7970 6528 7365 6c66 2e63 6f6d 7029  (type(self.comp)
-00000b80: 2c20 436f 6d6d 616e 6429 3a0d 0a20 2020  , Command):..   
-00000b90: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-00000ba0: 6d70 2e5f 5f73 6574 5f5f 2873 656c 662e  mp.__set__(self.
-00000bb0: 5f70 6172 656e 742e 636f 6d70 2c20 7661  _parent.comp, va
-00000bc0: 6c75 6529 0d0a 2020 2020 2020 2020 2020  lue)..          
-00000bd0: 2020 7365 6c66 2e5f 7661 6c75 6520 3d20    self._value = 
-00000be0: 7365 6c66 2e63 6f6d 702e 5f5f 6765 745f  self.comp.__get_
-00000bf0: 5f28 7365 6c66 2e5f 7061 7265 6e74 2e63  _(self._parent.c
-00000c00: 6f6d 702c 2073 656c 662e 5f70 6172 656e  omp, self._paren
-00000c10: 742e 636f 6d70 2e5f 5f63 6c61 7373 5f5f  t.comp.__class__
-00000c20: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
-00000c30: 656c 662e 7469 6d65 7374 616d 7020 3d20  elf.timestamp = 
-00000c40: 7469 6d65 2e74 696d 6528 290d 0a20 2020  time.time()..   
-00000c50: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00000c60: 2020 2020 2020 2020 7365 6c66 2e5f 7661          self._va
-00000c70: 6c75 6520 3d20 7661 6c75 650d 0a0d 0a20  lue = value.... 
-00000c80: 2020 2064 6566 2069 735f 6564 6974 6162     def is_editab
-00000c90: 6c65 2873 656c 6629 3a0d 0a20 2020 2020  le(self):..     
-00000ca0: 2020 2022 2222 5265 7475 726e 2054 7275     """Return Tru
-00000cb0: 6520 6966 2074 6865 2069 7465 6d20 6973  e if the item is
-00000cc0: 2065 6469 7461 626c 6522 2222 0d0a 2020   editable"""..  
-00000cd0: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
-00000ce0: 6d70 5f74 7970 6520 3d3d 2049 6e64 6578  mp_type == Index
-00000cf0: 2061 6e64 205c 0d0a 2020 2020 2020 2020   and \..        
-00000d00: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-00000d10: 5f65 6e61 626c 6520 616e 6420 7365 6c66  _enable and self
-00000d20: 2e67 6574 5f65 6e61 626c 6520 616e 6420  .get_enable and 
-00000d30: 6e6f 7420 7365 6c66 2e65 7863 6c75 6465  not self.exclude
-00000d40: 643a 0d0a 2020 2020 2020 2020 2020 2020  d:..            
-00000d50: 7265 7475 726e 2054 7275 650d 0a20 2020  return True..   
-00000d60: 2020 2020 2065 6c69 6620 6973 7375 6263       elif issubc
-00000d70: 6c61 7373 2874 7970 6528 7365 6c66 2e63  lass(type(self.c
-00000d80: 6f6d 7029 2c20 436f 6d6d 616e 6429 2061  omp), Command) a
-00000d90: 6e64 205c 0d0a 2020 2020 2020 2020 2020  nd \..          
-00000da0: 2020 2020 2020 7365 6c66 2e73 6574 5f65        self.set_e
-00000db0: 6e61 626c 6520 616e 6420 7365 6c66 2e67  nable and self.g
-00000dc0: 6574 5f65 6e61 626c 6520 616e 6420 6e6f  et_enable and no
-00000dd0: 7420 7365 6c66 2e65 7863 6c75 6465 643a  t self.excluded:
-00000de0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00000df0: 7475 726e 2054 7275 650d 0a20 2020 2020  turn True..     
-00000e00: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00000e10: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00000e20: 7365 0d0a 0d0a 2020 2020 6465 6620 6765  se....    def ge
-00000e30: 745f 666f 726d 6174 7465 645f 7661 6c75  t_formatted_valu
-00000e40: 6528 7365 6c66 2c20 7661 6c75 6529 3a0d  e(self, value):.
-00000e50: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
-00000e60: 726e 2066 6f72 6d61 7474 6564 2076 616c  rn formatted val
-00000e70: 7565 206f 6620 6120 666c 6f61 7422 2222  ue of a float"""
-00000e80: 0d0a 0d0a 2020 2020 2020 2020 636f 6d70  ....        comp
-00000e90: 203d 204e 6f6e 650d 0a20 2020 2020 2020   = None..       
-00000ea0: 2069 6620 7365 6c66 2e63 6f6d 705f 7479   if self.comp_ty
-00000eb0: 7065 203d 3d20 496e 6465 783a 0d0a 2020  pe == Index:..  
-00000ec0: 2020 2020 2020 2020 2020 636f 6d70 203d            comp =
-00000ed0: 2073 656c 662e 7061 7265 6e74 2829 2e63   self.parent().c
-00000ee0: 6f6d 700d 0a20 2020 2020 2020 2065 6c69  omp..        eli
-00000ef0: 6620 6973 7375 6263 6c61 7373 2874 7970  f issubclass(typ
-00000f00: 6528 7365 6c66 2e63 6f6d 7029 2c20 436f  e(self.comp), Co
-00000f10: 6d6d 616e 6429 206f 7220 5c0d 0a20 2020  mmand) or \..   
-00000f20: 2020 2020 2020 2020 2020 6973 7375 6263            issubc
-00000f30: 6c61 7373 2874 7970 6528 7365 6c66 2e63  lass(type(self.c
-00000f40: 6f6d 7029 2c20 496e 6465 7843 6f6d 6d61  omp), IndexComma
-00000f50: 6e64 293a 0d0a 2020 2020 2020 2020 2020  nd):..          
-00000f60: 2020 636f 6d70 203d 2073 656c 662e 636f    comp = self.co
-00000f70: 6d70 0d0a 0d0a 2020 2020 2020 2020 666d  mp....        fm
-00000f80: 7420 3d20 636f 6d70 2e66 6d74 2069 6620  t = comp.fmt if 
-00000f90: 636f 6d70 2061 6e64 2068 6173 6174 7472  comp and hasattr
-00000fa0: 2863 6f6d 702c 2027 666d 7427 2920 656c  (comp, 'fmt') el
-00000fb0: 7365 2027 270d 0a20 2020 2020 2020 2075  se ''..        u
-00000fc0: 6e69 7420 3d20 636f 6d70 2e75 6e69 7420  nit = comp.unit 
-00000fd0: 6966 2063 6f6d 7020 616e 6420 6861 7361  if comp and hasa
-00000fe0: 7474 7228 636f 6d70 2c20 2775 6e69 7427  ttr(comp, 'unit'
-00000ff0: 2920 656c 7365 2027 270d 0a0d 0a20 2020  ) else ''....   
-00001000: 2020 2020 2069 6620 636f 6d70 2061 6e64       if comp and
-00001010: 2028 6973 7375 6263 6c61 7373 2874 7970   (issubclass(typ
-00001020: 6528 636f 6d70 292c 2046 6c6f 6174 496e  e(comp), FloatIn
-00001030: 6465 7843 6f6d 6d61 6e64 2920 6f72 0d0a  dexCommand) or..
-00001040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001050: 2020 2020 2069 7373 7562 636c 6173 7328       issubclass(
-00001060: 7479 7065 2863 6f6d 7029 2c20 466c 6f61  type(comp), Floa
-00001070: 7443 6f6d 6d61 6e64 2929 3a0d 0a20 2020  tCommand)):..   
-00001080: 2020 2020 2020 2020 2069 6620 7661 6c75           if valu
-00001090: 6520 3d3d 2030 2e30 3a0d 0a20 2020 2020  e == 0.0:..     
-000010a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000010b0: 6e20 2730 2720 2b20 6627 207b 756e 6974  n '0' + f' {unit
-000010c0: 7d27 0d0a 2020 2020 2020 2020 2020 2020  }'..            
-000010d0: 7374 6570 203d 2063 6f6d 702e 7374 6570  step = comp.step
-000010e0: 0d0a 2020 2020 2020 2020 2020 2020 7369  ..            si
-000010f0: 676e 6966 6963 616e 745f 6669 6775 7265  gnificant_figure
-00001100: 7320 3d20 636f 6d70 2e73 6967 6e69 6669  s = comp.signifi
-00001110: 6361 6e74 5f66 6967 7572 6573 0d0a 0d0a  cant_figures....
-00001120: 2020 2020 2020 2020 2020 2020 6465 6369              deci
-00001130: 6d61 6c73 203d 206d 6174 682e 6365 696c  mals = math.ceil
-00001140: 282d 6d61 7468 2e6c 6f67 3130 2873 7465  (-math.log10(ste
-00001150: 7029 290d 0a20 2020 2020 2020 2020 2020  p))..           
-00001160: 2064 6967 6974 7320 3d20 6d61 7468 2e63   digits = math.c
-00001170: 6569 6c28 6d61 7468 2e6c 6f67 3130 2861  eil(math.log10(a
-00001180: 6273 2876 616c 7565 2929 2920 6966 2076  bs(value))) if v
-00001190: 616c 7565 2065 6c73 6520 300d 0a20 2020  alue else 0..   
-000011a0: 2020 2020 2020 2020 2070 7265 6369 7369           precisi
-000011b0: 6f6e 203d 206d 696e 2864 6563 696d 616c  on = min(decimal
-000011c0: 732c 2073 6967 6e69 6669 6361 6e74 5f66  s, significant_f
-000011d0: 6967 7572 6573 202d 2064 6967 6974 7329  igures - digits)
-000011e0: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
-000011f0: 6563 6973 696f 6e20 3d20 6d61 7828 7072  ecision = max(pr
-00001200: 6563 6973 696f 6e2c 2030 290d 0a20 2020  ecision, 0)..   
-00001210: 2020 2020 2020 2020 2069 6620 6162 7328           if abs(
-00001220: 7661 6c75 6529 203e 3d20 302e 3120 6f72  value) >= 0.1 or
-00001230: 2070 7265 6369 7369 6f6e 203c 2073 6967   precision < sig
-00001240: 6e69 6669 6361 6e74 5f66 6967 7572 6573  nificant_figures
-00001250: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00001260: 2020 2023 2052 656d 6f76 6520 7472 6169     # Remove trai
-00001270: 6c69 6e67 207a 6572 6f73 2061 6e64 2072  ling zeros and r
-00001280: 6574 7572 6e0d 0a20 2020 2020 2020 2020  eturn..         
-00001290: 2020 2020 2020 2072 6574 7572 6e20 6627         return f'
-000012a0: 7b76 616c 7565 3a2e 7b70 7265 6369 7369  {value:.{precisi
-000012b0: 6f6e 7d66 7d27 2e72 7374 7269 7028 2730  on}f}'.rstrip('0
-000012c0: 2729 2e72 7374 7269 7028 272e 2729 202b  ').rstrip('.') +
-000012d0: 2066 2720 7b75 6e69 747d 270d 0a20 2020   f' {unit}'..   
-000012e0: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-000012f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001300: 7620 3d20 6627 7b76 616c 7565 3a2e 7b73  v = f'{value:.{s
-00001310: 6967 6e69 6669 6361 6e74 5f66 6967 7572  ignificant_figur
-00001320: 6573 7d65 7d27 0d0a 2020 2020 2020 2020  es}e}'..        
-00001330: 2020 2020 2020 2020 2320 5265 6d6f 7665          # Remove
-00001340: 2074 7261 696c 696e 6720 7a65 726f 7320   trailing zeros 
-00001350: 6265 666f 7265 2027 6527 2061 6e64 2072  before 'e' and r
-00001360: 6574 7572 6e0d 0a20 2020 2020 2020 2020  eturn..         
-00001370: 2020 2020 2020 2074 203d 2076 2e73 706c         t = v.spl
-00001380: 6974 2827 6527 290d 0a20 2020 2020 2020  it('e')..       
-00001390: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000013a0: 6627 7b74 5b30 5d2e 7273 7472 6970 2822  f'{t[0].rstrip("
-000013b0: 3022 292e 7273 7472 6970 2822 2e22 297d  0").rstrip(".")}
-000013c0: 657b 745b 315d 7d27 202b 2066 2720 207b  e{t[1]}' + f'  {
-000013d0: 756e 6974 7d27 0d0a 2020 2020 2020 2020  unit}'..        
-000013e0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-000013f0: 2020 2072 6574 7572 6e20 6627 7b76 616c     return f'{val
-00001400: 7565 3a7b 666d 747d 7d27 202b 2066 2720  ue:{fmt}}' + f' 
-00001410: 7b75 6e69 747d 270d 0a0d 0a20 2020 2040  {unit}'....    @
-00001420: 636c 6173 736d 6574 686f 640d 0a20 2020  classmethod..   
-00001430: 2064 6566 206c 6f61 6428 0d0a 2020 2020   def load(..    
-00001440: 2020 2020 636c 732c 2063 6f6d 702c 2070      cls, comp, p
-00001450: 6172 656e 743a 2022 436f 6d6d 616e 6449  arent: "CommandI
-00001460: 7465 6d22 203d 204e 6f6e 6529 202d 3e20  tem" = None) -> 
-00001470: 2243 6f6d 6d61 6e64 4974 656d 223a 0d0a  "CommandItem":..
-00001480: 2020 2020 2020 2020 2222 2243 7265 6174          """Creat
-00001490: 6520 6120 2772 6f6f 7427 2043 6f6d 6d61  e a 'root' Comma
-000014a0: 6e64 4974 656d 2066 726f 6d20 6120 436f  ndItem from a Co
-000014b0: 6d70 6f6e 656e 7420 616e 6420 0d0a 2020  mponent and ..  
-000014c0: 2020 2020 2020 706f 7075 6c61 7465 2069        populate i
-000014d0: 7473 2073 7562 636f 6d70 6f6e 656e 7420  ts subcomponent 
-000014e0: 616e 6420 636f 6d6d 616e 6473 2072 6563  and commands rec
-000014f0: 7572 7369 7665 6c79 2e0d 0a0d 0a20 2020  ursively.....   
-00001500: 2020 2020 2052 6574 7572 6e73 3a0d 0a20       Returns:.. 
-00001510: 2020 2020 2020 2020 2020 2043 6f6d 6d61             Comma
-00001520: 6e64 4974 656d 3a20 436f 6d6d 616e 6449  ndItem: CommandI
-00001530: 7465 6d0d 0a20 2020 2020 2020 2022 2222  tem..        """
-00001540: 0d0a 2020 2020 2020 2020 726f 6f74 5f69  ..        root_i
-00001550: 7465 6d20 3d20 436f 6d6d 616e 6449 7465  tem = CommandIte
-00001560: 6d28 7061 7265 6e74 290d 0a20 2020 2020  m(parent)..     
-00001570: 2020 2072 6f6f 745f 6974 656d 2e6e 616d     root_item.nam
-00001580: 6520 3d20 2272 6f6f 7422 0d0a 2020 2020  e = "root"..    
-00001590: 2020 2020 726f 6f74 5f69 7465 6d2e 636f      root_item.co
-000015a0: 6d70 203d 2063 6f6d 700d 0a0d 0a20 2020  mp = comp....   
-000015b0: 2020 2020 2069 6620 6973 7375 6263 6c61       if issubcla
-000015c0: 7373 2863 6f6d 702e 5f5f 636c 6173 735f  ss(comp.__class_
-000015d0: 5f2c 2043 6f6d 706f 6e65 6e74 293a 0d0a  _, Component):..
-000015e0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000015f0: 6a20 696e 2063 6f6d 702e 5f5f 6469 6374  j in comp.__dict
-00001600: 5f5f 3a0d 0a20 2020 2020 2020 2020 2020  __:..           
-00001610: 2020 2020 2069 6620 6a20 3d3d 2027 5f70       if j == '_p
-00001620: 6172 656e 7427 3a0d 0a20 2020 2020 2020  arent':..       
-00001630: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00001640: 7469 6e75 650d 0a20 2020 2020 2020 2020  tinue..         
-00001650: 2020 2020 2020 2069 6e73 7461 6e63 6520         instance 
-00001660: 3d20 636f 6d70 2e5f 5f64 6963 745f 5f5b  = comp.__dict__[
-00001670: 6a5d 0d0a 2020 2020 2020 2020 2020 2020  j]..            
-00001680: 2020 2020 6966 2069 7373 7562 636c 6173      if issubclas
-00001690: 7328 696e 7374 616e 6365 2e5f 5f63 6c61  s(instance.__cla
-000016a0: 7373 5f5f 2c20 2043 6f6d 706f 6e65 6e74  ss__,  Component
-000016b0: 293a 2020 2020 2020 2020 2020 2020 2020  ):              
-000016c0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-000016d0: 2020 2020 2020 2020 6368 696c 6420 3d20          child = 
-000016e0: 636c 732e 6c6f 6164 2869 6e73 7461 6e63  cls.load(instanc
-000016f0: 652c 2072 6f6f 745f 6974 656d 290d 0a20  e, root_item).. 
-00001700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001710: 2020 2063 6869 6c64 2e6e 616d 6520 3d20     child.name = 
-00001720: 6a0d 0a20 2020 2020 2020 2020 2020 2020  j..             
-00001730: 2020 2020 2020 2063 6869 6c64 2e63 6f6d         child.com
-00001740: 7020 3d20 696e 7374 616e 6365 0d0a 2020  p = instance..  
-00001750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001760: 2020 6966 2069 6e73 7461 6e63 6520 696e    if instance in
-00001770: 2063 6f6d 702e 6578 636c 7564 655f 6361   comp.exclude_ca
-00001780: 7074 7572 653a 0d0a 2020 2020 2020 2020  pture:..        
-00001790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017a0: 6368 696c 642e 6578 636c 7564 6564 203d  child.excluded =
-000017b0: 2054 7275 650d 0a20 2020 2020 2020 2020   True..         
-000017c0: 2020 2020 2020 2020 2020 2063 6869 6c64             child
-000017d0: 2e63 6f6d 705f 7479 7065 203d 2074 7970  .comp_type = typ
-000017e0: 6528 696e 7374 616e 6365 290d 0a20 2020  e(instance)..   
-000017f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001800: 2072 6f6f 745f 6974 656d 2e61 7070 656e   root_item.appen
-00001810: 6443 6869 6c64 2863 6869 6c64 290d 0a0d  dChild(child)...
-00001820: 0a20 2020 2020 2020 2020 2020 2063 7572  .            cur
-00001830: 7265 6e74 5f61 7474 7269 6275 7465 7320  rent_attributes 
-00001840: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00001850: 2020 666f 7220 6320 696e 2063 6f6d 702e    for c in comp.
-00001860: 5f5f 636c 6173 735f 5f2e 5f5f 6d72 6f5f  __class__.__mro_
-00001870: 5f3a 2020 2320 6c6f 6f70 2074 6872 6f75  _:  # loop throu
-00001880: 6768 2074 6865 2063 6c61 7373 6573 2069  gh the classes i
-00001890: 6e63 6c75 6469 6e67 2073 7570 6572 2063  ncluding super c
-000018a0: 6c61 7373 6573 0d0a 2020 2020 2020 2020  lasses..        
-000018b0: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
-000018c0: 7373 7562 636c 6173 7328 632c 2043 6f6d  ssubclass(c, Com
-000018d0: 706f 6e65 6e74 293a 2020 2320 6974 2073  ponent):  # it s
-000018e0: 686f 756c 6420 6265 2061 2073 7562 636c  hould be a subcl
-000018f0: 6173 7320 6f66 2043 6f6d 706f 6e65 6e74  ass of Component
-00001900: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001910: 2020 2020 2020 6272 6561 6b0d 0a20 2020        break..   
-00001920: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00001930: 6320 3d3d 2043 6f6d 706f 6e65 6e74 3a20  c == Component: 
-00001940: 2023 2042 7574 2069 7420 7368 6f75 6c64   # But it should
-00001950: 206e 6f74 2062 6520 436f 6d70 6f6e 656e   not be Componen
-00001960: 740d 0a20 2020 2020 2020 2020 2020 2020  t..             
-00001970: 2020 2020 2020 2062 7265 616b 0d0a 0d0a         break....
-00001980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001990: 666f 7220 6b65 7920 696e 2063 2e5f 5f64  for key in c.__d
-000019a0: 6963 745f 5f3a 0d0a 2020 2020 2020 2020  ict__:..        
-000019b0: 2020 2020 2020 2020 2020 2020 636d 645f              cmd_
-000019c0: 696e 7374 616e 6365 203d 2063 2e5f 5f64  instance = c.__d
-000019d0: 6963 745f 5f5b 6b65 795d 0d0a 2020 2020  ict__[key]..    
-000019e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019f0: 6966 206b 6579 2069 6e20 6375 7272 656e  if key in curren
-00001a00: 745f 6174 7472 6962 7574 6573 3a0d 0a20  t_attributes:.. 
-00001a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a20: 2020 2020 2020 2063 6f6e 7469 6e75 650d         continue.
-00001a30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001a40: 2020 2020 2063 7572 7265 6e74 5f61 7474       current_att
-00001a50: 7269 6275 7465 732e 6170 7065 6e64 286b  ributes.append(k
-00001a60: 6579 290d 0a0d 0a20 2020 2020 2020 2020  ey)....         
-00001a70: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-00001a80: 7375 6263 6c61 7373 2863 6d64 5f69 6e73  subclass(cmd_ins
-00001a90: 7461 6e63 652e 5f5f 636c 6173 735f 5f2c  tance.__class__,
-00001aa0: 2043 6f6d 6d61 6e64 293a 0d0a 2020 2020   Command):..    
-00001ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ac0: 2020 2020 6368 696c 6420 3d20 636c 732e      child = cls.
-00001ad0: 6c6f 6164 2863 6d64 5f69 6e73 7461 6e63  load(cmd_instanc
-00001ae0: 652c 2072 6f6f 745f 6974 656d 290d 0a20  e, root_item).. 
-00001af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b00: 2020 2020 2020 2063 6869 6c64 2e6e 616d         child.nam
-00001b10: 6520 3d20 6b65 790d 0a20 2020 2020 2020  e = key..       
-00001b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b30: 2063 6869 6c64 2e63 6f6d 7020 3d20 636d   child.comp = cm
-00001b40: 645f 696e 7374 616e 6365 0d0a 2020 2020  d_instance..    
-00001b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b60: 2020 2020 6368 696c 642e 636f 6d70 5f74      child.comp_t
-00001b70: 7970 6520 3d20 7479 7065 2863 6d64 5f69  ype = type(cmd_i
-00001b80: 6e73 7461 6e63 6529 0d0a 0d0a 2020 2020  nstance)....    
-00001b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ba0: 2020 2020 726f 6f74 5f69 7465 6d2e 6170      root_item.ap
-00001bb0: 7065 6e64 4368 696c 6428 6368 696c 6429  pendChild(child)
-00001bc0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00001bd0: 2020 2020 2020 2020 656c 6966 2069 7373          elif iss
-00001be0: 7562 636c 6173 7328 636d 645f 696e 7374  ubclass(cmd_inst
-00001bf0: 616e 6365 2e5f 5f63 6c61 7373 5f5f 2c20  ance.__class__, 
-00001c00: 496e 6465 7843 6f6d 6d61 6e64 293a 0d0a  IndexCommand):..
-00001c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c20: 2020 2020 2020 2020 6368 696c 6420 3d20          child = 
-00001c30: 636c 732e 6c6f 6164 2863 6d64 5f69 6e73  cls.load(cmd_ins
-00001c40: 7461 6e63 652c 2072 6f6f 745f 6974 656d  tance, root_item
-00001c50: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00001c60: 2020 2020 2020 2020 2020 2063 6869 6c64             child
-00001c70: 2e6e 616d 6520 3d20 6b65 790d 0a20 2020  .name = key..   
-00001c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c90: 2020 2020 2063 6869 6c64 2e63 6f6d 7020       child.comp 
-00001ca0: 3d20 636d 645f 696e 7374 616e 6365 0d0a  = cmd_instance..
+00000000: 0d0a 696d 706f 7274 2074 696d 650d 0a66  ..import time..f
+00000010: 726f 6d20 7372 7367 7569 2069 6d70 6f72  rom srsgui impor
+00000020: 7420 436f 6d70 6f6e 656e 740d 0a66 726f  t Component..fro
+00000030: 6d20 7372 7367 7569 2e69 6e73 7420 696d  m srsgui.inst im
+00000040: 706f 7274 2043 6f6d 6d61 6e64 2c20 496e  port Command, In
+00000050: 6465 7843 6f6d 6d61 6e64 2c20 5c0d 0a20  dexCommand, \.. 
+00000060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000070: 2020 2020 2020 2046 6c6f 6174 436f 6d6d         FloatComm
+00000080: 616e 642c 2046 6c6f 6174 496e 6465 7843  and, FloatIndexC
+00000090: 6f6d 6d61 6e64 0d0a 0d0a 0d0a 636c 6173  ommand......clas
+000000a0: 7320 496e 6465 783a 0d0a 2020 2020 7061  s Index:..    pa
+000000b0: 7373 0d0a 0d0a 0d0a 636c 6173 7320 436f  ss......class Co
+000000c0: 6d6d 616e 6449 7465 6d3a 0d0a 2020 2020  mmandItem:..    
+000000d0: 2222 2241 2043 6f6d 6d61 6e64 2069 7465  """A Command ite
+000000e0: 6d20 636f 7272 6573 706f 6e64 696e 6720  m corresponding 
+000000f0: 746f 2061 206c 696e 6520 696e 2051 5472  to a line in QTr
+00000100: 6565 5669 6577 2222 220d 0a0d 0a20 2020  eeView"""....   
+00000110: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+00000120: 6c66 2c20 7061 7265 6e74 3a20 2243 6f6d  lf, parent: "Com
+00000130: 6d61 6e64 4974 656d 2220 3d20 4e6f 6e65  mandItem" = None
+00000140: 293a 0d0a 2020 2020 2020 2020 7365 6c66  ):..        self
+00000150: 2e5f 7061 7265 6e74 203d 2070 6172 656e  ._parent = paren
+00000160: 740d 0a20 2020 2020 2020 2073 656c 662e  t..        self.
+00000170: 5f63 6869 6c64 7265 6e20 3d20 5b5d 0d0a  _children = []..
+00000180: 2020 2020 2020 2020 7365 6c66 2e5f 7661          self._va
+00000190: 6c75 6520 3d20 4e6f 6e65 0d0a 2020 2020  lue = None..    
+000001a0: 2020 2020 0d0a 2020 2020 2020 2020 7365      ..        se
+000001b0: 6c66 2e6e 616d 6520 3d20 2222 0d0a 2020  lf.name = ""..  
+000001c0: 2020 2020 2020 7365 6c66 2e76 616c 7565        self.value
+000001d0: 5f74 7970 6520 3d20 4e6f 6e65 2020 2320  _type = None  # 
+000001e0: 5468 6572 6520 6172 6520 3320 7479 7065  There are 3 type
+000001f0: 7320 6f66 2076 616c 7565 733a 2073 7472  s of values: str
+00000200: 2c20 696e 742c 2061 6e64 2066 6c6f 6174  , int, and float
+00000210: 0d0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
+00000220: 7265 6369 7369 6f6e 203d 2034 0d0a 2020  recision = 4..  
+00000230: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00000240: 7365 6c66 2e63 6f6d 7020 3d20 4e6f 6e65  self.comp = None
+00000250: 0d0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
+00000260: 6f6d 705f 7479 7065 203d 204e 6f6e 6520  omp_type = None 
+00000270: 2020 2320 5468 6572 6520 6172 6520 3520    # There are 5 
+00000280: 7479 7065 7320 6f66 2063 6f6d 706f 6e65  types of compone
+00000290: 6e74 733a 2043 6f6d 706f 6e65 6e74 2c20  nts: Component, 
+000002a0: 436f 6d6d 616e 6473 2c20 496e 6465 7843  Commands, IndexC
+000002b0: 6f6d 6d61 6e64 732c 206d 6574 686f 6420  ommands, method 
+000002c0: 616e 6420 496e 6465 780d 0a20 2020 2020  and Index..     
+000002d0: 2020 2073 656c 662e 7365 745f 656e 6162     self.set_enab
+000002e0: 6c65 203d 2046 616c 7365 0d0a 2020 2020  le = False..    
+000002f0: 2020 2020 7365 6c66 2e67 6574 5f65 6e61      self.get_ena
+00000300: 626c 6520 3d20 4661 6c73 650d 0a20 2020  ble = False..   
+00000310: 2020 2020 2073 656c 662e 6973 5f6d 6574       self.is_met
+00000320: 686f 6420 3d20 4661 6c73 650d 0a20 2020  hod = False..   
+00000330: 2020 2020 2073 656c 662e 6578 636c 7564       self.exclud
+00000340: 6564 203d 2046 616c 7365 0d0a 2020 2020  ed = False..    
+00000350: 2020 2020 7365 6c66 2e72 6177 5f72 656d      self.raw_rem
+00000360: 6f74 655f 636f 6d6d 616e 6420 3d20 2222  ote_command = ""
+00000370: 0d0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
+00000380: 696d 6573 7461 6d70 203d 2030 2e30 0d0a  imestamp = 0.0..
+00000390: 0d0a 2020 2020 6465 6620 6170 7065 6e64  ..    def append
+000003a0: 4368 696c 6428 7365 6c66 2c20 6974 656d  Child(self, item
+000003b0: 3a20 2243 6f6d 6d61 6e64 4974 656d 2229  : "CommandItem")
+000003c0: 3a0d 0a20 2020 2020 2020 2022 2222 4164  :..        """Ad
+000003d0: 6420 6974 656d 2061 7320 6120 6368 696c  d item as a chil
+000003e0: 6422 2222 0d0a 2020 2020 2020 2020 7365  d"""..        se
+000003f0: 6c66 2e5f 6368 696c 6472 656e 2e61 7070  lf._children.app
+00000400: 656e 6428 6974 656d 290d 0a0d 0a20 2020  end(item)....   
+00000410: 2064 6566 2063 6869 6c64 2873 656c 662c   def child(self,
+00000420: 2072 6f77 3a20 696e 7429 202d 3e20 2243   row: int) -> "C
+00000430: 6f6d 6d61 6e64 4974 656d 223a 0d0a 2020  ommandItem":..  
+00000440: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
+00000450: 7468 6520 6368 696c 6420 6f66 2074 6865  the child of the
+00000460: 2063 7572 7265 6e74 2069 7465 6d20 6672   current item fr
+00000470: 6f6d 2074 6865 2067 6976 656e 2072 6f77  om the given row
+00000480: 2222 220d 0a20 2020 2020 2020 2072 6574  """..        ret
+00000490: 7572 6e20 7365 6c66 2e5f 6368 696c 6472  urn self._childr
+000004a0: 656e 5b72 6f77 5d0d 0a0d 0a20 2020 2064  en[row]....    d
+000004b0: 6566 2070 6172 656e 7428 7365 6c66 2920  ef parent(self) 
+000004c0: 2d3e 2022 436f 6d6d 616e 6449 7465 6d22  -> "CommandItem"
+000004d0: 3a0d 0a20 2020 2020 2020 2022 2222 5265  :..        """Re
+000004e0: 7475 726e 2074 6865 2070 6172 656e 7420  turn the parent 
+000004f0: 6f66 2074 6865 2063 7572 7265 6e74 2069  of the current i
+00000500: 7465 6d22 2222 0d0a 2020 2020 2020 2020  tem"""..        
+00000510: 7265 7475 726e 2073 656c 662e 5f70 6172  return self._par
+00000520: 656e 740d 0a0d 0a20 2020 2064 6566 2063  ent....    def c
+00000530: 6869 6c64 436f 756e 7428 7365 6c66 2920  hildCount(self) 
+00000540: 2d3e 2069 6e74 3a0d 0a20 2020 2020 2020  -> int:..       
+00000550: 2022 2222 5265 7475 726e 2074 6865 206e   """Return the n
+00000560: 756d 6265 7220 6f66 2063 6869 6c64 7265  umber of childre
+00000570: 6e20 6f66 2074 6865 2063 7572 7265 6e74  n of the current
+00000580: 2069 7465 6d22 2222 0d0a 2020 2020 2020   item"""..      
+00000590: 2020 7265 7475 726e 206c 656e 2873 656c    return len(sel
+000005a0: 662e 5f63 6869 6c64 7265 6e29 0d0a 0d0a  f._children)....
+000005b0: 2020 2020 6465 6620 726f 7728 7365 6c66      def row(self
+000005c0: 2920 2d3e 2069 6e74 3a0d 0a20 2020 2020  ) -> int:..     
+000005d0: 2020 2022 2222 5265 7475 726e 2074 6865     """Return the
+000005e0: 2072 6f77 2077 6865 7265 2074 6865 2063   row where the c
+000005f0: 7572 7265 6e74 2069 7465 6d20 6f63 6375  urrent item occu
+00000600: 7069 6573 2069 6e20 7468 6520 7061 7265  pies in the pare
+00000610: 6e74 2222 220d 0a20 2020 2020 2020 2072  nt"""..        r
+00000620: 6574 7572 6e20 7365 6c66 2e5f 7061 7265  eturn self._pare
+00000630: 6e74 2e5f 6368 696c 6472 656e 2e69 6e64  nt._children.ind
+00000640: 6578 2873 656c 6629 2069 6620 7365 6c66  ex(self) if self
+00000650: 2e5f 7061 7265 6e74 2065 6c73 6520 300d  ._parent else 0.
+00000660: 0a0d 0a20 2020 2040 7072 6f70 6572 7479  ...    @property
+00000670: 0d0a 2020 2020 6465 6620 7661 6c75 6528  ..    def value(
+00000680: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00000690: 2222 2252 6574 7572 6e20 7468 6520 7661  """Return the va
+000006a0: 6c75 6520 6f66 2074 6865 2063 7572 7265  lue of the curre
+000006b0: 6e74 2069 7465 6d22 2222 0d0a 2020 2020  nt item"""..    
+000006c0: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+000006d0: 2020 2020 2020 7473 203d 2074 696d 652e        ts = time.
+000006e0: 7469 6d65 2829 0d0a 2020 2020 2020 2020  time()..        
+000006f0: 2020 2020 6966 2074 7320 2d20 7365 6c66      if ts - self
+00000700: 2e74 696d 6573 7461 6d70 203c 2030 2e31  .timestamp < 0.1
+00000710: 3a20 2320 5570 6461 7465 2076 616c 7565  : # Update value
+00000720: 206c 6174 6572 2074 6861 6e20 302e 3120   later than 0.1 
+00000730: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
+00000740: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00000750: 7661 6c75 650d 0a0d 0a20 2020 2020 2020  value....       
+00000760: 2020 2020 2069 6620 7365 6c66 2e63 6f6d       if self.com
+00000770: 705f 7479 7065 203d 3d20 496e 6465 7820  p_type == Index 
+00000780: 616e 6420 7365 6c66 2e67 6574 5f65 6e61  and self.get_ena
+00000790: 626c 6520 616e 6420 6e6f 7420 7365 6c66  ble and not self
+000007a0: 2e65 7863 6c75 6465 643a 0d0a 2020 2020  .excluded:..    
+000007b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000007c0: 2e5f 7661 6c75 6520 3d20 7365 6c66 2e5f  ._value = self._
+000007d0: 7061 7265 6e74 2e63 6f6d 702e 5f5f 6765  parent.comp.__ge
+000007e0: 7469 7465 6d5f 5f28 7365 6c66 2e63 6f6d  titem__(self.com
+000007f0: 7029 0d0a 2020 2020 2020 2020 2020 2020  p)..            
+00000800: 2020 2020 7365 6c66 2e5f 7661 6c75 655f      self._value_
+00000810: 7479 7065 203d 2074 7970 6528 7365 6c66  type = type(self
+00000820: 2e5f 7661 6c75 6529 0d0a 2020 2020 2020  ._value)..      
+00000830: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+00000840: 696d 6573 7461 6d70 203d 2074 730d 0a20  imestamp = ts.. 
+00000850: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00000860: 6973 7375 6263 6c61 7373 2874 7970 6528  issubclass(type(
+00000870: 7365 6c66 2e63 6f6d 7029 2c20 436f 6d6d  self.comp), Comm
+00000880: 616e 6429 2061 6e64 2073 656c 662e 6765  and) and self.ge
+00000890: 745f 656e 6162 6c65 2061 6e64 206e 6f74  t_enable and not
+000008a0: 2073 656c 662e 6578 636c 7564 6564 3a0d   self.excluded:.
+000008b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000008c0: 2073 656c 662e 5f76 616c 7565 203d 2073   self._value = s
+000008d0: 656c 662e 636f 6d70 2e5f 5f67 6574 5f5f  elf.comp.__get__
+000008e0: 2873 656c 662e 5f70 6172 656e 742e 636f  (self._parent.co
+000008f0: 6d70 2c20 7365 6c66 2e5f 7061 7265 6e74  mp, self._parent
+00000900: 2e63 6f6d 702e 5f5f 636c 6173 735f 5f29  .comp.__class__)
+00000910: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000920: 2020 7365 6c66 2e5f 7661 6c75 655f 7479    self._value_ty
+00000930: 7065 203d 2074 7970 6528 7365 6c66 2e5f  pe = type(self._
+00000940: 7661 6c75 6529 0d0a 2020 2020 2020 2020  value)..        
+00000950: 2020 2020 2020 2020 7365 6c66 2e74 696d          self.tim
+00000960: 6573 7461 6d70 203d 2074 730d 0a20 2020  estamp = ts..   
+00000970: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+00000980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000990: 7365 6c66 2e5f 7661 6c75 655f 7479 7065  self._value_type
+000009a0: 203d 2074 7970 6528 7365 6c66 2e5f 7661   = type(self._va
+000009b0: 6c75 6529 0d0a 0d0a 2020 2020 2020 2020  lue)....        
+000009c0: 2020 2020 2320 526f 756e 6420 666c 6f61      # Round floa
+000009d0: 7420 746f 2069 7473 2070 7265 6369 7369  t to its precisi
+000009e0: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
+000009f0: 6966 2073 656c 662e 636f 6d70 5f74 7970  if self.comp_typ
+00000a00: 6520 3d3d 2046 6c6f 6174 436f 6d6d 616e  e == FloatComman
+00000a10: 643a 0d0a 2020 2020 2020 2020 2020 2020  d:..            
+00000a20: 2020 2020 7365 6c66 2e5f 7661 6c75 6520      self._value 
+00000a30: 3d20 726f 756e 6428 7365 6c66 2e5f 7661  = round(self._va
+00000a40: 6c75 652c 2073 656c 662e 7072 6563 6973  lue, self.precis
+00000a50: 696f 6e29 0d0a 2020 2020 2020 2020 2020  ion)..          
+00000a60: 2020 656c 6966 2073 656c 662e 636f 6d70    elif self.comp
+00000a70: 5f74 7970 6520 3d3d 2049 6e64 6578 2061  _type == Index a
+00000a80: 6e64 2073 656c 662e 5f70 6172 656e 742e  nd self._parent.
+00000a90: 636f 6d70 5f74 7970 6520 3d3d 2046 6c6f  comp_type == Flo
+00000aa0: 6174 496e 6465 7843 6f6d 6d61 6e64 3a0d  atIndexCommand:.
+00000ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000ac0: 2073 656c 662e 5f76 616c 7565 203d 2072   self._value = r
+00000ad0: 6f75 6e64 2873 656c 662e 5f76 616c 7565  ound(self._value
+00000ae0: 2c20 7365 6c66 2e70 7265 6369 7369 6f6e  , self.precision
+00000af0: 290d 0a20 2020 2020 2020 2065 7863 6570  )..        excep
+00000b00: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+00000b10: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
+00000b20: 7269 6e74 2865 2c20 7365 6c66 2e6e 616d  rint(e, self.nam
+00000b30: 6529 0d0a 2020 2020 2020 2020 7265 7475  e)..        retu
+00000b40: 726e 2073 656c 662e 5f76 616c 7565 0d0a  rn self._value..
+00000b50: 0d0a 2020 2020 4076 616c 7565 2e73 6574  ..    @value.set
+00000b60: 7465 720d 0a20 2020 2064 6566 2076 616c  ter..    def val
+00000b70: 7565 2873 656c 662c 2076 616c 7565 293a  ue(self, value):
+00000b80: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+00000b90: 7661 6c75 6520 3d20 7661 6c75 650d 0a0d  value = value...
+00000ba0: 0a20 2020 2064 6566 2073 6574 5f76 616c  .    def set_val
+00000bb0: 7565 2873 656c 662c 2076 616c 7565 293a  ue(self, value):
+00000bc0: 0d0a 2020 2020 2020 2020 2222 2253 6574  ..        """Set
+00000bd0: 2076 616c 7565 2074 6f20 7468 6520 696e   value to the in
+00000be0: 7374 7275 6d65 6e74 2061 6e64 2075 7064  strument and upd
+00000bf0: 6174 6520 7468 6520 7661 6c75 6520 6f66  ate the value of
+00000c00: 2074 6865 2069 7465 6d22 2222 0d0a 2020   the item"""..  
+00000c10: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
+00000c20: 6d70 5f74 7970 6520 3d3d 2049 6e64 6578  mp_type == Index
+00000c30: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00000c40: 656c 662e 5f70 6172 656e 742e 636f 6d70  elf._parent.comp
+00000c50: 2e5f 5f73 6574 6974 656d 5f5f 2873 656c  .__setitem__(sel
+00000c60: 662e 636f 6d70 2c20 7661 6c75 6529 0d0a  f.comp, value)..
+00000c70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00000c80: 2e5f 7661 6c75 6520 3d20 7365 6c66 2e5f  ._value = self._
+00000c90: 7061 7265 6e74 2e63 6f6d 702e 5f5f 6765  parent.comp.__ge
+00000ca0: 7469 7465 6d5f 5f28 7365 6c66 2e63 6f6d  titem__(self.com
+00000cb0: 7029 0d0a 2020 2020 2020 2020 2020 2020  p)..            
+00000cc0: 7365 6c66 2e74 696d 6573 7461 6d70 203d  self.timestamp =
+00000cd0: 2074 696d 652e 7469 6d65 2829 0d0a 2020   time.time()..  
+00000ce0: 2020 2020 2020 656c 6966 2069 7373 7562        elif issub
+00000cf0: 636c 6173 7328 7479 7065 2873 656c 662e  class(type(self.
+00000d00: 636f 6d70 292c 2043 6f6d 6d61 6e64 293a  comp), Command):
+00000d10: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00000d20: 6c66 2e63 6f6d 702e 5f5f 7365 745f 5f28  lf.comp.__set__(
+00000d30: 7365 6c66 2e5f 7061 7265 6e74 2e63 6f6d  self._parent.com
+00000d40: 702c 2076 616c 7565 290d 0a20 2020 2020  p, value)..     
+00000d50: 2020 2020 2020 2073 656c 662e 5f76 616c         self._val
+00000d60: 7565 203d 2073 656c 662e 636f 6d70 2e5f  ue = self.comp._
+00000d70: 5f67 6574 5f5f 2873 656c 662e 5f70 6172  _get__(self._par
+00000d80: 656e 742e 636f 6d70 2c20 7365 6c66 2e5f  ent.comp, self._
+00000d90: 7061 7265 6e74 2e63 6f6d 702e 5f5f 636c  parent.comp.__cl
+00000da0: 6173 735f 5f29 0d0a 2020 2020 2020 2020  ass__)..        
+00000db0: 2020 2020 7365 6c66 2e74 696d 6573 7461      self.timesta
+00000dc0: 6d70 203d 2074 696d 652e 7469 6d65 2829  mp = time.time()
+00000dd0: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
+00000de0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00000df0: 662e 5f76 616c 7565 203d 2076 616c 7565  f._value = value
+00000e00: 0d0a 0d0a 2020 2020 6465 6620 6973 5f65  ....    def is_e
+00000e10: 6469 7461 626c 6528 7365 6c66 293a 0d0a  ditable(self):..
+00000e20: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
+00000e30: 6e20 5472 7565 2069 6620 7468 6520 6974  n True if the it
+00000e40: 656d 2069 7320 6564 6974 6162 6c65 2222  em is editable""
+00000e50: 220d 0a20 2020 2020 2020 2069 6620 7365  "..        if se
+00000e60: 6c66 2e63 6f6d 705f 7479 7065 203d 3d20  lf.comp_type == 
+00000e70: 496e 6465 7820 616e 6420 5c0d 0a20 2020  Index and \..   
+00000e80: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00000e90: 662e 7365 745f 656e 6162 6c65 2061 6e64  f.set_enable and
+00000ea0: 2073 656c 662e 6765 745f 656e 6162 6c65   self.get_enable
+00000eb0: 2061 6e64 206e 6f74 2073 656c 662e 6578   and not self.ex
+00000ec0: 636c 7564 6564 3a0d 0a20 2020 2020 2020  cluded:..       
+00000ed0: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+00000ee0: 0d0a 2020 2020 2020 2020 656c 6966 2069  ..        elif i
+00000ef0: 7373 7562 636c 6173 7328 7479 7065 2873  ssubclass(type(s
+00000f00: 656c 662e 636f 6d70 292c 2043 6f6d 6d61  elf.comp), Comma
+00000f10: 6e64 2920 616e 6420 5c0d 0a20 2020 2020  nd) and \..     
+00000f20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00000f30: 7365 745f 656e 6162 6c65 2061 6e64 2073  set_enable and s
+00000f40: 656c 662e 6765 745f 656e 6162 6c65 2061  elf.get_enable a
+00000f50: 6e64 206e 6f74 2073 656c 662e 6578 636c  nd not self.excl
+00000f60: 7564 6564 3a0d 0a20 2020 2020 2020 2020  uded:..         
+00000f70: 2020 2072 6574 7572 6e20 5472 7565 0d0a     return True..
+00000f80: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00000f90: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00000fa0: 6e20 4661 6c73 650d 0a0d 0a20 2020 2064  n False....    d
+00000fb0: 6566 2067 6574 5f75 6e69 7428 7365 6c66  ef get_unit(self
+00000fc0: 293a 0d0a 2020 2020 2020 2020 2222 2252  ):..        """R
+00000fd0: 6574 7572 6e20 7468 6520 756e 6974 206f  eturn the unit o
+00000fe0: 6620 7468 6520 6974 656d 2222 220d 0a20  f the item""".. 
+00000ff0: 2020 2020 2020 2063 6f6d 7020 3d20 4e6f         comp = No
+00001000: 6e65 0d0a 2020 2020 2020 2020 6966 2073  ne..        if s
+00001010: 656c 662e 636f 6d70 5f74 7970 6520 3d3d  elf.comp_type ==
+00001020: 2049 6e64 6578 3a0d 0a20 2020 2020 2020   Index:..       
+00001030: 2020 2020 2063 6f6d 7020 3d20 7365 6c66       comp = self
+00001040: 2e70 6172 656e 7428 292e 636f 6d70 0d0a  .parent().comp..
+00001050: 2020 2020 2020 2020 656c 6966 2069 7373          elif iss
+00001060: 7562 636c 6173 7328 7479 7065 2873 656c  ubclass(type(sel
+00001070: 662e 636f 6d70 292c 2043 6f6d 6d61 6e64  f.comp), Command
+00001080: 2920 6f72 205c 0d0a 2020 2020 2020 2020  ) or \..        
+00001090: 2020 2020 2069 7373 7562 636c 6173 7328       issubclass(
+000010a0: 7479 7065 2873 656c 662e 636f 6d70 292c  type(self.comp),
+000010b0: 2049 6e64 6578 436f 6d6d 616e 6429 3a0d   IndexCommand):.
+000010c0: 0a20 2020 2020 2020 2020 2020 2063 6f6d  .            com
+000010d0: 7020 3d20 7365 6c66 2e63 6f6d 700d 0a0d  p = self.comp...
+000010e0: 0a20 2020 2020 2020 2069 6620 636f 6d70  .        if comp
+000010f0: 2061 6e64 2068 6173 6174 7472 2863 6f6d   and hasattr(com
+00001100: 702c 2027 756e 6974 2729 3a0d 0a20 2020  p, 'unit'):..   
+00001110: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00001120: 636f 6d70 2e75 6e69 740d 0a20 2020 2020  comp.unit..     
+00001130: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00001140: 2020 2020 2020 7265 7475 726e 2022 220d        return "".
+00001150: 0a0d 0a20 2020 2064 6566 2067 6574 5f66  ...    def get_f
+00001160: 6f72 6d61 7428 7365 6c66 293a 0d0a 2020  ormat(self):..  
+00001170: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
+00001180: 7468 6520 666f 726d 6174 206f 6620 7468  the format of th
+00001190: 6520 6974 656d 2222 220d 0a20 2020 2020  e item"""..     
+000011a0: 2020 2063 6f6d 7020 3d20 4e6f 6e65 0d0a     comp = None..
+000011b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000011c0: 636f 6d70 5f74 7970 6520 3d3d 2049 6e64  comp_type == Ind
+000011d0: 6578 3a0d 0a20 2020 2020 2020 2020 2020  ex:..           
+000011e0: 2063 6f6d 7020 3d20 7365 6c66 2e70 6172   comp = self.par
+000011f0: 656e 7428 292e 636f 6d70 0d0a 2020 2020  ent().comp..    
+00001200: 2020 2020 656c 6966 2069 7373 7562 636c      elif issubcl
+00001210: 6173 7328 7479 7065 2873 656c 662e 636f  ass(type(self.co
+00001220: 6d70 292c 2043 6f6d 6d61 6e64 2920 6f72  mp), Command) or
+00001230: 205c 0d0a 2020 2020 2020 2020 2020 2020   \..            
+00001240: 2069 7373 7562 636c 6173 7328 7479 7065   issubclass(type
+00001250: 2873 656c 662e 636f 6d70 292c 2049 6e64  (self.comp), Ind
+00001260: 6578 436f 6d6d 616e 6429 3a0d 0a20 2020  exCommand):..   
+00001270: 2020 2020 2020 2020 2063 6f6d 7020 3d20           comp = 
+00001280: 7365 6c66 2e63 6f6d 700d 0a0d 0a20 2020  self.comp....   
+00001290: 2020 2020 2069 6620 636f 6d70 2061 6e64       if comp and
+000012a0: 2068 6173 6174 7472 2863 6f6d 702c 2027   hasattr(comp, '
+000012b0: 666d 7427 293a 0d0a 2020 2020 2020 2020  fmt'):..        
+000012c0: 2020 2020 7265 7475 726e 2063 6f6d 702e      return comp.
+000012d0: 666d 740d 0a20 2020 2020 2020 2065 6c73  fmt..        els
+000012e0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+000012f0: 7265 7475 726e 2027 270d 0a0d 0a20 2020  return ''....   
+00001300: 2040 636c 6173 736d 6574 686f 640d 0a20   @classmethod.. 
+00001310: 2020 2064 6566 206c 6f61 6428 0d0a 2020     def load(..  
+00001320: 2020 2020 2020 636c 732c 2063 6f6d 702c        cls, comp,
+00001330: 2070 6172 656e 743a 2022 436f 6d6d 616e   parent: "Comman
+00001340: 6449 7465 6d22 203d 204e 6f6e 652c 2073  dItem" = None, s
+00001350: 6f72 743d 4661 6c73 650d 0a20 2020 2029  ort=False..    )
+00001360: 202d 3e20 2243 6f6d 6d61 6e64 4974 656d   -> "CommandItem
+00001370: 223a 0d0a 2020 2020 2020 2020 2222 2243  ":..        """C
+00001380: 7265 6174 6520 6120 2772 6f6f 7427 2043  reate a 'root' C
+00001390: 6f6d 6d61 6e64 4974 656d 2066 726f 6d20  ommandItem from 
+000013a0: 6120 436f 6d70 6f6e 656e 7420 616e 6420  a Component and 
+000013b0: 0d0a 2020 2020 2020 2020 706f 7075 6c61  ..        popula
+000013c0: 7465 2069 7473 2073 7562 636f 6d70 6f6e  te its subcompon
+000013d0: 656e 7420 616e 6420 636f 6d6d 616e 6473  ent and commands
+000013e0: 2072 6563 7572 7369 7665 6c79 2e0d 0a0d   recursively....
+000013f0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00001400: 3a0d 0a20 2020 2020 2020 2020 2020 2043  :..            C
+00001410: 6f6d 6d61 6e64 4974 656d 3a20 436f 6d6d  ommandItem: Comm
+00001420: 616e 6449 7465 6d0d 0a20 2020 2020 2020  andItem..       
+00001430: 2022 2222 0d0a 2020 2020 2020 2020 726f   """..        ro
+00001440: 6f74 5f69 7465 6d20 3d20 436f 6d6d 616e  ot_item = Comman
+00001450: 6449 7465 6d28 7061 7265 6e74 290d 0a20  dItem(parent).. 
+00001460: 2020 2020 2020 2072 6f6f 745f 6974 656d         root_item
+00001470: 2e6e 616d 6520 3d20 2272 6f6f 7422 0d0a  .name = "root"..
+00001480: 2020 2020 2020 2020 726f 6f74 5f69 7465          root_ite
+00001490: 6d2e 636f 6d70 203d 2063 6f6d 700d 0a0d  m.comp = comp...
+000014a0: 0a20 2020 2020 2020 2069 6620 6973 7375  .        if issu
+000014b0: 6263 6c61 7373 2863 6f6d 702e 5f5f 636c  bclass(comp.__cl
+000014c0: 6173 735f 5f2c 2043 6f6d 706f 6e65 6e74  ass__, Component
+000014d0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+000014e0: 666f 7220 6a20 696e 2063 6f6d 702e 5f5f  for j in comp.__
+000014f0: 6469 6374 5f5f 3a0d 0a20 2020 2020 2020  dict__:..       
+00001500: 2020 2020 2020 2020 2069 6620 6a20 3d3d           if j ==
+00001510: 2027 5f70 6172 656e 7427 3a0d 0a20 2020   '_parent':..   
+00001520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001530: 2063 6f6e 7469 6e75 650d 0a20 2020 2020   continue..     
+00001540: 2020 2020 2020 2020 2020 2069 6e73 7461             insta
+00001550: 6e63 6520 3d20 636f 6d70 2e5f 5f64 6963  nce = comp.__dic
+00001560: 745f 5f5b 6a5d 0d0a 2020 2020 2020 2020  t__[j]..        
+00001570: 2020 2020 2020 2020 6966 2069 7373 7562          if issub
+00001580: 636c 6173 7328 696e 7374 616e 6365 2e5f  class(instance._
+00001590: 5f63 6c61 7373 5f5f 2c20 2043 6f6d 706f  _class__,  Compo
+000015a0: 6e65 6e74 293a 2020 2020 2020 2020 2020  nent):          
+000015b0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000015c0: 2020 2020 2020 2020 2020 2020 6368 696c              chil
+000015d0: 6420 3d20 636c 732e 6c6f 6164 2869 6e73  d = cls.load(ins
+000015e0: 7461 6e63 652c 2072 6f6f 745f 6974 656d  tance, root_item
+000015f0: 2c20 736f 7274 290d 0a20 2020 2020 2020  , sort)..       
+00001600: 2020 2020 2020 2020 2020 2020 2063 6869               chi
+00001610: 6c64 2e6e 616d 6520 3d20 6a0d 0a20 2020  ld.name = j..   
+00001620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001630: 2063 6869 6c64 2e63 6f6d 7020 3d20 696e   child.comp = in
+00001640: 7374 616e 6365 0d0a 2020 2020 2020 2020  stance..        
+00001650: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00001660: 6e73 7461 6e63 6520 696e 2063 6f6d 702e  nstance in comp.
+00001670: 6578 636c 7564 655f 6361 7074 7572 653a  exclude_capture:
+00001680: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001690: 2020 2020 2020 2020 2020 6368 696c 642e            child.
+000016a0: 6578 636c 7564 6564 203d 2054 7275 650d  excluded = True.
+000016b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000016c0: 2020 2020 2063 6869 6c64 2e63 6f6d 705f       child.comp_
+000016d0: 7479 7065 203d 2074 7970 6528 696e 7374  type = type(inst
+000016e0: 616e 6365 290d 0a20 2020 2020 2020 2020  ance)..         
+000016f0: 2020 2020 2020 2020 2020 2072 6f6f 745f             root_
+00001700: 6974 656d 2e61 7070 656e 6443 6869 6c64  item.appendChild
+00001710: 2863 6869 6c64 290d 0a0d 0a20 2020 2020  (child)....     
+00001720: 2020 2020 2020 2063 7572 7265 6e74 5f61         current_a
+00001730: 7474 7269 6275 7465 7320 3d20 5b5d 0d0a  ttributes = []..
+00001740: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00001750: 6320 696e 2063 6f6d 702e 5f5f 636c 6173  c in comp.__clas
+00001760: 735f 5f2e 5f5f 6d72 6f5f 5f3a 2020 2320  s__.__mro__:  # 
+00001770: 6c6f 6f70 2074 6872 6f75 6768 2074 6865  loop through the
+00001780: 2063 6c61 7373 6573 2069 6e63 6c75 6469   classes includi
+00001790: 6e67 2073 7570 6572 2063 6c61 7373 6573  ng super classes
+000017a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000017b0: 2020 6966 206e 6f74 2069 7373 7562 636c    if not issubcl
+000017c0: 6173 7328 632c 2043 6f6d 706f 6e65 6e74  ass(c, Component
+000017d0: 293a 2020 2320 6974 2073 686f 756c 6420  ):  # it should 
+000017e0: 6265 2061 2073 7562 636c 6173 7320 6f66  be a subclass of
+000017f0: 2043 6f6d 706f 6e65 6e74 0d0a 2020 2020   Component..    
+00001800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001810: 6272 6561 6b0d 0a20 2020 2020 2020 2020  break..         
+00001820: 2020 2020 2020 2069 6620 6320 3d3d 2043         if c == C
+00001830: 6f6d 706f 6e65 6e74 3a20 2023 2042 7574  omponent:  # But
+00001840: 2069 7420 7368 6f75 6c64 206e 6f74 2062   it should not b
+00001850: 6520 436f 6d70 6f6e 656e 740d 0a20 2020  e Component..   
+00001860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001870: 2062 7265 616b 0d0a 0d0a 2020 2020 2020   break....      
+00001880: 2020 2020 2020 2020 2020 666f 7220 6b65            for ke
+00001890: 7920 696e 2063 2e5f 5f64 6963 745f 5f3a  y in c.__dict__:
+000018a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000018b0: 2020 2020 2020 636d 645f 696e 7374 616e        cmd_instan
+000018c0: 6365 203d 2063 2e5f 5f64 6963 745f 5f5b  ce = c.__dict__[
+000018d0: 6b65 795d 0d0a 2020 2020 2020 2020 2020  key]..          
+000018e0: 2020 2020 2020 2020 2020 6966 206b 6579            if key
+000018f0: 2069 6e20 6375 7272 656e 745f 6174 7472   in current_attr
+00001900: 6962 7574 6573 3a0d 0a20 2020 2020 2020  ibutes:..       
+00001910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001920: 2063 6f6e 7469 6e75 650d 0a20 2020 2020   continue..     
+00001930: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00001940: 7572 7265 6e74 5f61 7474 7269 6275 7465  urrent_attribute
+00001950: 732e 6170 7065 6e64 286b 6579 290d 0a0d  s.append(key)...
+00001960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001970: 2020 2020 2069 6620 6973 7375 6263 6c61       if issubcla
+00001980: 7373 2863 6d64 5f69 6e73 7461 6e63 652e  ss(cmd_instance.
+00001990: 5f5f 636c 6173 735f 5f2c 2043 6f6d 6d61  __class__, Comma
+000019a0: 6e64 293a 0d0a 2020 2020 2020 2020 2020  nd):..          
+000019b0: 2020 2020 2020 2020 2020 2020 2020 6368                ch
+000019c0: 696c 6420 3d20 636c 732e 6c6f 6164 2863  ild = cls.load(c
+000019d0: 6d64 5f69 6e73 7461 6e63 652c 2072 6f6f  md_instance, roo
+000019e0: 745f 6974 656d 2c20 736f 7274 290d 0a20  t_item, sort).. 
+000019f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a00: 2020 2020 2020 2063 6869 6c64 2e6e 616d         child.nam
+00001a10: 6520 3d20 6b65 790d 0a20 2020 2020 2020  e = key..       
+00001a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a30: 2063 6869 6c64 2e63 6f6d 7020 3d20 636d   child.comp = cm
+00001a40: 645f 696e 7374 616e 6365 0d0a 2020 2020  d_instance..    
+00001a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a60: 2020 2020 6368 696c 642e 636f 6d70 5f74      child.comp_t
+00001a70: 7970 6520 3d20 7479 7065 2863 6d64 5f69  ype = type(cmd_i
+00001a80: 6e73 7461 6e63 6529 0d0a 0d0a 2020 2020  nstance)....    
+00001a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001aa0: 2020 2020 726f 6f74 5f69 7465 6d2e 6170      root_item.ap
+00001ab0: 7065 6e64 4368 696c 6428 6368 696c 6429  pendChild(child)
+00001ac0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00001ad0: 2020 2020 2020 2020 656c 6966 2069 7373          elif iss
+00001ae0: 7562 636c 6173 7328 636d 645f 696e 7374  ubclass(cmd_inst
+00001af0: 616e 6365 2e5f 5f63 6c61 7373 5f5f 2c20  ance.__class__, 
+00001b00: 496e 6465 7843 6f6d 6d61 6e64 293a 0d0a  IndexCommand):..
+00001b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b20: 2020 2020 2020 2020 6368 696c 6420 3d20          child = 
+00001b30: 636c 732e 6c6f 6164 2863 6d64 5f69 6e73  cls.load(cmd_ins
+00001b40: 7461 6e63 652c 2072 6f6f 745f 6974 656d  tance, root_item
+00001b50: 2c20 736f 7274 290d 0a20 2020 2020 2020  , sort)..       
+00001b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b70: 2063 6869 6c64 2e6e 616d 6520 3d20 6b65   child.name = ke
+00001b80: 790d 0a20 2020 2020 2020 2020 2020 2020  y..             
+00001b90: 2020 2020 2020 2020 2020 2063 6869 6c64             child
+00001ba0: 2e63 6f6d 7020 3d20 636d 645f 696e 7374  .comp = cmd_inst
+00001bb0: 616e 6365 0d0a 2020 2020 2020 2020 2020  ance..          
+00001bc0: 2020 2020 2020 2020 2020 2020 2020 6368                ch
+00001bd0: 696c 642e 636f 6d70 5f74 7970 6520 3d20  ild.comp_type = 
+00001be0: 7479 7065 2863 6d64 5f69 6e73 7461 6e63  type(cmd_instanc
+00001bf0: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+00001c00: 2020 2020 2020 2020 2020 2020 726f 6f74              root
+00001c10: 5f69 7465 6d2e 6170 7065 6e64 4368 696c  _item.appendChil
+00001c20: 6428 6368 696c 6429 0d0a 0d0a 2020 2020  d(child)....    
+00001c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c40: 656c 6966 2063 616c 6c61 626c 6528 636d  elif callable(cm
+00001c50: 645f 696e 7374 616e 6365 293a 0d0a 2020  d_instance):..  
+00001c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c70: 2020 2020 2020 6966 2069 7373 7562 636c        if issubcl
+00001c80: 6173 7328 636d 645f 696e 7374 616e 6365  ass(cmd_instance
+00001c90: 2e5f 5f63 6c61 7373 5f5f 2c20 7479 7065  .__class__, type
+00001ca0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
 00001cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001cc0: 2020 2020 2020 2020 6368 696c 642e 636f          child.co
-00001cd0: 6d70 5f74 7970 6520 3d20 7479 7065 2863  mp_type = type(c
-00001ce0: 6d64 5f69 6e73 7461 6e63 6529 0d0a 2020  md_instance)..  
-00001cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d00: 2020 2020 2020 726f 6f74 5f69 7465 6d2e        root_item.
-00001d10: 6170 7065 6e64 4368 696c 6428 6368 696c  appendChild(chil
-00001d20: 6429 0d0a 0d0a 2020 2020 2020 2020 2020  d)....          
-00001d30: 2020 2020 2020 2020 2020 656c 6966 2063            elif c
-00001d40: 616c 6c61 626c 6528 636d 645f 696e 7374  allable(cmd_inst
-00001d50: 616e 6365 293a 0d0a 2020 2020 2020 2020  ance):..        
-00001d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d70: 6966 2069 7373 7562 636c 6173 7328 636d  if issubclass(cm
-00001d80: 645f 696e 7374 616e 6365 2e5f 5f63 6c61  d_instance.__cla
-00001d90: 7373 5f5f 2c20 7479 7065 293a 0d0a 2020  ss__, type):..  
-00001da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001db0: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-00001dc0: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
-00001dd0: 2020 2020 2020 2020 2020 2020 6966 206b              if k
-00001de0: 6579 2e73 7461 7274 7377 6974 6828 275f  ey.startswith('_
-00001df0: 2729 3a0d 0a20 2020 2020 2020 2020 2020  '):..           
-00001e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e10: 2063 6f6e 7469 6e75 650d 0a20 2020 2020   continue..     
+00001cc0: 636f 6e74 696e 7565 0d0a 2020 2020 2020  continue..      
+00001cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ce0: 2020 6966 206b 6579 2e73 7461 7274 7377    if key.startsw
+00001cf0: 6974 6828 275f 2729 3a0d 0a20 2020 2020  ith('_'):..     
+00001d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d10: 2020 2020 2020 2063 6f6e 7469 6e75 650d         continue.
+00001d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001d30: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00001d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d50: 2020 2063 6869 6c64 203d 2063 6c73 2e6c     child = cls.l
+00001d60: 6f61 6428 636d 645f 696e 7374 616e 6365  oad(cmd_instance
+00001d70: 2c20 726f 6f74 5f69 7465 6d2c 2073 6f72  , root_item, sor
+00001d80: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
+00001d90: 2020 2020 2020 2020 2020 2020 6368 696c              chil
+00001da0: 642e 6e61 6d65 203d 206b 6579 0d0a 2020  d.name = key..  
+00001db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001dc0: 2020 2020 2020 6368 696c 642e 636f 6d70        child.comp
+00001dd0: 203d 2063 6d64 5f69 6e73 7461 6e63 650d   = cmd_instance.
+00001de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001df0: 2020 2020 2020 2020 2063 6869 6c64 2e63           child.c
+00001e00: 6f6d 705f 7479 7065 203d 2074 7970 6528  omp_type = type(
+00001e10: 636d 645f 696e 7374 616e 6365 290d 0a20  cmd_instance).. 
 00001e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e30: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00001e40: 2020 2020 2020 2020 2020 2020 2063 6869               chi
-00001e50: 6c64 203d 2063 6c73 2e6c 6f61 6428 636d  ld = cls.load(cm
-00001e60: 645f 696e 7374 616e 6365 2c20 726f 6f74  d_instance, root
-00001e70: 5f69 7465 6d29 0d0a 2020 2020 2020 2020  _item)..        
-00001e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e90: 6368 696c 642e 6e61 6d65 203d 206b 6579  child.name = key
-00001ea0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001eb0: 2020 2020 2020 2020 2020 6368 696c 642e            child.
-00001ec0: 636f 6d70 203d 2063 6d64 5f69 6e73 7461  comp = cmd_insta
-00001ed0: 6e63 650d 0a20 2020 2020 2020 2020 2020  nce..           
-00001ee0: 2020 2020 2020 2020 2020 2020 2063 6869               chi
-00001ef0: 6c64 2e63 6f6d 705f 7479 7065 203d 2074  ld.comp_type = t
-00001f00: 7970 6528 636d 645f 696e 7374 616e 6365  ype(cmd_instance
-00001f10: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00001f20: 2020 2020 2020 2020 2020 2072 6f6f 745f             root_
-00001f30: 6974 656d 2e61 7070 656e 6443 6869 6c64  item.appendChild
-00001f40: 2863 6869 6c64 290d 0a20 2020 2020 2020  (child)..       
-00001f50: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00001f60: 2020 2020 6966 2063 616c 6c61 626c 6528      if callable(
-00001f70: 636f 6d70 293a 0d0a 2020 2020 2020 2020  comp):..        
-00001f80: 2020 2020 2020 2020 726f 6f74 5f69 7465          root_ite
-00001f90: 6d2e 636f 6d70 203d 2063 6f6d 700d 0a20  m.comp = comp.. 
-00001fa0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00001fb0: 6f6f 745f 6974 656d 2e63 6f6d 705f 7479  oot_item.comp_ty
-00001fc0: 7065 203d 2074 7970 6528 636f 6d70 290d  pe = type(comp).
-00001fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001fe0: 2072 6f6f 745f 6974 656d 2e69 735f 6d65   root_item.is_me
-00001ff0: 7468 6f64 203d 2054 7275 650d 0a0d 0a20  thod = True.... 
-00002000: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00002010: 6973 7375 6263 6c61 7373 2874 7970 6528  issubclass(type(
-00002020: 636f 6d70 292c 2043 6f6d 6d61 6e64 293a  comp), Command):
-00002030: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002040: 2020 726f 6f74 5f69 7465 6d2e 636f 6d70    root_item.comp
-00002050: 203d 2063 6f6d 700d 0a20 2020 2020 2020   = comp..       
-00002060: 2020 2020 2020 2020 2072 6f6f 745f 6974           root_it
-00002070: 656d 2e63 6f6d 705f 7479 7065 203d 2074  em.comp_type = t
-00002080: 7970 6528 636f 6d70 290d 0a20 2020 2020  ype(comp)..     
-00002090: 2020 2020 2020 2020 2020 2072 6f6f 745f             root_
-000020a0: 6974 656d 2e65 7863 6c75 6465 6420 3d20  item.excluded = 
-000020b0: 636f 6d70 2069 6e20 726f 6f74 5f69 7465  comp in root_ite
-000020c0: 6d2e 7061 7265 6e74 2829 2e63 6f6d 702e  m.parent().comp.
-000020d0: 6578 636c 7564 655f 6361 7074 7572 650d  exclude_capture.
-000020e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000020f0: 2072 6f6f 745f 6974 656d 2e72 6177 5f72   root_item.raw_r
-00002100: 656d 6f74 655f 636f 6d6d 616e 6420 3d20  emote_command = 
-00002110: 636f 6d70 2e72 656d 6f74 655f 636f 6d6d  comp.remote_comm
-00002120: 616e 640d 0a20 2020 2020 2020 2020 2020  and..           
-00002130: 2020 2020 2072 6f6f 745f 6974 656d 2e73       root_item.s
-00002140: 6574 5f65 6e61 626c 6520 3d20 636f 6d70  et_enable = comp
-00002150: 2e5f 7365 745f 656e 6162 6c65 0d0a 2020  ._set_enable..  
-00002160: 2020 2020 2020 2020 2020 2020 2020 726f                ro
-00002170: 6f74 5f69 7465 6d2e 6765 745f 656e 6162  ot_item.get_enab
-00002180: 6c65 203d 2063 6f6d 702e 5f67 6574 5f65  le = comp._get_e
-00002190: 6e61 626c 650d 0a0d 0a20 2020 2020 2020  nable....       
-000021a0: 2020 2020 2065 6c69 6620 6973 7375 6263       elif issubc
-000021b0: 6c61 7373 2874 7970 6528 636f 6d70 292c  lass(type(comp),
-000021c0: 2049 6e64 6578 436f 6d6d 616e 6429 3a0d   IndexCommand):.
-000021d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000021e0: 2072 6f6f 745f 6974 656d 2e63 6f6d 7020   root_item.comp 
-000021f0: 3d20 636f 6d70 0d0a 2020 2020 2020 2020  = comp..        
-00002200: 2020 2020 2020 2020 726f 6f74 5f69 7465          root_ite
-00002210: 6d2e 636f 6d70 5f74 7970 6520 3d20 7479  m.comp_type = ty
-00002220: 7065 2863 6f6d 7029 0d0a 2020 2020 2020  pe(comp)..      
-00002230: 2020 2020 2020 2020 2020 726f 6f74 5f69            root_i
-00002240: 7465 6d2e 6578 636c 7564 6564 203d 2063  tem.excluded = c
-00002250: 6f6d 7020 696e 2072 6f6f 745f 6974 656d  omp in root_item
-00002260: 2e70 6172 656e 7428 292e 636f 6d70 2e65  .parent().comp.e
-00002270: 7863 6c75 6465 5f63 6170 7475 7265 0d0a  xclude_capture..
-00002280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002290: 726f 6f74 5f69 7465 6d2e 7261 775f 7265  root_item.raw_re
-000022a0: 6d6f 7465 5f63 6f6d 6d61 6e64 203d 2063  mote_command = c
-000022b0: 6f6d 702e 7265 6d6f 7465 5f63 6f6d 6d61  omp.remote_comma
-000022c0: 6e64 0d0a 2020 2020 2020 2020 2020 2020  nd..            
-000022d0: 2020 2020 726f 6f74 5f69 7465 6d2e 7365      root_item.se
-000022e0: 745f 656e 6162 6c65 203d 2063 6f6d 702e  t_enable = comp.
-000022f0: 5f73 6574 5f65 6e61 626c 650d 0a20 2020  _set_enable..   
-00002300: 2020 2020 2020 2020 2020 2020 2072 6f6f               roo
-00002310: 745f 6974 656d 2e67 6574 5f65 6e61 626c  t_item.get_enabl
-00002320: 6520 3d20 636f 6d70 2e5f 6765 745f 656e  e = comp._get_en
-00002330: 6162 6c65 0d0a 0d0a 2020 2020 2020 2020  able....        
-00002340: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
-00002350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002360: 2020 6966 2063 6f6d 702e 696e 6465 785f    if comp.index_
-00002370: 6469 6374 2069 7320 4e6f 6e65 3a0d 0a20  dict is None:.. 
-00002380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002390: 2020 2020 2020 2069 6e64 6578 203d 2063         index = c
-000023a0: 6f6d 702e 696e 6465 785f 6d69 6e0d 0a20  omp.index_min.. 
-000023b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023c0: 2020 2020 2020 2077 6869 6c65 2069 6e64         while ind
-000023d0: 6578 203c 3d20 636f 6d70 2e69 6e64 6578  ex <= comp.index
-000023e0: 5f6d 6178 3a0d 0a20 2020 2020 2020 2020  _max:..         
-000023f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002400: 2020 2063 6869 6c64 203d 2063 6c73 2e6c     child = cls.l
-00002410: 6f61 6428 696e 6465 782c 2072 6f6f 745f  oad(index, root_
-00002420: 6974 656d 290d 0a20 2020 2020 2020 2020  item)..         
-00002430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002440: 2020 2063 6869 6c64 2e6e 616d 6520 3d20     child.name = 
-00002450: 6627 7b69 6e64 6578 7d27 0d0a 2020 2020  f'{index}'..    
+00001e30: 2020 2020 2020 2072 6f6f 745f 6974 656d         root_item
+00001e40: 2e61 7070 656e 6443 6869 6c64 2863 6869  .appendChild(chi
+00001e50: 6c64 290d 0a20 2020 2020 2020 2065 6c73  ld)..        els
+00001e60: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00001e70: 6966 2063 616c 6c61 626c 6528 636f 6d70  if callable(comp
+00001e80: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00001e90: 2020 2020 726f 6f74 5f69 7465 6d2e 636f      root_item.co
+00001ea0: 6d70 203d 2063 6f6d 700d 0a20 2020 2020  mp = comp..     
+00001eb0: 2020 2020 2020 2020 2020 2072 6f6f 745f             root_
+00001ec0: 6974 656d 2e63 6f6d 705f 7479 7065 203d  item.comp_type =
+00001ed0: 2074 7970 6528 636f 6d70 290d 0a20 2020   type(comp)..   
+00001ee0: 2020 2020 2020 2020 2020 2020 2072 6f6f               roo
+00001ef0: 745f 6974 656d 2e69 735f 6d65 7468 6f64  t_item.is_method
+00001f00: 203d 2054 7275 650d 0a0d 0a20 2020 2020   = True....     
+00001f10: 2020 2020 2020 2065 6c69 6620 6973 7375         elif issu
+00001f20: 6263 6c61 7373 2874 7970 6528 636f 6d70  bclass(type(comp
+00001f30: 292c 2043 6f6d 6d61 6e64 293a 0d0a 2020  ), Command):..  
+00001f40: 2020 2020 2020 2020 2020 2020 2020 726f                ro
+00001f50: 6f74 5f69 7465 6d2e 636f 6d70 203d 2063  ot_item.comp = c
+00001f60: 6f6d 700d 0a20 2020 2020 2020 2020 2020  omp..           
+00001f70: 2020 2020 2072 6f6f 745f 6974 656d 2e63       root_item.c
+00001f80: 6f6d 705f 7479 7065 203d 2074 7970 6528  omp_type = type(
+00001f90: 636f 6d70 290d 0a20 2020 2020 2020 2020  comp)..         
+00001fa0: 2020 2020 2020 2072 6f6f 745f 6974 656d         root_item
+00001fb0: 2e65 7863 6c75 6465 6420 3d20 636f 6d70  .excluded = comp
+00001fc0: 2069 6e20 726f 6f74 5f69 7465 6d2e 7061   in root_item.pa
+00001fd0: 7265 6e74 2829 2e63 6f6d 702e 6578 636c  rent().comp.excl
+00001fe0: 7564 655f 6361 7074 7572 650d 0a20 2020  ude_capture..   
+00001ff0: 2020 2020 2020 2020 2020 2020 2072 6f6f               roo
+00002000: 745f 6974 656d 2e72 6177 5f72 656d 6f74  t_item.raw_remot
+00002010: 655f 636f 6d6d 616e 6420 3d20 636f 6d70  e_command = comp
+00002020: 2e72 656d 6f74 655f 636f 6d6d 616e 640d  .remote_command.
+00002030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002040: 2072 6f6f 745f 6974 656d 2e73 6574 5f65   root_item.set_e
+00002050: 6e61 626c 6520 3d20 636f 6d70 2e5f 7365  nable = comp._se
+00002060: 745f 656e 6162 6c65 0d0a 2020 2020 2020  t_enable..      
+00002070: 2020 2020 2020 2020 2020 726f 6f74 5f69            root_i
+00002080: 7465 6d2e 6765 745f 656e 6162 6c65 203d  tem.get_enable =
+00002090: 2063 6f6d 702e 5f67 6574 5f65 6e61 626c   comp._get_enabl
+000020a0: 650d 0a0d 0a20 2020 2020 2020 2020 2020  e....           
+000020b0: 2065 6c69 6620 6973 7375 6263 6c61 7373   elif issubclass
+000020c0: 2874 7970 6528 636f 6d70 292c 2049 6e64  (type(comp), Ind
+000020d0: 6578 436f 6d6d 616e 6429 3a0d 0a20 2020  exCommand):..   
+000020e0: 2020 2020 2020 2020 2020 2020 2072 6f6f               roo
+000020f0: 745f 6974 656d 2e63 6f6d 7020 3d20 636f  t_item.comp = co
+00002100: 6d70 0d0a 2020 2020 2020 2020 2020 2020  mp..            
+00002110: 2020 2020 726f 6f74 5f69 7465 6d2e 636f      root_item.co
+00002120: 6d70 5f74 7970 6520 3d20 7479 7065 2863  mp_type = type(c
+00002130: 6f6d 7029 0d0a 2020 2020 2020 2020 2020  omp)..          
+00002140: 2020 2020 2020 726f 6f74 5f69 7465 6d2e        root_item.
+00002150: 6578 636c 7564 6564 203d 2063 6f6d 7020  excluded = comp 
+00002160: 696e 2072 6f6f 745f 6974 656d 2e70 6172  in root_item.par
+00002170: 656e 7428 292e 636f 6d70 2e65 7863 6c75  ent().comp.exclu
+00002180: 6465 5f63 6170 7475 7265 0d0a 2020 2020  de_capture..    
+00002190: 2020 2020 2020 2020 2020 2020 726f 6f74              root
+000021a0: 5f69 7465 6d2e 7261 775f 7265 6d6f 7465  _item.raw_remote
+000021b0: 5f63 6f6d 6d61 6e64 203d 2063 6f6d 702e  _command = comp.
+000021c0: 7265 6d6f 7465 5f63 6f6d 6d61 6e64 0d0a  remote_command..
+000021d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000021e0: 726f 6f74 5f69 7465 6d2e 7365 745f 656e  root_item.set_en
+000021f0: 6162 6c65 203d 2063 6f6d 702e 5f73 6574  able = comp._set
+00002200: 5f65 6e61 626c 650d 0a20 2020 2020 2020  _enable..       
+00002210: 2020 2020 2020 2020 2072 6f6f 745f 6974           root_it
+00002220: 656d 2e67 6574 5f65 6e61 626c 6520 3d20  em.get_enable = 
+00002230: 636f 6d70 2e5f 6765 745f 656e 6162 6c65  comp._get_enable
+00002240: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00002250: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+00002260: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00002270: 2063 6f6d 702e 696e 6465 785f 6469 6374   comp.index_dict
+00002280: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
+00002290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022a0: 2020 2069 6e64 6578 203d 2063 6f6d 702e     index = comp.
+000022b0: 696e 6465 785f 6d69 6e0d 0a20 2020 2020  index_min..     
+000022c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022d0: 2020 2077 6869 6c65 2069 6e64 6578 203c     while index <
+000022e0: 3d20 636f 6d70 2e69 6e64 6578 5f6d 6178  = comp.index_max
+000022f0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00002300: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00002310: 6869 6c64 203d 2063 6c73 2e6c 6f61 6428  hild = cls.load(
+00002320: 696e 6465 782c 2072 6f6f 745f 6974 656d  index, root_item
+00002330: 2c20 736f 7274 290d 0a20 2020 2020 2020  , sort)..       
+00002340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002350: 2020 2020 2063 6869 6c64 2e6e 616d 6520       child.name 
+00002360: 3d20 6627 7b69 6e64 6578 7d27 0d0a 2020  = f'{index}'..  
+00002370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002380: 2020 2020 2020 2020 2020 6368 696c 642e            child.
+00002390: 636f 6d70 203d 2069 6e64 6578 0d0a 2020  comp = index..  
+000023a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023b0: 2020 2020 2020 2020 2020 6368 696c 642e            child.
+000023c0: 636f 6d70 5f74 7970 6520 3d20 496e 6465  comp_type = Inde
+000023d0: 780d 0a20 2020 2020 2020 2020 2020 2020  x..             
+000023e0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000023f0: 6869 6c64 2e65 7863 6c75 6465 6420 3d20  hild.excluded = 
+00002400: 726f 6f74 5f69 7465 6d2e 6578 636c 7564  root_item.exclud
+00002410: 6564 0d0a 2020 2020 2020 2020 2020 2020  ed..            
+00002420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002430: 6368 696c 642e 7365 745f 656e 6162 6c65  child.set_enable
+00002440: 203d 2072 6f6f 745f 6974 656d 2e73 6574   = root_item.set
+00002450: 5f65 6e61 626c 650d 0a20 2020 2020 2020  _enable..       
 00002460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002470: 2020 2020 2020 2020 6368 696c 642e 636f          child.co
-00002480: 6d70 203d 2069 6e64 6578 0d0a 2020 2020  mp = index..    
-00002490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024a0: 2020 2020 2020 2020 6368 696c 642e 636f          child.co
-000024b0: 6d70 5f74 7970 6520 3d20 496e 6465 780d  mp_type = Index.
-000024c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000024d0: 2020 2020 2020 2020 2020 2020 2063 6869               chi
-000024e0: 6c64 2e65 7863 6c75 6465 6420 3d20 726f  ld.excluded = ro
-000024f0: 6f74 5f69 7465 6d2e 6578 636c 7564 6564  ot_item.excluded
-00002500: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002510: 2020 2020 2020 2020 2020 2020 2020 6368                ch
-00002520: 696c 642e 7365 745f 656e 6162 6c65 203d  ild.set_enable =
-00002530: 2072 6f6f 745f 6974 656d 2e73 6574 5f65   root_item.set_e
-00002540: 6e61 626c 650d 0a20 2020 2020 2020 2020  nable..         
+00002470: 2020 2020 2063 6869 6c64 2e67 6574 5f65       child.get_e
+00002480: 6e61 626c 6520 3d20 726f 6f74 5f69 7465  nable = root_ite
+00002490: 6d2e 6765 745f 656e 6162 6c65 0d0a 2020  m.get_enable..  
+000024a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024b0: 2020 2020 2020 2020 2020 726f 6f74 5f69            root_i
+000024c0: 7465 6d2e 6170 7065 6e64 4368 696c 6428  tem.appendChild(
+000024d0: 6368 696c 6429 0d0a 2020 2020 2020 2020  child)..        
+000024e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024f0: 2020 2020 696e 6465 7820 2b3d 2031 0d0a      index += 1..
+00002500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002510: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00002520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002530: 2020 2066 6f72 206b 6579 2069 6e20 636f     for key in co
+00002540: 6d70 2e69 6e64 6578 5f64 6963 743a 0d0a  mp.index_dict:..
 00002550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002560: 2020 2063 6869 6c64 2e67 6574 5f65 6e61     child.get_ena
-00002570: 626c 6520 3d20 726f 6f74 5f69 7465 6d2e  ble = root_item.
-00002580: 6765 745f 656e 6162 6c65 0d0a 2020 2020  get_enable..    
-00002590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025a0: 2020 2020 2020 2020 726f 6f74 5f69 7465          root_ite
-000025b0: 6d2e 6170 7065 6e64 4368 696c 6428 6368  m.appendChild(ch
-000025c0: 696c 6429 0d0a 2020 2020 2020 2020 2020  ild)..          
+00002560: 2020 2020 2020 2020 2020 2020 6368 696c              chil
+00002570: 6420 3d20 636c 732e 6c6f 6164 286b 6579  d = cls.load(key
+00002580: 2c20 726f 6f74 5f69 7465 6d2c 2073 6f72  , root_item, sor
+00002590: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
+000025a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025b0: 6368 696c 642e 6e61 6d65 203d 2066 277b  child.name = f'{
+000025c0: 6b65 797d 270d 0a20 2020 2020 2020 2020  key}'..         
 000025d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025e0: 2020 696e 6465 7820 2b3d 2031 0d0a 2020    index += 1..  
-000025f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002600: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00002610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002620: 2066 6f72 206b 6579 2069 6e20 636f 6d70   for key in comp
-00002630: 2e69 6e64 6578 5f64 6963 743a 0d0a 2020  .index_dict:..  
-00002640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002650: 2020 2020 2020 2020 2020 6368 696c 6420            child 
-00002660: 3d20 636c 732e 6c6f 6164 286b 6579 2c20  = cls.load(key, 
-00002670: 726f 6f74 5f69 7465 6d29 0d0a 2020 2020  root_item)..    
-00002680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002690: 2020 2020 2020 2020 6368 696c 642e 6e61          child.na
-000026a0: 6d65 203d 2066 277b 6b65 797d 270d 0a20  me = f'{key}'.. 
+000025e0: 2020 2063 6869 6c64 2e63 6f6d 7020 3d20     child.comp = 
+000025f0: 6b65 790d 0a20 2020 2020 2020 2020 2020  key..           
+00002600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002610: 2063 6869 6c64 2e63 6f6d 705f 7479 7065   child.comp_type
+00002620: 203d 2049 6e64 6578 0d0a 2020 2020 2020   = Index..      
+00002630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002640: 2020 2020 2020 6368 696c 642e 6578 6c75        child.exlu
+00002650: 6465 6420 3d20 726f 6f74 5f69 7465 6d2e  ded = root_item.
+00002660: 6578 636c 7564 6564 0d0a 2020 2020 2020  excluded..      
+00002670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002680: 2020 2020 2020 6368 696c 642e 7365 745f        child.set_
+00002690: 656e 6162 6c65 203d 2063 6f6d 702e 5f73  enable = comp._s
+000026a0: 6574 5f65 6e61 626c 650d 0a20 2020 2020  et_enable..     
 000026b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026c0: 2020 2020 2020 2020 2020 2063 6869 6c64             child
-000026d0: 2e63 6f6d 7020 3d20 6b65 790d 0a20 2020  .comp = key..   
-000026e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026f0: 2020 2020 2020 2020 2063 6869 6c64 2e63           child.c
-00002700: 6f6d 705f 7479 7065 203d 2049 6e64 6578  omp_type = Index
-00002710: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002720: 2020 2020 2020 2020 2020 2020 2020 6368                ch
-00002730: 696c 642e 6578 6c75 6465 6420 3d20 726f  ild.exluded = ro
-00002740: 6f74 5f69 7465 6d2e 6578 636c 7564 6564  ot_item.excluded
-00002750: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002760: 2020 2020 2020 2020 2020 2020 2020 6368                ch
-00002770: 696c 642e 7365 745f 656e 6162 6c65 203d  ild.set_enable =
-00002780: 2063 6f6d 702e 5f73 6574 5f65 6e61 626c   comp._set_enabl
-00002790: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
-000027a0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000027b0: 6869 6c64 2e67 6574 5f65 6e61 626c 6520  hild.get_enable 
-000027c0: 3d20 636f 6d70 2e5f 6765 745f 656e 6162  = comp._get_enab
-000027d0: 6c65 0d0a 2020 2020 2020 2020 2020 2020  le..            
-000027e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027f0: 726f 6f74 5f69 7465 6d2e 6170 7065 6e64  root_item.append
-00002800: 4368 696c 6428 6368 696c 6429 0d0a 2020  Child(child)..  
-00002810: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-00002820: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
-00002830: 7320 653a 0d0a 2020 2020 2020 2020 2020  s e:..          
-00002840: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00002850: 6627 2020 7b74 7970 6528 6529 7d20 7b65  f'  {type(e)} {e
-00002860: 7d20 636f 6d6d 616e 643a 7b63 6f6d 702e  } command:{comp.
-00002870: 7265 6d6f 7465 5f63 6f6d 6d61 6e64 7d20  remote_command} 
-00002880: 696e 6465 783a 207b 696e 6465 787d 2729  index: {index}')
-00002890: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000028a0: 2072 6f6f 745f 6974 656d 0d0a             root_item..
+000026c0: 2020 2020 2020 2063 6869 6c64 2e67 6574         child.get
+000026d0: 5f65 6e61 626c 6520 3d20 636f 6d70 2e5f  _enable = comp._
+000026e0: 6765 745f 656e 6162 6c65 0d0a 2020 2020  get_enable..    
+000026f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002700: 2020 2020 2020 2020 726f 6f74 5f69 7465          root_ite
+00002710: 6d2e 6170 7065 6e64 4368 696c 6428 6368  m.appendChild(ch
+00002720: 696c 6429 0d0a 2020 2020 2020 2020 2020  ild)..          
+00002730: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
+00002740: 6570 7469 6f6e 2061 7320 653a 0d0a 2020  eption as e:..  
+00002750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002760: 2020 7072 696e 7428 6627 2020 7b74 7970    print(f'  {typ
+00002770: 6528 6529 7d20 7b65 7d20 636f 6d6d 616e  e(e)} {e} comman
+00002780: 643a 7b63 6f6d 702e 7265 6d6f 7465 5f63  d:{comp.remote_c
+00002790: 6f6d 6d61 6e64 7d20 696e 6465 783a 207b  ommand} index: {
+000027a0: 696e 6465 787d 2729 0d0a 2020 2020 2020  index}')..      
+000027b0: 2020 7265 7475 726e 2072 6f6f 745f 6974    return root_it
+000027c0: 656d 0d0a                                em..
```

### Comparing `srsgui-0.2.13/srsgui/ui/commandtree/commandmodel.py` & `srsgui-0.2.9/srsgui/ui/commandtree/commandmodel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 
 import time
 import json
 import sys
-
 from typing import Any, Iterable, List, Dict, Union
 
 from srsgui.ui.qt.QtWidgets import QTreeView, QApplication, QHeaderView
 from srsgui.ui.qt.QtGui import QBrush, QColor
 from srsgui.ui.qt.QtCore import QAbstractItemModel, QModelIndex, QObject, Qt, QFileInfo
 
 from srsgui import Component
@@ -17,40 +16,45 @@
 
 class CommandModel(QAbstractItemModel):
     """ An editable model of Command and Component """
 
     def __init__(self, parent: QObject = None):
         super().__init__(parent)
 
+        self.show_methods = True
+        self.show_excluded = True
+        self.show_set_only = True
+        self.show_query_only = True
         self.show_raw_remote_command = True
 
         self._rootItem = CommandItem()
         self._headers = ("  command  ", "  value  ")
 
     def clear(self):
         """ Clear data from the model """
         self.load(Component())
 
-    def load(self, document: Component):
+    def load(self, document: Component, sort=False):
         """Load model from a nested dictionary returned by json.loads()
 
         Arguments:
             document (dict): JSON-compatible dictionary
         """
 
         assert isinstance(
             document, Component
-        ), "`document` must be a Component, " f"not {type(document)}"
+        ), "`document` must be of dict, list or tuple, " f"not {type(document)}"
 
         self.beginResetModel()
 
-        self._rootItem = CommandItem.load(document)
+        self._rootItem = CommandItem.load(document, sort=sort)
         self._rootItem.value_type = type(document)
 
         self.endResetModel()
+
         return True
 
     def data(self, index: QModelIndex, role: Qt.ItemDataRole) -> Any:
         """Override from QAbstractItemModel
 
         Return data from an item according index and role
         """
@@ -61,45 +65,55 @@
         if role == Qt.DisplayRole:
             if index.column() == 0:
                 item = index.internalPointer()
                 name = item.name
 
                 if self.show_raw_remote_command:
                     name += f' <{item.raw_remote_command}>' if item.raw_remote_command else ''
-
-                name += ' [M]' if item.is_method else ''
-                name += ' [EX]' if item.excluded else ''
-                name += ' [SO]' if item.set_enable and not item.get_enable else ''
-                name += ' [QO]' if item.get_enable and not item.set_enable else ''
+                if self.show_methods:
+                    name += ' [M]' if item.is_method else ''
+                if self.show_excluded:
+                    name += ' [EX]' if item.excluded else ''
+                if self.show_set_only:
+                    name += ' [SO]' if item.set_enable and not item.get_enable else ''
+                if self.show_query_only:
+                    name += ' [QO]' if item.get_enable and not item.set_enable else ''
                 return name
 
             if index.column() == 1:
                 item = index.internalPointer()
                 v = item.value
-                if v is not None:
-                    return item.get_formatted_value(v)
+                if v is None:
+                    return
+                unit = item.get_unit()
+                fmt = item.get_format()
+                try:
+                    if unit:
+                        val = f'{v:{fmt}}  {item.get_unit()}'
+                    else:
+                        val = f'{v:{fmt}}'
+                except ValueError:
+                    print(f'ValueError: {item.raw_remote_command} {v} {fmt} {unit}')
+                    val = f'{v}'
+                return val
 
         elif role == Qt.EditRole:
             if index.column() == 1:
                 item = index.internalPointer()
-                return item.value
+                val = item.value
+                # print('data', item.name, item.comp, val)
+                return val
 
         elif role == Qt.BackgroundRole:
             item = index.internalPointer()
             if item.comp_type != Index and issubclass(item.comp_type, Component):
                 return QBrush(QColor(243, 230, 225))
             if item.row() % 2 == 0:
                 return QBrush(QColor(240, 240, 253))
 
-        elif role == Qt.ToolTipRole:
-            item = index.internalPointer()
-            if item.is_method or issubclass(item.comp_type, Component):
-                if hasattr(item.comp, '__doc__') and index.column() == 0:
-                    return item.comp.__doc__
-
     def setData(self, index: QModelIndex, value: Any, role: Qt.ItemDataRole):
         """Override from QAbstractItemModel
 
         Set CommandItem according to index and role
 
         Args:
             index (QModelIndex)
```

### Comparing `srsgui-0.2.13/srsgui/ui/commandtree/commandspinbox.py` & `srsgui-0.2.9/srsgui/ui/commandtree/commandspinbox.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     def stepBy(self, steps):
         prefix_len = len(self.prefix())
         min_pos = prefix_len + 1 if self.value() < 0 else prefix_len
 
         text = self.lineEdit().text()
         cur_pos = self.lineEdit().cursorPosition()
-        sep_pos = len(text) - len(self.suffix())
+        sep_pos = len(text)
 
         if cur_pos < min_pos:
             return
 
         exponent = sep_pos - cur_pos
 
         single_step = 10 ** exponent
@@ -32,15 +32,15 @@
         super().stepBy(steps)
 
         self.lineEdit().deselect()
 
         min_pos = prefix_len + 1 if self.value() < 0 else prefix_len
 
         text = self.lineEdit().text()
-        new_sep_pos = len(text) - len(self.suffix())
+        new_sep_pos = len(text)
 
         new_cur_pos = cur_pos + new_sep_pos - sep_pos
         if new_cur_pos < min_pos:
             new_cur_pos = min_pos
         self.lineEdit().setCursorPosition(new_cur_pos)
 
 
@@ -49,60 +49,56 @@
     Adjust step size depending on the cursor postion
     """
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.minimum_step = 0.1
         self.significant_figures = 4
         self.precision = 1
-        self.decis = 1
 
     def set_minimum_step(self, value):
         self.minimum_step = value
         step = self.minimum_step if self.minimum_step > 1e-12 else 1e-12
-        self.decis = math.ceil(-math.log10(step))
+        self.decimals = math.ceil(math.log10(1.0 / step))
 
     def set_significant_figures(self, value):
         self.significant_figures = value
 
     def valueFromText(self, text):
         try:
             if self.suffix():
                 unit_len = len(self.suffix())
                 value = float(text[:-unit_len])
-
             else:
                 value = float(text)
             if value < self.minimum():
                 value = self.minimum()
             elif value > self.maximum():
                 value = self.maximum()
-
-
         except ValueError:
             print('valueFromText ValueError', text, self.suffix())
             value = self.minimum()
         return value
 
     def textFromValue(self, value):
-        prec = self.decis
+        prec = self.decimals
         try:
             if value == 0:
                 return '0.0'
 
             digits = math.ceil(math.log10(abs(value)))
-            """
+            # digits = 0 if digits < 0 else digits
+
             if digits == self.significant_figures:
                 step = 1
             else:
                 step = 10 ** (digits - self.significant_figures)
             value = round(value / step) * step
-            """
             prec = self.significant_figures - digits
-            if prec > self.decis:
-                prec = self.decis
+            if prec > self.decimals:
+                prec = self.decimals
         except Exception as e:
             print(e)
         self.precision = prec
         format_string = '{:.' + str(prec) + 'f}'
         text = format_string.format(value)
         return text
```

### Comparing `srsgui-0.2.13/srsgui/ui/commandtree/commandtreeview.py` & `srsgui-0.2.9/srsgui/ui/commandtree/commandtreeview.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import inspect
 import logging
 
 from srsgui.ui.qt.QtCore import Qt, QModelIndex
-from srsgui.ui.qt.QtWidgets import QTreeView, QApplication, QHeaderView
+from srsgui.ui.qt.QtWidgets import QTreeView, QApplication, QHeaderView, QPushButton
 
 from .commandmodel import CommandModel
 from .commanddelegate import CommandDelegate
 from .commandspinbox import RunButton
 
 
 class CommandTreeView(QTreeView):
@@ -47,20 +47,15 @@
         for i in range(self.model().rowCount(parent)):
             index = self.model().index(i, 0, parent)
             self.connect_methods_to_buttons(index)
             try:
                 item = index.internalPointer()
                 if item.is_method:
                     widget_index = self.model().index(i, 1, parent)
-                    spec = inspect.getfullargspec(item.comp)
-                    if spec.defaults is None:
-                        flag = len(spec.args) == 1
-                    else:
-                        flag = len(spec.args) - len(spec.defaults) == 1
-                    if flag:
+                    if len(inspect.getfullargspec(item.comp).args) == 1:
                         parent_comp = item.parent().comp
                         meth = getattr(parent_comp, item.name)
                         if meth and meth.__func__ in parent_comp.allow_run_button:
                             button = RunButton()
                             button.pressed.connect(meth)
                             self.setIndexWidget(widget_index, button)
             except Exception as e:
```

### Comparing `srsgui-0.2.13/srsgui/ui/commandtree/commandtreewidget.py` & `srsgui-0.2.9/srsgui/ui/commandtree/commandtreewidget.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         self.tree_view.show_raw_command = state
         self.model.show_raw_remote_command = self.tree_view.show_raw_command
 
     def on_capture_clicked(self):
         if self.inst is not None and self.inst.is_connected():
             try:
                 self.model.show_raw_remote_command = self.show_raw_command
-                self.model.load(self.inst)
+                self.model.load(self.inst, False)
                 self.tree_view.expandToDepth(1)
                 self.tree_view.resizeColumnToContents(0)
                 # self.tree_view.collapseAll()
                 self.tree_view.update_item_display()
                 self.tree_view.connect_methods_to_buttons()
 
             except Exception as e:
```

### Comparing `srsgui-0.2.13/srsgui/ui/commandtree/jsonmodel.py` & `srsgui-0.2.9/srsgui/ui/commandtree/jsonmodel.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/ui/commandtree/ui_commandcapturewidget.py` & `srsgui-0.2.9/srsgui/ui/commandtree/ui_commandcapturewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/ui/commandtree/ui_commandtreewidget.py` & `srsgui-0.2.9/srsgui/ui/commandtree/ui_commandtreewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/ui/connectdlg.py` & `srsgui-0.2.9/srsgui/ui/connectdlg.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/ui/deviceinfohandler.py` & `srsgui-0.2.9/srsgui/ui/deviceinfohandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/ui/dockhandler.py` & `srsgui-0.2.9/srsgui/ui/dockhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/ui/inputpanel.py` & `srsgui-0.2.9/srsgui/ui/inputpanel.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/ui/qt/QtCore.py` & `srsgui-0.2.9/srsgui/ui/qt/QtCore.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/ui/qt/QtGui.py` & `srsgui-0.2.9/srsgui/ui/qt/QtGui.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/ui/qt/QtWidgets.py` & `srsgui-0.2.9/srsgui/ui/qt/QtWidgets.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/ui/qt/__init__.py` & `srsgui-0.2.9/srsgui/ui/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/ui/qtloghandler.py` & `srsgui-0.2.9/srsgui/ui/qtloghandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/ui/resource_rc.py` & `srsgui-0.2.9/srsgui/ui/resource_rc.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/ui/signalhandler.py` & `srsgui-0.2.9/srsgui/ui/signalhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/ui/srslogo.jpg` & `srsgui-0.2.9/srsgui/ui/srslogo.jpg`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/ui/stdout.py` & `srsgui-0.2.9/srsgui/ui/stdout.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/ui/taskmain.py` & `srsgui-0.2.9/srsgui/ui/taskmain.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/ui/taskmain.ui` & `srsgui-0.2.9/srsgui/ui/taskmain.ui`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui/ui/ui_taskmain.py` & `srsgui-0.2.9/srsgui/ui/ui_taskmain.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.13/srsgui.egg-info/PKG-INFO` & `srsgui-0.2.9/srsgui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.2.13
+Version: 0.2.9
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Keywords: instrument control,data acquisition,data visualization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `srsgui-0.2.13/srsgui.egg-info/SOURCES.txt` & `srsgui-0.2.9/srsgui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

