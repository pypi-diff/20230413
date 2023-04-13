# Comparing `tmp/pymino-1.1.7.3.tar.gz` & `tmp/pymino-1.1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\12095\Desktop\pymino-1.1.7.3\dist\.tmp-bqn8i7qo\pymino-1.1.7.3.tar", last modified: Mon Apr  3 18:51:03 2023, max compression
+gzip compressed data, was "C:\Users\12095\Desktop\pymino-1.1.7.4\dist\.tmp-bygfcxlr\pymino-1.1.7.4.tar", last modified: Thu Apr 13 01:05:09 2023, max compression
```

## Comparing `pymino-1.1.7.3.tar` & `pymino-1.1.7.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 18:51:03.028572 pymino-1.1.7.3/
--rw-rw-rw-   0        0        0     1085 2023-02-11 18:40:37.000000 pymino-1.1.7.3/LICENSE
--rw-rw-rw-   0        0        0     6082 2023-04-03 18:51:03.028572 pymino-1.1.7.3/PKG-INFO
--rw-rw-rw-   0        0        0     5364 2023-03-09 02:27:22.000000 pymino-1.1.7.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-03 18:51:02.989388 pymino-1.1.7.3/pymino/
--rw-rw-rw-   0        0        0      676 2023-04-03 18:37:50.000000 pymino-1.1.7.3/pymino/__init__.py
--rw-rw-rw-   0        0        0    26133 2023-04-03 18:49:59.000000 pymino-1.1.7.3/pymino/bot.py
--rw-rw-rw-   0        0        0    45388 2023-04-03 18:50:07.000000 pymino-1.1.7.3/pymino/client.py
-drwxrwxrwx   0        0        0        0 2023-04-03 18:51:03.011212 pymino-1.1.7.3/pymino/ext/
--rw-rw-rw-   0        0        0      372 2023-02-10 13:25:37.000000 pymino-1.1.7.3/pymino/ext/__init__.py
--rw-rw-rw-   0        0        0    10251 2023-03-09 02:24:21.000000 pymino-1.1.7.3/pymino/ext/account.py
--rw-rw-rw-   0        0        0   243704 2023-03-10 06:13:53.000000 pymino-1.1.7.3/pymino/ext/community.py
--rw-rw-rw-   0        0        0    39378 2023-03-05 23:08:15.000000 pymino-1.1.7.3/pymino/ext/context.py
--rw-rw-rw-   0        0        0      871 2023-03-04 01:25:46.000000 pymino-1.1.7.3/pymino/ext/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-04-03 18:51:03.023117 pymino-1.1.7.3/pymino/ext/entities/
--rw-rw-rw-   0        0        0      198 2023-03-05 23:07:04.000000 pymino-1.1.7.3/pymino/ext/entities/__init__.py
--rw-rw-rw-   0        0        0      765 2023-03-05 16:56:17.000000 pymino-1.1.7.3/pymino/ext/entities/enums.py
--rw-rw-rw-   0        0        0    14506 2023-03-10 06:04:42.000000 pymino-1.1.7.3/pymino/ext/entities/exceptions.py
--rw-rw-rw-   0        0        0    48713 2023-02-25 04:12:35.000000 pymino-1.1.7.3/pymino/ext/entities/general.py
--rw-rw-rw-   0        0        0     2536 2023-03-03 22:30:34.000000 pymino-1.1.7.3/pymino/ext/entities/handlers.py
--rw-rw-rw-   0        0        0    42816 2023-02-06 10:45:41.000000 pymino-1.1.7.3/pymino/ext/entities/messages.py
--rw-rw-rw-   0        0        0     6109 2023-02-10 17:39:14.000000 pymino-1.1.7.3/pymino/ext/entities/threads.py
--rw-rw-rw-   0        0        0    31609 2023-02-13 01:22:30.000000 pymino-1.1.7.3/pymino/ext/entities/userprofile.py
--rw-rw-rw-   0        0        0     2230 2023-03-05 23:07:39.000000 pymino-1.1.7.3/pymino/ext/entities/wsevents.py
--rw-rw-rw-   0        0        0     7414 2023-03-03 22:30:22.000000 pymino-1.1.7.3/pymino/ext/socket.py
-drwxrwxrwx   0        0        0        0 2023-04-03 18:51:03.027084 pymino-1.1.7.3/pymino/ext/utilities/
--rw-rw-rw-   0        0        0       80 2023-03-04 01:08:01.000000 pymino-1.1.7.3/pymino/ext/utilities/__init__.py
--rw-rw-rw-   0        0        0     6396 2023-03-02 00:41:30.000000 pymino-1.1.7.3/pymino/ext/utilities/commands.py
--rw-rw-rw-   0        0        0     1110 2023-02-28 16:10:43.000000 pymino-1.1.7.3/pymino/ext/utilities/generate.py
--rw-rw-rw-   0        0        0    10274 2023-04-02 23:47:45.000000 pymino-1.1.7.3/pymino/ext/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-04-03 18:51:03.004268 pymino-1.1.7.3/pymino.egg-info/
--rw-rw-rw-   0        0        0     6082 2023-04-03 18:51:02.000000 pymino-1.1.7.3/pymino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      799 2023-04-03 18:51:02.000000 pymino-1.1.7.3/pymino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 18:51:02.000000 pymino-1.1.7.3/pymino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-04-03 18:51:02.000000 pymino-1.1.7.3/pymino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-03 18:51:02.000000 pymino-1.1.7.3/pymino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      873 2023-04-03 18:51:03.034028 pymino-1.1.7.3/setup.cfg
--rw-rw-rw-   0        0        0     1340 2023-03-04 01:31:03.000000 pymino-1.1.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 01:05:09.349109 pymino-1.1.7.4/
+-rw-rw-rw-   0        0        0     1085 2023-02-11 18:40:37.000000 pymino-1.1.7.4/LICENSE
+-rw-rw-rw-   0        0        0     6082 2023-04-13 01:05:09.349109 pymino-1.1.7.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5364 2023-03-09 02:27:22.000000 pymino-1.1.7.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 01:05:09.289068 pymino-1.1.7.4/pymino/
+-rw-rw-rw-   0        0        0      676 2023-04-13 01:04:24.000000 pymino-1.1.7.4/pymino/__init__.py
+-rw-rw-rw-   0        0        0    26133 2023-04-03 18:49:59.000000 pymino-1.1.7.4/pymino/bot.py
+-rw-rw-rw-   0        0        0    48170 2023-04-13 01:03:38.000000 pymino-1.1.7.4/pymino/client.py
+drwxrwxrwx   0        0        0        0 2023-04-13 01:05:09.331723 pymino-1.1.7.4/pymino/ext/
+-rw-rw-rw-   0        0        0      372 2023-02-10 13:25:37.000000 pymino-1.1.7.4/pymino/ext/__init__.py
+-rw-rw-rw-   0        0        0    11206 2023-04-13 00:39:17.000000 pymino-1.1.7.4/pymino/ext/account.py
+-rw-rw-rw-   0        0        0   271440 2023-04-13 01:04:28.000000 pymino-1.1.7.4/pymino/ext/community.py
+-rw-rw-rw-   0        0        0    39378 2023-03-05 23:08:15.000000 pymino-1.1.7.4/pymino/ext/context.py
+-rw-rw-rw-   0        0        0      871 2023-03-04 01:25:46.000000 pymino-1.1.7.4/pymino/ext/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-04-13 01:05:09.342139 pymino-1.1.7.4/pymino/ext/entities/
+-rw-rw-rw-   0        0        0      198 2023-03-05 23:07:04.000000 pymino-1.1.7.4/pymino/ext/entities/__init__.py
+-rw-rw-rw-   0        0        0      765 2023-03-05 16:56:17.000000 pymino-1.1.7.4/pymino/ext/entities/enums.py
+-rw-rw-rw-   0        0        0    14506 2023-03-10 06:04:42.000000 pymino-1.1.7.4/pymino/ext/entities/exceptions.py
+-rw-rw-rw-   0        0        0    48713 2023-02-25 04:12:35.000000 pymino-1.1.7.4/pymino/ext/entities/general.py
+-rw-rw-rw-   0        0        0     2536 2023-03-03 22:30:34.000000 pymino-1.1.7.4/pymino/ext/entities/handlers.py
+-rw-rw-rw-   0        0        0    42816 2023-02-06 10:45:41.000000 pymino-1.1.7.4/pymino/ext/entities/messages.py
+-rw-rw-rw-   0        0        0     6109 2023-02-10 17:39:14.000000 pymino-1.1.7.4/pymino/ext/entities/threads.py
+-rw-rw-rw-   0        0        0    31609 2023-02-13 01:22:30.000000 pymino-1.1.7.4/pymino/ext/entities/userprofile.py
+-rw-rw-rw-   0        0        0     2230 2023-03-05 23:07:39.000000 pymino-1.1.7.4/pymino/ext/entities/wsevents.py
+-rw-rw-rw-   0        0        0     7414 2023-03-03 22:30:22.000000 pymino-1.1.7.4/pymino/ext/socket.py
+drwxrwxrwx   0        0        0        0 2023-04-13 01:05:09.348091 pymino-1.1.7.4/pymino/ext/utilities/
+-rw-rw-rw-   0        0        0       80 2023-03-04 01:08:01.000000 pymino-1.1.7.4/pymino/ext/utilities/__init__.py
+-rw-rw-rw-   0        0        0     6396 2023-03-02 00:41:30.000000 pymino-1.1.7.4/pymino/ext/utilities/commands.py
+-rw-rw-rw-   0        0        0     1110 2023-02-28 16:10:43.000000 pymino-1.1.7.4/pymino/ext/utilities/generate.py
+-rw-rw-rw-   0        0        0    10274 2023-04-02 23:47:45.000000 pymino-1.1.7.4/pymino/ext/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-04-13 01:05:09.304442 pymino-1.1.7.4/pymino.egg-info/
+-rw-rw-rw-   0        0        0     6082 2023-04-13 01:05:09.000000 pymino-1.1.7.4/pymino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      799 2023-04-13 01:05:09.000000 pymino-1.1.7.4/pymino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 01:05:09.000000 pymino-1.1.7.4/pymino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-04-13 01:05:09.000000 pymino-1.1.7.4/pymino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-13 01:05:09.000000 pymino-1.1.7.4/pymino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      873 2023-04-13 01:05:09.354539 pymino-1.1.7.4/setup.cfg
+-rw-rw-rw-   0        0        0     1340 2023-03-04 01:31:03.000000 pymino-1.1.7.4/setup.py
```

### Comparing `pymino-1.1.7.3/LICENSE` & `pymino-1.1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.3/PKG-INFO` & `pymino-1.1.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.7.3
+Version: 1.1.7.4
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.1.7.3 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.1.7.4 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.1.7.3/README.md` & `pymino-1.1.7.4/README.md`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.3/pymino/__init__.py` & `pymino-1.1.7.4/pymino/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __title__ = 'pymino'
 __author__ = 'cynical'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Cynical'
-__version__ = '1.1.7.3'
+__version__ = '1.1.7.4'
 __description__ = 'A Python wrapper for the aminoapps.com API'
 
 from .bot import Bot as Bot
 from .client import Client as Client
 
 from requests import get
 from colorama import Fore, Style
```

