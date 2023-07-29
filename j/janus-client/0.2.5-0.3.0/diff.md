# Comparing `tmp/janus_client-0.2.5.tar.gz` & `tmp/janus_client-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "janus_client-0.2.5.tar", max compression
+gzip compressed data, was "janus_client-0.3.0.tar", max compression
```

## Comparing `janus_client-0.2.5.tar` & `janus_client-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      211 2023-07-22 06:24:20.872509 janus_client-0.2.5/janus_client/__init__.py
--rw-r--r--   0        0        0    11251 2023-07-22 07:10:09.526094 janus_client-0.2.5/janus_client/core.py
--rw-r--r--   0        0        0     7186 2023-07-23 14:00:09.146471 janus_client-0.2.5/janus_client/media.py
--rw-r--r--   0        0        0     2223 2023-07-22 07:07:52.191119 janus_client-0.2.5/janus_client/plugin_base.py
--rw-r--r--   0        0        0    14360 2023-07-22 06:24:20.872509 janus_client-0.2.5/janus_client/plugin_video_room.py
--rw-r--r--   0        0        0     9181 2023-07-23 13:49:35.776875 janus_client-0.2.5/janus_client/plugin_video_room_ffmpeg.py
--rw-r--r--   0        0        0     3028 2023-07-22 07:08:40.841540 janus_client-0.2.5/janus_client/session.py
--rw-r--r--   0        0        0     1069 2023-07-22 06:24:20.872509 janus_client-0.2.5/LICENSE
--rw-r--r--   0        0        0      865 2023-07-23 15:10:41.141425 janus_client-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     6715 2023-07-23 14:33:40.913988 janus_client-0.2.5/README.md
--rw-r--r--   0        0        0     7670 1970-01-01 00:00:00.000000 janus_client-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      274 2023-07-29 17:16:45.751175 janus_client-0.3.0/janus_client/__init__.py
+-rw-r--r--   0        0        0    11597 2023-07-29 13:05:52.613860 janus_client-0.3.0/janus_client/core.py
+-rw-r--r--   0        0        0     7592 2023-07-29 16:26:44.628495 janus_client-0.3.0/janus_client/media.py
+-rw-r--r--   0        0        0     2570 2023-07-29 09:16:50.135149 janus_client-0.3.0/janus_client/plugin_base.py
+-rw-r--r--   0        0        0    14360 2023-07-22 06:24:20.872509 janus_client-0.3.0/janus_client/plugin_video_room.py
+-rw-r--r--   0        0        0     8225 2023-07-29 12:49:05.375883 janus_client-0.3.0/janus_client/plugin_video_room_ffmpeg.py
+-rw-r--r--   0        0        0     3552 2023-07-29 09:33:38.945245 janus_client-0.3.0/janus_client/session.py
+-rw-r--r--   0        0        0     1069 2023-07-22 06:24:20.872509 janus_client-0.3.0/LICENSE
+-rw-r--r--   0        0        0      886 2023-07-29 17:27:15.029727 janus_client-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4449 2023-07-29 17:22:33.485710 janus_client-0.3.0/README.md
+-rw-r--r--   0        0        0     5445 1970-01-01 00:00:00.000000 janus_client-0.3.0/PKG-INFO
```

### Comparing `janus_client-0.2.5/janus_client/core.py` & `janus_client-0.3.0/janus_client/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,58 @@
 import asyncio
-import websockets
 import json
 import uuid
-import traceback
-from .session import JanusSession
-from typing import Type, Dict, Any
+from typing import TYPE_CHECKING, Dict, Any, Optional
+
+import websockets
+from pydantic import BaseModel, Field
+
+if TYPE_CHECKING:
+    from .session import JanusSession
 
 import logging
 
 logger = logging.getLogger(__name__)
 
 
+class JanusMessage(BaseModel):
+    transaction: str = Field(default_factory=lambda: uuid.uuid4().hex)
+    apisecret: Optional[str] = None
+    token: Optional[str] = None
+    janus: str
+
+
 """
 Architecture design to handle Janus transactions and events
 Assumption 1: All transaction ids are unique, and they will always get
     at least one reply when there are no network errors
-So to handle transactions, it will be tracked in JanusClient only.
+So to handle transactions, it will be tracked in JanusConnection only.
 To handle events, it will be passed top down to all matching session id
     and plugin handle id.
-Each node down the tree with JanusClient as root, including JanusClient itself,
+Each node down the tree with JanusConnection as root, including JanusConnection itself,
 shall have:
 1. handle_async_response method
 
 E.g.
 class JanusSession
     def handle_async_response(self, response):
         pass
 """
 
 
