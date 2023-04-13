# Comparing `tmp/projectZ.py-1.1.6.6.tar.gz` & `tmp/projectZ.py-1.1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "projectZ.py-1.1.6.6.tar", last modified: Sat Apr  1 12:07:10 2023, max compression
+gzip compressed data, was "projectZ.py-1.1.6.7.tar", last modified: Thu Apr 13 17:38:51 2023, max compression
```

## Comparing `projectZ.py-1.1.6.6.tar` & `projectZ.py-1.1.6.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-01 12:07:10.300581 projectZ.py-1.1.6.6/
--rw-rw-rw-   0        0        0     2779 2023-04-01 12:07:10.300581 projectZ.py-1.1.6.6/PKG-INFO
--rw-rw-rw-   0        0        0     1777 2023-03-16 22:32:28.000000 projectZ.py-1.1.6.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-01 12:07:10.253584 projectZ.py-1.1.6.6/projectZ/
--rw-rw-rw-   0        0        0      748 2023-04-01 11:52:04.000000 projectZ.py-1.1.6.6/projectZ/__init__.py
--rw-rw-rw-   0        0        0    27230 2023-04-01 11:31:58.000000 projectZ.py-1.1.6.6/projectZ/async_client.py
--rw-rw-rw-   0        0        0     8701 2023-04-01 12:06:41.000000 projectZ.py-1.1.6.6/projectZ/async_socket.py
--rw-rw-rw-   0        0        0    25969 2023-03-29 17:12:25.000000 projectZ.py-1.1.6.6/projectZ/client.py
--rw-rw-rw-   0        0        0     9048 2023-04-01 11:50:15.000000 projectZ.py-1.1.6.6/projectZ/socket.py
-drwxrwxrwx   0        0        0        0 2023-04-01 12:07:10.299588 projectZ.py-1.1.6.6/projectZ/utils/
--rw-rw-rw-   0        0        0        0 2023-02-06 18:57:12.000000 projectZ.py-1.1.6.6/projectZ/utils/__init__.py
--rw-rw-rw-   0        0        0     1724 2023-04-01 11:47:12.000000 projectZ.py-1.1.6.6/projectZ/utils/exceptions.py
--rw-rw-rw-   0        0        0     2674 2023-03-17 11:05:21.000000 projectZ.py-1.1.6.6/projectZ/utils/generator.py
--rw-rw-rw-   0        0        0      985 2023-02-18 18:34:23.000000 projectZ.py-1.1.6.6/projectZ/utils/headers.py
--rw-rw-rw-   0        0        0    21006 2023-03-25 23:39:28.000000 projectZ.py-1.1.6.6/projectZ/utils/objects.py
-drwxrwxrwx   0        0        0        0 2023-04-01 12:07:10.283590 projectZ.py-1.1.6.6/projectZ.py.egg-info/
--rw-rw-rw-   0        0        0     2779 2023-04-01 12:07:08.000000 projectZ.py-1.1.6.6/projectZ.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      447 2023-04-01 12:07:08.000000 projectZ.py-1.1.6.6/projectZ.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-01 12:07:08.000000 projectZ.py-1.1.6.6/projectZ.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-04-01 12:07:08.000000 projectZ.py-1.1.6.6/projectZ.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-01 12:07:08.000000 projectZ.py-1.1.6.6/projectZ.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-01 12:07:10.302582 projectZ.py-1.1.6.6/setup.cfg
--rw-rw-rw-   0        0        0      857 2023-04-01 12:06:10.000000 projectZ.py-1.1.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:38:51.877354 projectZ.py-1.1.6.7/
+-rw-rw-rw-   0        0        0     2779 2023-04-13 17:38:51.878355 projectZ.py-1.1.6.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1777 2023-03-16 22:32:28.000000 projectZ.py-1.1.6.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 17:38:51.833728 projectZ.py-1.1.6.7/projectZ/
+-rw-rw-rw-   0        0        0      748 2023-04-13 17:36:05.000000 projectZ.py-1.1.6.7/projectZ/__init__.py
+-rw-rw-rw-   0        0        0    32362 2023-04-13 17:24:01.000000 projectZ.py-1.1.6.7/projectZ/async_client.py
+-rw-rw-rw-   0        0        0     8713 2023-04-01 11:49:21.000000 projectZ.py-1.1.6.7/projectZ/async_socket.py
+-rw-rw-rw-   0        0        0    28645 2023-04-13 17:30:53.000000 projectZ.py-1.1.6.7/projectZ/client.py
+-rw-rw-rw-   0        0        0     9048 2023-04-10 10:03:57.000000 projectZ.py-1.1.6.7/projectZ/socket.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:38:51.876354 projectZ.py-1.1.6.7/projectZ/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-06 18:57:12.000000 projectZ.py-1.1.6.7/projectZ/utils/__init__.py
+-rw-rw-rw-   0        0        0     1724 2023-04-01 11:47:12.000000 projectZ.py-1.1.6.7/projectZ/utils/exceptions.py
+-rw-rw-rw-   0        0        0     2674 2023-03-17 11:05:21.000000 projectZ.py-1.1.6.7/projectZ/utils/generator.py
+-rw-rw-rw-   0        0        0      985 2023-02-18 18:34:23.000000 projectZ.py-1.1.6.7/projectZ/utils/headers.py
+-rw-rw-rw-   0        0        0    21006 2023-03-25 23:39:28.000000 projectZ.py-1.1.6.7/projectZ/utils/objects.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:38:51.861721 projectZ.py-1.1.6.7/projectZ.py.egg-info/
+-rw-rw-rw-   0        0        0     2779 2023-04-13 17:38:50.000000 projectZ.py-1.1.6.7/projectZ.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      447 2023-04-13 17:38:51.000000 projectZ.py-1.1.6.7/projectZ.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 17:38:50.000000 projectZ.py-1.1.6.7/projectZ.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-04-13 17:38:50.000000 projectZ.py-1.1.6.7/projectZ.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-13 17:38:50.000000 projectZ.py-1.1.6.7/projectZ.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 17:38:51.879355 projectZ.py-1.1.6.7/setup.cfg
+-rw-rw-rw-   0        0        0      857 2023-04-13 17:37:26.000000 projectZ.py-1.1.6.7/setup.py
```

### Comparing `projectZ.py-1.1.6.6/PKG-INFO` & `projectZ.py-1.1.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projectZ.py
-Version: 1.1.6.6
+Version: 1.1.6.7
 Summary: Library for creating projectZ bots and scripts.
 Home-page: https://github.com/xXxCLOTIxXx/projectZ.py
 Author: Xsarz
 Author-email: xsarzy@gmail.com
 License: MIT
 Download-URL: https://github.com/xXxCLOTIxXx/projectZ.py/archive/refs/heads/main.zip
 Description: <table align="center">
