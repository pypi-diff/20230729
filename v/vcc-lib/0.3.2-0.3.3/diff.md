# Comparing `tmp/vcc_lib-0.3.2.tar.gz` & `tmp/vcc_lib-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcc_lib-0.3.2.tar", last modified: Wed Jul 26 05:50:54 2023, max compression
+gzip compressed data, was "vcc_lib-0.3.3.tar", last modified: Sat Jul 29 08:12:40 2023, max compression
```

## Comparing `vcc_lib-0.3.2.tar` & `vcc_lib-0.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-07-26 05:50:54.607603 vcc_lib-0.3.2/
--rw-r--r--   0 pi        (1000) pi        (1000)     1059 2023-03-19 04:21:24.000000 vcc_lib-0.3.2/LICENCE
--rw-r--r--   0 pi        (1000) pi        (1000)       73 2023-07-26 05:50:54.607603 vcc_lib-0.3.2/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)       97 2023-03-19 04:21:24.000000 vcc_lib-0.3.2/pyproject.toml
--rw-r--r--   0 pi        (1000) pi        (1000)      135 2023-07-26 05:50:54.617603 vcc_lib-0.3.2/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)       37 2023-03-19 04:21:24.000000 vcc_lib-0.3.2/setup.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-07-26 05:50:54.607603 vcc_lib-0.3.2/vcc/
--rw-r--r--   0 pi        (1000) pi        (1000)      223 2023-03-19 04:21:24.000000 vcc_lib-0.3.2/vcc/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)    11871 2023-07-25 14:37:14.000000 vcc_lib-0.3.2/vcc/service.py
--rw-r--r--   0 pi        (1000) pi        (1000)      165 2023-07-08 09:17:04.000000 vcc_lib-0.3.2/vcc/test.py
--rw-r--r--   0 pi        (1000) pi        (1000)     4333 2023-07-08 09:20:07.000000 vcc_lib-0.3.2/vcc/tools.py
--rw-r--r--   0 pi        (1000) pi        (1000)    24870 2023-07-25 14:37:14.000000 vcc_lib-0.3.2/vcc/vcc.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-07-26 05:50:54.607603 vcc_lib-0.3.2/vcc_lib.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)       73 2023-07-26 05:50:54.000000 vcc_lib-0.3.2/vcc_lib.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      262 2023-07-26 05:50:54.000000 vcc_lib-0.3.2/vcc_lib.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-07-26 05:50:54.000000 vcc_lib-0.3.2/vcc_lib.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        6 2023-07-26 05:50:54.000000 vcc_lib-0.3.2/vcc_lib.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        4 2023-07-26 05:50:54.000000 vcc_lib-0.3.2/vcc_lib.egg-info/top_level.txt
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-07-29 08:12:40.352985 vcc_lib-0.3.3/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1059 2023-03-19 04:21:24.000000 vcc_lib-0.3.3/LICENCE
+-rw-r--r--   0 pi        (1000) pi        (1000)       73 2023-07-29 08:12:40.352985 vcc_lib-0.3.3/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)       97 2023-03-19 04:21:24.000000 vcc_lib-0.3.3/pyproject.toml
+-rw-r--r--   0 pi        (1000) pi        (1000)      135 2023-07-29 08:12:40.352985 vcc_lib-0.3.3/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)       37 2023-03-19 04:21:24.000000 vcc_lib-0.3.3/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-07-29 08:12:40.342985 vcc_lib-0.3.3/vcc/
+-rw-r--r--   0 pi        (1000) pi        (1000)      223 2023-03-19 04:21:24.000000 vcc_lib-0.3.3/vcc/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    11871 2023-07-25 14:37:14.000000 vcc_lib-0.3.3/vcc/service.py
+-rw-r--r--   0 pi        (1000) pi        (1000)      165 2023-07-08 09:17:04.000000 vcc_lib-0.3.3/vcc/test.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     4525 2023-07-29 08:12:12.000000 vcc_lib-0.3.3/vcc/tools.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    25102 2023-07-29 08:12:12.000000 vcc_lib-0.3.3/vcc/vcc.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-07-29 08:12:40.352985 vcc_lib-0.3.3/vcc_lib.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)       73 2023-07-29 08:12:40.000000 vcc_lib-0.3.3/vcc_lib.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      262 2023-07-29 08:12:40.000000 vcc_lib-0.3.3/vcc_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-07-29 08:12:40.000000 vcc_lib-0.3.3/vcc_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        6 2023-07-29 08:12:40.000000 vcc_lib-0.3.3/vcc_lib.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        4 2023-07-29 08:12:40.000000 vcc_lib-0.3.3/vcc_lib.egg-info/top_level.txt
```

### Comparing `vcc_lib-0.3.2/LICENCE` & `vcc_lib-0.3.3/LICENCE`

 * *Files identical despite different names*

### Comparing `vcc_lib-0.3.2/vcc/service.py` & `vcc_lib-0.3.3/vcc/service.py`

 * *Files identical despite different names*

### Comparing `vcc_lib-0.3.2/vcc/tools.py` & `vcc_lib-0.3.3/vcc/tools.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,75 +12,105 @@
     from .vcc import RpcExchangerBaseClient
 
 T = TypeVar("T", bound=Callable)
 
 log = logging.getLogger("vcc")
 log.addHandler(logging.NullHandler())
 
