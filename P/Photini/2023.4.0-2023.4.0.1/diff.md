# Comparing `tmp/Photini-2023.4.0.tar.gz` & `tmp/Photini-2023.4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Photini-2023.4.0.tar", last modified: Wed Apr 12 08:05:37 2023, max compression
+gzip compressed data, was "dist/Photini-2023.4.0.1.tar", last modified: Thu Apr 13 09:47:54 2023, max compression
```

## Comparing `Photini-2023.4.0.tar` & `Photini-2023.4.0.1.tar`

### file list

```diff
@@ -1,337 +1,337 @@
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/
--rw-r--r--   0 jim       (1026) users      (100)    15393 2023-04-12 08:03:27.000000 Photini-2023.4.0/CHANGELOG.txt
--rw-r--r--   0 jim       (1026) users      (100)    35147 2023-04-12 08:03:27.000000 Photini-2023.4.0/LICENSE.txt
--rw-r--r--   0 jim       (1026) users      (100)      170 2023-04-12 08:03:27.000000 Photini-2023.4.0/MANIFEST.in
--rw-r--r--   0 jim       (1026) users      (100)    10317 2023-04-12 08:05:37.000000 Photini-2023.4.0/PKG-INFO
--rw-r--r--   0 jim       (1026) users      (100)     7814 2023-04-12 08:03:27.000000 Photini-2023.4.0/README.rst
--rw-r--r--   0 jim       (1026) users      (100)       38 2023-04-12 08:05:37.000000 Photini-2023.4.0/setup.cfg
--rw-r--r--   0 jim       (1026) users      (100)     4362 2023-04-12 08:03:27.000000 Photini-2023.4.0/setup.py
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/Photini.egg-info/
--rw-r--r--   0 jim       (1026) users      (100)    10317 2023-04-12 08:05:36.000000 Photini-2023.4.0/src/Photini.egg-info/PKG-INFO
--rw-r--r--   0 jim       (1026) users      (100)     9110 2023-04-12 08:05:36.000000 Photini-2023.4.0/src/Photini.egg-info/SOURCES.txt
--rw-r--r--   0 jim       (1026) users      (100)        1 2023-04-12 08:05:36.000000 Photini-2023.4.0/src/Photini.egg-info/dependency_links.txt
--rw-r--r--   0 jim       (1026) users      (100)      162 2023-04-12 08:05:36.000000 Photini-2023.4.0/src/Photini.egg-info/entry_points.txt
--rw-r--r--   0 jim       (1026) users      (100)        1 2023-04-12 08:05:36.000000 Photini-2023.4.0/src/Photini.egg-info/not-zip-safe
--rw-r--r--   0 jim       (1026) users      (100)     1044 2023-04-12 08:05:36.000000 Photini-2023.4.0/src/Photini.egg-info/requires.txt
--rw-r--r--   0 jim       (1026) users      (100)        8 2023-04-12 08:05:36.000000 Photini-2023.4.0/src/Photini.egg-info/top_level.txt
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/doc/
--rw-r--r--   0 jim       (1026) users      (100)    22962 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/DOC_LICENSE.txt
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/doc/_static/
--rw-r--r--   0 jim       (1026) users      (100)      362 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/_static/theme_overrides.css
--rw-r--r--   0 jim       (1026) users      (100)     9019 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/conf.py
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/doc/images/
--rw-r--r--   0 jim       (1026) users      (100)    28931 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/photini_logo.png
--rw-r--r--   0 jim       (1026) users      (100)    15962 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_001.png
--rw-r--r--   0 jim       (1026) users      (100)    66348 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_002.png
--rw-r--r--   0 jim       (1026) users      (100)    65845 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_003.png
--rw-r--r--   0 jim       (1026) users      (100)    64733 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_004.png
--rw-r--r--   0 jim       (1026) users      (100)    65131 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_005.png
--rw-r--r--   0 jim       (1026) users      (100)    64148 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_006.png
--rw-r--r--   0 jim       (1026) users      (100)    67023 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_007.png
--rw-r--r--   0 jim       (1026) users      (100)    48212 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_008.png
--rw-r--r--   0 jim       (1026) users      (100)    71994 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_009.png
--rw-r--r--   0 jim       (1026) users      (100)    70012 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_020.png
--rw-r--r--   0 jim       (1026) users      (100)    69525 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_021.png
--rw-r--r--   0 jim       (1026) users      (100)    73576 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_022.png
--rw-r--r--   0 jim       (1026) users      (100)    65341 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_023.png
--rw-r--r--   0 jim       (1026) users      (100)    68287 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_024.png
--rw-r--r--   0 jim       (1026) users      (100)    65622 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_025.png
--rw-r--r--   0 jim       (1026) users      (100)    67340 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_026.png
--rw-r--r--   0 jim       (1026) users      (100)    72586 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_027.png
--rw-r--r--   0 jim       (1026) users      (100)    67154 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_028.png
--rw-r--r--   0 jim       (1026) users      (100)    73216 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_029.png
--rw-r--r--   0 jim       (1026) users      (100)    77326 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_030.png
--rw-r--r--   0 jim       (1026) users      (100)    76697 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_031.png
--rw-r--r--   0 jim       (1026) users      (100)    68783 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_032.png
--rw-r--r--   0 jim       (1026) users      (100)    70474 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_033.png
--rw-r--r--   0 jim       (1026) users      (100)    70537 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_034.png
--rw-r--r--   0 jim       (1026) users      (100)    77800 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_100.png
--rw-r--r--   0 jim       (1026) users      (100)    79011 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_101.png
--rw-r--r--   0 jim       (1026) users      (100)    79185 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_102.png
--rw-r--r--   0 jim       (1026) users      (100)    78789 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_103.png
--rw-r--r--   0 jim       (1026) users      (100)    62313 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_104.png
--rw-r--r--   0 jim       (1026) users      (100)    65935 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_105.png
--rw-r--r--   0 jim       (1026) users      (100)    67648 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_106.png
--rw-r--r--   0 jim       (1026) users      (100)    64890 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_107.png
--rw-r--r--   0 jim       (1026) users      (100)    42875 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_108.png
--rw-r--r--   0 jim       (1026) users      (100)    44739 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_109.png
--rw-r--r--   0 jim       (1026) users      (100)    44484 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_110.png
--rw-r--r--   0 jim       (1026) users      (100)    44818 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_111.png
--rw-r--r--   0 jim       (1026) users      (100)    46451 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_112.png
--rw-r--r--   0 jim       (1026) users      (100)    45716 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_113.png
--rw-r--r--   0 jim       (1026) users      (100)    43760 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_114.png
--rw-r--r--   0 jim       (1026) users      (100)    45329 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_115.png
--rw-r--r--   0 jim       (1026) users      (100)    47052 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_116.png
--rw-r--r--   0 jim       (1026) users      (100)    45324 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_117.png
--rw-r--r--   0 jim       (1026) users      (100)    98669 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_130.png
--rw-r--r--   0 jim       (1026) users      (100)    98212 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_131.png
--rw-r--r--   0 jim       (1026) users      (100)   100910 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_132.png
--rw-r--r--   0 jim       (1026) users      (100)    89696 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_133.png
--rw-r--r--   0 jim       (1026) users      (100)    80113 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_134.png
--rw-r--r--   0 jim       (1026) users      (100)    81620 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_135.png
--rw-r--r--   0 jim       (1026) users      (100)    79965 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_136.png
--rw-r--r--   0 jim       (1026) users      (100)    78982 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_137.png
--rw-r--r--   0 jim       (1026) users      (100)    89190 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_138.png
--rw-r--r--   0 jim       (1026) users      (100)    98494 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_139.png
--rw-r--r--   0 jim       (1026) users      (100)    58825 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_141.png
--rw-r--r--   0 jim       (1026) users      (100)    65771 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_142.png
--rw-r--r--   0 jim       (1026) users      (100)    61383 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_143.png
--rw-r--r--   0 jim       (1026) users      (100)    74612 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_144.png
--rw-r--r--   0 jim       (1026) users      (100)    72082 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_145.png
--rw-r--r--   0 jim       (1026) users      (100)    72823 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_146.png
--rw-r--r--   0 jim       (1026) users      (100)    60251 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_150.png
--rw-r--r--   0 jim       (1026) users      (100)    45446 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_151a.png
--rw-r--r--   0 jim       (1026) users      (100)    13244 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_151d.png
--rw-r--r--   0 jim       (1026) users      (100)    72503 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_152.png
--rw-r--r--   0 jim       (1026) users      (100)    65762 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_154.png
--rw-r--r--   0 jim       (1026) users      (100)    72249 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_155.png
--rw-r--r--   0 jim       (1026) users      (100)    80606 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_156.png
--rw-r--r--   0 jim       (1026) users      (100)    81976 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_157.png
--rw-r--r--   0 jim       (1026) users      (100)    72070 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_158.png
--rw-r--r--   0 jim       (1026) users      (100)    84127 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_159.png
--rw-r--r--   0 jim       (1026) users      (100)    54712 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_160.png
--rw-r--r--   0 jim       (1026) users      (100)    76525 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_161.png
--rw-r--r--   0 jim       (1026) users      (100)    54226 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_170.png
--rw-r--r--   0 jim       (1026) users      (100)    63855 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_171.png
--rw-r--r--   0 jim       (1026) users      (100)    69774 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_172.png
--rw-r--r--   0 jim       (1026) users      (100)    70791 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_173.png
--rw-r--r--   0 jim       (1026) users      (100)    66013 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_174.png
--rw-r--r--   0 jim       (1026) users      (100)    77354 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_175.png
--rw-r--r--   0 jim       (1026) users      (100)    20588 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_180.png
--rw-r--r--   0 jim       (1026) users      (100)    35446 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_181.png
--rw-r--r--   0 jim       (1026) users      (100)    40375 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_182.png
--rw-r--r--   0 jim       (1026) users      (100)    38151 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_183.png
--rw-r--r--   0 jim       (1026) users      (100)    43644 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_184.png
--rw-r--r--   0 jim       (1026) users      (100)    56298 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_185.png
--rw-r--r--   0 jim       (1026) users      (100)    69510 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_200.png
--rw-r--r--   0 jim       (1026) users      (100)    31477 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_201.png
--rw-r--r--   0 jim       (1026) users      (100)    39167 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_202.png
--rw-r--r--   0 jim       (1026) users      (100)    52117 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_203.png
--rw-r--r--   0 jim       (1026) users      (100)    76102 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_204.png
--rw-r--r--   0 jim       (1026) users      (100)   106593 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_220.png
--rw-r--r--   0 jim       (1026) users      (100)   115906 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_221.png
--rw-r--r--   0 jim       (1026) users      (100)   114123 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_222.png
--rw-r--r--   0 jim       (1026) users      (100)    86341 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_223.png
--rw-r--r--   0 jim       (1026) users      (100)    84648 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_224.png
--rw-r--r--   0 jim       (1026) users      (100)    87434 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_225.png
--rw-r--r--   0 jim       (1026) users      (100)    59154 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_230.png
--rw-r--r--   0 jim       (1026) users      (100)    66436 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_231.png
--rw-r--r--   0 jim       (1026) users      (100)    48689 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_232.png
--rw-r--r--   0 jim       (1026) users      (100)    41507 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_233.png
--rw-r--r--   0 jim       (1026) users      (100)    64402 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_234.png
--rw-r--r--   0 jim       (1026) users      (100)    61030 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_235.png
--rw-r--r--   0 jim       (1026) users      (100)    64905 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_236.png
--rw-r--r--   0 jim       (1026) users      (100)    73976 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_237.png
--rw-r--r--   0 jim       (1026) users      (100)    76099 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_238.png
--rw-r--r--   0 jim       (1026) users      (100)    76183 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_239.png
--rw-r--r--   0 jim       (1026) users      (100)    75744 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_240.png
--rw-r--r--   0 jim       (1026) users      (100)    83965 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_242.png
--rw-r--r--   0 jim       (1026) users      (100)    72956 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_250.png
--rw-r--r--   0 jim       (1026) users      (100)    76602 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_251.png
--rw-r--r--   0 jim       (1026) users      (100)    77132 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_252.png
--rw-r--r--   0 jim       (1026) users      (100)    18523 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_253.png
--rw-r--r--   0 jim       (1026) users      (100)    73131 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_254.png
--rw-r--r--   0 jim       (1026) users      (100)    68348 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_255.png
--rw-r--r--   0 jim       (1026) users      (100)    72388 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_256.png
--rw-r--r--   0 jim       (1026) users      (100)    73136 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_257.png
--rw-r--r--   0 jim       (1026) users      (100)    70116 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_258.png
--rw-r--r--   0 jim       (1026) users      (100)    79413 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_259.png
--rw-r--r--   0 jim       (1026) users      (100)    80423 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_260.png
--rw-r--r--   0 jim       (1026) users      (100)    64029 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_270.png
--rw-r--r--   0 jim       (1026) users      (100)   108239 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_271.png
--rw-r--r--   0 jim       (1026) users      (100)   112504 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_272.png
--rw-r--r--   0 jim       (1026) users      (100)   109408 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_273.png
--rw-r--r--   0 jim       (1026) users      (100)   110228 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_274.png
--rw-r--r--   0 jim       (1026) users      (100)   112780 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_275.png
--rw-r--r--   0 jim       (1026) users      (100)   107839 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_276.png
--rw-r--r--   0 jim       (1026) users      (100)   115642 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_277.png
--rw-r--r--   0 jim       (1026) users      (100)   117777 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_278.png
--rw-r--r--   0 jim       (1026) users      (100)   110698 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_279.png
--rw-r--r--   0 jim       (1026) users      (100)   110108 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_280.png
--rw-r--r--   0 jim       (1026) users      (100)    73241 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_36.png
--rw-r--r--   0 jim       (1026) users      (100)    22828 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/images/screenshot_37.png
--rw-r--r--   0 jim       (1026) users      (100)     1057 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/index.rst
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/doc/manual/
--rw-r--r--   0 jim       (1026) users      (100)     3324 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/manual/address.rst
--rw-r--r--   0 jim       (1026) users      (100)     9850 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/manual/configuration.rst
--rw-r--r--   0 jim       (1026) users      (100)     7134 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/manual/descriptive_metadata.rst
--rw-r--r--   0 jim       (1026) users      (100)     2314 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/manual/extending.rst
--rw-r--r--   0 jim       (1026) users      (100)     4778 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/manual/flickr.rst
--rw-r--r--   0 jim       (1026) users      (100)     2592 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/manual/google_photos.rst
--rw-r--r--   0 jim       (1026) users      (100)     4697 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/manual/image_selector.rst
--rw-r--r--   0 jim       (1026) users      (100)     4512 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/manual/importer.rst
--rw-r--r--   0 jim       (1026) users      (100)      731 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/manual/index.rst
--rw-r--r--   0 jim       (1026) users      (100)     4541 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/manual/ipernity.rst
--rw-r--r--   0 jim       (1026) users      (100)     5345 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/manual/map.rst
--rw-r--r--   0 jim       (1026) users      (100)     5212 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/manual/ownership_metadata.rst
--rw-r--r--   0 jim       (1026) users      (100)     4528 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/manual/pixelfed.rst
--rw-r--r--   0 jim       (1026) users      (100)     3165 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/manual/regions.rst
--rw-r--r--   0 jim       (1026) users      (100)    11368 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/manual/tags.rst
--rw-r--r--   0 jim       (1026) users      (100)     8028 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/manual/technical_metadata.rst
--rw-r--r--   0 jim       (1026) users      (100)     1354 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/manual/video.rst
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/doc/misc/
--rw-r--r--   0 jim       (1026) users      (100)      235 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/misc/changelog.rst
--rw-r--r--   0 jim       (1026) users      (100)      352 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/misc/doc_licence.rst
--rw-r--r--   0 jim       (1026) users      (100)      248 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/misc/index.rst
--rw-r--r--   0 jim       (1026) users      (100)      337 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/misc/licence.rst
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/doc/other/
--rw-r--r--   0 jim       (1026) users      (100)    42560 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/other/installation.rst
--rw-r--r--   0 jim       (1026) users      (100)      609 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/other/introduction.rst
--rw-r--r--   0 jim       (1026) users      (100)    12643 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/other/localisation.rst
--rw-r--r--   0 jim       (1026) users      (100)      686 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/other/reading.rst
--rw-r--r--   0 jim       (1026) users      (100)     5239 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/other/workflow.rst
--rw-r--r--   0 jim       (1026) users      (100)       70 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/doc/requirements.txt
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/lang/
--rw-r--r--   0 jim       (1026) users      (100)     3134 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/lang/README.rst
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/lang/ca/
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/lang/ca/LC_MESSAGES/
--rw-r--r--   0 jim       (1026) users      (100)     2595 2023-04-12 08:04:21.000000 Photini-2023.4.0/src/lang/ca/LC_MESSAGES/index.po
--rw-r--r--   0 jim       (1026) users      (100)    75951 2023-04-12 08:04:24.000000 Photini-2023.4.0/src/lang/ca/LC_MESSAGES/manual.po
--rw-r--r--   0 jim       (1026) users      (100)     1384 2023-04-12 08:04:27.000000 Photini-2023.4.0/src/lang/ca/LC_MESSAGES/misc.po
--rw-r--r--   0 jim       (1026) users      (100)    41764 2023-04-12 08:04:30.000000 Photini-2023.4.0/src/lang/ca/LC_MESSAGES/other.po
--rw-r--r--   0 jim       (1026) users      (100)    96826 2023-04-12 08:04:43.000000 Photini-2023.4.0/src/lang/ca/photini.ts
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/lang/cs/
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/lang/cs/LC_MESSAGES/
--rw-r--r--   0 jim       (1026) users      (100)     2728 2023-04-12 08:04:22.000000 Photini-2023.4.0/src/lang/cs/LC_MESSAGES/index.po
--rw-r--r--   0 jim       (1026) users      (100)    75857 2023-04-12 08:04:25.000000 Photini-2023.4.0/src/lang/cs/LC_MESSAGES/manual.po
--rw-r--r--   0 jim       (1026) users      (100)     1708 2023-04-12 08:04:28.000000 Photini-2023.4.0/src/lang/cs/LC_MESSAGES/misc.po
--rw-r--r--   0 jim       (1026) users      (100)    49939 2023-04-12 08:04:30.000000 Photini-2023.4.0/src/lang/cs/LC_MESSAGES/other.po
--rw-r--r--   0 jim       (1026) users      (100)    99461 2023-04-12 08:04:43.000000 Photini-2023.4.0/src/lang/cs/photini.ts
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/lang/de/
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/lang/de/LC_MESSAGES/
--rw-r--r--   0 jim       (1026) users      (100)     1773 2023-04-12 08:04:22.000000 Photini-2023.4.0/src/lang/de/LC_MESSAGES/index.po
--rw-r--r--   0 jim       (1026) users      (100)    76335 2023-04-12 08:04:25.000000 Photini-2023.4.0/src/lang/de/LC_MESSAGES/manual.po
--rw-r--r--   0 jim       (1026) users      (100)     1302 2023-04-12 08:04:27.000000 Photini-2023.4.0/src/lang/de/LC_MESSAGES/misc.po
--rw-r--r--   0 jim       (1026) users      (100)    42298 2023-04-12 08:04:31.000000 Photini-2023.4.0/src/lang/de/LC_MESSAGES/other.po
--rw-r--r--   0 jim       (1026) users      (100)    99572 2023-04-12 08:04:43.000000 Photini-2023.4.0/src/lang/de/photini.ts
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/lang/en/
--rw-r--r--   0 jim       (1026) users      (100)    87978 2023-04-12 08:04:43.000000 Photini-2023.4.0/src/lang/en/photini.ts
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/lang/es/
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/lang/es/LC_MESSAGES/
--rw-r--r--   0 jim       (1026) users      (100)     1814 2023-04-12 08:04:22.000000 Photini-2023.4.0/src/lang/es/LC_MESSAGES/index.po
--rw-r--r--   0 jim       (1026) users      (100)    75982 2023-04-12 08:04:25.000000 Photini-2023.4.0/src/lang/es/LC_MESSAGES/manual.po
--rw-r--r--   0 jim       (1026) users      (100)     1171 2023-04-12 08:04:28.000000 Photini-2023.4.0/src/lang/es/LC_MESSAGES/misc.po
--rw-r--r--   0 jim       (1026) users      (100)    41696 2023-04-12 08:04:31.000000 Photini-2023.4.0/src/lang/es/LC_MESSAGES/other.po
--rw-r--r--   0 jim       (1026) users      (100)    96008 2023-04-12 08:04:43.000000 Photini-2023.4.0/src/lang/es/photini.ts
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/lang/fr/
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/lang/fr/LC_MESSAGES/
--rw-r--r--   0 jim       (1026) users      (100)     1824 2023-04-12 08:04:23.000000 Photini-2023.4.0/src/lang/fr/LC_MESSAGES/index.po
--rw-r--r--   0 jim       (1026) users      (100)    75661 2023-04-12 08:04:26.000000 Photini-2023.4.0/src/lang/fr/LC_MESSAGES/manual.po
--rw-r--r--   0 jim       (1026) users      (100)     1182 2023-04-12 08:04:28.000000 Photini-2023.4.0/src/lang/fr/LC_MESSAGES/misc.po
--rw-r--r--   0 jim       (1026) users      (100)    41713 2023-04-12 08:04:31.000000 Photini-2023.4.0/src/lang/fr/LC_MESSAGES/other.po
--rw-r--r--   0 jim       (1026) users      (100)   100291 2023-04-12 08:04:43.000000 Photini-2023.4.0/src/lang/fr/photini.ts
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/lang/it/
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/lang/it/LC_MESSAGES/
--rw-r--r--   0 jim       (1026) users      (100)     1648 2023-04-12 08:04:23.000000 Photini-2023.4.0/src/lang/it/LC_MESSAGES/index.po
--rw-r--r--   0 jim       (1026) users      (100)    75543 2023-04-12 08:04:26.000000 Photini-2023.4.0/src/lang/it/LC_MESSAGES/manual.po
--rw-r--r--   0 jim       (1026) users      (100)     1171 2023-04-12 08:04:28.000000 Photini-2023.4.0/src/lang/it/LC_MESSAGES/misc.po
--rw-r--r--   0 jim       (1026) users      (100)    41530 2023-04-12 08:04:31.000000 Photini-2023.4.0/src/lang/it/LC_MESSAGES/other.po
--rw-r--r--   0 jim       (1026) users      (100)    95701 2023-04-12 08:04:43.000000 Photini-2023.4.0/src/lang/it/photini.ts
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/lang/ko/
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/lang/ko/LC_MESSAGES/
--rw-r--r--   0 jim       (1026) users      (100)     2765 2023-04-12 08:04:24.000000 Photini-2023.4.0/src/lang/ko/LC_MESSAGES/index.po
--rw-r--r--   0 jim       (1026) users      (100)   141558 2023-04-12 08:04:26.000000 Photini-2023.4.0/src/lang/ko/LC_MESSAGES/manual.po
--rw-r--r--   0 jim       (1026) users      (100)     1662 2023-04-12 08:04:29.000000 Photini-2023.4.0/src/lang/ko/LC_MESSAGES/misc.po
--rw-r--r--   0 jim       (1026) users      (100)    67188 2023-04-12 08:04:32.000000 Photini-2023.4.0/src/lang/ko/LC_MESSAGES/other.po
--rw-r--r--   0 jim       (1026) users      (100)    95625 2023-04-12 08:04:43.000000 Photini-2023.4.0/src/lang/ko/photini.ts
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/lang/nb/
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/lang/nb/LC_MESSAGES/
--rw-r--r--   0 jim       (1026) users      (100)     1781 2023-04-12 08:04:24.000000 Photini-2023.4.0/src/lang/nb/LC_MESSAGES/index.po
--rw-r--r--   0 jim       (1026) users      (100)    75596 2023-04-12 08:04:27.000000 Photini-2023.4.0/src/lang/nb/LC_MESSAGES/manual.po
--rw-r--r--   0 jim       (1026) users      (100)     1142 2023-04-12 08:04:29.000000 Photini-2023.4.0/src/lang/nb/LC_MESSAGES/misc.po
--rw-r--r--   0 jim       (1026) users      (100)    41669 2023-04-12 08:04:32.000000 Photini-2023.4.0/src/lang/nb/LC_MESSAGES/other.po
--rw-r--r--   0 jim       (1026) users      (100)    95337 2023-04-12 08:04:43.000000 Photini-2023.4.0/src/lang/nb/photini.ts
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/lang/pl/
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/lang/pl/LC_MESSAGES/
--rw-r--r--   0 jim       (1026) users      (100)     1851 2023-04-12 08:04:24.000000 Photini-2023.4.0/src/lang/pl/LC_MESSAGES/index.po
--rw-r--r--   0 jim       (1026) users      (100)    75727 2023-04-12 08:04:27.000000 Photini-2023.4.0/src/lang/pl/LC_MESSAGES/manual.po
--rw-r--r--   0 jim       (1026) users      (100)     1277 2023-04-12 08:04:29.000000 Photini-2023.4.0/src/lang/pl/LC_MESSAGES/misc.po
--rw-r--r--   0 jim       (1026) users      (100)    41743 2023-04-12 08:04:32.000000 Photini-2023.4.0/src/lang/pl/LC_MESSAGES/other.po
--rw-r--r--   0 jim       (1026) users      (100)    95997 2023-04-12 08:04:43.000000 Photini-2023.4.0/src/lang/pl/photini.ts
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/lang/templates/
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/lang/templates/gettext/
--rw-r--r--   0 jim       (1026) users      (100)     1508 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/lang/templates/gettext/index.pot
--rw-r--r--   0 jim       (1026) users      (100)    72700 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/lang/templates/gettext/manual.pot
--rw-r--r--   0 jim       (1026) users      (100)     1055 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/lang/templates/gettext/misc.pot
--rw-r--r--   0 jim       (1026) users      (100)    40008 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/lang/templates/gettext/other.pot
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/lang/templates/qt/
--rw-r--r--   0 jim       (1026) users      (100)    96788 2023-04-12 08:04:43.000000 Photini-2023.4.0/src/lang/templates/qt/photini.ts
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/photini/
--rw-r--r--   0 jim       (1026) users      (100)      114 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/__init__.py
--rw-r--r--   0 jim       (1026) users      (100)      917 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/__main__.py
--rw-r--r--   0 jim       (1026) users      (100)    19879 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/address.py
--rw-r--r--   0 jim       (1026) users      (100)     4759 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/bingmap.py
--rw-r--r--   0 jim       (1026) users      (100)     5310 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/configstore.py
--rw-r--r--   0 jim       (1026) users      (100)     6890 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/cv.py
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/photini/data/
--rw-r--r--   0 jim       (1026) users      (100)    35147 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/data/LICENSE.txt
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/photini/data/bingmap/
--rw-r--r--   0 jim       (1026) users      (100)     7556 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/data/bingmap/script.js
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/photini/data/googlemap/
--rw-r--r--   0 jim       (1026) users      (100)     6239 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/data/googlemap/script.js
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/photini/data/icons/
--rw-r--r--   0 jim       (1026) users      (100)    14554 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/data/icons/photini_128.png
--rw-r--r--   0 jim       (1026) users      (100)     3262 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/data/icons/photini_48.png
--rw-r--r--   0 jim       (1026) users      (100)    86598 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/data/icons/photini_win.ico
--rw-r--r--   0 jim       (1026) users      (100)     2205 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/data/keys.txt
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/photini/data/lang/
--rw-r--r--   0 jim       (1026) users      (100)    22137 2023-04-12 08:05:22.000000 Photini-2023.4.0/src/photini/data/lang/photini.ca.qm
--rw-r--r--   0 jim       (1026) users      (100)    40194 2023-04-12 08:05:21.000000 Photini-2023.4.0/src/photini/data/lang/photini.cs.qm
--rw-r--r--   0 jim       (1026) users      (100)    44214 2023-04-12 08:05:20.000000 Photini-2023.4.0/src/photini/data/lang/photini.de.qm
--rw-r--r--   0 jim       (1026) users      (100)    28726 2023-04-12 08:05:20.000000 Photini-2023.4.0/src/photini/data/lang/photini.en.qm
--rw-r--r--   0 jim       (1026) users      (100)    10112 2023-04-12 08:05:21.000000 Photini-2023.4.0/src/photini/data/lang/photini.es.qm
--rw-r--r--   0 jim       (1026) users      (100)    41878 2023-04-12 08:05:20.000000 Photini-2023.4.0/src/photini/data/lang/photini.fr.qm
--rw-r--r--   0 jim       (1026) users      (100)      923 2023-04-12 08:05:21.000000 Photini-2023.4.0/src/photini/data/lang/photini.it.qm
--rw-r--r--   0 jim       (1026) users      (100)     2072 2023-04-12 08:05:21.000000 Photini-2023.4.0/src/photini/data/lang/photini.ko.qm
--rw-r--r--   0 jim       (1026) users      (100)    19489 2023-04-12 08:05:22.000000 Photini-2023.4.0/src/photini/data/lang/photini.nb.qm
--rw-r--r--   0 jim       (1026) users      (100)    10060 2023-04-12 08:05:22.000000 Photini-2023.4.0/src/photini/data/lang/photini.pl.qm
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/photini/data/linux/
--rw-r--r--   0 jim       (1026) users      (100)      991 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/data/linux/photini.desktop
--rw-r--r--   0 jim       (1026) users      (100)      209 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/data/map_circle_blue.png
--rw-r--r--   0 jim       (1026) users      (100)      207 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/data/map_circle_red.png
--rw-r--r--   0 jim       (1026) users      (100)     1867 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/data/map_pin_grey.png
--rw-r--r--   0 jim       (1026) users      (100)     2016 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/data/map_pin_red.png
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/photini/data/mapboxmap/
--rw-r--r--   0 jim       (1026) users      (100)     5715 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/data/mapboxmap/script.js
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/src/photini/data/windows/
--rw-r--r--   0 jim       (1026) users      (100)     2638 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/data/windows/install_shortcuts.vbs
--rw-r--r--   0 jim       (1026) users      (100)    13464 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/descriptive.py
--rw-r--r--   0 jim       (1026) users      (100)    22760 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/editor.py
--rw-r--r--   0 jim       (1026) users      (100)     7893 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/editsettings.py
--rw-r--r--   0 jim       (1026) users      (100)    31789 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/exiv2.py
--rw-r--r--   0 jim       (1026) users      (100)     3287 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/ffmpeg.py
--rw-r--r--   0 jim       (1026) users      (100)    33292 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/flickr.py
--rw-r--r--   0 jim       (1026) users      (100)     4191 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/googlemap.py
--rw-r--r--   0 jim       (1026) users      (100)    13099 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/googlephotos.py
--rw-r--r--   0 jim       (1026) users      (100)     4382 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/gpximporter.py
--rw-r--r--   0 jim       (1026) users      (100)    40241 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/imagelist.py
--rw-r--r--   0 jim       (1026) users      (100)    27611 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/importer.py
--rw-r--r--   0 jim       (1026) users      (100)    27252 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/ipernity.py
--rw-r--r--   0 jim       (1026) users      (100)     4396 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/loggerwindow.py
--rw-r--r--   0 jim       (1026) users      (100)     4235 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/mapboxmap.py
--rw-r--r--   0 jim       (1026) users      (100)    36681 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/metadata.py
--rw-r--r--   0 jim       (1026) users      (100)    21920 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/ownership.py
--rw-r--r--   0 jim       (1026) users      (100)    25534 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/photinimap.py
--rw-r--r--   0 jim       (1026) users      (100)    37738 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/pixelfed.py
--rw-r--r--   0 jim       (1026) users      (100)    10550 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/pyqt.py
--rw-r--r--   0 jim       (1026) users      (100)    36614 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/regions.py
--rw-r--r--   0 jim       (1026) users      (100)     6711 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/scripts.py
--rw-r--r--   0 jim       (1026) users      (100)     3687 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/spelling.py
--rw-r--r--   0 jim       (1026) users      (100)    40220 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/technical.py
--rw-r--r--   0 jim       (1026) users      (100)    71730 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/types.py
--rw-r--r--   0 jim       (1026) users      (100)    47911 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/uploader.py
--rw-r--r--   0 jim       (1026) users      (100)    34745 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/photini/widgets.py
--rw-r--r--   0 jim       (1026) users      (100)     1097 2023-04-12 08:03:27.000000 Photini-2023.4.0/src/run_photini.py
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/utils/
--rw-r--r--   0 jim       (1026) users      (100)     1257 2023-04-12 08:03:27.000000 Photini-2023.4.0/utils/build_docs.py
--rw-r--r--   0 jim       (1026) users      (100)     1511 2023-04-12 08:03:27.000000 Photini-2023.4.0/utils/build_lang.py
--rw-r--r--   0 jim       (1026) users      (100)     2723 2023-04-12 08:03:27.000000 Photini-2023.4.0/utils/download_cvs.py
--rw-r--r--   0 jim       (1026) users      (100)     8048 2023-04-12 08:03:27.000000 Photini-2023.4.0/utils/lang_update.py
--rw-r--r--   0 jim       (1026) users      (100)     2220 2023-04-12 08:03:27.000000 Photini-2023.4.0/utils/localise_desktop.py
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-12 08:05:37.000000 Photini-2023.4.0/utils/make_icons/
--rw-r--r--   0 jim       (1026) users      (100)      166 2023-04-12 08:03:27.000000 Photini-2023.4.0/utils/make_icons/circle.fig
--rw-r--r--   0 jim       (1026) users      (100)   178291 2023-04-12 08:03:27.000000 Photini-2023.4.0/utils/make_icons/icon_master.png
--rw-r--r--   0 jim       (1026) users      (100)     1279 2023-04-12 08:03:27.000000 Photini-2023.4.0/utils/make_icons/makefile
--rw-r--r--   0 jim       (1026) users      (100)     1539 2023-04-12 08:03:27.000000 Photini-2023.4.0/utils/tag_release.py
--rw-r--r--   0 jim       (1026) users      (100)     2846 2023-04-12 08:03:27.000000 Photini-2023.4.0/utils/update_version.py
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/
+-rw-r--r--   0 jim       (1026) users      (100)    15393 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/CHANGELOG.txt
+-rw-r--r--   0 jim       (1026) users      (100)    35147 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/LICENSE.txt
+-rw-r--r--   0 jim       (1026) users      (100)      170 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/MANIFEST.in
+-rw-r--r--   0 jim       (1026) users      (100)    10321 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/PKG-INFO
+-rw-r--r--   0 jim       (1026) users      (100)     7814 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/README.rst
+-rw-r--r--   0 jim       (1026) users      (100)       38 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/setup.cfg
+-rw-r--r--   0 jim       (1026) users      (100)     4362 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/setup.py
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:53.000000 Photini-2023.4.0.1/src/
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:53.000000 Photini-2023.4.0.1/src/Photini.egg-info/
+-rw-r--r--   0 jim       (1026) users      (100)    10321 2023-04-13 09:47:53.000000 Photini-2023.4.0.1/src/Photini.egg-info/PKG-INFO
+-rw-r--r--   0 jim       (1026) users      (100)     9110 2023-04-13 09:47:53.000000 Photini-2023.4.0.1/src/Photini.egg-info/SOURCES.txt
+-rw-r--r--   0 jim       (1026) users      (100)        1 2023-04-13 09:47:53.000000 Photini-2023.4.0.1/src/Photini.egg-info/dependency_links.txt
+-rw-r--r--   0 jim       (1026) users      (100)      162 2023-04-13 09:47:53.000000 Photini-2023.4.0.1/src/Photini.egg-info/entry_points.txt
+-rw-r--r--   0 jim       (1026) users      (100)        1 2023-04-12 08:05:36.000000 Photini-2023.4.0.1/src/Photini.egg-info/not-zip-safe
+-rw-r--r--   0 jim       (1026) users      (100)     1044 2023-04-13 09:47:53.000000 Photini-2023.4.0.1/src/Photini.egg-info/requires.txt
+-rw-r--r--   0 jim       (1026) users      (100)        8 2023-04-13 09:47:53.000000 Photini-2023.4.0.1/src/Photini.egg-info/top_level.txt
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:53.000000 Photini-2023.4.0.1/src/doc/
+-rw-r--r--   0 jim       (1026) users      (100)    22962 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/DOC_LICENSE.txt
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:53.000000 Photini-2023.4.0.1/src/doc/_static/
+-rw-r--r--   0 jim       (1026) users      (100)      362 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/_static/theme_overrides.css
+-rw-r--r--   0 jim       (1026) users      (100)     9019 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/conf.py
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/doc/images/
+-rw-r--r--   0 jim       (1026) users      (100)    28931 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/photini_logo.png
+-rw-r--r--   0 jim       (1026) users      (100)    15962 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_001.png
+-rw-r--r--   0 jim       (1026) users      (100)    66348 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_002.png
+-rw-r--r--   0 jim       (1026) users      (100)    65845 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_003.png
+-rw-r--r--   0 jim       (1026) users      (100)    64733 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_004.png
+-rw-r--r--   0 jim       (1026) users      (100)    65131 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_005.png
+-rw-r--r--   0 jim       (1026) users      (100)    64148 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_006.png
+-rw-r--r--   0 jim       (1026) users      (100)    67023 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_007.png
+-rw-r--r--   0 jim       (1026) users      (100)    48212 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_008.png
+-rw-r--r--   0 jim       (1026) users      (100)    71994 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_009.png
+-rw-r--r--   0 jim       (1026) users      (100)    70012 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_020.png
+-rw-r--r--   0 jim       (1026) users      (100)    69525 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_021.png
+-rw-r--r--   0 jim       (1026) users      (100)    73576 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_022.png
+-rw-r--r--   0 jim       (1026) users      (100)    65341 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_023.png
+-rw-r--r--   0 jim       (1026) users      (100)    68287 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_024.png
+-rw-r--r--   0 jim       (1026) users      (100)    65622 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_025.png
+-rw-r--r--   0 jim       (1026) users      (100)    67340 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_026.png
+-rw-r--r--   0 jim       (1026) users      (100)    72586 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_027.png
+-rw-r--r--   0 jim       (1026) users      (100)    67154 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_028.png
+-rw-r--r--   0 jim       (1026) users      (100)    73216 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_029.png
+-rw-r--r--   0 jim       (1026) users      (100)    77326 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_030.png
+-rw-r--r--   0 jim       (1026) users      (100)    76697 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_031.png
+-rw-r--r--   0 jim       (1026) users      (100)    68783 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_032.png
+-rw-r--r--   0 jim       (1026) users      (100)    70474 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_033.png
+-rw-r--r--   0 jim       (1026) users      (100)    70537 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_034.png
+-rw-r--r--   0 jim       (1026) users      (100)    77800 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_100.png
+-rw-r--r--   0 jim       (1026) users      (100)    79011 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_101.png
+-rw-r--r--   0 jim       (1026) users      (100)    79185 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_102.png
+-rw-r--r--   0 jim       (1026) users      (100)    78789 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_103.png
+-rw-r--r--   0 jim       (1026) users      (100)    62313 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_104.png
+-rw-r--r--   0 jim       (1026) users      (100)    65935 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_105.png
+-rw-r--r--   0 jim       (1026) users      (100)    67648 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_106.png
+-rw-r--r--   0 jim       (1026) users      (100)    64890 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_107.png
+-rw-r--r--   0 jim       (1026) users      (100)    42875 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_108.png
+-rw-r--r--   0 jim       (1026) users      (100)    44739 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_109.png
+-rw-r--r--   0 jim       (1026) users      (100)    44484 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_110.png
+-rw-r--r--   0 jim       (1026) users      (100)    44818 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_111.png
+-rw-r--r--   0 jim       (1026) users      (100)    46451 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_112.png
+-rw-r--r--   0 jim       (1026) users      (100)    45716 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_113.png
+-rw-r--r--   0 jim       (1026) users      (100)    43760 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_114.png
+-rw-r--r--   0 jim       (1026) users      (100)    45329 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_115.png
+-rw-r--r--   0 jim       (1026) users      (100)    47052 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_116.png
+-rw-r--r--   0 jim       (1026) users      (100)    45324 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_117.png
+-rw-r--r--   0 jim       (1026) users      (100)    98669 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_130.png
+-rw-r--r--   0 jim       (1026) users      (100)    98212 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_131.png
+-rw-r--r--   0 jim       (1026) users      (100)   100910 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_132.png
+-rw-r--r--   0 jim       (1026) users      (100)    89696 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_133.png
+-rw-r--r--   0 jim       (1026) users      (100)    80113 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_134.png
+-rw-r--r--   0 jim       (1026) users      (100)    81620 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_135.png
+-rw-r--r--   0 jim       (1026) users      (100)    79965 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_136.png
+-rw-r--r--   0 jim       (1026) users      (100)    78982 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_137.png
+-rw-r--r--   0 jim       (1026) users      (100)    89190 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_138.png
+-rw-r--r--   0 jim       (1026) users      (100)    98494 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_139.png
+-rw-r--r--   0 jim       (1026) users      (100)    58825 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_141.png
+-rw-r--r--   0 jim       (1026) users      (100)    65771 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_142.png
+-rw-r--r--   0 jim       (1026) users      (100)    61383 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_143.png
+-rw-r--r--   0 jim       (1026) users      (100)    74612 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_144.png
+-rw-r--r--   0 jim       (1026) users      (100)    72082 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_145.png
+-rw-r--r--   0 jim       (1026) users      (100)    72823 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_146.png
+-rw-r--r--   0 jim       (1026) users      (100)    60251 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_150.png
+-rw-r--r--   0 jim       (1026) users      (100)    45446 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_151a.png
+-rw-r--r--   0 jim       (1026) users      (100)    13244 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_151d.png
+-rw-r--r--   0 jim       (1026) users      (100)    72503 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_152.png
+-rw-r--r--   0 jim       (1026) users      (100)    65762 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_154.png
+-rw-r--r--   0 jim       (1026) users      (100)    72249 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_155.png
+-rw-r--r--   0 jim       (1026) users      (100)    80606 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_156.png
+-rw-r--r--   0 jim       (1026) users      (100)    81976 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_157.png
+-rw-r--r--   0 jim       (1026) users      (100)    72070 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_158.png
+-rw-r--r--   0 jim       (1026) users      (100)    84127 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_159.png
+-rw-r--r--   0 jim       (1026) users      (100)    54712 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_160.png
+-rw-r--r--   0 jim       (1026) users      (100)    76525 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_161.png
+-rw-r--r--   0 jim       (1026) users      (100)    54226 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_170.png
+-rw-r--r--   0 jim       (1026) users      (100)    63855 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_171.png
+-rw-r--r--   0 jim       (1026) users      (100)    69774 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_172.png
+-rw-r--r--   0 jim       (1026) users      (100)    70791 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_173.png
+-rw-r--r--   0 jim       (1026) users      (100)    66013 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_174.png
+-rw-r--r--   0 jim       (1026) users      (100)    77354 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_175.png
+-rw-r--r--   0 jim       (1026) users      (100)    20588 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_180.png
+-rw-r--r--   0 jim       (1026) users      (100)    35446 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_181.png
+-rw-r--r--   0 jim       (1026) users      (100)    40375 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_182.png
+-rw-r--r--   0 jim       (1026) users      (100)    38151 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_183.png
+-rw-r--r--   0 jim       (1026) users      (100)    43644 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_184.png
+-rw-r--r--   0 jim       (1026) users      (100)    56298 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_185.png
+-rw-r--r--   0 jim       (1026) users      (100)    69510 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_200.png
+-rw-r--r--   0 jim       (1026) users      (100)    31477 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_201.png
+-rw-r--r--   0 jim       (1026) users      (100)    39167 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_202.png
+-rw-r--r--   0 jim       (1026) users      (100)    52117 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_203.png
+-rw-r--r--   0 jim       (1026) users      (100)    76102 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_204.png
+-rw-r--r--   0 jim       (1026) users      (100)   106593 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_220.png
+-rw-r--r--   0 jim       (1026) users      (100)   115906 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_221.png
+-rw-r--r--   0 jim       (1026) users      (100)   114123 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_222.png
+-rw-r--r--   0 jim       (1026) users      (100)    86341 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_223.png
+-rw-r--r--   0 jim       (1026) users      (100)    84648 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_224.png
+-rw-r--r--   0 jim       (1026) users      (100)    87434 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_225.png
+-rw-r--r--   0 jim       (1026) users      (100)    59154 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_230.png
+-rw-r--r--   0 jim       (1026) users      (100)    66436 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_231.png
+-rw-r--r--   0 jim       (1026) users      (100)    48689 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_232.png
+-rw-r--r--   0 jim       (1026) users      (100)    41507 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_233.png
+-rw-r--r--   0 jim       (1026) users      (100)    64402 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_234.png
+-rw-r--r--   0 jim       (1026) users      (100)    61030 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_235.png
+-rw-r--r--   0 jim       (1026) users      (100)    64905 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_236.png
+-rw-r--r--   0 jim       (1026) users      (100)    73976 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_237.png
+-rw-r--r--   0 jim       (1026) users      (100)    76099 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_238.png
+-rw-r--r--   0 jim       (1026) users      (100)    76183 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_239.png
+-rw-r--r--   0 jim       (1026) users      (100)    75744 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_240.png
+-rw-r--r--   0 jim       (1026) users      (100)    83965 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_242.png
+-rw-r--r--   0 jim       (1026) users      (100)    72956 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_250.png
+-rw-r--r--   0 jim       (1026) users      (100)    76602 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_251.png
+-rw-r--r--   0 jim       (1026) users      (100)    77132 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_252.png
+-rw-r--r--   0 jim       (1026) users      (100)    18523 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_253.png
+-rw-r--r--   0 jim       (1026) users      (100)    73131 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_254.png
+-rw-r--r--   0 jim       (1026) users      (100)    68348 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_255.png
+-rw-r--r--   0 jim       (1026) users      (100)    72388 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_256.png
+-rw-r--r--   0 jim       (1026) users      (100)    73136 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_257.png
+-rw-r--r--   0 jim       (1026) users      (100)    70116 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_258.png
+-rw-r--r--   0 jim       (1026) users      (100)    79413 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_259.png
+-rw-r--r--   0 jim       (1026) users      (100)    80423 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_260.png
+-rw-r--r--   0 jim       (1026) users      (100)    64029 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_270.png
+-rw-r--r--   0 jim       (1026) users      (100)   108239 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_271.png
+-rw-r--r--   0 jim       (1026) users      (100)   112504 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_272.png
+-rw-r--r--   0 jim       (1026) users      (100)   109408 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_273.png
+-rw-r--r--   0 jim       (1026) users      (100)   110228 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_274.png
+-rw-r--r--   0 jim       (1026) users      (100)   112780 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_275.png
+-rw-r--r--   0 jim       (1026) users      (100)   107839 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_276.png
+-rw-r--r--   0 jim       (1026) users      (100)   115642 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_277.png
+-rw-r--r--   0 jim       (1026) users      (100)   117777 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_278.png
+-rw-r--r--   0 jim       (1026) users      (100)   110698 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_279.png
+-rw-r--r--   0 jim       (1026) users      (100)   110108 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_280.png
+-rw-r--r--   0 jim       (1026) users      (100)    73241 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_36.png
+-rw-r--r--   0 jim       (1026) users      (100)    22828 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/images/screenshot_37.png
+-rw-r--r--   0 jim       (1026) users      (100)     1057 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/index.rst
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/doc/manual/
+-rw-r--r--   0 jim       (1026) users      (100)     3324 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/manual/address.rst
+-rw-r--r--   0 jim       (1026) users      (100)     9850 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/manual/configuration.rst
+-rw-r--r--   0 jim       (1026) users      (100)     7134 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/manual/descriptive_metadata.rst
+-rw-r--r--   0 jim       (1026) users      (100)     2314 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/manual/extending.rst
+-rw-r--r--   0 jim       (1026) users      (100)     4778 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/manual/flickr.rst
+-rw-r--r--   0 jim       (1026) users      (100)     2592 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/manual/google_photos.rst
+-rw-r--r--   0 jim       (1026) users      (100)     4697 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/manual/image_selector.rst
+-rw-r--r--   0 jim       (1026) users      (100)     4512 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/manual/importer.rst
+-rw-r--r--   0 jim       (1026) users      (100)      731 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/manual/index.rst
+-rw-r--r--   0 jim       (1026) users      (100)     4541 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/manual/ipernity.rst
+-rw-r--r--   0 jim       (1026) users      (100)     5345 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/manual/map.rst
+-rw-r--r--   0 jim       (1026) users      (100)     5212 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/manual/ownership_metadata.rst
+-rw-r--r--   0 jim       (1026) users      (100)     4528 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/manual/pixelfed.rst
+-rw-r--r--   0 jim       (1026) users      (100)     3165 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/manual/regions.rst
+-rw-r--r--   0 jim       (1026) users      (100)    11368 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/manual/tags.rst
+-rw-r--r--   0 jim       (1026) users      (100)     8028 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/manual/technical_metadata.rst
+-rw-r--r--   0 jim       (1026) users      (100)     1354 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/manual/video.rst
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/doc/misc/
+-rw-r--r--   0 jim       (1026) users      (100)      235 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/misc/changelog.rst
+-rw-r--r--   0 jim       (1026) users      (100)      352 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/misc/doc_licence.rst
+-rw-r--r--   0 jim       (1026) users      (100)      248 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/misc/index.rst
+-rw-r--r--   0 jim       (1026) users      (100)      337 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/misc/licence.rst
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/doc/other/
+-rw-r--r--   0 jim       (1026) users      (100)    42560 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/other/installation.rst
+-rw-r--r--   0 jim       (1026) users      (100)      609 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/other/introduction.rst
+-rw-r--r--   0 jim       (1026) users      (100)    12643 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/other/localisation.rst
+-rw-r--r--   0 jim       (1026) users      (100)      686 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/other/reading.rst
+-rw-r--r--   0 jim       (1026) users      (100)     5239 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/other/workflow.rst
+-rw-r--r--   0 jim       (1026) users      (100)       70 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/doc/requirements.txt
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/lang/
+-rw-r--r--   0 jim       (1026) users      (100)     3134 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/lang/README.rst
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/lang/ca/
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/lang/ca/LC_MESSAGES/
+-rw-r--r--   0 jim       (1026) users      (100)     2595 2023-04-13 09:47:02.000000 Photini-2023.4.0.1/src/lang/ca/LC_MESSAGES/index.po
+-rw-r--r--   0 jim       (1026) users      (100)    75951 2023-04-13 09:47:05.000000 Photini-2023.4.0.1/src/lang/ca/LC_MESSAGES/manual.po
+-rw-r--r--   0 jim       (1026) users      (100)     1384 2023-04-13 09:47:08.000000 Photini-2023.4.0.1/src/lang/ca/LC_MESSAGES/misc.po
+-rw-r--r--   0 jim       (1026) users      (100)    41764 2023-04-13 09:47:11.000000 Photini-2023.4.0.1/src/lang/ca/LC_MESSAGES/other.po
+-rw-r--r--   0 jim       (1026) users      (100)    96826 2023-04-13 09:47:38.000000 Photini-2023.4.0.1/src/lang/ca/photini.ts
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/lang/cs/
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/lang/cs/LC_MESSAGES/
+-rw-r--r--   0 jim       (1026) users      (100)     2728 2023-04-13 09:47:03.000000 Photini-2023.4.0.1/src/lang/cs/LC_MESSAGES/index.po
+-rw-r--r--   0 jim       (1026) users      (100)    75857 2023-04-13 09:47:05.000000 Photini-2023.4.0.1/src/lang/cs/LC_MESSAGES/manual.po
+-rw-r--r--   0 jim       (1026) users      (100)     1708 2023-04-13 09:47:08.000000 Photini-2023.4.0.1/src/lang/cs/LC_MESSAGES/misc.po
+-rw-r--r--   0 jim       (1026) users      (100)    49939 2023-04-13 09:47:11.000000 Photini-2023.4.0.1/src/lang/cs/LC_MESSAGES/other.po
+-rw-r--r--   0 jim       (1026) users      (100)    99461 2023-04-13 09:47:38.000000 Photini-2023.4.0.1/src/lang/cs/photini.ts
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/lang/de/
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/lang/de/LC_MESSAGES/
+-rw-r--r--   0 jim       (1026) users      (100)     1773 2023-04-13 09:47:03.000000 Photini-2023.4.0.1/src/lang/de/LC_MESSAGES/index.po
+-rw-r--r--   0 jim       (1026) users      (100)    76335 2023-04-13 09:47:06.000000 Photini-2023.4.0.1/src/lang/de/LC_MESSAGES/manual.po
+-rw-r--r--   0 jim       (1026) users      (100)     1302 2023-04-13 09:47:08.000000 Photini-2023.4.0.1/src/lang/de/LC_MESSAGES/misc.po
+-rw-r--r--   0 jim       (1026) users      (100)    42298 2023-04-13 09:47:11.000000 Photini-2023.4.0.1/src/lang/de/LC_MESSAGES/other.po
+-rw-r--r--   0 jim       (1026) users      (100)    99572 2023-04-13 09:47:38.000000 Photini-2023.4.0.1/src/lang/de/photini.ts
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/lang/en/
+-rw-r--r--   0 jim       (1026) users      (100)    87978 2023-04-13 09:47:38.000000 Photini-2023.4.0.1/src/lang/en/photini.ts
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/lang/es/
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/lang/es/LC_MESSAGES/
+-rw-r--r--   0 jim       (1026) users      (100)     1814 2023-04-13 09:47:03.000000 Photini-2023.4.0.1/src/lang/es/LC_MESSAGES/index.po
+-rw-r--r--   0 jim       (1026) users      (100)    75982 2023-04-13 09:47:06.000000 Photini-2023.4.0.1/src/lang/es/LC_MESSAGES/manual.po
+-rw-r--r--   0 jim       (1026) users      (100)     1171 2023-04-13 09:47:09.000000 Photini-2023.4.0.1/src/lang/es/LC_MESSAGES/misc.po
+-rw-r--r--   0 jim       (1026) users      (100)    41696 2023-04-13 09:47:11.000000 Photini-2023.4.0.1/src/lang/es/LC_MESSAGES/other.po
+-rw-r--r--   0 jim       (1026) users      (100)    96008 2023-04-13 09:47:38.000000 Photini-2023.4.0.1/src/lang/es/photini.ts
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/lang/fr/
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/lang/fr/LC_MESSAGES/
+-rw-r--r--   0 jim       (1026) users      (100)     1824 2023-04-13 09:47:03.000000 Photini-2023.4.0.1/src/lang/fr/LC_MESSAGES/index.po
+-rw-r--r--   0 jim       (1026) users      (100)    75661 2023-04-13 09:47:06.000000 Photini-2023.4.0.1/src/lang/fr/LC_MESSAGES/manual.po
+-rw-r--r--   0 jim       (1026) users      (100)     1182 2023-04-13 09:47:09.000000 Photini-2023.4.0.1/src/lang/fr/LC_MESSAGES/misc.po
+-rw-r--r--   0 jim       (1026) users      (100)    41713 2023-04-13 09:47:12.000000 Photini-2023.4.0.1/src/lang/fr/LC_MESSAGES/other.po
+-rw-r--r--   0 jim       (1026) users      (100)   100291 2023-04-13 09:47:38.000000 Photini-2023.4.0.1/src/lang/fr/photini.ts
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/lang/it/
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/lang/it/LC_MESSAGES/
+-rw-r--r--   0 jim       (1026) users      (100)     1648 2023-04-13 09:47:03.000000 Photini-2023.4.0.1/src/lang/it/LC_MESSAGES/index.po
+-rw-r--r--   0 jim       (1026) users      (100)    75543 2023-04-13 09:47:07.000000 Photini-2023.4.0.1/src/lang/it/LC_MESSAGES/manual.po
+-rw-r--r--   0 jim       (1026) users      (100)     1171 2023-04-13 09:47:09.000000 Photini-2023.4.0.1/src/lang/it/LC_MESSAGES/misc.po
+-rw-r--r--   0 jim       (1026) users      (100)    41530 2023-04-13 09:47:12.000000 Photini-2023.4.0.1/src/lang/it/LC_MESSAGES/other.po
+-rw-r--r--   0 jim       (1026) users      (100)    95701 2023-04-13 09:47:38.000000 Photini-2023.4.0.1/src/lang/it/photini.ts
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/lang/ko/
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/lang/ko/LC_MESSAGES/
+-rw-r--r--   0 jim       (1026) users      (100)     2765 2023-04-13 09:47:04.000000 Photini-2023.4.0.1/src/lang/ko/LC_MESSAGES/index.po
+-rw-r--r--   0 jim       (1026) users      (100)   141558 2023-04-13 09:47:07.000000 Photini-2023.4.0.1/src/lang/ko/LC_MESSAGES/manual.po
+-rw-r--r--   0 jim       (1026) users      (100)     1662 2023-04-13 09:47:09.000000 Photini-2023.4.0.1/src/lang/ko/LC_MESSAGES/misc.po
+-rw-r--r--   0 jim       (1026) users      (100)    67188 2023-04-13 09:47:12.000000 Photini-2023.4.0.1/src/lang/ko/LC_MESSAGES/other.po
+-rw-r--r--   0 jim       (1026) users      (100)    95625 2023-04-13 09:47:38.000000 Photini-2023.4.0.1/src/lang/ko/photini.ts
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/lang/nb/
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/lang/nb/LC_MESSAGES/
+-rw-r--r--   0 jim       (1026) users      (100)     1781 2023-04-13 09:47:05.000000 Photini-2023.4.0.1/src/lang/nb/LC_MESSAGES/index.po
+-rw-r--r--   0 jim       (1026) users      (100)    75596 2023-04-13 09:47:08.000000 Photini-2023.4.0.1/src/lang/nb/LC_MESSAGES/manual.po
+-rw-r--r--   0 jim       (1026) users      (100)     1142 2023-04-13 09:47:10.000000 Photini-2023.4.0.1/src/lang/nb/LC_MESSAGES/misc.po
+-rw-r--r--   0 jim       (1026) users      (100)    41669 2023-04-13 09:47:12.000000 Photini-2023.4.0.1/src/lang/nb/LC_MESSAGES/other.po
+-rw-r--r--   0 jim       (1026) users      (100)    95337 2023-04-13 09:47:38.000000 Photini-2023.4.0.1/src/lang/nb/photini.ts
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/lang/pl/
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/lang/pl/LC_MESSAGES/
+-rw-r--r--   0 jim       (1026) users      (100)     1851 2023-04-13 09:47:05.000000 Photini-2023.4.0.1/src/lang/pl/LC_MESSAGES/index.po
+-rw-r--r--   0 jim       (1026) users      (100)    75727 2023-04-13 09:47:08.000000 Photini-2023.4.0.1/src/lang/pl/LC_MESSAGES/manual.po
+-rw-r--r--   0 jim       (1026) users      (100)     1277 2023-04-13 09:47:10.000000 Photini-2023.4.0.1/src/lang/pl/LC_MESSAGES/misc.po
+-rw-r--r--   0 jim       (1026) users      (100)    41743 2023-04-13 09:47:13.000000 Photini-2023.4.0.1/src/lang/pl/LC_MESSAGES/other.po
+-rw-r--r--   0 jim       (1026) users      (100)    95997 2023-04-13 09:47:38.000000 Photini-2023.4.0.1/src/lang/pl/photini.ts
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:53.000000 Photini-2023.4.0.1/src/lang/templates/
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/lang/templates/gettext/
+-rw-r--r--   0 jim       (1026) users      (100)     1508 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/lang/templates/gettext/index.pot
+-rw-r--r--   0 jim       (1026) users      (100)    72700 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/lang/templates/gettext/manual.pot
+-rw-r--r--   0 jim       (1026) users      (100)     1055 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/lang/templates/gettext/misc.pot
+-rw-r--r--   0 jim       (1026) users      (100)    40008 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/lang/templates/gettext/other.pot
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/lang/templates/qt/
+-rw-r--r--   0 jim       (1026) users      (100)    96788 2023-04-13 09:47:38.000000 Photini-2023.4.0.1/src/lang/templates/qt/photini.ts
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/photini/
+-rw-r--r--   0 jim       (1026) users      (100)      116 2023-04-13 09:46:40.000000 Photini-2023.4.0.1/src/photini/__init__.py
+-rw-r--r--   0 jim       (1026) users      (100)      917 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/__main__.py
+-rw-r--r--   0 jim       (1026) users      (100)    19879 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/address.py
+-rw-r--r--   0 jim       (1026) users      (100)     4759 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/bingmap.py
+-rw-r--r--   0 jim       (1026) users      (100)     5310 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/configstore.py
+-rw-r--r--   0 jim       (1026) users      (100)     6890 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/cv.py
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/photini/data/
+-rw-r--r--   0 jim       (1026) users      (100)    35147 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/data/LICENSE.txt
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/photini/data/bingmap/
+-rw-r--r--   0 jim       (1026) users      (100)     7556 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/data/bingmap/script.js
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/photini/data/googlemap/
+-rw-r--r--   0 jim       (1026) users      (100)     6239 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/data/googlemap/script.js
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/photini/data/icons/
+-rw-r--r--   0 jim       (1026) users      (100)    14554 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/data/icons/photini_128.png
+-rw-r--r--   0 jim       (1026) users      (100)     3262 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/data/icons/photini_48.png
+-rw-r--r--   0 jim       (1026) users      (100)    86598 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/data/icons/photini_win.ico
+-rw-r--r--   0 jim       (1026) users      (100)     2205 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/data/keys.txt
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/photini/data/lang/
+-rw-r--r--   0 jim       (1026) users      (100)    22137 2023-04-13 09:47:47.000000 Photini-2023.4.0.1/src/photini/data/lang/photini.ca.qm
+-rw-r--r--   0 jim       (1026) users      (100)    40194 2023-04-13 09:47:46.000000 Photini-2023.4.0.1/src/photini/data/lang/photini.cs.qm
+-rw-r--r--   0 jim       (1026) users      (100)    44214 2023-04-13 09:47:45.000000 Photini-2023.4.0.1/src/photini/data/lang/photini.de.qm
+-rw-r--r--   0 jim       (1026) users      (100)    28726 2023-04-13 09:47:45.000000 Photini-2023.4.0.1/src/photini/data/lang/photini.en.qm
+-rw-r--r--   0 jim       (1026) users      (100)    10112 2023-04-13 09:47:46.000000 Photini-2023.4.0.1/src/photini/data/lang/photini.es.qm
+-rw-r--r--   0 jim       (1026) users      (100)    41878 2023-04-13 09:47:45.000000 Photini-2023.4.0.1/src/photini/data/lang/photini.fr.qm
+-rw-r--r--   0 jim       (1026) users      (100)      923 2023-04-13 09:47:46.000000 Photini-2023.4.0.1/src/photini/data/lang/photini.it.qm
+-rw-r--r--   0 jim       (1026) users      (100)     2072 2023-04-13 09:47:47.000000 Photini-2023.4.0.1/src/photini/data/lang/photini.ko.qm
+-rw-r--r--   0 jim       (1026) users      (100)    19489 2023-04-13 09:47:47.000000 Photini-2023.4.0.1/src/photini/data/lang/photini.nb.qm
+-rw-r--r--   0 jim       (1026) users      (100)    10060 2023-04-13 09:47:47.000000 Photini-2023.4.0.1/src/photini/data/lang/photini.pl.qm
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/photini/data/linux/
+-rw-r--r--   0 jim       (1026) users      (100)      991 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/data/linux/photini.desktop
+-rw-r--r--   0 jim       (1026) users      (100)      209 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/data/map_circle_blue.png
+-rw-r--r--   0 jim       (1026) users      (100)      207 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/data/map_circle_red.png
+-rw-r--r--   0 jim       (1026) users      (100)     1867 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/data/map_pin_grey.png
+-rw-r--r--   0 jim       (1026) users      (100)     2016 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/data/map_pin_red.png
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/photini/data/mapboxmap/
+-rw-r--r--   0 jim       (1026) users      (100)     5715 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/data/mapboxmap/script.js
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/src/photini/data/windows/
+-rw-r--r--   0 jim       (1026) users      (100)     2638 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/data/windows/install_shortcuts.vbs
+-rw-r--r--   0 jim       (1026) users      (100)    13464 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/descriptive.py
+-rw-r--r--   0 jim       (1026) users      (100)    22760 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/editor.py
+-rw-r--r--   0 jim       (1026) users      (100)     7893 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/editsettings.py
+-rw-r--r--   0 jim       (1026) users      (100)    31789 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/exiv2.py
+-rw-r--r--   0 jim       (1026) users      (100)     3287 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/ffmpeg.py
+-rw-r--r--   0 jim       (1026) users      (100)    33292 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/flickr.py
+-rw-r--r--   0 jim       (1026) users      (100)     4191 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/googlemap.py
+-rw-r--r--   0 jim       (1026) users      (100)    13099 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/googlephotos.py
+-rw-r--r--   0 jim       (1026) users      (100)     4382 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/gpximporter.py
+-rw-r--r--   0 jim       (1026) users      (100)    40241 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/imagelist.py
+-rw-r--r--   0 jim       (1026) users      (100)    27611 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/importer.py
+-rw-r--r--   0 jim       (1026) users      (100)    27252 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/ipernity.py
+-rw-r--r--   0 jim       (1026) users      (100)     4396 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/loggerwindow.py
+-rw-r--r--   0 jim       (1026) users      (100)     4235 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/mapboxmap.py
+-rw-r--r--   0 jim       (1026) users      (100)    36681 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/metadata.py
+-rw-r--r--   0 jim       (1026) users      (100)    21920 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/ownership.py
+-rw-r--r--   0 jim       (1026) users      (100)    25534 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/photinimap.py
+-rw-r--r--   0 jim       (1026) users      (100)    37738 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/pixelfed.py
+-rw-r--r--   0 jim       (1026) users      (100)    10550 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/pyqt.py
+-rw-r--r--   0 jim       (1026) users      (100)    36517 2023-04-13 09:46:40.000000 Photini-2023.4.0.1/src/photini/regions.py
+-rw-r--r--   0 jim       (1026) users      (100)     6711 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/scripts.py
+-rw-r--r--   0 jim       (1026) users      (100)     3687 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/spelling.py
+-rw-r--r--   0 jim       (1026) users      (100)    40105 2023-04-13 09:46:40.000000 Photini-2023.4.0.1/src/photini/technical.py
+-rw-r--r--   0 jim       (1026) users      (100)    71730 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/types.py
+-rw-r--r--   0 jim       (1026) users      (100)    47911 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/photini/uploader.py
+-rw-r--r--   0 jim       (1026) users      (100)    34838 2023-04-13 09:46:40.000000 Photini-2023.4.0.1/src/photini/widgets.py
+-rw-r--r--   0 jim       (1026) users      (100)     1097 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/src/run_photini.py
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/utils/
+-rw-r--r--   0 jim       (1026) users      (100)     1257 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/utils/build_docs.py
+-rw-r--r--   0 jim       (1026) users      (100)     1511 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/utils/build_lang.py
+-rw-r--r--   0 jim       (1026) users      (100)     2723 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/utils/download_cvs.py
+-rw-r--r--   0 jim       (1026) users      (100)     8048 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/utils/lang_update.py
+-rw-r--r--   0 jim       (1026) users      (100)     2220 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/utils/localise_desktop.py
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-13 09:47:54.000000 Photini-2023.4.0.1/utils/make_icons/
+-rw-r--r--   0 jim       (1026) users      (100)      166 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/utils/make_icons/circle.fig
+-rw-r--r--   0 jim       (1026) users      (100)   178291 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/utils/make_icons/icon_master.png
+-rw-r--r--   0 jim       (1026) users      (100)     1279 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/utils/make_icons/makefile
+-rw-r--r--   0 jim       (1026) users      (100)     1539 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/utils/tag_release.py
+-rw-r--r--   0 jim       (1026) users      (100)     2846 2023-04-12 08:03:27.000000 Photini-2023.4.0.1/utils/update_version.py
```

### Comparing `Photini-2023.4.0/CHANGELOG.txt` & `Photini-2023.4.0.1/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/LICENSE.txt` & `Photini-2023.4.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/PKG-INFO` & `Photini-2023.4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: Photini
-Version: 2023.4.0
+Version: 2023.4.0.1
 Summary: Simple photo metadata editor
 Home-page: https://github.com/jim-easterbrook/Photini
 Author: Jim Easterbrook
 Author-email: jim@jim-easterbrook.me.uk
 License: GPLv3+
