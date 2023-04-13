# Comparing `tmp/jaeger-1.3.3.tar.gz` & `tmp/jaeger-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaeger-1.3.3.tar", max compression
+gzip compressed data, was "jaeger-1.3.4.tar", max compression
```

## Comparing `jaeger-1.3.3.tar` & `jaeger-1.3.4.tar`

### file list

```diff
@@ -1,75 +1,74 @@
--rw-r--r--   0        0        0     1504 2023-01-15 17:36:40.885530 jaeger-1.3.3/LICENSE.md
--rw-r--r--   0        0        0     2386 2023-01-15 17:36:40.885761 jaeger-1.3.3/README.md
--rw-r--r--   0        0        0     3309 2023-01-15 17:36:40.893718 jaeger-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     1746 2023-01-15 17:36:40.894147 jaeger-1.3.3/python/jaeger/__init__.py
--rw-r--r--   0        0        0    20341 2023-01-15 17:36:40.894460 jaeger-1.3.3/python/jaeger/__main__.py
--rw-r--r--   0        0        0       61 2023-01-15 17:36:40.894711 jaeger-1.3.3/python/jaeger/actor/__init__.py
--rw-r--r--   0        0        0     5034 2023-01-15 17:36:40.894964 jaeger-1.3.3/python/jaeger/actor/actor.py
--rw-r--r--   0        0        0      816 2023-01-15 17:36:40.895226 jaeger-1.3.3/python/jaeger/actor/commands/__init__.py
--rw-r--r--   0        0        0     1029 2023-01-15 17:36:40.895400 jaeger-1.3.3/python/jaeger/actor/commands/alerts.py
--rw-r--r--   0        0        0     1182 2023-01-15 17:36:40.895588 jaeger-1.3.3/python/jaeger/actor/commands/can.py
--rw-r--r--   0        0        0     3381 2023-01-15 17:36:40.895861 jaeger-1.3.3/python/jaeger/actor/commands/chiller.py
--rw-r--r--   0        0        0    32413 2023-01-15 17:36:40.896298 jaeger-1.3.3/python/jaeger/actor/commands/configuration.py
--rw-r--r--   0        0        0      721 2023-01-15 17:36:40.896524 jaeger-1.3.3/python/jaeger/actor/commands/debug.py
--rw-r--r--   0        0        0     2691 2023-01-15 17:36:40.896739 jaeger-1.3.3/python/jaeger/actor/commands/disable.py
--rw-r--r--   0        0        0    14511 2023-01-15 17:36:40.896971 jaeger-1.3.3/python/jaeger/actor/commands/fvc.py
--rw-r--r--   0        0        0    11354 2023-01-15 17:36:40.897182 jaeger-1.3.3/python/jaeger/actor/commands/home.py
--rw-r--r--   0        0        0     5315 2023-01-15 17:36:40.897362 jaeger-1.3.3/python/jaeger/actor/commands/ieb.py
--rw-r--r--   0        0        0     1410 2023-01-15 17:36:40.897609 jaeger-1.3.3/python/jaeger/actor/commands/pollers.py
--rw-r--r--   0        0        0    16072 2023-01-15 17:36:40.898132 jaeger-1.3.3/python/jaeger/actor/commands/positioner.py
--rw-r--r--   0        0        0     9996 2023-01-15 17:36:40.898491 jaeger-1.3.3/python/jaeger/actor/commands/power.py
--rw-r--r--   0        0        0      990 2023-01-15 17:36:40.898804 jaeger-1.3.3/python/jaeger/actor/commands/snapshot.py
--rw-r--r--   0        0        0     1323 2023-01-15 17:36:40.899110 jaeger-1.3.3/python/jaeger/actor/commands/talk.py
--rw-r--r--   0        0        0     1034 2023-01-15 17:36:40.899526 jaeger-1.3.3/python/jaeger/actor/commands/testing.py
--rw-r--r--   0        0        0     3579 2023-01-15 17:36:40.899891 jaeger-1.3.3/python/jaeger/actor/commands/unwind.py
--rw-r--r--   0        0        0      949 2023-01-15 17:36:40.900201 jaeger-1.3.3/python/jaeger/actor/commands/version.py
--rw-r--r--   0        0        0    14067 2023-01-15 17:36:40.900534 jaeger-1.3.3/python/jaeger/alerts.py
--rw-r--r--   0        0        0    21716 2023-01-15 17:36:40.900929 jaeger-1.3.3/python/jaeger/can.py
--rw-r--r--   0        0        0     5222 2023-01-15 17:36:40.901388 jaeger-1.3.3/python/jaeger/chiller.py
--rw-r--r--   0        0        0     3965 2023-01-15 17:36:40.901736 jaeger-1.3.3/python/jaeger/commands/__init__.py
--rw-r--r--   0        0        0    22140 2023-01-15 17:36:40.902083 jaeger-1.3.3/python/jaeger/commands/base.py
--rw-r--r--   0        0        0     9016 2023-01-15 17:36:40.902369 jaeger-1.3.3/python/jaeger/commands/bootloader.py
--rw-r--r--   0        0        0    12187 2023-01-15 17:36:40.902804 jaeger-1.3.3/python/jaeger/commands/calibration.py
--rw-r--r--   0        0        0    10794 2023-01-15 17:36:40.903049 jaeger-1.3.3/python/jaeger/commands/goto.py
--rw-r--r--   0        0        0     6016 2023-01-15 17:36:40.903265 jaeger-1.3.3/python/jaeger/commands/status.py
--rw-r--r--   0        0        0    26700 2023-01-15 17:36:40.903576 jaeger-1.3.3/python/jaeger/commands/trajectory.py
--rw-r--r--   0        0        0    10030 2023-01-15 17:36:40.903927 jaeger-1.3.3/python/jaeger/etc/chiller_APO.yaml
--rw-r--r--   0        0        0     7487 2023-01-15 17:36:40.904273 jaeger-1.3.3/python/jaeger/etc/chiller_APO_variables.csv
--rw-r--r--   0        0        0     1317 2023-01-15 17:36:40.904498 jaeger-1.3.3/python/jaeger/etc/fvc.yaml
--rw-r--r--   0        0        0    10541 2023-01-15 17:36:40.904725 jaeger-1.3.3/python/jaeger/etc/ieb_APO.yaml
--rw-r--r--   0        0        0    10539 2023-01-15 17:36:40.904938 jaeger-1.3.3/python/jaeger/etc/ieb_LCO.yaml
--rw-r--r--   0        0        0     3256 2023-01-15 17:36:40.905134 jaeger-1.3.3/python/jaeger/etc/jaeger_APO.yml
--rw-r--r--   0        0        0     3188 2023-01-15 17:36:40.905351 jaeger-1.3.3/python/jaeger/etc/jaeger_LCO.yml
--rw-r--r--   0        0        0     8628 2023-01-15 17:36:40.905528 jaeger-1.3.3/python/jaeger/etc/schema.json
--rw-r--r--   0        0        0     1815 2023-01-15 17:36:40.905835 jaeger-1.3.3/python/jaeger/etc/sextants/epfl.yaml
--rw-r--r--   0        0        0     2367 2023-01-15 17:36:40.905999 jaeger-1.3.3/python/jaeger/etc/sextants/osu.yaml
--rw-r--r--   0        0        0     1512 2023-01-15 17:36:40.906150 jaeger-1.3.3/python/jaeger/etc/sextants/schema.json
--rw-r--r--   0        0        0     2364 2023-01-15 17:36:40.906884 jaeger-1.3.3/python/jaeger/etc/sextants/uw.yaml
--rw-r--r--   0        0        0     3548 2023-01-15 17:36:40.907421 jaeger-1.3.3/python/jaeger/exceptions.py
--rw-r--r--   0        0        0    51463 2023-01-15 17:36:40.908085 jaeger-1.3.3/python/jaeger/fps.py
--rw-r--r--   0        0        0    39278 2023-01-15 17:36:40.908506 jaeger-1.3.3/python/jaeger/fvc.py
--rw-r--r--   0        0        0     4513 2023-01-15 17:36:40.908756 jaeger-1.3.3/python/jaeger/ieb.py
--rw-r--r--   0        0        0      162 2023-01-15 17:36:40.909046 jaeger-1.3.3/python/jaeger/interfaces/__init__.py
--rw-r--r--   0        0        0     1142 2023-01-15 17:36:40.909419 jaeger-1.3.3/python/jaeger/interfaces/bus.py
--rw-r--r--   0        0        0     6766 2023-01-15 17:36:40.909742 jaeger-1.3.3/python/jaeger/interfaces/cannet.py
--rw-r--r--   0        0        0    12893 2023-01-15 17:36:40.910076 jaeger-1.3.3/python/jaeger/interfaces/message.py
--rw-r--r--   0        0        0     1875 2023-01-15 17:36:40.910408 jaeger-1.3.3/python/jaeger/interfaces/notifier.py
--rw-r--r--   0        0        0     1200 2023-01-15 17:36:40.910714 jaeger-1.3.3/python/jaeger/interfaces/virtual.py
--rw-r--r--   0        0        0    19795 2023-01-15 17:36:40.911075 jaeger-1.3.3/python/jaeger/kaiju.py
--rw-r--r--   0        0        0     8034 2023-01-15 17:36:40.911424 jaeger-1.3.3/python/jaeger/maskbits.py
--rw-r--r--   0        0        0     7302 2023-01-15 17:36:40.911759 jaeger-1.3.3/python/jaeger/plotting.py
--rw-r--r--   0        0        0    18127 2023-01-15 17:36:40.912274 jaeger-1.3.3/python/jaeger/positioner.py
--rw-r--r--   0        0        0        0 2023-01-15 17:36:40.912606 jaeger-1.3.3/python/jaeger/scripts/__init__.py
--rw-r--r--   0        0        0     1825 2023-01-15 17:36:40.912783 jaeger-1.3.3/python/jaeger/scripts/generate_chiller_yaml.py
--rwxr-xr-x   0        0        0    19978 2023-01-15 17:36:40.913173 jaeger-1.3.3/python/jaeger/scripts/robotcalib.py
--rw-r--r--   0        0        0      293 2023-01-15 17:36:40.913704 jaeger-1.3.3/python/jaeger/target/__init__.py
--rw-r--r--   0        0        0    62381 2023-01-15 17:36:40.914183 jaeger-1.3.3/python/jaeger/target/configuration.py
--rw-r--r--   0        0        0     8119 2023-01-15 17:36:40.914664 jaeger-1.3.3/python/jaeger/target/design.py
--rw-r--r--   0        0        0    11809 2023-01-15 17:36:40.914925 jaeger-1.3.3/python/jaeger/target/tools.py
--rw-r--r--   0        0        0    12409 2023-01-15 17:36:40.915244 jaeger-1.3.3/python/jaeger/testing.py
--rw-r--r--   0        0        0       60 2023-01-15 17:36:40.915499 jaeger-1.3.3/python/jaeger/utils/__init__.py
--rw-r--r--   0        0        0     9562 2023-01-15 17:36:40.915718 jaeger-1.3.3/python/jaeger/utils/database.py
--rw-r--r--   0        0        0    14771 2023-01-15 17:36:40.915927 jaeger-1.3.3/python/jaeger/utils/helpers.py
--rw-r--r--   0        0        0     9549 2023-01-15 17:36:40.916119 jaeger-1.3.3/python/jaeger/utils/utils.py
--rw-r--r--   0        0        0     3819 1970-01-01 00:00:00.000000 jaeger-1.3.3/setup.py
--rw-r--r--   0        0        0     3926 1970-01-01 00:00:00.000000 jaeger-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-04-13 00:20:40.277423 jaeger-1.3.4/LICENSE.md
+-rw-r--r--   0        0        0     2386 2023-04-13 00:20:40.277643 jaeger-1.3.4/README.md
+-rw-r--r--   0        0        0     3309 2023-04-13 00:20:40.285686 jaeger-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1745 2023-04-13 00:20:40.286122 jaeger-1.3.4/python/jaeger/__init__.py
+-rw-r--r--   0        0        0    20331 2023-04-13 00:20:40.286430 jaeger-1.3.4/python/jaeger/__main__.py
+-rw-r--r--   0        0        0       61 2023-04-13 00:20:40.286736 jaeger-1.3.4/python/jaeger/actor/__init__.py
+-rw-r--r--   0        0        0     5033 2023-04-13 00:20:40.286972 jaeger-1.3.4/python/jaeger/actor/actor.py
+-rw-r--r--   0        0        0      816 2023-04-13 00:20:40.287269 jaeger-1.3.4/python/jaeger/actor/commands/__init__.py
+-rw-r--r--   0        0        0     1029 2023-04-13 00:20:40.287485 jaeger-1.3.4/python/jaeger/actor/commands/alerts.py
+-rw-r--r--   0        0        0     1182 2023-04-13 00:20:40.287730 jaeger-1.3.4/python/jaeger/actor/commands/can.py
+-rw-r--r--   0        0        0     3381 2023-04-13 00:20:40.287971 jaeger-1.3.4/python/jaeger/actor/commands/chiller.py
+-rw-r--r--   0        0        0    33052 2023-04-13 00:20:40.288303 jaeger-1.3.4/python/jaeger/actor/commands/configuration.py
+-rw-r--r--   0        0        0      721 2023-04-13 00:20:40.288552 jaeger-1.3.4/python/jaeger/actor/commands/debug.py
+-rw-r--r--   0        0        0     2690 2023-04-13 00:20:40.288773 jaeger-1.3.4/python/jaeger/actor/commands/disable.py
+-rw-r--r--   0        0        0    14510 2023-04-13 00:20:40.289025 jaeger-1.3.4/python/jaeger/actor/commands/fvc.py
+-rw-r--r--   0        0        0    11347 2023-04-13 00:20:40.289269 jaeger-1.3.4/python/jaeger/actor/commands/home.py
+-rw-r--r--   0        0        0     5314 2023-04-13 00:20:40.289486 jaeger-1.3.4/python/jaeger/actor/commands/ieb.py
+-rw-r--r--   0        0        0     1410 2023-04-13 00:20:40.289680 jaeger-1.3.4/python/jaeger/actor/commands/pollers.py
+-rw-r--r--   0        0        0    16070 2023-04-13 00:20:40.289991 jaeger-1.3.4/python/jaeger/actor/commands/positioner.py
+-rw-r--r--   0        0        0     9994 2023-04-13 00:20:40.290231 jaeger-1.3.4/python/jaeger/actor/commands/power.py
+-rw-r--r--   0        0        0      990 2023-04-13 00:20:40.290434 jaeger-1.3.4/python/jaeger/actor/commands/snapshot.py
+-rw-r--r--   0        0        0     1323 2023-04-13 00:20:40.290639 jaeger-1.3.4/python/jaeger/actor/commands/talk.py
+-rw-r--r--   0        0        0     1034 2023-04-13 00:20:40.290963 jaeger-1.3.4/python/jaeger/actor/commands/testing.py
+-rw-r--r--   0        0        0     3579 2023-04-13 00:20:40.291184 jaeger-1.3.4/python/jaeger/actor/commands/unwind.py
+-rw-r--r--   0        0        0      949 2023-04-13 00:20:40.291388 jaeger-1.3.4/python/jaeger/actor/commands/version.py
+-rw-r--r--   0        0        0    14065 2023-04-13 00:20:40.291629 jaeger-1.3.4/python/jaeger/alerts.py
+-rw-r--r--   0        0        0    21709 2023-04-13 00:20:40.291936 jaeger-1.3.4/python/jaeger/can.py
+-rw-r--r--   0        0        0     5220 2023-04-13 00:20:40.292193 jaeger-1.3.4/python/jaeger/chiller.py
+-rw-r--r--   0        0        0     3964 2023-04-13 00:20:40.292482 jaeger-1.3.4/python/jaeger/commands/__init__.py
+-rw-r--r--   0        0        0    22135 2023-04-13 00:20:40.292772 jaeger-1.3.4/python/jaeger/commands/base.py
+-rw-r--r--   0        0        0     9010 2023-04-13 00:20:40.293027 jaeger-1.3.4/python/jaeger/commands/bootloader.py
+-rw-r--r--   0        0        0    12181 2023-04-13 00:20:40.293252 jaeger-1.3.4/python/jaeger/commands/calibration.py
+-rw-r--r--   0        0        0    10788 2023-04-13 00:20:40.293480 jaeger-1.3.4/python/jaeger/commands/goto.py
+-rw-r--r--   0        0        0     6013 2023-04-13 00:20:40.293687 jaeger-1.3.4/python/jaeger/commands/status.py
+-rw-r--r--   0        0        0    26689 2023-04-13 00:20:40.293995 jaeger-1.3.4/python/jaeger/commands/trajectory.py
+-rw-r--r--   0        0        0    10030 2023-04-13 00:20:40.294321 jaeger-1.3.4/python/jaeger/etc/chiller_APO.yaml
+-rw-r--r--   0        0        0     7487 2023-04-13 00:20:40.294546 jaeger-1.3.4/python/jaeger/etc/chiller_APO_variables.csv
+-rw-r--r--   0        0        0     1317 2023-04-13 00:20:40.294767 jaeger-1.3.4/python/jaeger/etc/fvc.yaml
+-rw-r--r--   0        0        0    10541 2023-04-13 00:20:40.294986 jaeger-1.3.4/python/jaeger/etc/ieb_APO.yaml
+-rw-r--r--   0        0        0    10539 2023-04-13 00:20:40.295210 jaeger-1.3.4/python/jaeger/etc/ieb_LCO.yaml
+-rw-r--r--   0        0        0     3256 2023-04-13 00:20:40.295426 jaeger-1.3.4/python/jaeger/etc/jaeger_APO.yml
+-rw-r--r--   0        0        0     3188 2023-04-13 00:20:40.295631 jaeger-1.3.4/python/jaeger/etc/jaeger_LCO.yml
+-rw-r--r--   0        0        0     8711 2023-04-13 00:20:40.295846 jaeger-1.3.4/python/jaeger/etc/schema.json
+-rw-r--r--   0        0        0     1815 2023-04-13 00:20:40.296116 jaeger-1.3.4/python/jaeger/etc/sextants/epfl.yaml
+-rw-r--r--   0        0        0     2367 2023-04-13 00:20:40.296297 jaeger-1.3.4/python/jaeger/etc/sextants/osu.yaml
+-rw-r--r--   0        0        0     1512 2023-04-13 00:20:40.296535 jaeger-1.3.4/python/jaeger/etc/sextants/schema.json
+-rw-r--r--   0        0        0     2364 2023-04-13 00:20:40.296761 jaeger-1.3.4/python/jaeger/etc/sextants/uw.yaml
+-rw-r--r--   0        0        0     3545 2023-04-13 00:20:40.296967 jaeger-1.3.4/python/jaeger/exceptions.py
+-rw-r--r--   0        0        0    51683 2023-04-13 00:20:40.297390 jaeger-1.3.4/python/jaeger/fps.py
+-rw-r--r--   0        0        0    39277 2023-04-13 00:20:40.297790 jaeger-1.3.4/python/jaeger/fvc.py
+-rw-r--r--   0        0        0     4510 2023-04-13 00:20:40.301959 jaeger-1.3.4/python/jaeger/ieb.py
+-rw-r--r--   0        0        0      162 2023-04-13 00:20:40.302244 jaeger-1.3.4/python/jaeger/interfaces/__init__.py
+-rw-r--r--   0        0        0     1142 2023-04-13 00:20:40.302443 jaeger-1.3.4/python/jaeger/interfaces/bus.py
+-rw-r--r--   0        0        0     6759 2023-04-13 00:20:40.302734 jaeger-1.3.4/python/jaeger/interfaces/cannet.py
+-rw-r--r--   0        0        0    12892 2023-04-13 00:20:40.302984 jaeger-1.3.4/python/jaeger/interfaces/message.py
+-rw-r--r--   0        0        0     1874 2023-04-13 00:20:40.303204 jaeger-1.3.4/python/jaeger/interfaces/notifier.py
+-rw-r--r--   0        0        0     1199 2023-04-13 00:20:40.303397 jaeger-1.3.4/python/jaeger/interfaces/virtual.py
+-rw-r--r--   0        0        0    19795 2023-04-13 00:20:40.303664 jaeger-1.3.4/python/jaeger/kaiju.py
+-rw-r--r--   0        0        0     8034 2023-04-13 00:20:40.303916 jaeger-1.3.4/python/jaeger/maskbits.py
+-rw-r--r--   0        0        0     7296 2023-04-13 00:20:40.304126 jaeger-1.3.4/python/jaeger/plotting.py
+-rw-r--r--   0        0        0    18121 2023-04-13 00:20:40.304401 jaeger-1.3.4/python/jaeger/positioner.py
+-rw-r--r--   0        0        0        0 2023-04-13 00:20:40.304684 jaeger-1.3.4/python/jaeger/scripts/__init__.py
+-rw-r--r--   0        0        0     1825 2023-04-13 00:20:40.304899 jaeger-1.3.4/python/jaeger/scripts/generate_chiller_yaml.py
+-rwxr-xr-x   0        0        0    19977 2023-04-13 00:20:40.305203 jaeger-1.3.4/python/jaeger/scripts/robotcalib.py
+-rw-r--r--   0        0        0      293 2023-04-13 00:20:40.305615 jaeger-1.3.4/python/jaeger/target/__init__.py
+-rw-r--r--   0        0        0    62360 2023-04-13 00:20:40.306077 jaeger-1.3.4/python/jaeger/target/configuration.py
+-rw-r--r--   0        0        0     8410 2023-04-13 00:20:40.306357 jaeger-1.3.4/python/jaeger/target/design.py
+-rw-r--r--   0        0        0    11807 2023-04-13 00:20:40.306683 jaeger-1.3.4/python/jaeger/target/tools.py
+-rw-r--r--   0        0        0    12403 2023-04-13 00:20:40.306916 jaeger-1.3.4/python/jaeger/testing.py
+-rw-r--r--   0        0        0       60 2023-04-13 00:20:40.307196 jaeger-1.3.4/python/jaeger/utils/__init__.py
+-rw-r--r--   0        0        0     9562 2023-04-13 00:20:40.307427 jaeger-1.3.4/python/jaeger/utils/database.py
+-rw-r--r--   0        0        0    14766 2023-04-13 00:20:40.307671 jaeger-1.3.4/python/jaeger/utils/helpers.py
+-rw-r--r--   0        0        0     9549 2023-04-13 00:20:40.307900 jaeger-1.3.4/python/jaeger/utils/utils.py
+-rw-r--r--   0        0        0     3926 1970-01-01 00:00:00.000000 jaeger-1.3.4/PKG-INFO
```

### Comparing `jaeger-1.3.3/LICENSE.md` & `jaeger-1.3.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.3/README.md` & `jaeger-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.3/pyproject.toml` & `jaeger-1.3.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jaeger"
-version = "1.3.3"
+version = "1.3.4"
 description = "Controllers for the SDSS-V FPS"
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/jaeger"
 repository = "https://github.com/sdss/jaeger"
 documentation = "https://sdss-jaeger.readthedocs.io/en/latest/"