-class JanusClient:
-    """Janus client instance, connected through websocket"""
+class JanusConnection:
+    """Janus connection instance, connected through websocket
+
+    Manage Sessions and Transactions
+    """
+
+    connected: bool = False
 
     def __init__(self, uri: str, api_secret: str = None, token: str = None):
-        """Initialize client instance
+        """Create connection instance
 
         :param uri: Janus server address
         :param api_secret: (optional) API key for shared static secret authentication
         :param token: (optional) Token for shared token based authentication
         """
 
         self.ws: websockets.WebSocketClientProtocol
@@ -50,131 +65,134 @@
     async def connect(self, **kwargs: Any) -> None:
         """Connect to server
 
         All extra keyword arguments will be passed to websockets.connect
         """
 
         logger.info(f"Connecting to: {self.uri}")
-        # self.ws = await websockets.connect(self.uri, ssl=ssl_context)
+
         self.ws = await websockets.connect(
             self.uri, subprotocols=[websockets.Subprotocol("janus-protocol")], **kwargs
         )
         self.receive_message_task = asyncio.create_task(self.receive_message())
         self.receive_message_task.add_done_callback(self.receive_message_done_cb)
+
+        self.connected = True
         logger.info("Connected")
 
     async def disconnect(self) -> None:
         """Disconnect from server"""
 
         logger.info("Disconnecting")
         self.receive_message_task.cancel()
         await self.ws.close()
+        self.connected = False
 
-    def is_async_response(self, response: dict):
+    def is_async_response(self, response: dict) -> bool:
         janus_type = response["janus"]
         return (
             (janus_type == "event")
             or (janus_type == "detached")
             or (janus_type == "webrtcup")
             or (janus_type == "media")
             or (janus_type == "slowlink")
             or (janus_type == "hangup")
         )
 
-    def receive_message_done_cb(self, task, context=None):
+    def receive_message_done_cb(self, task: asyncio.Task, context=None) -> None:
         try:
             # Check if any exceptions are raised
-            exception = task.exception()
-            traceback.print_tb(exception.__traceback__)
-            logger.info(f"{type(exception)} : {exception}")
+            task.exception()
+            # traceback.print_tb(exception.__traceback__)
+            # logger.info(f"{type(exception)} : {exception}")
         except asyncio.CancelledError:
             logger.info("Receive message task ended")
         except asyncio.InvalidStateError:
             logger.info("receive_message_done_cb called with invalid state")
-        except Exception as e:
-            traceback.logger.info_tb(e.__traceback__)
+        # except Exception as e:
+        #     traceback.logger.info_tb(e.__traceback__)
+
+    async def receive_message(self) -> None:
+        if not self.ws:
+            raise Exception("Not connected to server.")
 
-    async def receive_message(self):
-        assert self.ws
         async for message_raw in self.ws:
             response = json.loads(message_raw)
+            logger.info(f"Receive: {response}")
+
             if self.is_async_response(response):
                 self.handle_async_response(response)
             else:
                 transaction_id = response["transaction"]
                 await self.transactions[transaction_id].put(response)
 
-    async def send(self, message: dict) -> dict:
-        """Semd message to server
+    async def send(self, message: JanusMessage) -> dict:
+        """Send message to server
 
         :param message: JSON serializable dictionary to send
 
         :returns: Synchronous response from Janus server
 
         """
-        # Create transaction
-        transaction_id = uuid.uuid4().hex
-        message["transaction"] = transaction_id
+        # # Create transaction
+        # transaction_id = uuid.uuid4().hex
+        # message["transaction"] = transaction_id
+
         # Transaction ID must be in the dict to receive response
-        self.transactions[transaction_id] = asyncio.Queue()
+        self.transactions[message.transaction] = asyncio.Queue()
 
         # Authentication
         if self.api_secret is not None:
-            message["apisecret"] = self.api_secret
+            message.apisecret = self.api_secret
         if self.token is not None:
-            message["token"] = self.token
+            message.token = self.token
 
         # Send the message