### Comparing `pymino-1.1.7.3/pymino/bot.py` & `pymino-1.1.7.4/pymino/bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.3/pymino/client.py` & `pymino-1.1.7.4/pymino/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .ext.entities.messages import CMessage, PrepareMessage
 
 from .ext.utilities.generate import device_id as generate_device_id
 from .ext.entities.exceptions import (
     LoginFailed, LoginRequired, MissingEmailPasswordOrSid, VerifyCommunityIdIsCorrect
     )
 from .ext.entities.general import (
-    ApiResponse, Authenticate, CCommunity, CCommunityList, ResetPassword, Wallet
+    ApiResponse, Authenticate, CCommunity, CCommunityList, ResetPassword, Wallet, LinkInfo
     )
 
 F = TypeVar("F", bound=Callable[..., Any])
 
 class Client:
     """
     `Client` - This is the main client.
@@ -601,14 +601,86 @@
 
         if self.debug:
             print(f"{Fore.MAGENTA}Logged in as {self.profile.username} ({self.profile.userId}){Style.RESET_ALL}")
 
         return response
 
 
+    def fetch_object_id(self, link: str) -> str:
+        """
+        Fetches the object ID given a link to the object.
+
+        :param link: The link to the object.
+        :type link: str
+        :raises NotLoggedIn: If the user is not logged in.
+        :raises MissingCommunityId: If the community ID is missing.
+        :return: The ID of the object.
+        :rtype: str
+
+        The `community` decorator is used to ensure that the user is logged in and the community ID is present.
+        The method caches the object ID for faster access in future calls.
+
+        **Example usage:**
+
+        >>> object_id = client.community.fetch_object_id(link="https://aminoapps.com/p/w2Fs6H")
+        >>> print(object_id)
+        """
+
+        KEY = str((link, "OBJECT_ID"))
+        if not self.cache.get(KEY):
+            self.cache.set(KEY, self.request.handler(
+                method = "GET",
+                url = f"/g/s/link-resolution?q={link}"
+                ))
+        return LinkInfo(self.cache.get(KEY)).objectId
+    
+
+    def fetch_object_info(self, link: str) -> LinkInfo:
+        """
+        Fetches information about an object given its link.
+
+        :param link: The link to the object.
+        :type link: str
+        :raises NotLoggedIn: If the user is not logged in.
+        :raises MissingCommunityId: If the community ID is missing.
+        :return: A LinkInfo object containing information about the object.
+        :rtype: LinkInfo
+
+        The `community` decorator is used to ensure that the user is logged in and the community ID is present.
+        The method caches the object information for faster access in future calls.
+
+        `LinkInfo`:
+
+        - `data`: The raw response data from the API.
+        - `linkInfoV2`: The link information data.
+        - `path`: The path of the object.
+        - `extensions`: The extensions data.
+        - `objectId`: The ID of the object.
+        - `shareURLShortCode`: The short code of the share URL.
+        - `targetCode`: The target code.
+        - `ndcId`: The NDC ID.
+        - `comId`: The community ID.
+        - `fullPath`: The full path of the object.
+        - `shortCode`: The short code of the object.
+        - `objectType`: The type of the object.
+
+        **Example usage:**
+
+        >>> object_info = client.community.fetch_object_info(link="https://aminoapps.com/p/w2Fs6H")
+        >>> print(object_info.objectId)
+        """
+
+        KEY = str((link, "OBJECT_INFO"))
+        if not self.cache.get(KEY):
+            self.cache.set(KEY, self.request.handler(
+                method = "GET",
+                url = f"/g/s/link-resolution?q={link}"
+                ))
+        return LinkInfo(self.cache.get(KEY))
+    
     @authenticated
     def disconnect_google(self, password: str) -> dict:
         """
         Disconnects the user's Google account from their account on Amino.
 
         :param password: The user's account password.
         :type password: str