-Download-URL: https://github.com/jim-easterbrook/Photini/archive/2023.4.0.tar.gz
+Download-URL: https://github.com/jim-easterbrook/Photini/archive/2023.4.0.1.tar.gz
 Description: Photini
         =======
         
         A free, easy to use, digital photograph metadata (Exif, IPTC, XMP) editing application for Linux, Windows and MacOS.
         
         "Metadata" is said to mean "data about data".
         In the context of digital photographs this means information that isn't essential in order to display the image, but tells you something about it.
```

### Comparing `Photini-2023.4.0/README.rst` & `Photini-2023.4.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/setup.py` & `Photini-2023.4.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/Photini.egg-info/PKG-INFO` & `Photini-2023.4.0.1/src/Photini.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: Photini
-Version: 2023.4.0
+Version: 2023.4.0.1
 Summary: Simple photo metadata editor
 Home-page: https://github.com/jim-easterbrook/Photini
 Author: Jim Easterbrook
 Author-email: jim@jim-easterbrook.me.uk
 License: GPLv3+
-Download-URL: https://github.com/jim-easterbrook/Photini/archive/2023.4.0.tar.gz
+Download-URL: https://github.com/jim-easterbrook/Photini/archive/2023.4.0.1.tar.gz
 Description: Photini
         =======
         
         A free, easy to use, digital photograph metadata (Exif, IPTC, XMP) editing application for Linux, Windows and MacOS.
         
         "Metadata" is said to mean "data about data".
         In the context of digital photographs this means information that isn't essential in order to display the image, but tells you something about it.
