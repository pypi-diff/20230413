# Comparing `tmp/python-pygaze-0.7.5a5.tar.gz` & `tmp/python-pygaze-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-pygaze-0.7.5a5.tar", last modified: Wed Aug 17 10:24:05 2022, max compression
+gzip compressed data, was "python-pygaze-0.7.6.tar", last modified: Thu Apr 13 09:53:19 2023, max compression
```

## Comparing `python-pygaze-0.7.5a5.tar` & `python-pygaze-0.7.6.tar`

### file list

```diff
@@ -1,134 +1,145 @@
-drwxrwxr-x   0 ha21245   (1001) ha21245   (1001)        0 2022-08-17 10:24:05.541275 python-pygaze-0.7.5a5/
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)      112 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/MANIFEST.in
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     3223 2022-08-17 10:24:05.541275 python-pygaze-0.7.5a5/PKG-INFO
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     2144 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/README.md
-drwxrwxr-x   0 ha21245   (1001) ha21245   (1001)        0 2022-08-17 10:24:05.521275 python-pygaze-0.7.5a5/opensesame_plugins/
-drwxrwxr-x   0 ha21245   (1001) ha21245   (1001)        0 2022-08-17 10:24:05.525275 python-pygaze-0.7.5a5/opensesame_plugins/artwork/
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)   709124 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/opensesame_plugins/artwork/icons.svg
-drwxrwxr-x   0 ha21245   (1001) ha21245   (1001)        0 2022-08-17 10:24:05.525275 python-pygaze-0.7.5a5/opensesame_plugins/pygaze_drift_correct/
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     1159 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/opensesame_plugins/pygaze_drift_correct/info.yaml
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     3538 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/opensesame_plugins/pygaze_drift_correct/pygaze_drift_correct.py
-drwxrwxr-x   0 ha21245   (1001) ha21245   (1001)        0 2022-08-17 10:24:05.525275 python-pygaze-0.7.5a5/opensesame_plugins/pygaze_init/
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     3331 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/opensesame_plugins/pygaze_init/info.yaml
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     9885 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/opensesame_plugins/pygaze_init/pygaze_init.py
-drwxrwxr-x   0 ha21245   (1001) ha21245   (1001)        0 2022-08-17 10:24:05.525275 python-pygaze-0.7.5a5/opensesame_plugins/pygaze_log/
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)      570 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/opensesame_plugins/pygaze_log/info.yaml
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     1707 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/opensesame_plugins/pygaze_log/pygaze_log.py
-drwxrwxr-x   0 ha21245   (1001) ha21245   (1001)        0 2022-08-17 10:24:05.525275 python-pygaze-0.7.5a5/opensesame_plugins/pygaze_start_recording/
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)      215 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/opensesame_plugins/pygaze_start_recording/info.yaml
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     1538 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/opensesame_plugins/pygaze_start_recording/pygaze_start_recording.py
-drwxrwxr-x   0 ha21245   (1001) ha21245   (1001)        0 2022-08-17 10:24:05.525275 python-pygaze-0.7.5a5/opensesame_plugins/pygaze_stop_recording/
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)      214 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/opensesame_plugins/pygaze_stop_recording/info.yaml
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     1629 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/opensesame_plugins/pygaze_stop_recording/pygaze_stop_recording.py
-drwxrwxr-x   0 ha21245   (1001) ha21245   (1001)        0 2022-08-17 10:24:05.525275 python-pygaze-0.7.5a5/opensesame_plugins/pygaze_wait/
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)      327 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/opensesame_plugins/pygaze_wait/info.yaml
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     2283 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/opensesame_plugins/pygaze_wait/pygaze_wait.py
-drwxrwxr-x   0 ha21245   (1001) ha21245   (1001)        0 2022-08-17 10:24:05.529275 python-pygaze-0.7.5a5/pygaze/
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     2219 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/__init__.py
-drwxrwxr-x   0 ha21245   (1001) ha21245   (1001)        0 2022-08-17 10:24:05.529275 python-pygaze-0.7.5a5/pygaze/_display/
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)      930 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_display/__init__.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     5214 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_display/basedisplay.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     2938 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_display/osdisplay.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     4012 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_display/psychopydisplay.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     4680 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_display/pygamedisplay.py
-drwxrwxr-x   0 ha21245   (1001) ha21245   (1001)        0 2022-08-17 10:24:05.533275 python-pygaze-0.7.5a5/pygaze/_eyetracker/
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)      930 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_eyetracker/__init__.py
-drwxrwxr-x   0 ha21245   (1001) ha21245   (1001)        0 2022-08-17 10:24:05.537275 python-pygaze-0.7.5a5/pygaze/_eyetracker/alea/
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)    15360 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_eyetracker/alea/CEtAPI.dll
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)    19456 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_eyetracker/alea/CEtAPIx64.dll
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)    86528 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_eyetracker/alea/EtApi.dll
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)    11357 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_eyetracker/alea/LICENSE
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     3534 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_eyetracker/alea/README.md
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)      297 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_eyetracker/alea/__init__.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)    73900 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_eyetracker/alea/alea.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)    22361 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_eyetracker/baseeyetracker.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)    20178 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_eyetracker/eyelinkgraphics.py
-drwxrwxr-x   0 ha21245   (1001) ha21245   (1001)        0 2022-08-17 10:24:05.537275 python-pygaze-0.7.5a5/pygaze/_eyetracker/eyelogic/
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)    11329 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_eyetracker/eyelogic/ELApi.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     1094 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_eyetracker/eyelogic/__init__.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     2383 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_eyetracker/iViewXAPI.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)    37904 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_eyetracker/libalea.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     7778 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_eyetracker/libdumbdummy.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)    14469 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_eyetracker/libdummytracker.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)    42188 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_eyetracker/libeyelink.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)    33328 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_eyetracker/libeyelogic.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)    42349 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_eyetracker/libeyetribe.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)    47636 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_eyetracker/libopengaze.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)    47545 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_eyetracker/libsmi.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)    51442 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_eyetracker/libtobii.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)    27139 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_eyetracker/libtobiiglasses.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)    71836 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_eyetracker/libtobiilegacy.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)    52906 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_eyetracker/opengaze.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)    70200 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_eyetracker/pytribe.py
-drwxrwxr-x   0 ha21245   (1001) ha21245   (1001)        0 2022-08-17 10:24:05.537275 python-pygaze-0.7.5a5/pygaze/_eyetracker/tobiiglasses/
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)        0 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_eyetracker/tobiiglasses/__init__.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)    12710 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_eyetracker/tobiiglasses/tobiiglassescontroller.py
-drwxrwxr-x   0 ha21245   (1001) ha21245   (1001)        0 2022-08-17 10:24:05.537275 python-pygaze-0.7.5a5/pygaze/_joystick/
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)      930 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_joystick/__init__.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     9247 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_joystick/basejoystick.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)    14470 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_joystick/pygamejoystick.py
-drwxrwxr-x   0 ha21245   (1001) ha21245   (1001)        0 2022-08-17 10:24:05.537275 python-pygaze-0.7.5a5/pygaze/_keyboard/
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)      930 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_keyboard/__init__.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     5248 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_keyboard/basekeyboard.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     3068 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_keyboard/oskeyboard.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     4552 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_keyboard/psychopykeyboard.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     4424 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_keyboard/pygamekeyboard.py
-drwxrwxr-x   0 ha21245   (1001) ha21245   (1001)        0 2022-08-17 10:24:05.537275 python-pygaze-0.7.5a5/pygaze/_logfile/
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)      930 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_logfile/__init__.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     3346 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_logfile/baselogfile.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     2770 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_logfile/logfile.py
-drwxrwxr-x   0 ha21245   (1001) ha21245   (1001)        0 2022-08-17 10:24:05.537275 python-pygaze-0.7.5a5/pygaze/_misc/
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)      930 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_misc/__init__.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     3888 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_misc/misc.py
-drwxrwxr-x   0 ha21245   (1001) ha21245   (1001)        0 2022-08-17 10:24:05.537275 python-pygaze-0.7.5a5/pygaze/_mouse/
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)      930 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_mouse/__init__.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     6902 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_mouse/basemouse.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     4134 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_mouse/osmouse.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     4414 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_mouse/psychopymouse.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     4345 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_mouse/pygamemouse.py
-drwxrwxr-x   0 ha21245   (1001) ha21245   (1001)        0 2022-08-17 10:24:05.541275 python-pygaze-0.7.5a5/pygaze/_screen/
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)      929 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_screen/__init__.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)    13678 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_screen/basescreen.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)    10110 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_screen/osscreen.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)    25745 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_screen/psychopyscreen.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)    24063 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_screen/pygamescreen.py
-drwxrwxr-x   0 ha21245   (1001) ha21245   (1001)        0 2022-08-17 10:24:05.541275 python-pygaze-0.7.5a5/pygaze/_sound/
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)      930 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_sound/__init__.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     5113 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_sound/basesound.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     7503 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_sound/pygamesound.py
-drwxrwxr-x   0 ha21245   (1001) ha21245   (1001)        0 2022-08-17 10:24:05.541275 python-pygaze-0.7.5a5/pygaze/_time/
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)      930 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_time/__init__.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     3709 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_time/basetime.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     2415 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_time/ostime.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     2563 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_time/psychopytime.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     2867 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/_time/pygametime.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     6424 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/defaults.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     1858 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/display.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     6243 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/eyetracker.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     1654 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/joystick.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     1941 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/keyboard.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     1138 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/libgazecon.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     1101 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/libinput.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)      990 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/liblog.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     1041 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/libscreen.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     1025 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/libsound.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     2716 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/libtime.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     1449 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/logfile.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     1875 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/mouse.py
-drwxrwxr-x   0 ha21245   (1001) ha21245   (1001)        0 2022-08-17 10:24:05.541275 python-pygaze-0.7.5a5/pygaze/plugins/
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)      930 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/plugins/__init__.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     4365 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/plugins/aoi.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     8016 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/plugins/frl.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     5351 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/plugins/gazecursor.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     2200 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/py3compat.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     2926 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/screen.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     1793 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/settings.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     1667 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/sound.py
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     1822 2022-08-17 10:18:14.000000 python-pygaze-0.7.5a5/pygaze/time.py
-drwxrwxr-x   0 ha21245   (1001) ha21245   (1001)        0 2022-08-17 10:24:05.541275 python-pygaze-0.7.5a5/python_pygaze.egg-info/
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     3223 2022-08-17 10:24:05.000000 python-pygaze-0.7.5a5/python_pygaze.egg-info/PKG-INFO
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)     3322 2022-08-17 10:24:05.000000 python-pygaze-0.7.5a5/python_pygaze.egg-info/SOURCES.txt
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)        1 2022-08-17 10:24:05.000000 python-pygaze-0.7.5a5/python_pygaze.egg-info/dependency_links.txt
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)        7 2022-08-17 10:24:05.000000 python-pygaze-0.7.5a5/python_pygaze.egg-info/top_level.txt
--rw-rw-r--   0 ha21245   (1001) ha21245   (1001)       67 2022-08-17 10:24:05.541275 python-pygaze-0.7.5a5/setup.cfg
--rwxrwxr-x   0 ha21245   (1001) ha21245   (1001)     3287 2022-08-17 10:23:30.000000 python-pygaze-0.7.5a5/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 09:53:19.219373 python-pygaze-0.7.6/
+-rwxrwxrwx   0 root         (0) root         (0)    35821 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/COPYING.txt
+-rwxrwxrwx   0 root         (0) root         (0)      112 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)     2749 2023-04-13 09:53:19.219633 python-pygaze-0.7.6/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2125 2023-04-13 09:28:55.000000 python-pygaze-0.7.6/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 09:53:19.120850 python-pygaze-0.7.6/opensesame_plugins/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 09:53:19.126766 python-pygaze-0.7.6/opensesame_plugins/artwork/
+-rwxrwxrwx   0 root         (0) root         (0)   709124 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/opensesame_plugins/artwork/icons.svg
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 09:53:19.132966 python-pygaze-0.7.6/opensesame_plugins/pygaze_drift_correct/
+-rwxrwxrwx   0 root         (0) root         (0)     1159 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/opensesame_plugins/pygaze_drift_correct/info.yaml
+-rwxrwxrwx   0 root         (0) root         (0)     3538 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/opensesame_plugins/pygaze_drift_correct/pygaze_drift_correct.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 09:53:19.133956 python-pygaze-0.7.6/opensesame_plugins/pygaze_init/
+-rwxrwxrwx   0 root         (0) root         (0)     3331 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/opensesame_plugins/pygaze_init/info.yaml
+-rwxrwxrwx   0 root         (0) root         (0)     9885 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/opensesame_plugins/pygaze_init/pygaze_init.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 09:53:19.134897 python-pygaze-0.7.6/opensesame_plugins/pygaze_log/
+-rwxrwxrwx   0 root         (0) root         (0)      570 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/opensesame_plugins/pygaze_log/info.yaml
+-rwxrwxrwx   0 root         (0) root         (0)     1707 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/opensesame_plugins/pygaze_log/pygaze_log.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 09:53:19.136040 python-pygaze-0.7.6/opensesame_plugins/pygaze_start_recording/
+-rwxrwxrwx   0 root         (0) root         (0)      215 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/opensesame_plugins/pygaze_start_recording/info.yaml
+-rwxrwxrwx   0 root         (0) root         (0)     1538 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/opensesame_plugins/pygaze_start_recording/pygaze_start_recording.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 09:53:19.137115 python-pygaze-0.7.6/opensesame_plugins/pygaze_stop_recording/
+-rwxrwxrwx   0 root         (0) root         (0)      214 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/opensesame_plugins/pygaze_stop_recording/info.yaml
+-rwxrwxrwx   0 root         (0) root         (0)     1629 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/opensesame_plugins/pygaze_stop_recording/pygaze_stop_recording.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 09:53:19.138069 python-pygaze-0.7.6/opensesame_plugins/pygaze_wait/
+-rwxrwxrwx   0 root         (0) root         (0)      327 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/opensesame_plugins/pygaze_wait/info.yaml
+-rwxrwxrwx   0 root         (0) root         (0)     2283 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/opensesame_plugins/pygaze_wait/pygaze_wait.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 09:53:19.147853 python-pygaze-0.7.6/pygaze/
+-rwxrwxrwx   0 root         (0) root         (0)     2217 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 09:53:19.150659 python-pygaze-0.7.6/pygaze/_display/
+-rwxrwxrwx   0 root         (0) root         (0)      930 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_display/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5214 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_display/basedisplay.py
+-rwxrwxrwx   0 root         (0) root         (0)     2938 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_display/osdisplay.py
+-rwxrwxrwx   0 root         (0) root         (0)     4012 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_display/psychopydisplay.py
+-rwxrwxrwx   0 root         (0) root         (0)     4680 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_display/pygamedisplay.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 09:53:19.164535 python-pygaze-0.7.6/pygaze/_eyetracker/
+-rwxrwxrwx   0 root         (0) root         (0)      930 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 09:53:19.169741 python-pygaze-0.7.6/pygaze/_eyetracker/alea/
+-rwxrwxrwx   0 root         (0) root         (0)    15360 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/alea/CEtAPI.dll
+-rwxrwxrwx   0 root         (0) root         (0)    19456 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/alea/CEtAPIx64.dll
+-rwxrwxrwx   0 root         (0) root         (0)    86528 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/alea/EtApi.dll
+-rwxrwxrwx   0 root         (0) root         (0)    11357 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/alea/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     3534 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/alea/README.md
+-rwxrwxrwx   0 root         (0) root         (0)      297 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/alea/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    73900 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/alea/alea.py
+-rwxrwxrwx   0 root         (0) root         (0)    22361 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/baseeyetracker.py
+-rwxrwxrwx   0 root         (0) root         (0)    21683 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/eyelinkgraphics.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 09:53:19.198564 python-pygaze-0.7.6/pygaze/_eyetracker/eyelogic/
+-rwxrwxrwx   0 root         (0) root         (0)   439808 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/eyelogic/ELApi.dll
+-rwxrwxrwx   0 root         (0) root         (0)    11329 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/eyelogic/ELApi.py
+-rwxrwxrwx   0 root         (0) root         (0)   177152 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/eyelogic/ELApi32.dll
+-rwxrwxrwx   0 root         (0) root         (0)   170496 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/eyelogic/ELCApi.dll
+-rwxrwxrwx   0 root         (0) root         (0)    29696 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/eyelogic/ELCApi32.dll
+-rwxrwxrwx   0 root         (0) root         (0)     1094 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/eyelogic/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)   332568 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/eyelogic/concrt140.dll
+-rwxrwxrwx   0 root         (0) root         (0)   627992 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/eyelogic/msvcp140.dll
+-rwxrwxrwx   0 root         (0) root         (0)    31512 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/eyelogic/msvcp140_1.dll
+-rwxrwxrwx   0 root         (0) root         (0)   206104 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/eyelogic/msvcp140_2.dll
+-rwxrwxrwx   0 root         (0) root         (0)   366872 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/eyelogic/vccorlib140.dll
+-rwxrwxrwx   0 root         (0) root         (0)    85784 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/eyelogic/vcruntime140.dll
+-rwxrwxrwx   0 root         (0) root         (0)     2383 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/iViewXAPI.py
+-rwxrwxrwx   0 root         (0) root         (0)    37904 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/libalea.py
+-rwxrwxrwx   0 root         (0) root         (0)     7778 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/libdumbdummy.py
+-rwxrwxrwx   0 root         (0) root         (0)    14469 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/libdummytracker.py
+-rwxrwxrwx   0 root         (0) root         (0)    42188 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/libeyelink.py
+-rwxrwxrwx   0 root         (0) root         (0)    33328 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/libeyelogic.py
+-rwxrwxrwx   0 root         (0) root         (0)    42349 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/libeyetribe.py
+-rwxrwxrwx   0 root         (0) root         (0)    47636 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/libopengaze.py
+-rwxrwxrwx   0 root         (0) root         (0)    47545 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/libsmi.py
+-rwxrwxrwx   0 root         (0) root         (0)    51646 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/libtobii.py
+-rwxrwxrwx   0 root         (0) root         (0)    27139 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/libtobiiglasses.py
+-rwxrwxrwx   0 root         (0) root         (0)    71836 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/libtobiilegacy.py
+-rwxrwxrwx   0 root         (0) root         (0)    53085 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/opengaze.py
+-rwxrwxrwx   0 root         (0) root         (0)    70200 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/pytribe.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 09:53:19.200143 python-pygaze-0.7.6/pygaze/_eyetracker/tobiiglasses/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/tobiiglasses/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    12710 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_eyetracker/tobiiglasses/tobiiglassescontroller.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 09:53:19.201921 python-pygaze-0.7.6/pygaze/_joystick/
+-rwxrwxrwx   0 root         (0) root         (0)      930 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_joystick/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     9247 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_joystick/basejoystick.py
+-rwxrwxrwx   0 root         (0) root         (0)    14470 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_joystick/pygamejoystick.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 09:53:19.204863 python-pygaze-0.7.6/pygaze/_keyboard/
+-rwxrwxrwx   0 root         (0) root         (0)      930 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_keyboard/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5248 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_keyboard/basekeyboard.py
+-rwxrwxrwx   0 root         (0) root         (0)     3068 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_keyboard/oskeyboard.py
+-rwxrwxrwx   0 root         (0) root         (0)     4552 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_keyboard/psychopykeyboard.py
+-rwxrwxrwx   0 root         (0) root         (0)     4424 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_keyboard/pygamekeyboard.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 09:53:19.206501 python-pygaze-0.7.6/pygaze/_logfile/
+-rwxrwxrwx   0 root         (0) root         (0)      930 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_logfile/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3346 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_logfile/baselogfile.py
+-rwxrwxrwx   0 root         (0) root         (0)     2770 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_logfile/logfile.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 09:53:19.207374 python-pygaze-0.7.6/pygaze/_misc/
+-rwxrwxrwx   0 root         (0) root         (0)      930 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_misc/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3888 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_misc/misc.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 09:53:19.209533 python-pygaze-0.7.6/pygaze/_mouse/
+-rwxrwxrwx   0 root         (0) root         (0)      930 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_mouse/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6902 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_mouse/basemouse.py
+-rwxrwxrwx   0 root         (0) root         (0)     4134 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_mouse/osmouse.py
+-rwxrwxrwx   0 root         (0) root         (0)     4414 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_mouse/psychopymouse.py
+-rwxrwxrwx   0 root         (0) root         (0)     4345 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_mouse/pygamemouse.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 09:53:19.211913 python-pygaze-0.7.6/pygaze/_screen/
+-rwxrwxrwx   0 root         (0) root         (0)      929 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_screen/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    13678 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_screen/basescreen.py
+-rwxrwxrwx   0 root         (0) root         (0)    10110 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_screen/osscreen.py
+-rwxrwxrwx   0 root         (0) root         (0)    25745 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_screen/psychopyscreen.py
+-rwxrwxrwx   0 root         (0) root         (0)    24063 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_screen/pygamescreen.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 09:53:19.213304 python-pygaze-0.7.6/pygaze/_sound/
+-rwxrwxrwx   0 root         (0) root         (0)      930 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_sound/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5113 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_sound/basesound.py
+-rwxrwxrwx   0 root         (0) root         (0)     7503 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_sound/pygamesound.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 09:53:19.215610 python-pygaze-0.7.6/pygaze/_time/
+-rwxrwxrwx   0 root         (0) root         (0)      930 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_time/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3709 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_time/basetime.py
+-rwxrwxrwx   0 root         (0) root         (0)     2415 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_time/ostime.py
+-rwxrwxrwx   0 root         (0) root         (0)     2563 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_time/psychopytime.py
+-rwxrwxrwx   0 root         (0) root         (0)     2867 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/_time/pygametime.py
+-rwxrwxrwx   0 root         (0) root         (0)     6424 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/defaults.py
+-rwxrwxrwx   0 root         (0) root         (0)     1858 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/display.py
+-rwxrwxrwx   0 root         (0) root         (0)     6243 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/eyetracker.py
+-rwxrwxrwx   0 root         (0) root         (0)     1654 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/joystick.py
+-rwxrwxrwx   0 root         (0) root         (0)     1941 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/keyboard.py
+-rwxrwxrwx   0 root         (0) root         (0)     1138 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/libgazecon.py
+-rwxrwxrwx   0 root         (0) root         (0)     1101 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/libinput.py
+-rwxrwxrwx   0 root         (0) root         (0)      990 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/liblog.py
+-rwxrwxrwx   0 root         (0) root         (0)     1041 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/libscreen.py
+-rwxrwxrwx   0 root         (0) root         (0)     1025 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/libsound.py
+-rwxrwxrwx   0 root         (0) root         (0)     2716 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/libtime.py
+-rwxrwxrwx   0 root         (0) root         (0)     1449 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/logfile.py
+-rwxrwxrwx   0 root         (0) root         (0)     1875 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/mouse.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 09:53:19.217326 python-pygaze-0.7.6/pygaze/plugins/
+-rwxrwxrwx   0 root         (0) root         (0)      930 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/plugins/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4365 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/plugins/aoi.py
+-rwxrwxrwx   0 root         (0) root         (0)     8016 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/plugins/frl.py
+-rwxrwxrwx   0 root         (0) root         (0)     5351 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/plugins/gazecursor.py
+-rwxrwxrwx   0 root         (0) root         (0)     2200 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/py3compat.py
+-rwxrwxrwx   0 root         (0) root         (0)     2926 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/screen.py
+-rwxrwxrwx   0 root         (0) root         (0)     1793 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/settings.py
+-rwxrwxrwx   0 root         (0) root         (0)     1667 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/sound.py
+-rwxrwxrwx   0 root         (0) root         (0)     1822 2023-04-13 09:25:51.000000 python-pygaze-0.7.6/pygaze/time.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 09:53:19.219025 python-pygaze-0.7.6/python_pygaze.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     2749 2023-04-13 09:53:19.000000 python-pygaze-0.7.6/python_pygaze.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     3750 2023-04-13 09:53:19.000000 python-pygaze-0.7.6/python_pygaze.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-13 09:53:19.000000 python-pygaze-0.7.6/python_pygaze.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        7 2023-04-13 09:53:19.000000 python-pygaze-0.7.6/python_pygaze.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       67 2023-04-13 09:53:19.220228 python-pygaze-0.7.6/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     3288 2023-04-13 09:53:04.000000 python-pygaze-0.7.6/setup.py
```

### Comparing `python-pygaze-0.7.5a5/PKG-INFO` & `python-pygaze-0.7.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,74 +1,73 @@
 Metadata-Version: 2.1
 Name: python-pygaze
