# Comparing `tmp/nonebot_plugin_quote-0.3.4.tar.gz` & `tmp/nonebot_plugin_quote-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_quote-0.3.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_quote-0.3.5.tar", max compression
```

## Comparing `nonebot_plugin_quote-0.3.4.tar` & `nonebot_plugin_quote-0.3.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     8041 2023-04-02 10:31:07.469032 nonebot_plugin_quote-0.3.4/README.md
--rw-r--r--   0        0        0    18550 2023-04-02 10:31:00.756762 nonebot_plugin_quote-0.3.4/nonebot_plugin_quote/__init__.py
--rw-r--r--   0        0        0      347 2023-03-29 02:55:51.708604 nonebot_plugin_quote-0.3.4/nonebot_plugin_quote/config.py
--rw-r--r--   0        0        0     7034 2023-04-02 06:00:36.006127 nonebot_plugin_quote-0.3.4/nonebot_plugin_quote/task.py
--rw-r--r--   0        0        0      458 2023-04-02 10:31:55.094773 nonebot_plugin_quote-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     8732 1970-01-01 00:00:00.000000 nonebot_plugin_quote-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     8125 2023-04-13 18:56:53.411208 nonebot_plugin_quote-0.3.5/README.md
+-rw-r--r--   0        0        0    18635 2023-04-13 18:50:34.390259 nonebot_plugin_quote-0.3.5/nonebot_plugin_quote/__init__.py
+-rw-r--r--   0        0        0      347 2023-03-29 02:55:51.708604 nonebot_plugin_quote-0.3.5/nonebot_plugin_quote/config.py
+-rw-r--r--   0        0        0     7034 2023-04-02 06:00:36.006127 nonebot_plugin_quote-0.3.5/nonebot_plugin_quote/task.py
+-rw-r--r--   0        0        0      458 2023-04-13 19:06:42.419410 nonebot_plugin_quote-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     8816 1970-01-01 00:00:00.000000 nonebot_plugin_quote-0.3.5/PKG-INFO
```

### Comparing `nonebot_plugin_quote-0.3.4/README.md` & `nonebot_plugin_quote-0.3.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,18 +28,20 @@
 一款适用于QQ群聊天的语录库插件。
 
 - [x] 上传聊天截图
 - [x] 随机投放聊天语录
 - [x] 根据关键词投放聊天语录 
 - [x] 支持白名单内用户删除语录
 - [x] 支持为指定语录增删标签
