# Comparing `tmp/labscript-utils-3.2.2.tar.gz` & `tmp/labscript-utils-3.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labscript-utils-3.2.2.tar", last modified: Tue Mar 28 00:47:24 2023, max compression
+gzip compressed data, was "labscript-utils-3.3.0rc1.tar", last modified: Thu Apr 13 17:18:07 2023, max compression
```

## Comparing `labscript-utils-3.2.2.tar` & `labscript-utils-3.3.0rc1.tar`

### file list

```diff
@@ -1,137 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:47:24.189525 labscript-utils-3.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:47:24.177525 labscript-utils-3.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:47:24.177525 labscript-utils-3.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/BSD-2-CLAUSE-LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/BSD-3-CLAUSE-LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/NEWS.md
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-03-28 00:47:24.193526 labscript-utils-3.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:47:24.177525 labscript-utils-3.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:47:24.181525 labscript-utils-3.2.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:47:24.181525 labscript-utils-3.2.2/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/docs/source/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:47:24.181525 labscript-utils-3.2.2/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/docs/source/_templates/autosummary-class.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/docs/source/_templates/autosummary-module.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/docs/source/_templates/components.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:47:24.181525 labscript-utils-3.2.2/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/docs/source/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:47:24.181525 labscript-utils-3.2.2/docs/source/img/
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/docs/source/img/blacs_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)    46681 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/docs/source/img/labscript-suite-rectangular-transparent_138nx70n.svg
--rw-r--r--   0 runner    (1001) docker     (123)    98716 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/docs/source/img/labscript.ico
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/docs/source/img/labscript_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/docs/source/img/labscript_64x64.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/docs/source/img/lyse_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/docs/source/img/runmanager_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/docs/source/img/runviewer_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/docs/source/labconfig.rst
--rw-r--r--   0 runner    (1001) docker     (123)    64143 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/docs/source/pyqt5-modified-objects.inv
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript-suite.pth
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:47:24.181525 labscript-utils-3.2.2/labscript_profile/
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_profile/create.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:47:24.177525 labscript-utils-3.2.2/labscript_profile/default_profile/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:47:24.181525 labscript-utils-3.2.2/labscript_profile/default_profile/app_saved_configs/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_profile/default_profile/app_saved_configs/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:47:24.181525 labscript-utils-3.2.2/labscript_profile/default_profile/labconfig/
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_profile/default_profile/labconfig/example.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:47:24.177525 labscript-utils-3.2.2/labscript_profile/default_profile/userlib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:47:24.181525 labscript-utils-3.2.2/labscript_profile/default_profile/userlib/analysislib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_profile/default_profile/userlib/analysislib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:47:24.181525 labscript-utils-3.2.2/labscript_profile/default_profile/userlib/analysislib/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_profile/default_profile/userlib/analysislib/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:47:24.181525 labscript-utils-3.2.2/labscript_profile/default_profile/userlib/analysislib/example_apparatus/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_profile/default_profile/userlib/analysislib/example_apparatus/example_IMAQdx_remote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:47:24.181525 labscript-utils-3.2.2/labscript_profile/default_profile/userlib/labscriptlib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_profile/default_profile/userlib/labscriptlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:47:24.181525 labscript-utils-3.2.2/labscript_profile/default_profile/userlib/labscriptlib/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_profile/default_profile/userlib/labscriptlib/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:47:24.181525 labscript-utils-3.2.2/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/connection_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/connection_table_IMAQdx_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/example_IMAQdx_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/example_experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:47:24.181525 labscript-utils-3.2.2/labscript_profile/default_profile/userlib/pythonlib/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_profile/default_profile/userlib/pythonlib/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:47:24.185526 labscript-utils-3.2.2/labscript_profile/default_profile/userlib/user_devices/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_profile/default_profile/userlib/user_devices/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:47:24.185526 labscript-utils-3.2.2/labscript_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9517 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/camera_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    16277 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/connections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:47:24.189525 labscript-utils-3.2.2/labscript_utils/device_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/device_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13809 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/device_registry/_device_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/dict_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/double_import_denier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:47:24.189525 labscript-utils-3.2.2/labscript_utils/excepthook/
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/excepthook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/excepthook/error.gif
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/excepthook/tk_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/filewatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/h5_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/impprof.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/labconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/ls_zprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/memprof.py
--rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/modulewatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:47:24.189525 labscript-utils-3.2.2/labscript_utils/qtwidgets/
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/qtwidgets/InputPlotWindow.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/qtwidgets/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5511 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/qtwidgets/analoginput.py
--rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/qtwidgets/analogoutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/qtwidgets/ddsoutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/qtwidgets/digitaloutput.py
--rw-r--r--   0 runner    (1001) docker     (123)    36372 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/qtwidgets/dragdroptab.py
--rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/qtwidgets/elide_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/qtwidgets/enumoutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/qtwidgets/fingertab.py
--rw-r--r--   0 runner    (1001) docker     (123)    12370 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/qtwidgets/headerview_with_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/qtwidgets/imageoutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/qtwidgets/outputbox.py
--rw-r--r--   0 runner    (1001) docker     (123)    21502 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/qtwidgets/toolpalette.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/setup_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/shared_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/splash.py
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/testing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/tracelog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:47:24.189525 labscript-utils-3.2.2/labscript_utils/unitconversions/
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/unitconversions/NovaTechDDS9m.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/unitconversions/UnitConversionBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/unitconversions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/unitconversions/aom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/unitconversions/detuning.py
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/unitconversions/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/unitconversions/generic_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/unitconversions/linear_coil_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/unitconversions/optotunelens.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/unitconversions/quad_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/unitconversions/quad_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/unitconversions/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10854 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/zlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/labscript_utils/zlog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:47:24.185526 labscript-utils-3.2.2/labscript_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-03-28 00:47:24.000000 labscript-utils-3.2.2/labscript_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-03-28 00:47:24.000000 labscript-utils-3.2.2/labscript_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 00:47:24.000000 labscript-utils-3.2.2/labscript_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-28 00:47:24.000000 labscript-utils-3.2.2/labscript_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 00:47:23.000000 labscript-utils-3.2.2/labscript_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-28 00:47:24.000000 labscript-utils-3.2.2/labscript_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-28 00:47:24.000000 labscript-utils-3.2.2/labscript_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-03-28 00:47:24.193526 labscript-utils-3.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-03-28 00:47:13.000000 labscript-utils-3.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.889528 labscript-utils-3.3.0rc1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.865528 labscript-utils-3.3.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.869528 labscript-utils-3.3.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/BSD-2-CLAUSE-LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/BSD-3-CLAUSE-LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/NEWS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-13 17:18:07.889528 labscript-utils-3.3.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.873528 labscript-utils-3.3.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.873528 labscript-utils-3.3.0rc1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.873528 labscript-utils-3.3.0rc1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.873528 labscript-utils-3.3.0rc1/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/_templates/autosummary-class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/_templates/autosummary-module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/_templates/components.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.873528 labscript-utils-3.3.0rc1/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.873528 labscript-utils-3.3.0rc1/docs/source/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/img/blacs_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    46681 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/img/labscript-suite-rectangular-transparent_138nx70n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    98716 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/img/labscript.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/img/labscript_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/img/labscript_64x64.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/img/lyse_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/img/runmanager_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/img/runviewer_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/labconfig.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    64143 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/pyqt5-modified-objects.inv
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript-suite.pth
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.877528 labscript-utils-3.3.0rc1/labscript_profile/
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_profile/create.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.869528 labscript-utils-3.3.0rc1/labscript_profile/default_profile/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.877528 labscript-utils-3.3.0rc1/labscript_profile/default_profile/app_saved_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_profile/default_profile/app_saved_configs/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.877528 labscript-utils-3.3.0rc1/labscript_profile/default_profile/labconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_profile/default_profile/labconfig/example.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.869528 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.877528 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/analysislib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/analysislib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.877528 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/analysislib/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/analysislib/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.877528 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/analysislib/example_apparatus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/analysislib/example_apparatus/example_IMAQdx_remote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.877528 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/labscriptlib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/labscriptlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.877528 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/labscriptlib/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/labscriptlib/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.877528 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/connection_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/connection_table_IMAQdx_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/example_IMAQdx_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/example_experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.877528 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/pythonlib/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/pythonlib/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.877528 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/user_devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/user_devices/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.881528 labscript-utils-3.3.0rc1/labscript_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9517 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/camera_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16277 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/connections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.885528 labscript-utils-3.3.0rc1/labscript_utils/device_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/device_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13809 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/device_registry/_device_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/dict_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/double_import_denier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.885528 labscript-utils-3.3.0rc1/labscript_utils/excepthook/
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/excepthook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/excepthook/error.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/excepthook/tk_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/filewatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/h5_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/impprof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/labconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/ls_zprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/memprof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/modulewatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.885528 labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/InputPlotWindow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5511 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/analoginput.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/analogoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/ddsoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/digitaloutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36434 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/dragdroptab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/elide_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/enumoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/fingertab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12370 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/headerview_with_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/imageoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/outputbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21502 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/toolpalette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/setup_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/shared_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/shot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/splash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/testing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/tracelog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.889528 labscript-utils-3.3.0rc1/labscript_utils/unitconversions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/unitconversions/NovaTechDDS9m.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/unitconversions/UnitConversionBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/unitconversions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/unitconversions/aom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/unitconversions/detuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/unitconversions/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/unitconversions/generic_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/unitconversions/linear_coil_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/unitconversions/optotunelens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/unitconversions/quad_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/unitconversions/quad_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/unitconversions/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10854 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/zlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/zlog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.885528 labscript-utils-3.3.0rc1/labscript_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-13 17:18:07.000000 labscript-utils-3.3.0rc1/labscript_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-13 17:18:07.000000 labscript-utils-3.3.0rc1/labscript_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:18:07.000000 labscript-utils-3.3.0rc1/labscript_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-13 17:18:07.000000 labscript-utils-3.3.0rc1/labscript_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:18:07.000000 labscript-utils-3.3.0rc1/labscript_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-13 17:18:07.000000 labscript-utils-3.3.0rc1/labscript_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-13 17:18:07.000000 labscript-utils-3.3.0rc1/labscript_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-13 17:18:07.889528 labscript-utils-3.3.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/setup.py
```

### Comparing `labscript-utils-3.2.2/.github/workflows/release.yml` & `labscript-utils-3.3.0rc1/.github/workflows/release.yml`

 * *Files 13% similar despite different names*

```diff
@@ -33,33 +33,37 @@
 jobs:
   build:
     name: Build
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         include:
-          # - { os: ubuntu-latest,   python: '3.10',  arch: x64 }
-          # - { os: ubuntu-latest,   python: '3.9',  arch: x64 }
-          - { os: ubuntu-latest,   python: '3.8',  arch: x64 }
-          # - { os: ubuntu-latest,   python: '3.7',  arch: x64 }
-
-          # - { os: macos-latest,    python: '3.10',  arch: x64 }
-          # - { os: macos-latest,    python: '3.9',  arch: x64 }
-          # - { os: macos-latest,    python: '3.8',  arch: x64 }
-          # - { os: macos-latest,    python: '3.7',  arch: x64 }
-
-          # - { os: windows-latest,  python: '3.10',  arch: x64 }
-          # - { os: windows-latest,  python: '3.9',  arch: x64 }
-          # - { os: windows-latest,  python: '3.8',  arch: x64 }
-          # - { os: windows-latest,  python: '3.7',  arch: x64 }
-
-          # - { os: windows-latest,  python: '3.10',  arch: x86 }
-          # - { os: windows-latest,  python: '3.9',  arch: x86 }
-          # - { os: windows-latest,  python: '3.8',  arch: x86 }
-          # - { os: windows-latest,  python: '3.7',  arch: x86 }
+          - { os: ubuntu-latest,   python: '3.11',  arch: x64, conda: true}
+          # - { os: ubuntu-latest,   python: '3.10',  arch: x64, conda: true }
+          # - { os: ubuntu-latest,   python: '3.9',  arch: x64, conda: true }
+          # - { os: ubuntu-latest,   python: '3.8',  arch: x64, conda: true }
+          # - { os: ubuntu-latest,   python: '3.7',  arch: x64, conda: true }
+
+          # - { os: macos-11,    python: '3.11',  arch: x64, conda: true }
+          # - { os: macos-11,    python: '3.10',  arch: x64, conda: true }
+          # - { os: macos-11,    python: '3.9',  arch: x64, conda: true }
+          # - { os: macos-11,    python: '3.8',  arch: x64, conda: true }
+          # - { os: macos-11,    python: '3.7',  arch: x64, conda: true }
+
+          # - { os: windows-latest,  python: '3.11',  arch: x64, conda: true }
+          # - { os: windows-latest,  python: '3.10',  arch: x64, conda: true }
+          # - { os: windows-latest,  python: '3.9',  arch: x64, conda: true }
+          # - { os: windows-latest,  python: '3.8',  arch: x64, conda: true }
+          # - { os: windows-latest,  python: '3.7',  arch: x64, conda: true }
+
+          # - { os: windows-latest,  python: '3.11',  arch: x86, conda: false } # conda not yet available
+          # - { os: windows-latest,  python: '3.10',  arch: x86, conda: true }
+          # - { os: windows-latest,  python: '3.9',  arch: x86, conda: true }
+          # - { os: windows-latest,  python: '3.8',  arch: x86, conda: true }
+          # - { os: windows-latest,  python: '3.7',  arch: x86, conda: true }
 
     if: github.repository == 'labscript-suite/labscript-utils' && (github.event_name != 'create' || github.event.ref_type != 'branch')
     steps:
       - name: Checkout
         uses: actions/checkout@v3
         with:
           fetch-depth: 0