```

### Comparing `jaeger-1.3.3/python/jaeger/__init__.py` & `jaeger-1.3.4/python/jaeger/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,14 @@
     )
 
 
 warnings.simplefilter("always", category=JaegerUserWarning)
 
 
 def start_file_loggers(start_log=True, start_can=True):
-
     if "files" in config and "log_dir" in config["files"]:
         log_dir = config["files"]["log_dir"]
     else:
         log_dir = "~/.jaeger"
 
     if start_log and log.fh is None:
         log.start_file_logger(os.path.join(log_dir, "jaeger.log"))
```

### Comparing `jaeger-1.3.3/python/jaeger/__main__.py` & `jaeger-1.3.4/python/jaeger/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,14 @@
         profile,
         ieb=None,
         initialise=True,
         npositioners=10,
         enable_low_temperature=True,
         skip_fibre_assignments_check=False,
     ):
-
         self.profile = profile
         if self.profile in ["test", "virtual"]:
             self.profile = "virtual"
 
         self.ieb = ieb
         self.enable_low_temperature = enable_low_temperature
         self.skip_fibre_assignments_check = skip_fibre_assignments_check
@@ -93,15 +92,14 @@
 
         self.vpositioners = []
         self.npositioners = npositioners
 
         self.fps = None
 
     async def __aenter__(self):
-
         global __FPS__
 
         # If profile is test we start a VirtualFPS first so that it can respond
         # to the FPS class.
         if self.profile == "virtual":
             self.fps = VirtualFPS()
             for pid in range(self.npositioners):
@@ -400,15 +398,14 @@
         click.confirm(
             f"Upgrade firmware for sextant(s) {', '.join(map(str, sextants))}?",
             default=False,
             abort=True,
         )
 
     async with fps_maker as fps:
-
         ps_devs = []
         if fps.ieb and no_cycle is False:
             for module in fps.ieb.modules.values():
                 for dev_name in module.devices:
                     if dev_name.upper().startswith("PS"):
                         ps_devs.append(dev_name)
 
@@ -540,15 +537,14 @@
     relative: bool = False,
     use_sync: bool = True,
     go_cowboy: bool = False,
 ):
     """Sends positioners to a given (alpha, beta) position."""
 
     with fps_maker as fps:
-
         if all:
             if not force:
                 raise JaegerError("Use --force to move all positioners at once.")
             positioner_ids = list(fps.positioners.keys())
         else:
             positioner_ids = list(positioner_ids)
 
@@ -585,15 +581,14 @@
     if alpha < 0 or alpha >= 360:
         raise click.UsageError("alpha must be in the range [0, 360)")
 
     if beta < 0 or beta >= 360:
         raise click.UsageError("beta must be in the range [0, 360)")
 
     async with fps_maker as fps:
-
         positioner = fps.positioners[positioner_id]
 
         result = await positioner.set_position(alpha, beta)
 
         if not result:
             log.error("failed to set positions.")
             return