```

### Comparing `projectZ.py-1.1.6.6/README.md` & `projectZ.py-1.1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `projectZ.py-1.1.6.6/projectZ/__init__.py` & `projectZ.py-1.1.6.7/projectZ/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,14 @@
 from json import loads
 from requests import get
 
 __title__ = 'projectZ.py'
 __author__ = 'Xsarz'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Xsarz'
-__version__ = '1.1.6.6'
+__version__ = '1.1.6.7'
 
 
 __newest__ = loads(get("https://pypi.org/pypi/projectZ.py/json").text)["info"]["version"]
 if __version__ != __newest__:
 	s('cls || clear')
 	print(f'\033[38;5;214m{__title__} made by {__author__}\nPlease update the library. Your version: {__version__}  A new version:{__newest__}\033[0m')
```

### Comparing `projectZ.py-1.1.6.6/projectZ/async_client.py` & `projectZ.py-1.1.6.7/projectZ/async_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -129,37 +129,55 @@
 
 		data = dumps({"link": link})
 		endpoint = f"/v1/links/path"
 		async with self.session.post(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint, data=data), data=data) as response:
 			return exceptions.CheckException(await response.text()) if response.status != 200 else objects.FromLink(loads(await response.text()))
 
 
-	async def get_link(self, userId: int):
+	async def get_link(self, userId: int = None, chatId: int = None, circleId: int = None, blogId: int = None):
 