@@ -91,55 +95,55 @@
         if: strategy.job-index == 0 || (env.PURE == 'false' && runner.os != 'Linux')
         uses: actions/upload-artifact@v3
         with:
           name: dist
           path: ./dist
 
       - name: Set Variables for Conda Build
+        if: matrix.conda
         shell: bash
         run: |
           if [ $NOARCH == true ]; then
               CONDA_BUILD_ARGS="--noarch"
           else
               CONDA_BUILD_ARGS=""
           fi
           echo "CONDA_BUILD_ARGS=$CONDA_BUILD_ARGS" >> $GITHUB_ENV
 
       - name: Install Miniconda
-        # We need https://github.com/conda-incubator/setup-miniconda/pull/189 in order
-        # to be able to install 32-bit miniconda on Windows. Once setup-miniconda 2.1.2
-        # is released with this fix, can change to @v2.
-        uses: conda-incubator/setup-miniconda@1a875d105ac03256664b54c882c8c374ce617ef6
+        if: matrix.conda
+        uses: conda-incubator/setup-miniconda@v2
         with:
           auto-update-conda: true
           python-version: ${{ matrix.python }}
           architecture: ${{ matrix.arch }}
           miniconda-version: "latest"
 
-      - name: Workaround conda-build incompatibility with xcode >12
+      - name: Workaround conda-build incompatibility with xcode 12+
         if: runner.os == 'macOS'
         uses: maxim-lobanov/setup-xcode@v1
         with:
           xcode-version: 11.7
 
       - name: Conda package (Unix)