```

### Comparing `Photini-2023.4.0/src/Photini.egg-info/SOURCES.txt` & `Photini-2023.4.0.1/src/Photini.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/Photini.egg-info/requires.txt` & `Photini-2023.4.0.1/src/Photini.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/DOC_LICENSE.txt` & `Photini-2023.4.0.1/src/doc/DOC_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/conf.py` & `Photini-2023.4.0.1/src/doc/conf.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/photini_logo.png` & `Photini-2023.4.0.1/src/doc/images/photini_logo.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_001.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_001.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_002.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_002.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_003.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_003.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_004.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_004.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_005.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_005.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_006.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_006.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_007.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_007.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_008.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_008.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_009.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_009.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_020.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_020.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_021.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_021.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_022.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_022.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_023.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_023.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_024.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_024.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_025.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_025.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_026.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_026.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_027.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_027.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_028.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_028.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_029.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_029.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_030.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_030.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_031.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_031.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_032.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_032.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_033.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_033.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_034.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_034.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_100.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_100.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_101.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_101.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_102.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_102.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_103.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_103.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_104.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_104.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_105.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_105.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_106.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_106.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_107.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_107.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_108.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_108.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_109.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_109.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_110.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_110.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_111.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_111.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_112.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_112.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_113.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_113.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_114.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_114.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_115.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_115.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_116.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_116.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_117.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_117.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_130.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_130.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_131.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_131.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_132.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_132.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_133.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_133.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_134.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_134.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_135.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_135.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_136.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_136.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_137.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_137.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_138.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_138.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_139.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_139.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_141.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_141.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_142.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_142.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_143.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_143.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_144.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_144.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_145.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_145.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_146.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_146.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_150.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_150.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_151a.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_151a.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_151d.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_151d.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_152.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_152.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_154.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_154.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_155.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_155.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_156.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_156.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_157.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_157.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_158.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_158.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_159.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_159.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_160.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_160.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_161.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_161.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_170.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_170.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_171.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_171.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_172.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_172.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_173.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_173.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_174.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_174.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_175.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_175.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_180.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_180.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_181.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_181.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_182.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_182.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_183.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_183.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_184.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_184.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_185.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_185.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_200.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_200.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_201.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_201.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_202.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_202.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_203.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_203.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_204.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_204.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_220.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_220.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_221.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_221.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_222.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_222.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_223.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_223.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_224.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_224.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_225.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_225.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_230.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_230.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_231.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_231.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_232.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_232.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_233.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_233.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_234.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_234.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_235.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_235.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_236.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_236.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_237.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_237.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_238.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_238.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_239.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_239.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_240.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_240.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_242.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_242.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_250.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_250.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_251.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_251.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_252.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_252.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_253.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_253.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_254.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_254.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_255.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_255.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_256.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_256.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_257.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_257.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_258.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_258.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_259.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_259.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_260.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_260.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_270.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_270.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_271.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_271.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_272.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_272.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_273.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_273.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_274.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_274.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_275.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_275.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_276.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_276.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_277.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_277.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_278.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_278.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_279.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_279.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_280.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_280.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_36.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_36.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/images/screenshot_37.png` & `Photini-2023.4.0.1/src/doc/images/screenshot_37.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/index.rst` & `Photini-2023.4.0.1/src/doc/index.rst`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/manual/address.rst` & `Photini-2023.4.0.1/src/doc/manual/address.rst`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/manual/configuration.rst` & `Photini-2023.4.0.1/src/doc/manual/configuration.rst`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/manual/descriptive_metadata.rst` & `Photini-2023.4.0.1/src/doc/manual/descriptive_metadata.rst`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/manual/extending.rst` & `Photini-2023.4.0.1/src/doc/manual/extending.rst`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/manual/flickr.rst` & `Photini-2023.4.0.1/src/doc/manual/flickr.rst`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/manual/google_photos.rst` & `Photini-2023.4.0.1/src/doc/manual/google_photos.rst`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/manual/image_selector.rst` & `Photini-2023.4.0.1/src/doc/manual/image_selector.rst`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/manual/importer.rst` & `Photini-2023.4.0.1/src/doc/manual/importer.rst`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/manual/index.rst` & `Photini-2023.4.0.1/src/doc/manual/index.rst`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/manual/ipernity.rst` & `Photini-2023.4.0.1/src/doc/manual/ipernity.rst`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/manual/map.rst` & `Photini-2023.4.0.1/src/doc/manual/map.rst`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/manual/ownership_metadata.rst` & `Photini-2023.4.0.1/src/doc/manual/ownership_metadata.rst`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/manual/pixelfed.rst` & `Photini-2023.4.0.1/src/doc/manual/pixelfed.rst`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/manual/regions.rst` & `Photini-2023.4.0.1/src/doc/manual/regions.rst`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/manual/tags.rst` & `Photini-2023.4.0.1/src/doc/manual/tags.rst`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/manual/technical_metadata.rst` & `Photini-2023.4.0.1/src/doc/manual/technical_metadata.rst`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/manual/video.rst` & `Photini-2023.4.0.1/src/doc/manual/video.rst`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/other/installation.rst` & `Photini-2023.4.0.1/src/doc/other/installation.rst`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/other/introduction.rst` & `Photini-2023.4.0.1/src/doc/other/introduction.rst`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/other/localisation.rst` & `Photini-2023.4.0.1/src/doc/other/localisation.rst`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/other/reading.rst` & `Photini-2023.4.0.1/src/doc/other/reading.rst`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/doc/other/workflow.rst` & `Photini-2023.4.0.1/src/doc/other/workflow.rst`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/README.rst` & `Photini-2023.4.0.1/src/lang/README.rst`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/ca/LC_MESSAGES/index.po` & `Photini-2023.4.0.1/src/lang/ca/LC_MESSAGES/index.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/ca/LC_MESSAGES/manual.po` & `Photini-2023.4.0.1/src/lang/ca/LC_MESSAGES/manual.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/ca/LC_MESSAGES/misc.po` & `Photini-2023.4.0.1/src/lang/ca/LC_MESSAGES/misc.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/ca/LC_MESSAGES/other.po` & `Photini-2023.4.0.1/src/lang/ca/LC_MESSAGES/other.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/ca/photini.ts` & `Photini-2023.4.0.1/src/lang/ca/photini.ts`

 * *Files 0% similar despite different names*

#### Comparing `Photini-2023.4.0/src/lang/ca/photini.ts` & `Photini-2023.4.0.1/src/lang/ca/photini.ts`

```diff
@@ -1008,20 +1008,20 @@
       <source>Set default language</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>LatLongDisplay</name>
     <message>
-      <location filename="../../photini/widgets.py" line="835"/>
+      <location filename="../../photini/widgets.py" line="834"/>
       <source>Lat, long</source>
       <translation>Lat, long</translation>
     </message>
     <message>
-      <location filename="../../photini/widgets.py" line="840"/>
+      <location filename="../../photini/widgets.py" line="839"/>
       <source>Latitude and longitude (in degrees) as two decimal numbers separated by a comma.</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>LoggerWindow</name>
     <message>
@@ -1698,362 +1698,362 @@
     </message>
     <message>
       <location filename="../../photini/regions.py" line="70"/>
       <source>New vertex</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="421"/>
+      <location filename="../../photini/regions.py" line="419"/>
       <source>Unreadable image format</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="597"/>
+      <location filename="../../photini/regions.py" line="595"/>
       <source>pixel</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="600"/>
+      <location filename="../../photini/regions.py" line="598"/>
       <source>A pixel of a digital image setting an absolute value.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="604"/>
+      <location filename="../../photini/regions.py" line="602"/>
       <source>relative</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="607"/>
+      <location filename="../../photini/regions.py" line="605"/>
       <source>Relative part of the size of an image along the x- or the y-axis.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="646"/>
+      <location filename="../../photini/regions.py" line="644"/>
       <source>Name</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="649"/>
+      <location filename="../../photini/regions.py" line="647"/>
       <source>Free-text name of the region. Should be unique among all Region Names of an image.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="658"/>