-- [x] [批量上传已有聊天截图(测试功能)](https://github.com/RongRongJi/nonebot_plugin_quote/blob/main/batch_upload.md)
+- [x] [批量处理已有聊天截图(测试功能)](https://github.com/RongRongJi/nonebot_plugin_quote/blob/main/batch.md)
 
 你的star是对我最好的支持！
 
+交流QQ群: 580407499
+
 ## 🎉 使用
 
 ### 上传
 
 @机器人，发送**上传**指令，开启上传通道。
 
 以图片的形式发送聊天语录，即可将语录上传至语录库中。
@@ -212,24 +214,25 @@
 
 ### v0.3.0 (2023/3/28)
 
 - 新增标签功能，包括针对一条语录【新增标签】、【删除标签】、【查看全部标签】
 - 增加了初始文件的默认路径，不再需要用户手动创建文件
 - IO统一为UTF-8
 
-### v0.3.1 (2023/3/28)
-
-- 适配了一个不同版本reply格式不同的问题
-
 ### v0.3.2 (2023/3/29)
 
 - 增加了是否需要at机器人的选项
 - 增加了指令前缀
 
 ### v0.3.4 (2023/4/2)
 
 - 增加批量上传语录功能（试验版）
 
+### v0.3.5 (2023/4/14)
+
+- 修改了匹配策略，使不同协议下的消息格式都可以匹配
+- 增加批量备份语录功能（试验版）
+
 ## 🎉 鸣谢
 
 - [NoneBot2](https://github.com/nonebot/nonebot2)：本插件使用的开发框架。
 - [go-cqhttp](https://github.com/Mrs4s/go-cqhttp)：稳定完善的 CQHTTP 实现。
```

#### html2text {}

```diff
@@ -2,18 +2,18 @@
                               [NoneBotPluginText]
            # nonebot-plugin-quote _â¨ QQç¾¤è è¯­å½åº â¨_ ð§¬
 æ¯æOCRè¯å«ï¼å³é®è¯æç´¢ | ä¸èµ·è®°å½ç¾¤åçéå¤©è¨è®ºå§ï¼ð
                       [license] [Python] [NoneBot] [pypi]
 ## ð ä»ç» ä¸æ¬¾éç¨äºQQç¾¤èå¤©çè¯­å½åºæä»¶ã - [x]
 ä¸ä¼ èå¤©æªå¾ - [x] éæºææ¾èå¤©è¯­å½ - [x]
 æ ¹æ®å³é®è¯ææ¾èå¤©è¯­å½ - [x] æ¯æç½åååç¨æ·å é¤è¯­å½ -
-[x] æ¯æä¸ºæå®è¯­å½å¢å æ ç­¾ - [x] [æ¹éä¸ä¼ å·²æèå¤©æªå¾
+[x] æ¯æä¸ºæå®è¯­å½å¢å æ ç­¾ - [x] [æ¹éå¤çå·²æèå¤©æªå¾
 (æµè¯åè½)](https://github.com/RongRongJi/nonebot_plugin_quote/blob/main/
-batch_upload.md) ä½ çstaræ¯å¯¹ææå¥½çæ¯æï¼ ## ð ä½¿ç¨ ###
-ä¸ä¼  @æºå¨äººï¼åé**ä¸ä¼ **æä»¤ï¼å¼å¯ä¸ä¼ ééã
+batch.md) ä½ çstaræ¯å¯¹ææå¥½çæ¯æï¼ äº¤æµQQç¾¤: 580407499 ## ð
+ä½¿ç¨ ### ä¸ä¼  @æºå¨äººï¼åé**ä¸ä¼ **æä»¤ï¼å¼å¯ä¸ä¼ ééã
 ä»¥å¾ççå½¢å¼åéèå¤©è¯­å½ï¼å³å¯å°è¯­å½ä¸ä¼ è³è¯­å½åºä¸­ã
 [https://github.com/RongRongJi/nonebot_plugin_quote/raw/main/screenshot/
 upload.jpg] ç´æ¥åå¤**ç»æ**ï¼å³å¯ç»æ­¢ä¸ä¼ ééã ###
 éæºåéè¯­å½
 @æºå¨äººï¼åé**è¯­å½**æä»¤ï¼æºå¨äººå°ä»è¯­å½åºä¸­éæºæéä¸æ¡è¯­å½åéã
 [https://github.com/RongRongJi/nonebot_plugin_quote/raw/main/screenshot/
 random.jpg] ### å³é®è¯æ£ç´¢è¯­å½
@@ -83,14 +83,15 @@
 -
 å¢å äºå¨å±ç®¡çåçè®¾ç½®ï¼å¨å±ç®¡çåæ¥æå é¤æ¯ä¸ªç¾¤è¯­å½åºçæé
 - ä¿®å¤äºä¸ä¸ªå³äºä¸ä¼ åç¼åä¸å¹éçbug ### v0.2.3 (2023/3/22) -
 å¨OCRè¯å«æå­åå¢å äºæ¢è¡é¿æå­ä¸ä¸åæå­æ®µçè¯å«ï¼ä½¿åè¯æ´å åç¡®
 ### v0.3.0 (2023/3/28) -
 æ°å¢æ ç­¾åè½ï¼åæ¬éå¯¹ä¸æ¡è¯­å½ãæ°å¢æ ç­¾ãããå é¤æ ç­¾ãããæ¥çå¨é¨æ ç­¾ã
 - å¢å äºåå§æä»¶çé»è®¤è·¯å¾ï¼ä¸åéè¦ç¨æ·æå¨åå»ºæä»¶ -
-IOç»ä¸ä¸ºUTF-8 ### v0.3.1 (2023/3/28) -
-ééäºä¸ä¸ªä¸åçæ¬replyæ ¼å¼ä¸åçé®é¢ ### v0.3.2 (2023/3/29) -
+IOç»ä¸ä¸ºUTF-8 ### v0.3.2 (2023/3/29) -
 å¢å äºæ¯å¦éè¦atæºå¨äººçéé¡¹ - å¢å äºæä»¤åç¼ ### v0.3.4
-(2023/4/2) - å¢å æ¹éä¸ä¼ è¯­å½åè½ï¼è¯éªçï¼ ## ð é¸£è°¢ -
-[NoneBot2](https://github.com/nonebot/
-nonebot2)ï¼æ¬æä»¶ä½¿ç¨çå¼åæ¡æ¶ã - [go-cqhttp](https://github.com/
-Mrs4s/go-cqhttp)ï¼ç¨³å®å®åç CQHTTP å®ç°ã
+(2023/4/2) - å¢å æ¹éä¸ä¼ è¯­å½åè½ï¼è¯éªçï¼ ### v0.3.5 (2023/4/
+14) - ä¿®æ¹äºå¹éç­ç¥ï¼ä½¿ä¸ååè®®ä¸çæ¶æ¯æ ¼å¼é½å¯ä»¥å¹é
+- å¢å æ¹éå¤ä»½è¯­å½åè½ï¼è¯éªçï¼ ## ð é¸£è°¢ - [NoneBot2]
+(https://github.com/nonebot/nonebot2)ï¼æ¬æä»¶ä½¿ç¨çå¼åæ¡æ¶ã -
+[go-cqhttp](https://github.com/Mrs4s/go-cqhttp)ï¼ç¨³å®å®åç CQHTTP
+å®ç°ã
```

### Comparing `nonebot_plugin_quote-0.3.4/nonebot_plugin_quote/__init__.py` & `nonebot_plugin_quote-0.3.5/nonebot_plugin_quote/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,20 +9,22 @@
 import re
 import json
 import base64
 import random
 import subprocess
 import sys
 import os
+import shutil
 from .task import offer, query, delete, handle_ocr_text, inverted2forward, findAlltag, addTag, delTag
 from .task import copy_images_files
 from .config import Config
 from nonebot.log import logger
 import time
 
+# v0.3.5
 
 plugin_config = Config.parse_obj(get_driver().config)
 
 need_at = {}
 if plugin_config.quote_needat:
     need_at['rule'] = to_me()
 
@@ -44,15 +46,61 @@
 
     with open(plugin_config.inverted_index_path, 'w', encoding='UTF-8') as fc:
         json.dump(inverted_index, fc, indent=2, separators=(',',': '), ensure_ascii=False)
     logger.warning('已创建json文件')
 
 
 forward_index = inverted2forward(inverted_index)
-# reply_index = {}
+
+
+# 回复信息处理
+async def reply_handle(bot, errMsg, raw_message, groupNum, user_id, listener):
+
+    # print(raw_message)
+    if 'reply' not in raw_message:
+        await bot.call_api('send_group_msg', **{
+            'group_id':int(groupNum),
+            'message': '[CQ:at,qq='+user_id+']' + errMsg
+        })
+        await listener.finish()
+    
+    # reply之后第一个等号，到数字后第一个非数字
+    idx = raw_message.find('reply')
+    reply_id = ''
+    for i in range(idx, len(raw_message)):
+        if raw_message[i] == '=':
+            idx = i
+            break
+    for i in range(idx+1, len(raw_message)):
+        if raw_message[i] != '-' and not raw_message[i].isdigit():
+            break
+        reply_id += raw_message[i]
+
+    # print(reply_id)
+
+    resp = await bot.get_msg(message_id=reply_id)
+
+    img_msg = str(resp['message'])
+    # print(img_msg)
+
+    if '.image' not in img_msg:
+        await bot.call_api('send_group_msg', **{
+            'group_id':int(groupNum),
+            'message': '[CQ:at,qq='+user_id+']' + errMsg
+        })
+        await listener.finish()
+    
+    idx = img_msg.find('.image')
+    img = '.image'
+    for i in range(0,32):
+        img = img_msg[idx-i-1] + img
+    
+    # print(img)
+    return img
+
 
 
  # 语录库
 record = on_command("{}上传".format(plugin_config.quote_startcmd), priority=10, block=True, rule=to_me())
 end_conversation = ['stop', '结束', '上传截图', '结束上传']
 
 
@@ -227,42 +275,18 @@
                 'message': '[CQ:at,qq='+user_id+'] 非常抱歉, 您没有删除权限TUT'
             })
             await delete_record.finish()
 
     raw_message = str(event)
 
     errMsg = '请回复需要删除的语录, 并输入删除指令'
-
-    rt = r"\[reply:id=(.*?)]"
-    ids = re.findall(rt, str(raw_message))
-
-    if len(ids) == 0:
-        await bot.call_api('send_group_msg', **{
-            'group_id':int(groupNum),
-            'message': '[CQ:at,qq='+user_id+']' + errMsg
-        })
-        await delete_record.finish()
-
-    rlyid = ids[0].split(",")[0]
-    resp = await bot.get_msg(message_id=rlyid)
-
-    img_msg = str(resp['message'])
-
-    rt = r"\[CQ:image,file=(.*?),subType=[\S]*,url=[\S]*\]"
-    imgs = re.findall(rt, img_msg)
-
-    if len(imgs) == 0:
-        await bot.call_api('send_group_msg', **{
-            'group_id':int(groupNum),
-            'message': '[CQ:at,qq='+user_id+']' + errMsg
-        })
-        await delete_record.finish()
+    imgs = await reply_handle(bot, errMsg, raw_message, groupNum, user_id, delete_record)
     
     # 搜索
-    is_Delete, record_dict, inverted_index, forward_index = delete(imgs[0], groupNum, record_dict, inverted_index, forward_index)
+    is_Delete, record_dict, inverted_index, forward_index = delete(imgs, groupNum, record_dict, inverted_index, forward_index)
 
     if is_Delete:
         with open(plugin_config.record_path, 'w', encoding='UTF-8') as f:
             json.dump(record_dict, f, indent=2, separators=(',', ': '), ensure_ascii=False)
         with open(plugin_config.inverted_index_path, 'w', encoding='UTF-8') as fc:
             json.dump(inverted_index, fc, indent=2, separators=(',',': '), ensure_ascii=False)
         msg = '删除成功'
@@ -294,41 +318,17 @@
     if 'group' not in session_id:
         await alltag.finish()
 
     groupNum = session_id.split('_')[1]
     raw_message = str(event)
 
     errMsg = '请回复需要指定语录'
+    imgs = await reply_handle(bot, errMsg, raw_message, groupNum, user_id, alltag)
 
-    rt = r"\[reply:id=(.*?)]"
-    ids = re.findall(rt, str(raw_message))
-
-    if len(ids) == 0:
-        await bot.call_api('send_group_msg', **{
-            'group_id':int(groupNum),
-            'message': '[CQ:at,qq='+user_id+']' + errMsg
-        })
-        await alltag.finish()
-
-    rlyid = ids[0].split(",")[0]
-    resp = await bot.get_msg(message_id=rlyid)
-
-    img_msg = str(resp['message'])
-
-    rt = r"\[CQ:image,file=(.*?),subType=[\S]*,url=[\S]*\]"
-    imgs = re.findall(rt, img_msg)
-
-    if len(imgs) == 0:
-        await bot.call_api('send_group_msg', **{
-            'group_id':int(groupNum),
-            'message': '[CQ:at,qq='+user_id+']' + errMsg
-        })
-        await alltag.finish()
-
-    tags = findAlltag(imgs[0], forward_index, groupNum)
+    tags = findAlltag(imgs, forward_index, groupNum)
     if tags is None:
         msg = '该语录不存在'
     else:
         msg = '该语录的所有Tag为: '
         for tag in tags:
             msg += tag + ' '
 
@@ -356,42 +356,17 @@
     if 'group' not in session_id:
         await addtag.finish()
 
     groupNum = session_id.split('_')[1]
     raw_message = str(event)
 
     errMsg = '请回复需要指定语录'
+    imgs = await reply_handle(bot, errMsg, raw_message, groupNum, user_id, addtag)
 
-    rt = r"\[reply:id=(.*?)]"
-    ids = re.findall(rt, str(raw_message))
-
-    if len(ids) == 0:
-        await bot.call_api('send_group_msg', **{
-            'group_id':int(groupNum),
-            'message': '[CQ:at,qq='+user_id+']' + errMsg
-        })
-        await addtag.finish()
-
-    rlyid = ids[0].split(",")[0]
-    resp = await bot.get_msg(message_id=rlyid)
-
-    img_msg = str(resp['message'])
-
-    rt = r"\[CQ:image,file=(.*?),subType=[\S]*,url=[\S]*\]"
-    imgs = re.findall(rt, img_msg)
-
-    if len(imgs) == 0:
-        await bot.call_api('send_group_msg', **{
-            'group_id':int(groupNum),
-            'message': '[CQ:at,qq='+user_id+']' + errMsg
-        })
-        await addtag.finish()
-
-
-    flag, forward_index, inverted_index = addTag(tags, imgs[0], groupNum, forward_index, inverted_index)
+    flag, forward_index, inverted_index = addTag(tags, imgs, groupNum, forward_index, inverted_index)
     with open(plugin_config.inverted_index_path, 'w', encoding='UTF-8') as fc:
         json.dump(inverted_index, fc, indent=2, separators=(',',': '), ensure_ascii=False)
 
     if flag is None:
         msg = '该语录不存在'
     else:
         msg = '已为该语录添加上{}标签'.format(tags)
@@ -420,42 +395,17 @@
     if 'group' not in session_id:
         await addtag.finish()
 
     groupNum = session_id.split('_')[1]
     raw_message = str(event)
 
     errMsg = '请回复需要指定语录'
+    imgs = await reply_handle(bot, errMsg, raw_message, groupNum, user_id, deltag)
 
-    rt = r"\[reply:id=(.*?)]"
-    ids = re.findall(rt, str(raw_message))
-
-    if len(ids) == 0:
-        await bot.call_api('send_group_msg', **{
-            'group_id':int(groupNum),
-            'message': '[CQ:at,qq='+user_id+']' + errMsg
-        })
-        await deltag.finish()
-
-    rlyid = ids[0].split(",")[0]
-    resp = await bot.get_msg(message_id=rlyid)
-
-    img_msg = str(resp['message'])
-
-    rt = r"\[CQ:image,file=(.*?),subType=[\S]*,url=[\S]*\]"
-    imgs = re.findall(rt, img_msg)
-
-    if len(imgs) == 0:
-        await bot.call_api('send_group_msg', **{
-            'group_id':int(groupNum),
-            'message': '[CQ:at,qq='+user_id+']' + errMsg
-        })
-        await deltag.finish()
-
-
-    flag, forward_index, inverted_index = delTag(tags, imgs[0], groupNum, forward_index, inverted_index)
+    flag, forward_index, inverted_index = delTag(tags, imgs, groupNum, forward_index, inverted_index)
     with open(plugin_config.inverted_index_path, 'w', encoding='UTF-8') as fc:
         json.dump(inverted_index, fc, indent=2, separators=(',',': '), ensure_ascii=False)
 
     if flag is None:
         msg = '该语录不存在'
     else:
         msg = '已移除该语录的{}标签'.format(tags)
@@ -464,15 +414,14 @@
         'group_id':int(groupNum),
         'message': '[CQ:at,qq='+user_id+']' + msg
     })
 
     await deltag.finish()
 
 
-# script_batch = on_command('{}脚本123'.format(plugin_config.quote_startcmd), **need_at)
 script_batch = on_regex(pattern="^{}batch_upload".format(plugin_config.quote_startcmd), **need_at)
 
 @script_batch.handle()
 async def script_batch_handle(bot: Bot, event: Event, state: T_State):
 
     global inverted_index
     global record_dict
@@ -496,24 +445,27 @@
 
     raw_msg = str(event.get_message())
     raw_msg = raw_msg.replace('\r','')
     group_id = re.findall(rqqid, raw_msg)
     your_path = re.findall(ryour_path, raw_msg)
     gocq_path = re.findall(rgocq_path, raw_msg)
     tags = re.findall(rtags, raw_msg)
+    # print(group_id, your_path, gocq_path, tags)
     instruction = '''指令如下:
 batch_upload
 qqgroup=123456
 your_path=/home/xxx/images
 gocq_path=/home/xxx/gocq/data/cache
 tags=aaa bbb ccc'''
     if len(group_id) == 0 or len(your_path) == 0 or len(gocq_path) == 0:
         await script_batch.finish(instruction)
     # 获取图片
+    # image_files = copy_images_files('/home/sr/project/data','/home/sr/newgocq/data/cache')
     image_files = copy_images_files(your_path[0], gocq_path[0])
+    # print(image_files)
 
     total_len = len(image_files)
     idx = 0
 
     for (imgid, img) in image_files:
         save_file = '../cache/' + img
         idx += 1
@@ -522,15 +474,15 @@
         if group_id[0] in forward_index and save_file in forward_index[group_id[0]]:
             await bot.send_msg(group_id=int(groupNum), message='上述图片已存在')
             continue
         try:
             ocr = await bot.ocr_image(image=imgid)
             ocr_content = handle_ocr_text(ocr['texts'])
         except exception.ActionFailed:
-            await bot.send_msg(group_id=int(groupNum), message='该图片ocr失败, 请单独上传')
+            await bot.send_msg(group_id=int(groupNum), message='该图片ocr失败')
             continue
         
         time.sleep(1)
         inverted_index, forward_index = offer(group_id[0], save_file, ocr_content, inverted_index, forward_index)
         if group_id[0] not in record_dict:
             record_dict[group_id[0]] = [save_file]
         else:
@@ -555,7 +507,49 @@
         json.dump(record_dict, f, indent=2, separators=(',', ': '), ensure_ascii=False)
 
     with open(plugin_config.inverted_index_path, 'w', encoding='UTF-8') as fc:
         json.dump(inverted_index, fc, indent=2, separators=(',',': '), ensure_ascii=False)
 
     await bot.send_msg(group_id=int(groupNum), message='批量导入完成')
     await script_batch.finish()
+
+
+
+copy_batch = on_regex(pattern="^{}batch_copy".format(plugin_config.quote_startcmd), **need_at)
+
+@copy_batch.handle()
+async def copy_batch_handle(bot: Bot, event: Event, state: T_State):
+
+    session_id = event.get_session_id()
+    user_id = str(event.get_user_id())
+
+    # 必须是超级管理员群聊
+    if user_id not in plugin_config.global_superuser:
+        await copy_batch.finish()
+
+
+    ryour_path =  r"your_path=(.*)\s"
+    rgocq_path =  r"gocq_path=(.*)"
+
+    raw_msg = str(event.get_message())
+    raw_msg = raw_msg.replace('\r','')
+    your_path = re.findall(ryour_path, raw_msg)
+    gocq_path = re.findall(rgocq_path, raw_msg)
+    # print(your_path, gocq_path)
+    instruction = '''指令如下:
+batch_copy
+your_path=/home/xxx/images
+gocq_path=/home/xxx/gocq/data/cache'''
+    if len(your_path) == 0 or len(gocq_path) == 0:
+        await copy_batch.finish(instruction)
+
+    global record_dict
+
+    try:
+        for value in record_dict.values():
+            for img in value:
+                num = len(img) - 8
+                name = img[-num:]
+                shutil.copyfile(gocq_path[0] + name, your_path[0] + name)
+    except FileNotFoundError:
+        await copy_batch.finish("路径不正确")
+    await copy_batch.finish("备份完成")
```

### Comparing `nonebot_plugin_quote-0.3.4/nonebot_plugin_quote/task.py` & `nonebot_plugin_quote-0.3.5/nonebot_plugin_quote/task.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_quote-0.3.4/PKG-INFO` & `nonebot_plugin_quote-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-quote
-Version: 0.3.4
+Version: 0.3.5
 Summary: 一款适用于QQ群聊天的语录库插件
 License: MIT
 Author: RongRongJi
 Author-email: 316315867@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -47,18 +47,20 @@
 一款适用于QQ群聊天的语录库插件。
 
 - [x] 上传聊天截图
 - [x] 随机投放聊天语录
 - [x] 根据关键词投放聊天语录 
 - [x] 支持白名单内用户删除语录
 - [x] 支持为指定语录增删标签
-- [x] [批量上传已有聊天截图(测试功能)](https://github.com/RongRongJi/nonebot_plugin_quote/blob/main/batch_upload.md)
+- [x] [批量处理已有聊天截图(测试功能)](https://github.com/RongRongJi/nonebot_plugin_quote/blob/main/batch.md)
 
 你的star是对我最好的支持！
 
+交流QQ群: 580407499
+
 ## 🎉 使用
 
 ### 上传
 
 @机器人，发送**上传**指令，开启上传通道。
 
 以图片的形式发送聊天语录，即可将语录上传至语录库中。
@@ -231,24 +233,25 @@
 
 ### v0.3.0 (2023/3/28)
 
 - 新增标签功能，包括针对一条语录【新增标签】、【删除标签】、【查看全部标签】
 - 增加了初始文件的默认路径，不再需要用户手动创建文件
 - IO统一为UTF-8
 
-### v0.3.1 (2023/3/28)
-
-- 适配了一个不同版本reply格式不同的问题
-
 ### v0.3.2 (2023/3/29)
 
 - 增加了是否需要at机器人的选项
 - 增加了指令前缀
 
 ### v0.3.4 (2023/4/2)
 
 - 增加批量上传语录功能（试验版）
 
+### v0.3.5 (2023/4/14)
+
+- 修改了匹配策略，使不同协议下的消息格式都可以匹配
+- 增加批量备份语录功能（试验版）
+
 ## 🎉 鸣谢
 
 - [NoneBot2](https://github.com/nonebot/nonebot2)：本插件使用的开发框架。
 - [go-cqhttp](https://github.com/Mrs4s/go-cqhttp)：稳定完善的 CQHTTP 实现。
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-quote Version: 0.3.4 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-quote Version: 0.3.5 Summary:
 ä¸æ¬¾éç¨äºQQç¾¤èå¤©çè¯­å½åºæä»¶ License: MIT Author: RongRongJi
 Author-email: 316315867@qq.com Requires-Python: >=3.8,<4.0 Classifier: License
 :: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: jieba
 (>=0.42.1,<0.43.0) Requires-Dist: nonebot-adapter-onebot (>=2.2.1,<3.0.0)
@@ -12,18 +12,18 @@
                               [NoneBotPluginText]
            # nonebot-plugin-quote _â¨ QQç¾¤è è¯­å½åº â¨_ ð§¬
 æ¯æOCRè¯å«ï¼å³é®è¯æç´¢ | ä¸èµ·è®°å½ç¾¤åçéå¤©è¨è®ºå§ï¼ð
                       [license] [Python] [NoneBot] [pypi]
 ## ð ä»ç» ä¸æ¬¾éç¨äºQQç¾¤èå¤©çè¯­å½åºæä»¶ã - [x]
 ä¸ä¼ èå¤©æªå¾ - [x] éæºææ¾èå¤©è¯­å½ - [x]
 æ ¹æ®å³é®è¯ææ¾èå¤©è¯­å½ - [x] æ¯æç½åååç¨æ·å é¤è¯­å½ -
-[x] æ¯æä¸ºæå®è¯­å½å¢å æ ç­¾ - [x] [æ¹éä¸ä¼ å·²æèå¤©æªå¾
+[x] æ¯æä¸ºæå®è¯­å½å¢å æ ç­¾ - [x] [æ¹éå¤çå·²æèå¤©æªå¾
 (æµè¯åè½)](https://github.com/RongRongJi/nonebot_plugin_quote/blob/main/
-batch_upload.md) ä½ çstaræ¯å¯¹ææå¥½çæ¯æï¼ ## ð ä½¿ç¨ ###
-ä¸ä¼  @æºå¨äººï¼åé**ä¸ä¼ **æä»¤ï¼å¼å¯ä¸ä¼ ééã
+batch.md) ä½ çstaræ¯å¯¹ææå¥½çæ¯æï¼ äº¤æµQQç¾¤: 580407499 ## ð
+ä½¿ç¨ ### ä¸ä¼  @æºå¨äººï¼åé**ä¸ä¼ **æä»¤ï¼å¼å¯ä¸ä¼ ééã
 ä»¥å¾ççå½¢å¼åéèå¤©è¯­å½ï¼å³å¯å°è¯­å½ä¸ä¼ è³è¯­å½åºä¸­ã
 [https://github.com/RongRongJi/nonebot_plugin_quote/raw/main/screenshot/
 upload.jpg] ç´æ¥åå¤**ç»æ**ï¼å³å¯ç»æ­¢ä¸ä¼ ééã ###
 éæºåéè¯­å½
 @æºå¨äººï¼åé**è¯­å½**æä»¤ï¼æºå¨äººå°ä»è¯­å½åºä¸­éæºæéä¸æ¡è¯­å½åéã
 [https://github.com/RongRongJi/nonebot_plugin_quote/raw/main/screenshot/
 random.jpg] ### å³é®è¯æ£ç´¢è¯­å½
@@ -93,14 +93,15 @@
 -
 å¢å äºå¨å±ç®¡çåçè®¾ç½®ï¼å¨å±ç®¡çåæ¥æå é¤æ¯ä¸ªç¾¤è¯­å½åºçæé
 - ä¿®å¤äºä¸ä¸ªå³äºä¸ä¼ åç¼åä¸å¹éçbug ### v0.2.3 (2023/3/22) -
 å¨OCRè¯å«æå­åå¢å äºæ¢è¡é¿æå­ä¸ä¸åæå­æ®µçè¯å«ï¼ä½¿åè¯æ´å åç¡®
 ### v0.3.0 (2023/3/28) -
 æ°å¢æ ç­¾åè½ï¼åæ¬éå¯¹ä¸æ¡è¯­å½ãæ°å¢æ ç­¾ãããå é¤æ ç­¾ãããæ¥çå¨é¨æ ç­¾ã
 - å¢å äºåå§æä»¶çé»è®¤è·¯å¾ï¼ä¸åéè¦ç¨æ·æå¨åå»ºæä»¶ -
-IOç»ä¸ä¸ºUTF-8 ### v0.3.1 (2023/3/28) -
-ééäºä¸ä¸ªä¸åçæ¬replyæ ¼å¼ä¸åçé®é¢ ### v0.3.2 (2023/3/29) -
+IOç»ä¸ä¸ºUTF-8 ### v0.3.2 (2023/3/29) -
 å¢å äºæ¯å¦éè¦atæºå¨äººçéé¡¹ - å¢å äºæä»¤åç¼ ### v0.3.4
-(2023/4/2) - å¢å æ¹éä¸ä¼ è¯­å½åè½ï¼è¯éªçï¼ ## ð é¸£è°¢ -
-[NoneBot2](https://github.com/nonebot/
-nonebot2)ï¼æ¬æä»¶ä½¿ç¨çå¼åæ¡æ¶ã - [go-cqhttp](https://github.com/
-Mrs4s/go-cqhttp)ï¼ç¨³å®å®åç CQHTTP å®ç°ã
+(2023/4/2) - å¢å æ¹éä¸ä¼ è¯­å½åè½ï¼è¯éªçï¼ ### v0.3.5 (2023/4/
+14) - ä¿®æ¹äºå¹éç­ç¥ï¼ä½¿ä¸ååè®®ä¸çæ¶æ¯æ ¼å¼é½å¯ä»¥å¹é
+- å¢å æ¹éå¤ä»½è¯­å½åè½ï¼è¯éªçï¼ ## ð é¸£è°¢ - [NoneBot2]
+(https://github.com/nonebot/nonebot2)ï¼æ¬æä»¶ä½¿ç¨çå¼åæ¡æ¶ã -
+[go-cqhttp](https://github.com/Mrs4s/go-cqhttp)ï¼ç¨³å®å®åç CQHTTP
+å®ç°ã
```

