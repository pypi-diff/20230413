# Comparing `tmp/powerplayer-0.2.0.tar.gz` & `tmp/powerplayer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powerplayer-0.2.0.tar", max compression
+gzip compressed data, was "powerplayer-0.2.1.tar", max compression
```

## Comparing `powerplayer-0.2.0.tar` & `powerplayer-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1097 2021-07-11 10:15:45.887029 powerplayer-0.2.0/LICENSE.MD
--rw-r--r--   0        0        0     4511 2021-11-26 05:23:44.739683 powerplayer-0.2.0/powerplayer.py
--rw-r--r--   0        0        0     1077 2021-11-25 16:12:04.906077 powerplayer-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      917 2021-09-12 16:22:05.648607 powerplayer-0.2.0/README.md
--rw-r--r--   0        0        0     1820 2021-11-26 06:03:53.078710 powerplayer-0.2.0/setup.py
--rw-r--r--   0        0        0     1913 2021-11-26 06:03:53.078710 powerplayer-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1097 2021-07-11 10:15:45.887029 powerplayer-0.2.1/LICENSE.MD
+-rw-r--r--   0        0        0     4511 2023-04-13 15:53:55.653870 powerplayer-0.2.1/powerplayer.py
+-rw-r--r--   0        0        0     1129 2023-04-13 15:54:17.837980 powerplayer-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1190 2023-04-13 15:50:22.469817 powerplayer-0.2.1/README.md
+-rw-r--r--   0        0        0     2100 2023-04-13 15:54:29.584554 powerplayer-0.2.1/setup.py
+-rw-r--r--   0        0        0     2243 2023-04-13 15:54:29.584554 powerplayer-0.2.1/PKG-INFO
```

### Comparing `powerplayer-0.2.0/LICENSE.MD` & `powerplayer-0.2.1/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `powerplayer-0.2.0/powerplayer.py` & `powerplayer-0.2.1/powerplayer.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     'quiet': True,
     'prefer_ffmpeg': True,
     'audioformat': 'mp3',
     'forceduration':True}
 
 @click.group(
     cls=HelpColorsGroup, help_headers_color="yellow", help_options_color="cyan")
-@click.version_option('0.2.0')
+@click.version_option('0.2.1')
 def main():
     """PowerPlayer - Play music in your terminal"""
 @main.command('yt', help = 'Play music from youtube. Give the song name')
 @click.argument('song', nargs = -1)
 def playfromyt(song):
     music_name = " ".join(song)
```

### Comparing `powerplayer-0.2.0/pyproject.toml` & `powerplayer-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
 00000010: 616d 6520 3d20 2270 6f77 6572 706c 6179  ame = "powerplay
 00000020: 6572 220d 0a76 6572 7369 6f6e 203d 2022  er"..version = "