@@ -613,15 +608,14 @@
 async def home(fps_maker: FPSWrapper, positioner_id: int, axis: str | None = None):
     """Home a single positioner, sending a GO_TO_DATUMS command."""
 
     alpha: bool = axis == "alpha" or axis is None
     beta: bool = axis == "beta" or axis is None
 
     async with fps_maker as fps:
-
         if positioner_id not in fps or fps[positioner_id].initialised is False:
             raise ValueError("Positioner is not connected.")
         if fps[positioner_id].disabled or fps[positioner_id].offline:
             raise ValueError("Positioner has been disabled.")
 
         await fps[positioner_id].home(alpha=alpha, beta=beta)
 
@@ -634,15 +628,14 @@
 @cli_coro
 async def status(fps_maker: FPSWrapper, positioner_id: int):
     """Returns the status of a positioner with low-level initialisation."""
 
     fps_maker.initialise = False
 
     async with fps_maker as fps:
-
         pos = Positioner(positioner_id, fps)
 
         try:
             await pos.update_firmware_version()
             print(f"Firmware: {pos.firmware}")
             print(f"Bootloader: {pos.is_bootloader()}")
         except Exception as err:
@@ -677,15 +670,14 @@
 @cli_coro
 async def unwind(fps_maker, collision_buffer: float | None = None, force: bool = False):
     """Unwinds the array."""
 
     from jaeger.kaiju import unwind
 
     async with fps_maker as fps:
-
         if fps.locked:
             FPSLockedError("The FPS is locked.")
 
         await fps.update_position()
         positions = {p.positioner_id: (p.alpha, p.beta) for p in fps.values()}
 
         log.info("Calculating trajectory.")
@@ -713,15 +705,14 @@
     one: int | None = None,
 ):
     """Explodes the array."""
 
     from jaeger.kaiju import explode
 
     async with fps_maker as fps:
-
         if fps.locked:
             FPSLockedError("The FPS is locked.")
 
         await fps.update_position()
         positions = {p.positioner_id: (p.alpha, p.beta) for p in fps.values()}
 
         log.info("Calculating trajectory.")
@@ -750,15 +741,14 @@
 ):
     """Takes a snapshot image."""
 
     if path is not None:
         path = str(path)
 
     async with fps_maker as fps:
-
         await fps.update_position()
         filename = await fps.save_snapshot(path, collision_buffer=collision_buffer)
 
     print(f"Snapshot saved to {filename}")
 
 
 @jaeger.command()
```

### Comparing `jaeger-1.3.3/python/jaeger/actor/actor.py` & `jaeger-1.3.4/python/jaeger/actor/actor.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,14 @@
             return tmpfile.name
 
 
 class JaegerActor(clu.LegacyActor):
     """The jaeger SDSS-style actor."""
 
     def __init__(self, fps: FPS, *args, observatory: str | None = None, **kwargs):
-
         jaeger.actor_instance = self
 
         self.fps = fps
 
         # This is mostly for the miniwoks. If the schema file is not the base
         # one, merge them.
         base = os.path.join(os.path.dirname(__file__), "..")
```

### Comparing `jaeger-1.3.3/python/jaeger/actor/commands/__init__.py` & `jaeger-1.3.4/python/jaeger/actor/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.3/python/jaeger/actor/commands/alerts.py` & `jaeger-1.3.4/python/jaeger/actor/commands/alerts.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.3/python/jaeger/actor/commands/can.py` & `jaeger-1.3.4/python/jaeger/actor/commands/can.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.3/python/jaeger/actor/commands/chiller.py` & `jaeger-1.3.4/python/jaeger/actor/commands/chiller.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.3/python/jaeger/actor/commands/configuration.py` & `jaeger-1.3.4/python/jaeger/actor/commands/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from typing import TYPE_CHECKING
 
 import click
 import numpy
 import peewee
 from astropy.time import Time
 
+from clu.parsers.click import timeout
 from sdssdb.peewee.sdss5db import opsdb
 
 from jaeger import config
 from jaeger.exceptions import JaegerError, TrajectoryError
 from jaeger.ieb import IEB
 from jaeger.kaiju import check_trajectory
 from jaeger.kaiju import explode as kaiju_explode
@@ -55,14 +56,15 @@
     scale: float | None = None,
     fudge_factor: float | None = None,
     epoch: float | None = None,
     epoch_delay: float = 0.0,
     get_paths: bool = True,
     path_generation_mode: str | None = None,
     safety_factor: float = 0.1,
+    offset_min_skybrightness: float = 0.5,
 ):
     """Helper to load or preload a design."""
 
     if design_id is None:
         design_id, _epoch_delay = get_designid_from_queue(
             pop=not preload,
             epoch_delay=True,
@@ -108,15 +110,14 @@
         configuration = await fps.configuration.clone(
             design_id=design_id,
             write_summary=False,
             write_to_database=False,
         )
 
     else:
-
         default_scale = config["configuration"].get("default_focal_scale", 1.0)
         use_guider_scale = config["configuration"].get("use_guider_scale", True)
 
         clip_scale: float = config["configuration"]["clip_scale"]
         SCALE_FUDGE: float = config["configuration"]["scale_fudge_factor"]
         fudge_factor = fudge_factor or SCALE_FUDGE
 
@@ -198,14 +199,15 @@
             epoch += epoch_delay / 86400.0
 
             design = await Design.create_async(
                 design_id,
                 epoch=epoch,
                 scale=scale,
                 safety_factor=safety_factor,
+                offset_min_skybrightness=offset_min_skybrightness,
             )
         except Exception as err:
             command.error(error=f"Failed retrieving design: {err}")
             return False
 
         configuration = design.configuration
 
@@ -308,14 +310,20 @@
 )
 @click.option(
     "--safety-factor",
     type=float,
     default=0.1,
     help="Safety factor to pass to the offset calculation function.",
 )
+@click.option(
+    "--offset-min-skybrightness",
+    type=float,
+    default=0.5,
+    help="Minimum sky brightness for the offset.",
+)
 @click.argument("DESIGNID", type=int, required=False)
 async def load(
     command: Command[JaegerActor],
     fps: FPS,
     designid: int | None = None,
     reload: bool = False,
     replace: bool = False,
@@ -329,14 +337,15 @@
     execute: bool = False,
     reissue: bool = False,
     scale: float | None = None,
     fudge_factor: float | None = None,
     no_clone: bool = False,
     path_generation_mode: str | None = None,
     safety_factor: float = 0.1,
+    offset_min_skybrightness: float = 0.5,
 ):
     """Creates and ingests a configuration from a design in the database."""
 
     assert command.actor is not None
 
     if reissue is True:
         if fps.configuration is None or fps.configuration.design is None:
@@ -373,14 +382,15 @@
             no_clone=no_clone,
             scale=scale,
             epoch=epoch,
             epoch_delay=epoch_delay,
             get_paths=False,
             path_generation_mode=path_generation_mode,
             safety_factor=safety_factor,
+            offset_min_skybrightness=offset_min_skybrightness,
         )
 
         if configuration is False:
             # _load_design already issues an error so we just fail.
             return command.fail()
         else:
             fps.configuration = configuration
@@ -573,27 +583,35 @@
 )
 @click.option(
     "--safety-factor",
     type=float,
     default=0.1,
     help="Safety factor to pass to the offset calculation function.",
 )
+@click.option(
+    "--offset-min-skybrightness",
+    type=float,
+    default=0.5,
+    help="Minimum sky brightness for the offset.",
+)
 @click.argument("DESIGNID", type=int, required=False)
