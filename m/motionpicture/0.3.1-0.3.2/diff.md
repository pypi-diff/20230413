# Comparing `tmp/motionpicture-0.3.1.tar.gz` & `tmp/motionpicture-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motionpicture-0.3.1.tar", max compression
+gzip compressed data, was "motionpicture-0.3.2.tar", max compression
```

## Comparing `motionpicture-0.3.1.tar` & `motionpicture-0.3.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    35149 2021-11-12 20:15:56.502413 motionpicture-0.3.1/LICENSE
--rw-r--r--   0        0        0    13639 2022-04-29 17:12:06.380649 motionpicture-0.3.1/README.md
--rwxr-xr-x   0        0        0      720 2022-07-06 12:01:02.475300 motionpicture-0.3.1/motionpicture/__init__.py
--rwxr-xr-x   0        0        0    17198 2022-07-06 11:59:55.825381 motionpicture-0.3.1/motionpicture/argparse.py
--rwxr-xr-x   0        0        0     5293 2022-05-16 00:48:29.605156 motionpicture-0.3.1/motionpicture/mopi.py
--rwxr-xr-x   0        0        0    14523 2022-04-29 17:16:07.113530 motionpicture-0.3.1/motionpicture/moviemaker.py
--rw-r--r--   0        0        0     1213 2022-07-06 12:00:57.361230 motionpicture-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    14877 2022-07-06 12:02:04.576373 motionpicture-0.3.1/setup.py
--rw-r--r--   0        0        0    14681 2022-07-06 12:02:04.577958 motionpicture-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-11-12 20:15:56.502413 motionpicture-0.3.2/LICENSE
+-rw-r--r--   0        0        0    13639 2022-04-29 17:12:06.380649 motionpicture-0.3.2/README.md
+-rw-r--r--   0        0        0    69632 2021-11-12 20:15:56.548415 motionpicture-0.3.2/motionpicture/.coverage
+-rwxr-xr-x   0        0        0      720 2023-04-13 16:15:07.663984 motionpicture-0.3.2/motionpicture/__init__.py
+-rwxr-xr-x   0        0        0    17198 2023-04-13 16:15:07.663984 motionpicture-0.3.2/motionpicture/argparse.py
+-rwxr-xr-x   0        0        0     5293 2023-04-13 16:15:07.663984 motionpicture-0.3.2/motionpicture/mopi.py
+-rwxr-xr-x   0        0        0    14523 2023-04-13 16:15:07.667984 motionpicture-0.3.2/motionpicture/moviemaker.py
+-rw-r--r--   0        0        0     1205 2023-04-13 16:14:23.183850 motionpicture-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0    14870 1970-01-01 00:00:00.000000 motionpicture-0.3.2/setup.py
+-rw-r--r--   0        0        0    14725 1970-01-01 00:00:00.000000 motionpicture-0.3.2/PKG-INFO
```

### Comparing `motionpicture-0.3.1/LICENSE` & `motionpicture-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `motionpicture-0.3.1/README.md` & `motionpicture-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `motionpicture-0.3.1/motionpicture/__init__.py` & `motionpicture-0.3.2/motionpicture/__init__.py`

 * *Files identical despite different names*

### Comparing `motionpicture-0.3.1/motionpicture/argparse.py` & `motionpicture-0.3.2/motionpicture/argparse.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright (C) 2020-2021 Gabriele Bozzola
+# Copyright (C) 2020-2023 Gabriele Bozzola
 #
 # This program is free software; you can redistribute it and/or modify it under
 # the terms of the GNU General Public License as published by the Free Software
 # Foundation; either version 3 of the License, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
```

### Comparing `motionpicture-0.3.1/motionpicture/mopi.py` & `motionpicture-0.3.2/motionpicture/mopi.py`

 * *Files identical despite different names*

### Comparing `motionpicture-0.3.1/motionpicture/moviemaker.py` & `motionpicture-0.3.2/motionpicture/moviemaker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright (C) 2020-2021 Gabriele Bozzola
+# Copyright (C) 2020-2023 Gabriele Bozzola
 #
 # This program is free software; you can redistribute it and/or modify it under
 # the terms of the GNU General Public License as published by the Free Software
 # Foundation; either version 3 of the License, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