-        logger.info(json.dumps(message))
-        await self.ws.send(json.dumps(message))
+        message_json = message.model_dump_json(exclude_none=True)
+        logger.info(f"Send: {message_json}")
+        await self.ws.send(message_json)
 
         # Wait for response
         # Assumption: there will be one and only one synchronous reply for a transaction.
         #   Other replies with the same transaction ID are asynchronous.
-        response = await self.transactions[transaction_id].get()
-        logger.info(f"Transaction reply: {response}")
+        response = await self.transactions[message.transaction].get()
 
         # Transaction complete, delete it
-        del self.transactions[transaction_id]
+        del self.transactions[message.transaction]
         return response
 
-    def handle_async_response(self, response: dict):
+    def handle_async_response(self, response: dict) -> None:
         if "session_id" in response:
             # This is response for session or plugin handle
             if response["session_id"] in self.sessions:
                 self.sessions[response["session_id"]].handle_async_response(response)
             else:
-                logger.info(
+                logger.warning(
                     f"Got response for session but session not found. Session ID: {response['session_id']}"
+                    f"Unhandeled response: {response}"
                 )
-                logger.info(f"Unhandeled response: {response}")
         else:
             # This is response for self
             logger.info(f"Async event for Janus client core: {response}")
 
-    async def create_session(
-        self, session_type: Type[JanusSession] = JanusSession
-    ) -> JanusSession:
-        """Create Janus session instance
+    async def create_session(self, session: "JanusSession") -> int:
+        """Create Janus Session"""
 
-        :param session_type: Class type of session. Should be JanusSession,
-            no other options yet.
-        """
+        response = await self.send(JanusMessage(janus="create"))
 
-        response = await self.send(
-            {
-                "janus": "create",
-            }
-        )
-        session = session_type(client=self, session_id=response["data"]["id"])
-        self.sessions[session.id] = session
-        return session
+        # Extract session ID
+        session_id = int(response["data"]["id"])
+
+        # Register session
+        self.sessions[session_id] = session
+
+        return session_id
 
     # Don't call this from client object, call destroy from session instead
-    def destroy_session(self, session):
+    def destroy_session(self, session: "JanusSession") -> None:
         del self.sessions[session.id]
 
 
 """
 # Take note to enable admin API with websockets in Janus, for example:
 # admin: {
 #         admin_ws = true                         # Whether to enable the Admin API WebSockets API
```

### Comparing `janus_client-0.2.5/janus_client/media.py` & `janus_client-0.3.0/janus_client/media.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 import logging
 import threading
-import time
 from typing import Optional, Set, Union
+import subprocess
+import time
 
 from av import VideoFrame
 from av.frame import Frame
 from av.packet import Packet
 import numpy as np
 import fractions
 
@@ -76,18 +77,14 @@
         """
         for task in self.__tracks.values():
             if task is not None:
                 task.cancel()
         self.__tracks = {}
 
 
-# format = "%(asctime)s: %(message)s"
-# logging.basicConfig(format=format, level=logging.INFO, datefmt="%H:%M:%S")
-
-
 class PlayerStreamTrack(MediaStreamTrack):
     def __init__(self, player, kind):
         super().__init__()
         self.kind = kind
         self._player = player
         self._queue = asyncio.Queue()
         self._start = None
@@ -97,27 +94,27 @@
             raise MediaStreamError
 
         self._player._start(self)
         data = await self._queue.get()
         if data is None:
             self.stop()
             raise MediaStreamError
-        data_time = None
+        # data_time = None
 
-        # control playback rate
-        if (
-            self._player is not None
-            and self._player._throttle_playback
-            and data_time is not None
-        ):
-            if self._start is None:
-                self._start = time.time() - data_time
-            else:
-                wait = self._start + data_time - time.time()
-                await asyncio.sleep(wait)
+        # # control playback rate
+        # if (
+        #     self._player is not None
+        #     and self._player._throttle_playback
+        #     and data_time is not None
+        # ):
+        #     if self._start is None:
+        #         self._start = time.time() - data_time
+        #     else:
+        #         wait = self._start + data_time - time.time()
+        #         await asyncio.sleep(wait)
 
         return data
 
     def stop(self):
         super().stop()
         if self._player is not None:
             self._player._stop(self)
@@ -146,15 +143,15 @@
         })
 
         # Open webcam on OS X.
         player = MediaPlayer('default:none', format='avfoundation', options={
             'video_size': '640x480'
         })
 
