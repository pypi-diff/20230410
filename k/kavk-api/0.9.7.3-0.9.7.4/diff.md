# Comparing `tmp/kavk_api-0.9.7.3.tar.gz` & `tmp/kavk_api-0.9.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kavk_api-0.9.7.3.tar", max compression
+gzip compressed data, was "kavk_api-0.9.7.4.tar", max compression
```

## Comparing `kavk_api-0.9.7.3.tar` & `kavk_api-0.9.7.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1066 2023-04-08 11:31:33.141480 kavk_api-0.9.7.3/LICENSE
--rw-r--r--   0        0        0     1251 2023-04-08 11:46:12.307389 kavk_api-0.9.7.3/README.rst
--rw-r--r--   0        0        0       51 2023-04-08 11:31:33.141480 kavk_api-0.9.7.3/kavk_api/__init__.py
--rw-r--r--   0        0        0     3192 2023-04-08 15:49:21.388876 kavk_api-0.9.7.3/kavk_api/bot_longpoll.py
--rw-r--r--   0        0        0    10766 2023-04-08 11:31:33.141480 kavk_api-0.9.7.3/kavk_api/enums.py
--rw-r--r--   0        0        0      341 2023-04-08 11:31:33.141480 kavk_api-0.9.7.3/kavk_api/exceptions.py
--rw-r--r--   0        0        0     4037 2023-04-08 11:31:33.141480 kavk_api-0.9.7.3/kavk_api/kavk_api.py
--rw-r--r--   0        0        0     7917 2023-04-08 11:31:33.142480 kavk_api-0.9.7.3/kavk_api/longpoll.py
--rw-r--r--   0        0        0     3773 2023-04-08 19:28:05.512515 kavk_api-0.9.7.3/kavk_api/types/base.py
--rw-r--r--   0        0        0     8143 2023-04-09 07:57:29.029583 kavk_api-0.9.7.3/kavk_api/types/bot_events.py
--rw-r--r--   0        0        0     5024 2023-04-09 07:57:45.848583 kavk_api-0.9.7.3/kavk_api/types/event_objects.py
--rw-r--r--   0        0        0   202079 2023-04-08 18:52:13.418738 kavk_api-0.9.7.3/kavk_api/types/methods.py
--rw-r--r--   0        0        0   144553 2023-04-08 11:31:33.144480 kavk_api-0.9.7.3/kavk_api/types/objects.py
--rw-r--r--   0        0        0    43554 2023-04-08 11:31:33.145480 kavk_api-0.9.7.3/kavk_api/types/responses.py
--rw-r--r--   0        0        0      123 2023-04-08 11:31:33.145480 kavk_api-0.9.7.3/kavk_api/utils.py
--rw-r--r--   0        0        0      423 2023-04-09 07:58:26.451582 kavk_api-0.9.7.3/pyproject.toml
--rw-r--r--   0        0        0     1689 1970-01-01 00:00:00.000000 kavk_api-0.9.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-08 11:31:33.141480 kavk_api-0.9.7.4/LICENSE
+-rw-r--r--   0        0        0     1251 2023-04-08 11:46:12.307389 kavk_api-0.9.7.4/README.rst
+-rw-r--r--   0        0        0       51 2023-04-08 11:31:33.141480 kavk_api-0.9.7.4/kavk_api/__init__.py
+-rw-r--r--   0        0        0     3192 2023-04-08 15:49:21.388876 kavk_api-0.9.7.4/kavk_api/bot_longpoll.py
+-rw-r--r--   0        0        0    10766 2023-04-08 11:31:33.141480 kavk_api-0.9.7.4/kavk_api/enums.py
+-rw-r--r--   0        0        0      341 2023-04-08 11:31:33.141480 kavk_api-0.9.7.4/kavk_api/exceptions.py
+-rw-r--r--   0        0        0     4037 2023-04-08 11:31:33.141480 kavk_api-0.9.7.4/kavk_api/kavk_api.py
+-rw-r--r--   0        0        0     8287 2023-04-09 08:41:13.287542 kavk_api-0.9.7.4/kavk_api/longpoll.py
+-rw-r--r--   0        0        0     3609 2023-04-10 10:30:26.347957 kavk_api-0.9.7.4/kavk_api/types/base.py
+-rw-r--r--   0        0        0     8143 2023-04-09 07:57:29.029583 kavk_api-0.9.7.4/kavk_api/types/bot_events.py
+-rw-r--r--   0        0        0     5024 2023-04-09 07:57:45.848583 kavk_api-0.9.7.4/kavk_api/types/event_objects.py
+-rw-r--r--   0        0        0   261659 2023-04-09 19:27:05.290321 kavk_api-0.9.7.4/kavk_api/types/methods.py
+-rw-r--r--   0        0        0   144553 2023-04-08 11:31:33.144480 kavk_api-0.9.7.4/kavk_api/types/objects.py
+-rw-r--r--   0        0        0    43571 2023-04-10 10:34:30.165969 kavk_api-0.9.7.4/kavk_api/types/responses.py
+-rw-r--r--   0        0        0      123 2023-04-08 11:31:33.145480 kavk_api-0.9.7.4/kavk_api/utils.py
+-rw-r--r--   0        0        0      423 2023-04-10 10:35:46.812972 kavk_api-0.9.7.4/pyproject.toml
+-rw-r--r--   0        0        0     1689 1970-01-01 00:00:00.000000 kavk_api-0.9.7.4/PKG-INFO
```

### Comparing `kavk_api-0.9.7.3/LICENSE` & `kavk_api-0.9.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kavk_api-0.9.7.3/README.rst` & `kavk_api-0.9.7.4/README.rst`

 * *Files identical despite different names*

### Comparing `kavk_api-0.9.7.3/kavk_api/bot_longpoll.py` & `kavk_api-0.9.7.4/kavk_api/bot_longpoll.py`

 * *Files identical despite different names*

### Comparing `kavk_api-0.9.7.3/kavk_api/enums.py` & `kavk_api-0.9.7.4/kavk_api/enums.py`

 * *Files identical despite different names*

### Comparing `kavk_api-0.9.7.3/kavk_api/kavk_api.py` & `kavk_api-0.9.7.4/kavk_api/kavk_api.py`

 * *Files identical despite different names*

### Comparing `kavk_api-0.9.7.3/kavk_api/longpoll.py` & `kavk_api-0.9.7.4/kavk_api/longpoll.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import datetime
 from .enums import *