+@timeout(180)
 async def preload(
     command: JaegerCommandType,
     fps: FPS,
     designid: int | None = None,
     epoch: float | None = None,
     epoch_delay: float = 0.0,
     scale: float | None = None,
     fudge_factor: float | None = None,
     no_clone: bool = False,
     make_active: bool = True,
     clear: bool = False,
     safety_factor: float = 0.1,
+    offset_min_skybrightness: float = 0.5,
 ):
     """Preloads a design.
 
     Preloading a design works similar to loading it, but no files are generated, no
     database entry is created, no configuration_loaded keyword is output, and the
     new configuration is stored separately. To make the preloaded configuration
     active either pass the --make-active flag or run
@@ -612,14 +630,15 @@
         preload=True,
         no_clone=no_clone,
         scale=scale,
         fudge_factor=fudge_factor,
         epoch=epoch,
         epoch_delay=epoch_delay,
         safety_factor=safety_factor,
+        offset_min_skybrightness=offset_min_skybrightness,
     )
 
     if configuration is False:
         # _load_design already issues an error so we just fail.
         return command.fail()
     elif configuration.design_id is None:
         return command.fail(
```

### Comparing `jaeger-1.3.3/python/jaeger/actor/commands/debug.py` & `jaeger-1.3.4/python/jaeger/actor/commands/debug.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.3/python/jaeger/actor/commands/disable.py` & `jaeger-1.3.4/python/jaeger/actor/commands/disable.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     """Disables a positioner"""
 
     permanently_disabled = config["fps"]["disabled_positioners"]
     if config["fps"]["offline_positioners"] is not None:
         permanently_disabled += list(config["fps"]["offline_positioners"].keys())
 
     if positioner_id:
-
         if positioner_id not in fps:
             return command.fail(f"Positioner {positioner_id} is not in the array.")
 
         positioner = fps.positioners[positioner_id]
 
         if positioner.disabled:
             command.warning(f"Positioner {positioner_id} is already disabled.")
```

### Comparing `jaeger-1.3.3/python/jaeger/actor/commands/fvc.py` & `jaeger-1.3.4/python/jaeger/actor/commands/fvc.py`

 * *Files 0% similar despite different names*

```diff
@@ -380,15 +380,14 @@
     proc_image_saved = False
 
     # Flag to determine when to exit the loop.
     reached: bool = False
     failed: bool = False
 
     try:
-
         n = 1
         while True:
             command.info(f"FVC iteration {n}")
 
             filename = None
             proc_image_saved: bool = False
```

### Comparing `jaeger-1.3.3/python/jaeger/actor/commands/home.py` & `jaeger-1.3.4/python/jaeger/actor/commands/home.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,14 @@
         for positioner_id in positioner_ids:
             if positioner_id not in fps.positioners.keys():
                 return command.fail(f"Unknown positioner {positioner_id}.")
             if fps[positioner_id].disabled or fps[positioner_id].offline:
                 return command.fail(f"Cannot home disabled positioner {positioner_id}.")
 
     if axis == "alpha":
-
         result = await check_positions(
             fps,
             beta_min=SAFE_BETA_MIN,
             beta_max=SAFE_BETA_MAX,
             check_disabled=True,
         )
         if not result:
@@ -136,15 +135,14 @@
                 },
                 go_cowboy=True,
             )
         except TrajectoryError as err:
             return command.fail(f"Trajectory failed with error {err}.")
 
     elif axis == "beta":
-
         if not (await fps.is_folded()):
             return command.fail("The FPS is not folded. Cannot home beta.")
 
         command.info("Creating paths for phase 1.")
 
         grid1 = get_robot_grid(fps, collision_buffer=COLLISION_BUFFER)
         for robot in grid1.robotDict.values():
@@ -183,15 +181,14 @@
         if failed:
             return command.fail("Failed generating paths for beta homing phase 2.")
 
         if skip_phase_1:
             phase_1_home_pids = []
 
         if len(phase_1_home_pids) > 0:
-
             _, from_destination_1, failed, _ = get_path_pair(
                 grid1,
                 path_generation_mode="greedy",
             )
             if failed:
                 return command.fail("Failed generating paths for beta homing phase 1.")
 
@@ -205,22 +202,20 @@
                     from_destination_1,
                     dry_run=dry_run,
                 )
             except JaegerError as err:
                 return command.fail(f"Phase 1 homing failed with error: {err}")
 
         else:
-
             command.info("No selected positioners in phase 1. Skipping ")
 
         # Robots in phase 2 that will be homed.
         phase_2_home_pids = list(set(positioner_ids) & set(phase_2_pids))
 
         if len(phase_2_home_pids) > 0:
-
             try:
                 await _home_beta_phase(
                     command,
                     fps,
                     phase_2_home_pids,
                     2,
                     start_angle,
@@ -228,15 +223,14 @@
                     dry_run=dry_run,
                     extra_zero_positioner_ids=phase_1_home_pids,
                 )
             except JaegerError as err:
                 return command.fail(f"Phase 2 homing failed with error: {err}")
 
         else:
-
             command.info("No selected positioners in phase 2. Skipping ")
 
     return command.finish("Homing complete.")
 
 
 async def check_positions(
     fps: FPS,
@@ -270,15 +264,14 @@
     home_positioner_ids: list[int],
     phase: int,
     start_angle: float,
     from_destination: dict,
     dry_run: bool = False,
     extra_zero_positioner_ids: list[int] = [],
 ):
-
     command.info(f"Moving robots to phase {phase} initial position.")
     try:
         await fps.send_trajectory(from_destination, command=command)
     except TrajectoryError as err:
         raise JaegerError(f"Trajectory failed with error: {err}")
 
     command.info(f"Starting phase {phase} calibration.")
```

### Comparing `jaeger-1.3.3/python/jaeger/actor/commands/ieb.py` & `jaeger-1.3.4/python/jaeger/actor/commands/ieb.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,14 @@
                     command.info(text=f"        channel: {dev.channel}")
                 if dev.__type__:
                     command.info(text=f"        type: {dev.__type__}")
                     if dev.__type__ == "relay" and dev.relay_type:
                         command.info(text=f"        relay type: {dev.relay_type}")
 
     if len(categories) > 0 and command.actor and command.actor.model:
-
         command.info(text="")
         command.info(text="Keywords:")
 
         for category in sorted(categories):
             cat_data = command.actor.model.schema["properties"][category]
             items = [item["title"] for item in cat_data["items"]]
             command.info(text=f"  {category}=[{', '.join(items)}]")
```

### Comparing `jaeger-1.3.3/python/jaeger/actor/commands/pollers.py` & `jaeger-1.3.4/python/jaeger/actor/commands/pollers.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.3/python/jaeger/actor/commands/positioner.py` & `jaeger-1.3.4/python/jaeger/actor/commands/positioner.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,14 @@
             new_positions = {}
             for positioner_id in trajectory:
                 alpha = trajectory[positioner_id]["alpha"][-1][0]
                 beta = trajectory[positioner_id]["beta"][-1][0]
                 new_positions[int(positioner_id)] = (alpha, beta)
 
     else:
-
         assert alpha is not None and beta is not None
 
         if all:
             if not force:
                 return command.fail("Use --force to move all positioners at once.")
             positioner_ids = list(fps.positioners.keys())
         else:
@@ -411,15 +410,14 @@
         )
 
     path = pathlib.Path(path).expanduser()
     if not path.exists():
         raise click.BadParameter(f"path {path!s} does not exist.")
 
     try:
-
         trajectory = Trajectory(fps, path)
 
         command.debug(text="sending trajectory ...")
         await trajectory.send()
         if trajectory.failed:
             return command.fail(error="failed sending trajectory with unknown error.")
```

### Comparing `jaeger-1.3.3/python/jaeger/actor/commands/power.py` & `jaeger-1.3.4/python/jaeger/actor/commands/power.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,14 @@
     ieb = fps.ieb
     assert isinstance(ieb, IEB)
 
     if len(devices) == 0:
         return command.fail(error="No devices specified.")
 
     for idev, device in enumerate(devices):
-
         if device.upper() in config["ieb"]["disabled_devices"] and on is True:
             if force is False:
                 command.warning(text=f"{device} is disabled. Skipping.")
                 continue
             else:
                 command.warning(text=f"{device} is disabled but overriding.")
 
@@ -144,15 +143,14 @@
         return False
 
     command.debug(power_sync=[False])
 
     disabled = config["ieb"]["disabled_devices"]
 
     for devname in seq:
-
         do_delay = False
         if isinstance(devname, str):
             if devname.upper() in config["ieb"]["disabled_devices"]:
                 command.warning(text=f"{devname} is disabled. Skipping.")
                 continue
 
             dev = ieb.get_device(devname)
```

### Comparing `jaeger-1.3.3/python/jaeger/actor/commands/snapshot.py` & `jaeger-1.3.4/python/jaeger/actor/commands/snapshot.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.3/python/jaeger/actor/commands/talk.py` & `jaeger-1.3.4/python/jaeger/actor/commands/talk.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.3/python/jaeger/actor/commands/testing.py` & `jaeger-1.3.4/python/jaeger/actor/commands/testing.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.3/python/jaeger/actor/commands/unwind.py` & `jaeger-1.3.4/python/jaeger/actor/commands/unwind.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.3/python/jaeger/actor/commands/version.py` & `jaeger-1.3.4/python/jaeger/actor/commands/version.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.3/python/jaeger/alerts.py` & `jaeger-1.3.4/python/jaeger/alerts.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 __all__ = ["AlertsBot"]
 
 
 class AlertsBot(BaseBot):
     """Monitors values and raises alerts."""
 
     def __init__(self, fps: FPS):
-
         super().__init__(fps)
 
         self.config: dict[str, Any] = config["alerts"]
         self.interval: float = self.config["interval"]
 
         self.keywords: dict[str, bool] = {}
         self._gfa_alerts: dict[str, bool] = {}
@@ -132,15 +131,14 @@
             coros.append(self._check_flow)
         if "temperature" in self.config["enabled"]:
             coros.append(self._check_outside_temperature)
         if "chiller" in self.config["enabled"]:
             coros.append(self._check_chiller)
 
         while True:
-
             for coro in coros:
                 try:
                     await coro()
                 except Exception as err:
                     self.notify(
                         f"Failed running alerts coroutine {coro.__name__}: {err}"
                     )
```

### Comparing `jaeger-1.3.3/python/jaeger/can.py` & `jaeger-1.3.4/python/jaeger/can.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,14 @@
 
     interface_type: str
     channels: list | tuple
     fps: Optional[jaeger.fps.FPS] = None
     interface_args: Dict[str, Any] = field(default_factory=dict)
 
     def __post_init__(self):
-
         if self.interface_type not in INTERFACES:
             raise ValueError(f"Invalid interface {self.interface_type}.")
 
         # Start can file logger
         if config["debug"] is True:
             start_file_loggers(start_log=False, start_can=True)
 
@@ -121,15 +120,14 @@
 
         self.command_queue: asyncio.Queue[Command] | None = None
         self._command_queue_task: asyncio.Task | None = None
 
         self.notifier: Notifier | None = None
 
     async def start(self: T) -> T:
-
         self.stop()
 
         itype = self.interface_type
 
         InterfaceClass: Type[Bus_co] = INTERFACES[itype]["class"]
         self.multibus = INTERFACES[itype]["multibus"]
 
@@ -274,15 +272,14 @@
 
     async def _process_command_queue(self):
         """Processes messages in the command queue."""
 
         assert self.command_queue
 
         while True:
-
             cmd = await self.command_queue.get()
 
             log_header = LOG_HEADER.format(cmd=cmd)
 
             if cmd.status != CommandStatus.READY:
                 if cmd.status != CommandStatus.CANCELLED:
                     can_log.error(
@@ -307,15 +304,14 @@
 
     async def _process_reply_queue(self, msg: Message):
         """Processes one reply message."""
 
         positioner_id, command_id, reply_uid, __ = parse_identifier(msg.arbitration_id)
 
         if command_id == CommandID.COLLISION_DETECTED:
-
             # Sending stop trajectories causes many more robots to report a collision
             # so if the FPS has already been locked we ignore those.
             if not self.fps or self.fps.locked:
                 return
 
             log.error(
                 f"A collision was detected in positioner {positioner_id}. "
@@ -394,15 +390,14 @@
             f"to positioners {cmd.positioner_ids!r}."
         )
         can_log.debug(log_header + " sending messages to CAN bus.")
 
         messages = cmd.get_messages()
 
         for message in messages:
-
             if cmd.status.failed:
                 can_log.debug(
                     f"{log_header} not sending more messages "
                     "since this command has failed."
                 )
                 break
 
@@ -418,15 +413,14 @@
             is_multibus = self.multibus or len(self.interfaces) > 1
             if is_multibus and message.positioner_id != 0:
                 if self.fps and message.positioner_id in self.fps.positioner_to_bus:
                     interface, bus = self.fps.positioner_to_bus[message.positioner_id]
                     interfaces = [cast(Bus_co, interface)]
 
             for iface in interfaces:
-
                 iface_idx = self.interfaces.index(iface)
                 data_hex = binascii.hexlify(message.data).decode()
                 can_log.debug(
                     log_header + "sending message with "
                     f"arbitration_id={message.arbitration_id}, "
                     f"UID={message.uid}, "
                     f"and data={data_hex!r} to "
@@ -591,15 +585,14 @@
             device_status[interface_id]["name"] = device
 
         elif dev_version:
             version = dev_version.group("version")
             device_status[interface_id]["version"] = version
 
         elif dev_error:
-
             if "errors" not in device_status[interface_id]:
                 device_status[interface_id]["errors"] = []
 
             device_status[interface_id]["errors"].insert(
                 0,
                 {
                     "error_code": dev_error.group("error_code"),
```

### Comparing `jaeger-1.3.3/python/jaeger/chiller.py` & `jaeger-1.3.4/python/jaeger/chiller.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,29 +25,27 @@
 __all__ = ["ChillerBot"]
 
 
 class ChillerBot(BaseBot):
     """Manages the FPS chiller."""
 
     def __init__(self, fps: FPS):
-
         self.chiller_config = config.get("chiller", {})
         self.temperature: bool | float = self.chiller_config.get("temperature", False)
         self.flow: bool | float = self.chiller_config.get("flow", False)
 
         super().__init__(fps)
 
     async def _loop(self):
         """Sets the chiller set point temperature."""
 
         chiller = Chiller.create()
         assert chiller is not None
 
         while True:
-
             await self._set_temperature(chiller)
             await self._set_flow(chiller)
 
             await asyncio.sleep(60)
 
     async def _set_temperature(self, chiller: Chiller):
         """Sets the temperature set point."""
```

### Comparing `jaeger-1.3.3/python/jaeger/commands/__init__.py` & `jaeger-1.3.4/python/jaeger/commands/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from typing import Dict, Type, Union
 
 
 class TypesEnumMeta(enum.EnumMeta):
     """Metaclass to allow initialising an Enum from a string."""
 
     def __call__(cls: Type[enum.Enum], value: Union[str, int]):  # type: ignore
-
         if isinstance(value, str):
             for flag in cls:
                 if flag.name.lower() == value.lower():
                     return cls(flag.value)
 
         return super().__call__(value)
```

### Comparing `jaeger-1.3.3/python/jaeger/commands/base.py` & `jaeger-1.3.4/python/jaeger/commands/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,14 @@
         command: Command,
         data: bytearray = bytearray([]),
         positioner_id: int = 0,
         uid: int = 0,
         response_code: int = 0,
         extended_id: bool = True,
     ):
-
         self.command = command
         self.positioner_id = positioner_id
         self.uid = uid
 
         uid_bits = config["positioner"]["uid_bits"]
         max_uid = 2**uid_bits
         assert self.uid < max_uid, f"UID must be <= {max_uid}."
@@ -106,15 +105,14 @@
         The received message
     command
         The `.Command` to which this message is replying.
 
     """
 
     def __init__(self, message: Message, command: Optional[Command] = None):
-
         assert isinstance(message, Message), "invalid message"
 
         #: The command for which this reply is intended.
         self.command = command
 
         #: The raw ``Message``.
         self.message = message
@@ -234,15 +232,14 @@
         positioner_ids: int | List[int],
         timeout: Optional[float] = None,
         done_callback: Optional[Callable] = None,
         n_positioners: Optional[int] = None,
         data: Union[None, data_co, Dict[int, data_co]] = None,
         ignore_unknown: bool = True,
     ):
-
         global COMMAND_UID
 
         assert self.broadcastable is not None, "broadcastable not set"
         assert self.command_id is not None, "command_id not set"
 
         if isinstance(positioner_ids, (list, tuple)):
             self.positioner_ids = list(positioner_ids)