-        # Open webcam on Windows.
+        # Open webcam on Windows.
         player = MediaPlayer('video=Integrated Camera', format='dshow', options={
             'video_size': '640x480'
         })
 
     :param file: The path to a file, or a file-like object.
     :param format: The format to use, defaults to autodect.
     :param options: Additional options to pass to FFmpeg.
@@ -172,16 +169,15 @@
         self.__thread_quit: Optional[threading.Event] = None
 
         self.__ffmpeg_input = ffmpeg_input
         self.__width = width
         self.__height = height
 
         # examine streams
-        self.__started: Set[PlayerStreamTrack] = set()
-        self.__streams = []
+        self.__started: Set[MediaStreamTrack] = set()
         self.__audio: Optional[PlayerStreamTrack] = None
         self.__video = PlayerStreamTrack(self, kind="video")
 
         self._throttle_playback = False
         self._loop_playback = False
 
     @property
@@ -202,38 +198,52 @@
         self,
         loop,
         video_track,
         quit_event,
     ):
         logging.info("Thread 1: starting")
         pts = 0
-        video_process = self.__ffmpeg_input.output(
+        video_process: subprocess.Popen = self.__ffmpeg_input.output(
             "pipe:", format="rawvideo", pix_fmt="rgb24"
-        ).run_async(pipe_stdout=True)
+        ).run_async(pipe_stdout=True, pipe_stdin=True)
 
+        count = 0
+        total_time = 0
+        total_cpu_time = 0
         while not quit_event.is_set():
             in_bytes = video_process.stdout.read(self.__width * self.__height * 3)
             if not in_bytes:
                 break
 
+            start_time = time.time()
+            start_cpu_time = time.process_time()
+
             in_frame = np.frombuffer(in_bytes, np.uint8).reshape(
                 [self.__height, self.__width, 3]
             )
             frame = VideoFrame.from_ndarray(in_frame, format="rgb24")
 
             frame.pts = pts
             pts += 1
             frame.time_base = fractions.Fraction(1, 48000)
 
+            total_time += time.time() - start_time
+            total_cpu_time += time.process_time() - start_cpu_time
+            count += 1
+
             # logging.info(frame)
             asyncio.run_coroutine_threadsafe(video_track._queue.put(frame), loop)
 
+        video_process.communicate(b"q", timeout=1)
         video_process.wait()
 
         logging.info("Thread 1: finishing")
