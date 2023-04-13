# Comparing `tmp/nonebot-plugin-fuckyou-0.1.0.tar.gz` & `tmp/nonebot-plugin-fuckyou-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-fuckyou-0.1.0.tar", last modified: Sun Apr  9 17:26:08 2023, max compression
+gzip compressed data, was "nonebot-plugin-fuckyou-0.1.1.tar", last modified: Thu Apr 13 16:28:47 2023, max compression
```

## Comparing `nonebot-plugin-fuckyou-0.1.0.tar` & `nonebot-plugin-fuckyou-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-04-09 17:25:59.585117 nonebot-plugin-fuckyou-0.1.0/LICENSE
--rw-r--r--   0        0        0     3802 2023-04-09 17:25:59.585117 nonebot-plugin-fuckyou-0.1.0/README.md
--rw-r--r--   0        0        0      391 2023-04-09 17:25:59.585117 nonebot-plugin-fuckyou-0.1.0/nonebot_plugin_fuckyou/__init__.py
--rw-r--r--   0        0        0     1353 2023-04-09 17:25:59.585117 nonebot-plugin-fuckyou-0.1.0/nonebot_plugin_fuckyou/__main__.py
--rw-r--r--   0        0        0      202 2023-04-09 17:25:59.585117 nonebot-plugin-fuckyou-0.1.0/nonebot_plugin_fuckyou/config.py
--rw-r--r--   0        0        0   221935 2023-04-09 17:25:59.585117 nonebot-plugin-fuckyou-0.1.0/nonebot_plugin_fuckyou/const.py
--rw-r--r--   0        0        0     1121 2023-04-09 17:25:59.585117 nonebot-plugin-fuckyou-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4141 1970-01-01 00:00:00.000000 nonebot-plugin-fuckyou-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-13 16:28:30.897175 nonebot-plugin-fuckyou-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4102 2023-04-13 16:28:30.897175 nonebot-plugin-fuckyou-0.1.1/README.md
+-rw-r--r--   0        0        0      318 2023-04-13 16:28:30.897175 nonebot-plugin-fuckyou-0.1.1/nonebot_plugin_fuckyou/__init__.py
+-rw-r--r--   0        0        0     1641 2023-04-13 16:28:30.897175 nonebot-plugin-fuckyou-0.1.1/nonebot_plugin_fuckyou/__main__.py
+-rw-r--r--   0        0        0      331 2023-04-13 16:28:30.897175 nonebot-plugin-fuckyou-0.1.1/nonebot_plugin_fuckyou/config.py
+-rw-r--r--   0        0        0   221958 2023-04-13 16:28:30.901175 nonebot-plugin-fuckyou-0.1.1/nonebot_plugin_fuckyou/const.py
+-rw-r--r--   0        0        0     1121 2023-04-13 16:28:30.901175 nonebot-plugin-fuckyou-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4441 1970-01-01 00:00:00.000000 nonebot-plugin-fuckyou-0.1.1/PKG-INFO
```

### Comparing `nonebot-plugin-fuckyou-0.1.0/LICENSE` & `nonebot-plugin-fuckyou-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-fuckyou-0.1.0/README.md` & `nonebot-plugin-fuckyou-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!-- markdownlint-disable MD031 MD033 MD036 MD041 -->
 
 <div align="center">
 
 <a href="https://v2.nonebot.dev/store">
-  <img src="https://raw.githubusercontent.com/A-kirami/nonebot-plugin-template/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo">
+  <img src="https://raw.githubusercontent.com/lgc2333/nonebot-plugin-fuckyou/master/readme/logo.png" width="180" height="180" alt="NoneBotPluginLogo">
 </a>
 
 <p>
   <img src="https://raw.githubusercontent.com/A-kirami/nonebot-plugin-template/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText">
 </p>
 
 # NoneBot-Plugin-FuckYou
@@ -101,17 +101,20 @@
 
 </details>
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的 `.env` 文件中添加下表中的必填配置
 