+      <location filename="../../photini/regions.py" line="656"/>
       <source>Identifier of the region. Must be unique among all Region Identifiers of an image. Does not have to be unique beyond the metadata of this image.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="660"/>
+      <location filename="../../photini/regions.py" line="658"/>
       <source>Identifier</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="666"/>
+      <location filename="../../photini/regions.py" line="664"/>
       <source>Unit used for measuring dimensions of the boundary of a region.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="669"/>
+      <location filename="../../photini/regions.py" line="667"/>
       <source>Boundary unit</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="676"/>
+      <location filename="../../photini/regions.py" line="674"/>
       <source>Role of this region among all regions of this image or of other images. The value SHOULD be taken from a Controlled Vocabulary.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="678"/>
+      <location filename="../../photini/regions.py" line="676"/>
       <source>Role</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="685"/>
+      <location filename="../../photini/regions.py" line="683"/>
       <source>The semantic type of what is shown inside the region. The value SHOULD be taken from a Controlled Vocabulary.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="688"/>
+      <location filename="../../photini/regions.py" line="686"/>
       <source>Content type</source>
       <translation>Tipus de contingut</translation>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="694"/>
+      <location filename="../../photini/regions.py" line="692"/>
       <source>Enter the names of people shown in this region. Separate multiple entries with &quot;;&quot; characters.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="697"/>
+      <location filename="../../photini/regions.py" line="695"/>
       <source>Person shown</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="701"/>
+      <location filename="../../photini/regions.py" line="699"/>
       <source>Description</source>
       <translation>Descripció</translation>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="704"/>
+      <location filename="../../photini/regions.py" line="702"/>
       <source>Enter a &quot;caption&quot; describing the who, what, and why of what is happening in this region.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="735"/>
+      <location filename="../../photini/regions.py" line="733"/>
       <source>The Image Region Structure includes optionally any metadata property which is related to the region.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="778"/>
+      <location filename="../../photini/regions.py" line="776"/>
       <source>New rectangle</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="780"/>
+      <location filename="../../photini/regions.py" line="778"/>
       <source>New circle</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="782"/>
+      <location filename="../../photini/regions.py" line="780"/>
       <source>New point</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="784"/>
+      <location filename="../../photini/regions.py" line="782"/>
       <source>New polygon</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="787"/>
+      <location filename="../../photini/regions.py" line="785"/>
       <source>Delete region</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="894"/>
+      <location filename="../../photini/regions.py" line="892"/>
       <source>Image &amp;Regions</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>TechnicalTab</name>
     <message>
-      <location filename="../../photini/technical.py" line="900"/>
+      <location filename="../../photini/technical.py" line="897"/>
       <source>min</source>
       <translation>min</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="901"/>
+      <location filename="../../photini/technical.py" line="898"/>
       <source>max</source>
       <translation>max</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="725"/>
-      <location filename="../../photini/technical.py" line="902"/>
+      <location filename="../../photini/technical.py" line="722"/>
+      <location filename="../../photini/technical.py" line="899"/>
       <source>Focal length</source>
       <translation>Distància focal</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="903"/>
+      <location filename="../../photini/technical.py" line="900"/>
       <source>Max aperture</source>
       <translation>Obertura màx</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="577"/>
+      <location filename="../../photini/technical.py" line="574"/>
       <source>Photini: define lens</source>
       <translation>Photini: define lens</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="538"/>
+      <location filename="../../photini/technical.py" line="535"/>
       <source>Model name</source>
       <translation>Nom del model</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="537"/>
+      <location filename="../../photini/technical.py" line="534"/>
       <source>Maker's name</source>
       <translation>Nom del fabricant</translation>
     </message>
     <message>
       <location filename="../../photini/technical.py" line="54"/>
       <source>Remove &quot;{camera_or_lens}&quot;</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="539"/>
+      <location filename="../../photini/technical.py" line="536"/>
       <source>Serial number</source>
       <translation>Número de serie</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="643"/>
+      <location filename="../../photini/technical.py" line="640"/>
       <source>&amp;Technical metadata</source>
       <translation>Medadades &amp;tècniques</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="651"/>
+      <location filename="../../photini/technical.py" line="648"/>
       <source>Date and time</source>
       <translation>Dia i hora</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="661"/>
+      <location filename="../../photini/technical.py" line="658"/>
       <source>Link 'taken' and 'digitised'</source>
       <translation>Enllaça 'capturades' i 'digitalitzades'</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="663"/>
+      <location filename="../../photini/technical.py" line="660"/>
       <source>Link 'digitised' and 'modified'</source>
       <translation>Enllaça 'digitalitzades' i 'modificades'</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="665"/>
+      <location filename="../../photini/technical.py" line="662"/>
       <source>Taken</source>
       <translation>Capturada</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="668"/>
+      <location filename="../../photini/technical.py" line="665"/>
       <source>Digitised</source>
       <translation>Digitalitzada</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="671"/>
+      <location filename="../../photini/technical.py" line="668"/>
       <source>Modified</source>
       <translation>Modificada</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="676"/>
+      <location filename="../../photini/technical.py" line="673"/>
       <source>Adjust times</source>
       <translation>Ajusta hores</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="680"/>
+      <location filename="../../photini/technical.py" line="677"/>
       <source>Other</source>
       <translation>Altres</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="704"/>
+      <location filename="../../photini/technical.py" line="701"/>
       <source>Orientation</source>
       <translation>Orientació</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="718"/>
+      <location filename="../../photini/technical.py" line="715"/>
       <source>Lens model</source>
       <translation>Model de lent</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="928"/>
+      <location filename="../../photini/technical.py" line="925"/>
       <source>Update aperture &amp; focal length</source>
       <translation>Actualitza obertura &amp; distància focal</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="930"/>
+      <location filename="../../photini/technical.py" line="927"/>
       <source>Adjust image aperture and focal length to agree with lens specification?</source>
       <translation>Ajustar la obertura de la imatge i la distància focal per coincidir amb les característiques de les lents?</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="597"/>
+      <location filename="../../photini/technical.py" line="594"/>
       <source>Minimum focal length</source>
       <translation>Distància focal mínima</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="599"/>
+      <location filename="../../photini/technical.py" line="596"/>
       <source>Aperture at min. focal length</source>
       <translation>Obertura al min. distància focal</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="600"/>
+      <location filename="../../photini/technical.py" line="597"/>
       <source>Maximum focal length</source>
       <translation>Distància focal màxima</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="602"/>
+      <location filename="../../photini/technical.py" line="599"/>
       <source>Aperture at max. focal length</source>
       <translation>Obertura al max. distància focal</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="732"/>
+      <location filename="../../photini/technical.py" line="729"/>
       <source>35mm equiv</source>
       <translation>equiv. 35 mm</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="739"/>
+      <location filename="../../photini/technical.py" line="736"/>
       <source>Aperture</source>
       <translation>Obertura</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="563"/>
+      <location filename="../../photini/technical.py" line="560"/>
       <source>Photini: define camera</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="711"/>
+      <location filename="../../photini/technical.py" line="708"/>
       <source>Camera</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="818"/>
+      <location filename="../../photini/technical.py" line="815"/>
       <source>Photini: maker name change</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="824"/>
+      <location filename="../../photini/technical.py" line="821"/>
       <source>Do you want to delete the Exif makernote?</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="821"/>
+      <location filename="../../photini/technical.py" line="818"/>
       <source>Changing maker name will invalidate Exif makernote information.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="687"/>
+      <location filename="../../photini/technical.py" line="684"/>
       <source>normal</source>
       <comment>orientation dropdown, no transformation</comment>
       <translation>normal</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="695"/>
+      <location filename="../../photini/technical.py" line="692"/>
       <source>reflect left to right</source>
       <comment>orientation dropdown, horizontal reflection</comment>
       <translation>reflexa esquerra-dreta</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="697"/>
+      <location filename="../../photini/technical.py" line="694"/>
       <source>reflect top to bottom</source>
       <comment>orientation dropdown, vertical reflection</comment>
       <translation>reflexa dalt-baix</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="699"/>
+      <location filename="../../photini/technical.py" line="696"/>
       <source>reflect top right to bottom left</source>
       <comment>orientation dropdown, diagonal reflection</comment>
       <translation>reflexa dd-be</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="701"/>
+      <location filename="../../photini/technical.py" line="698"/>
       <source>reflect top left to bottom right</source>
       <comment>orientation dropdown, diagonal reflection</comment>
       <translation>reflexa de-bd</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="689"/>
+      <location filename="../../photini/technical.py" line="686"/>
       <source>rotate -90°</source>
       <comment>orientation dropdown</comment>
       <translation>gira -90</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="691"/>
+      <location filename="../../photini/technical.py" line="688"/>
       <source>rotate +90°</source>
       <comment>orientation dropdown</comment>
       <translation>gira +90</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="693"/>
+      <location filename="../../photini/technical.py" line="690"/>
       <source>rotate 180°</source>
       <comment>orientation dropdown</comment>
       <translation>gira 180</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="387"/>
+      <location filename="../../photini/technical.py" line="384"/>
       <source>Precision</source>
       <translation>Precissió</translation>
     </message>
   </context>
   <context>
     <name>UploaderTabsAll</name>
     <message>
```

### Comparing `Photini-2023.4.0/src/lang/cs/LC_MESSAGES/index.po` & `Photini-2023.4.0.1/src/lang/cs/LC_MESSAGES/index.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/cs/LC_MESSAGES/manual.po` & `Photini-2023.4.0.1/src/lang/cs/LC_MESSAGES/manual.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/cs/LC_MESSAGES/misc.po` & `Photini-2023.4.0.1/src/lang/cs/LC_MESSAGES/misc.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/cs/LC_MESSAGES/other.po` & `Photini-2023.4.0.1/src/lang/cs/LC_MESSAGES/other.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/cs/photini.ts` & `Photini-2023.4.0.1/src/lang/cs/photini.ts`

 * *Files 1% similar despite different names*

#### Comparing `Photini-2023.4.0/src/lang/cs/photini.ts` & `Photini-2023.4.0.1/src/lang/cs/photini.ts`

```diff
@@ -1012,20 +1012,20 @@
       <source>Set default language</source>
       <translation>Nastavit výchozí jazyk</translation>
     </message>
   </context>
   <context>
     <name>LatLongDisplay</name>
     <message>
-      <location filename="../../photini/widgets.py" line="835"/>
+      <location filename="../../photini/widgets.py" line="834"/>
       <source>Lat, long</source>
       <translation>Zeměpisná šířka, délka</translation>
     </message>
     <message>
-      <location filename="../../photini/widgets.py" line="840"/>
+      <location filename="../../photini/widgets.py" line="839"/>
       <source>Latitude and longitude (in degrees) as two decimal numbers separated by a comma.</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>LoggerWindow</name>
     <message>
@@ -1702,362 +1702,362 @@
     </message>
     <message>
       <location filename="../../photini/regions.py" line="70"/>
       <source>New vertex</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="421"/>
+      <location filename="../../photini/regions.py" line="419"/>
       <source>Unreadable image format</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="597"/>
+      <location filename="../../photini/regions.py" line="595"/>
       <source>pixel</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="600"/>
+      <location filename="../../photini/regions.py" line="598"/>
       <source>A pixel of a digital image setting an absolute value.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="604"/>
+      <location filename="../../photini/regions.py" line="602"/>
       <source>relative</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="607"/>
+      <location filename="../../photini/regions.py" line="605"/>
       <source>Relative part of the size of an image along the x- or the y-axis.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="646"/>
+      <location filename="../../photini/regions.py" line="644"/>
       <source>Name</source>
       <translation>Název</translation>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="649"/>
+      <location filename="../../photini/regions.py" line="647"/>
       <source>Free-text name of the region. Should be unique among all Region Names of an image.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="658"/>
+      <location filename="../../photini/regions.py" line="656"/>
       <source>Identifier of the region. Must be unique among all Region Identifiers of an image. Does not have to be unique beyond the metadata of this image.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="660"/>
+      <location filename="../../photini/regions.py" line="658"/>
       <source>Identifier</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="666"/>
+      <location filename="../../photini/regions.py" line="664"/>
       <source>Unit used for measuring dimensions of the boundary of a region.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="669"/>
+      <location filename="../../photini/regions.py" line="667"/>
       <source>Boundary unit</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="676"/>
+      <location filename="../../photini/regions.py" line="674"/>
       <source>Role of this region among all regions of this image or of other images. The value SHOULD be taken from a Controlled Vocabulary.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="678"/>
+      <location filename="../../photini/regions.py" line="676"/>
       <source>Role</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="685"/>
+      <location filename="../../photini/regions.py" line="683"/>
       <source>The semantic type of what is shown inside the region. The value SHOULD be taken from a Controlled Vocabulary.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="688"/>
+      <location filename="../../photini/regions.py" line="686"/>
       <source>Content type</source>
       <translation>Typ obsahu</translation>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="694"/>
+      <location filename="../../photini/regions.py" line="692"/>
       <source>Enter the names of people shown in this region. Separate multiple entries with &quot;;&quot; characters.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="697"/>
+      <location filename="../../photini/regions.py" line="695"/>
       <source>Person shown</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="701"/>
+      <location filename="../../photini/regions.py" line="699"/>
       <source>Description</source>
       <translation>Popis</translation>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="704"/>
+      <location filename="../../photini/regions.py" line="702"/>
       <source>Enter a &quot;caption&quot; describing the who, what, and why of what is happening in this region.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="735"/>
+      <location filename="../../photini/regions.py" line="733"/>
       <source>The Image Region Structure includes optionally any metadata property which is related to the region.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="778"/>
+      <location filename="../../photini/regions.py" line="776"/>
       <source>New rectangle</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="780"/>
+      <location filename="../../photini/regions.py" line="778"/>
       <source>New circle</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="782"/>
+      <location filename="../../photini/regions.py" line="780"/>
       <source>New point</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="784"/>
+      <location filename="../../photini/regions.py" line="782"/>
       <source>New polygon</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="787"/>
+      <location filename="../../photini/regions.py" line="785"/>
       <source>Delete region</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="894"/>
+      <location filename="../../photini/regions.py" line="892"/>
       <source>Image &amp;Regions</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>TechnicalTab</name>
     <message>
-      <location filename="../../photini/technical.py" line="900"/>
+      <location filename="../../photini/technical.py" line="897"/>
       <source>min</source>
       <translation>min</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="901"/>
+      <location filename="../../photini/technical.py" line="898"/>
       <source>max</source>
       <translation>max</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="725"/>
-      <location filename="../../photini/technical.py" line="902"/>
+      <location filename="../../photini/technical.py" line="722"/>
+      <location filename="../../photini/technical.py" line="899"/>
       <source>Focal length</source>
       <translation>Ohnisková vzdálenost</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="903"/>
+      <location filename="../../photini/technical.py" line="900"/>
       <source>Max aperture</source>
       <translation>Největší clona</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="577"/>
+      <location filename="../../photini/technical.py" line="574"/>
       <source>Photini: define lens</source>
       <translation>Stanovit objektiv</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="538"/>
+      <location filename="../../photini/technical.py" line="535"/>
       <source>Model name</source>
       <translation>Název modelu</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="537"/>
+      <location filename="../../photini/technical.py" line="534"/>
       <source>Maker's name</source>
       <translation>Název výrobce</translation>
     </message>
     <message>
       <location filename="../../photini/technical.py" line="54"/>
       <source>Remove &quot;{camera_or_lens}&quot;</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="539"/>
+      <location filename="../../photini/technical.py" line="536"/>
       <source>Serial number</source>
       <translation>Sériové číslo</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="643"/>
+      <location filename="../../photini/technical.py" line="640"/>
       <source>&amp;Technical metadata</source>
       <translation>&amp;Technické popisné údaje</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="651"/>
+      <location filename="../../photini/technical.py" line="648"/>
       <source>Date and time</source>
       <translation>Datum a čas</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="661"/>
+      <location filename="../../photini/technical.py" line="658"/>
       <source>Link 'taken' and 'digitised'</source>
       <translation>Odkaz vzat a digitalizován</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="663"/>
+      <location filename="../../photini/technical.py" line="660"/>
       <source>Link 'digitised' and 'modified'</source>
       <translation>Odkaz digitalizován a změněn</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="665"/>
+      <location filename="../../photini/technical.py" line="662"/>
       <source>Taken</source>
       <translation>Vzat</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="668"/>
+      <location filename="../../photini/technical.py" line="665"/>
       <source>Digitised</source>
       <translation>Digitalizován</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="671"/>
+      <location filename="../../photini/technical.py" line="668"/>
       <source>Modified</source>
       <translation>Změněn</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="676"/>
+      <location filename="../../photini/technical.py" line="673"/>
       <source>Adjust times</source>
       <translation>Upravit časy</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="680"/>
+      <location filename="../../photini/technical.py" line="677"/>
       <source>Other</source>
       <translation>Jiné</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="704"/>
+      <location filename="../../photini/technical.py" line="701"/>
       <source>Orientation</source>
       <translation>Natočení</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="718"/>
+      <location filename="../../photini/technical.py" line="715"/>
       <source>Lens model</source>
       <translation>Model objektivu</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="928"/>
+      <location filename="../../photini/technical.py" line="925"/>
       <source>Update aperture &amp; focal length</source>
       <translation>Aktualizovat clonu a ohniskovou vzdálenost</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="930"/>
+      <location filename="../../photini/technical.py" line="927"/>
       <source>Adjust image aperture and focal length to agree with lens specification?</source>
       <translation>Upravit clonu obrázku a ohniskovou délku, aby souhlasily se specifikací objektivu?</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="597"/>
+      <location filename="../../photini/technical.py" line="594"/>
       <source>Minimum focal length</source>
       <translation>Nejmenší ohnisková vzdálenost</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="599"/>
+      <location filename="../../photini/technical.py" line="596"/>
       <source>Aperture at min. focal length</source>
       <translation>Clona při nejmenší ohniskové vzdálenosti</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="600"/>
+      <location filename="../../photini/technical.py" line="597"/>
       <source>Maximum focal length</source>
       <translation>Největší ohnisková vzdálenost</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="602"/>
+      <location filename="../../photini/technical.py" line="599"/>
       <source>Aperture at max. focal length</source>
       <translation>Clona při největší ohniskové vzdálenosti</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="732"/>
+      <location filename="../../photini/technical.py" line="729"/>
       <source>35mm equiv</source>
       <translation>35 mm equiv</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="739"/>
+      <location filename="../../photini/technical.py" line="736"/>
       <source>Aperture</source>
       <translation>Clona</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="563"/>
+      <location filename="../../photini/technical.py" line="560"/>
       <source>Photini: define camera</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="711"/>
+      <location filename="../../photini/technical.py" line="708"/>
       <source>Camera</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="818"/>
+      <location filename="../../photini/technical.py" line="815"/>
       <source>Photini: maker name change</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="824"/>
+      <location filename="../../photini/technical.py" line="821"/>
       <source>Do you want to delete the Exif makernote?</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="821"/>
+      <location filename="../../photini/technical.py" line="818"/>
       <source>Changing maker name will invalidate Exif makernote information.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="687"/>
+      <location filename="../../photini/technical.py" line="684"/>
       <source>normal</source>
       <comment>orientation dropdown, no transformation</comment>
       <translation>Normální</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="695"/>
+      <location filename="../../photini/technical.py" line="692"/>
       <source>reflect left to right</source>
       <comment>orientation dropdown, horizontal reflection</comment>
       <translation>Odrážet vlevo-vpravo</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="697"/>
+      <location filename="../../photini/technical.py" line="694"/>
       <source>reflect top to bottom</source>
       <comment>orientation dropdown, vertical reflection</comment>
       <translation>Odrážet nahoře-dole</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="699"/>
+      <location filename="../../photini/technical.py" line="696"/>
       <source>reflect top right to bottom left</source>
       <comment>orientation dropdown, diagonal reflection</comment>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="701"/>
+      <location filename="../../photini/technical.py" line="698"/>
       <source>reflect top left to bottom right</source>
       <comment>orientation dropdown, diagonal reflection</comment>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="689"/>
+      <location filename="../../photini/technical.py" line="686"/>
       <source>rotate -90°</source>
       <comment>orientation dropdown</comment>
       <translation>Otočit o -90°</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="691"/>
+      <location filename="../../photini/technical.py" line="688"/>
       <source>rotate +90°</source>
       <comment>orientation dropdown</comment>
       <translation>Otočit o +90°</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="693"/>
+      <location filename="../../photini/technical.py" line="690"/>
       <source>rotate 180°</source>
       <comment>orientation dropdown</comment>
       <translation>Otočit o 180°</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="387"/>
+      <location filename="../../photini/technical.py" line="384"/>
       <source>Precision</source>
       <translation>Přesnost</translation>
     </message>
   </context>
   <context>
     <name>UploaderTabsAll</name>
     <message>
```

### Comparing `Photini-2023.4.0/src/lang/de/LC_MESSAGES/index.po` & `Photini-2023.4.0.1/src/lang/de/LC_MESSAGES/index.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/de/LC_MESSAGES/manual.po` & `Photini-2023.4.0.1/src/lang/de/LC_MESSAGES/manual.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/de/LC_MESSAGES/misc.po` & `Photini-2023.4.0.1/src/lang/de/LC_MESSAGES/misc.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/de/LC_MESSAGES/other.po` & `Photini-2023.4.0.1/src/lang/de/LC_MESSAGES/other.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/de/photini.ts` & `Photini-2023.4.0.1/src/lang/de/photini.ts`

 * *Files 0% similar despite different names*

#### Comparing `Photini-2023.4.0/src/lang/de/photini.ts` & `Photini-2023.4.0.1/src/lang/de/photini.ts`

```diff
@@ -1008,20 +1008,20 @@
       <source>Set default language</source>
       <translation>Standardsprache festlegen</translation>
     </message>
   </context>
   <context>
     <name>LatLongDisplay</name>
     <message>
-      <location filename="../../photini/widgets.py" line="835"/>
+      <location filename="../../photini/widgets.py" line="834"/>
       <source>Lat, long</source>
       <translation>Breite, Länge</translation>
     </message>
     <message>
-      <location filename="../../photini/widgets.py" line="840"/>
+      <location filename="../../photini/widgets.py" line="839"/>
       <source>Latitude and longitude (in degrees) as two decimal numbers separated by a comma.</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>LoggerWindow</name>
     <message>
@@ -1698,362 +1698,362 @@
     </message>
     <message>
       <location filename="../../photini/regions.py" line="70"/>
       <source>New vertex</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="421"/>
+      <location filename="../../photini/regions.py" line="419"/>
       <source>Unreadable image format</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="597"/>
+      <location filename="../../photini/regions.py" line="595"/>
       <source>pixel</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="600"/>
+      <location filename="../../photini/regions.py" line="598"/>
       <source>A pixel of a digital image setting an absolute value.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="604"/>
+      <location filename="../../photini/regions.py" line="602"/>
       <source>relative</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="607"/>
+      <location filename="../../photini/regions.py" line="605"/>
       <source>Relative part of the size of an image along the x- or the y-axis.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="646"/>
+      <location filename="../../photini/regions.py" line="644"/>
       <source>Name</source>
       <translation>Name</translation>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="649"/>
+      <location filename="../../photini/regions.py" line="647"/>
       <source>Free-text name of the region. Should be unique among all Region Names of an image.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="658"/>
+      <location filename="../../photini/regions.py" line="656"/>
       <source>Identifier of the region. Must be unique among all Region Identifiers of an image. Does not have to be unique beyond the metadata of this image.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="660"/>
+      <location filename="../../photini/regions.py" line="658"/>
       <source>Identifier</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="666"/>
+      <location filename="../../photini/regions.py" line="664"/>
       <source>Unit used for measuring dimensions of the boundary of a region.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="669"/>
+      <location filename="../../photini/regions.py" line="667"/>
       <source>Boundary unit</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="676"/>
+      <location filename="../../photini/regions.py" line="674"/>
       <source>Role of this region among all regions of this image or of other images. The value SHOULD be taken from a Controlled Vocabulary.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="678"/>
+      <location filename="../../photini/regions.py" line="676"/>
       <source>Role</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="685"/>
+      <location filename="../../photini/regions.py" line="683"/>
       <source>The semantic type of what is shown inside the region. The value SHOULD be taken from a Controlled Vocabulary.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="688"/>
+      <location filename="../../photini/regions.py" line="686"/>
       <source>Content type</source>
       <translation>Inhaltstyp</translation>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="694"/>
+      <location filename="../../photini/regions.py" line="692"/>
       <source>Enter the names of people shown in this region. Separate multiple entries with &quot;;&quot; characters.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="697"/>
+      <location filename="../../photini/regions.py" line="695"/>
       <source>Person shown</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="701"/>
+      <location filename="../../photini/regions.py" line="699"/>
       <source>Description</source>
       <translation>Beschreibung</translation>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="704"/>
+      <location filename="../../photini/regions.py" line="702"/>
       <source>Enter a &quot;caption&quot; describing the who, what, and why of what is happening in this region.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="735"/>
+      <location filename="../../photini/regions.py" line="733"/>
       <source>The Image Region Structure includes optionally any metadata property which is related to the region.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="778"/>
+      <location filename="../../photini/regions.py" line="776"/>
       <source>New rectangle</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="780"/>
+      <location filename="../../photini/regions.py" line="778"/>
       <source>New circle</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="782"/>
+      <location filename="../../photini/regions.py" line="780"/>
       <source>New point</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="784"/>
+      <location filename="../../photini/regions.py" line="782"/>
       <source>New polygon</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="787"/>
+      <location filename="../../photini/regions.py" line="785"/>
       <source>Delete region</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="894"/>
+      <location filename="../../photini/regions.py" line="892"/>
       <source>Image &amp;Regions</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>TechnicalTab</name>
     <message>
-      <location filename="../../photini/technical.py" line="900"/>
+      <location filename="../../photini/technical.py" line="897"/>
       <source>min</source>
       <translation>min</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="901"/>
+      <location filename="../../photini/technical.py" line="898"/>
       <source>max</source>
       <translation>max</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="725"/>
