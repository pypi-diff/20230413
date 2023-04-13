# Comparing `tmp/nonebot_plugin_wordle-0.2.0.tar.gz` & `tmp/nonebot_plugin_wordle-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_wordle-0.2.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_wordle-0.2.1.tar", max compression
```

## Comparing `nonebot_plugin_wordle-0.2.0.tar` & `nonebot_plugin_wordle-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     1063 2023-01-28 08:24:34.341909 nonebot_plugin_wordle-0.2.0/LICENSE
--rw-r--r--   0        0        0     1302 2023-01-28 08:24:34.341909 nonebot_plugin_wordle-0.2.0/README.md
--rw-r--r--   0        0        0     9035 2023-01-28 08:24:34.341909 nonebot_plugin_wordle-0.2.0/nonebot_plugin_wordle/__init__.py
--rw-r--r--   0        0        0     5584 2023-01-28 08:24:34.341909 nonebot_plugin_wordle-0.2.0/nonebot_plugin_wordle/data_source.py
--rw-r--r--   0        0        0   139252 2023-01-28 08:24:34.345909 nonebot_plugin_wordle-0.2.0/nonebot_plugin_wordle/resources/fonts/KarnakPro-Bold.ttf
--rw-r--r--   0        0        0   695923 2023-01-28 08:24:34.349909 nonebot_plugin_wordle-0.2.0/nonebot_plugin_wordle/resources/words/CET4.json
--rw-r--r--   0        0        0   443930 2023-01-28 08:24:34.349909 nonebot_plugin_wordle-0.2.0/nonebot_plugin_wordle/resources/words/CET6.json
--rw-r--r--   0        0        0   480469 2023-01-28 08:24:34.353909 nonebot_plugin_wordle-0.2.0/nonebot_plugin_wordle/resources/words/GMAT.json
--rw-r--r--   0        0        0  1021713 2023-01-28 08:24:34.361909 nonebot_plugin_wordle-0.2.0/nonebot_plugin_wordle/resources/words/GRE.json
--rw-r--r--   0        0        0   521446 2023-01-28 08:24:34.365909 nonebot_plugin_wordle-0.2.0/nonebot_plugin_wordle/resources/words/IELTS.json
--rw-r--r--   0        0        0   637594 2023-01-28 08:24:34.369909 nonebot_plugin_wordle-0.2.0/nonebot_plugin_wordle/resources/words/SAT.json
--rw-r--r--   0        0        0  1252663 2023-01-28 08:24:34.377909 nonebot_plugin_wordle-0.2.0/nonebot_plugin_wordle/resources/words/TOEFL.json
--rw-r--r--   0        0        0  1750255 2023-01-28 08:24:34.385909 nonebot_plugin_wordle-0.2.0/nonebot_plugin_wordle/resources/words/专八.json
--rw-r--r--   0        0        0   620016 2023-01-28 08:24:34.389909 nonebot_plugin_wordle-0.2.0/nonebot_plugin_wordle/resources/words/专四.json
--rw-r--r--   0        0        0   675299 2023-01-28 08:24:34.393909 nonebot_plugin_wordle-0.2.0/nonebot_plugin_wordle/resources/words/考研.json
--rw-r--r--   0        0        0     1192 2023-01-28 08:24:34.393909 nonebot_plugin_wordle-0.2.0/nonebot_plugin_wordle/utils.py
--rw-r--r--   0        0        0      650 2023-01-28 08:24:34.397909 nonebot_plugin_wordle-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2232 1970-01-01 00:00:00.000000 nonebot_plugin_wordle-0.2.0/setup.py
--rw-r--r--   0        0        0     2174 1970-01-01 00:00:00.000000 nonebot_plugin_wordle-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-13 04:13:04.996661 nonebot_plugin_wordle-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1302 2023-04-13 04:13:04.996661 nonebot_plugin_wordle-0.2.1/README.md
+-rw-r--r--   0        0        0     9033 2023-04-13 04:13:04.996661 nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/__init__.py
+-rw-r--r--   0        0        0     5997 2023-04-13 04:13:04.996661 nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/data_source.py
+-rw-r--r--   0        0        0   139252 2023-04-13 04:13:05.000661 nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/fonts/KarnakPro-Bold.ttf
+-rw-r--r--   0        0        0   695923 2023-04-13 04:13:05.004661 nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/CET4.json
+-rw-r--r--   0        0        0   443930 2023-04-13 04:13:05.008662 nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/CET6.json
+-rw-r--r--   0        0        0   480469 2023-04-13 04:13:05.008662 nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/GMAT.json
+-rw-r--r--   0        0        0  1021713 2023-04-13 04:13:05.016662 nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/GRE.json
+-rw-r--r--   0        0        0   521446 2023-04-13 04:13:05.016662 nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/IELTS.json
+-rw-r--r--   0        0        0   637594 2023-04-13 04:13:05.020662 nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/SAT.json
+-rw-r--r--   0        0        0  1252663 2023-04-13 04:13:05.028663 nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/TOEFL.json
+-rw-r--r--   0        0        0  1750255 2023-04-13 04:13:05.036663 nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/专八.json
+-rw-r--r--   0        0        0   620016 2023-04-13 04:13:05.040663 nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/专四.json
+-rw-r--r--   0        0        0   675299 2023-04-13 04:13:05.044663 nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/考研.json
+-rw-r--r--   0        0        0     1193 2023-04-13 04:13:05.044663 nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/utils.py
+-rw-r--r--   0        0        0      650 2023-04-13 04:13:05.044663 nonebot_plugin_wordle-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2174 1970-01-01 00:00:00.000000 nonebot_plugin_wordle-0.2.1/PKG-INFO
```

### Comparing `nonebot_plugin_wordle-0.2.0/LICENSE` & `nonebot_plugin_wordle-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordle-0.2.0/README.md` & `nonebot_plugin_wordle-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordle-0.2.0/nonebot_plugin_wordle/__init__.py` & `nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,44 +1,42 @@
+import asyncio
 import re
 import shlex