-ChatUserPermissionName = Literal["kick", "rename", "invite", "modify_permission", "send"]
+ChatUserPermissionName = Literal[
+    "kick",
+    "rename",
+    "invite",
+    "modify_permission",
+    "send",
+    "create_sub_chat",
+    "create_session",
+    "banned",
+    "change_nickname",
+]
 ChatPermissionName = Literal["public"]
 
+
 class RpcException(Exception):
     pass
 
+
 class ChatAlreadyJoinedError(RpcException):
     pass
 
+
 class ChatNotJoinedError(RpcException):
     pass
 
+
 class UnknownError(RpcException):
     pass
 
+
 class NotAuthorizedError(RpcException):
     pass
 
+
 class PermissionDeniedError(RpcException):
     pass
 
+
 class ProviderNotFoundError(RpcException):
     pass
 
+
 class RedisMessage(TypedDict):
     username: str
     msg: str
     # TODO: add NotRequired after upgrading to python3.11
     session: str
     chat: int
     uid: int
+    id: str
+
 
 Event = Literal["join", "quit", "kick", "rename", "invite"]
 
-MessageCallback = Callable[[int, str, str, int, str | None], None | Awaitable[None]]
+MessageCallback = Callable[[int, str, str, int, str | None, str], None | Awaitable[None]]
 EventCallback = Callable[[Event, Any, int], None | Awaitable[None]]
 
+
 class RedisEvent(TypedDict):
     type: Event
     data: Any
     chat: int
 
+
 log = logging.getLogger("vcc")
 log.addHandler(logging.NullHandler())
 
+
 class ContextObject(object):
     def __init__(self):
         object.__setattr__(
             self, "_context", contextvars.ContextVar("context", default={})
         )
 
     def __getattr__(self, name):
         return self._context.get().get(name, None)
 
     def __setattr__(self, name, value):
         self._context.set(self._context.get() | {name: value})
 
 
-def check(*, auth: bool=True, joined: str | None=None, not_joined: str | None=None, error_return: Any=Exception):
+def check(
+    *,
+    auth: bool = True,
+    joined: str | None = None,
+    not_joined: str | None = None,
+    error_return: Any = Exception,
+):
     def decorator(func: T) -> T:
         signature = inspect.signature(func)
+
         @wraps(func)
         async def wrapper(self: RpcExchangerBaseClient, *args, **kwargs):
             bound_signature = signature.bind(self, *args, **kwargs)
             if auth:
                 self.check_authorized()
             try:
                 if joined is not None:
@@ -89,58 +119,70 @@
                     await self.check_not_joined(bound_signature.arguments[not_joined])
             except RpcException as e:
                 log.warning(e, exc_info=True)
                 if error_return is Exception:
                     raise
                 return copy.deepcopy(error_return)
             return await func(self, *args, **kwargs)
-        return wrapper # type: ignore
+
+        return wrapper  # type: ignore
+
     return decorator
 
-def rpc_request(_service: str | None=None, *, id_arg: str | None=None):
+
+def rpc_request(_service: str | None = None, *, id_arg: str | None = None):
     def decorator(func: T) -> T:
-        namespace, service = _service.split("/", 1) if _service is not None else func.__name__.split("_", 1)
+        namespace, service = (
+            _service.split("/", 1)
+            if _service is not None
+            else func.__name__.split("_", 1)
+        )
         signature = inspect.signature(func)
+
         @wraps(func)
         def wrapper(self: RpcExchangerBaseClient, *args, **kwargs):
             log.debug(f"{namespace=} {service=} {id_arg=} {args=} {kwargs=}")
             bound_signature = signature.bind(self, *args, **kwargs)
             bound_signature.apply_defaults()
             arguments = bound_signature.arguments
             if id_arg is not None:
-                arguments.update({
-                    id_arg: self._id
-                })
+                arguments.update({id_arg: self._id})
             del arguments["self"]
             return self._exchanger.rpc_request(namespace, service, arguments)
-        return wrapper # type: ignore
+
+        return wrapper  # type: ignore
+
     return decorator
-def list_get_default(l,index,default=None):
+
+
+def list_get_default(l, index, default=None):
     return l[index] if index < len(l) else default