-        if: runner.os != 'Windows'
+        if: (matrix.conda && runner.os != 'Windows')
         shell: bash -l {0}
         run: |
           conda install -c labscript-suite setuptools-conda
           setuptools-conda build $CONDA_BUILD_ARGS .
 
       - name: Conda Package (Windows)
-        if: runner.os == 'Windows'
+        if: (matrix.conda && runner.os == 'Windows')
         shell: cmd /C CALL {0}
         run: |
           conda install -c labscript-suite setuptools-conda && ^
           setuptools-conda build %CONDA_BUILD_ARGS% --croot ${{ runner.temp }}\cb .
 
       - name: Upload Artifact
+        if: matrix.conda
         uses: actions/upload-artifact@v3
         with:
           name: conda_packages
           path: ./conda_packages
 
 
   manylinux:
@@ -157,15 +161,15 @@
         if: github.event.ref_type != 'tag' && env.PURE == 'false'
         run: git tag -d $(git tag --points-at HEAD)
 
       - name: Build Manylinux Wheels
         if: env.PURE == 'false'
         uses: RalfG/python-wheels-manylinux-build@v0.4.2
         with:
-          python-versions: 'cp37-cp37m cp38-cp38 cp39-cp39 cp310-cp310'
+          python-versions: 'cp37-cp37m cp38-cp38 cp39-cp39 cp310-cp310 cp311-cp311'
           pre-build-command: 'git config --global --add safe.directory "*"'
 
       - name: Upload Artifact
         if: env.PURE == 'false'
         uses: actions/upload-artifact@v3
         with:
           name: dist