@@ -597,19 +594,17 @@
         """
 
         cid = self.command_id
 
         messages: List[SuperMessage] = []
 
         for pid in self.data:
-
             pid_data = self.data[pid]
 
             for d in pid_data:
-
                 try:
                     uid = UID_POOL[cid][pid].pop()
                 except KeyError:
                     # Before failing, put back the UIDs of the other messages
                     for message in messages:
                         UID_POOL[cid][pid].add(message.uid)
                     raise EmptyPool("no UIDs left in the pool.")
```

### Comparing `jaeger-1.3.3/python/jaeger/commands/bootloader.py` & `jaeger-1.3.4/python/jaeger/commands/bootloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,26 +109,24 @@
     filesize = os.path.getsize(firmware_file)
 
     # Check to make sure all positioners are in bootloader mode.
     valid_positioners = []
     n_bad = 0
 
     for positioner_id in fps.positioners:
-
         if positioners is not None and positioner_id not in positioners:
             continue
 
         positioner = fps.positioners[positioner_id]
 
         if (
             not positioner.is_bootloader()
             or BootloaderStatus.BOOTLOADER_INIT not in positioner.status
             or BootloaderStatus.UNKNOWN in positioner.status
         ):
-
             n_bad += 1
             continue
 
         valid_positioners.append(positioner)
 
     if len(valid_positioners) == 0:
         raise JaegerError(
@@ -174,15 +172,14 @@
     else:
         fh_handler = None
 
     chunk_size = 8
     n_chunks = int(numpy.ceil(filesize / chunk_size))
 
     with contextlib.ExitStack() as stack:
-
         if show_progressbar and progressbar:
             bar = stack.enter_context(progressbar.ProgressBar(max_value=n_chunks))
         else:
             bar = None
 
         messages_default = config["positioner"]["firmware_messages_per_positioner"]
         messages_per_positioner = messages_per_positioner or messages_default
@@ -238,15 +235,14 @@
     total_time = time.time() - start_time
     log.info(f"upgrading firmware took {total_time:.2f} s.")
 
     return True
 
 
 class GetFirmwareVersion(Command):
-
     command_id = CommandID.GET_FIRMWARE_VERSION
     broadcastable = True
     safe = True
     bootloader = True
 
     def get_replies(self) -> Dict[int, Any]:
         return self.get_firmware()
@@ -295,20 +291,18 @@
         for chunk in chunks:
             data += int_to_bytes(int(chunk), "u1")
 
         return data
 
 
 class StartFirmwareUpgrade(Command):
-
     command_id = CommandID.START_FIRMWARE_UPGRADE
     broadcastable = False
     safe = True
     bootloader = True
 
 
 class SendFirmwareData(Command):
-
     command_id = CommandID.SEND_FIRMWARE_DATA
     broadcastable = False
     safe = True
     bootloader = True
```

### Comparing `jaeger-1.3.3/python/jaeger/commands/calibration.py` & `jaeger-1.3.4/python/jaeger/commands/calibration.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,15 +277,14 @@
     def __init__(
         self,
         positioner_ids: int | List[int],
         alpha=None,
         beta=None,
         **kwargs,
     ):
-
         if alpha is not None and beta is not None:
             alpha_steps, beta_steps = motor_steps_to_angle(alpha, beta, inverse=True)
 
             data = int_to_bytes(int(alpha_steps)) + int_to_bytes(int(beta_steps))
             kwargs["data"] = data
 
         super().__init__(positioner_ids, **kwargs)
@@ -314,15 +313,14 @@
 
     command_id = CommandID.SET_HOLDING_CURRENT
     broadcastable = False
     safe = True
     move_command = False
 
     def __init__(self, positioner_ids, alpha=None, beta=None, **kwargs):
-
         if alpha is not None and beta is not None:
             data = int_to_bytes(int(alpha)) + int_to_bytes(int(beta))
             kwargs["data"] = data
 
         super().__init__(positioner_ids, **kwargs)
 
 
@@ -399,23 +397,21 @@
 
     command_id = CommandID.SET_INCREASE_COLLISION_MARGIN
     broadcastable = False
     move_command = False
     safe = False
 
     def __init__(self, positioner_ids, margin: int, **kwargs):
-
         data = int_to_bytes(int(margin), dtype="i4")
         kwargs["data"] = data
 
         super().__init__(positioner_ids, **kwargs)
 
 
 class GetAlphaHallCalibration(Command):
-
     command_id = CommandID.GET_ALPHA_HALL_CALIB
     broadcastable = False
     move_command = False
     safe = True
 
     def get_replies(self) -> Dict[int, Tuple[int, int, int, int]]:
         return self.get_values()
@@ -428,15 +424,14 @@
         for reply in self.replies:
             values[reply.positioner_id] = struct.unpack("HHHH", reply.data)
 
         return values
 
 
 class GetBetaHallCalibration(Command):
-
     command_id = CommandID.GET_BETA_HALL_CALIB
     broadcastable = False
     move_command = False
     safe = True
 
     def get_replies(self) -> Dict[int, Tuple[int, int, int, int]]:
         return self.get_values()
@@ -449,15 +444,14 @@
         for reply in self.replies:
             values[reply.positioner_id] = struct.unpack("HHHH", reply.data)
 
         return values
 
 
 class GetHallCalibrationError(Command):
-
     command_id = CommandID.GET_HALL_CALIB_ERROR
     broadcastable = False
     move_command = False
     safe = True
 
     def get_replies(self) -> Dict[int, Tuple[int, int]]:
         return self.get_values()
```

### Comparing `jaeger-1.3.3/python/jaeger/commands/goto.py` & `jaeger-1.3.4/python/jaeger/commands/goto.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,14 @@
     def __init__(
         self,
         positioner_ids: int | List[int],
         alpha: float | None = None,
         beta: float | None = None,
         **kwargs,
     ):
-
         if alpha is not None and beta is not None:
             alpha_steps, beta_steps = motor_steps_to_angle(alpha, beta, inverse=True)
 
             alpha_bytes = int_to_bytes(alpha_steps, dtype="i4")
             beta_bytes = int_to_bytes(beta_steps, dtype="i4")
 
             data = alpha_bytes + beta_bytes
@@ -160,17 +159,15 @@
     def __init__(
         self,
         positioner_ids: int | List[int],
         alpha: float | None = None,
         beta: float | None = None,
         **kwargs,
     ):
-
         if alpha is not None and beta is not None:
-
             alpha_steps, beta_steps = motor_steps_to_angle(alpha, beta, inverse=True)
 
             alpha_bytes = int_to_bytes(int(alpha_steps), dtype="i4")
             beta_bytes = int_to_bytes(int(beta_steps), dtype="i4")
 
             data = alpha_bytes + beta_bytes
 
@@ -190,15 +187,14 @@
     def __init__(
         self,
         positioner_ids: int | List[int],
         alpha: float | None = None,
         beta: float | None = None,
         **kwargs,
     ):
-
         if alpha is not None and beta is not None:
             assert alpha >= 0 and beta >= 0, "invalid speed."
 
             data = int_to_bytes(int(alpha)) + int_to_bytes(int(beta))
             kwargs["data"] = data
 
         super().__init__(positioner_ids, **kwargs)
@@ -223,15 +219,14 @@
     def __init__(
         self,
         positioner_ids: int | List[int],
         alpha: float | None = None,
         beta: float | None = None,
         **kwargs,
     ):
-
         if alpha is not None and beta is not None:
             assert alpha >= 0 and beta >= 0, "invalid current."
 
             data = int_to_bytes(int(alpha)) + int_to_bytes(int(beta))
             kwargs["data"] = data
 
         super().__init__(positioner_ids, **kwargs)
@@ -327,15 +322,14 @@
     else:
         if relative is True:
             raise JaegerError("relative is not implemented for kaiju moves.")
 
         data = {"collision_buffer": None, "grid": {}}
 
         for pid, (current_alpha, current_beta) in fps.get_positions_dict().items():
-
             if current_alpha is None or current_beta is None:
                 raise JaegerError(f"Positioner {pid} does not know its position.")
 
             if pid in new_positions:
                 data["grid"][int(pid)] = (
                     current_alpha,
                     current_beta,
```

### Comparing `jaeger-1.3.3/python/jaeger/commands/status.py` & `jaeger-1.3.4/python/jaeger/commands/status.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,14 @@
 
     command_id = CommandID.SWITCH_LED_ON
     broadcastable = False
     safe = True
 
 
 class GetNumberTrajectories(Command):
-
     command_id = CommandID.GET_NUMBER_TRAJECTORIES
     broadcastable = False
     safe = True
 
     def get_replies(self):
         return self.get_number_trajectories()
 
@@ -209,26 +208,24 @@
             else:
                 number_trajectories[reply.positioner_id] = bytes_to_int(data)
 
         return number_trajectories
 
 
 class SetNumberTrajectories(Command):
-
     command_id = CommandID.SET_NUMBER_TRAJECTORIES
     broadcastable = False
     safe = False
 
     def __init__(
         self,
         positioner_ids: int | List[int],
         moves: int | Dict[int, int],
         **kwargs,
     ):
-
         if isinstance(moves, int):
             data = int_to_bytes(moves)
         elif isinstance(moves, dict):
             data = {pos: int_to_bytes(moves[pos]) for pos in moves}
         else:
             raise TypeError("Invalid data type.")
```

### Comparing `jaeger-1.3.3/python/jaeger/commands/trajectory.py` & `jaeger-1.3.4/python/jaeger/commands/trajectory.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,14 @@
     log.info(msg)
     if command:
         command.info(msg)
 
     try:
         await traj.start(use_sync_line=use_sync_line)
     except TrajectoryError as err:
-
         if traj.start_time is not None and traj.end_time is not None:
             elapsed = traj.end_time - traj.start_time
             elapsed_msg = f" Trajectory failed {elapsed:.2f} seconds after start."
         else:
             elapsed_msg = ""
 
         raise TrajectoryError(
@@ -264,15 +263,14 @@
     def __init__(
         self,
         fps: FPS,
         trajectories: str | pathlib.Path | TrajectoryDataType,
         dump: bool | str = True,
         extra_dump_data: dict[str, Any] = {},
     ):
-
         self.fps = fps
         self.trajectories: TrajectoryDataType
 
         if isinstance(trajectories, (str, pathlib.Path)):
             path = pathlib.Path(trajectories)
             if path.suffix == ".json":
                 self.trajectories = json.loads(open(path, "r").read())["trajectory"]
@@ -392,15 +390,14 @@
             raise TrajectoryError("Some positioners did not respond.", self)
 
         if self.fps.moving:
             raise TrajectoryError("The FPS is moving. Cannot send trajectory.", self)
 
         # Check that all positioners are ready to receive a new trajectory.
         for pos_id in self.trajectories:
-
             positioner = self.fps.positioners[pos_id]
             status = positioner.status
 
             if positioner.disabled:
                 raise TrajectoryError(
                     f"positioner_id={pos_id} is disabled/offline but was "
                     "included in the trajectory.",
@@ -462,22 +459,19 @@
         # Gets the maximum number of points for each arm for all positioners.
         max_points = numpy.max(list(self.n_points.values()), axis=0)
         max_points = {"alpha": max_points[0], "beta": max_points[1]}
 
         # Send chunks of size n_chunk to all the positioners in parallel.
         # Do alpha first, then beta.
         for arm in ["alpha", "beta"]:
-
             for jj in range(0, max_points[arm], n_chunk):
-
                 data = {}
                 send_trajectory_pids = []
 
                 for pos_id in self.trajectories:
-
                     arm_chunk = self.trajectories[pos_id][arm][jj : jj + n_chunk]
                     if len(arm_chunk) == 0:
                         continue
 
                     send_trajectory_pids.append(pos_id)
 
                     positions = numpy.array(arm_chunk).astype(numpy.float64)
@@ -537,15 +531,14 @@
 
         if self.move_time is None:
             raise TrajectoryError("move_time not set.", self)
 
         self.use_sync_line = use_sync_line
 
         if use_sync_line:
-
             if not isinstance(self.fps.ieb, IEB) or self.fps.ieb.disabled:
                 raise TrajectoryError(
                     "IEB is not connected. Cannot use SYNC line.",
                     self,
                 )
             if (await self.fps.ieb.get_device("sync").read())[0] == "closed":
                 raise TrajectoryError("The SYNC line is on high.", self)
@@ -556,15 +549,14 @@
             # Set SYNC line to high.
             await sync.close()
 
             # Schedule reseting of SYNC line
             asyncio.get_event_loop().call_later(0.5, asyncio.create_task, sync.open())
 
         else:
-
             # Start trajectories
             command = await self.fps.send_command(
                 "START_TRAJECTORY",
                 positioner_ids=0,
                 timeout=1,
                 # All positioners reply, including those not in the trajectory.
                 n_positioners=len(self.fps.positioners),
@@ -578,15 +570,14 @@
         restart_pollers = True if self.fps.pollers.running else False
         await self.fps.pollers.stop()
 
         self.start_time = time.time()
 
         try:
             while True:
-
                 await asyncio.sleep(1)
 
                 if self.fps.locked:
                     raise TrajectoryError(
                         "The FPS got locked during the trajectory.",
                         self,
                     )
@@ -689,15 +680,14 @@
     """Starts a new trajectory and sends the number of points."""
 
     command_id = CommandID.SEND_NEW_TRAJECTORY
     broadcastable = False
     move_command = True
 
     def __init__(self, positioner_ids, n_alpha=None, n_beta=None, **kwargs):
-
         if n_alpha is not None and n_beta is not None:
             kwargs["data"] = self.get_data(n_alpha, n_beta)
         else:
             assert "data" in kwargs, "n_alpha/n_beta or data need to be passed."
 
         super().__init__(positioner_ids, **kwargs)
 
@@ -733,15 +723,14 @@
     """
 
     command_id = CommandID.SEND_TRAJECTORY_DATA
     broadcastable = False
     move_command = True
 
     def __init__(self, positioner_ids, positions=None, **kwargs):
-
         if positions is not None:
             kwargs["data"] = self.calculate_positions(positions)
         else:
             assert "data" in kwargs, "positions or data need to be passed."
 
         super().__init__(positioner_ids, **kwargs)