-import asyncio
-from io import BytesIO
 from asyncio import TimerHandle
 from dataclasses import dataclass
-from typing import Dict, List, Optional, NoReturn, Union
+from io import BytesIO
+from typing import Dict, List, NoReturn, Optional, Union
 
-from nonebot.typing import T_State
-from nonebot.matcher import Matcher
+from nonebot import on_command, on_message, on_shell_command
+from nonebot.adapters.onebot.v11 import Bot as V11Bot
+from nonebot.adapters.onebot.v11 import GroupMessageEvent as V11GMEvent
+from nonebot.adapters.onebot.v11 import Message as V11Msg
+from nonebot.adapters.onebot.v11 import MessageEvent as V11MEvent
+from nonebot.adapters.onebot.v11 import MessageSegment as V11MsgSeg
+from nonebot.adapters.onebot.v12 import Bot as V12Bot
+from nonebot.adapters.onebot.v12 import ChannelMessageEvent as V12CMEvent
+from nonebot.adapters.onebot.v12 import GroupMessageEvent as V12GMEvent
+from nonebot.adapters.onebot.v12 import Message as V12Msg
+from nonebot.adapters.onebot.v12 import MessageEvent as V12MEvent
+from nonebot.adapters.onebot.v12 import MessageSegment as V12MsgSeg
 from nonebot.exception import ParserExit
-from nonebot.plugin import PluginMetadata
-from nonebot.rule import Rule, ArgumentParser
-from nonebot import on_command, on_shell_command, on_message
+from nonebot.matcher import Matcher
 from nonebot.params import (
-    ShellCommandArgv,
     CommandArg,
     CommandStart,
     EventPlainText,
     EventToMe,
+    ShellCommandArgv,
 )
+from nonebot.plugin import PluginMetadata
+from nonebot.rule import ArgumentParser, Rule
+from nonebot.typing import T_State
 