@@ -185,53 +189,42 @@
 
       - name: Download Artifact
         uses: actions/download-artifact@v3
         with:
           name: conda_packages
           path: ./conda_packages
 
-      - name: Publish on TestPyPI
-        uses: pypa/gh-action-pypi-publish@release/v1
-        with:
-          user: __token__
-          password: ${{ secrets.testpypi }}
-          repository_url: https://test.pypi.org/legacy/
-
       - name: Get Version Number
         if: github.event.ref_type == 'tag'
         run: |
           VERSION="${GITHUB_REF/refs\/tags\/v/}"
           echo "VERSION=$VERSION" >> $GITHUB_ENV
 
-      - name: Create GitHub Release
+      - name: Create GitHub Release and Upload Release Asset
         if: github.event.ref_type == 'tag'
-        id: create_release
-        uses: actions/create-release@latest
+        uses: softprops/action-gh-release@v1
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         with:
           tag_name: ${{ github.event.ref }}
-          release_name: ${{ env.PACKAGE_NAME }} ${{ env.VERSION }}
+          name: ${{ env.PACKAGE_NAME }} ${{ env.VERSION }}
           draft: true
           prerelease: ${{ contains(github.event.ref, 'rc') }}
+          files: ./dist/${{ env.PACKAGE_NAME }}-${{ env.VERSION }}.tar.gz
 