-      <location filename="../../photini/technical.py" line="902"/>
+      <location filename="../../photini/technical.py" line="722"/>
+      <location filename="../../photini/technical.py" line="899"/>
       <source>Focal length</source>
       <translation>Brennweite</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="903"/>
+      <location filename="../../photini/technical.py" line="900"/>
       <source>Max aperture</source>
       <translation>Max. Blende</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="577"/>
+      <location filename="../../photini/technical.py" line="574"/>
       <source>Photini: define lens</source>
       <translation>Photini: Linse definieren</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="538"/>
+      <location filename="../../photini/technical.py" line="535"/>
       <source>Model name</source>
       <translation>Modellname</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="537"/>
+      <location filename="../../photini/technical.py" line="534"/>
       <source>Maker's name</source>
       <translation>Herstellername</translation>
     </message>
     <message>
       <location filename="../../photini/technical.py" line="54"/>
       <source>Remove &quot;{camera_or_lens}&quot;</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="539"/>
+      <location filename="../../photini/technical.py" line="536"/>
       <source>Serial number</source>
       <translation>Seriennummer</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="643"/>
+      <location filename="../../photini/technical.py" line="640"/>
       <source>&amp;Technical metadata</source>
       <translation>&amp;Technische Metadaten</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="651"/>
+      <location filename="../../photini/technical.py" line="648"/>
       <source>Date and time</source>
       <translation>Datum und Uhrzeit</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="661"/>
+      <location filename="../../photini/technical.py" line="658"/>
       <source>Link 'taken' and 'digitised'</source>
       <translation>Aufgenommen und Digitalisiert koppeln</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="663"/>
+      <location filename="../../photini/technical.py" line="660"/>
       <source>Link 'digitised' and 'modified'</source>
       <translation>Digitalisiert und Verändert koppeln</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="665"/>
+      <location filename="../../photini/technical.py" line="662"/>
       <source>Taken</source>
       <translation>Aufgenommen</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="668"/>
+      <location filename="../../photini/technical.py" line="665"/>
       <source>Digitised</source>
       <translation>Digitalisiert</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="671"/>
+      <location filename="../../photini/technical.py" line="668"/>
       <source>Modified</source>
       <translation>Verändert</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="676"/>
+      <location filename="../../photini/technical.py" line="673"/>
       <source>Adjust times</source>
       <translation>Uhrzeiten anpassen</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="680"/>
+      <location filename="../../photini/technical.py" line="677"/>
       <source>Other</source>
       <translation>Andere</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="704"/>
+      <location filename="../../photini/technical.py" line="701"/>
       <source>Orientation</source>
       <translation>Ausrichtung</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="718"/>
+      <location filename="../../photini/technical.py" line="715"/>
       <source>Lens model</source>
       <translation>Linsenmodell</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="928"/>
+      <location filename="../../photini/technical.py" line="925"/>
       <source>Update aperture &amp; focal length</source>
       <translation>Blende und Brennweite aktualisieren</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="930"/>
+      <location filename="../../photini/technical.py" line="927"/>
       <source>Adjust image aperture and focal length to agree with lens specification?</source>
       <translation>Blende und Brennweite aus Objektivdaten übernehmen?</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="597"/>
+      <location filename="../../photini/technical.py" line="594"/>
       <source>Minimum focal length</source>
       <translation>Minimale Brennweite</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="599"/>
+      <location filename="../../photini/technical.py" line="596"/>
       <source>Aperture at min. focal length</source>
       <translation>Blende bei min. Brennweite</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="600"/>
+      <location filename="../../photini/technical.py" line="597"/>
       <source>Maximum focal length</source>
       <translation>Maximale Brennweite</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="602"/>
+      <location filename="../../photini/technical.py" line="599"/>
       <source>Aperture at max. focal length</source>
       <translation>Blende bei max. Brennweite</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="732"/>
+      <location filename="../../photini/technical.py" line="729"/>
       <source>35mm equiv</source>
       <translation>35mm equiv</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="739"/>
+      <location filename="../../photini/technical.py" line="736"/>
       <source>Aperture</source>
       <translation>Blende</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="563"/>
+      <location filename="../../photini/technical.py" line="560"/>
       <source>Photini: define camera</source>
       <translation>Photini: Kamera definieren</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="711"/>
+      <location filename="../../photini/technical.py" line="708"/>
       <source>Camera</source>
       <translation>Kamera</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="818"/>
+      <location filename="../../photini/technical.py" line="815"/>
       <source>Photini: maker name change</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="824"/>
+      <location filename="../../photini/technical.py" line="821"/>
       <source>Do you want to delete the Exif makernote?</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="821"/>
+      <location filename="../../photini/technical.py" line="818"/>
       <source>Changing maker name will invalidate Exif makernote information.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="687"/>
+      <location filename="../../photini/technical.py" line="684"/>
       <source>normal</source>
       <comment>orientation dropdown, no transformation</comment>
       <translation>normal</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="695"/>
+      <location filename="../../photini/technical.py" line="692"/>
       <source>reflect left to right</source>
       <comment>orientation dropdown, horizontal reflection</comment>
       <translation>links-rechts spiegeln</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="697"/>
+      <location filename="../../photini/technical.py" line="694"/>
       <source>reflect top to bottom</source>
       <comment>orientation dropdown, vertical reflection</comment>
       <translation>oben-unten spiegeln</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="699"/>
+      <location filename="../../photini/technical.py" line="696"/>
       <source>reflect top right to bottom left</source>
       <comment>orientation dropdown, diagonal reflection</comment>
       <translation>rechts oben-links unten spiegeln</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="701"/>
+      <location filename="../../photini/technical.py" line="698"/>
       <source>reflect top left to bottom right</source>
       <comment>orientation dropdown, diagonal reflection</comment>
       <translation>links oben-rechts unten spiegeln</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="689"/>
+      <location filename="../../photini/technical.py" line="686"/>
       <source>rotate -90°</source>
       <comment>orientation dropdown</comment>
       <translation>90 Grad gegen Uhrzeigersinn drehen</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="691"/>
+      <location filename="../../photini/technical.py" line="688"/>
       <source>rotate +90°</source>
       <comment>orientation dropdown</comment>
       <translation>90 Grad im Uhrzeigersinn drehen</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="693"/>
+      <location filename="../../photini/technical.py" line="690"/>
       <source>rotate 180°</source>
       <comment>orientation dropdown</comment>
       <translation>180 Grad im Uhrzeigersinn drehen</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="387"/>
+      <location filename="../../photini/technical.py" line="384"/>
       <source>Precision</source>
       <translation>Genauigkeit</translation>
     </message>
   </context>
   <context>
     <name>UploaderTabsAll</name>
     <message>
```

### Comparing `Photini-2023.4.0/src/lang/en/photini.ts` & `Photini-2023.4.0.1/src/lang/en/photini.ts`

 * *Files 0% similar despite different names*

#### Comparing `Photini-2023.4.0/src/lang/en/photini.ts` & `Photini-2023.4.0.1/src/lang/en/photini.ts`

```diff
@@ -1008,20 +1008,20 @@
       <source>Set default language</source>
       <translation/>
     </message>
   </context>
   <context>
     <name>LatLongDisplay</name>
     <message>
-      <location filename="../../photini/widgets.py" line="835"/>
+      <location filename="../../photini/widgets.py" line="834"/>
       <source>Lat, long</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/widgets.py" line="840"/>
+      <location filename="../../photini/widgets.py" line="839"/>
       <source>Latitude and longitude (in degrees) as two decimal numbers separated by a comma.</source>
       <translation/>
     </message>
   </context>
   <context>
     <name>LoggerWindow</name>
     <message>
@@ -1698,362 +1698,362 @@
     </message>
     <message>
       <location filename="../../photini/regions.py" line="70"/>
       <source>New vertex</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="421"/>
+      <location filename="../../photini/regions.py" line="419"/>
       <source>Unreadable image format</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="597"/>
+      <location filename="../../photini/regions.py" line="595"/>
       <source>pixel</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="600"/>
+      <location filename="../../photini/regions.py" line="598"/>
       <source>A pixel of a digital image setting an absolute value.</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="604"/>
+      <location filename="../../photini/regions.py" line="602"/>
       <source>relative</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="607"/>
+      <location filename="../../photini/regions.py" line="605"/>
       <source>Relative part of the size of an image along the x- or the y-axis.</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="646"/>
+      <location filename="../../photini/regions.py" line="644"/>
       <source>Name</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="649"/>
+      <location filename="../../photini/regions.py" line="647"/>
       <source>Free-text name of the region. Should be unique among all Region Names of an image.</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="658"/>
+      <location filename="../../photini/regions.py" line="656"/>
       <source>Identifier of the region. Must be unique among all Region Identifiers of an image. Does not have to be unique beyond the metadata of this image.</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="660"/>
+      <location filename="../../photini/regions.py" line="658"/>
       <source>Identifier</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="666"/>
+      <location filename="../../photini/regions.py" line="664"/>
       <source>Unit used for measuring dimensions of the boundary of a region.</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="669"/>
+      <location filename="../../photini/regions.py" line="667"/>
       <source>Boundary unit</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="676"/>
+      <location filename="../../photini/regions.py" line="674"/>
       <source>Role of this region among all regions of this image or of other images. The value SHOULD be taken from a Controlled Vocabulary.</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="678"/>
+      <location filename="../../photini/regions.py" line="676"/>
       <source>Role</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="685"/>
+      <location filename="../../photini/regions.py" line="683"/>
       <source>The semantic type of what is shown inside the region. The value SHOULD be taken from a Controlled Vocabulary.</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="688"/>
+      <location filename="../../photini/regions.py" line="686"/>
       <source>Content type</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="694"/>
+      <location filename="../../photini/regions.py" line="692"/>
       <source>Enter the names of people shown in this region. Separate multiple entries with &quot;;&quot; characters.</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="697"/>
+      <location filename="../../photini/regions.py" line="695"/>
       <source>Person shown</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="701"/>
+      <location filename="../../photini/regions.py" line="699"/>
       <source>Description</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="704"/>
+      <location filename="../../photini/regions.py" line="702"/>
       <source>Enter a &quot;caption&quot; describing the who, what, and why of what is happening in this region.</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="735"/>
+      <location filename="../../photini/regions.py" line="733"/>
       <source>The Image Region Structure includes optionally any metadata property which is related to the region.</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="778"/>
+      <location filename="../../photini/regions.py" line="776"/>
       <source>New rectangle</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="780"/>
+      <location filename="../../photini/regions.py" line="778"/>
       <source>New circle</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="782"/>
+      <location filename="../../photini/regions.py" line="780"/>
       <source>New point</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="784"/>
+      <location filename="../../photini/regions.py" line="782"/>
       <source>New polygon</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="787"/>
+      <location filename="../../photini/regions.py" line="785"/>
       <source>Delete region</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="894"/>
+      <location filename="../../photini/regions.py" line="892"/>
       <source>Image &amp;Regions</source>
       <translation/>
     </message>
   </context>
   <context>
     <name>TechnicalTab</name>
     <message>
-      <location filename="../../photini/technical.py" line="900"/>
+      <location filename="../../photini/technical.py" line="897"/>
       <source>min</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="901"/>
+      <location filename="../../photini/technical.py" line="898"/>
       <source>max</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="725"/>
-      <location filename="../../photini/technical.py" line="902"/>
+      <location filename="../../photini/technical.py" line="722"/>
+      <location filename="../../photini/technical.py" line="899"/>
       <source>Focal length</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="903"/>
+      <location filename="../../photini/technical.py" line="900"/>
       <source>Max aperture</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="577"/>
+      <location filename="../../photini/technical.py" line="574"/>
       <source>Photini: define lens</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="538"/>
+      <location filename="../../photini/technical.py" line="535"/>
       <source>Model name</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="537"/>
+      <location filename="../../photini/technical.py" line="534"/>
       <source>Maker's name</source>
       <translation/>
     </message>
     <message>
       <location filename="../../photini/technical.py" line="54"/>
       <source>Remove &quot;{camera_or_lens}&quot;</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="539"/>
+      <location filename="../../photini/technical.py" line="536"/>
       <source>Serial number</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="643"/>
+      <location filename="../../photini/technical.py" line="640"/>
       <source>&amp;Technical metadata</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="651"/>
+      <location filename="../../photini/technical.py" line="648"/>
       <source>Date and time</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="661"/>
+      <location filename="../../photini/technical.py" line="658"/>
       <source>Link 'taken' and 'digitised'</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="663"/>
+      <location filename="../../photini/technical.py" line="660"/>
       <source>Link 'digitised' and 'modified'</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="665"/>
+      <location filename="../../photini/technical.py" line="662"/>
       <source>Taken</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="668"/>
+      <location filename="../../photini/technical.py" line="665"/>
       <source>Digitised</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="671"/>
+      <location filename="../../photini/technical.py" line="668"/>
       <source>Modified</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="676"/>
+      <location filename="../../photini/technical.py" line="673"/>
       <source>Adjust times</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="680"/>
+      <location filename="../../photini/technical.py" line="677"/>
       <source>Other</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="704"/>
+      <location filename="../../photini/technical.py" line="701"/>
       <source>Orientation</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="718"/>
+      <location filename="../../photini/technical.py" line="715"/>
       <source>Lens model</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="928"/>
+      <location filename="../../photini/technical.py" line="925"/>
       <source>Update aperture &amp; focal length</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="930"/>
+      <location filename="../../photini/technical.py" line="927"/>
       <source>Adjust image aperture and focal length to agree with lens specification?</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="597"/>
+      <location filename="../../photini/technical.py" line="594"/>
       <source>Minimum focal length</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="599"/>
+      <location filename="../../photini/technical.py" line="596"/>
       <source>Aperture at min. focal length</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="600"/>
+      <location filename="../../photini/technical.py" line="597"/>
       <source>Maximum focal length</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="602"/>
+      <location filename="../../photini/technical.py" line="599"/>
       <source>Aperture at max. focal length</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="732"/>
+      <location filename="../../photini/technical.py" line="729"/>
       <source>35mm equiv</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="739"/>
+      <location filename="../../photini/technical.py" line="736"/>
       <source>Aperture</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="563"/>
+      <location filename="../../photini/technical.py" line="560"/>
       <source>Photini: define camera</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="711"/>
+      <location filename="../../photini/technical.py" line="708"/>
       <source>Camera</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="818"/>
+      <location filename="../../photini/technical.py" line="815"/>
       <source>Photini: maker name change</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="824"/>
+      <location filename="../../photini/technical.py" line="821"/>
       <source>Do you want to delete the Exif makernote?</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="821"/>
+      <location filename="../../photini/technical.py" line="818"/>
       <source>Changing maker name will invalidate Exif makernote information.</source>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="687"/>
+      <location filename="../../photini/technical.py" line="684"/>
       <source>normal</source>
       <comment>orientation dropdown, no transformation</comment>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="695"/>
+      <location filename="../../photini/technical.py" line="692"/>
       <source>reflect left to right</source>
       <comment>orientation dropdown, horizontal reflection</comment>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="697"/>
+      <location filename="../../photini/technical.py" line="694"/>
       <source>reflect top to bottom</source>
       <comment>orientation dropdown, vertical reflection</comment>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="699"/>
+      <location filename="../../photini/technical.py" line="696"/>
       <source>reflect top right to bottom left</source>
       <comment>orientation dropdown, diagonal reflection</comment>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="701"/>
+      <location filename="../../photini/technical.py" line="698"/>
       <source>reflect top left to bottom right</source>
       <comment>orientation dropdown, diagonal reflection</comment>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="689"/>
+      <location filename="../../photini/technical.py" line="686"/>
       <source>rotate -90°</source>
       <comment>orientation dropdown</comment>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="691"/>
+      <location filename="../../photini/technical.py" line="688"/>
       <source>rotate +90°</source>
       <comment>orientation dropdown</comment>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="693"/>
+      <location filename="../../photini/technical.py" line="690"/>
       <source>rotate 180°</source>
       <comment>orientation dropdown</comment>
       <translation/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="387"/>
+      <location filename="../../photini/technical.py" line="384"/>
       <source>Precision</source>
       <translation/>
     </message>
   </context>
   <context>
     <name>UploaderTabsAll</name>
     <message>
```

### Comparing `Photini-2023.4.0/src/lang/es/LC_MESSAGES/index.po` & `Photini-2023.4.0.1/src/lang/es/LC_MESSAGES/index.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/es/LC_MESSAGES/manual.po` & `Photini-2023.4.0.1/src/lang/es/LC_MESSAGES/manual.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/es/LC_MESSAGES/misc.po` & `Photini-2023.4.0.1/src/lang/es/LC_MESSAGES/misc.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/es/LC_MESSAGES/other.po` & `Photini-2023.4.0.1/src/lang/es/LC_MESSAGES/other.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/es/photini.ts` & `Photini-2023.4.0.1/src/lang/es/photini.ts`

 * *Files 0% similar despite different names*

#### Comparing `Photini-2023.4.0/src/lang/es/photini.ts` & `Photini-2023.4.0.1/src/lang/es/photini.ts`

```diff
@@ -1008,20 +1008,20 @@
       <source>Set default language</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>LatLongDisplay</name>
     <message>
-      <location filename="../../photini/widgets.py" line="835"/>
+      <location filename="../../photini/widgets.py" line="834"/>
       <source>Lat, long</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/widgets.py" line="840"/>
+      <location filename="../../photini/widgets.py" line="839"/>
       <source>Latitude and longitude (in degrees) as two decimal numbers separated by a comma.</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>LoggerWindow</name>
     <message>
@@ -1698,362 +1698,362 @@
     </message>
     <message>
       <location filename="../../photini/regions.py" line="70"/>
       <source>New vertex</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="421"/>
+      <location filename="../../photini/regions.py" line="419"/>
       <source>Unreadable image format</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="597"/>
+      <location filename="../../photini/regions.py" line="595"/>
       <source>pixel</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="600"/>
+      <location filename="../../photini/regions.py" line="598"/>
       <source>A pixel of a digital image setting an absolute value.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="604"/>
+      <location filename="../../photini/regions.py" line="602"/>
       <source>relative</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="607"/>
+      <location filename="../../photini/regions.py" line="605"/>
       <source>Relative part of the size of an image along the x- or the y-axis.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="646"/>
+      <location filename="../../photini/regions.py" line="644"/>
       <source>Name</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="649"/>
+      <location filename="../../photini/regions.py" line="647"/>
       <source>Free-text name of the region. Should be unique among all Region Names of an image.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="658"/>
+      <location filename="../../photini/regions.py" line="656"/>
       <source>Identifier of the region. Must be unique among all Region Identifiers of an image. Does not have to be unique beyond the metadata of this image.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="660"/>
+      <location filename="../../photini/regions.py" line="658"/>
       <source>Identifier</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="666"/>
+      <location filename="../../photini/regions.py" line="664"/>
       <source>Unit used for measuring dimensions of the boundary of a region.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="669"/>
+      <location filename="../../photini/regions.py" line="667"/>
       <source>Boundary unit</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="676"/>
+      <location filename="../../photini/regions.py" line="674"/>
       <source>Role of this region among all regions of this image or of other images. The value SHOULD be taken from a Controlled Vocabulary.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="678"/>
+      <location filename="../../photini/regions.py" line="676"/>
       <source>Role</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="685"/>
+      <location filename="../../photini/regions.py" line="683"/>
       <source>The semantic type of what is shown inside the region. The value SHOULD be taken from a Controlled Vocabulary.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="688"/>
+      <location filename="../../photini/regions.py" line="686"/>
       <source>Content type</source>
       <translation>Tipo de contenido</translation>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="694"/>
+      <location filename="../../photini/regions.py" line="692"/>
       <source>Enter the names of people shown in this region. Separate multiple entries with &quot;;&quot; characters.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="697"/>
+      <location filename="../../photini/regions.py" line="695"/>
       <source>Person shown</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="701"/>
+      <location filename="../../photini/regions.py" line="699"/>
       <source>Description</source>
       <translation>Descripción</translation>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="704"/>
+      <location filename="../../photini/regions.py" line="702"/>
       <source>Enter a &quot;caption&quot; describing the who, what, and why of what is happening in this region.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="735"/>
+      <location filename="../../photini/regions.py" line="733"/>
       <source>The Image Region Structure includes optionally any metadata property which is related to the region.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="778"/>
+      <location filename="../../photini/regions.py" line="776"/>
       <source>New rectangle</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="780"/>
+      <location filename="../../photini/regions.py" line="778"/>
       <source>New circle</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="782"/>
+      <location filename="../../photini/regions.py" line="780"/>
       <source>New point</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="784"/>
+      <location filename="../../photini/regions.py" line="782"/>
       <source>New polygon</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="787"/>
+      <location filename="../../photini/regions.py" line="785"/>
       <source>Delete region</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="894"/>
+      <location filename="../../photini/regions.py" line="892"/>
       <source>Image &amp;Regions</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>TechnicalTab</name>
     <message>
-      <location filename="../../photini/technical.py" line="900"/>
+      <location filename="../../photini/technical.py" line="897"/>
       <source>min</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="901"/>
+      <location filename="../../photini/technical.py" line="898"/>
       <source>max</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="725"/>
-      <location filename="../../photini/technical.py" line="902"/>
+      <location filename="../../photini/technical.py" line="722"/>
+      <location filename="../../photini/technical.py" line="899"/>
       <source>Focal length</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="903"/>
+      <location filename="../../photini/technical.py" line="900"/>
       <source>Max aperture</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="577"/>
+      <location filename="../../photini/technical.py" line="574"/>
       <source>Photini: define lens</source>
       <translation>Photini: definir lente</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="538"/>
+      <location filename="../../photini/technical.py" line="535"/>
       <source>Model name</source>
       <translation>Nombre del modelo</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="537"/>
+      <location filename="../../photini/technical.py" line="534"/>
       <source>Maker's name</source>
       <translation>Nombre del fabricante</translation>
     </message>
     <message>
       <location filename="../../photini/technical.py" line="54"/>
       <source>Remove &quot;{camera_or_lens}&quot;</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="539"/>
+      <location filename="../../photini/technical.py" line="536"/>
       <source>Serial number</source>
       <translation>Número de serie</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="643"/>
+      <location filename="../../photini/technical.py" line="640"/>
       <source>&amp;Technical metadata</source>
       <translation>Metadatos &amp;técnicos</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="651"/>
+      <location filename="../../photini/technical.py" line="648"/>
       <source>Date and time</source>
       <translation>Fecha y hora</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="661"/>
+      <location filename="../../photini/technical.py" line="658"/>
       <source>Link 'taken' and 'digitised'</source>
       <translation>Vincular 'tomada' y 'digitalizada'</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="663"/>
+      <location filename="../../photini/technical.py" line="660"/>
       <source>Link 'digitised' and 'modified'</source>
       <translation>Vincular 'digitalizada' y 'modificada'</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="665"/>
+      <location filename="../../photini/technical.py" line="662"/>
       <source>Taken</source>
       <translation>Tomada</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="668"/>
+      <location filename="../../photini/technical.py" line="665"/>
       <source>Digitised</source>
       <translation>Digitalizada</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="671"/>
+      <location filename="../../photini/technical.py" line="668"/>
       <source>Modified</source>
       <translation>Modificada</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="676"/>
+      <location filename="../../photini/technical.py" line="673"/>
       <source>Adjust times</source>
       <translation>Ajustar tiempos</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="680"/>
+      <location filename="../../photini/technical.py" line="677"/>
       <source>Other</source>
       <translation>Otros</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="704"/>
+      <location filename="../../photini/technical.py" line="701"/>
       <source>Orientation</source>
       <translation>Orientación</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="718"/>
+      <location filename="../../photini/technical.py" line="715"/>
       <source>Lens model</source>
       <translation>Modelo del lente</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="928"/>
+      <location filename="../../photini/technical.py" line="925"/>
       <source>Update aperture &amp; focal length</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="930"/>
+      <location filename="../../photini/technical.py" line="927"/>
       <source>Adjust image aperture and focal length to agree with lens specification?</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="597"/>
+      <location filename="../../photini/technical.py" line="594"/>
       <source>Minimum focal length</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="599"/>
+      <location filename="../../photini/technical.py" line="596"/>
       <source>Aperture at min. focal length</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="600"/>
+      <location filename="../../photini/technical.py" line="597"/>
       <source>Maximum focal length</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="602"/>
+      <location filename="../../photini/technical.py" line="599"/>
       <source>Aperture at max. focal length</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="732"/>
+      <location filename="../../photini/technical.py" line="729"/>
       <source>35mm equiv</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="739"/>
+      <location filename="../../photini/technical.py" line="736"/>
       <source>Aperture</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="563"/>
+      <location filename="../../photini/technical.py" line="560"/>
       <source>Photini: define camera</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="711"/>
+      <location filename="../../photini/technical.py" line="708"/>
       <source>Camera</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="818"/>
+      <location filename="../../photini/technical.py" line="815"/>
       <source>Photini: maker name change</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="824"/>
+      <location filename="../../photini/technical.py" line="821"/>
       <source>Do you want to delete the Exif makernote?</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="821"/>
+      <location filename="../../photini/technical.py" line="818"/>
       <source>Changing maker name will invalidate Exif makernote information.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="687"/>
+      <location filename="../../photini/technical.py" line="684"/>
       <source>normal</source>
       <comment>orientation dropdown, no transformation</comment>
       <translation>normal</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="695"/>
+      <location filename="../../photini/technical.py" line="692"/>
       <source>reflect left to right</source>
       <comment>orientation dropdown, horizontal reflection</comment>
       <translation>reflejar izquierda-derecha</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="697"/>
+      <location filename="../../photini/technical.py" line="694"/>
       <source>reflect top to bottom</source>
       <comment>orientation dropdown, vertical reflection</comment>
       <translation>reflejar arriba-abajo</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="699"/>
+      <location filename="../../photini/technical.py" line="696"/>
       <source>reflect top right to bottom left</source>
       <comment>orientation dropdown, diagonal reflection</comment>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="701"/>
+      <location filename="../../photini/technical.py" line="698"/>
       <source>reflect top left to bottom right</source>
       <comment>orientation dropdown, diagonal reflection</comment>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="689"/>