-|      配置项       | 必填 | 默认值  |                             说明                             |
-| :---------------: | :--: | :-----: | :----------------------------------------------------------: |
-| `FUCKYOU_VIOLENT` |  否  | `False` | **慎用**，是否开启暴力模式，开启后攻击性极强，**后果自负**！ |
+|         配置项         | 必填 | 默认值  |                          说明                          |
+| :--------------------: | :--: | :-----: | :----------------------------------------------------: |
+|    `FUCKYOU_GENTLE`    |  否  | `True`  |                    是否启用温柔词库                    |
+|   `FUCKYOU_VIOLENT`    |  否  | `False` | **慎用**，是否启用攻击性极强的暴力词库，**后果自负**！ |
+|     `FUCKYOU_TOME`     |  否  | `True`  |             是否只有 @机器人 时才会骂回去              |
+| `FUCKYOU_EXTEND_WORDS` |  否  |  `[]`   |                   要额外添加的触发词                   |
 
 ## 🎉 使用
 
 直接 @Bot 对骂即可，插件为关键词检测，触发关键词可以看看 [const.py](./nonebot_plugin_fuckyou/const.py)
 
 理论支持所有 adapter
 
@@ -138,8 +141,10 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
-芝士刚刚发布的插件，还没有更新日志的说 qwq~
+### 0.1.1
+
+- 添加几个配置项
```

#### html2text {}

```diff
@@ -13,22 +13,24 @@
 install nonebot-plugin-fuckyou ```   pdm ```bash pdm add nonebot-plugin-fuckyou
 ```   poetry ```bash poetry add nonebot-plugin-fuckyou ```   conda ```bash
 conda install nonebot-plugin-fuckyou ```  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç `plugins`
 é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
 "nonebot_plugin_fuckyou" ] ```  ## âï¸ éç½® å¨ nonebot2 é¡¹ç®ç `.env`
 æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« | é»è®¤å¼ |
-è¯´æ | | :---------------: | :--: | :-----: | :------------------------------
-----------------------------: | | `FUCKYOU_VIOLENT` | å¦ | `False` |
-**æç¨**ï¼æ¯å¦å¼å¯æ´åæ¨¡å¼ï¼å¼å¯åæ»å»æ§æå¼ºï¼**åæèªè´**ï¼
-| ## ð ä½¿ç¨ ç´æ¥ @Bot
+è¯´æ | | :--------------------: | :--: | :-----: | :-------------------------
+---------------------------: | | `FUCKYOU_GENTLE` | å¦ | `True` |
+æ¯å¦å¯ç¨æ¸©æè¯åº | | `FUCKYOU_VIOLENT` | å¦ | `False` |
+**æç¨**ï¼æ¯å¦å¯ç¨æ»å»æ§æå¼ºçæ´åè¯åºï¼**åæèªè´**ï¼ |
+| `FUCKYOU_TOME` | å¦ | `True` | æ¯å¦åªæ @æºå¨äºº æ¶æä¼éªåå» |
+| `FUCKYOU_EXTEND_WORDS` | å¦ | `[]` | è¦é¢å¤æ·»å çè§¦åè¯ | ## ð
+ä½¿ç¨ ç´æ¥ @Bot
 å¯¹éªå³å¯ï¼æä»¶ä¸ºå³é®è¯æ£æµï¼è§¦åå³é®è¯å¯ä»¥çç
 [const.py](./nonebot_plugin_fuckyou/const.py) çè®ºæ¯æææ adapter ##
 ð èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333)
 å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [`xiaoye12123/js`](https://gitee.com/xiaoye12123/
 js) - æ»å»æ§æå¼ºçåå¤è¯åºæ¥æº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿
-èå£«åååå¸çæä»¶ï¼è¿æ²¡ææ´æ°æ¥å¿çè¯´ qwq~
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.1.1 - æ·»å å ä¸ªéç½®é¡¹
```

### Comparing `nonebot-plugin-fuckyou-0.1.0/nonebot_plugin_fuckyou/__main__.py` & `nonebot-plugin-fuckyou-0.1.1/nonebot_plugin_fuckyou/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,46 @@
 import random
-from typing import List
+from typing import List, Set
 
 from nonebot import on_message
 from nonebot.internal.adapter import Event
 from nonebot.matcher import Matcher
 
 from .config import config
