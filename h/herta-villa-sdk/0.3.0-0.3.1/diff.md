# Comparing `tmp/herta_villa_sdk-0.3.0.tar.gz` & `tmp/herta_villa_sdk-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "herta_villa_sdk-0.3.0.tar", last modified: Fri Jun 23 09:38:37 2023, max compression
+gzip compressed data, was "herta_villa_sdk-0.3.1.tar", last modified: Sat Jun 24 10:17:43 2023, max compression
```

## Comparing `herta_villa_sdk-0.3.0.tar` & `herta_villa_sdk-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     1069 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/LICENSE
--rw-r--r--   0        0        0     2039 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/README.md
--rw-r--r--   0        0        0      555 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/hertavilla/__init__.py
--rw-r--r--   0        0        0    11217 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/hertavilla/bot.py
--rw-r--r--   0        0        0     4833 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/hertavilla/event.py
--rw-r--r--   0        0        0      738 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/hertavilla/exception.py
--rw-r--r--   0        0        0     1481 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/hertavilla/match.py
--rw-r--r--   0        0        0      353 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/hertavilla/message/__init__.py
--rw-r--r--   0        0        0     1761 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/hertavilla/message/chain.py
--rw-r--r--   0        0        0     1617 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/hertavilla/message/image.py
--rw-r--r--   0        0        0      981 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/hertavilla/message/post.py
--rw-r--r--   0        0        0     6095 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/hertavilla/message/text.py
--rw-r--r--   0        0        0      369 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/hertavilla/message/types.py
--rw-r--r--   0        0        0     2372 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/hertavilla/model.py
--rw-r--r--   0        0        0     2932 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/hertavilla/server.py
--rw-r--r--   0        0        0      558 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/hertavilla/utils.py
--rw-r--r--   0        0        0       58 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/hertavilla/version.py
--rw-r--r--   0        0        0     1986 2023-06-23 09:38:37.121166 herta_villa_sdk-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2669 1970-01-01 00:00:00.000000 herta_villa_sdk-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2039 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/README.md
+-rw-r--r--   0        0        0      555 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/hertavilla/__init__.py
+-rw-r--r--   0        0        0    11250 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/hertavilla/bot.py
+-rw-r--r--   0        0        0     4864 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/hertavilla/event.py
+-rw-r--r--   0        0        0      738 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/hertavilla/exception.py
+-rw-r--r--   0        0        0     1481 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/hertavilla/match.py
+-rw-r--r--   0        0        0      353 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/hertavilla/message/__init__.py
+-rw-r--r--   0        0        0     1761 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/hertavilla/message/chain.py
+-rw-r--r--   0        0        0     1617 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/hertavilla/message/image.py
+-rw-r--r--   0        0        0      981 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/hertavilla/message/post.py
+-rw-r--r--   0        0        0     6461 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/hertavilla/message/text.py
+-rw-r--r--   0        0        0      369 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/hertavilla/message/types.py
+-rw-r--r--   0        0        0     2396 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/hertavilla/model.py
+-rw-r--r--   0        0        0     2932 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/hertavilla/server.py
+-rw-r--r--   0        0        0      565 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/hertavilla/utils.py
+-rw-r--r--   0        0        0       58 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/hertavilla/version.py
+-rw-r--r--   0        0        0     2128 2023-06-24 10:17:43.581042 herta_villa_sdk-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      572 2023-06-24 10:17:09.484352 herta_villa_sdk-0.3.1/tests/test_utils.py
+-rw-r--r--   0        0        0     2669 1970-01-01 00:00:00.000000 herta_villa_sdk-0.3.1/PKG-INFO
```

### Comparing `herta_villa_sdk-0.3.0/LICENSE` & `herta_villa_sdk-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.3.0/README.md` & `herta_villa_sdk-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.3.0/hertavilla/__init__.py` & `herta_villa_sdk-0.3.1/hertavilla/__init__.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.3.0/hertavilla/bot.py` & `herta_villa_sdk-0.3.1/hertavilla/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import asyncio
+from dataclasses import dataclass
 import json
 import logging
 import re
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
@@ -36,15 +37,16 @@
     ["SendMessageEvent", "VillaBot"],
     Coroutine[Any, Any, None],
 ]
 
 logger = logging.getLogger("hertavilla.bot")
 
 
-class Handler(NamedTuple, Generic[TE]):
+@dataclass
+class Handler(Generic[TE]):
     event: type[TE]
     func: Callable[[TE, VillaBot], Coroutine[Any, Any, None]]
 
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
         return self.func(*args, **kwargs)
 
     def __eq__(self, __value: Event) -> bool:
```

### Comparing `herta_villa_sdk-0.3.0/hertavilla/event.py` & `herta_villa_sdk-0.3.1/hertavilla/event.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # ruff: noqa: A003
 from __future__ import annotations
 
 import json
 import sys
-from typing import Any, Literal, Type
+from typing import Any, List, Literal, Optional, Type
 
 from hertavilla.message import (
     MessageChain,
 )
 from hertavilla.message.text import (
     EntityDict,
     MentionedInfo,
@@ -33,15 +33,15 @@
 
 
 class Template(BaseModel):
     id: str
     name: str
     desc: str
     icon: str
-    commands: list[Command]
+    commands: List[Command]
 
 
 class Robot(BaseModel):
     """机器人相关信息"""
 
     template: Template
     """机器人模板信息"""
@@ -120,21 +120,21 @@
     bot_msg_id: str
     client: str
     rong_sdk_version: str
 
 
 class MessageContent(BaseModel):
     content: MessageChain
-    mentioned_info: MentionedInfoModel | None = Field(  # type: ignore
+    mentioned_info: Optional[MentionedInfoModel] = Field(  # type: ignore
         None,
         alias="mentionedInfo",
     )
-    quote: QuoteInfoModel | None = None  # type: ignore
-    user: User | None = None
-    trace: Trace | None = None
+    quote: Optional[QuoteInfoModel] = None  # type: ignore
+    user: Optional[User] = None
+    trace: Optional[Trace] = None
 
     @validator("content", pre=True)
     def parse_content(cls, v: Any):
         chain = MessageChain()
         text = v["text"].encode("utf-16")
         entities = v["entities"]
         last_offset = 0
@@ -176,15 +176,15 @@
     """房间 id"""
     object_name: int
     """目前只支持文本类型消息"""
     nickname: str
     """用户昵称"""
     msg_uid: str
     """消息 id"""
-    bot_msg_id: str | None
+    bot_msg_id: Optional[str]
     """如果被回复的消息从属于机器人，则该字段不为空字符串"""
 
     @validator("content", pre=True)
     def str_to_json(cls, v: Any):
         return json.loads(v)
 
     @property
```

### Comparing `herta_villa_sdk-0.3.0/hertavilla/exception.py` & `herta_villa_sdk-0.3.1/hertavilla/exception.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.3.0/hertavilla/match.py` & `herta_villa_sdk-0.3.1/hertavilla/match.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.3.0/hertavilla/message/chain.py` & `herta_villa_sdk-0.3.1/hertavilla/message/chain.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.3.0/hertavilla/message/image.py` & `herta_villa_sdk-0.3.1/hertavilla/message/image.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.3.0/hertavilla/message/post.py` & `herta_villa_sdk-0.3.1/hertavilla/message/post.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.3.0/hertavilla/message/text.py` & `herta_villa_sdk-0.3.1/hertavilla/message/text.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Literal, TypedDict, cast
+import sys
+from typing import TYPE_CHECKING, Any, List, Literal, Optional, cast
+
+# Pydantic:
+#   TypeError: You should use `typing_extensions.TypedDict`
+#   instead of `typing.TypedDict` with Python < 3.9.2.
+#   Without it, there is no way to differentiate
+#   required and optional fields when subclassed.
+if sys.version_info >= (3, 9, 2):
+    from typing import TypedDict
+else:
+    from typing_extensions import TypedDict
 
 from hertavilla.message.types import MsgContent, MsgContentInfo, _Segment
 from hertavilla.utils import _c
 
 if TYPE_CHECKING:
     from hertavilla.bot import VillaBot
 
 entity_types: dict[str, type["_TextEntity"]] = {}
 
 # MsgContentInfo for text
 
 
 class TextMsgContentInfo(MsgContentInfo):
     content: TextMsgContent
-    mentionedInfo: MentionedInfo | None
-    quote: QuoteInfo | None
+    mentionedInfo: Optional[MentionedInfo]
+    quote: Optional[QuoteInfo]
 
 
 class QuoteInfo(TypedDict):
     quoted_message_id: str
     """引用消息 id"""
 
     quoted_message_send_time: str
@@ -35,15 +46,15 @@
 
 class MentionedInfo(TypedDict):
     type: Literal[1, 2]  # noqa: A003
     """提及类型:
     值为1: @全员
     值为2: @部分成员"""
 
-    userIdList: list[str]
+    userIdList: List[str]
     """如果不是提及全员，应该填写被提及的用户 id 列表"""
 
 
 class EntityDict(TypedDict):
     entity: Any
     length: int
     offset: int
```

### Comparing `herta_villa_sdk-0.3.0/hertavilla/model.py` & `herta_villa_sdk-0.3.1/hertavilla/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # ruff: noqa: A003
 from __future__ import annotations
 
 from enum import Enum
+from typing import List
 
 from pydantic import BaseModel
 
 
 class _BotMemberAccess(BaseModel):
     uid: int
     """用户 id"""
@@ -49,20 +50,20 @@
     """"""
 
 
 class Member(BaseModel):
     basic: MemberBasic
     """用户基本信息"""
 
-    role_id_list: list[int]
+    role_id_list: List[int]
     """用户加入的身份组 id 列表"""
 
     joined_at: str
     """用户加入时间 (ISO8601 timestamp)"""
-    role_list: list[Role]
+    role_list: List[Role]
 
 
 class BotMemberAccessInfo(BaseModel):
     access_info: _BotMemberAccess
     """token 解析的用户信息"""
     member: Member
     """用户详细信息"""
@@ -86,15 +87,15 @@
 
     introduce: str
     """介绍"""
 
     category_id: int
     """"""
 
-    tags: list[str]
+    tags: List[str]
     """标签"""
 
 
 class RoomType(str, Enum):
     CHAT_ROOM = "BOT_PLATFORM_ROOM_TYPE_CHAT_ROOM"
     """聊天房间"""
     POST_ROOM = "BOT_PLATFORM_ROOM_TYPE_POST_ROOM"
@@ -105,15 +106,15 @@
     """无效"""
 
 
 class SendMsgAuthRange(BaseModel):
     is_all_send_msg: bool
     """是否全局可发送"""
 
-    roles: list[int]
+    roles: List[int]
     """可发消息的身份组 id"""
 
 
 class Room(BaseModel):
     room_id: int
     """房间 id"""
```

### Comparing `herta_villa_sdk-0.3.0/hertavilla/server.py` & `herta_villa_sdk-0.3.1/hertavilla/server.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.3.0/hertavilla/utils.py` & `herta_villa_sdk-0.3.1/hertavilla/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 class MsgEncoder(json.JSONEncoder):
     def default(self, obj):
         from hertavilla.message.types import MsgContent
 
         if isinstance(obj, MsgContent):
             data = obj.__dict__
-            for k in data.keys():
+            for k in data.copy().keys():
                 if k.startswith("_"):
                     data.pop(k)
             return data
         return json.JSONEncoder.default(self, obj)
 
 
 def _c(text: str) -> int:
```

### Comparing `herta_villa_sdk-0.3.0/pyproject.toml` & `herta_villa_sdk-0.3.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 [project]
 name = "herta-villa-sdk"
-version = "0.3.0"
 description = "大别野「黑塔」Python SDK"
 authors = [
     { name = "MingxuanGame", email = "MingxuanGame@outlook.com" },
 ]
 dependencies = [
     "aiohttp>=3.8.4",
     "pydantic>=1.10.8",
@@ -13,14 +12,16 @@
 readme = "README.md"
 keywords = [
     "mihoyo",
     "miyoushe",
     "bot",
     "villa",
 ]
+dynamic = []
+version = "0.3.1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/MingxuanGame/Herta-villa-SDK"
 Documentation = "https://github.com/MingxuanGame/Herta-villa-SDK"
@@ -29,20 +30,28 @@
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
+[tool.pdm.version]
+source = "file"
+path = "hertavilla/version.py"
+
 [tool.pdm.dev-dependencies]
 dev = [
     "ruff>=0.0.270",
     "pre-commit>=3.3.2",
     "black>=23.3.0",
 ]
+test = [
+    "pytest>=7.4.0",
+    "pytest-asyncio>=0.21.0",
+]
 
 [tool.pdm.scripts]
 lint = "ruff check ."
 fix = "ruff check --fix ."
 
 [tool.ruff]
 line-length = 79
```

### Comparing `herta_villa_sdk-0.3.0/PKG-INFO` & `herta_villa_sdk-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herta-villa-sdk
-Version: 0.3.0
+Version: 0.3.1
 Summary: 大别野「黑塔」Python SDK
 Keywords: mihoyo miyoushe bot villa
 Author-Email: MingxuanGame <MingxuanGame@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/MingxuanGame/Herta-villa-SDK
 Project-URL: Documentation, https://github.com/MingxuanGame/Herta-villa-SDK
 Project-URL: Repository, https://github.com/MingxuanGame/Herta-villa-SDK
```