+
+
 def get_host() -> tuple[str, int]:
     if "RPCHOST" in os.environ:
         host = os.environ["RPCHOST"].split(":")
         return host[0], int(host[1])
     else:
         return ("localhost", 2474)
 
+
 __all__ = [
-    "check", 
-    "rpc_request", 
+    "check",
+    "rpc_request",
     "get_host",
     "RpcException",
-    "ChatAlreadyJoinedError", 
+    "ChatAlreadyJoinedError",
     "ChatNotJoinedError",
     "UnknownError",
     "NotAuthorizedError",
     "PermissionDeniedError",
     "ProviderNotFoundError",
     "log",
     "ChatUserPermissionName",
     "ChatPermissionName",
     "Event",
     "MessageCallback",
     "EventCallback",
     "RedisEvent",
-    "RedisMessage"
+    "RedisMessage",
 ]
-
```

### Comparing `vcc_lib-0.3.2/vcc/vcc.py` & `vcc_lib-0.3.3/vcc/vcc.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,17 +66,18 @@
                         session: str | None = None
                         username = json_message["username"]
                         msg = json_message["msg"]
                         chat = int(json_message["chat"])
                         uid = int(json_message["uid"])
                         if "session" in json_message:
                             session = json_message["session"]
+                        id = json_message["id"]
                         for client in self.client_list:
                             if chat in client._chat_list and (session is None or isinstance(client, RpcRobotExchangerClient) or (chat, session) in client._session_list):
-                                client._recv_future.set_result(("message", uid, username, msg, chat, session))
+                                client._recv_future.set_result(("message", uid, username, msg, chat, session, id))
                         if "session" in json_message:
                             session = json_message["session"]
                         log.debug(f"{username=} {msg=} {chat=} {session=}")
                     elif raw_message["channel"] == b"events":
                         json_content: RedisEvent = json_content_untyped
                         type = json_content["type"]
                         data = json_content["data"]
@@ -111,24 +112,26 @@
     async def __aexit__(self, *args: Any) -> None:
         self._recv_task.cancel()
         await self.pubsub.unsubscribe("messages")
         await self.pubsub.unsubscribe("events")
         await self._pubsub_raw.__aexit__(*args)
         await self._redis.close()
 
-    async def send_msg(self, uid: int, username: str, msg: str, chat: int, session: str | None=None) -> None:
+    async def send_msg(self, uid: int, username: str, msg: str, chat: int, session: str | None=None) -> str:
         log.debug(f"messages")
+        id = str(uuid.uuid4())
         await self._redis.publish(f"messages", json.dumps({
             "uid": uid,
             "username": username,
             "msg": msg,
             "chat": chat,
             **({} if session is None else {"session": session})
         }))
         log.debug(f"{username=} {msg=} {chat=}")