-		data = dumps({
+		data = {
 			"objectId": 0,
 			"objectType": 0,
 			"parentId": 0,
-			"path": f"user/{userId}",
 			"circleIdForCircleAnnouncement": 0,
 			"parentType": 0
-		})
+		}
+
+		if userId:
+			data["path"] = f"user/{userId}"
+
+		elif chatId:
+			data["path"] = f"chat/{chatId}"
+
+		elif circleId:
+			data["objectType"] = 5
+			data["objectId"] = circleId
+			data["path"] = f"circle/{circleId}"
+
+		elif blogId:
+			data["path"] = f"blog/{blogId}"
+
+		else:
+			raise exceptions.WrongType(fileType)
+
+		data = dumps(data)
 
 		endpoint = '/v1/links/share'
 		async with self.session.post(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint, data=data), data=data) as response:
 			return exceptions.CheckException(await response.text()) if response.status != 200 else objects.FromLink(loads(await response.text()))
 
 	async def get_my_chats(self, start: int = 0, size: int = 20, type: str = 'managed'):
 
 		endpoint = f'/v1/chat/joined-threads?start={start}&size={size}&type={type}'
 		async with self.session.get(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint)) as response:
 			return exceptions.CheckException(await response.text()) if response.status != 200 else  objects.Thread(loads(await response.text()))
 
 
-	async def send_message(self, chatId: int, message: str = None, file: AsyncBufferedReader = None, fileType: str = None, file_duration: int = None, message_type: int = 1, reply_to: int = None, poll_id: int = None, dice_id: int = None): 
+	async def send_message(self, chatId: int, message: str = None, file: AsyncBufferedReader = None, fileType: str = None, file_duration: int = None, message_type: int = 1, replyTo: int = None, pollId: int = None, diceId: int = None): 
 		data = {
 			"threadId": chatId,
 			"uid": self.profile.uid,
 			"seqId": randint(0, maxsize),
 			"extensions": {}
 		}
 		if message:
@@ -167,17 +185,17 @@
 			data["type"]=message_type
 		elif file:
 			data["type"]= 2 if fileType == "image" else 6
 			data["media"] = await self.upload_media(file=file, fileType=fileType, target= 8 if fileType == "image" else 10, returnType='dict', duration=file_duration*1000 if file_duration else 0)
 		else:
 			raise exceptions.WrongType('Specify the "message" or "file" argument')
 
-		if reply_to: data["extensions"]["replyMessage"] = reply_to
-		if poll_id: data["extensions"]["pollId"] = poll_id
-		if dice_id: data["extensions"]["diceId"] = dice_id
+		if replyTo: data["extensions"]["replyMessageId"] = replyTo
+		if pollId: data["extensions"]["pollId"] = pollId
+		if diceId: data["extensions"]["diceId"] = diceId
 
 		resp = await self.send(t=1, data=data, threadId=chatId)
 		return resp
 
 
 
 	async def send_verify_code(self, email: str, country_code: str = None):
@@ -579,15 +597,137 @@
 	async def get_circles_members(self, circleId: int, size: int = 30, type :str = 'normal', pageToken: str = None):
 
 		endpoint = f'/v1/circles/{circleId}/members?type={type}&size={size}&isExcludeManger=false{f"&pageToken={pageToken}" if pageToken else ""}'
 		async with self.session.get(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint)) as response:
 			return exceptions.CheckException(await response.text()) if response.status != 200 else objects.CirclesMembers(loads(await response.text()))
 
 
-	async def add_to_favorites(self, userId: Union[list, int]):
 
-		userIds = userId if isinstance(userId, list) else [userId]
-		data = dumps({"targetUids": userIds})
-		endpoint = '/v1/users/membership/favorites'
+	async def get_baners(self):
+
+		endpoint = '/v2/banners'
+		async with self.session.get(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint)) as response:
+			return exceptions.CheckException(await response.text()) if response.status != 200 else objects.Baners(loads(await response.text()))
+
+
+	async def activate_wallet(self, wallet_password: str, code: str, email: str = None):
+
+		data = dumps({
+			"authType": 1,
+			"identity": email if email else self.profile.email if self.profile.email else exceptions.NotLoggined('You are not authorized'),
+			"paymentPassword": wallet_password,
+			"securityCode": code
+		})
+
+		endpoint = '/biz/v1/wallet/0/activate'
 		async with self.session.post(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint, data=data), data=data) as response:
 			return exceptions.CheckException(await response.text()) if response.status != 200 else response.status
 