+      <location filename="../../photini/technical.py" line="686"/>
       <source>rotate -90°</source>
       <comment>orientation dropdown</comment>
       <translation>rotar -90</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="691"/>
+      <location filename="../../photini/technical.py" line="688"/>
       <source>rotate +90°</source>
       <comment>orientation dropdown</comment>
       <translation>rotar +90</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="693"/>
+      <location filename="../../photini/technical.py" line="690"/>
       <source>rotate 180°</source>
       <comment>orientation dropdown</comment>
       <translation>rotar 180</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="387"/>
+      <location filename="../../photini/technical.py" line="384"/>
       <source>Precision</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>UploaderTabsAll</name>
     <message>
```

### Comparing `Photini-2023.4.0/src/lang/fr/LC_MESSAGES/index.po` & `Photini-2023.4.0.1/src/lang/fr/LC_MESSAGES/index.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/fr/LC_MESSAGES/manual.po` & `Photini-2023.4.0.1/src/lang/fr/LC_MESSAGES/manual.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/fr/LC_MESSAGES/misc.po` & `Photini-2023.4.0.1/src/lang/fr/LC_MESSAGES/misc.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/fr/LC_MESSAGES/other.po` & `Photini-2023.4.0.1/src/lang/fr/LC_MESSAGES/other.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/fr/photini.ts` & `Photini-2023.4.0.1/src/lang/fr/photini.ts`

 * *Files 0% similar despite different names*

#### Comparing `Photini-2023.4.0/src/lang/fr/photini.ts` & `Photini-2023.4.0.1/src/lang/fr/photini.ts`

```diff
@@ -1008,20 +1008,20 @@
       <source>Set default language</source>
       <translation>Définir la langue par défaut</translation>
     </message>
   </context>
   <context>
     <name>LatLongDisplay</name>
     <message>
-      <location filename="../../photini/widgets.py" line="835"/>
+      <location filename="../../photini/widgets.py" line="834"/>
       <source>Lat, long</source>
       <translation>Lat, lon</translation>
     </message>
     <message>
-      <location filename="../../photini/widgets.py" line="840"/>
+      <location filename="../../photini/widgets.py" line="839"/>
       <source>Latitude and longitude (in degrees) as two decimal numbers separated by a comma.</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>LoggerWindow</name>
     <message>
@@ -1698,362 +1698,362 @@
     </message>
     <message>
       <location filename="../../photini/regions.py" line="70"/>
       <source>New vertex</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="421"/>
+      <location filename="../../photini/regions.py" line="419"/>
       <source>Unreadable image format</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="597"/>
+      <location filename="../../photini/regions.py" line="595"/>
       <source>pixel</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="600"/>
+      <location filename="../../photini/regions.py" line="598"/>
       <source>A pixel of a digital image setting an absolute value.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="604"/>
+      <location filename="../../photini/regions.py" line="602"/>
       <source>relative</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="607"/>
+      <location filename="../../photini/regions.py" line="605"/>
       <source>Relative part of the size of an image along the x- or the y-axis.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="646"/>
+      <location filename="../../photini/regions.py" line="644"/>
       <source>Name</source>
       <translation>Nom</translation>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="649"/>
+      <location filename="../../photini/regions.py" line="647"/>
       <source>Free-text name of the region. Should be unique among all Region Names of an image.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="658"/>
+      <location filename="../../photini/regions.py" line="656"/>
       <source>Identifier of the region. Must be unique among all Region Identifiers of an image. Does not have to be unique beyond the metadata of this image.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="660"/>
+      <location filename="../../photini/regions.py" line="658"/>
       <source>Identifier</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="666"/>
+      <location filename="../../photini/regions.py" line="664"/>
       <source>Unit used for measuring dimensions of the boundary of a region.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="669"/>
+      <location filename="../../photini/regions.py" line="667"/>
       <source>Boundary unit</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="676"/>
+      <location filename="../../photini/regions.py" line="674"/>
       <source>Role of this region among all regions of this image or of other images. The value SHOULD be taken from a Controlled Vocabulary.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="678"/>
+      <location filename="../../photini/regions.py" line="676"/>
       <source>Role</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="685"/>
+      <location filename="../../photini/regions.py" line="683"/>
       <source>The semantic type of what is shown inside the region. The value SHOULD be taken from a Controlled Vocabulary.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="688"/>
+      <location filename="../../photini/regions.py" line="686"/>
       <source>Content type</source>
       <translation>Type de contenu</translation>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="694"/>
+      <location filename="../../photini/regions.py" line="692"/>
       <source>Enter the names of people shown in this region. Separate multiple entries with &quot;;&quot; characters.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="697"/>
+      <location filename="../../photini/regions.py" line="695"/>
       <source>Person shown</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="701"/>
+      <location filename="../../photini/regions.py" line="699"/>
       <source>Description</source>
       <translation>Description</translation>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="704"/>
+      <location filename="../../photini/regions.py" line="702"/>
       <source>Enter a &quot;caption&quot; describing the who, what, and why of what is happening in this region.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="735"/>
+      <location filename="../../photini/regions.py" line="733"/>
       <source>The Image Region Structure includes optionally any metadata property which is related to the region.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="778"/>
+      <location filename="../../photini/regions.py" line="776"/>
       <source>New rectangle</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="780"/>
+      <location filename="../../photini/regions.py" line="778"/>
       <source>New circle</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="782"/>
+      <location filename="../../photini/regions.py" line="780"/>
       <source>New point</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="784"/>
+      <location filename="../../photini/regions.py" line="782"/>
       <source>New polygon</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="787"/>
+      <location filename="../../photini/regions.py" line="785"/>
       <source>Delete region</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="894"/>
+      <location filename="../../photini/regions.py" line="892"/>
       <source>Image &amp;Regions</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>TechnicalTab</name>
     <message>
-      <location filename="../../photini/technical.py" line="900"/>
+      <location filename="../../photini/technical.py" line="897"/>
       <source>min</source>
       <translation>min</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="901"/>
+      <location filename="../../photini/technical.py" line="898"/>
       <source>max</source>
       <translation>max</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="725"/>
-      <location filename="../../photini/technical.py" line="902"/>
+      <location filename="../../photini/technical.py" line="722"/>
+      <location filename="../../photini/technical.py" line="899"/>
       <source>Focal length</source>
       <translation>Longueur focale</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="903"/>
+      <location filename="../../photini/technical.py" line="900"/>
       <source>Max aperture</source>
       <translation>Ouverture maximale</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="577"/>
+      <location filename="../../photini/technical.py" line="574"/>
       <source>Photini: define lens</source>
       <translation>Photini : Définir la lentille</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="538"/>
+      <location filename="../../photini/technical.py" line="535"/>
       <source>Model name</source>
       <translation>Nom du modèle</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="537"/>
+      <location filename="../../photini/technical.py" line="534"/>
       <source>Maker's name</source>
       <translation>Nom du fabricant</translation>
     </message>
     <message>
       <location filename="../../photini/technical.py" line="54"/>
       <source>Remove &quot;{camera_or_lens}&quot;</source>
       <translation>Supprimer « {camera_or_lens} »</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="539"/>
+      <location filename="../../photini/technical.py" line="536"/>
       <source>Serial number</source>
       <translation>Numéro de série</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="643"/>
+      <location filename="../../photini/technical.py" line="640"/>
       <source>&amp;Technical metadata</source>
       <translation>Métadonnées &amp;techniques</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="651"/>
+      <location filename="../../photini/technical.py" line="648"/>
       <source>Date and time</source>
       <translation>Date et heure</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="661"/>
+      <location filename="../../photini/technical.py" line="658"/>
       <source>Link 'taken' and 'digitised'</source>
       <translation>Lien « prise » et « numérisée »</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="663"/>
+      <location filename="../../photini/technical.py" line="660"/>
       <source>Link 'digitised' and 'modified'</source>
       <translation>Lien « numérisée » et « modifiée »</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="665"/>
+      <location filename="../../photini/technical.py" line="662"/>
       <source>Taken</source>
       <translation>Prise</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="668"/>
+      <location filename="../../photini/technical.py" line="665"/>
       <source>Digitised</source>
       <translation>Numérisée</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="671"/>
+      <location filename="../../photini/technical.py" line="668"/>
       <source>Modified</source>
       <translation>Modifiée</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="676"/>
+      <location filename="../../photini/technical.py" line="673"/>
       <source>Adjust times</source>
       <translation>Ajuster les horaires</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="680"/>
+      <location filename="../../photini/technical.py" line="677"/>
       <source>Other</source>
       <translation>Autre</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="704"/>
+      <location filename="../../photini/technical.py" line="701"/>
       <source>Orientation</source>
       <translation>Orientation</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="718"/>
+      <location filename="../../photini/technical.py" line="715"/>
       <source>Lens model</source>
       <translation>Modèle de lentille</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="928"/>
+      <location filename="../../photini/technical.py" line="925"/>
       <source>Update aperture &amp; focal length</source>
       <translation>Mettre à jour l'ouverture et la longueur focale</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="930"/>
+      <location filename="../../photini/technical.py" line="927"/>
       <source>Adjust image aperture and focal length to agree with lens specification?</source>
       <translation>Ajuster l'ouverture et la longueur focale pour correspondre aux spécifications de la lentille ?</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="597"/>
+      <location filename="../../photini/technical.py" line="594"/>
       <source>Minimum focal length</source>
       <translation>Longueur focale minimale</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="599"/>
+      <location filename="../../photini/technical.py" line="596"/>
       <source>Aperture at min. focal length</source>
       <translation>Ouverture à la longueur focale min.</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="600"/>
+      <location filename="../../photini/technical.py" line="597"/>
       <source>Maximum focal length</source>
       <translation>Longueur focale maximale</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="602"/>
+      <location filename="../../photini/technical.py" line="599"/>
       <source>Aperture at max. focal length</source>
       <translation>Ouverture à la longueur focale max.</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="732"/>
+      <location filename="../../photini/technical.py" line="729"/>
       <source>35mm equiv</source>
       <translation>35mm équiv</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="739"/>
+      <location filename="../../photini/technical.py" line="736"/>
       <source>Aperture</source>
       <translation>Ouverture</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="563"/>
+      <location filename="../../photini/technical.py" line="560"/>
       <source>Photini: define camera</source>
       <translation>Photini : Définir l'appareil photo</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="711"/>
+      <location filename="../../photini/technical.py" line="708"/>
       <source>Camera</source>
       <translation>Appareil photo</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="818"/>
+      <location filename="../../photini/technical.py" line="815"/>
       <source>Photini: maker name change</source>
       <translation>Photini : changement de nom du fabricant</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="824"/>
+      <location filename="../../photini/technical.py" line="821"/>
       <source>Do you want to delete the Exif makernote?</source>
       <translation>Voulez-vous supprimer la note Exif ?</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="821"/>
+      <location filename="../../photini/technical.py" line="818"/>
       <source>Changing maker name will invalidate Exif makernote information.</source>
       <translation>La modification du nom du fabricant invalidera les informations Exif sur les notes de fabrication.</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="687"/>
+      <location filename="../../photini/technical.py" line="684"/>
       <source>normal</source>
       <comment>orientation dropdown, no transformation</comment>
       <translation>Normal</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="695"/>
+      <location filename="../../photini/technical.py" line="692"/>
       <source>reflect left to right</source>
       <comment>orientation dropdown, horizontal reflection</comment>
       <translation>refléter gauche-droite</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="697"/>
+      <location filename="../../photini/technical.py" line="694"/>
       <source>reflect top to bottom</source>
       <comment>orientation dropdown, vertical reflection</comment>
       <translation>refléter de haut en bas</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="699"/>
+      <location filename="../../photini/technical.py" line="696"/>
       <source>reflect top right to bottom left</source>
       <comment>orientation dropdown, diagonal reflection</comment>
       <translation>refléter haut droite-bas gauche</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="701"/>
+      <location filename="../../photini/technical.py" line="698"/>
       <source>reflect top left to bottom right</source>
       <comment>orientation dropdown, diagonal reflection</comment>
       <translation>refléter haut gauche-bas droite</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="689"/>
+      <location filename="../../photini/technical.py" line="686"/>
       <source>rotate -90°</source>
       <comment>orientation dropdown</comment>
       <translation>Rotation -90</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="691"/>
+      <location filename="../../photini/technical.py" line="688"/>
       <source>rotate +90°</source>
       <comment>orientation dropdown</comment>
       <translation>Rotation +90</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="693"/>
+      <location filename="../../photini/technical.py" line="690"/>
       <source>rotate 180°</source>
       <comment>orientation dropdown</comment>
       <translation>Rotation 180</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="387"/>
+      <location filename="../../photini/technical.py" line="384"/>
       <source>Precision</source>
       <translation>Précision</translation>
     </message>
   </context>
   <context>
     <name>UploaderTabsAll</name>
     <message>
```

### Comparing `Photini-2023.4.0/src/lang/it/LC_MESSAGES/index.po` & `Photini-2023.4.0.1/src/lang/it/LC_MESSAGES/index.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/it/LC_MESSAGES/manual.po` & `Photini-2023.4.0.1/src/lang/it/LC_MESSAGES/manual.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/it/LC_MESSAGES/misc.po` & `Photini-2023.4.0.1/src/lang/it/LC_MESSAGES/misc.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/it/LC_MESSAGES/other.po` & `Photini-2023.4.0.1/src/lang/it/LC_MESSAGES/other.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/it/photini.ts` & `Photini-2023.4.0.1/src/lang/it/photini.ts`

 * *Files 0% similar despite different names*

#### Comparing `Photini-2023.4.0/src/lang/it/photini.ts` & `Photini-2023.4.0.1/src/lang/it/photini.ts`

```diff
@@ -1008,20 +1008,20 @@
       <source>Set default language</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>LatLongDisplay</name>
     <message>
-      <location filename="../../photini/widgets.py" line="835"/>
+      <location filename="../../photini/widgets.py" line="834"/>
       <source>Lat, long</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/widgets.py" line="840"/>
+      <location filename="../../photini/widgets.py" line="839"/>
       <source>Latitude and longitude (in degrees) as two decimal numbers separated by a comma.</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>LoggerWindow</name>
     <message>
@@ -1698,362 +1698,362 @@
     </message>
     <message>
       <location filename="../../photini/regions.py" line="70"/>
       <source>New vertex</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="421"/>
+      <location filename="../../photini/regions.py" line="419"/>
       <source>Unreadable image format</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="597"/>
+      <location filename="../../photini/regions.py" line="595"/>
       <source>pixel</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="600"/>
+      <location filename="../../photini/regions.py" line="598"/>
       <source>A pixel of a digital image setting an absolute value.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="604"/>
+      <location filename="../../photini/regions.py" line="602"/>
       <source>relative</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="607"/>
+      <location filename="../../photini/regions.py" line="605"/>
       <source>Relative part of the size of an image along the x- or the y-axis.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="646"/>
+      <location filename="../../photini/regions.py" line="644"/>
       <source>Name</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="649"/>
+      <location filename="../../photini/regions.py" line="647"/>
       <source>Free-text name of the region. Should be unique among all Region Names of an image.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="658"/>
+      <location filename="../../photini/regions.py" line="656"/>
       <source>Identifier of the region. Must be unique among all Region Identifiers of an image. Does not have to be unique beyond the metadata of this image.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="660"/>
+      <location filename="../../photini/regions.py" line="658"/>
       <source>Identifier</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="666"/>
+      <location filename="../../photini/regions.py" line="664"/>
       <source>Unit used for measuring dimensions of the boundary of a region.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="669"/>
+      <location filename="../../photini/regions.py" line="667"/>
       <source>Boundary unit</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="676"/>
+      <location filename="../../photini/regions.py" line="674"/>
       <source>Role of this region among all regions of this image or of other images. The value SHOULD be taken from a Controlled Vocabulary.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="678"/>
+      <location filename="../../photini/regions.py" line="676"/>
       <source>Role</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="685"/>
+      <location filename="../../photini/regions.py" line="683"/>
       <source>The semantic type of what is shown inside the region. The value SHOULD be taken from a Controlled Vocabulary.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="688"/>
+      <location filename="../../photini/regions.py" line="686"/>
       <source>Content type</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="694"/>
+      <location filename="../../photini/regions.py" line="692"/>
       <source>Enter the names of people shown in this region. Separate multiple entries with &quot;;&quot; characters.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="697"/>
+      <location filename="../../photini/regions.py" line="695"/>
       <source>Person shown</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="701"/>
+      <location filename="../../photini/regions.py" line="699"/>
       <source>Description</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="704"/>
+      <location filename="../../photini/regions.py" line="702"/>
       <source>Enter a &quot;caption&quot; describing the who, what, and why of what is happening in this region.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="735"/>
+      <location filename="../../photini/regions.py" line="733"/>
       <source>The Image Region Structure includes optionally any metadata property which is related to the region.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="778"/>
+      <location filename="../../photini/regions.py" line="776"/>
       <source>New rectangle</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="780"/>
+      <location filename="../../photini/regions.py" line="778"/>
       <source>New circle</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="782"/>
+      <location filename="../../photini/regions.py" line="780"/>
       <source>New point</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="784"/>
+      <location filename="../../photini/regions.py" line="782"/>
       <source>New polygon</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="787"/>
+      <location filename="../../photini/regions.py" line="785"/>
       <source>Delete region</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="894"/>
+      <location filename="../../photini/regions.py" line="892"/>
       <source>Image &amp;Regions</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>TechnicalTab</name>
     <message>
-      <location filename="../../photini/technical.py" line="900"/>
+      <location filename="../../photini/technical.py" line="897"/>
       <source>min</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="901"/>
+      <location filename="../../photini/technical.py" line="898"/>
       <source>max</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="725"/>
-      <location filename="../../photini/technical.py" line="902"/>
+      <location filename="../../photini/technical.py" line="722"/>
+      <location filename="../../photini/technical.py" line="899"/>
       <source>Focal length</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="903"/>
+      <location filename="../../photini/technical.py" line="900"/>
       <source>Max aperture</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="577"/>
+      <location filename="../../photini/technical.py" line="574"/>
       <source>Photini: define lens</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="538"/>
+      <location filename="../../photini/technical.py" line="535"/>
       <source>Model name</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="537"/>
+      <location filename="../../photini/technical.py" line="534"/>
       <source>Maker's name</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../../photini/technical.py" line="54"/>
       <source>Remove &quot;{camera_or_lens}&quot;</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="539"/>
+      <location filename="../../photini/technical.py" line="536"/>
       <source>Serial number</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="643"/>
+      <location filename="../../photini/technical.py" line="640"/>
       <source>&amp;Technical metadata</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="651"/>
+      <location filename="../../photini/technical.py" line="648"/>
       <source>Date and time</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="661"/>
+      <location filename="../../photini/technical.py" line="658"/>
       <source>Link 'taken' and 'digitised'</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="663"/>
+      <location filename="../../photini/technical.py" line="660"/>
       <source>Link 'digitised' and 'modified'</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="665"/>
+      <location filename="../../photini/technical.py" line="662"/>
       <source>Taken</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="668"/>
+      <location filename="../../photini/technical.py" line="665"/>
       <source>Digitised</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="671"/>
+      <location filename="../../photini/technical.py" line="668"/>
       <source>Modified</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="676"/>
+      <location filename="../../photini/technical.py" line="673"/>
       <source>Adjust times</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="680"/>
+      <location filename="../../photini/technical.py" line="677"/>
       <source>Other</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="704"/>
+      <location filename="../../photini/technical.py" line="701"/>
       <source>Orientation</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="718"/>
+      <location filename="../../photini/technical.py" line="715"/>
       <source>Lens model</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="928"/>
+      <location filename="../../photini/technical.py" line="925"/>
       <source>Update aperture &amp; focal length</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="930"/>
+      <location filename="../../photini/technical.py" line="927"/>
       <source>Adjust image aperture and focal length to agree with lens specification?</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="597"/>
+      <location filename="../../photini/technical.py" line="594"/>
       <source>Minimum focal length</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="599"/>
+      <location filename="../../photini/technical.py" line="596"/>
       <source>Aperture at min. focal length</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="600"/>
+      <location filename="../../photini/technical.py" line="597"/>
       <source>Maximum focal length</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="602"/>
+      <location filename="../../photini/technical.py" line="599"/>
       <source>Aperture at max. focal length</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="732"/>
+      <location filename="../../photini/technical.py" line="729"/>
       <source>35mm equiv</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="739"/>
+      <location filename="../../photini/technical.py" line="736"/>
       <source>Aperture</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="563"/>
+      <location filename="../../photini/technical.py" line="560"/>
       <source>Photini: define camera</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="711"/>
+      <location filename="../../photini/technical.py" line="708"/>
       <source>Camera</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="818"/>
+      <location filename="../../photini/technical.py" line="815"/>
       <source>Photini: maker name change</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="824"/>
+      <location filename="../../photini/technical.py" line="821"/>
       <source>Do you want to delete the Exif makernote?</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="821"/>
+      <location filename="../../photini/technical.py" line="818"/>
       <source>Changing maker name will invalidate Exif makernote information.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="687"/>
+      <location filename="../../photini/technical.py" line="684"/>
       <source>normal</source>
       <comment>orientation dropdown, no transformation</comment>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="695"/>
+      <location filename="../../photini/technical.py" line="692"/>
       <source>reflect left to right</source>
       <comment>orientation dropdown, horizontal reflection</comment>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="697"/>
+      <location filename="../../photini/technical.py" line="694"/>
       <source>reflect top to bottom</source>
       <comment>orientation dropdown, vertical reflection</comment>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="699"/>
+      <location filename="../../photini/technical.py" line="696"/>
       <source>reflect top right to bottom left</source>
       <comment>orientation dropdown, diagonal reflection</comment>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="701"/>
+      <location filename="../../photini/technical.py" line="698"/>
       <source>reflect top left to bottom right</source>
       <comment>orientation dropdown, diagonal reflection</comment>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="689"/>
+      <location filename="../../photini/technical.py" line="686"/>
       <source>rotate -90°</source>
       <comment>orientation dropdown</comment>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="691"/>
+      <location filename="../../photini/technical.py" line="688"/>
       <source>rotate +90°</source>
       <comment>orientation dropdown</comment>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="693"/>
+      <location filename="../../photini/technical.py" line="690"/>
       <source>rotate 180°</source>
       <comment>orientation dropdown</comment>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="387"/>
+      <location filename="../../photini/technical.py" line="384"/>
       <source>Precision</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>UploaderTabsAll</name>
     <message>
```

### Comparing `Photini-2023.4.0/src/lang/ko/LC_MESSAGES/index.po` & `Photini-2023.4.0.1/src/lang/ko/LC_MESSAGES/index.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/ko/LC_MESSAGES/manual.po` & `Photini-2023.4.0.1/src/lang/ko/LC_MESSAGES/manual.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/ko/LC_MESSAGES/misc.po` & `Photini-2023.4.0.1/src/lang/ko/LC_MESSAGES/misc.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/ko/LC_MESSAGES/other.po` & `Photini-2023.4.0.1/src/lang/ko/LC_MESSAGES/other.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/ko/photini.ts` & `Photini-2023.4.0.1/src/lang/ko/photini.ts`

 * *Files 0% similar despite different names*

#### Comparing `Photini-2023.4.0/src/lang/ko/photini.ts` & `Photini-2023.4.0.1/src/lang/ko/photini.ts`

```diff
@@ -1004,20 +1004,20 @@
       <source>Set default language</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>LatLongDisplay</name>
     <message>
-      <location filename="../../photini/widgets.py" line="835"/>
+      <location filename="../../photini/widgets.py" line="834"/>
       <source>Lat, long</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/widgets.py" line="840"/>
+      <location filename="../../photini/widgets.py" line="839"/>
       <source>Latitude and longitude (in degrees) as two decimal numbers separated by a comma.</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>LoggerWindow</name>
     <message>
@@ -1694,362 +1694,362 @@
     </message>
     <message>
       <location filename="../../photini/regions.py" line="70"/>
       <source>New vertex</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="421"/>
+      <location filename="../../photini/regions.py" line="419"/>
       <source>Unreadable image format</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="597"/>
+      <location filename="../../photini/regions.py" line="595"/>
       <source>pixel</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="600"/>
+      <location filename="../../photini/regions.py" line="598"/>
       <source>A pixel of a digital image setting an absolute value.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="604"/>
+      <location filename="../../photini/regions.py" line="602"/>
       <source>relative</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="607"/>
+      <location filename="../../photini/regions.py" line="605"/>
       <source>Relative part of the size of an image along the x- or the y-axis.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="646"/>
+      <location filename="../../photini/regions.py" line="644"/>
       <source>Name</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="649"/>
+      <location filename="../../photini/regions.py" line="647"/>
       <source>Free-text name of the region. Should be unique among all Region Names of an image.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="658"/>
+      <location filename="../../photini/regions.py" line="656"/>
       <source>Identifier of the region. Must be unique among all Region Identifiers of an image. Does not have to be unique beyond the metadata of this image.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="660"/>
+      <location filename="../../photini/regions.py" line="658"/>
       <source>Identifier</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="666"/>
+      <location filename="../../photini/regions.py" line="664"/>
       <source>Unit used for measuring dimensions of the boundary of a region.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="669"/>
+      <location filename="../../photini/regions.py" line="667"/>
       <source>Boundary unit</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="676"/>
+      <location filename="../../photini/regions.py" line="674"/>
       <source>Role of this region among all regions of this image or of other images. The value SHOULD be taken from a Controlled Vocabulary.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="678"/>
+      <location filename="../../photini/regions.py" line="676"/>
       <source>Role</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="685"/>
+      <location filename="../../photini/regions.py" line="683"/>
       <source>The semantic type of what is shown inside the region. The value SHOULD be taken from a Controlled Vocabulary.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="688"/>
+      <location filename="../../photini/regions.py" line="686"/>
       <source>Content type</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="694"/>
+      <location filename="../../photini/regions.py" line="692"/>
       <source>Enter the names of people shown in this region. Separate multiple entries with &quot;;&quot; characters.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="697"/>