+        return id
     async def send_event(self, type:str,data:Any, chat: int, session: str | None=None) -> None:
         log.debug(f"event")
         await self._redis.publish(f"events", json.dumps({
             "type": type,
             "data": data,
             "chat": chat,
             **({} if session is None else {"session": session})
@@ -153,15 +156,15 @@
 class RpcExchangerBaseClient:
     _exchanger: RpcExchanger
     _chat_list: set[int]
     _session_list: set[tuple[int, str]]
     _id: int | None
     _name: str | None
     _pubsub: PubSub
-    _recv_future: asyncio.Future[tuple[Literal["message"], int, str, str, int, str | None] | tuple[Literal["event"], Event, Any, int]]
+    _recv_future: asyncio.Future[tuple[Literal["message"], int, str, str, int, str | None, str] | tuple[Literal["event"], Event, Any, int]]
     _chat_list_inited: bool
 
     _msg_callback: MessageCallback | None
     _event_callbacks: dict[Event, EventCallback]
 
     @property
     def id(self) -> int | None:
@@ -210,15 +213,15 @@
     async def send_with_another_username(self, uid: int, username: str, msg: str, chat: int, session: str | None) -> None:
         if session is not None and (chat, session) not in self._session_list:
             raise ChatNotJoinedError()
         if not await self._rpc.chat.check_send_with_another_username(chat_id=chat, user_id=self._id):
             raise PermissionDeniedError()
         await self._exchanger.send_msg(uid, username, msg, chat, session)  
     
-    async def recv(self) -> tuple[Literal["message"], int, str, str, int, str | None] | tuple[Literal["event"], Event, Any, int]:
+    async def recv(self) -> tuple[Literal["message"], int, str, str, int, str | None, str] | tuple[Literal["event"], Event, Any, int]:
         content = await self._recv_future
         if content[0] == "event":
             data = content[2]
             chat = content[3]
             match content[1]:
                 case "join" if data["user_id"] == self._id:
                     self._chat_list.add(chat)
@@ -275,15 +278,15 @@
     @check()
     @rpc_request()
     async def file_get_object_content(self, id: str, bucket: str="file") -> tuple[str, str]: ...
 
     def __aiter__(self) -> RpcExchangerBaseClient:
         return self
 
-    async def __anext__(self) -> tuple[Literal["message"], int, str, str, int, str | None] | tuple[Literal["event"], Event, Any, int]:
+    async def __anext__(self) -> tuple[Literal["message"], int, str, str, int, str | None, str] | tuple[Literal["event"], Event, Any, int]:
         return await self.recv()
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, *args: Any) -> None:
         self._exchanger.client_list.discard(self)
@@ -307,19 +310,20 @@
                 self._event_callbacks[cast(Any, event_type)] = callback
                 return callback
             return event_callback_handler
         else:
             raise TypeError("Wrong usage")
 
     async def run_forever(self) -> None:
+        warnings.warn(DeprecationWarning("This function is deprecated, use recv instead"))
         async for result in self:
             if result[0] == "message":
-                _, uid, username, msg, chat, session = result
+                _, uid, username, msg, chat, session, id = result
                 if self._msg_callback is not None:
-                    returned = self._msg_callback(uid, username, msg, chat, session)
+                    returned = self._msg_callback(uid, username, msg, chat, session, id)
                     if isinstance(returned, Awaitable):
                         await returned
             else:
                 _, type, data, chat = result
                 if type in self._event_callbacks:
                     returned = self._event_callbacks[type](type, data, chat)
                     if isinstance(returned, Awaitable):
@@ -378,41 +382,41 @@
         success = await self._rpc.login.register(username=username, password=password)
         if success and auto_login:
             await self.login(username, password)
         return cast(bool, success)
     
 
     @check(joined="chat")
-    async def send(self, msg: str, chat: int, session: str | None) -> None:
+    async def send(self, msg: str, chat: int, session: str | None) -> str:
         if session is not None and (chat, session) not in self._session_list:
             raise ChatNotJoinedError()
         if not await self._rpc.chat.check_send(chat_id=chat, user_id=self._id):
             raise PermissionDeniedError()
-        await self._exchanger.send_msg(cast(int, self._id), cast(str, self._name), msg, chat, session)   
+        return await self._exchanger.send_msg(cast(int, self._id), cast(str, self._name), msg, chat, session)   
     @check(joined="chat")
     async def send_typing_event(self,status:bool,chat:int,session: str|None) -> None:
         self.check_authorized()
         await self.check_joined(chat)
         if session is not None and (chat, session) not in self._session_list:
             raise ChatNotJoinedError()
         if not await self._rpc.chat.check_send(chat_id=chat, user_id=self._id):
             raise PermissionDeniedError()
         await self._exchanger.send_event("typing", {
             "status": status,
             "uid": self.id
         }, chat, session)
 
     @check(joined="chat")
-    async def send_with_another_username(self, uid: int, msg: str, chat: int, session: str | None) -> None:
+    async def send_with_another_username(self, uid: int, msg: str, chat: int, session: str | None) -> str:
         if session is not None and (chat, session) not in self._session_list:
             raise ChatNotJoinedError()
         if not await self._rpc.chat.check_send_with_another_username(chat_id=chat, user_id=self._id):
             raise PermissionDeniedError()
         username = await self._rpc.chat.get_nickname(chat_id=chat, user_id=uid)
-        await self._exchanger.send_msg(uid, username, msg, chat, session)  
+        return await self._exchanger.send_msg(uid, username, msg, chat, session)  
 
     @check(joined="chat_id", error_return=False)
     async def session_join(self, name: str, chat_id: int) -> bool:
         result = await self._rpc.chat.check_create_session(chat_id=chat_id, user_id=self._id)
         if result:
             self._session_list.add((chat_id, name))
         return cast(bool, result)
@@ -519,19 +523,19 @@
         uid: int | None = await self._rpc.bot.register(name=name, token=token)
         if uid is not None:
             self._id = uid
             self._name = name
         return uid
 
     @check(joined="chat")
-    async def send(self, username: str, msg: str, chat: int, session: str | None) -> None:
+    async def send(self, username: str, msg: str, chat: int, session: str | None) -> str:
         if not await self._rpc.bot.check_send(chat_id=chat, bot_id=self._id):
             raise PermissionDeniedError()
         # -1 means system or robot
-        await self._exchanger.send_msg(-1, f"{username}[{cast(str, self.name)}]", msg, chat, session)
+        return await self._exchanger.send_msg(-1, f"{username}[{cast(str, self.name)}]", msg, chat, session)
     
     @check(not_joined="id", error_return=False)
     async def chat_join(self, id: int) -> bool:
         """Join a chat by its id"""
         if not await self._rpc.bot.join(chat_id=id, bot_id=self._id):
             return False
         async with self._chat_list_lock:
```