-      - name: Upload Release Asset
-        if: github.event.ref_type == 'tag'
-        uses: actions/upload-release-asset@v1
-        env:
-          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+      - name: Publish on TestPyPI
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
-          upload_url: ${{ steps.create_release.outputs.upload_url }}
-          asset_path: ./dist/${{ env.PACKAGE_NAME }}-${{ env.VERSION }}.tar.gz
-          asset_name: ${{ env.PACKAGE_NAME }}-${{ env.VERSION }}.tar.gz
-          asset_content_type: application/gzip
+          user: __token__
+          password: ${{ secrets.testpypi }}
+          repository-url: https://test.pypi.org/legacy/
 
       - name: Publish on PyPI
         if: github.event.ref_type == 'tag'
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: __token__
           password: ${{ secrets.pypi }}
 
       - name: Install Miniconda
         uses: conda-incubator/setup-miniconda@v2
         with:
```

### Comparing `labscript-utils-3.2.2/.gitignore` & `labscript-utils-3.3.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/BSD-2-CLAUSE-LICENSE.txt` & `labscript-utils-3.3.0rc1/BSD-2-CLAUSE-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/BSD-3-CLAUSE-LICENSE.txt` & `labscript-utils-3.3.0rc1/BSD-3-CLAUSE-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/LICENSE.txt` & `labscript-utils-3.3.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/NEWS.md` & `labscript-utils-3.3.0rc1/NEWS.md`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/PKG-INFO` & `labscript-utils-3.3.0rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labscript-utils
-Version: 3.2.2
+Version: 3.3.0rc1
 Summary: Shared utilities for the labscript suite
 Home-page: http://labscriptsuite.org
 Author: The labscript suite community
 Author-email: labscriptsuite@googlegroups.com
 License: BSD
 Project-URL: Source Code, https://github.com/labscript-suite/labscript-utils
 Project-URL: Download, https://github.com/labscript-suite/labscript-utils/releases
@@ -12,14 +12,16 @@
 Keywords: experiment control automation
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 <img src="https://raw.githubusercontent.com/labscript-suite/labscript-suite/master/art/labscript_32nx32n.svg" height="64" alt="the labscript suite" align="right">
```