-Version: 0.7.5a5
+Version: 0.7.6
 Summary: A Python library for eye tracking
-Home-page: http://www.pygaze.org/
+Home-page: https://www.pygaze.org/
 Author: Edwin Dalmaijer
 Author-email: edwin@dalmaijer.org
-License: UNKNOWN
-Description: # PyGaze - the open-source toolbox for eye tracking
-        
-        *Copyright 2013 - 2022, Edwin Dalmaijer, Sebastiaan Mathôt, and contributors*
-        
-        For more information, see: <https://www.pygaze.org/contributors>
-        
-        
-        ## Citation
-        
-        * Dalmaijer, E.S., Mathôt, S., & Van der Stigchel, S. (2013). PyGaze: an open-source, cross-platform toolbox for minimal-effort programming of eye tracking experiments. *Behaviour Research Methods*. doi:[10.3758/s13428-013-0422-2](http://link.springer.com/article/10.3758%2Fs13428-013-0422-2)
-        
-        
-        ## Documentation
-        
-        - <https://pygaze.org/>
-        - <https://osdoc.cogsci.nl/manual/eyetracking/pygaze/>
-        
-        
-        ## Installation
-        
-        ```
-        pip install python-pygaze
-        ```
-        
-        
-        ## License
-        
-        PyGaze is open source software and therefore free to use and modify at will.
-        Warranty, however, is NOT given. If this software fails, causes your computer
-        to blow up, your spouse to leave you, your toilet to clog and/or the entire
-        supply of nuclear missles on earth to launch, or anything else that you might
-        want to blame on us, the author(s) CANNOT IN ANY WAY be held responsible.
-        
-        PyGaze was released under the GNU Public License (version 3), of which you
-        should have received a copy of together with the software:
-        
-            PyGaze is a Python package for easily creating gaze contingent experiments
-            or other software (as well as non-gaze contingent experiments/software)
-            Copyright (C) 2012-2020 Edwin S. Dalmaijer
-        
-            This program is free software: you can redistribute it and/or modify
-            it under the terms of the GNU General Public License as published by
-            the Free Software Foundation, either version 3 of the License, or
-            (at your option) any later version.
-        
-            This program is distributed in the hope that it will be useful,
-            but WITHOUT ANY WARRANTY; without even the implied warranty of
-            MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-            GNU General Public License for more details.
-        
-            You should have received a copy of the GNU General Public License
-            along with this program.  If not, see <http://www.gnu.org/licenses/>
-        
-        I hope PyGaze proves to be helpful to you!
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Environment :: MacOS X
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: COPYING.txt
+
+# PyGaze - the open-source toolbox for eye tracking
+
+*Copyright 2013 - 2023, Edwin Dalmaijer, Sebastiaan Mathôt, and contributors*
+
+For more information, see: <https://www.pygaze.org/contributors>
+
+
+## Citation
+
+* Dalmaijer, E.S., Mathôt, S., & Van der Stigchel, S. (2013). PyGaze: an open-source, cross-platform toolbox for minimal-effort programming of eye tracking experiments. *Behaviour Research Methods*. doi:[10.3758/s13428-013-0422-2](https://doi.org/10.3758/s13428-013-0422-2)
+
+
+## Documentation
+
+- <https://pygaze.org/>
+- <https://osdoc.cogsci.nl/manual/eyetracking/pygaze/>
+
+
+## Installation
+
+```
+pip install python-pygaze
+```
+
+
+## License
+
+PyGaze is open source software and therefore free to use and modify at will.
+Warranty, however, is NOT given. If this software fails, causes your computer
+to blow up, your spouse to leave you, your toilet to clog and/or the entire
+supply of nuclear missles on earth to launch, or anything else that you might
+want to blame on us, the author(s) CANNOT IN ANY WAY be held responsible.
+
+PyGaze was released under the GNU Public License (version 3), of which you
+should have received a copy of together with the software:
+
+    PyGaze is a Python package for easily creating gaze contingent experiments
+    or other software (as well as non-gaze contingent experiments/software)
+    Copyright (C) 2012-2023 Edwin S. Dalmaijer
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <http://www.gnu.org/licenses/>
+
+I hope PyGaze proves to be helpful to you!
```

### Comparing `python-pygaze-0.7.5a5/README.md` & `python-pygaze-0.7.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # PyGaze - the open-source toolbox for eye tracking
 
-*Copyright 2013 - 2022, Edwin Dalmaijer, Sebastiaan Mathôt, and contributors*
+*Copyright 2013 - 2023, Edwin Dalmaijer, Sebastiaan Mathôt, and contributors*
 
 For more information, see: <https://www.pygaze.org/contributors>
 
 
 ## Citation
 
-* Dalmaijer, E.S., Mathôt, S., & Van der Stigchel, S. (2013). PyGaze: an open-source, cross-platform toolbox for minimal-effort programming of eye tracking experiments. *Behaviour Research Methods*. doi:[10.3758/s13428-013-0422-2](http://link.springer.com/article/10.3758%2Fs13428-013-0422-2)
+* Dalmaijer, E.S., Mathôt, S., & Van der Stigchel, S. (2013). PyGaze: an open-source, cross-platform toolbox for minimal-effort programming of eye tracking experiments. *Behaviour Research Methods*. doi:[10.3758/s13428-013-0422-2](https://doi.org/10.3758/s13428-013-0422-2)
 
 
 ## Documentation
 
 - <https://pygaze.org/>
 - <https://osdoc.cogsci.nl/manual/eyetracking/pygaze/>
 
@@ -32,15 +32,15 @@
 want to blame on us, the author(s) CANNOT IN ANY WAY be held responsible.
 
 PyGaze was released under the GNU Public License (version 3), of which you
 should have received a copy of together with the software:
 
     PyGaze is a Python package for easily creating gaze contingent experiments
     or other software (as well as non-gaze contingent experiments/software)
-    Copyright (C) 2012-2020 Edwin S. Dalmaijer
+    Copyright (C) 2012-2023 Edwin S. Dalmaijer
 
     This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
     This program is distributed in the hope that it will be useful,
```

### Comparing `python-pygaze-0.7.5a5/opensesame_plugins/artwork/icons.svg` & `python-pygaze-0.7.6/opensesame_plugins/artwork/icons.svg`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/opensesame_plugins/pygaze_drift_correct/info.yaml` & `python-pygaze-0.7.6/opensesame_plugins/pygaze_drift_correct/info.yaml`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/opensesame_plugins/pygaze_drift_correct/pygaze_drift_correct.py` & `python-pygaze-0.7.6/opensesame_plugins/pygaze_drift_correct/pygaze_drift_correct.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/opensesame_plugins/pygaze_init/info.yaml` & `python-pygaze-0.7.6/opensesame_plugins/pygaze_init/info.yaml`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/opensesame_plugins/pygaze_init/pygaze_init.py` & `python-pygaze-0.7.6/opensesame_plugins/pygaze_init/pygaze_init.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/opensesame_plugins/pygaze_log/info.yaml` & `python-pygaze-0.7.6/opensesame_plugins/pygaze_log/info.yaml`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/opensesame_plugins/pygaze_log/pygaze_log.py` & `python-pygaze-0.7.6/opensesame_plugins/pygaze_log/pygaze_log.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/opensesame_plugins/pygaze_start_recording/pygaze_start_recording.py` & `python-pygaze-0.7.6/opensesame_plugins/pygaze_start_recording/pygaze_start_recording.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/opensesame_plugins/pygaze_stop_recording/pygaze_stop_recording.py` & `python-pygaze-0.7.6/opensesame_plugins/pygaze_stop_recording/pygaze_stop_recording.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/opensesame_plugins/pygaze_wait/pygaze_wait.py` & `python-pygaze-0.7.6/opensesame_plugins/pygaze_wait/pygaze_wait.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/__init__.py` & `python-pygaze-0.7.6/pygaze/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 from pygaze.py3compat import *
 from pygaze.settings import settings
 from distutils.version import StrictVersion
 import sys
 import os
 
-__version__ = version = "0.7.5a5"
+__version__ = version = "0.7.6"
 strict_version = StrictVersion(__version__)
 # The version without the prerelease (if any): e.g. 3.0.0
 main_version = ".".join([str(i) for i in strict_version.version])
 # The version following the debian convention: e.g. 3.0.0~a1
 if strict_version.prerelease is None:
     deb_version = main_version
 else:
```

### Comparing `python-pygaze-0.7.5a5/pygaze/_display/__init__.py` & `python-pygaze-0.7.6/pygaze/_display/__init__.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_display/basedisplay.py` & `python-pygaze-0.7.6/pygaze/_display/basedisplay.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_display/osdisplay.py` & `python-pygaze-0.7.6/pygaze/_display/osdisplay.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_display/psychopydisplay.py` & `python-pygaze-0.7.6/pygaze/_display/psychopydisplay.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_display/pygamedisplay.py` & `python-pygaze-0.7.6/pygaze/_display/pygamedisplay.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_eyetracker/__init__.py` & `python-pygaze-0.7.6/pygaze/_eyetracker/__init__.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_eyetracker/alea/CEtAPI.dll` & `python-pygaze-0.7.6/pygaze/_eyetracker/alea/CEtAPI.dll`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_eyetracker/alea/CEtAPIx64.dll` & `python-pygaze-0.7.6/pygaze/_eyetracker/alea/CEtAPIx64.dll`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_eyetracker/alea/EtApi.dll` & `python-pygaze-0.7.6/pygaze/_eyetracker/alea/EtApi.dll`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_eyetracker/alea/LICENSE` & `python-pygaze-0.7.6/pygaze/_eyetracker/alea/LICENSE`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_eyetracker/alea/README.md` & `python-pygaze-0.7.6/pygaze/_eyetracker/alea/README.md`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_eyetracker/alea/alea.py` & `python-pygaze-0.7.6/pygaze/_eyetracker/alea/alea.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_eyetracker/baseeyetracker.py` & `python-pygaze-0.7.6/pygaze/_eyetracker/baseeyetracker.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_eyetracker/eyelinkgraphics.py` & `python-pygaze-0.7.6/pygaze/_eyetracker/eyelinkgraphics.py`

 * *Files 5% similar despite different names*

```diff
@@ -534,28 +534,51 @@
             except:
                 pass
         # If the buffer is full, push it to the display.
         if line == totlines:
             self.scale = totlines/320.0
             self._size = int(self.scale*self.size[0]), int(
                 self.scale*self.size[1])
+
+            # Get buffer as bytes. From Python 3.2, `tostring` was renamed 
+            # `tobytes`. Then, from Python 3.9, `tostring` was dropped 
+            # completely. While the newer function name makes more sense (as 
+            # it returns a byte representation), it simply does not exist if 
+            # we're on Python versions prior to 3.2. Hence the following 
+            # awkward way of checking if the function exists, and then to call
+            # it if it does. We call the function by its old name if the new
+            # name doesn't exist. This is awkward, but a lot less awkward than
+            # my previous solution of creating a child class of array.array 
+            # with the single purpose of defining `tostring` with a call to
+            # `tobytes`. (Decided against that as it would change the class,
+            # and that would break any code that checks whether a variable's 
+            # type is array.array.)
+            # Do you think this is insane, and that we should just use the 
+            # newer and more sensible `tobytes`? I've seen lab computers that 
+            # run Python 2.4 on Windows XP. I'm not ready to have the 
+            # conversation that they should consider upgrading. (Also, maybe
+            # they have an ancient EyeLink that requires such an old system.
+            # You don't know their life!)
+            if hasattr(self.imagebuffer, "tobytes"):
+                baby_b_buffer = self.imagebuffer.tobytes()
+            else:
+                baby_b_buffer = self.imagebuffer.tostring()
+
             # Convert the image buffer to a pygame image, save it ...
             try:
                 # This is based on PyLink >= 1.1
                 self.cam_img = pygame.image.fromstring(
-                    self.imagebuffer.tostring(), self._size, 'RGBX'
-                )
+                    baby_b_buffer, self._size, 'RGBX')
             except ValueError:
                 # This is for PyLink <= 1.0. This try ... except construction
                 # is a hack. It would be better to understand the difference
                 # between these two versions.
                 try:
                     self.cam_img = pygame.image.fromstring(
-                        self.imagebuffer.tostring(), self.size, 'RGBX'
-                    )
+                        baby_b_buffer, self.size, 'RGBX')
                     self.scale = 1.0
                 # In some cases, the conversion fails because the imagebuffer
                 # is too long to begin with. Therefore, we need to make sure
                 # that it's cleared.
                 except ValueError:
                     print('EyelinkGraphics.draw_image_line(): clearing invalid imagebuffer')
                     self.imagebuffer = self.new_array()
```

### Comparing `python-pygaze-0.7.5a5/pygaze/_eyetracker/eyelogic/ELApi.py` & `python-pygaze-0.7.6/pygaze/_eyetracker/eyelogic/ELApi.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_eyetracker/eyelogic/__init__.py` & `python-pygaze-0.7.6/pygaze/_eyetracker/eyelogic/__init__.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_eyetracker/iViewXAPI.py` & `python-pygaze-0.7.6/pygaze/_eyetracker/iViewXAPI.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_eyetracker/libalea.py` & `python-pygaze-0.7.6/pygaze/_eyetracker/libalea.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_eyetracker/libdumbdummy.py` & `python-pygaze-0.7.6/pygaze/_eyetracker/libdumbdummy.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_eyetracker/libdummytracker.py` & `python-pygaze-0.7.6/pygaze/_eyetracker/libdummytracker.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_eyetracker/libeyelink.py` & `python-pygaze-0.7.6/pygaze/_eyetracker/libeyelink.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_eyetracker/libeyelogic.py` & `python-pygaze-0.7.6/pygaze/_eyetracker/libeyelogic.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_eyetracker/libeyetribe.py` & `python-pygaze-0.7.6/pygaze/_eyetracker/libeyetribe.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_eyetracker/libopengaze.py` & `python-pygaze-0.7.6/pygaze/_eyetracker/libopengaze.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_eyetracker/libsmi.py` & `python-pygaze-0.7.6/pygaze/_eyetracker/libsmi.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_eyetracker/libtobii.py` & `python-pygaze-0.7.6/pygaze/_eyetracker/libtobii.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,22 +41,23 @@
 
         # initialize keyboard
         self.kb = Keyboard(keylist=['space', 'escape', 'q'], timeout=1)
 
         self.recording = False
 
         self.screendist = settings.SCREENDIST
-
-        if hasattr(settings, 'TRACKERSERIALNUMBER'):
-            # Search for a specific eye tracker
-            self.eyetrackers = [t for t in tr.find_all_eyetrackers() if t.serial_number == settings.TRACKERSERIALNUMBER]
-        else:
-            # Search for all eye trackers (The first one found will be selected)
-            self.eyetrackers = tr.find_all_eyetrackers()
-
+        try:
+            if hasattr(settings, 'TRACKERSERIALNUMBER'):
+                # Search for a specific eye tracker
+                self.eyetrackers = [t for t in tr.find_all_eyetrackers() if t.serial_number == settings.TRACKERSERIALNUMBER]
+            else:
+                # Search for all eye trackers (The first one found will be selected)
+                self.eyetrackers = tr.find_all_eyetrackers()
+        except Exception:
+                self.eyetrackers = tr.find_all_eyetrackers()
         if self.eyetrackers:
             self.eyetracker = self.eyetrackers[0]
         else:
             print("WARNING! libtobii.TobiiProTracker.__init__: no eye trackers found!")
             return
 
         self.LEFT_EYE = 0
@@ -1005,15 +1006,18 @@
         # get valid sample
         prevpos = self.sample()
         while not self.is_valid_sample(prevpos):
             prevpos = self.sample()
         # get starting time, intersample distance, and velocity
         t1 = clock.get_time()
         s = ((prevpos[0] - spos[0])**2 + (prevpos[1] - spos[1])**2)**0.5  # = intersample distance = speed in px/sample
-        v0 = s / (t1 - t0)
+        try:
+            v0 = s / (t1 - t0)
+        except ZeroDivisionError:
+            v0 = s / 1e-20
 
         # run until velocity and acceleration go below threshold
         saccadic = True
         while saccadic:
             # get new sample
             newpos = self.sample()
             t1 = clock.get_time()
```

### Comparing `python-pygaze-0.7.5a5/pygaze/_eyetracker/libtobiiglasses.py` & `python-pygaze-0.7.6/pygaze/_eyetracker/libtobiiglasses.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_eyetracker/libtobiilegacy.py` & `python-pygaze-0.7.6/pygaze/_eyetracker/libtobiilegacy.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_eyetracker/opengaze.py` & `python-pygaze-0.7.6/pygaze/_eyetracker/opengaze.py`

 * *Files 0% similar despite different names*

```diff
@@ -387,16 +387,18 @@
             # Skip further processing if no new message came in.
             if timeout:
                 self._debug_print("socket recv timeout")
                 continue
 
             self._debug_print(r"Raw instring: {}".format(instring))
 
-            # Split the messages (they are separated by '\r\n').
-            messages = instring.split('\r\n')
+            # Split the messages. These should be are separated by '\r\n', but
+            # the safest way to split them is to split them by any newline
+            # character while ignoring the empty messages.
+            messages = [msg for msg in instring.splitlines() if msg.strip()]
 
             # Check if there is currently an unfinished message.
             if self._unfinished:
                 # Combine the currently unfinished message and the
                 # most recent incoming message.
                 messages[0] = copy.copy(self._unfinished) + messages[0]
                 # Reset the unfinished message.
```

### Comparing `python-pygaze-0.7.5a5/pygaze/_eyetracker/pytribe.py` & `python-pygaze-0.7.6/pygaze/_eyetracker/pytribe.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_eyetracker/tobiiglasses/tobiiglassescontroller.py` & `python-pygaze-0.7.6/pygaze/_eyetracker/tobiiglasses/tobiiglassescontroller.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_joystick/__init__.py` & `python-pygaze-0.7.6/pygaze/_joystick/__init__.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_joystick/basejoystick.py` & `python-pygaze-0.7.6/pygaze/_joystick/basejoystick.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_joystick/pygamejoystick.py` & `python-pygaze-0.7.6/pygaze/_joystick/pygamejoystick.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_keyboard/__init__.py` & `python-pygaze-0.7.6/pygaze/_keyboard/__init__.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_keyboard/basekeyboard.py` & `python-pygaze-0.7.6/pygaze/_keyboard/basekeyboard.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_keyboard/oskeyboard.py` & `python-pygaze-0.7.6/pygaze/_keyboard/oskeyboard.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_keyboard/psychopykeyboard.py` & `python-pygaze-0.7.6/pygaze/_keyboard/psychopykeyboard.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_keyboard/pygamekeyboard.py` & `python-pygaze-0.7.6/pygaze/_keyboard/pygamekeyboard.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_logfile/__init__.py` & `python-pygaze-0.7.6/pygaze/_logfile/__init__.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_logfile/baselogfile.py` & `python-pygaze-0.7.6/pygaze/_logfile/baselogfile.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_logfile/logfile.py` & `python-pygaze-0.7.6/pygaze/_logfile/logfile.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_misc/__init__.py` & `python-pygaze-0.7.6/pygaze/_misc/__init__.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_misc/misc.py` & `python-pygaze-0.7.6/pygaze/_misc/misc.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_mouse/__init__.py` & `python-pygaze-0.7.6/pygaze/_mouse/__init__.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_mouse/basemouse.py` & `python-pygaze-0.7.6/pygaze/_mouse/basemouse.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_mouse/osmouse.py` & `python-pygaze-0.7.6/pygaze/_mouse/osmouse.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_mouse/psychopymouse.py` & `python-pygaze-0.7.6/pygaze/_mouse/psychopymouse.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_mouse/pygamemouse.py` & `python-pygaze-0.7.6/pygaze/_mouse/pygamemouse.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_screen/__init__.py` & `python-pygaze-0.7.6/pygaze/_screen/__init__.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_screen/basescreen.py` & `python-pygaze-0.7.6/pygaze/_screen/basescreen.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_screen/osscreen.py` & `python-pygaze-0.7.6/pygaze/_screen/osscreen.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_screen/psychopyscreen.py` & `python-pygaze-0.7.6/pygaze/_screen/psychopyscreen.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_screen/pygamescreen.py` & `python-pygaze-0.7.6/pygaze/_screen/pygamescreen.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_sound/__init__.py` & `python-pygaze-0.7.6/pygaze/_sound/__init__.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_sound/basesound.py` & `python-pygaze-0.7.6/pygaze/_sound/basesound.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_sound/pygamesound.py` & `python-pygaze-0.7.6/pygaze/_sound/pygamesound.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_time/__init__.py` & `python-pygaze-0.7.6/pygaze/_time/__init__.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_time/basetime.py` & `python-pygaze-0.7.6/pygaze/_time/basetime.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_time/ostime.py` & `python-pygaze-0.7.6/pygaze/_time/ostime.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_time/psychopytime.py` & `python-pygaze-0.7.6/pygaze/_time/psychopytime.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/_time/pygametime.py` & `python-pygaze-0.7.6/pygaze/_time/pygametime.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/defaults.py` & `python-pygaze-0.7.6/pygaze/defaults.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/display.py` & `python-pygaze-0.7.6/pygaze/display.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/eyetracker.py` & `python-pygaze-0.7.6/pygaze/eyetracker.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/joystick.py` & `python-pygaze-0.7.6/pygaze/joystick.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/keyboard.py` & `python-pygaze-0.7.6/pygaze/keyboard.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/libgazecon.py` & `python-pygaze-0.7.6/pygaze/libgazecon.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/libinput.py` & `python-pygaze-0.7.6/pygaze/libinput.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/liblog.py` & `python-pygaze-0.7.6/pygaze/liblog.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/libscreen.py` & `python-pygaze-0.7.6/pygaze/libscreen.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/libsound.py` & `python-pygaze-0.7.6/pygaze/libsound.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/libtime.py` & `python-pygaze-0.7.6/pygaze/libtime.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/logfile.py` & `python-pygaze-0.7.6/pygaze/logfile.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/mouse.py` & `python-pygaze-0.7.6/pygaze/mouse.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/plugins/__init__.py` & `python-pygaze-0.7.6/pygaze/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/plugins/aoi.py` & `python-pygaze-0.7.6/pygaze/plugins/aoi.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/plugins/frl.py` & `python-pygaze-0.7.6/pygaze/plugins/frl.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/plugins/gazecursor.py` & `python-pygaze-0.7.6/pygaze/plugins/gazecursor.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/py3compat.py` & `python-pygaze-0.7.6/pygaze/py3compat.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/screen.py` & `python-pygaze-0.7.6/pygaze/screen.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/settings.py` & `python-pygaze-0.7.6/pygaze/settings.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/sound.py` & `python-pygaze-0.7.6/pygaze/sound.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/pygaze/time.py` & `python-pygaze-0.7.6/pygaze/time.py`

 * *Files identical despite different names*

### Comparing `python-pygaze-0.7.5a5/python_pygaze.egg-info/PKG-INFO` & `python-pygaze-0.7.6/python_pygaze.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,74 +1,73 @@
 Metadata-Version: 2.1
 Name: python-pygaze
-Version: 0.7.5a5
+Version: 0.7.6
 Summary: A Python library for eye tracking
-Home-page: http://www.pygaze.org/
+Home-page: https://www.pygaze.org/
 Author: Edwin Dalmaijer
 Author-email: edwin@dalmaijer.org
-License: UNKNOWN
-Description: # PyGaze - the open-source toolbox for eye tracking
-        
-        *Copyright 2013 - 2022, Edwin Dalmaijer, Sebastiaan Mathôt, and contributors*
-        
-        For more information, see: <https://www.pygaze.org/contributors>
-        
-        
-        ## Citation
-        
-        * Dalmaijer, E.S., Mathôt, S., & Van der Stigchel, S. (2013). PyGaze: an open-source, cross-platform toolbox for minimal-effort programming of eye tracking experiments. *Behaviour Research Methods*. doi:[10.3758/s13428-013-0422-2](http://link.springer.com/article/10.3758%2Fs13428-013-0422-2)
-        
-        
-        ## Documentation
-        
-        - <https://pygaze.org/>
-        - <https://osdoc.cogsci.nl/manual/eyetracking/pygaze/>
-        
-        
-        ## Installation
-        
-        ```
-        pip install python-pygaze
-        ```
-        
-        
-        ## License
-        
-        PyGaze is open source software and therefore free to use and modify at will.
-        Warranty, however, is NOT given. If this software fails, causes your computer
-        to blow up, your spouse to leave you, your toilet to clog and/or the entire
-        supply of nuclear missles on earth to launch, or anything else that you might
-        want to blame on us, the author(s) CANNOT IN ANY WAY be held responsible.
-        
-        PyGaze was released under the GNU Public License (version 3), of which you
-        should have received a copy of together with the software:
-        
-            PyGaze is a Python package for easily creating gaze contingent experiments
-            or other software (as well as non-gaze contingent experiments/software)
-            Copyright (C) 2012-2020 Edwin S. Dalmaijer
-        
-            This program is free software: you can redistribute it and/or modify
-            it under the terms of the GNU General Public License as published by
-            the Free Software Foundation, either version 3 of the License, or
-            (at your option) any later version.
-        
-            This program is distributed in the hope that it will be useful,
-            but WITHOUT ANY WARRANTY; without even the implied warranty of
-            MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-            GNU General Public License for more details.
-        
-            You should have received a copy of the GNU General Public License
-            along with this program.  If not, see <http://www.gnu.org/licenses/>
-        
-        I hope PyGaze proves to be helpful to you!
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Environment :: MacOS X
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: COPYING.txt
+
+# PyGaze - the open-source toolbox for eye tracking
+
+*Copyright 2013 - 2023, Edwin Dalmaijer, Sebastiaan Mathôt, and contributors*
+
+For more information, see: <https://www.pygaze.org/contributors>
+
+
+## Citation
+
+* Dalmaijer, E.S., Mathôt, S., & Van der Stigchel, S. (2013). PyGaze: an open-source, cross-platform toolbox for minimal-effort programming of eye tracking experiments. *Behaviour Research Methods*. doi:[10.3758/s13428-013-0422-2](https://doi.org/10.3758/s13428-013-0422-2)
+
+
+## Documentation
+
+- <https://pygaze.org/>
+- <https://osdoc.cogsci.nl/manual/eyetracking/pygaze/>
+
+
+## Installation
+
+```
+pip install python-pygaze
+```
+
+
+## License
+
+PyGaze is open source software and therefore free to use and modify at will.
+Warranty, however, is NOT given. If this software fails, causes your computer
+to blow up, your spouse to leave you, your toilet to clog and/or the entire
+supply of nuclear missles on earth to launch, or anything else that you might
+want to blame on us, the author(s) CANNOT IN ANY WAY be held responsible.
+
+PyGaze was released under the GNU Public License (version 3), of which you
+should have received a copy of together with the software:
+
+    PyGaze is a Python package for easily creating gaze contingent experiments
+    or other software (as well as non-gaze contingent experiments/software)
+    Copyright (C) 2012-2023 Edwin S. Dalmaijer
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <http://www.gnu.org/licenses/>
+
+I hope PyGaze proves to be helpful to you!
```

### Comparing `python-pygaze-0.7.5a5/python_pygaze.egg-info/SOURCES.txt` & `python-pygaze-0.7.6/python_pygaze.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+COPYING.txt
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 opensesame_plugins/artwork/icons.svg
 opensesame_plugins/pygaze_drift_correct/info.yaml
 opensesame_plugins/pygaze_drift_correct/pygaze_drift_correct.py
@@ -59,16 +60,26 @@
 pygaze/_eyetracker/alea/CEtAPI.dll
 pygaze/_eyetracker/alea/CEtAPIx64.dll
 pygaze/_eyetracker/alea/EtApi.dll
 pygaze/_eyetracker/alea/LICENSE
 pygaze/_eyetracker/alea/README.md
 pygaze/_eyetracker/alea/__init__.py
 pygaze/_eyetracker/alea/alea.py
+pygaze/_eyetracker/eyelogic/ELApi.dll
 pygaze/_eyetracker/eyelogic/ELApi.py
+pygaze/_eyetracker/eyelogic/ELApi32.dll
+pygaze/_eyetracker/eyelogic/ELCApi.dll
+pygaze/_eyetracker/eyelogic/ELCApi32.dll
 pygaze/_eyetracker/eyelogic/__init__.py
+pygaze/_eyetracker/eyelogic/concrt140.dll
+pygaze/_eyetracker/eyelogic/msvcp140.dll
+pygaze/_eyetracker/eyelogic/msvcp140_1.dll
+pygaze/_eyetracker/eyelogic/msvcp140_2.dll
+pygaze/_eyetracker/eyelogic/vccorlib140.dll
+pygaze/_eyetracker/eyelogic/vcruntime140.dll
 pygaze/_eyetracker/tobiiglasses/__init__.py
 pygaze/_eyetracker/tobiiglasses/tobiiglassescontroller.py
 pygaze/_joystick/__init__.py
 pygaze/_joystick/basejoystick.py
 pygaze/_joystick/pygamejoystick.py
 pygaze/_keyboard/__init__.py
 pygaze/_keyboard/basekeyboard.py
```

### Comparing `python-pygaze-0.7.5a5/setup.py` & `python-pygaze-0.7.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 	python_requires=">=3",
 	version=pygaze.__version__,
 	description="A Python library for eye tracking",
 	long_description=get_readme(),
 	long_description_content_type='text/markdown',
 	author="Edwin Dalmaijer",
 	author_email="edwin@dalmaijer.org",
-	url="http://www.pygaze.org/",
+	url="https://www.pygaze.org/",
 	classifiers=[
 		'Development Status :: 4 - Beta',
 		'Intended Audience :: Science/Research',
 		'Topic :: Scientific/Engineering',
 		'Environment :: MacOS X',
 		'Environment :: Win32 (MS Windows)',
 		'Environment :: X11 Applications',
```