+        logger.info(
+            f"time: {total_time * 1000 / count}ms | cpu time: {total_cpu_time * 1000 / count}ms"
+        )
 
     def _start(self, track: PlayerStreamTrack) -> None:
         self.__started.add(track)
         if self.__thread is None:
             self.__log_debug("Starting worker thread")
             self.__thread_quit = threading.Event()
             self.__thread = threading.Thread(
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `janus_client-0.2.5/janus_client/plugin_base.py` & `janus_client-0.3.0/janus_client/plugin_base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,55 @@
-from __future__ import annotations
-from typing import TYPE_CHECKING
+from .session import JanusSession, SessionMessage
 
-if TYPE_CHECKING:
-    from .session import JanusSession
+
+class PluginMessage(SessionMessage):
+    handle_id: int = None
 
 
 class JanusPlugin:
     """Base class to inherit when implementing a plugin"""
 
-    name = "janus.plugin.base.dummy"
+    name: str = "janus.plugin.base.dummy"
     """Plugin name
 
     Must override to match plugin name in Janus server.
     """
+    __id: str = None
+    session: JanusSession
+
+    @property
+    def id(self) -> int:
+        return self.__id
+
+    async def attach(self, session: JanusSession):
+        if self.__id:
+            raise Exception(f"Plugin already attached to session ({self.session.id})")
 
-    def __init__(self, session: JanusSession, handle_id: int):
         self.session = session
-        self.id = handle_id
+        self.__id = await session.attach_plugin(self)
 
     async def destroy(self):
         """Destroy plugin handle"""
 
-        message = {
-            "janus": "detach",
-        }
-        await self.send(message)
-        self.session.destroy_plugin_handle(self)
+        await self.send(PluginMessage(janus="detach"))
+        self.session.detach_plugin(self)
 
-    async def send(self, message: dict) -> dict:
+    async def send(self, message: PluginMessage) -> dict:
         """Send raw message to plugin
 
         Will auto attach plugin ID to the message.
 
         :param message: JSON serializable dictionary to send
         :return: Synchronous reply from server
         """
 
-        if "handle_id" in message:
-            raise Exception("Handle ID in message must not be manually added")
-        message["handle_id"] = self.id
+        if message.handle_id:
+            raise Exception("Plugin handle ID must not be manually added")
+
+        message.handle_id = self.__id
         return await self.session.send(message)
 
     def handle_async_response(self, response: dict):
         """Handle asynchronous events from Janus
 
         Must be overridden
 
@@ -54,20 +61,25 @@
     async def trickle(self, sdpMLineIndex, candidate):
         """Send WebRTC candidates to Janus
 
         :param sdpMLineIndex: (I don't know what is this)
         :param candidate: Candidate payload. (I got it from WebRTC instance callback)
         """
 
+        class TrickleMessage(PluginMessage):
+            candidate: dict
+
         candidate_payload = dict()
         if candidate:
             candidate_payload = {
                 "sdpMLineIndex": sdpMLineIndex,
                 "candidate": candidate,
             }
         else:
             # Reference: https://janus.conf.meetecho.com/docs/rest.html
             # - a null candidate or a completed JSON object to notify the end of the candidates.
             # TODO: test it
             candidate_payload = None
-        await self.send({"janus": "trickle", "candidate": candidate_payload})
+
+        # await self.send({"janus": "trickle", "candidate": candidate_payload})
+        await self.send(TrickleMessage(janus="trickle", candidate=candidate_payload))
         # TODO: Implement sending an array of candidates
```

### Comparing `janus_client-0.2.5/janus_client/plugin_video_room.py` & `janus_client-0.3.0/janus_client/plugin_video_room.py`

 * *Files identical despite different names*

### Comparing `janus_client-0.2.5/janus_client/plugin_video_room_ffmpeg.py` & `janus_client-0.3.0/janus_client/plugin_video_room_ffmpeg.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-from janus_client import JanusPlugin
 import asyncio
 import logging
+
+from .plugin_base import JanusPlugin, PluginMessage
 from aiortc import RTCPeerConnection, RTCSessionDescription, VideoStreamTrack
 from .media import MediaPlayer
 
 logger = logging.getLogger(__name__)
 
 
 class JanusVideoRoomPlugin(JanusPlugin):
     """Janus VideoRoom plugin instance
 
     Implements API to interact with VideoRoom plugin.
+
+    Each plugin instance is expected to have only 1 PeerConnection
     """
 
     name = "janus.plugin.videoroom"  #: Plugin name
     pc = RTCPeerConnection()
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.joined_event = asyncio.Event()
-        self.gst_webrtc_ready = asyncio.Event()
         self.loop = asyncio.get_running_loop()
 
     def handle_async_response(self, response: dict):
         if response["janus"] == "event":
             logger.info(f"Event response: {response}")
             if "plugindata" in response:
                 if response["plugindata"]["data"]["videoroom"] == "attached":
@@ -47,90 +49,110 @@
         | There is an API to configure and publish at the same time, but it's not implemented yet.
 
         :param room_id: Room ID to join. This must be available at the server.
         :param publisher_id: Your publisher ID to set.
         :param display_name: Your display name when you join the room.
         """
 
-        await self.send(
-            {
-                "janus": "message",
-                "body": {
+        class JoinMessage(PluginMessage):
+            body: dict
+
+        response = await self.send(
+            JoinMessage(
+                janus="message",
+                body={
                     "request": "join",
                     "ptype": "publisher",
                     "room": room_id,
                     "id": publisher_id,
                     "display": display_name,
                 },
-            }
+            )
         )
+        logger.info(f"Room join response: {response}")
         await self.joined_event.wait()
 
-    async def publish(self, player: MediaPlayer) -> None:
+    async def leave(self):
+        class LeaveMessage(PluginMessage):
+            body: dict
+
+        response = await self.send(
+            LeaveMessage(
+                janus="message",
+                body={
+                    "request": "leave",
+                },
+            )
+        )
+        logger.info(f"Room leave response: {response}")
+
+    async def publish(self, ffmpeg_input, width: int, height: int) -> None:
         """Publish video stream to the room
 
         Should already have joined a room before this. Then this will publish the
         video stream to the handle.
         """
 
+        # create media source
+        player = MediaPlayer(
+            ffmpeg_input,
+            width,
+            height,
+        )
+        # Just save the media player. Not used
+        self.player = player
+
         # configure media
         media = {"audio": False, "video": True}
         if player and player.audio:
             self.pc.addTrack(player.audio)
             media["audio"] = True
 
         if player and player.video:
             self.pc.addTrack(player.video)
         else:
             self.pc.addTrack(VideoStreamTrack())
 
         # send offer
         await self.pc.setLocalDescription(await self.pc.createOffer())
+
         request = {"request": "configure"}
         request.update(media)
+
+        class PublishMessage(PluginMessage):
+            body: dict
+            jsep: dict
+
         await self.send(
-            {
-                "janus": "message",
-                "body": request,
-                "jsep": {
+            PublishMessage(
+                janus="message",
+                body=request,
+                jsep={
                     "sdp": self.pc.localDescription.sdp,
                     "trickle": False,
                     "type": self.pc.localDescription.type,
                 },
-            }
+            )
         )
 
-        # text = offer.sdp.as_text()
-        # logger.info("Sending offer and publishing:\n%s" % text)
-        # await self.send(
-        #     {
-        #         "janus": "message",
-        #         "body": {
-        #             "request": "publish",
-        #             "audio": True,
-        #             "video": True,
-        #         },
-        #         "jsep": {
-        #             "sdp": text,
-        #             "type": "offer",
-        #             "trickle": True,
-        #         },
-        #     }
-        # )
         await self.joined_event.wait()
 
     async def unpublish(self) -> None:
         """Stop publishing"""
+
+        class UnpublishMessage(PluginMessage):
+            body: dict
+
         await self.send(
-            {
-                "janus": "message",
-                "body": {
+            UnpublishMessage(
+                janus="message",
+                body={
                     "request": "unpublish",
                 },
-            }
+            )
         )
         await self.pc.close()
 
     async def subscribe(self, room_id: int, feed_id: int) -> None:
         """Subscribe to a feed
 
         :param room_id: Room ID containing the feed. The same ID that
@@ -211,46 +233,14 @@
                     "request": "listparticipants",
                     "room": room_id,
                 },
             }
         )
         return response["plugindata"]["data"]["participants"]
 