-from .kavk_api import Vk
+from .kavk_vk import Vk
 
 class Event(object):
     """ Событие, полученное от longpoll-сервера.
     Имеет поля в соответствии с `документацией
     <https://vk.com/dev/using_longpoll_2?f=3.%2BСтруктура%2Bсобытий>`_.
     События `MESSAGE_NEW` и `MESSAGE_EDIT` имеют (среди прочих) такие поля:
         - `text` - `экранированный <https://ru.wikipedia.org/wiki/Мнемоники_в_HTML>`_ текст
@@ -154,69 +154,81 @@
                               VkChatEventType.USER_LEFT.value,
                               VkChatEventType.USER_KICKED.value,
                               VkChatEventType.ADMIN_REMOVED.value]:
             self.info = {'user_id': self.info}
 
 
 class LongPoll:
-    def __init__(self, vk:Vk, wait:int=25, mode:int=2, v:int=3) -> None:
+    def __init__(self, vk:Vk, _wait:int=25, _mode:int=2, _v:int=3) -> None:
         self._vk = vk
-        self._api = vk.get_api()
-        self._wait = wait
-        self._mode = mode
-        self._v = v
-        self.params = None
-
-        self.updates = []
+        self._wait = _wait
+        self._mode = _mode
+        self._v = _v
+        self._params = {}
+        self._server = ''
+        self._updates = []
 
     async def listen(self):
         while 1:
             async for event in LongPoll(self._vk, self._wait, self._mode, self._v):
                 yield event 
 
     async def get_event(self, url:str, params:dict) -> dict:
         r = await self._vk.client.get(url=url, params=params)
         r = await r.json()
         return r
 
+    async def _update_params(self) -> None:
+        r = await self._vk.messages.getLongPollServer(lp_version=self._v)
+        self._params = {'key': r.key, 'ts': r.ts,
+                        'wait': self._wait, 'mode': self._mode,
+                       'version': self._v, 'act': 'a_check'}
+        self._server = 'https://'+r.server
+
+    async def _get_event(self) -> list:
+        r = await self.get_event(url=self._server, params=self._params)
+        try:
+            updates:list = r['updates']
+            self._params.update({'ts': r['ts']})
+            return updates
+        except IndexError:
+            error = r['failed']
+            if error == 1:
+                self._params.update({'ts': r['ts']})
+            elif error in (2,3):
+                self._params.clear()
+            elif error == 4:
+                self._params.update({'v': r['min_version']})
+            updates = []
+
+            return updates
+        except Exception as e:
+            raise e
+
     # Что происходит дальше?
     # __aiter__ возвращает коду `async for e in LongPoll.listem()`
     # функцию __anext__.
     # Она же в свою очередь просто получает наш новый ивент
 
     def __aiter__(self): return self
 
     async def __anext__(self) -> Event:
-        if not self.params: 
-            r = await self._api.messages.getLongPollServer(lp_version=self._v)
-            self.params = {'key': r.key, 'ts': r.ts,
-                           'wait': self._wait, 'mode': self._mode,
-                           'version': self._v, 'act': 'a_check'}
-            self.server = 'https://'+r.server
+        if self._params == {}: 
+            await self._update_params()
 
-        if self.updates != []:
-            u = self.updates.pop(0)
+        if self._updates != []:
+            u = self._updates.pop(0)
             return Event(u)
-            
-        r = await self.get_event(url=self.server, params=self.params)
-        try:
-            updates = r['updates']
-        except IndexError:
-            error = r['failed']
-            if error == 1:
-                self.params.update({'ts': r['ts']})
-            elif error in (2,3):
-                self.params = {}
-            updates = [[0]]
-        except Exception as e:
-            raise e
-
+        
+        updates = []
+        while updates == []:
+            updates = await self._get_event()
+        
         if len(updates) > 0:
-            self.updates = updates[1:]
+            self._updates = updates[1:]
             update = updates[0]
         else:
             update = updates
-        self.params.update({'ts': r['ts']})
         return Event(update)
 
 
 __all__ = ("Event", "LongPoll")
```

### Comparing `kavk_api-0.9.7.3/kavk_api/types/base.py` & `kavk_api-0.9.7.4/kavk_api/types/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from enum import Enum
-from typing import Any, Callable
+from typing import Any, TypeVar
 from pydantic import BaseModel as BM
 
-class MethodTypeHandlerException(Exception):
+T = TypeVar('T')
+
+class GetResponseHandlerException(Exception):
     def __init__(self, response:dict, responses_handlers:list):
         self.response = response
         self.responses_handlers = responses_handlers
 
     def __str__(self) -> str:
         return (f'It is not possible to process the response with handlers: {self.responses_handlers}\n' +
                 f'response: {self.response}')
@@ -17,24 +19,28 @@
 
     async def _method(self, method:str, **params):
         try:
             params.pop('self')
         except: pass
         return await self.vk.call_method(method, **params)
 
-    def _type_handler(self, response:Any, response_handlers:list[Callable]):
-        for response_handler in response_handlers:
-            try: return response_handler(**response)
-            except:
-                try: return response_handler.parse_obj(response)
-                except: 
-                    try: return response_handler(response)
-                    except: raise MethodTypeHandlerException(response, response_handlers)
-
-
+class Int:
+    @classmethod
+    def parse_obj(cls, obj:int):
+        return int(obj)
+
+class Bool:
+    @classmethod
+    def parse_obj(cls, obj:bool):
+        return bool(obj)
+
+class Str:
+    @classmethod
+    def parse_obj(cls, obj:str):
+        return str(obj)
 
 class BaseList(BM):
     __root__:list
 
     def __iter__(self):
         return iter(self.__root__)
```

### Comparing `kavk_api-0.9.7.3/kavk_api/types/bot_events.py` & `kavk_api-0.9.7.4/kavk_api/types/bot_events.py`

 * *Files identical despite different names*

### Comparing `kavk_api-0.9.7.3/kavk_api/types/event_objects.py` & `kavk_api-0.9.7.4/kavk_api/types/event_objects.py`

 * *Files identical despite different names*

### Comparing `kavk_api-0.9.7.3/kavk_api/types/objects.py` & `kavk_api-0.9.7.4/kavk_api/types/objects.py`

 * *Files identical despite different names*

### Comparing `kavk_api-0.9.7.3/kavk_api/types/responses.py` & `kavk_api-0.9.7.4/kavk_api/types/responses.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from .objects import *
-from .base import BM
+from .base import BM, Int, Bool, Str
 from .base import BaseList as BL
 
 class AccountChangePasswordResponse(BM):
 	token:str
 	secret:str
 
 class AccountGetActiveOffersResponse(BM):
 	count:int
 	items:list[AccountOffer]
 
-AccountGetAppPermissionsResponse = int
+AccountGetAppPermissionsResponse = Int
 
 class AccountGetBannedResponse(BM):
 	count:int
 	items:list[int]
 	profiles:list[UsersUserFull]
 	groups:list[GroupsGroup]
 
@@ -27,15 +27,15 @@
 AccountGetPushSettingsResponse = AccountPushSettings
 
 class AccountSaveProfileInfoResponse(BM):
 	changed:bool
 	name_request:AccountNameRequest
 
 
-AdsAddOfficeUsersResponse = bool
+AdsAddOfficeUsersResponse = Bool
 
 AdsCheckLinkResponse = AdsLinkStatus
 
 class AdsCreateAdsResponse(BL):
 	__root__:list[AdsCreateAdStatus]
 
 class AdsCreateCampaignsResponse(BL):
@@ -65,15 +65,15 @@
 
 class AdsGetAdsTargetingResponse(BL):
 	__root__:list[AdsTargSettings]
 
 class AdsGetAdsResponse(BL):
 	__root__:list[AdsAd]
 
-AdsGetBudgetResponse = int
+AdsGetBudgetResponse = Int
 
 class AdsGetCampaignsResponse(BL):
 	__root__:list[AdsCampaign]
 
 class AdsGetCategoriesResponse(BM):
 	v1:list[AdsCategory]
 	v2:list[AdsCategory]
@@ -117,28 +117,28 @@
 	__root__:list[AdsTargSuggestionsSchools]
 
 class AdsGetTargetGroupsResponse(BL):
 	__root__:list[AdsTargetGroup]
 
 AdsGetTargetingStatsResponse = AdsTargStats
 
-AdsGetUploadURLResponse = str
+AdsGetUploadURLResponse = Str
 
-AdsGetVideoUploadURLResponse = str
+AdsGetVideoUploadURLResponse = Str
 
-AdsImportTargetContactsResponse = int
+AdsImportTargetContactsResponse = Int
 
-AdsRemoveOfficeUsersResponse = bool
+AdsRemoveOfficeUsersResponse = Bool
 
 class AdsUpdateAdsResponse(BL):
 	__root__:list[int]
 
-AdsUpdateCampaignsResponse = int
+AdsUpdateCampaignsResponse = Int
 
-AdsUpdateClientsResponse = int
+AdsUpdateClientsResponse = Int
 
 class AdsUpdateOfficeUsersResponse(BL):
 	__root__:list[AdsUpdateOfficeUsersResult]
 
 
 class AdswebGetAdCategoriesResponse(BM):
 	categories:list[AdswebGetAdCategoriesResponseCategoriesCategory]
@@ -204,42 +204,42 @@
 	privacy_policy:str
 	terms:str
 
 class AppsGetScopesResponse(BM):
 	count:int
 	items:list[AppsScope]
 
-AppsGetScoreResponse = int
+AppsGetScoreResponse = Int
 
 class AppsGetResponse(BM):
 	count:int
 	items:list[AppsApp]
 
 class AppsImageUploadResponse(BM):
 	hash:str
 	image:str
 
-AppsSendRequestResponse = int
+AppsSendRequestResponse = Int
 
 
 class AuthRestoreResponse(BM):
 	success:int
 	sid:str
 
 
-BaseBoolResponse = bool
+BaseBoolResponse = Bool
 
 BaseGetUploadServerResponse = BaseUploadServer
 
-BaseOkResponse = int
+BaseOkResponse = Int
 
 
-BoardAddTopicResponse = int
+BoardAddTopicResponse = Int
 
-BoardCreateCommentResponse = int
+BoardCreateCommentResponse = Int
 
 class BoardGetCommentsExtendedResponse(BM):
 	count:int
 	items:list[BoardTopicComment]
 	poll:object
 	profiles:list[UsersUserFull]
 	groups:list[GroupsGroupFull]
@@ -307,15 +307,15 @@
 	items:list[DatabaseSchool]
 
 class DatabaseGetUniversitiesResponse(BM):
 	count:int
 	items:list[DatabaseUniversity]
 
 
-DocsAddResponse = int
+DocsAddResponse = Int
 
 class DocsDocUploadResponse(BM):
 	file:str
 
 class DocsGetByIdResponse(BL):
 	__root__:list[DocsDoc]
 
@@ -373,15 +373,15 @@
 	count:int
 	items:list[FaveBookmark]
 
 
 class FriendsAddListResponse(BM):
 	list_id:int
 
-FriendsAddResponse = int
+FriendsAddResponse = Int
 
 class FriendsAreFriendsExtendedResponse(BL):
 	__root__:list[FriendsFriendExtendedStatus]
 
 class FriendsAreFriendsResponse(BL):
 	__root__:list[FriendsFriendStatus]
 
@@ -597,15 +597,15 @@
 class GroupsIsMemberExtendedResponse(BM):
 	member:bool
 	invitation:bool
 	can_invite:bool
 	can_recall:bool
 	request:bool
 
-GroupsIsMemberResponse = bool
+GroupsIsMemberResponse = Bool
 
 class GroupsIsMemberUserIdsExtendedResponse(BL):
 	__root__:list[GroupsMemberStatusFull]
 
 class GroupsIsMemberUserIdsResponse(BL):
 	__root__:list[GroupsMemberStatus]
 
@@ -626,15 +626,15 @@
 	next_page_token:str
 
 LeadFormsGetResponse = LeadFormsForm
 
 class LeadFormsListResponse(BL):
 	__root__:list[LeadFormsForm]
 
-LeadFormsUploadUrlResponse = str
+LeadFormsUploadUrlResponse = Str
 
 
 class LikesAddResponse(BM):
 	likes:int
 
 class LikesDeleteResponse(BM):
 	likes:int
@@ -655,17 +655,17 @@
 class MarketAddAlbumResponse(BM):
 	market_album_id:int
 	albums_count:int
 
 class MarketAddResponse(BM):
 	market_item_id:int
 
-MarketCreateCommentResponse = int
+MarketCreateCommentResponse = Int
 
-MarketDeleteCommentResponse = bool
+MarketDeleteCommentResponse = Bool
 
 class MarketGetAlbumByIdResponse(BM):
 	count:int
 	items:list[MarketMarketAlbum]
 
 class MarketGetAlbumsResponse(BM):
 	count:int
@@ -716,15 +716,15 @@
 	variants:list[MarketMarketItemFull]
 
 class MarketGetResponse(BM):
 	count:int
 	items:list[MarketMarketItem]
 	variants:list[MarketMarketItem]
 
-MarketRestoreCommentResponse = bool
+MarketRestoreCommentResponse = Bool
 
 class MarketSearchExtendedResponse(BM):
 	count:int
 	view_type:MarketServicesViewType
 	items:list[MarketMarketItemFull]
 	variants:list[MarketMarketItemFull]
 
@@ -732,26 +732,26 @@
 	count:int
 	view_type:MarketServicesViewType
 	items:list[MarketMarketItem]
 	variants:list[MarketMarketItem]
 	groups:list[GroupsGroupFull]
 
 
-MessagesCreateChatResponse = int
+MessagesCreateChatResponse = Int
 
 class MessagesDeleteChatPhotoResponse(BM):
 	message_id:int
 	chat:MessagesChat
 
 class MessagesDeleteConversationResponse(BM):
 	last_deleted_id:int
 
-MessagesDeleteResponse = bool
+MessagesDeleteResponse = Bool
 
-MessagesEditResponse = bool
+MessagesEditResponse = Bool
 
 class MessagesGetByConversationMessageIdExtendedResponse(BM):
 	count:int
 	items:list[MessagesMessage]
 	profiles:list[UsersUserFull]
 	groups:list[GroupsGroupFull]
 
@@ -878,15 +878,15 @@
 	groups:list[GroupsGroupFull]
 	conversations:list[MessagesConversation]
 
 class MessagesSearchResponse(BM):
 	count:int
 	items:list[MessagesMessage]
 
-MessagesSendResponse = int
+MessagesSendResponse = Int
 
 class MessagesSendUserIdsResponse(BL):
 	__root__:list[MessagesSendUserIdsResponseItem]
 
 class MessagesSetChatPhotoResponse(BM):
 	message_id:int
 	chat:MessagesChat
@@ -927,15 +927,15 @@
 class NewsfeedGetSuggestedSourcesResponse(BM):
 	count:int
 	items:list[UsersSubscriptionsItem]
 
 class NewsfeedIgnoreItemResponse(BM):
 	status:bool
 
-NewsfeedSaveListResponse = int
+NewsfeedSaveListResponse = Int
 
 class NewsfeedSearchExtendedResponse(BM):
 	items:list[WallWallpostFull]
 	profiles:list[UsersUserFull]
 	groups:list[GroupsGroupFull]
 	suggested_queries:list[str]
 	next_from:str
@@ -946,17 +946,17 @@
 	items:list[WallWallpostFull]
 	suggested_queries:list[str]
 	next_from:str
 	count:int
 	total_count:int
 
 
-NotesAddResponse = int
+NotesAddResponse = Int
 
-NotesCreateCommentResponse = int
+NotesCreateCommentResponse = Int
 
 NotesGetByIdResponse = NotesNote
 
 class NotesGetCommentsResponse(BM):
 	count:int
 	items:list[NotesNoteComment]
 
@@ -973,23 +973,23 @@
 	last_viewed:int
 	photos:list[PhotosPhoto]
 	videos:list[VideoVideo]
 	apps:list[AppsApp]
 	next_from:str
 	ttl:int
 
-NotificationsMarkAsViewedResponse = bool
+NotificationsMarkAsViewedResponse = Bool
 
 class NotificationsSendMessageResponse(BL):
 	__root__:list[NotificationsSendMessageItem]
 
 
-OrdersCancelSubscriptionResponse = bool
+OrdersCancelSubscriptionResponse = Bool
 
-OrdersChangeStateResponse = str
+OrdersChangeStateResponse = Str
 
 class OrdersGetAmountResponse(BL):
 	__root__:list[OrdersAmount]
 
 class OrdersGetByIdResponse(BL):
 	__root__:list[OrdersOrder]
 
@@ -998,43 +998,43 @@
 class OrdersGetUserSubscriptionsResponse(BM):
 	count:int
 	items:list[OrdersSubscription]
 
 class OrdersGetResponse(BL):
 	__root__:list[OrdersOrder]
 
-OrdersUpdateSubscriptionResponse = bool
+OrdersUpdateSubscriptionResponse = Bool
 
 
 class PagesGetHistoryResponse(BL):
 	__root__:list[PagesWikipageHistory]
 
 class PagesGetTitlesResponse(BL):
 	__root__:list[PagesWikipage]
 
 PagesGetVersionResponse = PagesWikipageFull
 
 PagesGetResponse = PagesWikipageFull
 
-PagesParseWikiResponse = str
+PagesParseWikiResponse = Str
 
-PagesSaveAccessResponse = int
+PagesSaveAccessResponse = Int
 
-PagesSaveResponse = int
+PagesSaveResponse = Int
 
 
-PhotosCopyResponse = int
+PhotosCopyResponse = Int
 
 PhotosCreateAlbumResponse = PhotosPhotoAlbumFull
 
-PhotosCreateCommentResponse = int
+PhotosCreateCommentResponse = Int
 
-PhotosDeleteCommentResponse = bool
+PhotosDeleteCommentResponse = Bool
 
-PhotosGetAlbumsCountResponse = int
+PhotosGetAlbumsCountResponse = Int
 
 class PhotosGetAlbumsResponse(BM):
 	count:int
 	items:list[PhotosPhotoAlbumFull]
 
 class PhotosGetAllCommentsResponse(BM):
 	count:int
@@ -1119,17 +1119,17 @@
 class PhotosPhotoUploadResponse(BM):
 	aid:int
 	hash:str
 	photo:str
 	photos_list:str
 	server:int
 
-PhotosPutTagResponse = int
+PhotosPutTagResponse = Int
 
-PhotosRestoreCommentResponse = bool
+PhotosRestoreCommentResponse = Bool
 
 class PhotosSaveMarketAlbumPhotoResponse(BL):
 	__root__:list[PhotosPhoto]
 
 class PhotosSaveMarketPhotoResponse(BL):
 	__root__:list[PhotosPhoto]
 
@@ -1164,19 +1164,19 @@
 
 
 class PodcastsSearchPodcastResponse(BM):
 	podcasts:list[PodcastExternalData]
 	results_total:int
 
 
-PollsAddVoteResponse = bool
+PollsAddVoteResponse = Bool
 
 PollsCreateResponse = PollsPoll
 
-PollsDeleteVoteResponse = bool
+PollsDeleteVoteResponse = Bool
 
 class PollsGetBackgroundsResponse(BL):
 	__root__:list[PollsBackground]
 
 PollsGetByIdResponse = PollsPoll
 
 class PollsGetVotersResponse(BL):
@@ -1197,30 +1197,30 @@
 class PrettyCardsEditResponse(BM):
 	owner_id:int
 	card_id:str
 
 class PrettyCardsGetByIdResponse(BL):
 	__root__:list[PrettyCardsPrettyCardOrError]
 
-PrettyCardsGetUploadURLResponse = str
+PrettyCardsGetUploadURLResponse = Str
 
 class PrettyCardsGetResponse(BM):
 	count:int
 	items:list[PrettyCardsPrettyCard]
 
 
 class SearchGetHintsResponse(BM):
 	count:int
 	items:list[SearchHint]
 	suggested_queries:list[str]
 
 
 SecureCheckTokenResponse = SecureTokenChecked
 
-SecureGetAppBalanceResponse = int
+SecureGetAppBalanceResponse = Int
 
 class SecureGetSMSHistoryResponse(BL):
 	__root__:list[SecureSmsNotification]
 
 class SecureGetTransactionsHistoryResponse(BL):
 	__root__:list[SecureTransaction]
 
@@ -1363,28 +1363,28 @@
 	count:int
 	items:list[UtilsLastShortenedLink]
 
 UtilsGetLinkStatsExtendedResponse = UtilsLinkStatsExtended
 
 UtilsGetLinkStatsResponse = UtilsLinkStats
 
-UtilsGetServerTimeResponse = int
+UtilsGetServerTimeResponse = Int
 
 UtilsGetShortLinkResponse = UtilsShortLink
 
 UtilsResolveScreenNameResponse = UtilsDomainResolved
 
 
 class VideoAddAlbumResponse(BM):
 	album_id:int
 
 class VideoChangeVideoAlbumsResponse(BL):
 	__root__:list[int]
 
-VideoCreateCommentResponse = int
+VideoCreateCommentResponse = Int
 
 VideoGetAlbumByIdResponse = VideoVideoAlbumFull
 
 class VideoGetAlbumsByVideoExtendedResponse(BM):
 	count:int
 	items:list[VideoVideoAlbumFull]
 
@@ -1421,15 +1421,15 @@
 
 class VideoGetResponse(BM):
 	count:int
 	items:list[VideoVideoFull]
 	profiles:list[UsersUserFull]
 	groups:list[GroupsGroupFull]
 
-VideoRestoreCommentResponse = bool
+VideoRestoreCommentResponse = Bool
 
 VideoSaveResponse = VideoSaveResult
 
 class VideoSearchExtendedResponse(BM):
 	count:int
 	items:list[VideoVideoFull]
 	profiles:list[UsersUser]
@@ -1532,8 +1532,8 @@
 	posts:list[WidgetsWidgetComment]
 
 class WidgetsGetPagesResponse(BM):
 	count:int
 	pages:list[WidgetsWidgetPage]
 
 
-__all__ = ('AccountChangePasswordResponse', 'AccountGetActiveOffersResponse', 'AccountGetAppPermissionsResponse', 'AccountGetBannedResponse', 'AccountGetCountersResponse', 'AccountGetInfoResponse', 'AccountGetProfileInfoResponse', 'AccountGetPushSettingsResponse', 'AccountSaveProfileInfoResponse', 'AdsAddOfficeUsersResponse', 'AdsCheckLinkResponse', 'AdsCreateAdsResponse', 'AdsCreateCampaignsResponse', 'AdsCreateClientsResponse', 'AdsCreateTargetGroupResponse', 'AdsDeleteAdsResponse', 'AdsDeleteCampaignsResponse', 'AdsDeleteClientsResponse', 'AdsGetAccountsResponse', 'AdsGetAdsLayoutResponse', 'AdsGetAdsTargetingResponse', 'AdsGetAdsResponse', 'AdsGetBudgetResponse', 'AdsGetCampaignsResponse', 'AdsGetCategoriesResponse', 'AdsGetClientsResponse', 'AdsGetDemographicsResponse', 'AdsGetFloodStatsResponse', 'AdsGetLookalikeRequestsResponse', 'AdsGetMusiciansResponse', 'AdsGetOfficeUsersResponse', 'AdsGetPostsReachResponse', 'AdsGetRejectionReasonResponse', 'AdsGetStatisticsResponse', 'AdsGetSuggestionsCitiesResponse', 'AdsGetSuggestionsRegionsResponse', 'AdsGetSuggestionsResponse', 'AdsGetSuggestionsSchoolsResponse', 'AdsGetTargetGroupsResponse', 'AdsGetTargetingStatsResponse', 'AdsGetUploadURLResponse', 'AdsGetVideoUploadURLResponse', 'AdsImportTargetContactsResponse', 'AdsRemoveOfficeUsersResponse', 'AdsUpdateAdsResponse', 'AdsUpdateCampaignsResponse', 'AdsUpdateClientsResponse', 'AdsUpdateOfficeUsersResponse', 'AdswebGetAdCategoriesResponse', 'AdswebGetAdUnitCodeResponse', 'AdswebGetAdUnitsResponse', 'AdswebGetFraudHistoryResponse', 'AdswebGetSitesResponse', 'AdswebGetStatisticsResponse', 'AppWidgetsGetAppImageUploadServerResponse', 'AppWidgetsGetAppImagesResponse', 'AppWidgetsGetGroupImageUploadServerResponse', 'AppWidgetsGetGroupImagesResponse', 'AppWidgetsGetImagesByIdResponse', 'AppWidgetsSaveAppImageResponse', 'AppWidgetsSaveGroupImageResponse', 'AppsGetCatalogResponse', 'AppsGetFriendsListExtendedResponse', 'AppsGetFriendsListResponse', 'AppsGetLeaderboardExtendedResponse', 'AppsGetLeaderboardResponse', 'AppsGetMiniAppPoliciesResponse', 'AppsGetScopesResponse', 'AppsGetScoreResponse', 'AppsGetResponse', 'AppsImageUploadResponse', 'AppsSendRequestResponse', 'AuthRestoreResponse', 'BaseBoolResponse', 'BaseGetUploadServerResponse', 'BaseOkResponse', 'BoardAddTopicResponse', 'BoardCreateCommentResponse', 'BoardGetCommentsExtendedResponse', 'BoardGetCommentsResponse', 'BoardGetTopicsExtendedResponse', 'BoardGetTopicsResponse', 'DatabaseGetChairsResponse', 'DatabaseGetCitiesByIdResponse', 'DatabaseGetCitiesResponse', 'DatabaseGetCountriesByIdResponse', 'DatabaseGetCountriesResponse', 'DatabaseGetFacultiesResponse', 'DatabaseGetMetroStationsByIdResponse', 'DatabaseGetMetroStationsResponse', 'DatabaseGetRegionsResponse', 'DatabaseGetSchoolClassesResponse', 'DatabaseGetSchoolsResponse', 'DatabaseGetUniversitiesResponse', 'DocsAddResponse', 'DocsDocUploadResponse', 'DocsGetByIdResponse', 'DocsGetTypesResponse', 'DocsGetUploadServerResponse', 'DocsGetResponse', 'DocsSaveResponse', 'DocsSearchResponse', 'DonutGetSubscriptionResponse', 'DonutGetSubscriptionsResponse', 'DownloadedGamesPaidStatusResponse', 'FaveAddTagResponse', 'FaveGetPagesResponse', 'FaveGetTagsResponse', 'FaveGetExtendedResponse', 'FaveGetResponse', 'FriendsAddListResponse', 'FriendsAddResponse', 'FriendsAreFriendsExtendedResponse', 'FriendsAreFriendsResponse', 'FriendsDeleteResponse', 'FriendsGetAppUsersResponse', 'FriendsGetByPhonesResponse', 'FriendsGetListsResponse', 'FriendsGetMutualResponse', 'FriendsGetMutualTargetUidsResponse', 'FriendsGetOnlineOnlineMobileResponse', 'FriendsGetOnlineResponse', 'FriendsGetRecentResponse', 'FriendsGetRequestsExtendedResponse', 'FriendsGetRequestsNeedMutualResponse', 'FriendsGetRequestsResponse', 'FriendsGetSuggestionsResponse', 'FriendsGetFieldsResponse', 'FriendsGetResponse', 'FriendsSearchResponse', 'GiftsGetResponse', 'GroupsAddAddressResponse', 'GroupsAddCallbackServerResponse', 'GroupsAddLinkResponse', 'GroupsCreateResponse', 'GroupsEditAddressResponse', 'GroupsGetAddressesResponse', 'GroupsGetBannedResponse', 'GroupsGetByIdObjectLegacyResponse', 'GroupsGetCallbackConfirmationCodeResponse', 'GroupsGetCallbackServersResponse', 'GroupsGetCallbackSettingsResponse', 'GroupsGetCatalogInfoExtendedResponse', 'GroupsGetCatalogInfoResponse', 'GroupsGetCatalogResponse', 'GroupsGetInvitedUsersResponse', 'GroupsGetInvitesExtendedResponse', 'GroupsGetInvitesResponse', 'GroupsGetLongPollServerResponse', 'GroupsGetLongPollSettingsResponse', 'GroupsGetMembersFieldsResponse', 'GroupsGetMembersFilterResponse', 'GroupsGetMembersResponse', 'GroupsGetRequestsFieldsResponse', 'GroupsGetRequestsResponse', 'GroupsGetSettingsResponse', 'GroupsGetTagListResponse', 'GroupsGetTokenPermissionsResponse', 'GroupsGetObjectExtendedResponse', 'GroupsGetResponse', 'GroupsIsMemberExtendedResponse', 'GroupsIsMemberResponse', 'GroupsIsMemberUserIdsExtendedResponse', 'GroupsIsMemberUserIdsResponse', 'GroupsSearchResponse', 'LeadFormsCreateResponse', 'LeadFormsDeleteResponse', 'LeadFormsGetLeadsResponse', 'LeadFormsGetResponse', 'LeadFormsListResponse', 'LeadFormsUploadUrlResponse', 'LikesAddResponse', 'LikesDeleteResponse', 'LikesGetListExtendedResponse', 'LikesGetListResponse', 'LikesIsLikedResponse', 'MarketAddAlbumResponse', 'MarketAddResponse', 'MarketCreateCommentResponse', 'MarketDeleteCommentResponse', 'MarketGetAlbumByIdResponse', 'MarketGetAlbumsResponse', 'MarketGetByIdExtendedResponse', 'MarketGetByIdResponse', 'MarketGetCategoriesNewResponse', 'MarketGetCategoriesResponse', 'MarketGetCommentsResponse', 'MarketGetGroupOrdersResponse', 'MarketGetOrderByIdResponse', 'MarketGetOrderItemsResponse', 'MarketGetOrdersExtendedResponse', 'MarketGetOrdersResponse', 'MarketGetExtendedResponse', 'MarketGetResponse', 'MarketRestoreCommentResponse', 'MarketSearchExtendedResponse', 'MarketSearchResponse', 'MessagesCreateChatResponse', 'MessagesDeleteChatPhotoResponse', 'MessagesDeleteConversationResponse', 'MessagesDeleteResponse', 'MessagesEditResponse', 'MessagesGetByConversationMessageIdExtendedResponse', 'MessagesGetByConversationMessageIdResponse', 'MessagesGetByIdExtendedResponse', 'MessagesGetByIdResponse', 'MessagesGetChatPreviewResponse', 'MessagesGetChatChatIdsFieldsResponse', 'MessagesGetChatChatIdsResponse', 'MessagesGetChatFieldsResponse', 'MessagesGetChatResponse', 'MessagesGetConversationMembersResponse', 'MessagesGetConversationsByIdExtendedResponse', 'MessagesGetConversationsByIdResponse', 'MessagesGetConversationsResponse', 'MessagesGetHistoryAttachmentsResponse', 'MessagesGetHistoryExtendedResponse', 'MessagesGetHistoryResponse', 'MessagesGetImportantMessagesExtendedResponse', 'MessagesGetImportantMessagesResponse', 'MessagesGetIntentUsersResponse', 'MessagesGetInviteLinkResponse', 'MessagesGetLastActivityResponse', 'MessagesGetLongPollHistoryResponse', 'MessagesGetLongPollServerResponse', 'MessagesIsMessagesFromGroupAllowedResponse', 'MessagesJoinChatByInviteLinkResponse', 'MessagesMarkAsImportantResponse', 'MessagesPinResponse', 'MessagesSearchConversationsExtendedResponse', 'MessagesSearchConversationsResponse', 'MessagesSearchExtendedResponse', 'MessagesSearchResponse', 'MessagesSendResponse', 'MessagesSendUserIdsResponse', 'MessagesSetChatPhotoResponse', 'NewsfeedGenericResponse', 'NewsfeedGetBannedExtendedResponse', 'NewsfeedGetBannedResponse', 'NewsfeedGetCommentsResponse', 'NewsfeedGetListsExtendedResponse', 'NewsfeedGetListsResponse', 'NewsfeedGetMentionsResponse', 'NewsfeedGetSuggestedSourcesResponse', 'NewsfeedIgnoreItemResponse', 'NewsfeedSaveListResponse', 'NewsfeedSearchExtendedResponse', 'NewsfeedSearchResponse', 'NotesAddResponse', 'NotesCreateCommentResponse', 'NotesGetByIdResponse', 'NotesGetCommentsResponse', 'NotesGetResponse', 'NotificationsGetResponse', 'NotificationsMarkAsViewedResponse', 'NotificationsSendMessageResponse', 'OrdersCancelSubscriptionResponse', 'OrdersChangeStateResponse', 'OrdersGetAmountResponse', 'OrdersGetByIdResponse', 'OrdersGetUserSubscriptionByIdResponse', 'OrdersGetUserSubscriptionsResponse', 'OrdersGetResponse', 'OrdersUpdateSubscriptionResponse', 'PagesGetHistoryResponse', 'PagesGetTitlesResponse', 'PagesGetVersionResponse', 'PagesGetResponse', 'PagesParseWikiResponse', 'PagesSaveAccessResponse', 'PagesSaveResponse', 'PhotosCopyResponse', 'PhotosCreateAlbumResponse', 'PhotosCreateCommentResponse', 'PhotosDeleteCommentResponse', 'PhotosGetAlbumsCountResponse', 'PhotosGetAlbumsResponse', 'PhotosGetAllCommentsResponse', 'PhotosGetAllExtendedResponse', 'PhotosGetAllResponse', 'PhotosGetByIdResponse', 'PhotosGetCommentsExtendedResponse', 'PhotosGetCommentsResponse', 'PhotosGetMarketUploadServerResponse', 'PhotosGetMessagesUploadServerResponse', 'PhotosGetNewTagsResponse', 'PhotosGetTagsResponse', 'PhotosGetUploadServerResponse', 'PhotosGetUserPhotosResponse', 'PhotosGetWallUploadServerResponse', 'PhotosGetResponse', 'PhotosMarketAlbumUploadResponse', 'PhotosMarketUploadResponse', 'PhotosMessageUploadResponse', 'PhotosOwnerCoverUploadResponse', 'PhotosOwnerUploadResponse', 'PhotosPhotoUploadResponse', 'PhotosPutTagResponse', 'PhotosRestoreCommentResponse', 'PhotosSaveMarketAlbumPhotoResponse', 'PhotosSaveMarketPhotoResponse', 'PhotosSaveMessagesPhotoResponse', 'PhotosSaveOwnerCoverPhotoResponse', 'PhotosSaveOwnerPhotoResponse', 'PhotosSaveWallPhotoResponse', 'PhotosSaveResponse', 'PhotosSearchResponse', 'PhotosWallUploadResponse', 'PodcastsSearchPodcastResponse', 'PollsAddVoteResponse', 'PollsCreateResponse', 'PollsDeleteVoteResponse', 'PollsGetBackgroundsResponse', 'PollsGetByIdResponse', 'PollsGetVotersResponse', 'PollsSavePhotoResponse', 'PrettyCardsCreateResponse', 'PrettyCardsDeleteResponse', 'PrettyCardsEditResponse', 'PrettyCardsGetByIdResponse', 'PrettyCardsGetUploadURLResponse', 'PrettyCardsGetResponse', 'SearchGetHintsResponse', 'SecureCheckTokenResponse', 'SecureGetAppBalanceResponse', 'SecureGetSMSHistoryResponse', 'SecureGetTransactionsHistoryResponse', 'SecureGetUserLevelResponse', 'SecureGiveEventStickerResponse', 'SecureSendNotificationResponse', 'SecureSetCounterArrayResponse', 'StatsGetPostReachResponse', 'StatsGetResponse', 'StatusGetResponse', 'StorageGetKeysResponse', 'StorageGetResponse', 'StoreGetFavoriteStickersResponse', 'StoreGetProductsResponse', 'StoreGetStickersKeywordsResponse', 'StoriesGetBannedExtendedResponse', 'StoriesGetBannedResponse', 'StoriesGetByIdExtendedResponse', 'StoriesGetPhotoUploadServerResponse', 'StoriesGetStatsResponse', 'StoriesGetVideoUploadServerResponse', 'StoriesGetViewersExtendedV5115Response', 'StoriesGetViewersExtendedResponse', 'StoriesGetV5113Response', 'StoriesGetResponse', 'StoriesSaveResponse', 'StoriesUploadResponse', 'StreamingGetServerUrlResponse', 'UsersGetFollowersFieldsResponse', 'UsersGetFollowersResponse', 'UsersGetSubscriptionsExtendedResponse', 'UsersGetSubscriptionsResponse', 'UsersGetResponse', 'UsersSearchResponse', 'UtilsCheckLinkResponse', 'UtilsGetLastShortenedLinksResponse', 'UtilsGetLinkStatsExtendedResponse', 'UtilsGetLinkStatsResponse', 'UtilsGetServerTimeResponse', 'UtilsGetShortLinkResponse', 'UtilsResolveScreenNameResponse', 'VideoAddAlbumResponse', 'VideoChangeVideoAlbumsResponse', 'VideoCreateCommentResponse', 'VideoGetAlbumByIdResponse', 'VideoGetAlbumsByVideoExtendedResponse', 'VideoGetAlbumsByVideoResponse', 'VideoGetAlbumsExtendedResponse', 'VideoGetAlbumsResponse', 'VideoGetCommentsExtendedResponse', 'VideoGetCommentsResponse', 'VideoGetResponse', 'VideoRestoreCommentResponse', 'VideoSaveResponse', 'VideoSearchExtendedResponse', 'VideoSearchResponse', 'VideoUploadResponse', 'WallCreateCommentResponse', 'WallEditResponse', 'WallGetByIdExtendedResponse', 'WallGetByIdLegacyResponse', 'WallGetByIdResponse', 'WallGetCommentExtendedResponse', 'WallGetCommentResponse', 'WallGetCommentsExtendedResponse', 'WallGetCommentsResponse', 'WallGetRepostsResponse', 'WallGetExtendedResponse', 'WallGetResponse', 'WallPostAdsStealthResponse', 'WallPostResponse', 'WallRepostResponse', 'WallSearchExtendedResponse', 'WallSearchResponse', 'WidgetsGetCommentsResponse', 'WidgetsGetPagesResponse')
+__all__ = ('AccountChangePasswordResponse', 'AccountGetActiveOffersResponse', 'AccountGetAppPermissionsResponse', 'AccountGetBannedResponse', 'AccountGetCountersResponse', 'AccountGetInfoResponse', 'AccountGetProfileInfoResponse', 'AccountGetPushSettingsResponse', 'AccountSaveProfileInfoResponse', 'AdsAddOfficeUsersResponse', 'AdsCheckLinkResponse', 'AdsCreateAdsResponse', 'AdsCreateCampaignsResponse', 'AdsCreateClientsResponse', 'AdsCreateTargetGroupResponse', 'AdsDeleteAdsResponse', 'AdsDeleteCampaignsResponse', 'AdsDeleteClientsResponse', 'AdsGetAccountsResponse', 'AdsGetAdsLayoutResponse', 'AdsGetAdsTargetingResponse', 'AdsGetAdsResponse', 'AdsGetBudgetResponse', 'AdsGetCampaignsResponse', 'AdsGetCategoriesResponse', 'AdsGetClientsResponse', 'AdsGetDemographicsResponse', 'AdsGetFloodStatsResponse', 'AdsGetLookalikeRequestsResponse', 'AdsGetMusiciansResponse', 'AdsGetOfficeUsersResponse', 'AdsGetPostsReachResponse', 'AdsGetRejectionReasonResponse', 'AdsGetStatisticsResponse', 'AdsGetSuggestionsCitiesResponse', 'AdsGetSuggestionsRegionsResponse', 'AdsGetSuggestionsResponse', 'AdsGetSuggestionsSchoolsResponse', 'AdsGetTargetGroupsResponse', 'AdsGetTargetingStatsResponse', 'AdsGetUploadURLResponse', 'AdsGetVideoUploadURLResponse', 'AdsImportTargetContactsResponse', 'AdsRemoveOfficeUsersResponse', 'AdsUpdateAdsResponse', 'AdsUpdateCampaignsResponse', 'AdsUpdateClientsResponse', 'AdsUpdateOfficeUsersResponse', 'AdswebGetAdCategoriesResponse', 'AdswebGetAdUnitCodeResponse', 'AdswebGetAdUnitsResponse', 'AdswebGetFraudHistoryResponse', 'AdswebGetSitesResponse', 'AdswebGetStatisticsResponse', 'AppWidgetsGetAppImageUploadServerResponse', 'AppWidgetsGetAppImagesResponse', 'AppWidgetsGetGroupImageUploadServerResponse', 'AppWidgetsGetGroupImagesResponse', 'AppWidgetsGetImagesByIdResponse', 'AppWidgetsSaveAppImageResponse', 'AppWidgetsSaveGroupImageResponse', 'AppsGetCatalogResponse', 'AppsGetFriendsListExtendedResponse', 'AppsGetFriendsListResponse', 'AppsGetLeaderboardExtendedResponse', 'AppsGetLeaderboardResponse', 'AppsGetMiniAppPoliciesResponse', 'AppsGetScopesResponse', 'AppsGetScoreResponse', 'AppsGetResponse', 'AppsImageUploadResponse', 'AppsSendRequestResponse', 'AuthRestoreResponse', 'BaseBoolResponse', 'BaseGetUploadServerResponse', 'BaseOkResponse', 'BoardAddTopicResponse', 'BoardCreateCommentResponse', 'BoardGetCommentsExtendedResponse', 'BoardGetCommentsResponse', 'BoardGetTopicsExtendedResponse', 'BoardGetTopicsResponse', 'DatabaseGetChairsResponse', 'DatabaseGetCitiesByIdResponse', 'DatabaseGetCitiesResponse', 'DatabaseGetCountriesByIdResponse', 'DatabaseGetCountriesResponse', 'DatabaseGetFacultiesResponse', 'DatabaseGetMetroStationsByIdResponse', 'DatabaseGetMetroStationsResponse', 'DatabaseGetRegionsResponse', 'DatabaseGetSchoolClassesResponse', 'DatabaseGetSchoolsResponse', 'DatabaseGetUniversitiesResponse', 'DocsAddResponse', 'DocsDocUploadResponse', 'DocsGetByIdResponse', 'DocsGetTypesResponse', 'DocsGetUploadServerResponse', 'DocsGetResponse', 'DocsSaveResponse', 'DocsSearchResponse', 'DonutGetSubscriptionResponse', 'DonutGetSubscriptionsResponse', 'DownloadedGamesPaidStatusResponse', 'FaveAddTagResponse', 'FaveGetPagesResponse', 'FaveGetTagsResponse', 'FaveGetExtendedResponse', 'FaveGetResponse', 'FriendsAddListResponse', 'FriendsAddResponse', 'FriendsAreFriendsExtendedResponse', 'FriendsAreFriendsResponse', 'FriendsDeleteResponse', 'FriendsGetAppUsersResponse', 'FriendsGetByPhonesResponse', 'FriendsGetListsResponse', 'FriendsGetMutualResponse', 'FriendsGetMutualTargetUidsResponse', 'FriendsGetOnlineOnlineMobileResponse', 'FriendsGetOnlineResponse', 'FriendsGetRecentResponse', 'FriendsGetRequestsExtendedResponse', 'FriendsGetRequestsNeedMutualResponse', 'FriendsGetRequestsResponse', 'FriendsGetSuggestionsResponse', 'FriendsGetFieldsResponse', 'FriendsGetResponse', 'FriendsSearchResponse', 'GiftsGetResponse', 'GroupsAddAddressResponse', 'GroupsAddCallbackServerResponse', 'GroupsAddLinkResponse', 'GroupsCreateResponse', 'GroupsEditAddressResponse', 'GroupsGetAddressesResponse', 'GroupsGetBannedResponse', 'GroupsGetByIdObjectLegacyResponse', 'GroupsGetCallbackConfirmationCodeResponse', 'GroupsGetCallbackServersResponse', 'GroupsGetCallbackSettingsResponse', 'GroupsGetCatalogInfoExtendedResponse', 'GroupsGetCatalogInfoResponse', 'GroupsGetCatalogResponse', 'GroupsGetInvitedUsersResponse', 'GroupsGetInvitesExtendedResponse', 'GroupsGetInvitesResponse', 'GroupsGetLongPollServerResponse', 'GroupsGetLongPollSettingsResponse', 'GroupsGetMembersFieldsResponse', 'GroupsGetMembersFilterResponse', 'GroupsGetMembersResponse', 'GroupsGetRequestsFieldsResponse', 'GroupsGetRequestsResponse', 'GroupsGetSettingsResponse', 'GroupsGetTagListResponse', 'GroupsGetTokenPermissionsResponse', 'GroupsGetObjectExtendedResponse', 'GroupsGetResponse', 'GroupsIsMemberExtendedResponse', 'GroupsIsMemberResponse', 'GroupsIsMemberUserIdsExtendedResponse', 'GroupsIsMemberUserIdsResponse', 'GroupsSearchResponse', 'LeadFormsCreateResponse', 'LeadFormsDeleteResponse', 'LeadFormsGetLeadsResponse', 'LeadFormsGetResponse', 'LeadFormsListResponse', 'LeadFormsUploadUrlResponse', 'LikesAddResponse', 'LikesDeleteResponse', 'LikesGetListExtendedResponse', 'LikesGetListResponse', 'LikesIsLikedResponse', 'MarketAddAlbumResponse', 'MarketAddResponse', 'MarketCreateCommentResponse', 'MarketDeleteCommentResponse', 'MarketGetAlbumByIdResponse', 'MarketGetAlbumsResponse', 'MarketGetByIdExtendedResponse', 'MarketGetByIdResponse', 'MarketGetCategoriesNewResponse', 'MarketGetCategoriesResponse', 'MarketGetCommentsResponse', 'MarketGetGroupOrdersResponse', 'MarketGetOrderByIdResponse', 'MarketGetOrderItemsResponse', 'MarketGetOrdersExtendedResponse', 'MarketGetOrdersResponse', 'MarketGetExtendedResponse', 'MarketGetResponse', 'MarketRestoreCommentResponse', 'MarketSearchExtendedResponse', 'MarketSearchResponse', 'MessagesCreateChatResponse', 'MessagesDeleteChatPhotoResponse', 'MessagesDeleteConversationResponse', 'MessagesDeleteResponse', 'MessagesEditResponse', 'MessagesGetByConversationMessageIdExtendedResponse', 'MessagesGetByConversationMessageIdResponse', 'MessagesGetByIdExtendedResponse', 'MessagesGetByIdResponse', 'MessagesGetChatPreviewResponse', 'MessagesGetChatChatIdsFieldsResponse', 'MessagesGetChatChatIdsResponse', 'MessagesGetChatFieldsResponse', 'MessagesGetChatResponse', 'MessagesGetConversationMembersResponse', 'MessagesGetConversationsByIdExtendedResponse', 'MessagesGetConversationsByIdResponse', 'MessagesGetConversationsResponse', 'MessagesGetHistoryAttachmentsResponse', 'MessagesGetHistoryExtendedResponse', 'MessagesGetHistoryResponse', 'MessagesGetImportantMessagesExtendedResponse', 'MessagesGetImportantMessagesResponse', 'MessagesGetIntentUsersResponse', 'MessagesGetInviteLinkResponse', 'MessagesGetLastActivityResponse', 'MessagesGetLongPollHistoryResponse', 'MessagesGetLongPollServerResponse', 'MessagesIsMessagesFromGroupAllowedResponse', 'MessagesJoinChatByInviteLinkResponse', 'MessagesMarkAsImportantResponse', 'MessagesPinResponse', 'MessagesSearchConversationsExtendedResponse', 'MessagesSearchConversationsResponse', 'MessagesSearchExtendedResponse', 'MessagesSearchResponse', 'MessagesSendResponse', 'MessagesSendUserIdsResponse', 'MessagesSetChatPhotoResponse', 'NewsfeedGenericResponse', 'NewsfeedGetBannedExtendedResponse', 'NewsfeedGetBannedResponse', 'NewsfeedGetCommentsResponse', 'NewsfeedGetListsExtendedResponse', 'NewsfeedGetListsResponse', 'NewsfeedGetMentionsResponse', 'NewsfeedGetSuggestedSourcesResponse', 'NewsfeedIgnoreItemResponse', 'NewsfeedSaveListResponse', 'NewsfeedSearchExtendedResponse', 'NewsfeedSearchResponse', 'NotesAddResponse', 'NotesCreateCommentResponse', 'NotesGetByIdResponse', 'NotesGetCommentsResponse', 'NotesGetResponse', 'NotificationsGetResponse', 'NotificationsMarkAsViewedResponse', 'NotificationsSendMessageResponse', 'OrdersCancelSubscriptionResponse', 'OrdersChangeStateResponse', 'OrdersGetAmountResponse', 'OrdersGetByIdResponse', 'OrdersGetUserSubscriptionByIdResponse', 'OrdersGetUserSubscriptionsResponse', 'OrdersGetResponse', 'OrdersUpdateSubscriptionResponse', 'PagesGetHistoryResponse', 'PagesGetTitlesResponse', 'PagesGetVersionResponse', 'PagesGetResponse', 'PagesParseWikiResponse', 'PagesSaveAccessResponse', 'PagesSaveResponse', 'PhotosCopyResponse', 'PhotosCreateAlbumResponse', 'PhotosCreateCommentResponse', 'PhotosDeleteCommentResponse', 'PhotosGetAlbumsCountResponse', 'PhotosGetAlbumsResponse', 'PhotosGetAllCommentsResponse', 'PhotosGetAllExtendedResponse', 'PhotosGetAllResponse', 'PhotosGetByIdResponse', 'PhotosGetCommentsExtendedResponse', 'PhotosGetCommentsResponse', 'PhotosGetMarketUploadServerResponse', 'PhotosGetMessagesUploadServerResponse', 'PhotosGetNewTagsResponse', 'PhotosGetTagsResponse', 'PhotosGetUploadServerResponse', 'PhotosGetUserPhotosResponse', 'PhotosGetWallUploadServerResponse', 'PhotosGetResponse', 'PhotosMarketAlbumUploadResponse', 'PhotosMarketUploadResponse', 'PhotosMessageUploadResponse', 'PhotosOwnerCoverUploadResponse', 'PhotosOwnerUploadResponse', 'PhotosPhotoUploadResponse', 'PhotosPutTagResponse', 'PhotosRestoreCommentResponse', 'PhotosSaveMarketAlbumPhotoResponse', 'PhotosSaveMarketPhotoResponse', 'PhotosSaveMessagesPhotoResponse', 'PhotosSaveOwnerCoverPhotoResponse', 'PhotosSaveOwnerPhotoResponse', 'PhotosSaveWallPhotoResponse', 'PhotosSaveResponse', 'PhotosSearchResponse', 'PhotosWallUploadResponse', 'PodcastsSearchPodcastResponse', 'PollsAddVoteResponse', 'PollsCreateResponse', 'PollsDeleteVoteResponse', 'PollsGetBackgroundsResponse', 'PollsGetByIdResponse', 'PollsGetVotersResponse', 'PollsSavePhotoResponse', 'PrettyCardsCreateResponse', 'PrettyCardsDeleteResponse', 'PrettyCardsEditResponse', 'PrettyCardsGetByIdResponse', 'PrettyCardsGetUploadURLResponse', 'PrettyCardsGetResponse', 'SearchGetHintsResponse', 'SecureCheckTokenResponse', 'SecureGetAppBalanceResponse', 'SecureGetSMSHistoryResponse', 'SecureGetTransactionsHistoryResponse', 'SecureGetUserLevelResponse', 'SecureGiveEventStickerResponse', 'SecureSendNotificationResponse', 'SecureSetCounterArrayResponse', 'StatsGetPostReachResponse', 'StatsGetResponse', 'StatusGetResponse', 'StorageGetKeysResponse', 'StorageGetResponse', 'StoreGetFavoriteStickersResponse', 'StoreGetProductsResponse', 'StoreGetStickersKeywordsResponse', 'StoriesGetBannedExtendedResponse', 'StoriesGetBannedResponse', 'StoriesGetByIdExtendedResponse', 'StoriesGetPhotoUploadServerResponse', 'StoriesGetStatsResponse', 'StoriesGetVideoUploadServerResponse', 'StoriesGetViewersExtendedV5115Response', 'StoriesGetViewersExtendedResponse', 'StoriesGetV5113Response', 'StoriesGetResponse', 'StoriesSaveResponse', 'StoriesUploadResponse', 'StreamingGetServerUrlResponse', 'UsersGetFollowersFieldsResponse', 'UsersGetFollowersResponse', 'UsersGetSubscriptionsExtendedResponse', 'UsersGetSubscriptionsResponse', 'UsersGetResponse', 'UsersSearchResponse', 'UtilsCheckLinkResponse', 'UtilsGetLastShortenedLinksResponse', 'UtilsGetLinkStatsExtendedResponse', 'UtilsGetLinkStatsResponse', 'UtilsGetServerTimeResponse', 'UtilsGetShortLinkResponse', 'UtilsResolveScreenNameResponse', 'VideoAddAlbumResponse', 'VideoChangeVideoAlbumsResponse', 'VideoCreateCommentResponse', 'VideoGetAlbumByIdResponse', 'VideoGetAlbumsByVideoExtendedResponse', 'VideoGetAlbumsByVideoResponse', 'VideoGetAlbumsExtendedResponse', 'VideoGetAlbumsResponse', 'VideoGetCommentsExtendedResponse', 'VideoGetCommentsResponse', 'VideoGetResponse', 'VideoRestoreCommentResponse', 'VideoSaveResponse', 'VideoSearchExtendedResponse', 'VideoSearchResponse', 'VideoUploadResponse', 'WallCreateCommentResponse', 'WallEditResponse', 'WallGetByIdExtendedResponse', 'WallGetByIdLegacyResponse', 'WallGetByIdResponse', 'WallGetCommentExtendedResponse', 'WallGetCommentResponse', 'WallGetCommentsExtendedResponse', 'WallGetCommentsResponse', 'WallGetRepostsResponse', 'WallGetExtendedResponse', 'WallGetResponse', 'WallPostAdsStealthResponse', 'WallPostResponse', 'WallRepostResponse', 'WallSearchExtendedResponse', 'WallSearchResponse', 'WidgetsGetCommentsResponse', 'WidgetsGetPagesResponse')
```

### Comparing `kavk_api-0.9.7.3/PKG-INFO` & `kavk_api-0.9.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kavk-api
-Version: 0.9.7.3
+Version: 0.9.7.4
 Summary: 
 License: MIT
 Author: Kravandir
 Author-email: kravandir@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