-from nonebot.adapters.onebot.v11 import Bot as V11Bot
-from nonebot.adapters.onebot.v11 import Message as V11Msg
-from nonebot.adapters.onebot.v11 import MessageSegment as V11MsgSeg
-from nonebot.adapters.onebot.v11 import MessageEvent as V11MEvent
-from nonebot.adapters.onebot.v11 import GroupMessageEvent as V11GMEvent
-
-from nonebot.adapters.onebot.v12 import Bot as V12Bot
-from nonebot.adapters.onebot.v12 import Message as V12Msg
-from nonebot.adapters.onebot.v12 import MessageSegment as V12MsgSeg
-from nonebot.adapters.onebot.v12 import MessageEvent as V12MEvent
-from nonebot.adapters.onebot.v12 import GroupMessageEvent as V12GMEvent
-from nonebot.adapters.onebot.v12 import ChannelMessageEvent as V12CMEvent
-
+from .data_source import GuessResult, Wordle
 from .utils import dic_list, random_word
-from .data_source import Wordle, GuessResult
 
 __plugin_meta__ = PluginMetadata(
     name="猜单词",
     description="wordle猜单词游戏",
     usage=(
         "@我 + “猜单词”开始游戏；\n"
         "答案为指定长度单词，发送对应长度单词即可；\n"
@@ -51,15 +49,15 @@
         "可使用 -d/--dic 指定词典，默认为CET4\n"
         f"支持的词典：{'、'.join(dic_list)}"
     ),
     extra={
         "unique_name": "wordle",
         "example": "@小Q 猜单词\nwordle -l 6 -d CET6",
         "author": "meetwq <meetwq@gmail.com>",
-        "version": "0.2.0",
+        "version": "0.2.1",
     },
 )
 
 
 parser = ArgumentParser("wordle", description="猜单词")
 parser.add_argument("-l", "--length", type=int, default=5, help="单词长度")
 parser.add_argument("-d", "--dic", default="CET4", help="词典")
```

### Comparing `nonebot_plugin_wordle-0.2.0/nonebot_plugin_wordle/data_source.py` & `nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/data_source.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from enum import Enum
 from io import BytesIO
+from typing import List, Optional, Tuple
+
 from PIL import Image, ImageDraw
 from PIL.Image import Image as IMG
-from typing import Tuple, List, Optional
 
 from .utils import legal_word, load_font, save_png
 
 
 class GuessResult(Enum):
     WIN = 0  # 猜出正确单词
     LOSS = 1  # 达到最大可猜次数，未猜出正确单词
@@ -69,42 +70,52 @@
         board_w = self.length * self.block_size[0]
         board_w += (self.length - 1) * self.block_padding[0] + 2 * self.padding[0]
         board_h = self.rows * self.block_size[1]
         board_h += (self.rows - 1) * self.block_padding[1] + 2 * self.padding[1]
         board_size = (board_w, board_h)
         board = Image.new("RGB", board_size, self.bg_color)
 
-        for i in range(self.rows):
-            word_temp = self.word_lower  # 临时变量
-            for j in range(self.length):
-                letter = self.guessed_words[i][j] if len(self.guessed_words) > i else ""
-                if letter:
-                    if letter == self.word_lower[j]:
-                        color = self.correct_color
+        for row in range(self.rows):
+            if row < len(self.guessed_words):
+                guessed_word = self.guessed_words[row]
+
+                word_incorrect = ""  # 猜错的字母
+                for i in range(self.length):
+                    if guessed_word[i] != self.word_lower[i]:
+                        word_incorrect += self.word_lower[i]
+                    else:
+                        word_incorrect += "_"  # 猜对的字母用下划线代替
 
-                    elif (
-                        letter in word_temp
-                        and self.guessed_words[i][word_temp.find(letter)] != letter
-                    ):
+                blocks: List[IMG] = []
+                for i in range(self.length):
+                    letter = guessed_word[i]
+                    if letter == self.word_lower[i]:
+                        color = self.correct_color
+                    elif letter in word_incorrect:
                         """
                         一个字母的黄色和绿色数量与答案中的数量保持一致
                         以输入apple，答案adapt为例
                         结果为apple的第一个p是黄色，第二个p是灰色
                         代表答案中只有一个p，且不在第二个位置
                         """