```

### Comparing `pymino-1.1.7.3/pymino/ext/account.py` & `pymino-1.1.7.4/pymino/ext/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,14 +299,48 @@
             data={
                 "type": 1,
                 "identity": email,
                 "data": {"code":code},
                 "deviceID": device_id(),
                 "timestamp": int(time() * 1000)
             }))
+    
+    
+    def verify(self, email: str, code: str, deviceId: str) -> ApiResponse:
+        """
+        `**verify**` - Verifies the code sent to the email.
+
+        `**Parameters**`
+        
+        - `email` - The email of the account.
+        
+        - `code` - The code sent to the email.
+
+        - `deviceId` - The device id.
+        
+        `**Example**`
+        
+        ```py
+        from pymino import *
+        
+        bot = Bot()
+        response = bot.verify(email=email, code=code, deviceId=deviceId)
+        print(response)
+        ```
+        """
+        return ApiResponse(self.session.handler(
+            method = "POST",
+            url="/g/s/auth/check-security-validation",
+            data={
+                "type": 1,
+                "identity": email,
+                "data": {"code":code},
+                "deviceID": deviceId,
+                "timestamp": int(time() * 1000)
+            }))
 
     def reset_password(self, email: str, newPassword: str, code: str, deviceId: str = device_id()) -> ResetPassword:
         """
         `**reset_password**` - Resets the password.
 
         `**Parameters**`
```

### Comparing `pymino-1.1.7.3/pymino/ext/community.py` & `pymino-1.1.7.4/pymino/ext/community.py`

 * *Files 3% similar despite different names*

```diff
@@ -900,14 +900,48 @@
         >>> notifications = client.community.fetch_notifications(size=10)
         >>> listOfOfObjectIds = notifications.objectId
         """
         return NotificationList(self.session.handler(
             method = "GET",
             url = f"/x{self.community_id if comId is None else comId}/s/notification?pagingType=t&size={size}"
             ))