+      <location filename="../../photini/regions.py" line="695"/>
       <source>Person shown</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="701"/>
+      <location filename="../../photini/regions.py" line="699"/>
       <source>Description</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="704"/>
+      <location filename="../../photini/regions.py" line="702"/>
       <source>Enter a &quot;caption&quot; describing the who, what, and why of what is happening in this region.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="735"/>
+      <location filename="../../photini/regions.py" line="733"/>
       <source>The Image Region Structure includes optionally any metadata property which is related to the region.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="778"/>
+      <location filename="../../photini/regions.py" line="776"/>
       <source>New rectangle</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="780"/>
+      <location filename="../../photini/regions.py" line="778"/>
       <source>New circle</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="782"/>
+      <location filename="../../photini/regions.py" line="780"/>
       <source>New point</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="784"/>
+      <location filename="../../photini/regions.py" line="782"/>
       <source>New polygon</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="787"/>
+      <location filename="../../photini/regions.py" line="785"/>
       <source>Delete region</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="894"/>
+      <location filename="../../photini/regions.py" line="892"/>
       <source>Image &amp;Regions</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>TechnicalTab</name>
     <message>
-      <location filename="../../photini/technical.py" line="900"/>
+      <location filename="../../photini/technical.py" line="897"/>
       <source>min</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="901"/>
+      <location filename="../../photini/technical.py" line="898"/>
       <source>max</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="725"/>
-      <location filename="../../photini/technical.py" line="902"/>
+      <location filename="../../photini/technical.py" line="722"/>
+      <location filename="../../photini/technical.py" line="899"/>
       <source>Focal length</source>
       <translation>초점 거리</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="903"/>
+      <location filename="../../photini/technical.py" line="900"/>
       <source>Max aperture</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="577"/>
+      <location filename="../../photini/technical.py" line="574"/>
       <source>Photini: define lens</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="538"/>
+      <location filename="../../photini/technical.py" line="535"/>
       <source>Model name</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="537"/>
+      <location filename="../../photini/technical.py" line="534"/>
       <source>Maker's name</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../../photini/technical.py" line="54"/>
       <source>Remove &quot;{camera_or_lens}&quot;</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="539"/>
+      <location filename="../../photini/technical.py" line="536"/>
       <source>Serial number</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="643"/>
+      <location filename="../../photini/technical.py" line="640"/>
       <source>&amp;Technical metadata</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="651"/>
+      <location filename="../../photini/technical.py" line="648"/>
       <source>Date and time</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="661"/>
+      <location filename="../../photini/technical.py" line="658"/>
       <source>Link 'taken' and 'digitised'</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="663"/>
+      <location filename="../../photini/technical.py" line="660"/>
       <source>Link 'digitised' and 'modified'</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="665"/>
+      <location filename="../../photini/technical.py" line="662"/>
       <source>Taken</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="668"/>
+      <location filename="../../photini/technical.py" line="665"/>
       <source>Digitised</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="671"/>
+      <location filename="../../photini/technical.py" line="668"/>
       <source>Modified</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="676"/>
+      <location filename="../../photini/technical.py" line="673"/>
       <source>Adjust times</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="680"/>
+      <location filename="../../photini/technical.py" line="677"/>
       <source>Other</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="704"/>
+      <location filename="../../photini/technical.py" line="701"/>
       <source>Orientation</source>
       <translation>Orientation</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="718"/>
+      <location filename="../../photini/technical.py" line="715"/>
       <source>Lens model</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="928"/>
+      <location filename="../../photini/technical.py" line="925"/>
       <source>Update aperture &amp; focal length</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="930"/>
+      <location filename="../../photini/technical.py" line="927"/>
       <source>Adjust image aperture and focal length to agree with lens specification?</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="597"/>
+      <location filename="../../photini/technical.py" line="594"/>
       <source>Minimum focal length</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="599"/>
+      <location filename="../../photini/technical.py" line="596"/>
       <source>Aperture at min. focal length</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="600"/>
+      <location filename="../../photini/technical.py" line="597"/>
       <source>Maximum focal length</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="602"/>
+      <location filename="../../photini/technical.py" line="599"/>
       <source>Aperture at max. focal length</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="732"/>
+      <location filename="../../photini/technical.py" line="729"/>
       <source>35mm equiv</source>
       <translation>35mm equiv</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="739"/>
+      <location filename="../../photini/technical.py" line="736"/>
       <source>Aperture</source>
       <translation>조리개</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="563"/>
+      <location filename="../../photini/technical.py" line="560"/>
       <source>Photini: define camera</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="711"/>
+      <location filename="../../photini/technical.py" line="708"/>
       <source>Camera</source>
       <translation>카메라</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="818"/>
+      <location filename="../../photini/technical.py" line="815"/>
       <source>Photini: maker name change</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="824"/>
+      <location filename="../../photini/technical.py" line="821"/>
       <source>Do you want to delete the Exif makernote?</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="821"/>
+      <location filename="../../photini/technical.py" line="818"/>
       <source>Changing maker name will invalidate Exif makernote information.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="687"/>
+      <location filename="../../photini/technical.py" line="684"/>
       <source>normal</source>
       <comment>orientation dropdown, no transformation</comment>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="695"/>
+      <location filename="../../photini/technical.py" line="692"/>
       <source>reflect left to right</source>
       <comment>orientation dropdown, horizontal reflection</comment>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="697"/>
+      <location filename="../../photini/technical.py" line="694"/>
       <source>reflect top to bottom</source>
       <comment>orientation dropdown, vertical reflection</comment>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="699"/>
+      <location filename="../../photini/technical.py" line="696"/>
       <source>reflect top right to bottom left</source>
       <comment>orientation dropdown, diagonal reflection</comment>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="701"/>
+      <location filename="../../photini/technical.py" line="698"/>
       <source>reflect top left to bottom right</source>
       <comment>orientation dropdown, diagonal reflection</comment>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="689"/>
+      <location filename="../../photini/technical.py" line="686"/>
       <source>rotate -90°</source>
       <comment>orientation dropdown</comment>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="691"/>
+      <location filename="../../photini/technical.py" line="688"/>
       <source>rotate +90°</source>
       <comment>orientation dropdown</comment>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="693"/>
+      <location filename="../../photini/technical.py" line="690"/>
       <source>rotate 180°</source>
       <comment>orientation dropdown</comment>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="387"/>
+      <location filename="../../photini/technical.py" line="384"/>
       <source>Precision</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>UploaderTabsAll</name>
     <message>
```

### Comparing `Photini-2023.4.0/src/lang/nb/LC_MESSAGES/index.po` & `Photini-2023.4.0.1/src/lang/nb/LC_MESSAGES/index.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/nb/LC_MESSAGES/manual.po` & `Photini-2023.4.0.1/src/lang/nb/LC_MESSAGES/manual.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/nb/LC_MESSAGES/misc.po` & `Photini-2023.4.0.1/src/lang/nb/LC_MESSAGES/misc.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/nb/LC_MESSAGES/other.po` & `Photini-2023.4.0.1/src/lang/nb/LC_MESSAGES/other.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/nb/photini.ts` & `Photini-2023.4.0.1/src/lang/nb/photini.ts`

 * *Files 1% similar despite different names*

#### Comparing `Photini-2023.4.0/src/lang/nb/photini.ts` & `Photini-2023.4.0.1/src/lang/nb/photini.ts`

```diff
@@ -1008,20 +1008,20 @@
       <source>Set default language</source>
       <translation>Sett forvalgt språk</translation>
     </message>
   </context>
   <context>
     <name>LatLongDisplay</name>
     <message>
-      <location filename="../../photini/widgets.py" line="835"/>
+      <location filename="../../photini/widgets.py" line="834"/>
       <source>Lat, long</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/widgets.py" line="840"/>
+      <location filename="../../photini/widgets.py" line="839"/>
       <source>Latitude and longitude (in degrees) as two decimal numbers separated by a comma.</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>LoggerWindow</name>
     <message>
@@ -1698,362 +1698,362 @@
     </message>
     <message>
       <location filename="../../photini/regions.py" line="70"/>
       <source>New vertex</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="421"/>
+      <location filename="../../photini/regions.py" line="419"/>
       <source>Unreadable image format</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="597"/>
+      <location filename="../../photini/regions.py" line="595"/>
       <source>pixel</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="600"/>
+      <location filename="../../photini/regions.py" line="598"/>
       <source>A pixel of a digital image setting an absolute value.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="604"/>
+      <location filename="../../photini/regions.py" line="602"/>
       <source>relative</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="607"/>
+      <location filename="../../photini/regions.py" line="605"/>
       <source>Relative part of the size of an image along the x- or the y-axis.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="646"/>
+      <location filename="../../photini/regions.py" line="644"/>
       <source>Name</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="649"/>
+      <location filename="../../photini/regions.py" line="647"/>
       <source>Free-text name of the region. Should be unique among all Region Names of an image.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="658"/>
+      <location filename="../../photini/regions.py" line="656"/>
       <source>Identifier of the region. Must be unique among all Region Identifiers of an image. Does not have to be unique beyond the metadata of this image.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="660"/>
+      <location filename="../../photini/regions.py" line="658"/>
       <source>Identifier</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="666"/>
+      <location filename="../../photini/regions.py" line="664"/>
       <source>Unit used for measuring dimensions of the boundary of a region.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="669"/>
+      <location filename="../../photini/regions.py" line="667"/>
       <source>Boundary unit</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="676"/>
+      <location filename="../../photini/regions.py" line="674"/>
       <source>Role of this region among all regions of this image or of other images. The value SHOULD be taken from a Controlled Vocabulary.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="678"/>
+      <location filename="../../photini/regions.py" line="676"/>
       <source>Role</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="685"/>
+      <location filename="../../photini/regions.py" line="683"/>
       <source>The semantic type of what is shown inside the region. The value SHOULD be taken from a Controlled Vocabulary.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="688"/>
+      <location filename="../../photini/regions.py" line="686"/>
       <source>Content type</source>
       <translation>Innholdstype</translation>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="694"/>
+      <location filename="../../photini/regions.py" line="692"/>
       <source>Enter the names of people shown in this region. Separate multiple entries with &quot;;&quot; characters.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="697"/>
+      <location filename="../../photini/regions.py" line="695"/>
       <source>Person shown</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="701"/>
+      <location filename="../../photini/regions.py" line="699"/>
       <source>Description</source>
       <translation>Beskrivelse</translation>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="704"/>
+      <location filename="../../photini/regions.py" line="702"/>
       <source>Enter a &quot;caption&quot; describing the who, what, and why of what is happening in this region.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="735"/>
+      <location filename="../../photini/regions.py" line="733"/>
       <source>The Image Region Structure includes optionally any metadata property which is related to the region.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="778"/>
+      <location filename="../../photini/regions.py" line="776"/>
       <source>New rectangle</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="780"/>
+      <location filename="../../photini/regions.py" line="778"/>
       <source>New circle</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="782"/>
+      <location filename="../../photini/regions.py" line="780"/>
       <source>New point</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="784"/>
+      <location filename="../../photini/regions.py" line="782"/>
       <source>New polygon</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="787"/>
+      <location filename="../../photini/regions.py" line="785"/>
       <source>Delete region</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="894"/>
+      <location filename="../../photini/regions.py" line="892"/>
       <source>Image &amp;Regions</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>TechnicalTab</name>
     <message>
-      <location filename="../../photini/technical.py" line="900"/>
+      <location filename="../../photini/technical.py" line="897"/>
       <source>min</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="901"/>
+      <location filename="../../photini/technical.py" line="898"/>
       <source>max</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="725"/>
-      <location filename="../../photini/technical.py" line="902"/>
+      <location filename="../../photini/technical.py" line="722"/>
+      <location filename="../../photini/technical.py" line="899"/>
       <source>Focal length</source>
       <translation>Brennvidde</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="903"/>
+      <location filename="../../photini/technical.py" line="900"/>
       <source>Max aperture</source>
       <translation>Maks. blenderåpning</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="577"/>
+      <location filename="../../photini/technical.py" line="574"/>
       <source>Photini: define lens</source>
       <translation>Photini: definer linse</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="538"/>
+      <location filename="../../photini/technical.py" line="535"/>
       <source>Model name</source>
       <translation>Modellnavn</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="537"/>
+      <location filename="../../photini/technical.py" line="534"/>
       <source>Maker's name</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../../photini/technical.py" line="54"/>
       <source>Remove &quot;{camera_or_lens}&quot;</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="539"/>
+      <location filename="../../photini/technical.py" line="536"/>
       <source>Serial number</source>
       <translation>Serienummer</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="643"/>
+      <location filename="../../photini/technical.py" line="640"/>
       <source>&amp;Technical metadata</source>
       <translation>&amp;Teknisk metadata</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="651"/>
+      <location filename="../../photini/technical.py" line="648"/>
       <source>Date and time</source>
       <translation>Dato og tid</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="661"/>
+      <location filename="../../photini/technical.py" line="658"/>
       <source>Link 'taken' and 'digitised'</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="663"/>
+      <location filename="../../photini/technical.py" line="660"/>
       <source>Link 'digitised' and 'modified'</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="665"/>
+      <location filename="../../photini/technical.py" line="662"/>
       <source>Taken</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="668"/>
+      <location filename="../../photini/technical.py" line="665"/>
       <source>Digitised</source>
       <translation>Digitalisert</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="671"/>
+      <location filename="../../photini/technical.py" line="668"/>
       <source>Modified</source>
       <translation>Endret</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="676"/>
+      <location filename="../../photini/technical.py" line="673"/>
       <source>Adjust times</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="680"/>
+      <location filename="../../photini/technical.py" line="677"/>
       <source>Other</source>
       <translation>Annet</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="704"/>
+      <location filename="../../photini/technical.py" line="701"/>
       <source>Orientation</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="718"/>
+      <location filename="../../photini/technical.py" line="715"/>
       <source>Lens model</source>
       <translation>Linsemodell</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="928"/>
+      <location filename="../../photini/technical.py" line="925"/>
       <source>Update aperture &amp; focal length</source>
       <translation>Oppdater brennvidde og blenderåpning</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="930"/>
+      <location filename="../../photini/technical.py" line="927"/>
       <source>Adjust image aperture and focal length to agree with lens specification?</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="597"/>
+      <location filename="../../photini/technical.py" line="594"/>
       <source>Minimum focal length</source>
       <translation>Min. brennvidde</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="599"/>
+      <location filename="../../photini/technical.py" line="596"/>
       <source>Aperture at min. focal length</source>
       <translation>Blenderåpning ved min. brennvidde</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="600"/>
+      <location filename="../../photini/technical.py" line="597"/>
       <source>Maximum focal length</source>
       <translation>Maks. brennvidde</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="602"/>
+      <location filename="../../photini/technical.py" line="599"/>
       <source>Aperture at max. focal length</source>
       <translation>Blenderåpning ved maks. brennvidde</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="732"/>
+      <location filename="../../photini/technical.py" line="729"/>
       <source>35mm equiv</source>
       <translation>35 mm-ekvivalent</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="739"/>
+      <location filename="../../photini/technical.py" line="736"/>
       <source>Aperture</source>
       <translation>Blenderåpning</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="563"/>
+      <location filename="../../photini/technical.py" line="560"/>
       <source>Photini: define camera</source>
       <translation>Photini: definer kamera</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="711"/>
+      <location filename="../../photini/technical.py" line="708"/>
       <source>Camera</source>
       <translation>Kamera</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="818"/>
+      <location filename="../../photini/technical.py" line="815"/>
       <source>Photini: maker name change</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="824"/>
+      <location filename="../../photini/technical.py" line="821"/>
       <source>Do you want to delete the Exif makernote?</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="821"/>
+      <location filename="../../photini/technical.py" line="818"/>
       <source>Changing maker name will invalidate Exif makernote information.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="687"/>
+      <location filename="../../photini/technical.py" line="684"/>
       <source>normal</source>
       <comment>orientation dropdown, no transformation</comment>
       <translation>normal</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="695"/>
+      <location filename="../../photini/technical.py" line="692"/>
       <source>reflect left to right</source>
       <comment>orientation dropdown, horizontal reflection</comment>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="697"/>
+      <location filename="../../photini/technical.py" line="694"/>
       <source>reflect top to bottom</source>
       <comment>orientation dropdown, vertical reflection</comment>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="699"/>
+      <location filename="../../photini/technical.py" line="696"/>
       <source>reflect top right to bottom left</source>
       <comment>orientation dropdown, diagonal reflection</comment>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="701"/>
+      <location filename="../../photini/technical.py" line="698"/>
       <source>reflect top left to bottom right</source>
       <comment>orientation dropdown, diagonal reflection</comment>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="689"/>
+      <location filename="../../photini/technical.py" line="686"/>
       <source>rotate -90°</source>
       <comment>orientation dropdown</comment>
       <translation>roter -90</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="691"/>
+      <location filename="../../photini/technical.py" line="688"/>
       <source>rotate +90°</source>
       <comment>orientation dropdown</comment>
       <translation>roter +90</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="693"/>
+      <location filename="../../photini/technical.py" line="690"/>
       <source>rotate 180°</source>
       <comment>orientation dropdown</comment>
       <translation>roter 180</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="387"/>
+      <location filename="../../photini/technical.py" line="384"/>
       <source>Precision</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>UploaderTabsAll</name>
     <message>
```

### Comparing `Photini-2023.4.0/src/lang/pl/LC_MESSAGES/index.po` & `Photini-2023.4.0.1/src/lang/pl/LC_MESSAGES/index.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/pl/LC_MESSAGES/manual.po` & `Photini-2023.4.0.1/src/lang/pl/LC_MESSAGES/manual.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/pl/LC_MESSAGES/misc.po` & `Photini-2023.4.0.1/src/lang/pl/LC_MESSAGES/misc.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/pl/LC_MESSAGES/other.po` & `Photini-2023.4.0.1/src/lang/pl/LC_MESSAGES/other.po`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/pl/photini.ts` & `Photini-2023.4.0.1/src/lang/pl/photini.ts`

 * *Files 0% similar despite different names*

#### Comparing `Photini-2023.4.0/src/lang/pl/photini.ts` & `Photini-2023.4.0.1/src/lang/pl/photini.ts`

```diff
@@ -1012,20 +1012,20 @@
       <source>Set default language</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>LatLongDisplay</name>
     <message>
-      <location filename="../../photini/widgets.py" line="835"/>
+      <location filename="../../photini/widgets.py" line="834"/>
       <source>Lat, long</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/widgets.py" line="840"/>
+      <location filename="../../photini/widgets.py" line="839"/>
       <source>Latitude and longitude (in degrees) as two decimal numbers separated by a comma.</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>LoggerWindow</name>
     <message>
@@ -1702,362 +1702,362 @@
     </message>
     <message>
       <location filename="../../photini/regions.py" line="70"/>
       <source>New vertex</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="421"/>
+      <location filename="../../photini/regions.py" line="419"/>
       <source>Unreadable image format</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="597"/>
+      <location filename="../../photini/regions.py" line="595"/>
       <source>pixel</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="600"/>
+      <location filename="../../photini/regions.py" line="598"/>
       <source>A pixel of a digital image setting an absolute value.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="604"/>
+      <location filename="../../photini/regions.py" line="602"/>
       <source>relative</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="607"/>
+      <location filename="../../photini/regions.py" line="605"/>
       <source>Relative part of the size of an image along the x- or the y-axis.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="646"/>
+      <location filename="../../photini/regions.py" line="644"/>
       <source>Name</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="649"/>
+      <location filename="../../photini/regions.py" line="647"/>
       <source>Free-text name of the region. Should be unique among all Region Names of an image.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="658"/>
+      <location filename="../../photini/regions.py" line="656"/>
       <source>Identifier of the region. Must be unique among all Region Identifiers of an image. Does not have to be unique beyond the metadata of this image.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="660"/>
+      <location filename="../../photini/regions.py" line="658"/>
       <source>Identifier</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="666"/>
+      <location filename="../../photini/regions.py" line="664"/>
       <source>Unit used for measuring dimensions of the boundary of a region.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="669"/>
+      <location filename="../../photini/regions.py" line="667"/>
       <source>Boundary unit</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="676"/>
+      <location filename="../../photini/regions.py" line="674"/>
       <source>Role of this region among all regions of this image or of other images. The value SHOULD be taken from a Controlled Vocabulary.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="678"/>
+      <location filename="../../photini/regions.py" line="676"/>
       <source>Role</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="685"/>
+      <location filename="../../photini/regions.py" line="683"/>
       <source>The semantic type of what is shown inside the region. The value SHOULD be taken from a Controlled Vocabulary.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="688"/>
+      <location filename="../../photini/regions.py" line="686"/>
       <source>Content type</source>
       <translation>Typ zawartości</translation>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="694"/>
+      <location filename="../../photini/regions.py" line="692"/>
       <source>Enter the names of people shown in this region. Separate multiple entries with &quot;;&quot; characters.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="697"/>
+      <location filename="../../photini/regions.py" line="695"/>
       <source>Person shown</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="701"/>
+      <location filename="../../photini/regions.py" line="699"/>
       <source>Description</source>
       <translation>Opis</translation>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="704"/>
+      <location filename="../../photini/regions.py" line="702"/>
       <source>Enter a &quot;caption&quot; describing the who, what, and why of what is happening in this region.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="735"/>
+      <location filename="../../photini/regions.py" line="733"/>
       <source>The Image Region Structure includes optionally any metadata property which is related to the region.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="778"/>
+      <location filename="../../photini/regions.py" line="776"/>
       <source>New rectangle</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="780"/>
+      <location filename="../../photini/regions.py" line="778"/>
       <source>New circle</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="782"/>
+      <location filename="../../photini/regions.py" line="780"/>
       <source>New point</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="784"/>
+      <location filename="../../photini/regions.py" line="782"/>
       <source>New polygon</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="787"/>
+      <location filename="../../photini/regions.py" line="785"/>
       <source>Delete region</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/regions.py" line="894"/>
+      <location filename="../../photini/regions.py" line="892"/>
       <source>Image &amp;Regions</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>TechnicalTab</name>
     <message>
-      <location filename="../../photini/technical.py" line="900"/>
+      <location filename="../../photini/technical.py" line="897"/>
       <source>min</source>
       <translation>Min</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="901"/>
+      <location filename="../../photini/technical.py" line="898"/>
       <source>max</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="725"/>
-      <location filename="../../photini/technical.py" line="902"/>
+      <location filename="../../photini/technical.py" line="722"/>
+      <location filename="../../photini/technical.py" line="899"/>
       <source>Focal length</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="903"/>
+      <location filename="../../photini/technical.py" line="900"/>
       <source>Max aperture</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="577"/>
+      <location filename="../../photini/technical.py" line="574"/>
       <source>Photini: define lens</source>
       <translation>Photini: definicja obiektu</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="538"/>
+      <location filename="../../photini/technical.py" line="535"/>
       <source>Model name</source>
       <translation>Nazwa modelu</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="537"/>
+      <location filename="../../photini/technical.py" line="534"/>
       <source>Maker's name</source>
       <translation>Nazwa Makera</translation>
     </message>
     <message>
       <location filename="../../photini/technical.py" line="54"/>
       <source>Remove &quot;{camera_or_lens}&quot;</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="539"/>
+      <location filename="../../photini/technical.py" line="536"/>
       <source>Serial number</source>
       <translation>Numer seryjny</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="643"/>
+      <location filename="../../photini/technical.py" line="640"/>
       <source>&amp;Technical metadata</source>
       <translation>Metadane &amp;techniczne</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="651"/>
+      <location filename="../../photini/technical.py" line="648"/>
       <source>Date and time</source>
       <translation>Data i czas</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="661"/>
+      <location filename="../../photini/technical.py" line="658"/>
       <source>Link 'taken' and 'digitised'</source>
       <translation>Link 'taken' i'digitised'</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="663"/>
+      <location filename="../../photini/technical.py" line="660"/>
       <source>Link 'digitised' and 'modified'</source>
       <translation>Link 'digitised' i 'modified'</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="665"/>
+      <location filename="../../photini/technical.py" line="662"/>
       <source>Taken</source>
       <translation>Zrobione</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="668"/>
+      <location filename="../../photini/technical.py" line="665"/>
       <source>Digitised</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="671"/>
+      <location filename="../../photini/technical.py" line="668"/>
       <source>Modified</source>
       <translation>Zmodyfikowany</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="676"/>
+      <location filename="../../photini/technical.py" line="673"/>
       <source>Adjust times</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="680"/>
+      <location filename="../../photini/technical.py" line="677"/>
       <source>Other</source>
       <translation>Inny</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="704"/>
+      <location filename="../../photini/technical.py" line="701"/>
       <source>Orientation</source>
       <translation>Orientacja</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="718"/>
+      <location filename="../../photini/technical.py" line="715"/>
       <source>Lens model</source>
       <translation>Model obiektywu</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="928"/>
+      <location filename="../../photini/technical.py" line="925"/>
       <source>Update aperture &amp; focal length</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="930"/>
+      <location filename="../../photini/technical.py" line="927"/>
       <source>Adjust image aperture and focal length to agree with lens specification?</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="597"/>
+      <location filename="../../photini/technical.py" line="594"/>
       <source>Minimum focal length</source>
       <translation>Minimalna ogniskowa</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="599"/>
+      <location filename="../../photini/technical.py" line="596"/>
       <source>Aperture at min. focal length</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="600"/>
+      <location filename="../../photini/technical.py" line="597"/>
       <source>Maximum focal length</source>
       <translation>Maksymalna ogniskowa</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="602"/>
+      <location filename="../../photini/technical.py" line="599"/>
       <source>Aperture at max. focal length</source>
       <translation>Przysłona przy max. ogniskowej</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="732"/>
+      <location filename="../../photini/technical.py" line="729"/>
       <source>35mm equiv</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="739"/>
+      <location filename="../../photini/technical.py" line="736"/>
       <source>Aperture</source>
       <translation>Przesłona</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="563"/>
+      <location filename="../../photini/technical.py" line="560"/>
       <source>Photini: define camera</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="711"/>
+      <location filename="../../photini/technical.py" line="708"/>
       <source>Camera</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="818"/>
+      <location filename="../../photini/technical.py" line="815"/>
       <source>Photini: maker name change</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="824"/>
+      <location filename="../../photini/technical.py" line="821"/>
       <source>Do you want to delete the Exif makernote?</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="821"/>
+      <location filename="../../photini/technical.py" line="818"/>
       <source>Changing maker name will invalidate Exif makernote information.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="687"/>
+      <location filename="../../photini/technical.py" line="684"/>
       <source>normal</source>
       <comment>orientation dropdown, no transformation</comment>
       <translation>Normalny</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="695"/>
+      <location filename="../../photini/technical.py" line="692"/>
       <source>reflect left to right</source>
       <comment>orientation dropdown, horizontal reflection</comment>
       <translation>Odbicie lewa-prawa</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="697"/>
+      <location filename="../../photini/technical.py" line="694"/>
       <source>reflect top to bottom</source>
       <comment>orientation dropdown, vertical reflection</comment>
       <translation>Odbicie góra-dół</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="699"/>
+      <location filename="../../photini/technical.py" line="696"/>
       <source>reflect top right to bottom left</source>
       <comment>orientation dropdown, diagonal reflection</comment>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="701"/>
+      <location filename="../../photini/technical.py" line="698"/>
       <source>reflect top left to bottom right</source>
       <comment>orientation dropdown, diagonal reflection</comment>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="689"/>
+      <location filename="../../photini/technical.py" line="686"/>
       <source>rotate -90°</source>
       <comment>orientation dropdown</comment>
       <translation>Obrót -90</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="691"/>
+      <location filename="../../photini/technical.py" line="688"/>
       <source>rotate +90°</source>
       <comment>orientation dropdown</comment>
       <translation>Obrót +90</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="693"/>
+      <location filename="../../photini/technical.py" line="690"/>
       <source>rotate 180°</source>
       <comment>orientation dropdown</comment>
       <translation>Obrót 180</translation>
     </message>
     <message>
-      <location filename="../../photini/technical.py" line="387"/>
+      <location filename="../../photini/technical.py" line="384"/>
       <source>Precision</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>UploaderTabsAll</name>
     <message>
```