-                        word_temp = word_temp.replace(letter, "_", 1)
+                        word_incorrect = word_incorrect.replace(letter, "_", 1)
                         color = self.exist_color
                     else:
                         color = self.wrong_color
-                else:
-                    color = self.bg_color
+                    blocks.append(self.draw_block(color, letter))
 
-                x = self.padding[0] + (self.block_size[0] + self.block_padding[0]) * j
-                y = self.padding[1] + (self.block_size[1] + self.block_padding[1]) * i
-                board.paste(self.draw_block(color, letter), (x, y))
+            else:
+                blocks = [
+                    self.draw_block(self.bg_color, "") for _ in range(self.length)
+                ]
+
+            for col, block in enumerate(blocks):
+                x = self.padding[0] + (self.block_size[0] + self.block_padding[0]) * col
+                y = self.padding[1] + (self.block_size[1] + self.block_padding[1]) * row
+                board.paste(block, (x, y))
         return save_png(board)
 
     def get_hint(self) -> str:
         letters = set()
         for word in self.guessed_words:
             for letter in word:
                 if letter in self.word_lower:
```

### Comparing `nonebot_plugin_wordle-0.2.0/nonebot_plugin_wordle/resources/fonts/KarnakPro-Bold.ttf` & `nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/fonts/KarnakPro-Bold.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordle-0.2.0/nonebot_plugin_wordle/resources/words/CET4.json` & `nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/CET4.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordle-0.2.0/nonebot_plugin_wordle/resources/words/CET6.json` & `nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/CET6.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordle-0.2.0/nonebot_plugin_wordle/resources/words/GMAT.json` & `nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/GMAT.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordle-0.2.0/nonebot_plugin_wordle/resources/words/GRE.json` & `nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/GRE.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordle-0.2.0/nonebot_plugin_wordle/resources/words/IELTS.json` & `nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/IELTS.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordle-0.2.0/nonebot_plugin_wordle/resources/words/SAT.json` & `nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/SAT.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordle-0.2.0/nonebot_plugin_wordle/resources/words/TOEFL.json` & `nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/TOEFL.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordle-0.2.0/nonebot_plugin_wordle/resources/words/专八.json` & `nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/专八.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordle-0.2.0/nonebot_plugin_wordle/resources/words/专四.json` & `nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/专四.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordle-0.2.0/nonebot_plugin_wordle/resources/words/考研.json` & `nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/resources/words/考研.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordle-0.2.0/nonebot_plugin_wordle/utils.py` & `nonebot_plugin_wordle-0.2.1/nonebot_plugin_wordle/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import random
 from io import BytesIO
 from pathlib import Path
 from typing import Tuple
+
 from PIL import ImageFont
 from PIL.Image import Image as IMG
 from PIL.ImageFont import FreeTypeFont
 from spellchecker import SpellChecker
 
 data_dir = Path(__file__).parent / "resources"
 fonts_dir = data_dir / "fonts"
```

### Comparing `nonebot_plugin_wordle-0.2.0/pyproject.toml` & `nonebot_plugin_wordle-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_wordle"
-version = "0.2.0"
+version = "0.2.1"
 description = "Nonebot2 wordle猜单词插件"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noneplugin/nonebot-plugin-wordle"
 repository = "https://github.com/noneplugin/nonebot-plugin-wordle"
```

### Comparing `nonebot_plugin_wordle-0.2.0/PKG-INFO` & `nonebot_plugin_wordle-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-wordle
-Version: 0.2.0
+Version: 0.2.1
 Summary: Nonebot2 wordle猜单词插件
 Home-page: https://github.com/noneplugin/nonebot-plugin-wordle
 License: MIT
 Author: meetwq
 Author-email: meetwq@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