+	async def activate_shop(self):
+
+		endpoint = '/biz/v1/activate-store'
+		async with self.session.post(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint)) as response:
+			return exceptions.CheckException(await response.text()) if response.status != 200 else objects.ActivateShop(loads(await response.text()))
+
+	async def wallet_info(self):
+
+		endpoint = '/biz/v1/wallet'
+		async with self.session.get(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint)) as response:
+			return exceptions.CheckException(await response.text()) if response.status != 200 else objects.WalletInfo(loads(await response.text()))
+
+
+	async def my_nfts(self):
+
+		endpoint = '/biz/v1/nfts/count'
+		async with self.session.get(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint)) as response:
+			return exceptions.CheckException(await response.text()) if response.status != 200 else objects.Nfts(loads(await response.text()))
+
+
+
+	async def comment(self, message: str, userId: int = None, blogId: int = None, replyId: dict = None):
+
+		data = {
+			"commentId": 0,
+			"status":1,
+			"parentId": userId,
+			"replyId": 0,
+			"circleId": 0,
+			"uid": 0,
+			"content": message,
+			"mediaList": [],
+			"commentType": 1,
+			"subComments": [],
+			"subCommentsCount": 0,
+			"isPinned": False
+		}
+
+		if userId:
+			data['parentType'] = 4
+
+		elif blogId:
+			data['parentType'] = 2
+
+		else:
+			raise exceptions.WrongType()
+
+
+		if replyId:
+			data['replyId'] = replyId['commentId']
+			data['extensions'] = {"replyToUid": replyId['userId'], "contentStatus": 1}
+
+		data = dumps(data)
+		endpoint = f'/v1/comments'
+		async with self.session.post(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint, data=data), data=data) as response:
+			return exceptions.CheckException(await response.text()) if response.status != 200 else objects.Comments(loads(await response.text()))
+
+
+
+	async def get_alerts(groupId: int = 3, size: int = 30):
+
+		endpoint = f"/v1/alerts?groupId={groupId}&size={size}"
+		async with self.session.get(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint)) as response:
+			return exceptions.CheckException(await response.text()) if response.status != 200 else loads(await response.text())
+
+	async def get_moods(self):
+		endpoint = f"/v1/moods"
+		async with self.session.get(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint)) as response:
+			return exceptions.CheckException(await response.text()) if response.status != 200 else loads(await response.text())
+
+
+
+	async def change_password(self, oldPassword: str, newPassword: str):
+
+		data = dumps({"oldPassword": oldPassword, "newPassword": newPassword})
+		endpoint="/v1/auth/change-password"
+		async with self.session.post(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint, data=data), data=data) as response:
+			return exceptions.CheckException(await response.text()) if response.status != 200 else response.status
+
+
+	async def get_message_info(self, chatId: int, messageId: int):
+
+		endpoint = f"/v1/chat/threads/{chatId}/messages/{messageId}"
+		async with self.session.get(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint)) as response:
+			return exceptions.CheckException(await response.text()) if response.status != 200 else loads(await response.text())
+
+
+	async def delete_chat(self, chatId: int):
+
+		endpoint = f"/v1/chat/threads/{chatId}"
+		async with self.session.delete(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint)) as response:
+			return exceptions.CheckException(await response.text()) if response.status != 200 else response.status
+
+
+	async def qivotes_chat(self, chatId: int):
+
+		data = dumps({
+			"uid": 0,
+			"objectId": {chatId},
+			"objectType": 1,
+			"timezone": self.time_zone,
+			"votedCount": 1,
+			"votedDate": 0,
+			"createdTime": 0,
+			"lastVoteTime": 0
+		})
+		endpoint = "/v1/qivotes"
+		async with self.session.post(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint, data=data), data=data) as response:
+			return exceptions.CheckException(await response.text()) if response.status != 200 else loads(await response.text())
```

### Comparing `projectZ.py-1.1.6.6/projectZ/async_socket.py` & `projectZ.py-1.1.6.7/projectZ/async_socket.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from aiohttp import ClientSession, WSMsgType
-from .utils import objects
+from .utils import objects, exceptions
 from asyncio import create_task, sleep
 from json import dumps, loads
 from traceback import format_exc
 
 
 class AsyncSocket:
 	def __init__(self, headers, debug: bool = False):