### Comparing `labscript-utils-3.2.2/README.md` & `labscript-utils-3.3.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/docs/Makefile` & `labscript-utils-3.3.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/docs/make.bat` & `labscript-utils-3.3.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/docs/source/_static/custom.css` & `labscript-utils-3.3.0rc1/docs/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/docs/source/_templates/autosummary-class.rst` & `labscript-utils-3.3.0rc1/docs/source/_templates/autosummary-class.rst`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/docs/source/_templates/autosummary-module.rst` & `labscript-utils-3.3.0rc1/docs/source/_templates/autosummary-module.rst`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/docs/source/_templates/components.rst` & `labscript-utils-3.3.0rc1/docs/source/_templates/components.rst`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/docs/source/conf.py` & `labscript-utils-3.3.0rc1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/docs/source/img/blacs_32nx32n.svg` & `labscript-utils-3.3.0rc1/docs/source/img/blacs_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/docs/source/img/labscript-suite-rectangular-transparent_138nx70n.svg` & `labscript-utils-3.3.0rc1/docs/source/img/labscript-suite-rectangular-transparent_138nx70n.svg`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/docs/source/img/labscript.ico` & `labscript-utils-3.3.0rc1/docs/source/img/labscript.ico`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/docs/source/img/labscript_32nx32n.svg` & `labscript-utils-3.3.0rc1/docs/source/img/labscript_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/docs/source/img/labscript_64x64.svg` & `labscript-utils-3.3.0rc1/docs/source/img/labscript_64x64.svg`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/docs/source/img/lyse_32nx32n.svg` & `labscript-utils-3.3.0rc1/docs/source/img/lyse_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/docs/source/img/runmanager_32nx32n.svg` & `labscript-utils-3.3.0rc1/docs/source/img/runmanager_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/docs/source/img/runviewer_32nx32n.svg` & `labscript-utils-3.3.0rc1/docs/source/img/runviewer_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/docs/source/index.rst` & `labscript-utils-3.3.0rc1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/docs/source/labconfig.rst` & `labscript-utils-3.3.0rc1/docs/source/labconfig.rst`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/docs/source/pyqt5-modified-objects.inv` & `labscript-utils-3.3.0rc1/docs/source/pyqt5-modified-objects.inv`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_profile/__init__.py` & `labscript-utils-3.3.0rc1/labscript_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_profile/create.py` & `labscript-utils-3.3.0rc1/labscript_profile/create.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_profile/default_profile/labconfig/example.ini` & `labscript-utils-3.3.0rc1/labscript_profile/default_profile/labconfig/example.ini`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_profile/default_profile/userlib/analysislib/example_apparatus/example_IMAQdx_remote.py` & `labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/analysislib/example_apparatus/example_IMAQdx_remote.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/connection_table.py` & `labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/connection_table.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/connection_table_IMAQdx_remote.py` & `labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/connection_table_IMAQdx_remote.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/example_IMAQdx_remote.py` & `labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/example_IMAQdx_remote.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/example_experiment.py` & `labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/example_experiment.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_profile/default_profile/userlib/user_devices/README.txt` & `labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/user_devices/README.txt`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/__init__.py` & `labscript-utils-3.3.0rc1/labscript_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/camera_server.py` & `labscript-utils-3.3.0rc1/labscript_utils/camera_server.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/connections.py` & `labscript-utils-3.3.0rc1/labscript_utils/connections.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/device_registry/__init__.py` & `labscript-utils-3.3.0rc1/labscript_utils/device_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/device_registry/_device_registry.py` & `labscript-utils-3.3.0rc1/labscript_utils/device_registry/_device_registry.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/dict_diff.py` & `labscript-utils-3.3.0rc1/labscript_utils/dict_diff.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/double_import_denier.py` & `labscript-utils-3.3.0rc1/labscript_utils/double_import_denier.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/excepthook/__init__.py` & `labscript-utils-3.3.0rc1/labscript_utils/excepthook/__init__.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/excepthook/error.gif` & `labscript-utils-3.3.0rc1/labscript_utils/excepthook/error.gif`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/excepthook/tk_exception.py` & `labscript-utils-3.3.0rc1/labscript_utils/excepthook/tk_exception.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/filewatcher.py` & `labscript-utils-3.3.0rc1/labscript_utils/filewatcher.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/h5_lock.py` & `labscript-utils-3.3.0rc1/labscript_utils/h5_lock.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/impprof.py` & `labscript-utils-3.3.0rc1/labscript_utils/impprof.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/labconfig.py` & `labscript-utils-3.3.0rc1/labscript_utils/labconfig.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/ls_zprocess.py` & `labscript-utils-3.3.0rc1/labscript_utils/ls_zprocess.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/memprof.py` & `labscript-utils-3.3.0rc1/labscript_utils/memprof.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/modulewatcher.py` & `labscript-utils-3.3.0rc1/labscript_utils/modulewatcher.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/properties.py` & `labscript-utils-3.3.0rc1/labscript_utils/properties.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/qtwidgets/InputPlotWindow.py` & `labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/InputPlotWindow.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/qtwidgets/__init__.py` & `labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/qtwidgets/analoginput.py` & `labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/analoginput.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/qtwidgets/analogoutput.py` & `labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/analogoutput.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/qtwidgets/ddsoutput.py` & `labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/ddsoutput.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/qtwidgets/digitaloutput.py` & `labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/digitaloutput.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/qtwidgets/dragdroptab.py` & `labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/dragdroptab.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,15 +312,17 @@
 
                 # Check for overshoot:
                 if dx * (target_pos_x - new_pos_x) < 0:
                     new_pos_x = target_pos_x
                 if dy * (target_pos_y - new_pos_y) < 0:
                     new_pos_y = target_pos_y
 
