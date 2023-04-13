# Comparing `tmp/labscript-devices-3.2.0.tar.gz` & `tmp/labscript-devices-3.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labscript-devices-3.2.0.tar", last modified: Thu Apr 13 00:13:04 2023, max compression
+gzip compressed data, was "labscript-devices-3.2.0rc1.tar", last modified: Wed Apr 12 19:48:14 2023, max compression
```

## Comparing `labscript-devices-3.2.0.tar` & `labscript-devices-3.2.0rc1.tar`

### file list

```diff
@@ -1,218 +1,218 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:13:04.878219 labscript-devices-3.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:13:04.806218 labscript-devices-3.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:13:04.814218 labscript-devices-3.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/BSD-2-CLAUSE-LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/BSD-3-CLAUSE-LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/NEWS.md
--rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-04-13 00:13:04.878219 labscript-devices-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8669 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:13:04.814218 labscript-devices-3.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:13:04.818218 labscript-devices-3.2.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:13:04.818218 labscript-devices-3.2.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:13:04.818218 labscript-devices-3.2.0/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/_templates/components.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:13:04.818218 labscript-devices-3.2.0/docs/source/_templates/models/
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/_templates/models/package.rst_t
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/adding_devices.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:13:04.826218 labscript-devices-3.2.0/docs/source/devices/
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/devices/IMAQdx.rst
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/devices/alazartechboard.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/devices/andorsolis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/devices/dummyintermediate.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/devices/dummypseudoclock.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/devices/flycapture2.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/devices/functionrunner.rst
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/devices/lightcrafterdmd.rst
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/devices/ni_daq_models.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/devices/ni_daqs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/devices/novatechDDS9m.rst
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/devices/opalkellyXEM3001.rst
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/devices/phasematrixquicksyn.rst
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/devices/pineblaster.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/devices/prawnblaster.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/devices/pulseblaster.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/devices/pulseblaster_no_dds.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/devices/pylon.rst
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/devices/rfblaster.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/devices/spinnaker.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/devices/tekscope.rst
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/devices/testdevice.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/devices/zaberstagecontroller.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/devices.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/ex_conn_tables.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:13:04.830218 labscript-devices-3.2.0/docs/source/img/
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/img/blacs_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)    98716 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/img/labscript.ico
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/img/labscript_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/img/labscript_64x64.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/img/lyse_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/img/runmanager_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/img/runviewer_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)    64143 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/pyqt5-modified-objects.inv
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/docs/source/user_devices.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:13:04.838219 labscript-devices-3.2.0/labscript_devices/
--rw-r--r--   0 runner    (1001) docker     (123)    34928 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/AlazarTechBoard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:13:04.842218 labscript-devices-3.2.0/labscript_devices/AndorSolis/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/AndorSolis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:13:04.846218 labscript-devices-3.2.0/labscript_devices/AndorSolis/andor_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/AndorSolis/andor_sdk/andor_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    64381 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/AndorSolis/andor_sdk/andor_solis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/AndorSolis/andor_sdk/andor_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)    27658 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/AndorSolis/andor_sdk/andor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/AndorSolis/andor_sdk/status_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/AndorSolis/blacs_tabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/AndorSolis/blacs_workers.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/AndorSolis/labscript_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/AndorSolis/register_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14617 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/Camera.py
--rw-r--r--   0 runner    (1001) docker     (123)    34845 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/CiceroOpalKellyXEM3001.py
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/DummyIntermediateDevice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:13:04.846218 labscript-devices-3.2.0/labscript_devices/DummyPseudoclock/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/DummyPseudoclock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/DummyPseudoclock/blacs_tabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/DummyPseudoclock/blacs_workers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/DummyPseudoclock/labscript_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/DummyPseudoclock/register_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/DummyPseudoclock/runviewer_parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:13:04.850218 labscript-devices-3.2.0/labscript_devices/FlyCapture2Camera/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/FlyCapture2Camera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/FlyCapture2Camera/blacs_tabs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20538 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/FlyCapture2Camera/blacs_workers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/FlyCapture2Camera/labscript_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/FlyCapture2Camera/register_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:13:04.850218 labscript-devices-3.2.0/labscript_devices/FunctionRunner/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/FunctionRunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/FunctionRunner/blacs_tabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/FunctionRunner/blacs_workers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/FunctionRunner/labscript_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/FunctionRunner/register_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:13:04.850218 labscript-devices-3.2.0/labscript_devices/FunctionRunner/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/FunctionRunner/testing/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/FunctionRunner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:13:04.854219 labscript-devices-3.2.0/labscript_devices/IMAQdxCamera/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/IMAQdxCamera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/IMAQdxCamera/attributes_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/IMAQdxCamera/blacs_tab.ui
--rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/IMAQdxCamera/blacs_tabs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/IMAQdxCamera/blacs_workers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11899 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/IMAQdxCamera/labscript_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/IMAQdxCamera/register_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:13:04.854219 labscript-devices-3.2.0/labscript_devices/IMAQdxCamera/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/IMAQdxCamera/testing/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16904 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/LightCrafterDMD.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:13:04.858219 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/blacs_tabs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42192 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/blacs_workers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/daqmx_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    30327 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/labscript_devices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:13:04.866219 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_PCI_6251.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_PCI_6534.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_PCI_6713.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_PCI_6733.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_PCI_DIO_32HS.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_PCIe_6343.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_PCIe_6363.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_PCIe_6738.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_PXI_6733.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_PXIe_4499.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_PXIe_6361.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_PXIe_6363.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_PXIe_6535.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_PXIe_6738.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_USB_6008.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_USB_6229.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_USB_6343.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_USB_6363.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_USB_6366.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/_subclass_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    43041 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/capabilities.json
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/generate_subclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)    24733 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/get_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/register_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/runviewer_parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:13:04.866219 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/testing/
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/testing/test_NI_DAQmx_labscript.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_DAQmx/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_PCI_6733.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_PCIe_6363.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NI_USB_6343.py
--rw-r--r--   0 runner    (1001) docker     (123)    32545 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/NovaTechDDS9M.py
--rw-r--r--   0 runner    (1001) docker     (123)    16193 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/PhaseMatrixQuickSyn.py
--rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/PineBlaster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:13:04.870219 labscript-devices-3.2.0/labscript_devices/PrawnBlaster/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/PrawnBlaster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/PrawnBlaster/blacs_tabs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18525 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/PrawnBlaster/blacs_workers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19713 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/PrawnBlaster/labscript_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/PrawnBlaster/register_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/PrawnBlaster/runviewer_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)    69933 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/PulseBlaster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/PulseBlasterESRPro200.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/PulseBlasterESRPro500.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/PulseBlasterUSB.py
--rw-r--r--   0 runner    (1001) docker     (123)    22696 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/PulseBlaster_No_DDS.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/PulseBlaster_SP2_24_100_32k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:13:04.870219 labscript-devices-3.2.0/labscript_devices/PylonCamera/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/PylonCamera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/PylonCamera/blacs_tabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/PylonCamera/blacs_workers.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/PylonCamera/labscript_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/PylonCamera/register_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:13:04.870219 labscript-devices-3.2.0/labscript_devices/PylonCamera/testing/
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/PylonCamera/testing/ExposureTiming.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/PythonCamera.py
--rw-r--r--   0 runner    (1001) docker     (123)    25523 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/RFBlaster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:13:04.874219 labscript-devices-3.2.0/labscript_devices/SpinnakerCamera/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/SpinnakerCamera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/SpinnakerCamera/blacs_tabs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/SpinnakerCamera/blacs_workers.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/SpinnakerCamera/labscript_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/SpinnakerCamera/register_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:13:04.874219 labscript-devices-3.2.0/labscript_devices/TekScope/
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/TekScope/TekScope.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/TekScope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/TekScope/blacs_tabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/TekScope/blacs_workers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/TekScope/labscript_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/TekScope/register_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:13:04.878219 labscript-devices-3.2.0/labscript_devices/ZaberStageController/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/ZaberStageController/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/ZaberStageController/blacs_tabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/ZaberStageController/blacs_workers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/ZaberStageController/labscript_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/ZaberStageController/register_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:13:04.878219 labscript-devices-3.2.0/labscript_devices/ZaberStageController/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/ZaberStageController/testing/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/ZaberStageController/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44881 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/atsapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/camera.ui
--rw-r--r--   0 runner    (1001) docker     (123)    19575 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/imaqdx_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/phasematrixquicksyn.ui
--rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/pulseblaster.ui
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/labscript_devices/test_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:13:04.842218 labscript-devices-3.2.0/labscript_devices.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-04-13 00:13:04.000000 labscript-devices-3.2.0/labscript_devices.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-04-13 00:13:04.000000 labscript-devices-3.2.0/labscript_devices.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 00:13:04.000000 labscript-devices-3.2.0/labscript_devices.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 00:13:04.000000 labscript-devices-3.2.0/labscript_devices.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-13 00:13:04.000000 labscript-devices-3.2.0/labscript_devices.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 00:13:04.000000 labscript-devices-3.2.0/labscript_devices.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-13 00:13:04.878219 labscript-devices-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-13 00:12:53.000000 labscript-devices-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.682700 labscript-devices-3.2.0rc1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.654699 labscript-devices-3.2.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.658700 labscript-devices-3.2.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/BSD-2-CLAUSE-LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/BSD-3-CLAUSE-LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/NEWS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-04-12 19:48:14.682700 labscript-devices-3.2.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8669 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.658700 labscript-devices-3.2.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.658700 labscript-devices-3.2.0rc1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.658700 labscript-devices-3.2.0rc1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.658700 labscript-devices-3.2.0rc1/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/_templates/components.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.658700 labscript-devices-3.2.0rc1/docs/source/_templates/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/_templates/models/package.rst_t
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/adding_devices.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.662700 labscript-devices-3.2.0rc1/docs/source/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/IMAQdx.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/alazartechboard.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/andorsolis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/dummyintermediate.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/dummypseudoclock.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/flycapture2.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/functionrunner.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/lightcrafterdmd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/ni_daq_models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/ni_daqs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/novatechDDS9m.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/opalkellyXEM3001.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/phasematrixquicksyn.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/pineblaster.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/prawnblaster.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/pulseblaster.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/pulseblaster_no_dds.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/pylon.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/rfblaster.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/spinnaker.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/tekscope.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/testdevice.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices/zaberstagecontroller.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/devices.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/ex_conn_tables.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.662700 labscript-devices-3.2.0rc1/docs/source/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/img/blacs_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    98716 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/img/labscript.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/img/labscript_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/img/labscript_64x64.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/img/lyse_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/img/runmanager_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/img/runviewer_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    64143 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/pyqt5-modified-objects.inv
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/docs/source/user_devices.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.666700 labscript-devices-3.2.0rc1/labscript_devices/
+-rw-r--r--   0 runner    (1001) docker     (123)    34928 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/AlazarTechBoard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.670700 labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.670700 labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/andor_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/andor_sdk/andor_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64381 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/andor_sdk/andor_solis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/andor_sdk/andor_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27658 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/andor_sdk/andor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/andor_sdk/status_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/blacs_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/blacs_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/labscript_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/register_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14617 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/Camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34845 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/CiceroOpalKellyXEM3001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/DummyIntermediateDevice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.670700 labscript-devices-3.2.0rc1/labscript_devices/DummyPseudoclock/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/DummyPseudoclock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/DummyPseudoclock/blacs_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/DummyPseudoclock/blacs_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/DummyPseudoclock/labscript_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/DummyPseudoclock/register_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/DummyPseudoclock/runviewer_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.670700 labscript-devices-3.2.0rc1/labscript_devices/FlyCapture2Camera/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/FlyCapture2Camera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/FlyCapture2Camera/blacs_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20538 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/FlyCapture2Camera/blacs_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/FlyCapture2Camera/labscript_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/FlyCapture2Camera/register_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.670700 labscript-devices-3.2.0rc1/labscript_devices/FunctionRunner/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/FunctionRunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/FunctionRunner/blacs_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/FunctionRunner/blacs_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/FunctionRunner/labscript_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/FunctionRunner/register_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.670700 labscript-devices-3.2.0rc1/labscript_devices/FunctionRunner/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/FunctionRunner/testing/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/FunctionRunner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.674700 labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/attributes_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/blacs_tab.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/blacs_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/blacs_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11899 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/labscript_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/register_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.674700 labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/testing/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16904 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/LightCrafterDMD.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.674700 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/blacs_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42192 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/blacs_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/daqmx_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30327 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/labscript_devices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.674700 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PCI_6251.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PCI_6534.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PCI_6713.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PCI_6733.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PCI_DIO_32HS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PCIe_6343.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PCIe_6363.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PCIe_6738.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PXI_6733.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PXIe_4499.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PXIe_6361.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PXIe_6363.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PXIe_6535.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PXIe_6738.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_USB_6008.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_USB_6229.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_USB_6343.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_USB_6363.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_USB_6366.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/_subclass_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43041 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/capabilities.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/generate_subclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24733 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/get_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/register_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/runviewer_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.678700 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/testing/test_NI_DAQmx_labscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_PCI_6733.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_PCIe_6363.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NI_USB_6343.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32545 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/NovaTechDDS9M.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16193 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PhaseMatrixQuickSyn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PineBlaster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.678700 labscript-devices-3.2.0rc1/labscript_devices/PrawnBlaster/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PrawnBlaster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PrawnBlaster/blacs_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18525 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PrawnBlaster/blacs_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19713 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PrawnBlaster/labscript_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PrawnBlaster/register_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PrawnBlaster/runviewer_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69933 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PulseBlaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PulseBlasterESRPro200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PulseBlasterESRPro500.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PulseBlasterUSB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22696 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PulseBlaster_No_DDS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PulseBlaster_SP2_24_100_32k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.678700 labscript-devices-3.2.0rc1/labscript_devices/PylonCamera/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PylonCamera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PylonCamera/blacs_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PylonCamera/blacs_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PylonCamera/labscript_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PylonCamera/register_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.678700 labscript-devices-3.2.0rc1/labscript_devices/PylonCamera/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PylonCamera/testing/ExposureTiming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/PythonCamera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25523 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/RFBlaster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.682700 labscript-devices-3.2.0rc1/labscript_devices/SpinnakerCamera/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/SpinnakerCamera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/SpinnakerCamera/blacs_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/SpinnakerCamera/blacs_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/SpinnakerCamera/labscript_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/SpinnakerCamera/register_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.682700 labscript-devices-3.2.0rc1/labscript_devices/TekScope/
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/TekScope/TekScope.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/TekScope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/TekScope/blacs_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/TekScope/blacs_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/TekScope/labscript_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/TekScope/register_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.682700 labscript-devices-3.2.0rc1/labscript_devices/ZaberStageController/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/ZaberStageController/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/ZaberStageController/blacs_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/ZaberStageController/blacs_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/ZaberStageController/labscript_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/ZaberStageController/register_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.682700 labscript-devices-3.2.0rc1/labscript_devices/ZaberStageController/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/ZaberStageController/testing/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/ZaberStageController/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44881 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/atsapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/camera.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    19575 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/imaqdx_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/phasematrixquicksyn.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/pulseblaster.ui
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/labscript_devices/test_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:48:14.666700 labscript-devices-3.2.0rc1/labscript_devices.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-04-12 19:48:14.000000 labscript-devices-3.2.0rc1/labscript_devices.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-04-12 19:48:14.000000 labscript-devices-3.2.0rc1/labscript_devices.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 19:48:14.000000 labscript-devices-3.2.0rc1/labscript_devices.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 19:48:14.000000 labscript-devices-3.2.0rc1/labscript_devices.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-12 19:48:14.000000 labscript-devices-3.2.0rc1/labscript_devices.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 19:48:14.000000 labscript-devices-3.2.0rc1/labscript_devices.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-12 19:48:14.682700 labscript-devices-3.2.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-12 19:48:04.000000 labscript-devices-3.2.0rc1/setup.py
```

### Comparing `labscript-devices-3.2.0/.github/workflows/release.yml` & `labscript-devices-3.2.0rc1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/.gitignore` & `labscript-devices-3.2.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/BSD-2-CLAUSE-LICENSE.txt` & `labscript-devices-3.2.0rc1/BSD-2-CLAUSE-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/BSD-3-CLAUSE-LICENSE.txt` & `labscript-devices-3.2.0rc1/BSD-3-CLAUSE-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/LICENSE.txt` & `labscript-devices-3.2.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/NEWS.md` & `labscript-devices-3.2.0rc1/NEWS.md`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/PKG-INFO` & `labscript-devices-3.2.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labscript-devices
-Version: 3.2.0
+Version: 3.2.0rc1
 Summary: Device drivers for hardware controlled by the labscript suite
 Home-page: http://labscriptsuite.org
 Author: The labscript suite community
 Author-email: labscriptsuite@googlegroups.com
 License: BSD
 Project-URL: Source Code, https://github.com/labscript-suite/labscript-devices
 Project-URL: Download, https://github.com/labscript-suite/labscript-devices/releases
```