-00000030: 302e 322e 3022 0d0a 6465 7363 7269 7074  0.2.0"..descript
+00000030: 302e 322e 3122 0d0a 6465 7363 7269 7074  0.2.1"..descript
 00000040: 696f 6e20 3d20 2241 2063 6f6d 6d61 6e64  ion = "A command
 00000050: 206c 696e 6520 696e 7465 7266 6163 6520   line interface 
 00000060: 746f 2070 6c61 7920 6d75 7369 6322 0d0a  to play music"..
 00000070: 6175 7468 6f72 7320 3d20 5b22 4176 616e  authors = ["Avan
 00000080: 696e 6472 6120 4368 616b 7261 626f 7274  indra Chakrabort
 00000090: 7922 5d0d 0a6c 6963 656e 7365 203d 2022  y"]..license = "
 000000a0: 4d49 5422 0d0a 7265 6164 6d65 3d22 5245  MIT"..readme="RE
@@ -32,37 +32,40 @@
 000001f0: 3a20 5079 7468 6f6e 203a 3a20 332e 3722  : Python :: 3.7"
 00000200: 2c0d 0a20 2020 2020 2020 2022 5072 6f67  ,..        "Prog
 00000210: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
 00000220: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
 00000230: 3822 2c0d 0a09 2250 726f 6772 616d 6d69  8",..."Programmi
 00000240: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
 00000250: 7974 686f 6e20 3a3a 2033 2e39 222c 0d0a  ython :: 3.9",..
-00000260: 2020 2020 2020 2020 224f 7065 7261 7469          "Operati
-00000270: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
-00000280: 496e 6465 7065 6e64 656e 7422 2c0d 0a20  Independent",.. 
-00000290: 2020 205d 0d0a 0d0a 5b74 6f6f 6c2e 706f     ]....[tool.po
-000002a0: 6574 7279 2e64 6570 656e 6465 6e63 6965  etry.dependencie
-000002b0: 735d 0d0a 7079 7468 6f6e 203d 2022 5e33  s]..python = "^3
-000002c0: 2e37 220d 0a63 6c69 636b 203d 2022 5e38  .7"..click = "^8
-000002d0: 2e30 2e31 220d 0a63 6c69 636b 2d68 656c  .0.1"..click-hel
-000002e0: 702d 636f 6c6f 7273 203d 2022 5e30 2e39  p-colors = "^0.9
-000002f0: 2e31 220d 0a62 7334 203d 2022 5e30 2e30  .1"..bs4 = "^0.0
-00000300: 2e31 220d 0a72 6571 7565 7374 7320 3d20  .1"..requests = 
-00000310: 225e 322e 3235 2e31 220d 0a70 6c61 7973  "^2.25.1"..plays
-00000320: 6f75 6e64 203d 2022 5e31 2e32 2e32 220d  ound = "^1.2.2".
-00000330: 0a70 7974 686f 6e2d 766c 6320 3d20 225e  .python-vlc = "^
-00000340: 332e 302e 3132 3131 3822 0d0a 796f 7574  3.0.12118"..yout
-00000350: 7562 655f 646c 203d 2022 5e32 3032 312e  ube_dl = "^2021.
-00000360: 362e 3622 0d0a 796f 7574 7562 652d 7365  6.6"..youtube-se
-00000370: 6172 6368 203d 2022 322e 312e 3022 0d0a  arch = "2.1.0"..
-00000380: 5b74 6f6f 6c2e 706f 6574 7279 2e64 6576  [tool.poetry.dev
-00000390: 2d64 6570 656e 6465 6e63 6965 735d 0d0a  -dependencies]..
-000003a0: 0d0a 5b74 6f6f 6c2e 706f 6574 7279 2e73  ..[tool.poetry.s
-000003b0: 6372 6970 7473 5d0d 0a70 706c 6179 203d  cripts]..pplay =
-000003c0: 2022 706f 7765 7270 6c61 7965 723a 6d61   "powerplayer:ma
-000003d0: 696e 220d 0a0d 0a5b 6275 696c 642d 7379  in"....[build-sy
-000003e0: 7374 656d 5d0d 0a72 6571 7569 7265 7320  stem]..requires 
-000003f0: 3d20 5b22 706f 6574 7279 2d63 6f72 653e  = ["poetry-core>
-00000400: 3d31 2e30 2e30 225d 0d0a 6275 696c 642d  =1.0.0"]..build-
-00000410: 6261 636b 656e 6420 3d20 2270 6f65 7472  backend = "poetr
-00000420: 792e 636f 7265 2e6d 6173 6f6e 7279 2e61  y.core.masonry.a
-00000430: 7069 220d 0a                             pi"..
+00000260: 2020 2020 2020 2020 2250 726f 6772 616d          "Program
+00000270: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000280: 2050 7974 686f 6e20 3a3a 2033 2e31 3022   Python :: 3.10"
+00000290: 2c0d 0a20 2020 2020 2020 2022 4f70 6572  ,..        "Oper
+000002a0: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
+000002b0: 4f53 2049 6e64 6570 656e 6465 6e74 222c  OS Independent",
+000002c0: 0d0a 2020 2020 5d0d 0a0d 0a5b 746f 6f6c  ..    ]....[tool
+000002d0: 2e70 6f65 7472 792e 6465 7065 6e64 656e  .poetry.dependen
+000002e0: 6369 6573 5d0d 0a70 7974 686f 6e20 3d20  cies]..python = 
+000002f0: 225e 332e 3722 0d0a 636c 6963 6b20 3d20  "^3.7"..click = 
+00000300: 225e 382e 302e 3122 0d0a 636c 6963 6b2d  "^8.0.1"..click-
+00000310: 6865 6c70 2d63 6f6c 6f72 7320 3d20 225e  help-colors = "^
+00000320: 302e 392e 3122 0d0a 6273 3420 3d20 225e  0.9.1"..bs4 = "^
+00000330: 302e 302e 3122 0d0a 7265 7175 6573 7473  0.0.1"..requests
+00000340: 203d 2022 5e32 2e32 352e 3122 0d0a 706c   = "^2.25.1"..pl
+00000350: 6179 736f 756e 6420 3d20 225e 312e 322e  aysound = "^1.2.
+00000360: 3222 0d0a 7079 7468 6f6e 2d76 6c63 203d  2"..python-vlc =
+00000370: 2022 5e33 2e30 2e31 3231 3138 220d 0a79   "^3.0.12118"..y
+00000380: 6f75 7475 6265 5f64 6c20 3d20 225e 3230  outube_dl = "^20
+00000390: 3231 2e36 2e36 220d 0a79 6f75 7475 6265  21.6.6"..youtube
+000003a0: 2d73 6561 7263 6820 3d20 225e 322e 312e  -search = "^2.1.
+000003b0: 3022 0d0a 5b74 6f6f 6c2e 706f 6574 7279  0"..[tool.poetry
+000003c0: 2e64 6576 2d64 6570 656e 6465 6e63 6965  .dev-dependencie
+000003d0: 735d 0d0a 0d0a 5b74 6f6f 6c2e 706f 6574  s]....[tool.poet
+000003e0: 7279 2e73 6372 6970 7473 5d0d 0a70 706c  ry.scripts]..ppl
+000003f0: 6179 203d 2022 706f 7765 7270 6c61 7965  ay = "powerplaye
+00000400: 723a 6d61 696e 220d 0a0d 0a5b 6275 696c  r:main"....[buil
+00000410: 642d 7379 7374 656d 5d0d 0a72 6571 7569  d-system]..requi
+00000420: 7265 7320 3d20 5b22 706f 6574 7279 2d63  res = ["poetry-c
+00000430: 6f72 653e 3d31 2e30 2e30 225d 0d0a 6275  ore>=1.0.0"]..bu
+00000440: 696c 642d 6261 636b 656e 6420 3d20 2270  ild-backend = "p
+00000450: 6f65 7472 792e 636f 7265 2e6d 6173 6f6e  oetry.core.mason
+00000460: 7279 2e61 7069 220d 0a                   ry.api"..
```

### Comparing `powerplayer-0.2.0/README.md` & `powerplayer-0.2.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # Powerplayer
 https://pypi.org/project/powerplayer/
 A python based terminal music player
 Inspired by [Pauloo27](https://github.com/Pauloo27)'s [Tuner](https://github.com/Pauloo27/tuner)
 ## OS
-Tested in Windows 10(x64)
+Tested in Windows 10(x86_64)
 Should work in MAC and Linux
 ## Installation
 ### Prerequisites
 
 - VLC Media Player
 - Python ^3.7
 ### Windows
 Open the powershell and type
 ```pip install powerplayer```
+``` pip uninstall youtube_dl && pip install git+https://github.com/ytdl-org/youtube-dl.git@master#egg=youtube_dl ```                                         
 
 ### Linux/Mac
 Open the terminal and type
 ```pip3 install powerplayer```
-
+``` pip3 uninstall youtube_dl && pip3 install git+https://github.com/ytdl-org/youtube-dl.git@master#egg=youtube_dl ``` 
 ## Usage
 After installation, type `pplay` in the terminal 
 It is fine if the output is this
 ![image](https://user-images.githubusercontent.com/77975448/127959037-abe6f843-fafd-4f89-9c45-91d2bd6867b6.png)
 
 ### Then to play music from youtube, type
-```pplay playfromyt songname```
+```pplay yt songname```
 
 The output should look like this
 
 ![image](https://user-images.githubusercontent.com/77975448/125312335-cf050180-e351-11eb-9aae-2f5d20c1df9b.png)
```

### Comparing `powerplayer-0.2.0/setup.py` & `powerplayer-0.2.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 install_requires = \
 ['bs4>=0.0.1,<0.0.2',
  'click-help-colors>=0.9.1,<0.10.0',
  'click>=8.0.1,<9.0.0',
  'playsound>=1.2.2,<2.0.0',
  'python-vlc>=3.0.12118,<4.0.0',
  'requests>=2.25.1,<3.0.0',
- 'youtube-search==2.1.0',
+ 'youtube-search>=2.1.0,<3.0.0',
  'youtube_dl>=2021.6.6,<2022.0.0']
 
 entry_points = \
 {'console_scripts': ['pplay = powerplayer:main']}
 
 setup_kwargs = {
     'name': 'powerplayer',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'A command line interface to play music',
-    'long_description': "# Powerplayer\nhttps://pypi.org/project/powerplayer/\nA python based terminal music player\nInspired by [Pauloo27](https://github.com/Pauloo27)'s [Tuner](https://github.com/Pauloo27/tuner)\n## OS\nTested in Windows 10(x64)\nShould work in MAC and Linux\n## Installation\n### Prerequisites\n\n- VLC Media Player\n- Python ^3.7\n### Windows\nOpen the powershell and type\n```pip install powerplayer```\n\n### Linux/Mac\nOpen the terminal and type\n```pip3 install powerplayer```\n\n## Usage\nAfter installation, type `pplay` in the terminal \nIt is fine if the output is this\n![image](https://user-images.githubusercontent.com/77975448/127959037-abe6f843-fafd-4f89-9c45-91d2bd6867b6.png)\n\n### Then to play music from youtube, type\n```pplay playfromyt songname```\n\nThe output should look like this\n\n![image](https://user-images.githubusercontent.com/77975448/125312335-cf050180-e351-11eb-9aae-2f5d20c1df9b.png)\n",
+    'long_description': "# Powerplayer\nhttps://pypi.org/project/powerplayer/\nA python based terminal music player\nInspired by [Pauloo27](https://github.com/Pauloo27)'s [Tuner](https://github.com/Pauloo27/tuner)\n## OS\nTested in Windows 10(x86_64)\nShould work in MAC and Linux\n## Installation\n### Prerequisites\n\n- VLC Media Player\n- Python ^3.7\n### Windows\nOpen the powershell and type\n```pip install powerplayer```\n``` pip uninstall youtube_dl && pip install git+https://github.com/ytdl-org/youtube-dl.git@master#egg=youtube_dl ```                                         \n\n### Linux/Mac\nOpen the terminal and type\n```pip3 install powerplayer```\n``` pip3 uninstall youtube_dl && pip3 install git+https://github.com/ytdl-org/youtube-dl.git@master#egg=youtube_dl ``` \n## Usage\nAfter installation, type `pplay` in the terminal \nIt is fine if the output is this\n![image](https://user-images.githubusercontent.com/77975448/127959037-abe6f843-fafd-4f89-9c45-91d2bd6867b6.png)\n\n### Then to play music from youtube, type\n```pplay yt songname```\n\nThe output should look like this\n\n![image](https://user-images.githubusercontent.com/77975448/125312335-cf050180-e351-11eb-9aae-2f5d20c1df9b.png)\n",
     'author': 'Avanindra Chakraborty',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/AvanindraC/Powerplayer',
     'py_modules': modules,
     'install_requires': install_requires,
```

### Comparing `powerplayer-0.2.0/PKG-INFO` & `powerplayer-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,60 @@
 Metadata-Version: 2.1
 Name: powerplayer
-Version: 0.2.0
+Version: 0.2.1
 Summary: A command line interface to play music
 Home-page: https://github.com/AvanindraC/Powerplayer
 License: MIT
 Author: Avanindra Chakraborty
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: click (>=8.0.1,<9.0.0)
 Requires-Dist: click-help-colors (>=0.9.1,<0.10.0)
 Requires-Dist: playsound (>=1.2.2,<2.0.0)
 Requires-Dist: python-vlc (>=3.0.12118,<4.0.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
-Requires-Dist: youtube-search (==2.1.0)
+Requires-Dist: youtube-search (>=2.1.0,<3.0.0)
 Requires-Dist: youtube_dl (>=2021.6.6,<2022.0.0)
 Project-URL: Repository, https://github.com/AvanindraC/Powerplayer
 Description-Content-Type: text/markdown
 
 # Powerplayer
 https://pypi.org/project/powerplayer/
 A python based terminal music player
 Inspired by [Pauloo27](https://github.com/Pauloo27)'s [Tuner](https://github.com/Pauloo27/tuner)
 ## OS
-Tested in Windows 10(x64)
+Tested in Windows 10(x86_64)
 Should work in MAC and Linux
 ## Installation
 ### Prerequisites
 
 - VLC Media Player
 - Python ^3.7
 ### Windows
 Open the powershell and type
 ```pip install powerplayer```
+``` pip uninstall youtube_dl && pip install git+https://github.com/ytdl-org/youtube-dl.git@master#egg=youtube_dl ```                                         
 
 ### Linux/Mac
 Open the terminal and type
 ```pip3 install powerplayer```
-
+``` pip3 uninstall youtube_dl && pip3 install git+https://github.com/ytdl-org/youtube-dl.git@master#egg=youtube_dl ``` 
 ## Usage
 After installation, type `pplay` in the terminal 
 It is fine if the output is this
 ![image](https://user-images.githubusercontent.com/77975448/127959037-abe6f843-fafd-4f89-9c45-91d2bd6867b6.png)
 
 ### Then to play music from youtube, type
-```pplay playfromyt songname```
+```pplay yt songname```
 
 The output should look like this
 
 ![image](https://user-images.githubusercontent.com/77975448/125312335-cf050180-e351-11eb-9aae-2f5d20c1df9b.png)
```