```

### Comparing `jaeger-1.3.3/python/jaeger/etc/chiller_APO.yaml` & `jaeger-1.3.4/python/jaeger/etc/chiller_APO.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.3/python/jaeger/etc/chiller_APO_variables.csv` & `jaeger-1.3.4/python/jaeger/etc/chiller_APO_variables.csv`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.3/python/jaeger/etc/fvc.yaml` & `jaeger-1.3.4/python/jaeger/etc/fvc.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.3/python/jaeger/etc/ieb_APO.yaml` & `jaeger-1.3.4/python/jaeger/etc/ieb_APO.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.3/python/jaeger/etc/ieb_LCO.yaml` & `jaeger-1.3.4/python/jaeger/etc/ieb_LCO.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.3/python/jaeger/etc/jaeger_APO.yml` & `jaeger-1.3.4/python/jaeger/etc/jaeger_APO.yml`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.3/python/jaeger/etc/jaeger_LCO.yml` & `jaeger-1.3.4/python/jaeger/etc/jaeger_LCO.yml`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.3/python/jaeger/etc/schema.json` & `jaeger-1.3.4/python/jaeger/etc/schema.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9958333333333333%*

 * *Differences: {"'properties'": "{'locked_alpha': OrderedDict([('type', 'number')]), 'locked_beta': "*

 * *                 "OrderedDict([('type', 'number')])}"}*

```diff
@@ -234,22 +234,28 @@
         },
         "kaiju_version": {
             "type": "string"
         },
         "locked": {
             "type": "boolean"
         },
+        "locked_alpha": {
+            "type": "number"
+        },
         "locked_axes": {
             "enum": [
                 "alpha",
                 "beta",
                 "both",
                 "?"
             ]
         },
+        "locked_beta": {
+            "type": "number"
+        },
         "locked_by": {
             "items": {
                 "type": "number"
             },
             "type": "array"
         },
         "manually_disabled": {
```

### Comparing `jaeger-1.3.3/python/jaeger/etc/sextants/epfl.yaml` & `jaeger-1.3.4/python/jaeger/etc/sextants/epfl.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.3/python/jaeger/etc/sextants/osu.yaml` & `jaeger-1.3.4/python/jaeger/etc/sextants/osu.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.3/python/jaeger/etc/sextants/schema.json` & `jaeger-1.3.4/python/jaeger/etc/sextants/schema.json`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.3/python/jaeger/etc/sextants/uw.yaml` & `jaeger-1.3.4/python/jaeger/etc/sextants/uw.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.3/python/jaeger/exceptions.py` & `jaeger-1.3.4/python/jaeger/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,29 +39,27 @@
         super(JaegerNotImplemented, self).__init__(message)
 
 
 class JaegerCANError(JaegerError):
     """Exception class for CAN-related errors."""
 
     def __init__(self, message=None, serial_reply=None):
-
         if message is None:
             message = ""
 
         if serial_reply is not None:
             message = message.strip() + " " + serial_reply
 
         super(JaegerCANError, self).__init__(message)
 
 
 class PositionerError(JaegerError):
     """Exception class for positioner-related errors."""
 
     def __init__(self, message=None, positioner=None):
-
         if message is None:
             message = ""
 
         if positioner is not None:
             pid = positioner.positioner_id
         else:
             stack = inspect.stack()
@@ -77,15 +75,14 @@
         super(PositionerError, self).__init__(message)
 
 
 class CommandError(JaegerError):
     """Exception class for command-related errors."""
 
     def __init__(self, message=None, command=None):
-
         if message is None:
             message = ""
 
         if command is None:
             stack = inspect.stack()
             f_locals = stack[1][0].f_locals
```

### Comparing `jaeger-1.3.3/python/jaeger/fps.py` & `jaeger-1.3.4/python/jaeger/fps.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,23 +100,21 @@
 
     positioner_class: ClassVar[Type[Positioner]] = Positioner
     _instance: dict[Type[BaseFPS], FPS_T] = {}
 
     initialised: bool
 
     def __new__(cls: Type[FPS_T], *args, **kwargs):
-
         if cls in cls._instance and kwargs == {}:
             raise JaegerError(
                 "An instance of FPS is already running. "
                 "Use get_instance() to retrieve it."
             )
 
         if cls not in cls._instance or kwargs != {}:
-
             if cls not in cls._instance:
                 new_obj = super().__new__(cls)
                 cls._instance[cls] = new_obj
             else:
                 new_obj = cls._instance[cls]
 
             dict.__init__(new_obj, {})
@@ -220,15 +218,14 @@
     # __instance: ClassVar[dict[Type[FPS], FPS]] = {}
 
     can: JaegerCAN | str | None = None
     ieb: Union[bool, IEB, dict, str, pathlib.Path, None] = None
     status: FPSStatus = FPSStatus.IDLE | FPSStatus.TEMPERATURE_NORMAL
 
     def __post_init__(self):
-
         super().__init__()
 
         # Start file logger
         start_file_loggers(start_log=True, start_can=False)
 
         if config.CONFIG_FILE:
             log.debug(f"Using configuration from {config.CONFIG_FILE}")
@@ -361,15 +358,14 @@
     def add_positioner(
         self,
         positioner: int | Positioner,
         centre=(None, None),
         interface: Optional[BusABC | int] = None,
         bus: Optional[int] = None,
     ) -> Positioner:
-
         positioner = super().add_positioner(positioner, centre=centre)
         positioner.fps = self
 
         if interface is not None:
             if isinstance(interface, int):
                 assert isinstance(self.can, JaegerCAN), "JaegerCAN not initialised."
                 interface = self.can.interfaces[interface]
@@ -476,15 +472,14 @@
         if get_fw_command.status.failed:
             raise JaegerError("Failed retrieving firmware version.")
 
         # Loops over each reply and set the positioner status to OK. If the
         # positioner was not in the list, adds it.
         for reply in get_fw_command.replies:
             if reply.positioner_id not in self.positioners:
-
                 if hasattr(reply.message, "interface"):
                     interface = reply.message.interface
                     bus = reply.message.bus
                 else:
                     interface = bus = None
 
                 self.add_positioner(reply.positioner_id, interface=interface, bus=bus)
@@ -650,15 +645,14 @@
                     CommandID.BETA_OPEN_LOOP_WITHOUT_COLLISION_DETECTION,
                     positioner_ids=open_loop_positioners,
                 )
 
         # Ensure closed loop mode for remaining robots. This does not work if
         # any of the robots is collided.
         if not self.locked:
-
             closed_loop_positioners = list(
                 set([pid for pid in self.positioners if not self[pid].disabled])
                 - set(disable_collision)
                 - set(open_loop_positioners)
             )
             await self.send_command(
                 CommandID.ALPHA_CLOSED_LOOP_COLLISION_DETECTION,
@@ -928,33 +922,41 @@
         if stop_trajectories:
             await self.stop_trajectory()
 
         await self.update_status()
 
         axes = "?"
 
+        alpha = -999.0
+        beta = -999.0
+
         if by and len(by) > 0:
             self.locked_by += by
 
             status_bits = self.positioners[by[0]].status
             if status_bits & PositionerStatus.COLLISION_ALPHA:
                 axes = "alpha"
             if status_bits & PositionerStatus.COLLISION_BETA:
                 if axes == "alpha":
                     axes = "both"
                 else:
                     axes = "beta"
 
+            alpha = self.positioners[by[0]].alpha
+            beta = self.positioners[by[0]].beta
+
         if jaeger.actor_instance:
             jaeger.actor_instance.write(
                 "e",
                 {
                     "locked": True,
                     "locked_by": self.locked_by,
                     "locked_axes": axes,
+                    "locked_alpha": alpha,
+                    "locked_beta": beta,
                 },
             )
 
         if snapshot:
             if self.locked_by is not None:
                 highlight = self.locked_by[0]
             else:
@@ -1062,15 +1064,14 @@
             return await self.update_status(positioner_ids, is_retry=True)
 
         if len(command.replies) == 0:
             return True
 
         update_status_coros = []
         for pid, status_int in command.get_positioner_status().items():  # type: ignore
-
             if pid not in self:
                 continue
 
             update_status_coros.append(self[pid].update_status(status_int))
 
         await asyncio.gather(*update_status_coros)
 
@@ -1336,15 +1337,14 @@
 
     async def report_status(self) -> Dict[str, Any]:
         """Returns a dict with the position and status of each positioner."""
 
         status: Dict[str, Any] = {"positioners": {}}
 
         for positioner in self.positioners.values():
-
             pos_status = positioner.status
             pos_firmware = positioner.firmware
             pos_alpha = positioner.alpha
             pos_beta = positioner.beta
 
             status["positioners"][positioner.positioner_id] = {
                 "position": [pos_alpha, pos_beta],
@@ -1465,15 +1465,14 @@
 
         sensor = config["low_temperature"]["sensor"]
         cold = config["low_temperature"]["cold_threshold"]
         very_cold = config["low_temperature"]["very_cold_threshold"]
         interval = config["low_temperature"]["interval"]
 
         while True:
-
             try:
                 assert isinstance(self.ieb, IEB) and self.ieb.disabled is False
                 device = self.ieb.get_device(sensor)
                 temp = (await device.read())[0]
 
                 # Get the status without the temperature bits.
                 base_status = self.status & ~FPSStatus.TEMPERATURE_BITS
```

### Comparing `jaeger-1.3.3/python/jaeger/fvc.py` & `jaeger-1.3.4/python/jaeger/fvc.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,14 @@
     centroid_method: str | None
     fitrms: float
     k: float
 
     ieb_data: dict[str, Any] = {}
 
     def __init__(self, site: str, command: Optional[Command[JaegerActor]] = None):
-
         if len(calibration.positionerTable) == 0:
             warnings.warn(
                 "FPS calibrations not loaded or the array is empty.",
                 JaegerUserWarning,
             )
 
         self.site = site
```

### Comparing `jaeger-1.3.3/python/jaeger/ieb.py` & `jaeger-1.3.4/python/jaeger/ieb.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,14 @@
     Allows additional features such as disabling the interface.
 
     """
 
     MAX_RETRIES: int = 5
 
     def __init__(self, *args, **kwargs):
-
         self.disabled = False
 
         super().__init__(*args, **kwargs)
 
         self._categories = None
         self._n_failures: int = 0
 
@@ -92,30 +91,28 @@
             ]
             self._categories = set(categories)
             self._categories.discard(None)
 
         return self._categories
 
     async def __aenter__(self):
-
         if self.disabled:
             raise DriftError("IEB is disabled.")
 
         n_retries = 0
         while True:
             try:
                 await Drift.__aenter__(self)
                 break
             except DriftError:
                 n_retries += 1
                 if n_retries >= 5:
                     raise DriftError("Failed connecting to the IEB.")
 
     async def __aexit__(self, *args):
-
         await Drift.__aexit__(self, *args)
 
     def enable(self):
         """Re-enables the IEB instance."""
 
         self._n_failures = 0
         self.disabled = False
```

### Comparing `jaeger-1.3.3/python/jaeger/interfaces/bus.py` & `jaeger-1.3.4/python/jaeger/interfaces/bus.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.3/python/jaeger/interfaces/cannet.py` & `jaeger-1.3.4/python/jaeger/interfaces/cannet.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,14 @@
         channel,
         port=None,
         bitrate=None,
         buses=[1],
         timeout=5,
         **kwargs,
     ):
-
         if not channel:  # if None or empty
             raise TypeError("Must specify a TCP address.")
 
         self.channel = channel
 
         if not bitrate:
             raise TypeError("Must specify a bitrate.")
@@ -86,15 +85,14 @@
         self._timeout = timeout
 
         self.channel_info = f"CAN@net channel={channel!r}, buses={self.buses!r}"
 
         super(CANNetBus, self).__init__(channel, bitrate=None, **kwargs)
 
     def write(self, string):
-
         if not self.connected or not self.writer:
             raise ConnectionError(f"Interface {self.channel} is not connected.")
 
         self.writer.write(string.encode() + self.LINE_TERMINATOR)
 
     def _write_to_buses(self, string, buses=None):
         """Writes a string to the correct bus."""
@@ -104,15 +102,14 @@
         elif not isinstance(buses, (list, tuple)):
             buses = [buses]
 
         for bus in buses:
             self.write(string.format(bus=bus))
 
     async def _open_internal(self, timeout=None):
-
         timeout = timeout or self._timeout
 
         self.close()
 
         try:
             open_conn = asyncio.open_connection(self.channel, self.port)
             self.reader, self.writer = await asyncio.wait_for(open_conn, timeout)
@@ -137,24 +134,22 @@
 
         # Clear buffer
         await self.reader.read(8192)
 
         return True
 
     def close(self, buses=None):
-
         if self.writer and not self.writer.is_closing():
             self._write_to_buses("CAN {bus} STOP")
             self.writer.close()
 
         self.connected = False
         self.writer = self.reader = None
 
     async def get(self):
-
         canId = None
         remote = False
         extended = False
         frame = []
 
         if not self.reader:
             raise ConnectionError(f"Interface {self.channel} is not connected.")
@@ -224,21 +219,19 @@
             msg.interface = self
             msg.bus = bus
             return msg
 
         return None
 
     def send(self, msg, bus=None):
-
         buses = bus or self.buses
         if not isinstance(buses, (list, tuple)):
             buses = [buses]
 
         for bus in buses:
-
             sendStr = f"M {bus} "
 
             if msg.is_extended_id:
                 if msg.is_remote_frame:
                     sendStr += f"CER {msg.arbitration_id:08X}"
                 else:
                     sendStr += f"CED {msg.arbitration_id:08X}"
```

### Comparing `jaeger-1.3.3/python/jaeger/interfaces/message.py` & `jaeger-1.3.4/python/jaeger/interfaces/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
         "bitrate_switch",
         "error_state_indicator",
         "__weakref__",  # support weak references to messages
         "_dict",  # see __getattr__
     )
 
     def __getattr__(self, key):
-
         if key not in self.__slots__:
             raise AttributeError
         try:
             warnings.warn(
                 "Custom attributes of messages are deprecated "
                 "and will be removed in 4.0",
                 DeprecationWarning,
```

### Comparing `jaeger-1.3.3/python/jaeger/interfaces/notifier.py` & `jaeger-1.3.4/python/jaeger/interfaces/notifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 Bus_co = TypeVar("Bus_co", bound="BusABC")
 
 
 class Notifier:
     """Notifier class to report bus messages to multiple listeners."""
 
     def __init__(self, listeners: List[Listener_co] = [], buses: List[Bus_co] = []):
-
         self.loop = asyncio.get_running_loop()
 
         self.listeners = listeners
 
         self.tasks: list[asyncio.Task] = []
 
         self.buses: List[BusABC] = []
```

### Comparing `jaeger-1.3.3/python/jaeger/interfaces/virtual.py` & `jaeger-1.3.4/python/jaeger/interfaces/virtual.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 queues: Dict[str, List[asyncio.Queue]] = {}
 
 
 class VirtualBus(BusABC):
     """A class implementing a virtual CAN bus that listens to messages on a channel."""
 
     def __init__(self, channel: str):
-
         self.channel = channel
 
         self.queue: asyncio.Queue[Message] = asyncio.Queue()
 
         if self.channel not in queues:
             queues[self.channel] = [self.queue]
         else:
```

### Comparing `jaeger-1.3.3/python/jaeger/kaiju.py` & `jaeger-1.3.4/python/jaeger/kaiju.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.3/python/jaeger/maskbits.py` & `jaeger-1.3.4/python/jaeger/maskbits.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.3/python/jaeger/plotting.py` & `jaeger-1.3.4/python/jaeger/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,18 +18,16 @@
 from jaeger.target.configuration import BaseConfiguration
 
 
 __all__ = ["plot_fvc_distances"]
 
 
 def _plot_wok_distance(data_F: pandas.DataFrame, ax: plt.Axes, is_dither: bool = False):
-
     colours = ["g", "r", "b"]
     for ii, fibre in enumerate(["Metrology", "APOGEE", "BOSS"]):
-
         data_fibre = data_F.loc[pandas.IndexSlice[:, fibre], :].copy()
 
         if fibre != "Metrology" and is_dither is False:
             data_fibre = data_fibre.loc[
                 (data_fibre.assigned == 1) & (data_fibre.on_target == 1), :
             ]
         if len(data_fibre) == 0:
@@ -67,15 +65,14 @@
     data_F: pandas.DataFrame,
     ax: plt.Axes,
     column: str,
     is_dither: bool = False,
     plot_metrology: bool = True,
     title: str = "Sky distance",
 ):
-
     colours = ["g", "r", "b"]
     for ii, fibre in enumerate(["Metrology", "APOGEE", "BOSS"]):
         if fibre == "Metrology" and not plot_metrology:
             continue
 
         data_fibre = data_F.loc[pandas.IndexSlice[:, fibre], :].copy()
 
@@ -111,18 +108,16 @@
 
         ax.set_title(title)
 
         ax.legend()
 
 
 def _plot_sky_quiver(data_F: pandas.DataFrame, ax: plt.Axes, is_dither: bool = False):
-
     colours = ["r", "b"]
     for ii, fibre in enumerate(["APOGEE", "BOSS"]):
-
         data_fibre = data_F.loc[pandas.IndexSlice[:, fibre], :].copy()
 
         if is_dither is False:
             data_fibre = data_fibre.loc[
                 (data_fibre.assigned == 1) & (data_fibre.on_target == 1), :
             ]
         if len(data_fibre) == 0:
@@ -200,15 +195,14 @@
         data_F["racat_distance"] = (data_F.ra_icrs - data_F.ra_epoch) * cos_dec * 3600.0
         data_F["deccat_distance"] = (data_F.dec_icrs - data_F.dec_epoch) * 3600.0
         data_F["skycat_distance"] = numpy.hypot(
             data_F.racat_distance, data_F.deccat_distance
         )
 
     with plt.ioff():  # type: ignore
-
         seaborn.set_theme()
 
         fig, axes = plt.subplots(1, 3, figsize=(30, 10))
 
         if not is_dither:
             data_F = data_F.groupby("positioner_id").filter(
                 lambda g: g.assigned.any() & g.on_target.any() & g.valid.all()
```

### Comparing `jaeger-1.3.3/python/jaeger/positioner.py` & `jaeger-1.3.4/python/jaeger/positioner.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 
     def __init__(
         self,
         positioner_id: int,
         fps: jaeger.FPS | None = None,
         centre: Tuple[Optional[float], Optional[float]] = (None, None),
     ):
-
         self.fps = fps
 
         self.positioner_id = positioner_id
 
         self.centre = centre
 
         self.alpha = None
@@ -171,15 +170,14 @@
         self,
         position: Tuple[float, float] | None = None,
         timeout=1,
     ):
         """Updates the position of the alpha and beta arms."""
 
         if position is None:
-
             command = await self.send_command(
                 CommandID.GET_ACTUAL_POSITION,
                 timeout=timeout,
             )
 
             assert isinstance(command, GetActualPosition)
 
@@ -204,15 +202,14 @@
         assert self.fps, "FPS is not set."
 
         # Need to update the firmware to make sure we get the right flags.
         if not self.firmware:
             await self.update_firmware_version()
 
         if not status:
-
             command = await self.send_command(
                 CommandID.GET_STATUS,
                 timeout=timeout,
                 error="cannot get status.",
             )
 
             n_replies = len(command.replies)
@@ -267,15 +264,14 @@
         if self.is_bootloader():
             raise JaegerError("wait_for_status cannot be scheduled in bootloader mode.")
 
         if not isinstance(status, (list, tuple)):
             status = [status]
 
         async def status_waiter(wait_for_status):
-
             while True:
                 await self.update_status()
                 # Check all statuses in the list
                 all_reached = True
                 for ss in wait_for_status:
                     if ss not in self.status:
                         all_reached = False
@@ -567,15 +563,14 @@
 
         if motor == "both":
             motors = ["alpha", "beta"]
         else:
             motors = [motor]
 
         for motor in motors:
-
             command_name = motor.upper() + "_" + loop.upper() + "_LOOP"
             if collisions:
                 command_name += "_COLLISION_DETECTION"
             else:
                 command_name += "_WITHOUT_COLLISION_DETECTION"
 
             await self.send_command(
@@ -586,15 +581,14 @@
                 f"set motor={motor!r}, loop={loop!r}, "
                 f"detect_collision={collisions}",
             )
 
         return True
 
     def __repr__(self):
-
         return (
             f"<Positioner (id={self.positioner_id}, "
             f"status={self.status!s}, initialised={self.initialised})>"
         )
 
     async def get_number_trajectories(self) -> int | None:
         """Returns the number of trajectories executed by the positioner.
```

### Comparing `jaeger-1.3.3/python/jaeger/scripts/generate_chiller_yaml.py` & `jaeger-1.3.4/python/jaeger/scripts/generate_chiller_yaml.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.3/python/jaeger/scripts/robotcalib.py` & `jaeger-1.3.4/python/jaeger/scripts/robotcalib.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
     xwok = []
     ywok = []
     alpha = []
     beta = []
     offline = []
 
     for r in rg.robotDict.values():
-
         # append metrology fiber info
         positioner_id.append(r.id)
         hole_id.append(r.holeID)
         fibre_type.append("Metrology")
         xwok.append(r.metWokXYZ[0])
         ywok.append(r.metWokXYZ[1])
         alpha.append(r.alpha)
```

### Comparing `jaeger-1.3.3/python/jaeger/target/configuration.py` & `jaeger-1.3.4/python/jaeger/target/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,14 @@
 class BaseConfiguration:
     """A base configuration class."""
 
     assignment_data: BaseAssignmentData
     epoch: float | None
 
     def __init__(self, scale: float | None = None):
-
         if len(calibration.positionerTable) == 0:
             raise ValueError("FPS calibrations not loaded or the array is empty.")
 
         # Configuration ID is None until we insert in the database.
         # Once set, it cannot be changed.
         self.configuration_id: int | None = None
         self._summary_file: str | None = None
@@ -625,17 +624,15 @@
         if "admin" in targetdb.database._config:
             targetdb.database.become_admin()
 
         assert self.assignment_data.site.time
         epoch = self.assignment_data.site.time.jd
 
         if self.configuration_id is None:
-
             with opsdb.database.atomic():
-
                 if self.design is None:
                     if (
                         targetdb.Design()
                         .select()
                         .where(targetdb.Design.design_id == self.design_id)
                         .exists()
                     ):
@@ -654,15 +651,14 @@
 
             if configuration.configuration_id is None:
                 raise JaegerError("Failed loading configuration.")
 
             self.configuration_id = configuration.configuration_id
 
         else:
-
             if self.configuration_id is None:
                 raise JaegerError("Must have a configuration_id to replace.")
 
             if not self.ingested:
                 raise JaegerError(
                     f"Configuration ID {self.configuration_id} does not exists "
                     "in opsdb and cannot be replaced."
@@ -685,15 +681,14 @@
 
                 return self.write_to_database(replace=False)
 
         a_data = self.assignment_data.fibre_table
 
         focals = []
         for index, data in a_data.iterrows():
-
             index = cast(tuple, index)
             pid = index[0]
             hole_id = data.hole_id
             try:
                 if data.valid == 0:
                     raise ValueError(f"Invalid coordinate found for positioner {pid}.")
 
@@ -720,15 +715,14 @@
             )
 
         with opsdb.database.atomic():
             opsdb.AssignmentToFocal.insert_many(focals).execute(opsdb.database)
 
     @staticmethod
     def _get_summary_file_path(configuration_id: int, observatory: str, flavour: str):
-
         if configuration_id is None:
             raise JaegerError("Configuration ID not set.")
 
         if "SDSSCORE_DIR" not in os.environ:
             raise JaegerError("$SDSSCORE_DIR is not set. Cannot write summary file.")
 
         sdsscore_dir = os.environ["SDSSCORE_DIR"]
@@ -823,15 +817,14 @@
         header.update(headers)
         header.update(self.extra_summary_data)
 
         fibermap, default = get_fibermap_table(len(fdata))
 
         i = 0
         for index, row_data in fdata.iterrows():
-
             index = cast(tuple, index)
 
             pid, fibre_type = index
             hole_id = row_data.hole_id
 
             # Start with the default row.
             row = default.copy()
@@ -945,15 +938,14 @@
 
     def __init__(
         self,
         design: Design,
         epoch: float | None = None,
         scale: float | None = None,
     ):
-
         super().__init__(scale=scale)
 
         self.design = design
         self.design_id = design.design_id
         self.assignment_data = AssignmentData(self, epoch=epoch, scale=scale)
 
         assert self.assignment_data.site.time
@@ -973,15 +965,14 @@
 
     def __init__(
         self,
         parent_configuration: BaseConfiguration,
         radius: float,
         epoch: float | None = None,
     ):
-
         assert parent_configuration.design
 
         super().__init__(scale=parent_configuration.scale)
 
         # This needs to be set after the __init__ beccause __init__ sets
         # parent_configuration=None.
         self.parent_configuration = parent_configuration
@@ -1016,15 +1007,14 @@
         self.extra_summary_data = {
             "parent_configuration": self.parent_configuration.configuration_id or -999,
             "is_dithered": 1,
             "dither_radius": radius,
         }
 
     def compute_coordinates(self, new_positions: dict):
-
         assert self.design
 
         ftable = self.assignment_data.fibre_table
 
         data = {}
 
         for index, _ in self.assignment_data.fibre_table.iterrows():
@@ -1157,15 +1147,14 @@
         target_data: dict[str, dict],
         field_centre: tuple[float, float] | numpy.ndarray | None = None,
         design_id: int = -999,
         observatory: str | None = None,
         position_angle: float = 0.0,
         scale: float | None = None,
     ):
-
         super().__init__(scale=scale)
 
         self.design = None
         self.design_id = design_id
         self.epoch = None
 
         if observatory is None:
@@ -1258,15 +1247,14 @@
 
     def __init__(
         self,
         configuration: Configuration | ManualConfiguration | DitheredConfiguration,
         observatory: Optional[str] = None,
         scale: float | None = None,
     ):
-
         self.configuration = configuration
 
         self.design = configuration.design
         self.design_id = self.configuration.design_id
 
         self.observatory: str
         if observatory is None:
@@ -1356,21 +1344,19 @@
     def _init_from_icrs(self):
         """Loads fibre data from target data using ICRS coordinates."""
 
         alpha0, beta0 = config["kaiju"]["lattice_position"]
 
         data = {}
         for pid in self.wok_data.index:
-
             positioner_data = self.wok_data.loc[pid]
             hole_id = positioner_data.holeID
 
             target_fibre_type: str | None = None
             if hole_id in self.target_data:
-
                 # First do the assigned fibre.
                 ftype = self.target_data[hole_id]["fibre_type"].upper()
                 target_fibre_type = ftype
 
                 target_data = self.target_data[hole_id]
                 positioner_data = self.icrs_to_positioner(
                     pid,
@@ -1380,15 +1366,14 @@
                     update=False,
                     on_target=1,
                     assigned=1,
                 )
                 data[(pid, ftype)] = positioner_data
 
             else:
-
                 # If a positioner does not have an assigned target, leave it folded.
                 target_fibre_type = None
                 positioner_data = {"alpha": alpha0, "beta": beta0}
 
             # Now calculate some coordinates for the other two non-assigned fibres.
             for ftype in ["APOGEE", "BOSS", "Metrology"]:
                 if ftype == target_fibre_type:
@@ -1412,15 +1397,14 @@
     def _init_from_wok(self):
         """Loads fibre data from target data using wok coordinates."""
 
         self._check_all_assigned()
 
         # Calculate positioner coordinates for each wok coordinate.
         for hole_id, data in self.target_data.items():
-
             xwok = data["xwok"]
             ywok = data["ywok"]
             zwok = data.get("zwok", POSITIONER_HEIGHT)
             fibre_type = data["fibre_type"]
 
             (alpha, beta), _ = wok_to_positioner(
                 hole_id,
@@ -1461,22 +1445,20 @@
     def _init_from_positioner(self):
         """Loads fibre data from target data using positioner coordinates."""
 
         self._check_all_assigned()
 
         data = {}
         for pid in self.wok_data.index:
-
             hole_id = self.wok_data.at[pid, "holeID"]
             alpha = self.target_data[hole_id]["alpha"]
             beta = self.target_data[hole_id]["beta"]
 
             # Now calculate some coordinates for the other two non-assigned fibres.
             for ftype in ["APOGEE", "BOSS", "Metrology"]:
-
                 assigned = self.target_data[hole_id]["fibre_type"] == ftype
 
                 # If boresight has been set, go all the way from positioner to ICRS.
                 # Otherwise just calculate tangent and wok.
                 if self.boresight:
                     icrs_data = self.positioner_to_icrs(
                         pid,
@@ -1487,15 +1469,14 @@
                         update=False,
                         assigned=int(assigned),
                         on_target=int(assigned),
                     )
                     data[(pid, ftype)] = icrs_data
 
                 else:
-
                     wok, tangent = positioner_to_wok(
                         hole_id,
                         self.site.name,
                         ftype,
                         alpha,
                         beta,
                     )
@@ -1724,15 +1705,14 @@
     def __init__(
         self,
         configuration: Configuration | DitheredConfiguration,
         epoch: float | None = None,
         compute_coordinates: bool = True,
         scale: float | None = None,
     ):
-
         super().__init__(configuration, scale=scale)
 
         if compute_coordinates:
             self.compute_coordinates(epoch)
 
     def compute_coordinates(self, jd: Optional[float] = None):
         """Computes coordinates in different systems.
@@ -1799,15 +1779,14 @@
         configuration: ManualConfiguration,
         target_data: dict,
         observatory: str,
         field_centre: tuple[float, float] | numpy.ndarray | None = None,
         position_angle: float = 0.0,
         scale: float | None = None,
     ):
-
         super().__init__(configuration, observatory=observatory, scale=scale)
 
         self.target_data = target_data
 
         if field_centre is not None:
             self.field_centre = numpy.array(field_centre)
         else:
```

### Comparing `jaeger-1.3.3/python/jaeger/target/design.py` & `jaeger-1.3.4/python/jaeger/target/design.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import pandas
 import peewee
 
 from coordio.defaults import calibration
 from coordio.utils import object_offset
 from sdssdb.peewee.sdss5db import targetdb
 
+from jaeger import log
 from jaeger.utils.database import connect_database
 from jaeger.utils.helpers import run_in_executor
 
 from .configuration import Configuration
 
 
 __all__ = ["Design"]
@@ -50,26 +51,28 @@
     epoch
         The JD epoch for which to calculate the configuration coordinates. If
         `None`, uses the current time.
     scale
         Focal plane scale factor to apply. Defaults to coordio's internal value.
     safety_factor
         For offset calculation. Factor to add to ``mag_limit``. See ``object_offset``.
+    offset_min_skybrightness
+        Minimum sky brightness for the offset. See ``object_offset``.
 
     """
 
     def __init__(
         self,
         design_id: int,
         load_configuration: bool = True,
         epoch: float | None = None,
         scale: float | None = None,
         safety_factor: float = 0.1,
+        offset_min_skybrightness: float = 0.5,
     ):
-
         if calibration.wokCoords is None:
             raise RuntimeError("Cannot retrieve wok calibration. Is $WOKCALIB_DIR set?")
 
         self.design_id = design_id
 
         if connect_database(targetdb.database) is False:
             raise RuntimeError("Cannot connect to database.")
@@ -85,14 +88,15 @@
             observatory=self.design.field.observatory.label,
             racen=self.design.field.racen,
             deccen=self.design.field.deccen,
             position_angle=self.design.field.position_angle,
         )
 
         self.safety_factor = safety_factor
+        self.offset_min_skybrightness = offset_min_skybrightness
         self.target_data: dict[str, dict] = self.get_target_data()
 
         self.configuration: Configuration
         if load_configuration:
             self.configuration = Configuration(self, epoch=epoch, scale=scale)
 
     def get_target_data(self) -> dict[str, dict]:
@@ -145,15 +149,14 @@
 
         return {data["holeid"]: data for data in list(target_data)}
 
     def calculate_offsets(self, target_data: list[dict]):
         """Determines the target offsets."""
 
         def _offset(group: pandas.DataFrame):
-
             design_mode = group.iloc[0].design_mode
             fibre_type = group.iloc[0].fibre_type
 
             design_mode_rec = targetdb.DesignMode.get(label=design_mode)
 
             if fibre_type == "APOGEE":
                 # Use 2MASS H magnitude for APOGEE
@@ -167,33 +170,33 @@
             if "bright" in design_mode:
                 lunation = "bright"
                 skybrightness = 1.0
             else:
                 lunation = "dark"
                 skybrightness = 0.35
 
-            # Hardcoding this for now.
-            offset_min_skybrightness = 0.5
-
             delta_ra, delta_dec, _ = object_offset(
                 mag,
                 mag_lim,
                 lunation,
                 fibre_type.capitalize(),
                 can_offset=group.can_offset.values,
                 skybrightness=skybrightness,
-                offset_min_skybrightness=offset_min_skybrightness,
                 safety_factor=self.safety_factor,
+                offset_min_skybrightness=self.offset_min_skybrightness,
             )
 
             group.loc[:, "delta_ra"] = delta_ra
             group.loc[:, "delta_dec"] = delta_dec
 
             return group
 
+        log.debug(f"offset_min_skybrightness={self.offset_min_skybrightness}")
+        log.debug(f"safety_factor={self.safety_factor}")
+
         # Convert to data frame to group by fibre type (no need to group by design
         # mode since a design can only have one design mode).
         df = pandas.DataFrame.from_records(target_data)
         df = df.groupby(["fibre_type"], group_keys=False).apply(_offset)
 
         # Return as a list of dicts again.
         return [vv for vv in df.transpose().to_dict().values()]
```

### Comparing `jaeger-1.3.3/python/jaeger/target/tools.py` & `jaeger-1.3.4/python/jaeger/target/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,14 @@
 
     robot_grid = get_robot_grid(fps, seed=seed, collision_buffer=collision_buffer)
 
     alphaL, betaL = config["kaiju"]["lattice_position"]
 
     # We use Kaiju for convenience in the non-safe mode.
     for robot in robot_grid.robotDict.values():
-
         if robot.isOffline:
             continue
 
         if uniform is not None:
             alpha0, alpha1, beta0, beta1 = uniform
             robot.setAlphaBeta(
                 numpy.random.uniform(alpha0, alpha1),
@@ -264,15 +263,14 @@
             robot_grid = get_robot_grid(
                 fps,
                 seed=seed + 1,
                 collision_buffer=collision_buffer,
             )
 
             for robot in robot_grid.robotDict.values():
-
                 if robot.isOffline:
                     continue
 
                 if robot.id == to_replace_robot:
                     robot.setXYUniform()
                 else:
                     robot.setAlphaBeta(*grid_data[robot.id])
```

### Comparing `jaeger-1.3.3/python/jaeger/testing.py` & `jaeger-1.3.4/python/jaeger/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,37 +30,33 @@
 
     This class listens to a virtual bus and responds as if real positioners were
     plugged into the system.
 
     """
 
     def __post_init__(self):
-
         self.can = "virtual"
         self.ieb = True
         self.observatory = "APO"
 
         super().__post_init__()
 
         self._vpositioner_bus = VirtualBus(config["profiles"]["virtual"]["channel"])
         self._vpositioners = {}
 
         asyncio.create_task(self.process_messages())
 
     def add_virtual_positioner(self, pid: int):
-
         self._vpositioners[pid] = VirtualPositioner(pid, bus=self._vpositioner_bus)
 
     def _check_fibre_assignments(self, *args, **kwargs):
         pass
 
     async def process_messages(self):
-
         while True:
-
             msg = await self._vpositioner_bus.get()
 
             if msg is None:
                 continue
 
             arbitration_id = msg.arbitration_id
             positioner_id, command_id, uid, __ = utils.parse_identifier(arbitration_id)
@@ -125,15 +121,14 @@
         positioner_id: int,
         bus: Optional[VirtualBus] = None,
         centre: Optional[tuple] = None,
         position: Tuple[float, float] = (0.0, 0.0),
         speed: Optional[tuple] = None,
         firmware: str = "10.11.12",
     ):
-
         self.positioner_id = positioner_id
         self.centre = centre or (None, None)
 
         self.position = position
         self.speed = speed or (
             config["positioner"]["motor_speed"],
             config["positioner"]["motor_speed"],
@@ -232,15 +227,14 @@
 
         else:
             # Should be a valid command or CommandID(command_id) would
             # have failed. Just return OK.
             self.reply(command_id, uid)
 
     def reply(self, command_id, uid, response_code=None, data=None):
-
         response_code = response_code or ResponseCode.COMMAND_ACCEPTED
 
         if isinstance(data, (bytearray, bytes)):
             data = [data]
         elif not data:
             data = [None]
```

### Comparing `jaeger-1.3.3/python/jaeger/utils/database.py` & `jaeger-1.3.4/python/jaeger/utils/database.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.3/python/jaeger/utils/helpers.py` & `jaeger-1.3.4/python/jaeger/utils/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,14 @@
     def __init__(
         self,
         maskbit_flags: Type[Status_co],
         initial_status: Optional[Status_co] = None,
         callback_func: Optional[Callable] = None,
         call_now: bool = False,
     ):
-
         self._flags = maskbit_flags
         self.callbacks = []
         self._status: Optional[Status_co] = initial_status
         self.watcher = None
 
         if callback_func is not None:
             self.callbacks.append(callback_func)
@@ -183,15 +182,14 @@
         self.watcher = None
 
 
 class PollerList(list):
     """A list of `.Poller` to be managed jointly."""
 
     def __init__(self, pollers=[]):
-
         names = [poller.name for poller in pollers]
         assert len(names) == len(set(names)), "repeated names in poller list."
 
         list.__init__(self, pollers)
 
     @property
     def names(self):
@@ -288,15 +286,14 @@
         Initial delay between calls to the callback.
     loop : event loop
         The event loop to which to attach the task.
 
     """
 
     def __init__(self, name, callback, delay=1.0, loop=None):
-
         self.name = name
         self.callback = callback
 
         self._orig_delay = delay
         self.delay = delay
 
         self.loop: asyncio.AbstractEventLoop = loop or asyncio.get_event_loop()
@@ -310,15 +307,14 @@
     async def poller(self):
         """The polling loop."""
 
         if self._task is None:
             raise RuntimeError("Task is not running.")
 
         while True:
-
             try:
                 if asyncio.iscoroutinefunction(self.callback):
                     await self.callback()
                 else:
                     self.callback()
             except Exception as ee:
                 if ee.__class__ == asyncio.CancelledError:
@@ -489,15 +485,14 @@
     return result
 
 
 class BaseBot:
     """A class that monitors a subsystem."""
 
     def __init__(self, fps: FPS):
-
         self.fps = fps
         self.ieb = fps.ieb
 
         self.actor: JaegerActor | None = None
 
         self._task: asyncio.Task | None = None
```

### Comparing `jaeger-1.3.3/python/jaeger/utils/utils.py` & `jaeger-1.3.4/python/jaeger/utils/utils.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.3/PKG-INFO` & `jaeger-1.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaeger
-Version: 1.3.3
+Version: 1.3.4
 Summary: Controllers for the SDSS-V FPS
 Home-page: https://github.com/sdss/jaeger
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.8,<3.12
```