-from .const import GENTLE, TRIGGER_WORDS, VIOLENT
+from .const import DEFAULT_TRIGGER_WORDS, GENTLE, VIOLENT
 
 try:
     from nonebot.adapters.onebot.v11 import MessageEvent as OBV11MsgEv
     from nonebot.adapters.onebot.v12 import MessageEvent as OBV12MsgEv
 except:
     OBV11MsgEv = None
     OBV12MsgEv = None
 
 try:
     from nonebot.adapters.telegram.event import MessageEvent as TGMsgEv
 except:
     TGMsgEv = None
 
 
-phases: List[str] = VIOLENT if config.fuckyou_violent else GENTLE
+PHASES: List[str] = (GENTLE if config.fuckyou_gentle else []) + (
+    VIOLENT if config.fuckyou_violent else []
+)
+TRIGGER_WORDS: Set[str] = DEFAULT_TRIGGER_WORDS | config.fuckyou_extend_words
+
+if not PHASES:
+    raise ValueError("请至少选择一个骂人词库")
+
+
+def get_phase() -> str:
+    return random.choice(PHASES)
 
 
 # nb2 的 on_message 貌似不支持忽略大小写，自己写一个
 def trigger_rule(event: Event):
-    if not event.is_tome():
+    if config.fuckyou_tome and (not event.is_tome()):
         return False
 
     try:
         msg = event.get_plaintext().lower()
     except:
         return False
 
@@ -48,8 +58,8 @@
         OBV12MsgEv and isinstance(event, OBV12MsgEv)
     ):
         kwargs["reply_message"] = True
 
     elif TGMsgEv and isinstance(event, TGMsgEv):
         kwargs["reply_to_message_id"] = event.message_id
 
-    await matcher.finish(random.choice(phases), **kwargs)
+    await matcher.finish(get_phase(), **kwargs)
```

### Comparing `nonebot-plugin-fuckyou-0.1.0/nonebot_plugin_fuckyou/const.py` & `nonebot-plugin-fuckyou-0.1.1/nonebot_plugin_fuckyou/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from typing import List
+from typing import List, Set
 