### Comparing `labscript-devices-3.2.0/README.md` & `labscript-devices-3.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/Makefile` & `labscript-devices-3.2.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/make.bat` & `labscript-devices-3.2.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/source/_static/custom.css` & `labscript-devices-3.2.0rc1/docs/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/source/_templates/components.rst` & `labscript-devices-3.2.0rc1/docs/source/_templates/components.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/source/_templates/models/package.rst_t` & `labscript-devices-3.2.0rc1/docs/source/_templates/models/package.rst_t`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/source/adding_devices.rst` & `labscript-devices-3.2.0rc1/docs/source/adding_devices.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/source/conf.py` & `labscript-devices-3.2.0rc1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/source/devices/IMAQdx.rst` & `labscript-devices-3.2.0rc1/docs/source/devices/IMAQdx.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/source/devices/alazartechboard.rst` & `labscript-devices-3.2.0rc1/docs/source/devices/alazartechboard.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/source/devices/andorsolis.rst` & `labscript-devices-3.2.0rc1/docs/source/devices/andorsolis.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/source/devices/dummypseudoclock.rst` & `labscript-devices-3.2.0rc1/docs/source/devices/dummypseudoclock.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/source/devices/flycapture2.rst` & `labscript-devices-3.2.0rc1/docs/source/devices/flycapture2.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/source/devices/functionrunner.rst` & `labscript-devices-3.2.0rc1/docs/source/devices/functionrunner.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/source/devices/ni_daqs.rst` & `labscript-devices-3.2.0rc1/docs/source/devices/ni_daqs.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/source/devices/opalkellyXEM3001.rst` & `labscript-devices-3.2.0rc1/docs/source/devices/opalkellyXEM3001.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/source/devices/prawnblaster.rst` & `labscript-devices-3.2.0rc1/docs/source/devices/prawnblaster.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/source/devices/pulseblaster.rst` & `labscript-devices-3.2.0rc1/docs/source/devices/pulseblaster.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/source/devices/pulseblaster_no_dds.rst` & `labscript-devices-3.2.0rc1/docs/source/devices/pulseblaster_no_dds.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/source/devices/pylon.rst` & `labscript-devices-3.2.0rc1/docs/source/devices/pylon.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/source/devices/spinnaker.rst` & `labscript-devices-3.2.0rc1/docs/source/devices/spinnaker.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/source/devices/tekscope.rst` & `labscript-devices-3.2.0rc1/docs/source/devices/tekscope.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/source/devices/zaberstagecontroller.rst` & `labscript-devices-3.2.0rc1/docs/source/devices/zaberstagecontroller.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/source/devices.rst` & `labscript-devices-3.2.0rc1/docs/source/devices.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/source/ex_conn_tables.rst` & `labscript-devices-3.2.0rc1/docs/source/ex_conn_tables.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/source/img/blacs_32nx32n.svg` & `labscript-devices-3.2.0rc1/docs/source/img/blacs_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/source/img/labscript.ico` & `labscript-devices-3.2.0rc1/docs/source/img/labscript.ico`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/source/img/labscript_32nx32n.svg` & `labscript-devices-3.2.0rc1/docs/source/img/labscript_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/source/img/labscript_64x64.svg` & `labscript-devices-3.2.0rc1/docs/source/img/labscript_64x64.svg`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/source/img/lyse_32nx32n.svg` & `labscript-devices-3.2.0rc1/docs/source/img/lyse_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/source/img/runmanager_32nx32n.svg` & `labscript-devices-3.2.0rc1/docs/source/img/runmanager_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/source/img/runviewer_32nx32n.svg` & `labscript-devices-3.2.0rc1/docs/source/img/runviewer_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/source/index.rst` & `labscript-devices-3.2.0rc1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/source/introduction.rst` & `labscript-devices-3.2.0rc1/docs/source/introduction.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/source/pyqt5-modified-objects.inv` & `labscript-devices-3.2.0rc1/docs/source/pyqt5-modified-objects.inv`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/docs/source/user_devices.rst` & `labscript-devices-3.2.0rc1/docs/source/user_devices.rst`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/AlazarTechBoard.py` & `labscript-devices-3.2.0rc1/labscript_devices/AlazarTechBoard.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/AndorSolis/__init__.py` & `labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/__init__.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/AndorSolis/andor_sdk/andor_capabilities.py` & `labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/andor_sdk/andor_capabilities.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/AndorSolis/andor_sdk/andor_solis.py` & `labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/andor_sdk/andor_solis.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/AndorSolis/andor_sdk/andor_structures.py` & `labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/andor_sdk/andor_structures.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/AndorSolis/andor_sdk/andor_utils.py` & `labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/andor_sdk/andor_utils.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/AndorSolis/andor_sdk/status_codes.py` & `labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/andor_sdk/status_codes.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/AndorSolis/blacs_tabs.py` & `labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/blacs_tabs.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/AndorSolis/blacs_workers.py` & `labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/blacs_workers.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/AndorSolis/labscript_devices.py` & `labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/labscript_devices.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/AndorSolis/register_classes.py` & `labscript-devices-3.2.0rc1/labscript_devices/AndorSolis/register_classes.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/Camera.py` & `labscript-devices-3.2.0rc1/labscript_devices/Camera.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/CiceroOpalKellyXEM3001.py` & `labscript-devices-3.2.0rc1/labscript_devices/CiceroOpalKellyXEM3001.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/DummyIntermediateDevice.py` & `labscript-devices-3.2.0rc1/labscript_devices/DummyIntermediateDevice.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/DummyPseudoclock/__init__.py` & `labscript-devices-3.2.0rc1/labscript_devices/DummyPseudoclock/__init__.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/DummyPseudoclock/blacs_tabs.py` & `labscript-devices-3.2.0rc1/labscript_devices/DummyPseudoclock/blacs_tabs.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/DummyPseudoclock/blacs_workers.py` & `labscript-devices-3.2.0rc1/labscript_devices/DummyPseudoclock/blacs_workers.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/DummyPseudoclock/labscript_devices.py` & `labscript-devices-3.2.0rc1/labscript_devices/DummyPseudoclock/labscript_devices.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/DummyPseudoclock/register_classes.py` & `labscript-devices-3.2.0rc1/labscript_devices/DummyPseudoclock/register_classes.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/DummyPseudoclock/runviewer_parsers.py` & `labscript-devices-3.2.0rc1/labscript_devices/DummyPseudoclock/runviewer_parsers.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/FlyCapture2Camera/blacs_tabs.py` & `labscript-devices-3.2.0rc1/labscript_devices/FlyCapture2Camera/blacs_tabs.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/FlyCapture2Camera/blacs_workers.py` & `labscript-devices-3.2.0rc1/labscript_devices/FlyCapture2Camera/blacs_workers.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/FlyCapture2Camera/labscript_devices.py` & `labscript-devices-3.2.0rc1/labscript_devices/FlyCapture2Camera/labscript_devices.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/FlyCapture2Camera/register_classes.py` & `labscript-devices-3.2.0rc1/labscript_devices/FlyCapture2Camera/register_classes.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/FunctionRunner/__init__.py` & `labscript-devices-3.2.0rc1/labscript_devices/FunctionRunner/__init__.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/FunctionRunner/blacs_tabs.py` & `labscript-devices-3.2.0rc1/labscript_devices/FunctionRunner/blacs_tabs.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/FunctionRunner/blacs_workers.py` & `labscript-devices-3.2.0rc1/labscript_devices/FunctionRunner/blacs_workers.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/FunctionRunner/labscript_devices.py` & `labscript-devices-3.2.0rc1/labscript_devices/FunctionRunner/labscript_devices.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/FunctionRunner/register_classes.py` & `labscript-devices-3.2.0rc1/labscript_devices/FunctionRunner/register_classes.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/FunctionRunner/testing/test.py` & `labscript-devices-3.2.0rc1/labscript_devices/FunctionRunner/testing/test.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/FunctionRunner/utils.py` & `labscript-devices-3.2.0rc1/labscript_devices/FunctionRunner/utils.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/IMAQdxCamera/attributes_dialog.ui` & `labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/attributes_dialog.ui`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/IMAQdxCamera/blacs_tab.ui` & `labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/blacs_tab.ui`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/IMAQdxCamera/blacs_tabs.py` & `labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/blacs_tabs.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/IMAQdxCamera/blacs_workers.py` & `labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/blacs_workers.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/IMAQdxCamera/labscript_devices.py` & `labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/labscript_devices.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/IMAQdxCamera/register_classes.py` & `labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/register_classes.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/IMAQdxCamera/testing/test.py` & `labscript-devices-3.2.0rc1/labscript_devices/IMAQdxCamera/testing/test.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/LightCrafterDMD.py` & `labscript-devices-3.2.0rc1/labscript_devices/LightCrafterDMD.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/__init__.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/__init__.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/blacs_tabs.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/blacs_tabs.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/blacs_workers.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/blacs_workers.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/daqmx_utils.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/daqmx_utils.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/labscript_devices.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/labscript_devices.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_PCI_6251.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PCI_6251.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_PCI_6534.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PCI_6534.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_PCI_6713.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PCI_6713.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_PCI_6733.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PCI_6733.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_PCI_DIO_32HS.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PCI_DIO_32HS.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_PCIe_6343.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PCIe_6343.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_PCIe_6363.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PCIe_6363.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_PCIe_6738.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PCIe_6738.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_PXI_6733.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PXI_6733.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_PXIe_4499.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PXIe_4499.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_PXIe_6361.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PXIe_6361.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_PXIe_6363.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PXIe_6363.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_PXIe_6535.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PXIe_6535.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_PXIe_6738.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_PXIe_6738.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_USB_6008.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_USB_6008.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_USB_6229.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_USB_6229.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_USB_6343.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_USB_6343.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_USB_6363.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_USB_6363.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/NI_USB_6366.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/NI_USB_6366.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/README.txt` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/README.txt`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/__init__.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/__init__.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/_subclass_template.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/_subclass_template.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/capabilities.json` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/capabilities.json`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/generate_subclasses.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/generate_subclasses.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/models/get_capabilities.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/models/get_capabilities.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/register_classes.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/register_classes.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/runviewer_parsers.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/runviewer_parsers.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/testing/test_NI_DAQmx_labscript.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/testing/test_NI_DAQmx_labscript.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_DAQmx/utils.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_DAQmx/utils.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_PCI_6733.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_PCI_6733.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_PCIe_6363.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_PCIe_6363.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NI_USB_6343.py` & `labscript-devices-3.2.0rc1/labscript_devices/NI_USB_6343.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/NovaTechDDS9M.py` & `labscript-devices-3.2.0rc1/labscript_devices/NovaTechDDS9M.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/PhaseMatrixQuickSyn.py` & `labscript-devices-3.2.0rc1/labscript_devices/PhaseMatrixQuickSyn.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/PineBlaster.py` & `labscript-devices-3.2.0rc1/labscript_devices/PineBlaster.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/PrawnBlaster/__init__.py` & `labscript-devices-3.2.0rc1/labscript_devices/PrawnBlaster/__init__.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/PrawnBlaster/blacs_tabs.py` & `labscript-devices-3.2.0rc1/labscript_devices/PrawnBlaster/blacs_tabs.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/PrawnBlaster/blacs_workers.py` & `labscript-devices-3.2.0rc1/labscript_devices/PrawnBlaster/blacs_workers.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/PrawnBlaster/labscript_devices.py` & `labscript-devices-3.2.0rc1/labscript_devices/PrawnBlaster/labscript_devices.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/PrawnBlaster/register_classes.py` & `labscript-devices-3.2.0rc1/labscript_devices/PrawnBlaster/register_classes.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/PrawnBlaster/runviewer_parsers.py` & `labscript-devices-3.2.0rc1/labscript_devices/PrawnBlaster/runviewer_parsers.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/PulseBlaster.py` & `labscript-devices-3.2.0rc1/labscript_devices/PulseBlaster.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/PulseBlasterESRPro200.py` & `labscript-devices-3.2.0rc1/labscript_devices/PulseBlasterESRPro200.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/PulseBlasterESRPro500.py` & `labscript-devices-3.2.0rc1/labscript_devices/PulseBlasterESRPro500.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/PulseBlasterUSB.py` & `labscript-devices-3.2.0rc1/labscript_devices/PulseBlasterUSB.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/PulseBlaster_No_DDS.py` & `labscript-devices-3.2.0rc1/labscript_devices/PulseBlaster_No_DDS.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/PulseBlaster_SP2_24_100_32k.py` & `labscript-devices-3.2.0rc1/labscript_devices/PulseBlaster_SP2_24_100_32k.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/PylonCamera/blacs_tabs.py` & `labscript-devices-3.2.0rc1/labscript_devices/PylonCamera/blacs_tabs.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/PylonCamera/blacs_workers.py` & `labscript-devices-3.2.0rc1/labscript_devices/PylonCamera/blacs_workers.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/PylonCamera/labscript_devices.py` & `labscript-devices-3.2.0rc1/labscript_devices/PylonCamera/labscript_devices.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/PylonCamera/register_classes.py` & `labscript-devices-3.2.0rc1/labscript_devices/PylonCamera/register_classes.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/PylonCamera/testing/ExposureTiming.py` & `labscript-devices-3.2.0rc1/labscript_devices/PylonCamera/testing/ExposureTiming.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/PythonCamera.py` & `labscript-devices-3.2.0rc1/labscript_devices/PythonCamera.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/RFBlaster.py` & `labscript-devices-3.2.0rc1/labscript_devices/RFBlaster.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/SpinnakerCamera/blacs_tabs.py` & `labscript-devices-3.2.0rc1/labscript_devices/SpinnakerCamera/blacs_tabs.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/SpinnakerCamera/blacs_workers.py` & `labscript-devices-3.2.0rc1/labscript_devices/SpinnakerCamera/blacs_workers.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/SpinnakerCamera/labscript_devices.py` & `labscript-devices-3.2.0rc1/labscript_devices/SpinnakerCamera/labscript_devices.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/SpinnakerCamera/register_classes.py` & `labscript-devices-3.2.0rc1/labscript_devices/SpinnakerCamera/register_classes.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/TekScope/TekScope.py` & `labscript-devices-3.2.0rc1/labscript_devices/TekScope/TekScope.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/TekScope/blacs_tabs.py` & `labscript-devices-3.2.0rc1/labscript_devices/TekScope/blacs_tabs.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/TekScope/blacs_workers.py` & `labscript-devices-3.2.0rc1/labscript_devices/TekScope/blacs_workers.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/TekScope/labscript_devices.py` & `labscript-devices-3.2.0rc1/labscript_devices/TekScope/labscript_devices.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/ZaberStageController/__init__.py` & `labscript-devices-3.2.0rc1/labscript_devices/ZaberStageController/__init__.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/ZaberStageController/blacs_tabs.py` & `labscript-devices-3.2.0rc1/labscript_devices/ZaberStageController/blacs_tabs.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/ZaberStageController/blacs_workers.py` & `labscript-devices-3.2.0rc1/labscript_devices/ZaberStageController/blacs_workers.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/ZaberStageController/labscript_devices.py` & `labscript-devices-3.2.0rc1/labscript_devices/ZaberStageController/labscript_devices.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/ZaberStageController/register_classes.py` & `labscript-devices-3.2.0rc1/labscript_devices/ZaberStageController/register_classes.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/ZaberStageController/utils.py` & `labscript-devices-3.2.0rc1/labscript_devices/ZaberStageController/utils.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/__version__.py` & `labscript-devices-3.2.0rc1/labscript_devices/__version__.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/atsapi.py` & `labscript-devices-3.2.0rc1/labscript_devices/atsapi.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/camera.ui` & `labscript-devices-3.2.0rc1/labscript_devices/camera.ui`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/imaqdx_server.py` & `labscript-devices-3.2.0rc1/labscript_devices/imaqdx_server.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/phasematrixquicksyn.ui` & `labscript-devices-3.2.0rc1/labscript_devices/phasematrixquicksyn.ui`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/pulseblaster.ui` & `labscript-devices-3.2.0rc1/labscript_devices/pulseblaster.ui`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices/test_device.py` & `labscript-devices-3.2.0rc1/labscript_devices/test_device.py`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/labscript_devices.egg-info/PKG-INFO` & `labscript-devices-3.2.0rc1/labscript_devices.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labscript-devices
-Version: 3.2.0
+Version: 3.2.0rc1
 Summary: Device drivers for hardware controlled by the labscript suite
 Home-page: http://labscriptsuite.org
 Author: The labscript suite community
 Author-email: labscriptsuite@googlegroups.com
 License: BSD
 Project-URL: Source Code, https://github.com/labscript-suite/labscript-devices
 Project-URL: Download, https://github.com/labscript-suite/labscript-devices/releases
```

### Comparing `labscript-devices-3.2.0/labscript_devices.egg-info/SOURCES.txt` & `labscript-devices-3.2.0rc1/labscript_devices.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/readthedocs.yaml` & `labscript-devices-3.2.0rc1/readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `labscript-devices-3.2.0/setup.cfg` & `labscript-devices-3.2.0rc1/setup.cfg`

 * *Files identical despite different names*