```

### Comparing `motionpicture-0.3.1/pyproject.toml` & `motionpicture-0.3.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [tool.poetry]
 name = "motionpicture"
-version = "0.3.1"
+version = "0.3.2"
 description = "Make animations with Python"
 authors = ["Gabriele Bozzola <gabrielebozzola@arizona.edu>"]
 maintainers = ["Gabriele Bozzola <gabrielebozzola@arizona.edu>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/sbozzolo/motionpicture"
 repository = "https://github.com/sbozzolo/motionpicture"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/sbozzolo/motionpicture/issues"
 
 [tool.poetry.dependencies]
-python = "^3.6.2, <3.11"
+python = ">3.6.2"
 ffmpeg-python = "^0.1.0"
 ConfigArgParse = "^1.0.0"
 tqdm = "^4.0.0"
 python-magic = "^0.4.27"
 
 [tool.poetry.dev-dependencies]
 black = "^22.3.0"
 pytest = "^6.2.1"
 pytest-cov = "^2.10.1"
-# Older NumPy version doe not support Python 3.10, so we have to install it (for
+# Older NumPy version do not support Python 3.10, so we have to install it (for
 # matplotlib, which is only needed to make plots in the README)
 numpy = [
     { version = "^1.18.5", python = ">=3.6, <3.10" },
     { version = "^1.21.4", python = ">=3.10" },
 ]
 matplotlib = "^3.3.3"
```

### Comparing `motionpicture-0.3.1/setup.py` & `motionpicture-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,24 +14,24 @@
  'tqdm>=4.0.0,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['mopi = motionpicture.mopi:main']}
 
 setup_kwargs = {
     'name': 'motionpicture',
-    'version': '0.3.1',
+    'version': '0.3.2',
     'description': 'Make animations with Python',
     'long_description': '<p align="center">\n<img src="https://github.com/Sbozzolo/motionpicture/raw/master/logo.png" width="636" height="131">\n</p>\n\n[![GPLv3\nlicense](https://img.shields.io/badge/License-GPLv3-blue.svg)](http://perso.crans.org/besson/LICENSE.html)\n![Tests and documentation](https://github.com/Sbozzolo/motionpicture/workflows/Tests/badge.svg)\n[![codecov](https://codecov.io/gh/Sbozzolo/motionpicture/branch/master/graph/badge.svg?token=z7jvNNdwVS)](https://codecov.io/gh/Sbozzolo/motionpicture)\n[![PyPI version](https://badge.fury.io/py/motionpicture.svg)](https://badge.fury.io/py/motionpicture)\n\n# Introduction\n\n`motionpicture` is a Python library to simplify the creation of videos out of\nindividual frames. With `motionpicture`, you just have to specify how to produce\na generic frame, and the package will do everything else for you. In\n`motionpicture`, your code can be configured via command-line or text files:\nturning your code into a plug-in for `motionpicture` is trivial, so you will be\nable to reuse your code with ease.\n\n# Examples\n\nThere are two important ingredients to use `motionpicture`: `mopi`, and a\n_movie_ file. `mopi` is a command-line utility that comes when you install this\npackage. It will be your main interface to `motionpicture` and it has a\ncomprehensive `--help` function. A movie file is a recipe on how to produce a\ngeneric frame. With few small restrictions, you have full control over this file\n(more info in section [Movie files](#movie-files)).\n\nIn these examples we are going to use `matplotlib` to do the plotting, but you\nare completely free to generate frames with any Python package you wish.\n\n## Unveiling a sine wave\n\nIn this example, we show how to use `mopi` to generate the following video.\n![sine_wave](https://github.com/Sbozzolo/motionpicture/raw/master/sine_wave.gif)\n\nTo produce this video, we need the following movie file.\n``` python\nimport matplotlib.pyplot as plt\nimport numpy as np\n\nclass MOPIMovie:\n    def __init__(self, _args):\n        self.times = np.linspace(0, 10, 100)\n        self.values = np.sin(self.times)\n\n    def get_frames(self):\n        # Here we tell motionpicture what we consider a frame\n        return range(self.times)\n\n    def make_frame(self, path, frame_number):\n        # Here we plot a specific frame\n        plt.clf()\n        plt.plot(self.times[:frame_number], self.values[:frame_number])\n        plt.xlim([0, self.times[-1]])\n        plt.ylim([-1, 1])\n        plt.savefig(path)\n```\nAssuming this file is saved in `sin_wave.py`, we run\n\n``` sh\nmopi -m sin_wave.py -o frames_dir --parallel\n```\nThis is produce the individual frames in a folder `frames_dir` using all the CPUs\navailable on your machine. Then, it will glue the frames together in a video\nthat has the default name of `video.mp4`. If you want to change name, or other\nproperties (e.g., the fps), you can add options to `mopi`\n``` sh\nmopi -m sin_wave.py -o frames_dir --parallel --fps 10 --movie-name sin_wave\n```\nThis will produce a `sin_wave.mp4` video with 10 frames per second instead\n\n## Unveiling a sine wave with controllable frequency\n\nLet us continue on the example of the sine wave, and let us assume that we want\nto explore different frequencies.\n\nWe can edit the previous movie file adding a `mopi_add_custom_options`\nfunction:\n\n``` python\ndef mopi_add_custom_options(parser):\n    """Add command-line options specific to this movie."""\n    parser.add_argument(\n        "-f",\n        "--frequency",\n        default=1,\n        type=int,\n        help="Frequency of the sine wave (default: %(default)s)",\n    )\n```\nThen, we edit the `__init__` function too:\n``` python\ndef __init__(self, args):\n    self.times = np.linspace(0, 10, 100)\n    self.values = np.sin(args.frequency * self.times)\n```\nMovie files have to have an `__init__` that takes two arguments. The second\nis a `Namespace` that contains all the controllable options. These arguments\ncan be passed via command-line or configuration file.\n``` sh\nmopi -m sin_wave.py -o frames_dir --parallel --frequency 3\n```\nThis command will produce the following video.\n\n![sine_wave_fast](https://github.com/Sbozzolo/motionpicture/raw/master/sine_wave_fast.gif)\n\nAlternatively, you can put any of arguments in a config file `conf`, for example:\n\n``` text\noutdir: frames_dir\nfrequency: 3\n```\nConfig files support several syntaxes. Once you have the file, just call\n``` sh\nmopi sin_wave.py -c conf\n```\nYou can use config files and command-line options at the same time, but in case\nof conflict, the command-line arguments have the precedence.\n\n## Unveiling data in an arbitrary file\n\nNow that you have seen that you can control movies via command-line, it is time\nto introduce you to the plugin system in `motionpicture`.\n\nSuppose we have two-column files with time series data, we can modify the movie\nfile used in the previous example to animate those files, specifying which one\nat run-time.\n\n``` python\ndef mopi_add_custom_options(parser):\n    """Add command-line options specific to this movie."""\n    parser.add_argument(\n        "-f",\n        "--file",\n        required=True,\n        help="File to plot",\n    )\n```\nThen, we `import numpy as np` and edit the `__init__` function too:\n``` python\ndef __init__(self, args):\n    self.times, self.values = np.loadtxt(args.file).T\n    self.y_min, self.y_max = np.amin(self.value), np.amax(self.value)\n```\nWe computed the minimum and maximum of the value so that we can adjust the y axis\nrange. The  `make_frame` method will be the same, with the exception that we change\nthe `plt.ylim([-1, 1])` line to `plt.ylim([self.y_min, self.y_max])`.\n\nWe can save this file as `plot_timeseries` and call `mopi`:\n``` sh\nmopi -m plot_timeseries -o frames -f my_file.dat\n```\nOf course, we can add as many options as we wish to control the output. For instance,\nwe may want to add a switch to use logarithmic axes instead. The class\n`MOPIMovie` has full access to the user-supplied options, so you can do anything\nyou wish.\n\nWe did not hard-code anything in `plot_timeseries`, so the code will work for\nany dataset. However, if we want to use this file again, but in a different\nfolder, we would have to copy it over, since `mopi -m` expects the path of the\nmovie file. Alternatively, we can copy `plot_timeseries` to a specific folder\nof our choice, for example `~/.mopi_videos`. Then, we can set the environment\nvariable `MOPI_MOVIES_DIR` to be `~/.mopi_videos`, and `mopi` will be able to\nfind `plot_timeseries` from anywhere in your filesystem. In this case, you can\nsimply call:\n``` sh\nmopi plot_timeseries -o frames -f my_other_file.dat\n```\nEssentially, `plot_timeseries` became a plugin for `motionpicture` and you can\nanimate any data without having to write new code. This is one of the greatest\nstrengths of `motionpicture`, as it encourages you to write generic code that you\ncan easily reuse.\n\n# Installation\n\n`motionpicture` is available on PyPI. You can install it with `pip`:\n\n``` sh\npip3 install motionpicture\n```\n\nTo produce the final video, you have to have `ffmpeg` installed. Without\n`ffmpeg`, you will not be able to glue together the frames, but you can still\nuse `motionpicture` to render the frames.\n\n# Movie files\n\nIn the language of `motionpicture`, a movie file is a recipe on how to\ngenerate an individual frame. It is completely up to you how you do that, but\n`motionpicture` imposes some minimum requirements:\n\n- It has to be a valid Python 3 file.\n- It has to contain a class `MOPIMovie` with a method `make_frame` and a method\n  `get_frames`.\n- The method `__init__` has to take two arguments.\n- The method `get_frames` has to return an iterable (e.g., a list) that\n  identifies each frame. The elements of this iterable are passed as the `frame`\n  argument to `make_frame`.\n- The method `make_frame` has to take two arguments, the `path` of the output of\n  the frame, and `frame`, the value that identifies frame (typically the frame\n  number). `path` is where the image has to be saved. You are in charge of\n  saving the image using the save method of your plotting package.\n\nOther than these requirements, you can do anything you want in the movie file\n(e.g., you can add more methods, functions, classes...).\n\nTo have support for the `--overwrite` option, the function `make_frame` must\nalways write the data regardless of possible pre-existing files at destination.\n\n> :warning: Due to its own nature, `motionpicture` has to execute any code that\n>           you supply. Do not use `motionpicture` with codes you do not trust!\n\n# `mopi`\n\n`mopi` is a command-line utility with several options. Its `--help` flag can\ntell you what it can do:\n``` text\nGeneral options:\n  movie                 Movie to render among the ones found in MOPI_MOVIES_DIR. See bottom of the help message for list.\n  -m MOVIE_FILE, --movie-file MOVIE_FILE\n                        Path of the movie file.\n  -c CONFIG, --config CONFIG\n                        Config file path\n  --movies-dir MOVIES_DIR\n                        Folder where to look form movies.   [env var: MOPI_MOVIES_DIR]\n  -o OUTDIR, --outdir OUTDIR\n                        Output directory for frames and video.\n  --snapshot SNAPSHOT   Only produce the specified snapshot (useful for testing).\n  --overwrite           Overwrite files that already exist.\n  --disable-progress-bar\n                        Do not display the progress bar when generating frames.\n  --parallel            Render frames in parallel.\n  --skip-existing       Do not generate frames that already exist. No consistency checks are performed.\n  --num-workers NUM_WORKERS\n                        Number of cores to use (default: 8).\n  --max-tasks-per-child MAX_TASKS_PER_CHILD\n                        How many chunks does a worker have to process before it is respawned? Higher number typically leads to higher performance\n                        and higher memory usage. (default: 1).\n  --chunks-size CHUNKS_SIZE\n                        How many frames does a worker have to do each time? Higher number typically leads to higher performance and higher memory usage.\n  --only-render-movie   Do not generate frames but only render the final video.\n  --frame-name-format FRAME_NAME_FORMAT\n                        If only-render-movie is set, use this C-style frame name format instead of computing it. For example, \'%04d.png\' will\n                        assemble a video with frames with names 0000.png, 0001.png, and so on, as found in the outdir folder.\n  -v, --verbose         Enable verbose output.\n  -h, --help            Show this help message and exit.\n\nFrame selection:\n  --min-frame MIN_FRAME\n                        Do not render frames before this one.\n  --max-frame MAX_FRAME\n                        Do not render frames after this one.\n  --frames-every FRAMES_EVERY\n                        Render a frame every N (default: render all the possible frames).\n\nVideo rendering options:\n  --movie-name MOVIE_NAME\n                        Name of output video file, without extension (default: video).\n  --extension EXTENSION\n                        File extension of the video (default: mp4).\n  --fps FPS             Frames-per-second of the video (default: 25).\n  --codec CODEC         Codec to use for the final encoding. If not specified, it is determined from the file extension.\n  --author AUTHOR       Author metadata in the final video.\n  --title TITLE         Title metadata in the final video.\n  --comment COMMENT     Comment metadata in the final video.\n\nNo movies found in the MOPI_MOVIES_DIR (.)\n```\n\nA useful option for debugging is `--snapshot`. If you pass the keyword\n`--snapshot` and the identifier for a specific frame (an element of the iterable\n`MOPIMoive.get_frames()`), `mopi` will only render that single frame. This\ncan be used to test your movie file.\n\nAnother interesting option is `--only-render-movie`. This skips the generation\nof frames and only produces the final video. When this option is enable, `mopi`\nwill still go through the selection of frames from the movie file, so options\nlike `--min-frame` or `--frames-every` will affect the result. If you specify\nalso `--frame-name-format`, you can skip this step too (which skips the movie\nfile entirely), and just render the final video. This option requires a C-style\nformat string to specify which files have to be assembled to the final video.\nThis refers to the name of the files in the output folder.\n\n# Development\n\nWe use:\n* [Poetry](python-poetry.org) to manage dependencies, build, and publish\n  `motionpicture`.\n* [Black](https://github.com/psf/black) for formatting the code (with 89\n  columns).\n* [pytest](https://pytest.org) for unit tests (with `pytest-cov` for test\n  coverage).\n* GitHub actions for continuous integration.\n\nWe are happy to accept contributions.\n\n## A note on the inner workings\n\nMultiprocessing with Python is a pain. Hence, we need to hack our way lo support\nparallelism in such a way that is completely transparent to the user. To achieve\nthis `motionpicture` uses two tricks:\n- The movie file is evaluated verbatim with `exec` in the global namespace\n- The `MOPIMovie` class is patched to a `pMOPIMovie` (always using `exec`) to\n  provide a function `p_make_frames` that works better with `multiprocessing`.\n\nSo, `motionpicture` directly manipulates the global namespace to be able to\nuse multiple processes. This can lead to surprises in the code, for example,\n`MOPIMovie` is used without apparently being imported.\n\n# Changelog\n\nSee [NEWS.md](https://github.com/Sbozzolo/motionpicture/blob/master/NEWS.md) for\na changelog.\n\n# Credits\n\nThe idea for `motionpicture` originated from the `SimVideo` package developed by\nWolfgang Kastaun.\n\n',
     'author': 'Gabriele Bozzola',
     'author_email': 'gabrielebozzola@arizona.edu',
     'maintainer': 'Gabriele Bozzola',
     'maintainer_email': 'gabrielebozzola@arizona.edu',
     'url': 'https://github.com/sbozzolo/motionpicture',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.6.2,<3.11',
+    'python_requires': '>3.6.2',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `motionpicture-0.3.1/PKG-INFO` & `motionpicture-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: motionpicture
-Version: 0.3.1
+Version: 0.3.2
 Summary: Make animations with Python
 Home-page: https://github.com/sbozzolo/motionpicture
 License: GPL-3.0-or-later
 Author: Gabriele Bozzola
 Author-email: gabrielebozzola@arizona.edu
 Maintainer: Gabriele Bozzola
 Maintainer-email: gabrielebozzola@arizona.edu
-Requires-Python: >=3.6.2,<3.11
+Requires-Python: >3.6.2
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ConfigArgParse (>=1.0.0,<2.0.0)
 Requires-Dist: ffmpeg-python (>=0.1.0,<0.2.0)
 Requires-Dist: python-magic (>=0.4.27,<0.5.0)
 Requires-Dist: tqdm (>=4.0.0,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/sbozzolo/motionpicture/issues
 Project-URL: Repository, https://github.com/sbozzolo/motionpicture
 Description-Content-Type: text/markdown
```