-                self.limbo_position = QPoint(new_pos_x, new_pos_y)
+                self.limbo_position = QPoint(
+                    int(round(new_pos_x)), int(round(new_pos_y))
+                )
             else:
                 self.limbo.animation_over()
                 self.limbo = None
                 self.limbo_position = None
                 self.limbo_target_tab = None
         if finished:
             self.previous_time = 0
```

### Comparing `labscript-utils-3.2.2/labscript_utils/qtwidgets/elide_label.py` & `labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/elide_label.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/qtwidgets/enumoutput.py` & `labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/enumoutput.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/qtwidgets/fingertab.py` & `labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/fingertab.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/qtwidgets/headerview_with_widgets.py` & `labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/headerview_with_widgets.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/qtwidgets/imageoutput.py` & `labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/imageoutput.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/qtwidgets/outputbox.py` & `labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/outputbox.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/qtwidgets/toolpalette.py` & `labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/toolpalette.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/remote.py` & `labscript-utils-3.3.0rc1/labscript_utils/remote.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/settings.py` & `labscript-utils-3.3.0rc1/labscript_utils/settings.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/setup_logging.py` & `labscript-utils-3.3.0rc1/labscript_utils/setup_logging.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/shared_drive.py` & `labscript-utils-3.3.0rc1/labscript_utils/shared_drive.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/splash.py` & `labscript-utils-3.3.0rc1/labscript_utils/splash.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/testing_utils.py` & `labscript-utils-3.3.0rc1/labscript_utils/testing_utils.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/tracelog.py` & `labscript-utils-3.3.0rc1/labscript_utils/tracelog.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/unitconversions/NovaTechDDS9m.py` & `labscript-utils-3.3.0rc1/labscript_utils/unitconversions/NovaTechDDS9m.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/unitconversions/UnitConversionBase.py` & `labscript-utils-3.3.0rc1/labscript_utils/unitconversions/UnitConversionBase.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/unitconversions/__init__.py` & `labscript-utils-3.3.0rc1/labscript_utils/unitconversions/__init__.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/unitconversions/aom.py` & `labscript-utils-3.3.0rc1/labscript_utils/unitconversions/aom.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/unitconversions/detuning.py` & `labscript-utils-3.3.0rc1/labscript_utils/unitconversions/detuning.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/unitconversions/example.py` & `labscript-utils-3.3.0rc1/labscript_utils/unitconversions/example.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/unitconversions/generic_frequency.py` & `labscript-utils-3.3.0rc1/labscript_utils/unitconversions/generic_frequency.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/unitconversions/linear_coil_driver.py` & `labscript-utils-3.3.0rc1/labscript_utils/unitconversions/linear_coil_driver.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/unitconversions/optotunelens.py` & `labscript-utils-3.3.0rc1/labscript_utils/unitconversions/optotunelens.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/unitconversions/quad_driver.py` & `labscript-utils-3.3.0rc1/labscript_utils/unitconversions/quad_driver.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/unitconversions/quad_monitor.py` & `labscript-utils-3.3.0rc1/labscript_utils/unitconversions/quad_monitor.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/unitconversions/test.py` & `labscript-utils-3.3.0rc1/labscript_utils/unitconversions/test.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/versions.py` & `labscript-utils-3.3.0rc1/labscript_utils/versions.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/zlock.py` & `labscript-utils-3.3.0rc1/labscript_utils/zlock.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils/zlog.py` & `labscript-utils-3.3.0rc1/labscript_utils/zlog.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/labscript_utils.egg-info/PKG-INFO` & `labscript-utils-3.3.0rc1/labscript_utils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labscript-utils
-Version: 3.2.2
+Version: 3.3.0rc1
 Summary: Shared utilities for the labscript suite
 Home-page: http://labscriptsuite.org
 Author: The labscript suite community
 Author-email: labscriptsuite@googlegroups.com
 License: BSD
 Project-URL: Source Code, https://github.com/labscript-suite/labscript-utils
 Project-URL: Download, https://github.com/labscript-suite/labscript-utils/releases