+    
+    
+    @community
+    def clear_notifications(self, comId: Union[str, int] = None) -> ApiResponse:
+        """
+        Clears all notifications for the current or specified community.
+
+        :param comId: The ID of the community to clear the notifications for. If not provided, the current community ID is used.
+        :type comId: Union[str, int]
+        :raises NotLoggedIn: If the user is not logged in.
+        :return: An ApiResponse object containing the status of the request.
+        :rtype: ApiResponse
+
+        The `community` decorator is used to ensure that the user is logged in and the community ID is present.
+
+        The function sends a DELETE request to the API to clear the notifications.
+
+        `ApiResponse`:
+
+        - `statuscode`: The status code of the request.
+        - `status`: The status of the request.
+        - `duration`: The duration of the API request.
+        - `timestamp`: The timestamp of the API response.
+
+        **Example usage:**
+
+        >>> api_response = client.community.clear_notifications()
+        >>> if api_response.statuscode == 0:
+        ...     print("Notifications cleared successfully!")
+        """
+        return ApiResponse(self.session.handler(
+            method = "DELETE",
+            url = f"/x{self.community_id if comId is None else comId}/s/notification"
+            ))
 
 
     @community
     def fetch_user(self, userId: str, comId: Union[str, int] = None) -> UserProfile:
         """
         Fetches the user profile of the specified user in the current or specified community.
 
@@ -5157,8 +5191,593 @@
             "adminOpName": 18,
             "timestamp": int(time() * 1000)
             } if reason is None else {
             "adminOpNote": {"content": reason},
             "adminOpName": 18,
             "timestamp": int(time() * 1000)
             }))
-    
+    
+    @community
+    def invite_to_vc(self, chatId: str, userId: str, comId: Union[str, int] = None) -> ApiResponse:
+        """
+        Invites a user to a voice chat in the current or specified community.
+
+        :param chatId: The ID of the chat to invite the user to.
+        :type chatId: str
+        :param userId: The ID of the user to invite.
+        :type userId: str
+        :param comId: The ID of the community where the chat is located. If not provided, the current community ID is used.
+        :type comId: Union[str, int]
+        :return: An `ApiResponse` object containing information about the request status.
+        :rtype: ApiResponse
+
+        This function sends a POST request to the API to invite a user to a voice chat in the specified community.
+
+        `ApiResponse`:
+
+        - `message` (str): A message indicating whether the user was successfully invited to the voice chat.
+        - `statuscode` (int): The status code of the API response.
+        - `duration` (str): The duration of the API request.
+        - `timestamp` (str): The timestamp of the API request.
+
+        **Example usage:**
+
+        To invite a user with ID "0000-0000-0000-0000" to a voice chat with ID "1111-1111-1111-1111" in the current community:
+
+        >>> response = client.community.invite_to_vc(chatId="1111-1111-1111-1111", userId="0000-0000-0000-0000")
+        ... if response.statuscode == 0:
+        ...     print("User invited successfully!")
+        ... else:
+        ...     print("Failed to invite user.")
+
+        To invite a user with ID "1111-1111-1111-1111" to a voice chat with ID "2222-2222-2222-2222" in a community with ID "123":
+
+        >>> response = client.community.invite_to_vc(chatId="2222-2222-2222-2222", userId="1111-1111-1111-1111", comId=123)
+        ... if response.statuscode == 0:
+        ...     print("User invited successfully!")
+        ... else:
+        ...     print("Failed to invite user.")
+        """
+        return ApiResponse(self.session.handler(
+            method = "POST",
+            url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/vvchat-presenter/invite/",
+            data = {"uid": userId}))
+    
+    @community
+    def feature_user(self, time: int, userId: str, comId: Union[str, int] = None) -> ApiResponse:
+        """
+        Features a user in the current or specified community.
+
+        :param time: The duration of the feature. 1 = 1 day, 2 = 2 days, 3 = 3 days.
+        :type time: int
+        :param userId: The ID of the user to feature.
+        :type userId: str
+        :param comId: The ID of the community to feature the user in. If not provided, the current community ID is used.
+        :type comId: Union[str, int]
+        :return: An `ApiResponse` object containing information about the request status.
+        :rtype: ApiResponse
+
+        This function sends a POST request to the API to feature a user in the specified community.
+
+        `ApiResponse`:
+
+        - `message` (str): A message indicating whether the user was successfully featured.
+        - `statuscode` (int): The status code of the API response.
+        - `duration` (str): The duration of the API request.
+        - `timestamp` (str): The timestamp of the API request.
+
+        **Example usage:**
+
+        To feature a user with ID "0000-0000-0000-0000" for 1 day in the current community:
+
+        >>> response = client.community.feature_user(time=1, userId="0000-0000-0000-0000")
+        ... if response.statuscode == 0:
+        ...     print("User featured successfully!")
+        ... else:
+        ...     print("Failed to feature user.")
+
+        To feature a user with ID "1111-1111-1111-1111" for 2 days in a community with ID "123":
+
+        >>> response = client.community.feature_user(time=2, userId="1111-1111-1111-1111", comId=123)
+        ... if response.statuscode == 0:
+        ...     print("User featured successfully!")
+        ... else:
+        ...     print("Failed to feature user.")
+        """
+        return ApiResponse(self.session.handler(
+            method = "POST",
+            url = f"/x{self.community_id if comId is None else comId}/s/user-profile/{userId}/admin",
+            data = {
+            "adminOpName": 114,
+            "adminOpValue": {"featuredType": 4, "featuredDuration": 86400 if time == 1 else 172800 if time == 2 else 259200 if time == 3 else None},
+            "timestamp": int(time() * 1000)
+            }))
+    
+    @community
+    def feature_chat(self, time: int, chatId: str, comId: Union[str, int] = None) -> ApiResponse:
+        """
+        Features a chat in the current or specified community.
+
+        :param time: The duration of the feature. 1 = 1 hour, 2 = 2 hours, 3 = 3 hours.
+        :type time: int
+        :param chatId: The ID of the chat to feature.
+        :type chatId: str
+        :param comId: The ID of the community to feature the chat in. If not provided, the current community ID is used.
+        :type comId: Union[str, int]
+        :return: An `ApiResponse` object containing information about the request status.
+        :rtype: ApiResponse
+
+        This function sends a POST request to the API to feature a chat in the specified community.
+
+        `ApiResponse`:
+
+        - `message` (str): A message indicating whether the chat was successfully featured.
+        - `statuscode` (int): The status code of the API response.
+        - `duration` (str): The duration of the API request.
+        - `timestamp` (str): The timestamp of the API request.
+
+        **Example usage:**
+
+        To feature a chat with ID "0000-0000-0000-0000" for 1 hour in the current community:
+
+        >>> response = client.community.feature_chat(time=1, chatId="0000-0000-0000-0000")
+        ... if response.statuscode == 0:
+        ...     print("Chat featured successfully!")
+        ... else:
+        ...     print("Failed to feature chat.")
+
+        To feature a chat with ID "1111-1111-1111-1111" for 2 hours in a community with ID "123":
+
+        >>> response = client.community.feature_chat(time=2, chatId="1111-1111-1111-1111", comId=123)
+        ... if response.statuscode == 0:
+        ...     print("Chat featured successfully!")
+        ... else:
+        ...     print("Failed to feature chat.")
+        """
+        return ApiResponse(self.session.handler(
+            method = "POST",
+            url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/admin",
+            data = {
+            "adminOpName": 114,
+            "adminOpValue": {"featuredType": 5, "featuredDuration": 3600 if time == 1 else 7200 if time == 2 else 10800 if time == 3 else None},
+            "timestamp": int(time() * 1000)
+            }))
+    
+    @community
+    def feature_blog(self, time: int, blogId: str, comId: Union[str, int] = None) -> ApiResponse:
+        """
+        Features a blog in the current or specified community.
+
+        :param time: The duration of the feature. 1 = 1 day, 2 = 2 days, 3 = 3 days.
+        :type time: int
+        :param blogId: The ID of the blog to feature.
+        :type blogId: str
+        :param comId: The ID of the community to feature the blog in. If not provided, the current community ID is used.
+        :type comId: Union[str, int]
+        :return: An `ApiResponse` object containing information about the request status.
+        :rtype: ApiResponse
+
+        This function sends a POST request to the API to feature a blog in the specified community.
+
+        `ApiResponse`:
+
+        - `message` (str): A message indicating whether the blog was successfully featured.
+        - `statuscode` (int): The status code of the API response.
+        - `duration` (str): The duration of the API request.
+        - `timestamp` (str): The timestamp of the API request.
+
+        **Example usage:**
+
+        To feature a blog with ID "0000-0000-0000-0000" for 1 day in the current community:
+
+        >>> response = client.community.feature_blog(time=1, blogId="0000-0000-0000-0000")
+        ... if response.statuscode == 0:
+        ...     print("Blog featured successfully!")
+        ... else:
+        ...     print("Failed to feature blog.")
+
+        To feature a blog with ID "1111-1111-1111-1111" for 2 days in a community with ID "123":
+
+        >>> response = client.community.feature_blog(time=2, blogId="1111-1111-1111-1111", comId=123)
+        ... if response.statuscode == 0:
+        ...     print("Blog featured successfully!")
+        ... else:
+        ...     print("Failed to feature blog.")
+        """
+        return ApiResponse(self.session.handler(
+            method = "POST",
+            url = f"/x{self.community_id if comId is None else comId}/s/blog/{blogId}/admin",
+            data = {
+            "adminOpName": 114,
+            "adminOpValue": {"featuredType": 1, "featuredDuration": 86400 if time == 1 else 172800 if time == 2 else 259200 if time == 3 else None},
+            "timestamp": int(time() * 1000)
+            }))
+    
+    @community
+    def feature_wiki(self, time: int, wikiId: str, comId: Union[str, int] = None) -> ApiResponse:
+        """
+        Features a wiki in the current or specified community.
+
+        :param time: The duration of the feature. 1 = 1 day, 2 = 2 days, 3 = 3 days.
+        :type time: int
+        :param wikiId: The ID of the wiki to feature.
+        :type wikiId: str
+        :param comId: The ID of the community to feature the wiki in. If not provided, the current community ID is used.
+        :type comId: Union[str, int]
+        :return: An `ApiResponse` object containing information about the request status.
+        :rtype: ApiResponse
+
+        This function sends a POST request to the API to feature a wiki in the specified community.
+
+        `ApiResponse`:
+
+        - `message` (str): A message indicating whether the wiki was successfully featured.
+        - `statuscode` (int): The status code of the API response.
+        - `duration` (str): The duration of the API request.
+        - `timestamp` (str): The timestamp of the API request.
+
+        **Example usage:**
+
+        To feature a wiki with ID "0000-0000-0000-0000" for 1 day in the current community:
+
+        >>> response = client.community.feature_wiki(time=1, wikiId="0000-0000-0000-0000")
+        ... if response.statuscode == 0:
+        ...     print("Wiki featured successfully!")
+        ... else:
+        ...     print("Failed to feature wiki.")
+
+        To feature a wiki with ID "1111-1111-1111-1111" for 2 days in a community with ID "123":
+
+        >>> response = client.community.feature_wiki(time=2, wikiId="1111-1111-1111-1111", comId=123)
+        ... if response.statuscode == 0:
+        ...     print("Wiki featured successfully!")
+        ... else:
+        ...     print("Failed to feature wiki.")
+        """
+        return ApiResponse(self.session.handler(
+            method = "POST",
+            url = f"/x{self.community_id if comId is None else comId}/s/item/{wikiId}/admin",
+            data = {
+            "adminOpName": 114,
+            "adminOpValue": {"featuredType": 2, "featuredDuration": 86400 if time == 1 else 172800 if time == 2 else 259200 if time == 3 else None},
+            "timestamp": int(time() * 1000)
+            }))
+
+    @community
+    def unfeature_chat(self, chatId: str, comId: Union[str, int] = None) -> ApiResponse:
+        """
+        Unfeatures a chat in the current or specified community.
+
+        :param chatId: The ID of the chat to unfeature.
+        :type chatId: str
+        :param comId: The ID of the community to unfeature the chat in. If not provided, the current community ID is used.
+        :type comId: Union[str, int]
+        :return: An `ApiResponse` object containing information about the request status.
+        :rtype: ApiResponse
+
+        This function sends a POST request to the API to unfeature a chat in the specified community.
+
+        `ApiResponse`:
+
+        - `message` (str): A message indicating whether the chat was successfully unfeatured.
+        - `statuscode` (int): The status code of the API response.
+        - `duration` (str): The duration of the API request.
+        - `timestamp` (str): The timestamp of the API request.
+
+        **Example usage:**
+
+        To unfeature a chat with ID "0000-0000-0000-0000" in the current community:
+
+        >>> response = client.community.unfeature_chat(chatId="0000-0000-0000-0000")
+        ... if response.statuscode == 0:
+        ...     print("Chat unfeatured successfully!")
+        ... else:
+        ...     print("Failed to unfeature chat.")
+
+        To unfeature a chat with ID "1111-1111-1111-1111" in a community with ID "123":
+
+        >>> response = client.community.unfeature_chat(chatId="1111-1111-1111-1111", comId=123)
+        ... if response.statuscode == 0:
+        ...     print("Chat unfeatured successfully!")
+        ... else:
+        ...     print("Failed to unfeature chat.")
+        """
+        return ApiResponse(self.session.handler(
+            method = "POST",
+            url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/admin",
+            data = {
+            "adminOpName": 114,
+            "adminOpValue": {"featuredType": 0},
+            "timestamp": int(time() * 1000)
+            }))
+
+    @community
+    def unfeature_wiki(self, wikiId: str, comId: Union[str, int] = None) -> ApiResponse:
+        """
+        Unfeatures a wiki in the current or specified community.
+
+        :param wikiId: The ID of the wiki to unfeature.
+        :type wikiId: str
+        :param comId: The ID of the community to unfeature the wiki in. If not provided, the current community ID is used.
+        :type comId: Union[str, int]
+        :return: An `ApiResponse` object containing information about the request status.
+        :rtype: ApiResponse
+
+        This function sends a POST request to the API to unfeature a wiki in the specified community.
+
+        `ApiResponse`:
+
+        - `message` (str): A message indicating whether the wiki was successfully unfeatured.
+        - `statuscode` (int): The status code of the API response.
+        - `duration` (str): The duration of the API request.
+        - `timestamp` (str): The timestamp of the API request.
+
+        **Example usage:**
+
+        To unfeature a wiki with ID "0000-0000-0000-0000" in the current community:
+
+        >>> response = client.community.unfeature_wiki(wikiId="0000-0000-0000-0000")
+        ... if response.statuscode == 0:
+        ...     print("Wiki unfeatured successfully!")
+        ... else:
+        ...     print("Failed to unfeature wiki.")
+
+        To unfeature a wiki with ID "1111-1111-1111-1111" in a community with ID "123":
+
+        >>> response = client.community.unfeature_wiki(wikiId="1111-1111-1111-1111", comId=123)
+        ... if response.statuscode == 0:
+        ...     print("Wiki unfeatured successfully!")
+        ... else:
+        ...     print("Failed to unfeature wiki.")
+        """
+        return ApiResponse(self.session.handler(
+            method = "POST",
+            url = f"/x{self.community_id if comId is None else comId}/s/item/{wikiId}/admin",
+            data = {
+            "adminOpName": 114,
+            "adminOpValue": {"featuredType": 0},
+            "timestamp": int(time() * 1000)
+            }))
+
+    @community
+    def unfeature_blog(self, blogId: str, comId: Union[str, int] = None) -> ApiResponse:
+        """
+        Unfeatures a blog in the current or specified community.
+
+        :param blogId: The ID of the blog to unfeature.
+        :type blogId: str
+        :param comId: The ID of the community to unfeature the blog in. If not provided, the current community ID is used.
+        :type comId: Union[str, int]
+        :return: An `ApiResponse` object containing information about the request status.
+        :rtype: ApiResponse
+
+        This function sends a POST request to the API to unfeature a blog in the specified community.
+
+        `ApiResponse`:
+
+        - `message` (str): A message indicating whether the blog was successfully unfeatured.
+        - `statuscode` (int): The status code of the API response.
+        - `duration` (str): The duration of the API request.
+        - `timestamp` (str): The timestamp of the API request.
+
+        **Example usage:**
+
+        To unfeature a blog with ID "0000-0000-0000-0000" in the current community:
+
+        >>> response = client.community.unfeature_blog(blogId="0000-0000-0000-0000")
+        ... if response.statuscode == 0:
+        ...     print("Blog unfeatured successfully!")
+        ... else:
+        ...     print("Failed to unfeature blog.")
+
+        To unfeature a blog with ID "1111-1111-1111-1111" in a community with ID "123":
+
+        >>> response = client.community.unfeature_blog(blogId="1111-1111-1111-1111", comId=123)
+        ... if response.statuscode == 0:
+        ...     print("Blog unfeatured successfully!")
+        ... else:
+        ...     print("Failed to unfeature blog.")
+        """
+        return ApiResponse(self.session.handler(
+            method = "POST",
+            url = f"/x{self.community_id if comId is None else comId}/s/blog/{blogId}/admin",
+            data = {
+            "adminOpName": 114,
+            "adminOpValue": {"featuredType": 0},
+            "timestamp": int(time() * 1000)
+            }))
+    
+    @community
+    def unfeature_user(self, userId: str, comId: Union[str, int] = None) -> ApiResponse:
+        """
+        Unfeatures a user in the current or specified community.
+
+        :param userId: The ID of the user to unfeature.
+        :type userId: str
+        :param comId: The ID of the community to unfeature the user in. If not provided, the current community ID is used.
+        :type comId: Union[str, int]
+        :return: An `ApiResponse` object containing information about the request status.
+        :rtype: ApiResponse
+
+        This function sends a POST request to the API to unfeature a user in the specified community.
+
+        `ApiResponse`:
+
+        - `message` (str): A message indicating whether the user was successfully unfeatured.
+        - `statuscode` (int): The status code of the API response.
+        - `duration` (str): The duration of the API request.
+        - `timestamp` (str): The timestamp of the API request.
+
+        **Example usage:**
+
+        To unfeature a user with ID "0000-0000-0000-0000" in the current community:
+
+        >>> response = client.community.unfeature_user(userId="0000-0000-0000-0000")
+        ... if response.statuscode == 0:
+        ...     print("User unfeatured successfully!")
+        ... else:
+        ...     print("Failed to unfeature user.")
+
+        To unfeature a user with ID "1111-1111-1111-1111" in a community with ID "123":
+
+        >>> response = client.community.unfeature_user(userId="1111-1111-1111-1111", comId=123)
+        ... if response.statuscode == 0:
+        ...     print("User unfeatured successfully!")
+        ... else:
+        ...     print("Failed to unfeature user.")
+        """
+        return ApiResponse(self.session.handler(
+            method = "POST",
+            url = f"/x{self.community_id if comId is None else comId}/s/user-profile/{userId}/admin",
+            data = {
+            "adminOpName": 114,
+            "adminOpValue": {"featuredType": 0},
+            "timestamp": int(time() * 1000)
+            }))
+
+
+    @community
+    def claim_vc_reputation(self, chatId: str, comId: Union[str, int] = None) -> ApiResponse:
+        """
+        Claims VC reputation for the current or specified community.
+
+        :param chatId: The ID of the chat to claim VC reputation for.
+        :type chatId: str
+        :param comId: The ID of the community to claim VC reputation for. If not provided, the current community ID is used.
+        :type comId: Union[str, int]
+        :return: An `ApiResponse` object containing information about the request status.
+        :rtype: ApiResponse
+
+        This function sends a POST request to the API to claim VC reputation for the specified community.
+
+        `ApiResponse`:
+
+        - `message` (str): A message indicating whether the VC reputation was successfully claimed.
+        - `statuscode` (int): The status code of the API response.
+        - `duration` (str): The duration of the API request.
+        - `timestamp` (str): The timestamp of the API request.
+
+        **Example usage:**
+
+        To claim VC reputation for the current community:
+
+        >>> response = client.community.claim_vc_reputation(chatId="0000-0000-0000-0000")
+        ... if response.statuscode == 0:
+        ...     print("VC reputation claimed successfully!")
+        ... else:
+        ...     print("Failed to claim VC reputation.")
+
+        To claim VC reputation for a community with ID "123":
+
+        >>> response = client.community.claim_vc_reputation(chatId="0000-0000-0000-0000", comId=123)
+        ... if response.statuscode == 0:
+        ...     print("VC reputation claimed successfully!")
+        ... else:
+        ...     print("Failed to claim VC reputation.")
+        """
+        return ApiResponse(self.session.handler(
+            method = "POST",
+            url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/avchat-reputation",
+            data = {
+            "timestamp": int(time() * 1000)
+            }))
+    
+
+    @community
+    def fetch_vc_reputation_info(self, chatId: str, comId: Union[str, int] = None) -> ApiResponse:
+        """
+        Fetches VC reputation information for the current or specified community.
+
+        :param chatId: The ID of the chat to fetch VC reputation information for.
+        :type chatId: str
+        :param comId: The ID of the community to fetch VC reputation information for. If not provided, the current community ID is used.
+        :type comId: Union[str, int]
+        :return: An `ApiResponse` object containing information about the request status.
+        :rtype: ApiResponse
+
+        This function sends a GET request to the API to fetch VC reputation information for the specified community.
+
+        `ApiResponse`:
+
+        - `message` (str): A message indicating whether the VC reputation information was successfully fetched.
+        - `statuscode` (int): The status code of the API response.
+        - `duration` (str): The duration of the API request.
+        - `timestamp` (str): The timestamp of the API request.
+
+        **Example usage:**
+
+        To fetch VC reputation information for the current community:
+
+        >>> response = client.community.fetch_vc_reputation_info(chatId="0000-0000-0000-0000")
+        ... if response.statuscode == 0:
+        ...     print("VC reputation information fetched successfully!")
+        ... else:
+        ...     print("Failed to fetch VC reputation information.")
+
+        To fetch VC reputation information for a community with ID "123":
+
+        >>> response = client.community.fetch_vc_reputation_info(chatId="0000-0000-0000-0000", comId=123)
+        ... if response.statuscode == 0:
+        ...     print("VC reputation information fetched successfully!")
+        ... else:
+        ...     print("Failed to fetch VC reputation information.")
+        """
+        return ApiResponse(self.session.handler(
+            method = "GET",
+            url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/avchat-reputation",
+            data = {
+            "timestamp": int(time() * 1000)
+            }))
+
+
+    def subscribe_influencer(self, userId: str, autoRenew: bool = False, transactionId: str = None, comId: Union[str, int] = None) -> ApiResponse:
+        """
+        Subscribes to an influencer.
+
+        :param userId: The ID of the user to subscribe to.
+        :type userId: str
+        :param autoRenew: Whether to automatically renew the subscription.
+        :type autoRenew: bool
+        :param transactionId: The ID of the transaction. If not provided, a random UUID is used.
+        :type transactionId: str
+        :param comId: The ID of the community to subscribe to the influencer in. If not provided, the current community ID is used.
+        :type comId: Union[str, int]
+        :return: An `ApiResponse` object containing information about the request status.
+        :rtype: ApiResponse
+
+        This function sends a POST request to the API to subscribe to an influencer.
+
+        `ApiResponse`:
+
+        - `message` (str): A message indicating whether the subscription was successful.
+        - `statuscode` (int): The status code of the API response.
+        - `duration` (str): The duration of the API request.
+        - `timestamp` (str): The timestamp of the API request.
+
+        **Example usage:**
+
+        To subscribe to an influencer with ID "0000-0000-0000-0000" in the current community:
+
+        >>> response = client.community.subscribe_influencer(userId="0000-0000-0000-0000")
+        ... if response.statuscode == 0:
+        ...     print("Subscribed successfully!")
+        ... else:
+        ...     print("Failed to subscribe.")
+
+        To subscribe to an influencer with ID "1111-1111-1111-1111" in a community with ID "123":
+
+        >>> response = client.community.subscribe_influencer(userId="1111-1111-1111-1111", comId=123)
+        ... if response.statuscode == 0:
+        ...     print("Subscribed successfully!")
+        ... else:
+        ...     print("Failed to subscribe.")
+        """
+        return ApiResponse(self.session.handler(
+            method = "POST",
+            url = f"/x{self.community_id if comId is None else comId}/s/influencer/{userId}/subscribe",
+            data = {
+            "paymentContext": {
+                "transactionId": str(uuid4()) if transactionId is None else transactionId,
+                "isAutoRenew": autoRenew
+            },
+            "timestamp": int(time() * 1000)
+            }))
```

### Comparing `pymino-1.1.7.3/pymino/ext/context.py` & `pymino-1.1.7.4/pymino/ext/context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.3/pymino/ext/dispatcher.py` & `pymino-1.1.7.4/pymino/ext/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.3/pymino/ext/entities/enums.py` & `pymino-1.1.7.4/pymino/ext/entities/enums.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.3/pymino/ext/entities/exceptions.py` & `pymino-1.1.7.4/pymino/ext/entities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.3/pymino/ext/entities/general.py` & `pymino-1.1.7.4/pymino/ext/entities/general.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.3/pymino/ext/entities/handlers.py` & `pymino-1.1.7.4/pymino/ext/entities/handlers.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.3/pymino/ext/entities/messages.py` & `pymino-1.1.7.4/pymino/ext/entities/messages.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.3/pymino/ext/entities/threads.py` & `pymino-1.1.7.4/pymino/ext/entities/threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.3/pymino/ext/entities/userprofile.py` & `pymino-1.1.7.4/pymino/ext/entities/userprofile.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.3/pymino/ext/entities/wsevents.py` & `pymino-1.1.7.4/pymino/ext/entities/wsevents.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.3/pymino/ext/socket.py` & `pymino-1.1.7.4/pymino/ext/socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.3/pymino/ext/utilities/commands.py` & `pymino-1.1.7.4/pymino/ext/utilities/commands.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.3/pymino/ext/utilities/generate.py` & `pymino-1.1.7.4/pymino/ext/utilities/generate.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.3/pymino/ext/utilities/request_handler.py` & `pymino-1.1.7.4/pymino/ext/utilities/request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.3/pymino.egg-info/PKG-INFO` & `pymino-1.1.7.4/pymino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.7.3
+Version: 1.1.7.4
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.1.7.3 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.1.7.4 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.1.7.3/pymino.egg-info/SOURCES.txt` & `pymino-1.1.7.4/pymino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.3/setup.cfg` & `pymino-1.1.7.4/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 696e 6f0d 0a76 6572 7369   = pymino..versi
-00000020: 6f6e 203d 2031 2e31 2e37 2e33 0d0a 6175  on = 1.1.7.3..au
+00000020: 6f6e 203d 2031 2e31 2e37 2e34 0d0a 6175  on = 1.1.7.4..au
 00000030: 7468 6f72 203d 2066 6f72 6576 6572 6379  thor = forevercy
 00000040: 6e69 6361 6c0d 0a61 7574 686f 725f 656d  nical..author_em
 00000050: 6169 6c20 3d20 6d65 4063 796e 6963 616c  ail = me@cynical
 00000060: 2e67 670d 0a64 6573 6372 6970 7469 6f6e  .gg..description
 00000070: 203d 2045 6173 696c 7920 6372 6561 7465   = Easily create
 00000080: 2061 2062 6f74 2066 6f72 2041 6d69 6e6f   a bot for Amino
 00000090: 2041 7070 7320 7573 696e 6720 6120 6d6f   Apps using a mo
```

### Comparing `pymino-1.1.7.3/setup.py` & `pymino-1.1.7.4/setup.py`

 * *Files identical despite different names*