```

### Comparing `projectZ.py-1.1.6.6/projectZ/client.py` & `projectZ.py-1.1.6.7/projectZ/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,50 +101,70 @@
 	def get_from_link(self, link: str):
 		data = dumps({"link": link})
 
 		endpoint = f"/v1/links/path"
 		response = self.session.post(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint, data=data), data=data, proxies=self.proxies)
 		return exceptions.CheckException(response.text) if response.status_code != 200 else objects.FromLink(loads(response.text))
 
-	def get_link(self, userId: int):
 
-		data = dumps({
+
+	def get_link(self, userId: int = None, chatId: int = None, circleId: int = None, blogId: int = None):
+
+		data = {
 			"objectId": 0,
 			"objectType": 0,
 			"parentId": 0,
-			"path": f"user/{userId}",
 			"circleIdForCircleAnnouncement": 0,
 			"parentType": 0
-		})
+		}
+
+		if userId:
+			data["path"] = f"user/{userId}"
+
+		elif chatId:
+			data["path"] = f"chat/{chatId}"
+
+		elif circleId:
+			data["objectType"] = 5
+			data["objectId"] = circleId
+			data["path"] = f"circle/{circleId}"
+
+		elif blogId:
+			data["path"] = f"blog/{blogId}"
+
+		else:
+			raise exceptions.WrongType(fileType)
+
+		data = dumps(data)
 
 		endpoint = '/v1/links/share'
 		response = self.session.post(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint, data=data), data=data, proxies=self.proxies)
 		return exceptions.CheckException(response.text) if response.status_code != 200 else objects.FromLink(loads(response.text))
 
 	def get_my_chats(self, start: int = 0, size: int = 20, type: str = 'managed'):
 
 		endpoint = f'/v1/chat/joined-threads?start={start}&size={size}&type={type}'
 		response = self.session.get(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint), proxies=self.proxies)
 		return exceptions.CheckException(response.text) if response.status_code != 200 else objects.Thread(loads(response.text))
 
 
-	def send_message(self, chatId: int, message: str, message_type: int = 1, reply_to: int = None, poll_id: int = None, dice_id: int = None):
+	def send_message(self, chatId: int, message: str, message_type: int = 1, replyTo: int = None, pollId: int = None, diceId: int = None):
 
 		data = {
 			"type": message_type,
 			"threadId": chatId,
 			"uid": self.profile.uid,
 			"seqId": randint(0, maxsize),
 			"extensions": {}
 		}
 		data["content"] = message
 