@@ -12,14 +12,16 @@
 Keywords: experiment control automation
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 <img src="https://raw.githubusercontent.com/labscript-suite/labscript-suite/master/art/labscript_32nx32n.svg" height="64" alt="the labscript suite" align="right">
```

### Comparing `labscript-utils-3.2.2/labscript_utils.egg-info/SOURCES.txt` & `labscript-utils-3.3.0rc1/labscript_utils.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 labscript_utils/memprof.py
 labscript_utils/modulewatcher.py
 labscript_utils/properties.py
 labscript_utils/remote.py
 labscript_utils/settings.py
 labscript_utils/setup_logging.py
 labscript_utils/shared_drive.py
+labscript_utils/shot_utils.py
 labscript_utils/splash.py
 labscript_utils/testing_utils.py
 labscript_utils/tracelog.py
 labscript_utils/versions.py
 labscript_utils/zlock.py
 labscript_utils/zlog.py
 labscript_utils.egg-info/PKG-INFO
```

### Comparing `labscript-utils-3.2.2/readthedocs.yaml` & `labscript-utils-3.3.0rc1/readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.2.2/setup.cfg` & `labscript-utils-3.3.0rc1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -15,26 +15,28 @@
 classifiers = 
 	License :: OSI Approved :: BSD License
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = labscript_utils, labscript_profile
 python_requires = >=3.6
 install_requires = 
 	importlib_metadata>=1.0
 	h5py>=2.9
 	numpy>=1.15
 	packaging>=20.4
-	pyqtgraph>=0.11.0
+	pyqtgraph>=0.11.0rc0
 	qtutils>=2.2.3
 	scipy
 	setuptools_scm>=4.1.0
 	zprocess>=2.18.0
 
 [options.extras_require]
 docs =
```

### Comparing `labscript-utils-3.2.2/setup.py` & `labscript-utils-3.3.0rc1/setup.py`

 * *Files identical despite different names*