-    def on_negotiation_needed(self, element):
-        logger.info("on_negotiation_needed called")
-        self.gst_webrtc_ready.set()
-        # promise = Gst.Promise.new_with_change_func(self.on_offer_created, element, None)
-        # element.emit('create-offer', None, promise)
-
-    def send_ice_candidate_message(self, _, sdpMLineIndex, candidate):
-        icemsg = {"candidate": candidate, "sdpMLineIndex": sdpMLineIndex}
-        logger.info(f"Sending ICE {icemsg}")
-        # loop = asyncio.new_event_loop()
-        future = asyncio.run_coroutine_threadsafe(
-            self.trickle(sdpMLineIndex, candidate), self.loop
-        )
-        future.result()
-
-    def extract_ice_from_sdp(self, sdp):
-        mlineindex = -1
-        for line in sdp.splitlines():
-            if line.startswith("a=candidate"):
-                candidate = line[2:]
-                if mlineindex < 0:
-                    logger.info("Received ice candidate in SDP before any m= line")
-                    continue
-                logger.info(
-                    "Received remote ice-candidate mlineindex {}: {}".format(
-                        mlineindex, candidate
-                    )
-                )
-                self.webrtcbin.emit("add-ice-candidate", mlineindex, candidate)
-            elif line.startswith("m="):
-                mlineindex += 1
-
     async def handle_jsep(self, jsep):
         logger.info(jsep)
         if "sdp" in jsep:
             sdp = jsep["sdp"]
             if jsep["type"] == "answer":
                 logger.info(f"Received answer:\n{sdp}")
```

### Comparing `janus_client-0.2.5/LICENSE` & `janus_client-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `janus_client-0.2.5/pyproject.toml` & `janus_client-0.3.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "janus-client"
-version = "0.2.5"
+version = "0.3.0"
 description = "Janus webrtc client in async Python."
 authors = ["Joseph Lim <josephlim_94@hotmail.co.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "janus_client"}]
 repository = "https://github.com/josephlim94/janus_gst_client_py"
 classifiers = [
@@ -19,12 +19,13 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 websockets = "^11.0.3"
 aiortc = "^1.5.0"
 ffmpeg-python = "^0.2.0"
 numpy = "^1.25.1"
 av = "^10.0.0"
+pydantic = "^2.1.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