-TRIGGER_WORDS = [
+DEFAULT_TRIGGER_WORDS: Set[str] = {
     "傻逼",
     "你妈逼",
     "日你妈",
     "草你妈",
     "操你妈",
     "cnm",
     "煞笔",
     "啥比",
     "杀币",
     "鲨臂",
     "shabi",
     "sb",
     "我是你爹",
-]
+}
 
 GENTLE: List[str] = [
     "你一个阴间的东西，就别指望着能理解咱们阳间的话",
     "我看你嘴挺能说的 能帮我暖暖脚么",
     "你出生的时候是不是被扔起来三次，被接住了两次？",
     "你不当厨师真是可惜了，添油加醋这么厉害。",
     "亮剑吧，我没的是素质，你没的是亲妈",
```

### Comparing `nonebot-plugin-fuckyou-0.1.0/pyproject.toml` & `nonebot-plugin-fuckyou-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-fuckyou"
-version = "0.1.0"
+version = "0.1.1"
 description = "A NoneBot2 plugin designed for curse users"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0-rc.1",
     "pydantic>=1.10.4",
```

### Comparing `nonebot-plugin-fuckyou-0.1.0/PKG-INFO` & `nonebot-plugin-fuckyou-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-fuckyou
-Version: 0.1.0
+Version: 0.1.1
 Summary: A NoneBot2 plugin designed for curse users
 License: MIT
 Author-email: student_2333 <lgc2333@126.com>
 Requires-Python: >=3.8,<4.0
 Provides-Extra: dev
 Project-URL: homepage, https://github.com/lgc2333/nonebot-plugin-fuckyou
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD031 MD033 MD036 MD041 -->
 
 <div align="center">
 
 <a href="https://v2.nonebot.dev/store">
-  <img src="https://raw.githubusercontent.com/A-kirami/nonebot-plugin-template/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo">
+  <img src="https://raw.githubusercontent.com/lgc2333/nonebot-plugin-fuckyou/master/readme/logo.png" width="180" height="180" alt="NoneBotPluginLogo">
 </a>
 
 <p>
   <img src="https://raw.githubusercontent.com/A-kirami/nonebot-plugin-template/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText">
 </p>
 
 # NoneBot-Plugin-FuckYou
@@ -112,17 +112,20 @@
 
 </details>
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的 `.env` 文件中添加下表中的必填配置
 
-|      配置项       | 必填 | 默认值  |                             说明                             |
-| :---------------: | :--: | :-----: | :----------------------------------------------------------: |
-| `FUCKYOU_VIOLENT` |  否  | `False` | **慎用**，是否开启暴力模式，开启后攻击性极强，**后果自负**！ |
+|         配置项         | 必填 | 默认值  |                          说明                          |
+| :--------------------: | :--: | :-----: | :----------------------------------------------------: |
+|    `FUCKYOU_GENTLE`    |  否  | `True`  |                    是否启用温柔词库                    |
+|   `FUCKYOU_VIOLENT`    |  否  | `False` | **慎用**，是否启用攻击性极强的暴力词库，**后果自负**！ |
+|     `FUCKYOU_TOME`     |  否  | `True`  |             是否只有 @机器人 时才会骂回去              |
+| `FUCKYOU_EXTEND_WORDS` |  否  |  `[]`   |                   要额外添加的触发词                   |
 
 ## 🎉 使用
 
 直接 @Bot 对骂即可，插件为关键词检测，触发关键词可以看看 [const.py](./nonebot_plugin_fuckyou/const.py)
 
 理论支持所有 adapter
 
@@ -149,9 +152,11 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
-芝士刚刚发布的插件，还没有更新日志的说 qwq~
+### 0.1.1
+
+- 添加几个配置项
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-fuckyou Version: 0.1.0 Summary: A
+Metadata-Version: 2.1 Name: nonebot-plugin-fuckyou Version: 0.1.1 Summary: A
 NoneBot2 plugin designed for curse users License: MIT Author-email:
 student_2333
 126.com> Requires-Python: >=3.8,<4.0 Provides-Extra: dev Project-URL: homepage,
 https://github.com/lgc2333/nonebot-plugin-fuckyou Description-Content-Type:
 text/markdown
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
@@ -19,22 +19,24 @@
 install nonebot-plugin-fuckyou ```   pdm ```bash pdm add nonebot-plugin-fuckyou
 ```   poetry ```bash poetry add nonebot-plugin-fuckyou ```   conda ```bash
 conda install nonebot-plugin-fuckyou ```  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç `plugins`
 é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
 "nonebot_plugin_fuckyou" ] ```  ## âï¸ éç½® å¨ nonebot2 é¡¹ç®ç `.env`
 æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« | é»è®¤å¼ |
-è¯´æ | | :---------------: | :--: | :-----: | :------------------------------
-----------------------------: | | `FUCKYOU_VIOLENT` | å¦ | `False` |
-**æç¨**ï¼æ¯å¦å¼å¯æ´åæ¨¡å¼ï¼å¼å¯åæ»å»æ§æå¼ºï¼**åæèªè´**ï¼
-| ## ð ä½¿ç¨ ç´æ¥ @Bot
+è¯´æ | | :--------------------: | :--: | :-----: | :-------------------------
+---------------------------: | | `FUCKYOU_GENTLE` | å¦ | `True` |
+æ¯å¦å¯ç¨æ¸©æè¯åº | | `FUCKYOU_VIOLENT` | å¦ | `False` |
+**æç¨**ï¼æ¯å¦å¯ç¨æ»å»æ§æå¼ºçæ´åè¯åºï¼**åæèªè´**ï¼ |
+| `FUCKYOU_TOME` | å¦ | `True` | æ¯å¦åªæ @æºå¨äºº æ¶æä¼éªåå» |
+| `FUCKYOU_EXTEND_WORDS` | å¦ | `[]` | è¦é¢å¤æ·»å çè§¦åè¯ | ## ð
+ä½¿ç¨ ç´æ¥ @Bot
 å¯¹éªå³å¯ï¼æä»¶ä¸ºå³é®è¯æ£æµï¼è§¦åå³é®è¯å¯ä»¥çç
 [const.py](./nonebot_plugin_fuckyou/const.py) çè®ºæ¯æææ adapter ##
 ð èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333)
 å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [`xiaoye12123/js`](https://gitee.com/xiaoye12123/
 js) - æ»å»æ§æå¼ºçåå¤è¯åºæ¥æº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿
-èå£«åååå¸çæä»¶ï¼è¿æ²¡ææ´æ°æ¥å¿çè¯´ qwq~
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.1.1 - æ·»å å ä¸ªéç½®é¡¹
```