-		if reply_to: data["extensions"]["replyMessage"] = reply_to
-		if poll_id: data["extensions"]["pollId"] = poll_id
-		if dice_id: data["extensions"]["diceId"] = dice_id
+		if replyTo: data["extensions"]["replyMessageId"] = replyTo
+		if pollId: data["extensions"]["pollId"] = pollId
+		if diceId: data["extensions"]["diceId"] = diceId
 
 		resp = self.send(t=1, data=data, threadId=chatId)
 		return resp
 
 	def send_verify_code(self, email: str, country_code: str = None):
 
 		data = dumps({
@@ -575,8 +595,60 @@
 
 
 	def online_chat_status(self, chatId: int, online: bool = True):
 
 		data = dumps({"partyOnlineStatus": 1 if online else 2})
 		endpoint = f"/v1/chat/threads/{chatId}/party-online-status"
 		response = self.session.post(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint, data=data), data=data, proxies=self.proxies)
-		return exceptions.CheckException(response.text) if response.status_code != 200 else loads(response.text)
+		return exceptions.CheckException(response.text) if response.status_code != 200 else loads(response.text)
+
+
+	def get_alerts(groupId: int = 3, size: int = 30):
+
+		endpoint = f"/v1/alerts?groupId={groupId}&size={size}"
+		response = self.session.get(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint), proxies=self.proxies)
+		return exceptions.CheckException(response.text) if response.status_code != 200 else loads(response.text)
+
+	def get_moods(self):
+		endpoint = f"/v1/moods"
+		response = self.session.get(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint), proxies=self.proxies)
+		return exceptions.CheckException(response.text) if response.status_code != 200 else loads(response.text)
+
+
+
+	def change_password(self, oldPassword: str, newPassword: str):
+
+		data = dumps({"oldPassword": oldPassword, "newPassword": newPassword})
+		endpoint="/v1/auth/change-password"
+		response = self.session.post(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint, data=data), data=data, proxies=self.proxies)
+		return exceptions.CheckException(response.text) if response.status_code != 200 else response.status_code
+
+
+
+	def get_message_info(self, chatId: int, messageId: int):
+
+		endpoint = f"/v1/chat/threads/{chatId}/messages/{messageId}"
+		response = self.session.get(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint), proxies=self.proxies)
+		return exceptions.CheckException(response.text) if response.status_code != 200 else loads(response.text)
+
+
+	def delete_chat(self, chatId: int):
+
+		endpoint = f"/v1/chat/threads/{chatId}"
+		response = self.session.delete(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint), proxies=self.proxies)
+		return exceptions.CheckException(response.text) if response.status_code != 200 else response.status_code
+
+	def qivotes_chat(self, chatId: int):
+
+		data = dumps({
+			"uid": 0,
+			"objectId": chatId,
+			"objectType": 1,
+			"timezone": self.time_zone,
+			"votedCount": 1,
+			"votedDate": 0,
+			"createdTime": 0,
+			"lastVoteTime": 0
+		})
+		endpoint = "/v1/qivotes"
+		response = self.session.post(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint, data=data), data=data, proxies=self.proxies)
+		return exceptions.CheckException(response.text) if response.status_code != 200 else loads(response.text)
```

### Comparing `projectZ.py-1.1.6.6/projectZ/socket.py` & `projectZ.py-1.1.6.7/projectZ/socket.py`

 * *Files identical despite different names*

### Comparing `projectZ.py-1.1.6.6/projectZ/utils/exceptions.py` & `projectZ.py-1.1.6.7/projectZ/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `projectZ.py-1.1.6.6/projectZ/utils/generator.py` & `projectZ.py-1.1.6.7/projectZ/utils/generator.py`

 * *Files identical despite different names*

### Comparing `projectZ.py-1.1.6.6/projectZ/utils/headers.py` & `projectZ.py-1.1.6.7/projectZ/utils/headers.py`

 * *Files identical despite different names*

### Comparing `projectZ.py-1.1.6.6/projectZ/utils/objects.py` & `projectZ.py-1.1.6.7/projectZ/utils/objects.py`

 * *Files identical despite different names*

### Comparing `projectZ.py-1.1.6.6/projectZ.py.egg-info/PKG-INFO` & `projectZ.py-1.1.6.7/projectZ.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projectZ.py
-Version: 1.1.6.6
+Version: 1.1.6.7
 Summary: Library for creating projectZ bots and scripts.
 Home-page: https://github.com/xXxCLOTIxXx/projectZ.py
 Author: Xsarz
 Author-email: xsarzy@gmail.com
 License: MIT
 Download-URL: https://github.com/xXxCLOTIxXx/projectZ.py/archive/refs/heads/main.zip
 Description: <table align="center">
```

### Comparing `projectZ.py-1.1.6.6/setup.py` & `projectZ.py-1.1.6.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as file:
 	long_description = file.read()
 
 link = 'https://github.com/xXxCLOTIxXx/projectZ.py/archive/refs/heads/main.zip'
-ver = '1.1.6.6'
+ver = '1.1.6.7'
 
 setup(
 	name = "projectZ.py",
 	version = ver,
 	url = "https://github.com/xXxCLOTIxXx/projectZ.py",
 	download_url = link,
 	license = "MIT",
```