### Comparing `Photini-2023.4.0/src/lang/templates/gettext/index.pot` & `Photini-2023.4.0.1/src/lang/templates/gettext/index.pot`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/templates/gettext/manual.pot` & `Photini-2023.4.0.1/src/lang/templates/gettext/manual.pot`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/templates/gettext/misc.pot` & `Photini-2023.4.0.1/src/lang/templates/gettext/misc.pot`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/templates/gettext/other.pot` & `Photini-2023.4.0.1/src/lang/templates/gettext/other.pot`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/lang/templates/qt/photini.ts` & `Photini-2023.4.0.1/src/lang/templates/qt/photini.ts`

 * *Files 0% similar despite different names*

#### Comparing `Photini-2023.4.0/src/lang/templates/qt/photini.ts` & `Photini-2023.4.0.1/src/lang/templates/qt/photini.ts`

```diff
@@ -1004,20 +1004,20 @@
       <source>Set default language</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>LatLongDisplay</name>
     <message>
-      <location filename="../../../photini/widgets.py" line="835"/>
+      <location filename="../../../photini/widgets.py" line="834"/>
       <source>Lat, long</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/widgets.py" line="840"/>
+      <location filename="../../../photini/widgets.py" line="839"/>
       <source>Latitude and longitude (in degrees) as two decimal numbers separated by a comma.</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>LoggerWindow</name>
     <message>
@@ -1694,362 +1694,362 @@
     </message>
     <message>
       <location filename="../../../photini/regions.py" line="70"/>
       <source>New vertex</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/regions.py" line="421"/>
+      <location filename="../../../photini/regions.py" line="419"/>
       <source>Unreadable image format</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/regions.py" line="597"/>
+      <location filename="../../../photini/regions.py" line="595"/>
       <source>pixel</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/regions.py" line="600"/>
+      <location filename="../../../photini/regions.py" line="598"/>
       <source>A pixel of a digital image setting an absolute value.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/regions.py" line="604"/>
+      <location filename="../../../photini/regions.py" line="602"/>
       <source>relative</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/regions.py" line="607"/>
+      <location filename="../../../photini/regions.py" line="605"/>
       <source>Relative part of the size of an image along the x- or the y-axis.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/regions.py" line="646"/>
+      <location filename="../../../photini/regions.py" line="644"/>
       <source>Name</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/regions.py" line="649"/>
+      <location filename="../../../photini/regions.py" line="647"/>
       <source>Free-text name of the region. Should be unique among all Region Names of an image.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/regions.py" line="658"/>
+      <location filename="../../../photini/regions.py" line="656"/>
       <source>Identifier of the region. Must be unique among all Region Identifiers of an image. Does not have to be unique beyond the metadata of this image.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/regions.py" line="660"/>
+      <location filename="../../../photini/regions.py" line="658"/>
       <source>Identifier</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/regions.py" line="666"/>
+      <location filename="../../../photini/regions.py" line="664"/>
       <source>Unit used for measuring dimensions of the boundary of a region.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/regions.py" line="669"/>
+      <location filename="../../../photini/regions.py" line="667"/>
       <source>Boundary unit</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/regions.py" line="676"/>
+      <location filename="../../../photini/regions.py" line="674"/>
       <source>Role of this region among all regions of this image or of other images. The value SHOULD be taken from a Controlled Vocabulary.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/regions.py" line="678"/>
+      <location filename="../../../photini/regions.py" line="676"/>
       <source>Role</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/regions.py" line="685"/>
+      <location filename="../../../photini/regions.py" line="683"/>
       <source>The semantic type of what is shown inside the region. The value SHOULD be taken from a Controlled Vocabulary.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/regions.py" line="688"/>
+      <location filename="../../../photini/regions.py" line="686"/>
       <source>Content type</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/regions.py" line="694"/>
+      <location filename="../../../photini/regions.py" line="692"/>
       <source>Enter the names of people shown in this region. Separate multiple entries with &quot;;&quot; characters.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/regions.py" line="697"/>
+      <location filename="../../../photini/regions.py" line="695"/>
       <source>Person shown</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/regions.py" line="701"/>
+      <location filename="../../../photini/regions.py" line="699"/>
       <source>Description</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/regions.py" line="704"/>
+      <location filename="../../../photini/regions.py" line="702"/>
       <source>Enter a &quot;caption&quot; describing the who, what, and why of what is happening in this region.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/regions.py" line="735"/>
+      <location filename="../../../photini/regions.py" line="733"/>
       <source>The Image Region Structure includes optionally any metadata property which is related to the region.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/regions.py" line="778"/>
+      <location filename="../../../photini/regions.py" line="776"/>
       <source>New rectangle</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/regions.py" line="780"/>
+      <location filename="../../../photini/regions.py" line="778"/>
       <source>New circle</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/regions.py" line="782"/>
+      <location filename="../../../photini/regions.py" line="780"/>
       <source>New point</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/regions.py" line="784"/>
+      <location filename="../../../photini/regions.py" line="782"/>
       <source>New polygon</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/regions.py" line="787"/>
+      <location filename="../../../photini/regions.py" line="785"/>
       <source>Delete region</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/regions.py" line="894"/>
+      <location filename="../../../photini/regions.py" line="892"/>
       <source>Image &amp;Regions</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>TechnicalTab</name>
     <message>
-      <location filename="../../../photini/technical.py" line="537"/>
+      <location filename="../../../photini/technical.py" line="534"/>
       <source>Maker's name</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="538"/>
+      <location filename="../../../photini/technical.py" line="535"/>
       <source>Model name</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="539"/>
+      <location filename="../../../photini/technical.py" line="536"/>
       <source>Serial number</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="563"/>
+      <location filename="../../../photini/technical.py" line="560"/>
       <source>Photini: define camera</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="577"/>
+      <location filename="../../../photini/technical.py" line="574"/>
       <source>Photini: define lens</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="597"/>
+      <location filename="../../../photini/technical.py" line="594"/>
       <source>Minimum focal length</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="599"/>
+      <location filename="../../../photini/technical.py" line="596"/>
       <source>Aperture at min. focal length</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="600"/>
+      <location filename="../../../photini/technical.py" line="597"/>
       <source>Maximum focal length</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="602"/>
+      <location filename="../../../photini/technical.py" line="599"/>
       <source>Aperture at max. focal length</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="643"/>
+      <location filename="../../../photini/technical.py" line="640"/>
       <source>&amp;Technical metadata</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="651"/>
+      <location filename="../../../photini/technical.py" line="648"/>
       <source>Date and time</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="661"/>
+      <location filename="../../../photini/technical.py" line="658"/>
       <source>Link 'taken' and 'digitised'</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="663"/>
+      <location filename="../../../photini/technical.py" line="660"/>
       <source>Link 'digitised' and 'modified'</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="665"/>
+      <location filename="../../../photini/technical.py" line="662"/>
       <source>Taken</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="668"/>
+      <location filename="../../../photini/technical.py" line="665"/>
       <source>Digitised</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="671"/>
+      <location filename="../../../photini/technical.py" line="668"/>
       <source>Modified</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="676"/>
+      <location filename="../../../photini/technical.py" line="673"/>
       <source>Adjust times</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="680"/>
+      <location filename="../../../photini/technical.py" line="677"/>
       <source>Other</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="704"/>
+      <location filename="../../../photini/technical.py" line="701"/>
       <source>Orientation</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="711"/>
+      <location filename="../../../photini/technical.py" line="708"/>
       <source>Camera</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="718"/>
+      <location filename="../../../photini/technical.py" line="715"/>
       <source>Lens model</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="725"/>
-      <location filename="../../../photini/technical.py" line="902"/>
+      <location filename="../../../photini/technical.py" line="722"/>
+      <location filename="../../../photini/technical.py" line="899"/>
       <source>Focal length</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="732"/>
+      <location filename="../../../photini/technical.py" line="729"/>
       <source>35mm equiv</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="739"/>
+      <location filename="../../../photini/technical.py" line="736"/>
       <source>Aperture</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="818"/>
+      <location filename="../../../photini/technical.py" line="815"/>
       <source>Photini: maker name change</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="821"/>
+      <location filename="../../../photini/technical.py" line="818"/>
       <source>Changing maker name will invalidate Exif makernote information.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="824"/>
+      <location filename="../../../photini/technical.py" line="821"/>
       <source>Do you want to delete the Exif makernote?</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="900"/>
+      <location filename="../../../photini/technical.py" line="897"/>
       <source>min</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="901"/>
+      <location filename="../../../photini/technical.py" line="898"/>
       <source>max</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="903"/>
+      <location filename="../../../photini/technical.py" line="900"/>
       <source>Max aperture</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="928"/>
+      <location filename="../../../photini/technical.py" line="925"/>
       <source>Update aperture &amp; focal length</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="930"/>
+      <location filename="../../../photini/technical.py" line="927"/>
       <source>Adjust image aperture and focal length to agree with lens specification?</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="687"/>
+      <location filename="../../../photini/technical.py" line="684"/>
       <source>normal</source>
       <comment>orientation dropdown, no transformation</comment>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../../../photini/technical.py" line="54"/>
       <source>Remove &quot;{camera_or_lens}&quot;</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="695"/>
+      <location filename="../../../photini/technical.py" line="692"/>
       <source>reflect left to right</source>
       <comment>orientation dropdown, horizontal reflection</comment>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="697"/>
+      <location filename="../../../photini/technical.py" line="694"/>
       <source>reflect top to bottom</source>
       <comment>orientation dropdown, vertical reflection</comment>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="699"/>
+      <location filename="../../../photini/technical.py" line="696"/>
       <source>reflect top right to bottom left</source>
       <comment>orientation dropdown, diagonal reflection</comment>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="701"/>
+      <location filename="../../../photini/technical.py" line="698"/>
       <source>reflect top left to bottom right</source>
       <comment>orientation dropdown, diagonal reflection</comment>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="689"/>
+      <location filename="../../../photini/technical.py" line="686"/>
       <source>rotate -90°</source>
       <comment>orientation dropdown</comment>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="691"/>
+      <location filename="../../../photini/technical.py" line="688"/>
       <source>rotate +90°</source>
       <comment>orientation dropdown</comment>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="693"/>
+      <location filename="../../../photini/technical.py" line="690"/>
       <source>rotate 180°</source>
       <comment>orientation dropdown</comment>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../../../photini/technical.py" line="387"/>
+      <location filename="../../../photini/technical.py" line="384"/>
       <source>Precision</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>UploaderTabsAll</name>
     <message>
```

### Comparing `Photini-2023.4.0/src/photini/__main__.py` & `Photini-2023.4.0.1/src/photini/__main__.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/address.py` & `Photini-2023.4.0.1/src/photini/address.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/bingmap.py` & `Photini-2023.4.0.1/src/photini/bingmap.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/configstore.py` & `Photini-2023.4.0.1/src/photini/configstore.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/cv.py` & `Photini-2023.4.0.1/src/photini/cv.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/data/LICENSE.txt` & `Photini-2023.4.0.1/src/photini/data/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/data/bingmap/script.js` & `Photini-2023.4.0.1/src/photini/data/bingmap/script.js`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/data/googlemap/script.js` & `Photini-2023.4.0.1/src/photini/data/googlemap/script.js`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/data/icons/photini_128.png` & `Photini-2023.4.0.1/src/photini/data/icons/photini_128.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/data/icons/photini_48.png` & `Photini-2023.4.0.1/src/photini/data/icons/photini_48.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/data/icons/photini_win.ico` & `Photini-2023.4.0.1/src/photini/data/icons/photini_win.ico`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/data/keys.txt` & `Photini-2023.4.0.1/src/photini/data/keys.txt`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/data/lang/photini.ca.qm` & `Photini-2023.4.0.1/src/photini/data/lang/photini.ca.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/data/lang/photini.cs.qm` & `Photini-2023.4.0.1/src/photini/data/lang/photini.cs.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/data/lang/photini.de.qm` & `Photini-2023.4.0.1/src/photini/data/lang/photini.de.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/data/lang/photini.en.qm` & `Photini-2023.4.0.1/src/photini/data/lang/photini.en.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/data/lang/photini.es.qm` & `Photini-2023.4.0.1/src/photini/data/lang/photini.es.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/data/lang/photini.fr.qm` & `Photini-2023.4.0.1/src/photini/data/lang/photini.fr.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/data/lang/photini.it.qm` & `Photini-2023.4.0.1/src/photini/data/lang/photini.it.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/data/lang/photini.ko.qm` & `Photini-2023.4.0.1/src/photini/data/lang/photini.ko.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/data/lang/photini.nb.qm` & `Photini-2023.4.0.1/src/photini/data/lang/photini.nb.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/data/lang/photini.pl.qm` & `Photini-2023.4.0.1/src/photini/data/lang/photini.pl.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/data/linux/photini.desktop` & `Photini-2023.4.0.1/src/photini/data/linux/photini.desktop`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/data/map_pin_grey.png` & `Photini-2023.4.0.1/src/photini/data/map_pin_grey.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/data/map_pin_red.png` & `Photini-2023.4.0.1/src/photini/data/map_pin_red.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/data/mapboxmap/script.js` & `Photini-2023.4.0.1/src/photini/data/mapboxmap/script.js`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/data/windows/install_shortcuts.vbs` & `Photini-2023.4.0.1/src/photini/data/windows/install_shortcuts.vbs`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/descriptive.py` & `Photini-2023.4.0.1/src/photini/descriptive.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/editor.py` & `Photini-2023.4.0.1/src/photini/editor.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/editsettings.py` & `Photini-2023.4.0.1/src/photini/editsettings.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/exiv2.py` & `Photini-2023.4.0.1/src/photini/exiv2.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/ffmpeg.py` & `Photini-2023.4.0.1/src/photini/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/flickr.py` & `Photini-2023.4.0.1/src/photini/flickr.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/googlemap.py` & `Photini-2023.4.0.1/src/photini/googlemap.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/googlephotos.py` & `Photini-2023.4.0.1/src/photini/googlephotos.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/gpximporter.py` & `Photini-2023.4.0.1/src/photini/gpximporter.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/imagelist.py` & `Photini-2023.4.0.1/src/photini/imagelist.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/importer.py` & `Photini-2023.4.0.1/src/photini/importer.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/ipernity.py` & `Photini-2023.4.0.1/src/photini/ipernity.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/loggerwindow.py` & `Photini-2023.4.0.1/src/photini/loggerwindow.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/mapboxmap.py` & `Photini-2023.4.0.1/src/photini/mapboxmap.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/metadata.py` & `Photini-2023.4.0.1/src/photini/metadata.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/ownership.py` & `Photini-2023.4.0.1/src/photini/ownership.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/photinimap.py` & `Photini-2023.4.0.1/src/photini/photinimap.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/pixelfed.py` & `Photini-2023.4.0.1/src/photini/pixelfed.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/pyqt.py` & `Photini-2023.4.0.1/src/photini/pyqt.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/regions.py` & `Photini-2023.4.0.1/src/photini/regions.py`

 * *Files 0% similar despite different names*

```diff
@@ -378,16 +378,14 @@
     new_value = QtSignal(int, dict)
 
     def __init__(self, *arg, **kw):
         super(ImageDisplayWidget, self).__init__(*arg, **kw)
         self.setRenderHint(
             QtGui.QPainter.RenderHint.Antialiasing, True)
         self.setRenderHint(
-            QtGui.QPainter.RenderHint.HighQualityAntialiasing, True)
-        self.setRenderHint(
             QtGui.QPainter.RenderHint.SmoothPixmapTransform, True)
         self.setScene(QtWidgets.QGraphicsScene())
         self.boundary = None
 
     def set_image(self, image):
         self.image = image
         scene = self.scene()
```

### Comparing `Photini-2023.4.0/src/photini/scripts.py` & `Photini-2023.4.0.1/src/photini/scripts.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/spelling.py` & `Photini-2023.4.0.1/src/photini/spelling.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/technical.py` & `Photini-2023.4.0.1/src/photini/technical.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,21 +149,20 @@
         self.app.config_store.remove_section('lens ' + lens_model.get_name())
         return super(LensList, self).remove_item(lens_model, **kwds)
 
     def data_to_text(self, lens_model):
         return lens_model.get_name()
 
 
-class IntSpinBox(QtWidgets.QSpinBox, AugmentSpinBox):
+class IntSpinBox(AugmentSpinBox, QtWidgets.QSpinBox):
     def __init__(self, key, *arg, **kw):
         self.default_value = 0
         self.multiple = multiple_values()
         self._key = key
         super(IntSpinBox, self).__init__(*arg, **kw)
-        AugmentSpinBox.__init__(self)
         self.setSingleStep(1)
         lim = (2 ** 31) - 1
         self.setRange(-lim, lim)
         self.setButtonSymbols(self.ButtonSymbols.NoButtons)
 
     @catch_all
     def contextMenuEvent(self, event):
@@ -197,27 +196,26 @@
     @catch_all
     def showEvent(self, event):
         if self.selectedDate() == self.minimumDate():
             self.setSelectedDate(QtCore.QDate.currentDate())
         return super(CalendarWidget, self).showEvent(event)
 
 
-class DateTimeEdit(QtWidgets.QDateTimeEdit, AugmentDateTime):
+class DateTimeEdit(AugmentDateTime, QtWidgets.QDateTimeEdit):
     def __init__(self, key, *arg, **kw):
         self.default_value = QtCore.QDateTime(
             QtCore.QDate.currentDate(), QtCore.QTime())
         self.multiple = multiple_values()
         self._key = key
         # rename some methods for compatibility with AugmentSpinBox
         self.minimum = self.minimumDateTime
         self.setValue = self.setDateTime
         self.textFromValue = self.textFromDateTime
         self.value = self.dateTime
         super(DateTimeEdit, self).__init__(*arg, **kw)
-        AugmentDateTime.__init__(self)
         self.setCalendarPopup(True)
         self.setCalendarWidget(CalendarWidget())
         self.precision = 1
         self.set_precision(7)
 
     @catch_all
     def contextMenuEvent(self, event):
@@ -261,21 +259,20 @@
         if value != self.precision:
             self.precision = value
             self.setDisplayFormat(
                 ''.join(('yyyy', '-MM', '-dd',
                          ' hh', ':mm', ':ss', '.zzz')[:self.precision]))
 
 
-class TimeZoneWidget(QtWidgets.QSpinBox, AugmentSpinBox):
+class TimeZoneWidget(AugmentSpinBox, QtWidgets.QSpinBox):
     def __init__(self, key, *arg, **kw):
         self.default_value = 0
         self.multiple = multiple()
         self._key = key
         super(TimeZoneWidget, self).__init__(*arg, **kw)
-        AugmentSpinBox.__init__(self)
         self.setRange(-14 * 60, 15 * 60)
         self.setSingleStep(15)
         self.setWrapping(True)
 
     @catch_all
     def contextMenuEvent(self, event):
         self.context_menu_event()
```

### Comparing `Photini-2023.4.0/src/photini/types.py` & `Photini-2023.4.0.1/src/photini/types.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/uploader.py` & `Photini-2023.4.0.1/src/photini/uploader.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/src/photini/widgets.py` & `Photini-2023.4.0.1/src/photini/widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -700,19 +700,19 @@
         for choice in choices:
             self.choices[str(choice)] = MD_LangAlt(choice, strip=False)
         self.edit.set_multiple(choices=self.choices.keys())
         self.lang.setEnabled(False)
 
 
 class AugmentSpinBoxBase(WidgetMixin):
-    def __init__(self):
+    def __init__(self, *arg, **kw):
         self._is_multiple = False
         self._prefix = ''
         self._suffix = ''
-        super(AugmentSpinBoxBase, self).__init__()
+        super(AugmentSpinBoxBase, self).__init__(*arg, **kw)
         if self.isRightToLeft():
             self.setAlignment(
                 Qt.AlignmentFlag.AlignRight | Qt.AlignmentFlag.AlignVCenter)
         self.set_value(None)
         self.editingFinished.connect(self.emit_value)
 
     class ContextAction(QtGui2.QAction):
@@ -816,21 +816,20 @@
         self.setPrefix(prefix)
 
     def set_suffix(self, suffix):
         self._suffix = suffix
         self.setSuffix(suffix)
 
 
-class LatLongDisplay(QtWidgets.QAbstractSpinBox, AugmentSpinBox):
+class LatLongDisplay(AugmentSpinBox, QtWidgets.QAbstractSpinBox):
     def __init__(self, *args, **kwds):
         self._key = ('exif:GPSLatitude', 'exif:GPSLongitude')
         self.default_value = ''
         self.multiple = multiple_values()
         super(LatLongDisplay, self).__init__(*args, **kwds)
-        AugmentSpinBox.__init__(self)
         self.lat_validator = QtGui.QDoubleValidator(
             -90.0, 90.0, 20, parent=self)
         self.lng_validator = QtGui.QDoubleValidator(
             -180.0, 180.0, 20, parent=self)
         self.setButtonSymbols(self.ButtonSymbols.NoButtons)
         self.label = QtWidgets.QLabel(translate('LatLongDisplay', 'Lat, long'))
         self.label.setAlignment(Qt.AlignmentFlag.AlignRight)
@@ -875,18 +874,20 @@
     def validate(self, text, pos):
         if not text:
             return QtGui.QValidator.State.Acceptable, text, pos
         parts = [x.strip() for x in text.split(',')]
         if len(parts) > 2:
             return QtGui.QValidator.State.Invalid, text, pos
         result = self.lat_validator.validate(parts[0], pos)[0]
-        if len(parts) > 1:
-            result = min(result, self.lng_validator.validate(parts[1], pos)[0])
-        else:
-            result = min(result, QtGui.QValidator.State.Intermediate)
+        if result != QtGui.QValidator.State.Invalid and len(parts) > 1:
+            lng_result = self.lng_validator.validate(parts[1], pos)[0]
+            if lng_result == QtGui.QValidator.State.Invalid:
+                result = lng_result
+            elif result == QtGui.QValidator.State.Acceptable:
+                result = lng_result
         return result, text, pos
 
     @catch_all
     def fixup(self, value):
         value = value.split(',')
         if len(value) != 2 or not all(value):
             return
@@ -930,21 +931,20 @@
             choices.add(None)
         if len(choices) > 1:
             self.set_multiple(choices=[x for x in choices if x])
         else:
             self.set_value(choices and choices.pop())
 
 
-class DoubleSpinBox(QtWidgets.QDoubleSpinBox, AugmentSpinBox):
+class DoubleSpinBox(AugmentSpinBox, QtWidgets.QDoubleSpinBox):
     def __init__(self, key, *arg, **kw):
         self._key = key
         self.default_value = 0
         self.multiple = multiple_values()
         super(DoubleSpinBox, self).__init__(*arg, **kw)
-        AugmentSpinBox.__init__(self)
         self.setSingleStep(0.1)
         self.setDecimals(4)
         lim = (2 ** 31) - 1
         self.setRange(-lim, lim)
         self.setButtonSymbols(self.ButtonSymbols.NoButtons)
 
     @catch_all
```

### Comparing `Photini-2023.4.0/src/run_photini.py` & `Photini-2023.4.0.1/src/run_photini.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/utils/build_docs.py` & `Photini-2023.4.0.1/utils/build_docs.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/utils/build_lang.py` & `Photini-2023.4.0.1/utils/build_lang.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/utils/download_cvs.py` & `Photini-2023.4.0.1/utils/download_cvs.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/utils/lang_update.py` & `Photini-2023.4.0.1/utils/lang_update.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/utils/localise_desktop.py` & `Photini-2023.4.0.1/utils/localise_desktop.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/utils/make_icons/icon_master.png` & `Photini-2023.4.0.1/utils/make_icons/icon_master.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/utils/make_icons/makefile` & `Photini-2023.4.0.1/utils/make_icons/makefile`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/utils/tag_release.py` & `Photini-2023.4.0.1/utils/tag_release.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0/utils/update_version.py` & `Photini-2023.4.0.1/utils/update_version.py`

 * *Files identical despite different names*

