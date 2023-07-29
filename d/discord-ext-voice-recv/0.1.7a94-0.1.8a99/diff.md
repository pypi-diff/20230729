# Comparing `tmp/discord-ext-voice_recv-0.1.7a94.tar.gz` & `tmp/discord-ext-voice_recv-0.1.8a99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-ext-voice_recv-0.1.7a94.tar", last modified: Sun Jul 23 07:21:04 2023, max compression
+gzip compressed data, was "discord-ext-voice_recv-0.1.8a99.tar", last modified: Sat Jul 29 00:59:47 2023, max compression
```

## Comparing `discord-ext-voice_recv-0.1.7a94.tar` & `discord-ext-voice_recv-0.1.8a99.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 07:21:04.939924 discord-ext-voice_recv-0.1.7a94/
--rw-rw-rw-   0        0        0     1091 2023-04-09 21:50:44.000000 discord-ext-voice_recv-0.1.7a94/LICENSE
--rw-rw-rw-   0        0        0     7879 2023-07-23 07:21:04.938925 discord-ext-voice_recv-0.1.7a94/PKG-INFO
--rw-rw-rw-   0        0        0     6852 2023-06-25 07:12:33.000000 discord-ext-voice_recv-0.1.7a94/README.md
-drwxrwxrwx   0        0        0        0 2023-07-23 07:21:04.888953 discord-ext-voice_recv-0.1.7a94/discord/
-drwxrwxrwx   0        0        0        0 2023-07-23 07:21:04.889959 discord-ext-voice_recv-0.1.7a94/discord/ext/
-drwxrwxrwx   0        0        0        0 2023-07-23 07:21:04.919936 discord-ext-voice_recv-0.1.7a94/discord/ext/voice_recv/
--rw-rw-rw-   0        0        0      362 2023-07-23 07:00:35.000000 discord-ext-voice_recv-0.1.7a94/discord/ext/voice_recv/__init__.py
--rw-rw-rw-   0        0        0     5487 2023-06-19 01:13:13.000000 discord-ext-voice_recv-0.1.7a94/discord/ext/voice_recv/buffer.py
--rw-rw-rw-   0        0        0     2982 2023-07-23 06:54:34.000000 discord-ext-voice_recv-0.1.7a94/discord/ext/voice_recv/gateway.py
--rw-rw-rw-   0        0        0    33786 2023-07-23 06:54:34.000000 discord-ext-voice_recv-0.1.7a94/discord/ext/voice_recv/opus.py
--rw-rw-rw-   0        0        0     8387 2023-06-22 02:45:57.000000 discord-ext-voice_recv-0.1.7a94/discord/ext/voice_recv/reader.py
--rw-rw-rw-   0        0        0    12486 2023-06-19 07:12:45.000000 discord-ext-voice_recv-0.1.7a94/discord/ext/voice_recv/rtp.py
--rw-rw-rw-   0        0        0      265 2023-07-23 06:54:34.000000 discord-ext-voice_recv-0.1.7a94/discord/ext/voice_recv/silence.py
--rw-rw-rw-   0        0        0     8742 2023-07-23 06:54:34.000000 discord-ext-voice_recv-0.1.7a94/discord/ext/voice_recv/sinks.py
--rw-rw-rw-   0        0        0      911 2023-06-17 04:25:42.000000 discord-ext-voice_recv-0.1.7a94/discord/ext/voice_recv/types.py
--rw-rw-rw-   0        0        0     2237 2023-04-09 21:50:44.000000 discord-ext-voice_recv-0.1.7a94/discord/ext/voice_recv/utils.py
--rw-rw-rw-   0        0        0     2623 2023-06-17 05:04:12.000000 discord-ext-voice_recv-0.1.7a94/discord/ext/voice_recv/video.py
--rw-rw-rw-   0        0        0     5707 2023-06-25 02:50:41.000000 discord-ext-voice_recv-0.1.7a94/discord/ext/voice_recv/voice_client.py
-drwxrwxrwx   0        0        0        0 2023-07-23 07:21:04.936937 discord-ext-voice_recv-0.1.7a94/discord_ext_voice_recv.egg-info/
--rw-rw-rw-   0        0        0     7879 2023-07-23 07:21:04.000000 discord-ext-voice_recv-0.1.7a94/discord_ext_voice_recv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      697 2023-07-23 07:21:04.000000 discord-ext-voice_recv-0.1.7a94/discord_ext_voice_recv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 07:21:04.000000 discord-ext-voice_recv-0.1.7a94/discord_ext_voice_recv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-05 23:03:01.000000 discord-ext-voice_recv-0.1.7a94/discord_ext_voice_recv.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       25 2023-07-23 07:21:04.000000 discord-ext-voice_recv-0.1.7a94/discord_ext_voice_recv.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-23 07:21:04.000000 discord-ext-voice_recv-0.1.7a94/discord_ext_voice_recv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-23 07:21:04.939924 discord-ext-voice_recv-0.1.7a94/setup.cfg
--rw-rw-rw-   0        0        0     1897 2023-07-23 07:07:48.000000 discord-ext-voice_recv-0.1.7a94/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 00:59:47.897738 discord-ext-voice_recv-0.1.8a99/
+-rw-rw-rw-   0        0        0     1091 2023-04-09 21:50:44.000000 discord-ext-voice_recv-0.1.8a99/LICENSE
+-rw-rw-rw-   0        0        0    10038 2023-07-29 00:59:47.896739 discord-ext-voice_recv-0.1.8a99/PKG-INFO
+-rw-rw-rw-   0        0        0     8952 2023-07-29 00:55:14.000000 discord-ext-voice_recv-0.1.8a99/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 00:59:47.795797 discord-ext-voice_recv-0.1.8a99/discord/
+drwxrwxrwx   0        0        0        0 2023-07-29 00:59:47.796796 discord-ext-voice_recv-0.1.8a99/discord/ext/
+drwxrwxrwx   0        0        0        0 2023-07-29 00:59:47.858761 discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/
+-rw-rw-rw-   0        0        0      362 2023-07-29 00:57:11.000000 discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/__init__.py
+-rw-rw-rw-   0        0        0     5487 2023-06-19 01:13:13.000000 discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/buffer.py
+-rw-rw-rw-   0        0        0     3278 2023-07-23 07:28:37.000000 discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/gateway.py
+-rw-rw-rw-   0        0        0    35866 2023-07-28 22:56:15.000000 discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/opus.py
+-rw-rw-rw-   0        0        0     8387 2023-06-22 02:45:57.000000 discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/reader.py
+-rw-rw-rw-   0        0        0    12486 2023-06-19 07:12:45.000000 discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/rtp.py
+-rw-rw-rw-   0        0        0     1617 2023-07-23 07:28:37.000000 discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/silence.py
+-rw-rw-rw-   0        0        0    12401 2023-07-29 00:55:44.000000 discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/sinks.py
+-rw-rw-rw-   0        0        0      911 2023-06-17 04:25:42.000000 discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/types.py
+-rw-rw-rw-   0        0        0     2237 2023-04-09 21:50:44.000000 discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/utils.py
+-rw-rw-rw-   0        0        0     2623 2023-06-17 05:04:12.000000 discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/video.py
+-rw-rw-rw-   0        0        0     5707 2023-07-28 22:01:55.000000 discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/voice_client.py
+drwxrwxrwx   0        0        0        0 2023-07-29 00:59:47.894740 discord-ext-voice_recv-0.1.8a99/discord_ext_voice_recv.egg-info/
+-rw-rw-rw-   0        0        0    10038 2023-07-29 00:59:47.000000 discord-ext-voice_recv-0.1.8a99/discord_ext_voice_recv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2023-07-29 00:59:47.000000 discord-ext-voice_recv-0.1.8a99/discord_ext_voice_recv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 00:59:47.000000 discord-ext-voice_recv-0.1.8a99/discord_ext_voice_recv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-05 23:03:01.000000 discord-ext-voice_recv-0.1.8a99/discord_ext_voice_recv.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       25 2023-07-29 00:59:47.000000 discord-ext-voice_recv-0.1.8a99/discord_ext_voice_recv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-29 00:59:47.000000 discord-ext-voice_recv-0.1.8a99/discord_ext_voice_recv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 00:59:47.897738 discord-ext-voice_recv-0.1.8a99/setup.cfg
+-rw-rw-rw-   0        0        0     1917 2023-07-23 07:43:28.000000 discord-ext-voice_recv-0.1.8a99/setup.py
```

### Comparing `discord-ext-voice_recv-0.1.7a94/LICENSE` & `discord-ext-voice_recv-0.1.8a99/LICENSE`

 * *Files identical despite different names*

### Comparing `discord-ext-voice_recv-0.1.7a94/PKG-INFO` & `discord-ext-voice_recv-0.1.8a99/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,146 +1,161 @@
-Metadata-Version: 2.1
-Name: discord-ext-voice_recv
-Version: 0.1.7a94
-Summary: Experimental voice receive extension for discord.py
-Home-page: https://github.com/imayhaveborkedit/discord-ext-voice-recv
-Author: Imayhaveborkedit
-License: MIT
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# discord-ext-voice-recv
-Voice receive extension package for discord.py
-
-### Warning
-**This extension should be more or less functional, but the code is not yet feature complete.  No guarantees are given for stability or random breaking changes.**
-
-## Installing
-**Python 3.8 or higher is required**
-
-`python -m pip install git+https://github.com/imayhaveborkedit/discord-ext-voice-recv`
-
-This package will be uploaded to pypi eventually.
-
-Naturally, this extension depends on `discord.py` being installed with voice support.
-
-## Example
-See the [example script](examples/recv.py).
-
-## Usage
-### VoiceRecvClient
-The class `voice_recv.VoiceRecvClient` must be used in `VoiceChannel.connect()` to use voice receive functionality.
-```python
-voice_client = await voice_channel.connect(cls=voice_recv.VoiceRecvClient)
-```
-
-### New voice client functions
-```python
-def listen(sink: voice_recv.AudioSink, *, after=None) -> None
-```
-Receives audio data into an `AudioSink`.  A sink is similar to the `AudioSource` class, where most of the logic is done in a single callback function, but in reverse.  Sinks are explained in detail in the [Sinks](#sinks) section below.
-
-The finalizer, `after` is called after the sink has been exhausted or an error occurred.  The callback signature is the same as the after callback for `play()`, one parameter for an optional Exception object.
-
-```python
-def is_listening() -> bool
-```
-Returns `True` if the voice client is currently receiving audio.  Specifically, if the bot is reading from the voice socket.
-
-```python
-def stop() -> None
-```
-This function has been altered to stop both receiving and sending of audio.
-
-```python
-def stop_listening() -> None
-```
-Stops receiving audio.
-
-```python
-def stop_playing() -> None
-```
-Stops playing audio.  This function is identical to `discord.VoiceClient.stop()`.
-
-## Sinks
-The api of this extension is designed to mirror the discord.py voice send api.  Sending audio uses the `AudioSource` class, while receiving audio uses the `AudioSink` class.  A sink is designed to be the inverse of a source.  Essentially, a source is a callback called by discord.py to produce a chunk of audio data.  Conversely, a sink is a callback called by the library to handle a chunk of audio.  Sinks can be composed in the same fashion as sources, creating an audio processing pipeline.  Sources and sinks can even combined into one object to handle both tasks, such as creating a feedback loop.
-
-Special care should be taken not to write excessively computationally expensive code, as python is not particularly well suited to realtime audio processing.
-
-Due to voice receive being somewhat more complex than voice sending, sinks have additional functionality compared to sources.  However, the core sink functions should look relatively familiar.
-
-```python
-class MySink(voice_recv.AudioSink):
-    def __init__(self):
-        super().__init__()
-
-    def wants_opus(self) -> bool:
-        return False
-
-    def write(self, user: Optional[User | Member], data: VoiceData):
-        ...
-
-    def cleanup(self):
-        ...
-```
-
-These are the main functions of a sink, names and purpose reflecting that of their source counterparts.  It is important to note that `super().__init__()` must be called when inheriting from `AudioSink`, in contrast to `AudioSource` which does not have a default `__init__` function.
-
-- The `wants_opus()` function determines if the sink should receive opus packets or decoded PCM packets.  Care should be taken not to unintentionally mix sinks that want different types.
-- The `write()` function is the main callback, where the sink logic takes place.  In a sink pipeline, this could alter, inspect, or log a packet, and then write it to a child sink.  `VoiceData` is a simple container class with attributes for the origin member, opus data, optionally pcm data, and raw audio packet.
-- The `cleanup()` function is identical to `AudioSource.cleanup()`, a finalizer to cleanup any loose ends when the sink has finished its job.
-
-In addition, sinks also have properties for their `voice_client`, as well as `parent` and `child`/`children` sinks.  Furthermore, sinks will be able to receive events in a similar manner to cogs, but this has not been implemented yet. (TODO)
-
-This extension comes with several useful built in sinks, which I will briefly explain another time.  For now just [source dive](discord/ext/voice_recv/sinks.py).  (TODO)
-
-## New events
-```python
-async def on_voice_member_speak(member: discord.Member, ssrc: int)
-```
-Called when a member first speaks (transmits audio) in a voice channel.  This event is only called once per their voice session (ssrc assignment).  Any packets received from this member before this event fires can (probably) be safely ignored since they are likely just silence packets.  The main purpose of this event is to reveal the ssrc of a member, to map packets to their originating member.
-
-This is **NOT** a speaking indicator event.  The speaking indicator is determined by packet activity.  This functionality will be added in the future.
-
-```python
-async def on_voice_member_disconnect(member: discord.Member, ssrc: int)
-```
-Called when a member disconnects from a voice channel. The `ssrc` parameter is the unique id a member has to identify which packets belong to them.  This is useful when using custom sinks, particularly those that handle packets from multiple members.
-
-```python
-async def on_voice_member_video(member: discord.Member, data: voice_recv.VoiceVideoStreams)
-```
-Called when a member in voice channel toggles their webcam on or off, NOT screenshare.  Screenshare status is only indicated in the `self_video` attribute of `discord.VoiceState`.
-
-```python
-async def on_voice_member_flags(member: discord.Member, flags: Optional[int])
-```
-An undocumented event dispatched when a member joins a voice channel containing a flags bitfield.  Only values `0`, `2`, and `None` have been observed so far, but their meaning remains unknown.
-
-```python
-async def on_voice_member_platform(member: discord.Member, platform: Optional[int | str])
-```
-An undocumented event dispatched when a member joins a voice channel containing a platform key, presumably with what platform the member joined on.  However, this field has only ever been seen to contain `None`.
-
-## Currently missing features
-- Sink events (similar to cog event handlers)
-- Silence generation (will be implemented as an included AudioSink)
-- Member speaking state status/event (design not yet decided)
-- Various internal impl details to maintain audio stability and consistency
-
-## Future plans
-- Muxer AudioSink (mixes multiple audio streams into a single stream)
-- Rust implementations of some components for improved performance
-- Alternative voice client implementation with a minimal interface intended for use with external data processing
+# discord-ext-voice-recv
+Voice receive extension package for discord.py
+
+## Warning
+**This extension should be more or less functional, but the code is not yet feature complete.  No guarantees are given for stability or random breaking changes.**
+
+## Installing
+**Python 3.8 or higher is required**, preferably 3.11 or whatever is latest
+
+```
+python -m pip install discord-ext-voice-recv
+```
+
+To install directly from github:
+```
+python -m pip install git+https://github.com/imayhaveborkedit/discord-ext-voice-recv
+```
+
+Naturally, this extension depends on `discord.py` being installed with voice support (`pynacl`).
+
+## Example
+See the [example script](examples/recv.py).
+
+## Feature overview
+### Custom VoiceProtocol client
+No monkey patching or bizarre hacks required.  Simply use the library feature to use `VoiceRecvClient` as the voice client class.  See [Usage](#usage).
+
+### Six new events
+This extension adds the unimplemented voice websocket events and one virtual event.  See [New Events](#new-events).
+
+### Simple and familiar API
+The overall API is designed to mirror the discord.py voice send API, with `AudioSink` being the counterpart to the existing `AudioSource`.  See [Sinks](#sinks).
+
+### Convenient included utilities
+Batteries included in the form of useful built in `AudioSinks`.  Some to match their `AudioSource` counterpart, some I merely considered useful.  See... uh... TODO.
+
+### More or less typed
+Its probably fine.
+
+## Usage
+### VoiceRecvClient
+The class `voice_recv.VoiceRecvClient` must be used in `VoiceChannel.connect()` to use voice receive functionality.
+```python
+voice_client = await voice_channel.connect(cls=voice_recv.VoiceRecvClient)
+```
+
+### New voice client functions
+```python
+def listen(sink: voice_recv.AudioSink, *, after=None) -> None
+```
+Receives audio data into an `AudioSink`.  A sink is similar to the `AudioSource` class, where most of the logic is done in a single callback function, but in reverse.  Sinks are explained in detail in the [Sinks](#sinks) section below.
+
+The finalizer, `after` is called after the sink has been exhausted or an error occurred.  The callback signature is the same as the after callback for `play()`, one parameter for an optional Exception object.
+
+```python
+def is_listening() -> bool
+```
+Returns `True` if the voice client is currently receiving audio.  Specifically, if the bot is reading from the voice socket.
+
+```python
+def stop() -> None
+```
+This function has been altered to stop both receiving and sending of audio.
+
+```python
+def stop_listening() -> None
+```
+Stops receiving audio.
+
+```python
+def stop_playing() -> None
+```
+Stops playing audio.  This function is identical to `discord.VoiceClient.stop()`.
+
+## Sinks
+The api of this extension is designed to mirror the discord.py voice send api.  Sending audio uses the `AudioSource` class, while receiving audio uses the `AudioSink` class.  A sink is designed to be the inverse of a source.  Essentially, a source is a callback called by discord.py to produce a chunk of audio data.  Conversely, a sink is a callback called by the library to handle a chunk of audio.  Sinks can be composed in the same fashion as sources, creating an audio processing pipeline.  Sources and sinks can even combined into one object to handle both tasks, such as creating a feedback loop.
+
+Special care should be taken not to write excessively computationally expensive code, as python is not particularly well suited to realtime audio processing.
+
+Due to voice receive being somewhat more complex than voice sending, sinks have additional functionality compared to sources.  However, the core sink functions should look relatively familiar.
+
+```python
+class MySink(voice_recv.AudioSink):
+    def __init__(self):
+        super().__init__()
+
+    def wants_opus(self) -> bool:
+        return False
+
+    def write(self, user: User | Member | None, data: VoiceData):
+        ...
+
+    def cleanup(self):
+        ...
+```
+
+These are the main functions of a sink, names and purpose reflecting that of their source counterparts.  It is important to note that `super().__init__()` must be called when inheriting from `AudioSink`, in contrast to `AudioSource` which does not have a default `__init__` function.
+
+- The `wants_opus()` function determines if the sink should receive opus packets or decoded PCM packets.  Care should be taken not to unintentionally mix sinks that want different types.
+- The `write()` function is the main callback, where the sink logic takes place.  In a sink pipeline, this could alter, inspect, or log a packet, and then write it to a child sink.  `VoiceData` is a simple container class with attributes for the origin member, opus data, optionally pcm data, and raw audio packet.
+- The `cleanup()` function is identical to `AudioSource.cleanup()`, a finalizer to cleanup any loose ends when the sink has finished its job.
+
+Additionally, sinks also have properties for their `voice_client`, as well as `parent` and `child`/`children` sinks.
+
+This extension comes with several useful built in sinks, which I will briefly explain another time.  For now just [source dive](discord/ext/voice_recv/sinks.py).  (TODO)
+
+### Sink event listeners
+With AudioSinks being potentially more complex and stateful than AudioSources and the addition of new events, it is sometimes necessary to handle events in the context of a sink.  It would be rather awkward to have to register a sink function with `commands.Bot.add_listener()` while dealing with thread safety, and even moreso using `discord.Client`.  To remedy this, listeners can be defined within sinks, similarly to how they work in Cogs.
+
+```python
+class MySink(AudioSink):
+    @AudioSink.listener()
+    def on_voice_member_disconnect(self, member: discord.Member, ssrc: int | None):
+        print(f"{member} has disconnected")
+        self.do_something_like_handle_disconnect(ssrc)
+```
+
+Note that these functions must be sync functions, as they are dispatched from a thread.  Trying to use a coroutine will result in an error.  This restriction only applies to sink listeners, and normal async event listeners will function as per usual.  The event listener dispatch thread is different from the one used to dispatch the `write()` callback so potential threadsafety issues should be considered.  A decorator argument to run the event callback in the other thread may be added later.
+
+## New events
+```python
+async def on_voice_member_speak(member: discord.Member, ssrc: int)
+```
+Called when a member first speaks (transmits audio) in a voice channel.  This event is only called once per their voice session (ssrc assignment).  Any packets received from this member before this event fires can (probably) be safely ignored since they are likely just silence packets.  The main purpose of this event is to reveal the ssrc of a member, to map packets to their originating member.
+
+This is **NOT** a speaking indicator event.  The speaking indicator is determined by packet activity.  This functionality will be added in the future.
+
+```python
+async def on_voice_member_disconnect(member: discord.Member, ssrc: int | None)
+```
+Called when a member disconnects from a voice channel. The `ssrc` parameter is the unique id a member has to identify which packets belong to them.  This is useful when using custom sinks, particularly those that handle packets from multiple members.
+
+```python
+async def on_voice_member_video(member: discord.Member, data: voice_recv.VoiceVideoStreams)
+```
+Called when a member in voice channel toggles their webcam on or off, NOT screenshare.  Screenshare status is only indicated in the `self_video` attribute of `discord.VoiceState`.
+
+```python
+async def on_voice_member_flags(member: discord.Member, flags: int | None)
+```
+An undocumented event dispatched when a member joins a voice channel containing a flags bitfield.  Only values `0`, `2`, and `None` have been observed so far, but their meaning remains unknown.
+
+```python
+async def on_voice_member_platform(member: discord.Member, platform: int | str | None)
+```
+An undocumented event dispatched when a member joins a voice channel containing a platform key, presumably with what platform the member joined on.  However, this field has only ever been seen to contain `None`.
+
+```python
+def on_rtcp_packet(packet: RTCPPacket, guild: discord.Guild)
+```
+A virtual event for when an RTCP packet is received.  This event only works inside of sinks, so it cannot be async.
+
+## Currently missing features
+- Silence generation (will be implemented as an included AudioSink)
+- Member speaking state status/event (design not yet decided)
+- Various internal impl details to maintain audio stability and consistency
+
+## Future plans
+- Muxer AudioSink (mixes multiple audio streams into a single stream)
+- Rust implementations of some components for improved performance
+- Alternative voice client implementation with a minimal interface intended for use with external data processing
```

### Comparing `discord-ext-voice_recv-0.1.7a94/README.md` & `discord-ext-voice_recv-0.1.8a99/discord_ext_voice_recv.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,123 +1,184 @@
-# discord-ext-voice-recv
-Voice receive extension package for discord.py
-
-### Warning
-**This extension should be more or less functional, but the code is not yet feature complete.  No guarantees are given for stability or random breaking changes.**
-
-## Installing
-**Python 3.8 or higher is required**
-
-`python -m pip install git+https://github.com/imayhaveborkedit/discord-ext-voice-recv`
-
-This package will be uploaded to pypi eventually.
-
-Naturally, this extension depends on `discord.py` being installed with voice support.
-
-## Example
-See the [example script](examples/recv.py).
-
-## Usage
-### VoiceRecvClient
-The class `voice_recv.VoiceRecvClient` must be used in `VoiceChannel.connect()` to use voice receive functionality.
-```python
-voice_client = await voice_channel.connect(cls=voice_recv.VoiceRecvClient)
-```
-
-### New voice client functions
-```python
-def listen(sink: voice_recv.AudioSink, *, after=None) -> None
-```
-Receives audio data into an `AudioSink`.  A sink is similar to the `AudioSource` class, where most of the logic is done in a single callback function, but in reverse.  Sinks are explained in detail in the [Sinks](#sinks) section below.
-
-The finalizer, `after` is called after the sink has been exhausted or an error occurred.  The callback signature is the same as the after callback for `play()`, one parameter for an optional Exception object.
-
-```python
-def is_listening() -> bool
-```
-Returns `True` if the voice client is currently receiving audio.  Specifically, if the bot is reading from the voice socket.
-
-```python
-def stop() -> None
-```
-This function has been altered to stop both receiving and sending of audio.
-
-```python
-def stop_listening() -> None
-```
-Stops receiving audio.
-
-```python
-def stop_playing() -> None
-```
-Stops playing audio.  This function is identical to `discord.VoiceClient.stop()`.
-
-## Sinks
-The api of this extension is designed to mirror the discord.py voice send api.  Sending audio uses the `AudioSource` class, while receiving audio uses the `AudioSink` class.  A sink is designed to be the inverse of a source.  Essentially, a source is a callback called by discord.py to produce a chunk of audio data.  Conversely, a sink is a callback called by the library to handle a chunk of audio.  Sinks can be composed in the same fashion as sources, creating an audio processing pipeline.  Sources and sinks can even combined into one object to handle both tasks, such as creating a feedback loop.
-
-Special care should be taken not to write excessively computationally expensive code, as python is not particularly well suited to realtime audio processing.
-
-Due to voice receive being somewhat more complex than voice sending, sinks have additional functionality compared to sources.  However, the core sink functions should look relatively familiar.
-
-```python
-class MySink(voice_recv.AudioSink):
-    def __init__(self):
-        super().__init__()
-
-    def wants_opus(self) -> bool:
-        return False
-
-    def write(self, user: Optional[User | Member], data: VoiceData):
-        ...
-
-    def cleanup(self):
-        ...
-```
-
-These are the main functions of a sink, names and purpose reflecting that of their source counterparts.  It is important to note that `super().__init__()` must be called when inheriting from `AudioSink`, in contrast to `AudioSource` which does not have a default `__init__` function.
-
-- The `wants_opus()` function determines if the sink should receive opus packets or decoded PCM packets.  Care should be taken not to unintentionally mix sinks that want different types.
-- The `write()` function is the main callback, where the sink logic takes place.  In a sink pipeline, this could alter, inspect, or log a packet, and then write it to a child sink.  `VoiceData` is a simple container class with attributes for the origin member, opus data, optionally pcm data, and raw audio packet.
-- The `cleanup()` function is identical to `AudioSource.cleanup()`, a finalizer to cleanup any loose ends when the sink has finished its job.
-
-In addition, sinks also have properties for their `voice_client`, as well as `parent` and `child`/`children` sinks.  Furthermore, sinks will be able to receive events in a similar manner to cogs, but this has not been implemented yet. (TODO)
-
-This extension comes with several useful built in sinks, which I will briefly explain another time.  For now just [source dive](discord/ext/voice_recv/sinks.py).  (TODO)
-
-## New events
-```python
-async def on_voice_member_speak(member: discord.Member, ssrc: int)
-```
-Called when a member first speaks (transmits audio) in a voice channel.  This event is only called once per their voice session (ssrc assignment).  Any packets received from this member before this event fires can (probably) be safely ignored since they are likely just silence packets.  The main purpose of this event is to reveal the ssrc of a member, to map packets to their originating member.
-
-This is **NOT** a speaking indicator event.  The speaking indicator is determined by packet activity.  This functionality will be added in the future.
-
-```python
-async def on_voice_member_disconnect(member: discord.Member, ssrc: int)
-```
-Called when a member disconnects from a voice channel. The `ssrc` parameter is the unique id a member has to identify which packets belong to them.  This is useful when using custom sinks, particularly those that handle packets from multiple members.
-
-```python
-async def on_voice_member_video(member: discord.Member, data: voice_recv.VoiceVideoStreams)
-```
-Called when a member in voice channel toggles their webcam on or off, NOT screenshare.  Screenshare status is only indicated in the `self_video` attribute of `discord.VoiceState`.
-
-```python
-async def on_voice_member_flags(member: discord.Member, flags: Optional[int])
-```
-An undocumented event dispatched when a member joins a voice channel containing a flags bitfield.  Only values `0`, `2`, and `None` have been observed so far, but their meaning remains unknown.
-
-```python
-async def on_voice_member_platform(member: discord.Member, platform: Optional[int | str])
-```
-An undocumented event dispatched when a member joins a voice channel containing a platform key, presumably with what platform the member joined on.  However, this field has only ever been seen to contain `None`.
-
-## Currently missing features
-- Sink events (similar to cog event handlers)
-- Silence generation (will be implemented as an included AudioSink)
-- Member speaking state status/event (design not yet decided)
-- Various internal impl details to maintain audio stability and consistency
-
-## Future plans
-- Muxer AudioSink (mixes multiple audio streams into a single stream)
-- Rust implementations of some components for improved performance
-- Alternative voice client implementation with a minimal interface intended for use with external data processing
+Metadata-Version: 2.1
+Name: discord-ext-voice-recv
+Version: 0.1.8a99
+Summary: Experimental voice receive extension for discord.py
+Home-page: https://github.com/imayhaveborkedit/discord-ext-voice-recv
+Author: Imayhaveborkedit
+License: MIT
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS
+Classifier: Topic :: Multimedia :: Sound/Audio :: Capture/Recording
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# discord-ext-voice-recv
+Voice receive extension package for discord.py
+
+## Warning
+**This extension should be more or less functional, but the code is not yet feature complete.  No guarantees are given for stability or random breaking changes.**
+
+## Installing
+**Python 3.8 or higher is required**, preferably 3.11 or whatever is latest
+
+```
+python -m pip install discord-ext-voice-recv
+```
+
+To install directly from github:
+```
+python -m pip install git+https://github.com/imayhaveborkedit/discord-ext-voice-recv
+```
+
+Naturally, this extension depends on `discord.py` being installed with voice support (`pynacl`).
+
+## Example
+See the [example script](examples/recv.py).
+
+## Feature overview
+### Custom VoiceProtocol client
+No monkey patching or bizarre hacks required.  Simply use the library feature to use `VoiceRecvClient` as the voice client class.  See [Usage](#usage).
+
+### Six new events
+This extension adds the unimplemented voice websocket events and one virtual event.  See [New Events](#new-events).
+
+### Simple and familiar API
+The overall API is designed to mirror the discord.py voice send API, with `AudioSink` being the counterpart to the existing `AudioSource`.  See [Sinks](#sinks).
+
+### Convenient included utilities
+Batteries included in the form of useful built in `AudioSinks`.  Some to match their `AudioSource` counterpart, some I merely considered useful.  See... uh... TODO.
+
+### More or less typed
+Its probably fine.
+
+## Usage
+### VoiceRecvClient
+The class `voice_recv.VoiceRecvClient` must be used in `VoiceChannel.connect()` to use voice receive functionality.
+```python
+voice_client = await voice_channel.connect(cls=voice_recv.VoiceRecvClient)
+```
+
+### New voice client functions
+```python
+def listen(sink: voice_recv.AudioSink, *, after=None) -> None
+```
+Receives audio data into an `AudioSink`.  A sink is similar to the `AudioSource` class, where most of the logic is done in a single callback function, but in reverse.  Sinks are explained in detail in the [Sinks](#sinks) section below.
+
+The finalizer, `after` is called after the sink has been exhausted or an error occurred.  The callback signature is the same as the after callback for `play()`, one parameter for an optional Exception object.
+
+```python
+def is_listening() -> bool
+```
+Returns `True` if the voice client is currently receiving audio.  Specifically, if the bot is reading from the voice socket.
+
+```python
+def stop() -> None
+```
+This function has been altered to stop both receiving and sending of audio.
+
+```python
+def stop_listening() -> None
+```
+Stops receiving audio.
+
+```python
+def stop_playing() -> None
+```
+Stops playing audio.  This function is identical to `discord.VoiceClient.stop()`.
+
+## Sinks
+The api of this extension is designed to mirror the discord.py voice send api.  Sending audio uses the `AudioSource` class, while receiving audio uses the `AudioSink` class.  A sink is designed to be the inverse of a source.  Essentially, a source is a callback called by discord.py to produce a chunk of audio data.  Conversely, a sink is a callback called by the library to handle a chunk of audio.  Sinks can be composed in the same fashion as sources, creating an audio processing pipeline.  Sources and sinks can even combined into one object to handle both tasks, such as creating a feedback loop.
+
+Special care should be taken not to write excessively computationally expensive code, as python is not particularly well suited to realtime audio processing.
+
+Due to voice receive being somewhat more complex than voice sending, sinks have additional functionality compared to sources.  However, the core sink functions should look relatively familiar.
+
+```python
+class MySink(voice_recv.AudioSink):
+    def __init__(self):
+        super().__init__()
+
+    def wants_opus(self) -> bool:
+        return False
+
+    def write(self, user: User | Member | None, data: VoiceData):
+        ...
+
+    def cleanup(self):
+        ...
+```
+
+These are the main functions of a sink, names and purpose reflecting that of their source counterparts.  It is important to note that `super().__init__()` must be called when inheriting from `AudioSink`, in contrast to `AudioSource` which does not have a default `__init__` function.
+
+- The `wants_opus()` function determines if the sink should receive opus packets or decoded PCM packets.  Care should be taken not to unintentionally mix sinks that want different types.
+- The `write()` function is the main callback, where the sink logic takes place.  In a sink pipeline, this could alter, inspect, or log a packet, and then write it to a child sink.  `VoiceData` is a simple container class with attributes for the origin member, opus data, optionally pcm data, and raw audio packet.
+- The `cleanup()` function is identical to `AudioSource.cleanup()`, a finalizer to cleanup any loose ends when the sink has finished its job.
+
+Additionally, sinks also have properties for their `voice_client`, as well as `parent` and `child`/`children` sinks.
+
+This extension comes with several useful built in sinks, which I will briefly explain another time.  For now just [source dive](discord/ext/voice_recv/sinks.py).  (TODO)
+
+### Sink event listeners
+With AudioSinks being potentially more complex and stateful than AudioSources and the addition of new events, it is sometimes necessary to handle events in the context of a sink.  It would be rather awkward to have to register a sink function with `commands.Bot.add_listener()` while dealing with thread safety, and even moreso using `discord.Client`.  To remedy this, listeners can be defined within sinks, similarly to how they work in Cogs.
+
+```python
+class MySink(AudioSink):
+    @AudioSink.listener()
+    def on_voice_member_disconnect(self, member: discord.Member, ssrc: int | None):
+        print(f"{member} has disconnected")
+        self.do_something_like_handle_disconnect(ssrc)
+```
+
+Note that these functions must be sync functions, as they are dispatched from a thread.  Trying to use a coroutine will result in an error.  This restriction only applies to sink listeners, and normal async event listeners will function as per usual.  The event listener dispatch thread is different from the one used to dispatch the `write()` callback so potential threadsafety issues should be considered.  A decorator argument to run the event callback in the other thread may be added later.
+
+## New events
+```python
+async def on_voice_member_speak(member: discord.Member, ssrc: int)
+```
+Called when a member first speaks (transmits audio) in a voice channel.  This event is only called once per their voice session (ssrc assignment).  Any packets received from this member before this event fires can (probably) be safely ignored since they are likely just silence packets.  The main purpose of this event is to reveal the ssrc of a member, to map packets to their originating member.
+
+This is **NOT** a speaking indicator event.  The speaking indicator is determined by packet activity.  This functionality will be added in the future.
+
+```python
+async def on_voice_member_disconnect(member: discord.Member, ssrc: int | None)
+```
+Called when a member disconnects from a voice channel. The `ssrc` parameter is the unique id a member has to identify which packets belong to them.  This is useful when using custom sinks, particularly those that handle packets from multiple members.
+
+```python
+async def on_voice_member_video(member: discord.Member, data: voice_recv.VoiceVideoStreams)
+```
+Called when a member in voice channel toggles their webcam on or off, NOT screenshare.  Screenshare status is only indicated in the `self_video` attribute of `discord.VoiceState`.
+
+```python
+async def on_voice_member_flags(member: discord.Member, flags: int | None)
+```
+An undocumented event dispatched when a member joins a voice channel containing a flags bitfield.  Only values `0`, `2`, and `None` have been observed so far, but their meaning remains unknown.
+
+```python
+async def on_voice_member_platform(member: discord.Member, platform: int | str | None)
+```
+An undocumented event dispatched when a member joins a voice channel containing a platform key, presumably with what platform the member joined on.  However, this field has only ever been seen to contain `None`.
+
+```python
+def on_rtcp_packet(packet: RTCPPacket, guild: discord.Guild)
+```
+A virtual event for when an RTCP packet is received.  This event only works inside of sinks, so it cannot be async.
+
+## Currently missing features
+- Silence generation (will be implemented as an included AudioSink)
+- Member speaking state status/event (design not yet decided)
+- Various internal impl details to maintain audio stability and consistency
+
+## Future plans
+- Muxer AudioSink (mixes multiple audio streams into a single stream)
+- Rust implementations of some components for improved performance
+- Alternative voice client implementation with a minimal interface intended for use with external data processing
```

### Comparing `discord-ext-voice_recv-0.1.7a94/discord/ext/voice_recv/buffer.py` & `discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/buffer.py`

 * *Files identical despite different names*

### Comparing `discord-ext-voice_recv-0.1.7a94/discord/ext/voice_recv/gateway.py` & `discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/gateway.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,24 @@
 
 
 async def hook(self: DiscordVoiceWebSocket, msg: dict):
     op: int = msg['op']
     data: dict = msg.get('d') # type: ignore
     vc: VoiceRecvClient = self._connection # type: ignore
 
+    from pprint import pformat
+    if op not in (3, 6):
+        log.debug("Received op %s: \n%s", op, pformat(data, compact=True))
+
+        if len(msg.keys()) > 2:
+            m = msg.copy()
+            m.pop('op')
+            m.pop('d')
+            log.info("WS payload has extra keys: %s", m)
+
     if op == self.READY:
         self.ssrc: int = data['ssrc'] # type: ignore
         vc._add_ssrc(vc.client.user.id, data['ssrc']) # type: ignore
 
     elif op == self.SESSION_DESCRIPTION:
         # log.info("Doing voice hacks")
         # await _do_hacks(self)
```

### Comparing `discord-ext-voice_recv-0.1.7a94/discord/ext/voice_recv/opus.py` & `discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/opus.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,22 +13,27 @@
 from .rtp import *
 
 import discord
 
 from discord.opus import Decoder
 
 if TYPE_CHECKING:
-    from typing import Deque, Optional, Tuple, Dict
+    from typing import Optional, Tuple, Dict, Callable, Any
+    from queue import SimpleQueue
     from .sinks import AudioSink
+    from .voice_client import VoiceRecvClient
 
     AudioPacket = RTPPacket | FakePacket
     # Packet = AudioPacket | SilencePacket
     Packet = AudioPacket
     User = discord.User | discord.Member
 
+    EventCB = Callable[..., Any]
+    EventData = Tuple[str, Tuple[Any], Dict[str, Any]]
+
 log = logging.getLogger(__name__)
 
 __all__ = [
     "VoiceData"
 ]
 
 
@@ -53,24 +58,27 @@
 class PacketRouter:
     """docstring for PacketRouter"""
 
     def __init__(self, sink: AudioSink):
         self.sink = sink
         self.decoders: Dict[int, PacketDecoder] = {}
 
-        self._rtcp_buffer = queue.Queue()
+        self._event_listeners: dict[str, list[EventCB]] = {}
+        self._event_buffer: SimpleQueue[EventData] = queue.SimpleQueue()
         self._lock = threading.RLock()
         self._end_writer = threading.Event()
 
-        self._rtcp_writer = threading.Thread(
-            target=self._rtcp_loop,
+        self._event_writer = threading.Thread(
+            target=self._event_loop,
             daemon=True,
-            name=f"rtcp-writer-{id(self):x}"
+            name=f"event-writer-{id(self):x}"
         )
-        self._rtcp_writer.start()
+        self._event_writer.start()
+
+        self.register_events()
 
     def _get_decoder(self, ssrc: int) -> PacketDecoder:
         decoder = self.decoders.get(ssrc, None)
 
         if decoder is None:
             log.debug("Creating decoder for ssrc %s", ssrc)
             decoder = self.decoders.setdefault(ssrc, PacketDecoder(self.sink, ssrc))
@@ -78,41 +86,84 @@
         return decoder
 
     def feed_rtp(self, packet: RTPPacket):
         decoder = self._get_decoder(packet.ssrc)
         decoder.feed_rtp(packet)
 
     def feed_rtcp(self, packet: RTCPPacket):
-        self._rtcp_buffer.put_nowait(packet)
+        guild = self.sink.voice_client.guild if self.sink.voice_client else None
+        self.dispatch('rtcp_packet', packet, guild)
 
-    def _rtcp_loop(self):
+    def _event_loop(self):
         while not self._end_writer.is_set():
             try:
-                rtcp_packet = self._rtcp_buffer.get(timeout=2)
+                event, args, kwargs = self._event_buffer.get(timeout=0.5)
             except queue.Empty:
                 continue
             else:
                 with self._lock:
-                    self.sink.write_rtcp(rtcp_packet)
+                    self._dispatch_to_listeners(event, *args, **kwargs)
+
+    def register_events(self):
+        with self._lock:
+            self._register_listeners(self.sink)
+            for child in self.sink.walk_children():
+                self._register_listeners(child)
+
+    def _register_listeners(self, sink: AudioSink):
+        log.warning("registering events for %s", self.sink)
+        log.warning("listeners: %s", self.sink.__sink_listeners__)
+
+        for name, method_name in sink.__sink_listeners__:
+            func = getattr(sink, method_name)
+
+            log.warning("Registering %s for %s", name, method_name)
+            if name in self._event_listeners:
+                self._event_listeners[name].append(func)
+            else:
+                self._event_listeners[name] = [func]
+
+    def unregister_events(self):
+        with self._lock:
+            self._unregister_listeners(self.sink)
+            for child in self.sink.walk_children():
+                self._unregister_listeners(child)
+
+    def _unregister_listeners(self, sink: AudioSink):
+        for name, method_name in sink.__sink_listeners__:
+            func = getattr(sink, method_name)
+
+            if name in self._event_listeners:
+                try:
+                    self._event_listeners[name].remove(func)
+                except ValueError:
+                    pass
 
     def set_sink(self, sink: AudioSink):
         with self._lock:
+            self.unregister_events()
             self.sink = sink
 
             for decoder in self.decoders.values():
                 decoder.set_sink(sink)
 
+            self.register_events()
+
     def notify(self, ssrc: int, user_id: int):
         decoder = self.decoders.get(ssrc, None)
 
         if decoder is not None:
             decoder.notify(user_id)
 
-    def dispatch(self, event: str, *args, **kwargs):
-        ...
+    def dispatch(self, event: str, *args: Any, **kwargs: Any):
+        self._event_buffer.put_nowait((event, args, kwargs))
+
+    def _dispatch_to_listeners(self, event: str, *args: Any, **kwargs: Any):
+        for listener in self._event_listeners.get(f'on_{event}', []):
+            listener(*args, **kwargs)
 
     def destroy_decoder(self, ssrc: int):
         with self._lock:
             decoder = self.decoders.pop(ssrc, None)
 
             if decoder:
                 decoder.flush()
@@ -174,15 +225,15 @@
 
         self._end_thread = threading.Event()
         self._lock = threading.Lock()
 
         self.start() # no way this causes any problems haha
 
     def _get_user(self, user_id: int) -> Optional[User]:
-        vc = self.sink.voice_client
+        vc: VoiceRecvClient = self.sink.voice_client # type: ignore
         return vc.guild.get_member(user_id) or vc.client.get_user(user_id)
 
     def _get_cached_member(self) -> Optional[User]:
         return self._get_user(self._cached_id) if self._cached_id else None
 
     def feed_rtp(self, packet: RTPPacket):
         if self._end_thread.is_set():
@@ -284,15 +335,15 @@
         pcm = None
         if not self.sink.wants_opus():
             packet, pcm = self._handle_decode(packet)
 
         member = self._get_cached_member()
 
         if not member:
-            self._cached_id = self.sink.voice_client._get_id_from_ssrc(self.ssrc)
+            self._cached_id = self.sink.voice_client._get_id_from_ssrc(self.ssrc) # type: ignore
             member = self._get_cached_member()
 
         data = VoiceData(packet, member, pcm=pcm)
 
         self.sink.write(member, data)
         self._last_seq = packet.sequence
         self._last_ts = packet.timestamp
```

### Comparing `discord-ext-voice_recv-0.1.7a94/discord/ext/voice_recv/reader.py` & `discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/reader.py`

 * *Files identical despite different names*

### Comparing `discord-ext-voice_recv-0.1.7a94/discord/ext/voice_recv/rtp.py` & `discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/rtp.py`

 * *Files identical despite different names*

### Comparing `discord-ext-voice_recv-0.1.7a94/discord/ext/voice_recv/sinks.py` & `discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/sinks.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import abc
 import time
 import wave
+import inspect
 import audioop
 import logging
 
-from typing import TYPE_CHECKING
-
 from .opus import VoiceData
+from .silence import SilenceGenerator
 
 import discord
 
+from discord.utils import MISSING
 from discord.opus import Decoder as OpusDecoder
 
+from typing import TYPE_CHECKING
+
 if TYPE_CHECKING:
-    from typing import Callable, Optional, Any, IO, Sequence
+    from typing import Callable, Optional, Any, IO, Sequence, Tuple, Generator
 
     from .rtp import RTPPacket, RTCPPacket, FakePacket
     from .voice_client import VoiceRecvClient
     from .opus import VoiceData
 
     Packet = RTPPacket | FakePacket
     User = discord.User | discord.Member
@@ -48,17 +51,47 @@
 class VoiceRecvException(discord.DiscordException):
     """Generic exception for voice recv related errors"""
 
     def __init__(self, message: str):
         self.message = message
 
 
-class BaseSink(metaclass=abc.ABCMeta):
-    _voice_client: Optional[VoiceRecvClient] = None
-    _parent: Optional[AudioSink] = None
+class SinkMeta(abc.ABCMeta):
+    __sink_listeners__: list[Tuple[str, str]]
+
+    def __new__(cls, name: str, bases: Tuple[type, ...], attrs: dict[str, Any], **kwargs):
+        listeners: dict[str, Any] = {}
+        new_cls = super().__new__(cls, name, bases, attrs, **kwargs)
+
+        for base in reversed(new_cls.__mro__):
+            for elem, value in base.__dict__.items():
+                # If it exists in a subclass, delete the higher level one
+                if elem in listeners:
+                    del listeners[elem]
+
+                is_static_method = isinstance(value, staticmethod)
+                if is_static_method:
+                    value = value.__func__
+
+                if not hasattr(value, '__sink_listener__'):
+                    continue
+
+                listeners[elem] = value
+
+        listener_list = []
+        for listener in listeners.values():
+            for listener_name in listener.__sink_listener_names__:
+                listener_list.append((listener_name, listener.__name__))
+
+        new_cls.__sink_listeners__ = listener_list
+        return new_cls
+
+# TODO: replace AudioSink hints with a sink generic
+class SinkABC(metaclass=SinkMeta):
+    __sink_listeners__: list[Tuple[str, str]]
 
     @property
     @abc.abstractmethod
     def parent(self) -> Optional[AudioSink]:
         raise NotImplementedError
 
     @property
@@ -67,14 +100,19 @@
         raise NotImplementedError
 
     @property
     @abc.abstractmethod
     def children(self) -> Sequence[AudioSink]:
         raise NotImplementedError
 
+    @property
+    @abc.abstractmethod
+    def voice_client(self) -> Optional[VoiceRecvClient]:
+        raise NotImplementedError
+
     # TODO: handling opus vs pcm is not strictly mutually exclusive
     #       a sink could handle both but idk about that pattern
     @abc.abstractmethod
     def wants_opus(self) -> bool:
         """If sink handles opus data"""
         raise NotImplementedError
 
@@ -87,64 +125,100 @@
         """Optional callback for when the sink receives an rtcp packet"""
         pass
 
     @abc.abstractmethod
     def cleanup(self):
         raise NotImplementedError
 
+    def walk_children(self) -> Generator[AudioSink, None, None]:
+        for child in self.children:
+            yield child
+            yield from child.walk_children()
+
+
+class AudioSink(SinkABC):
+    _voice_client: Optional[VoiceRecvClient]
+    _parent: Optional[AudioSink] = None
+    _child: Optional[AudioSink]
 
-class AudioSink(BaseSink):
     def __init__(self, destination: Optional[AudioSink]=None, /):
         self._child = destination
 
         if destination is not None:
             destination._parent = self
 
     def __del__(self):
         self.cleanup()
 
     @property
-    def voice_client(self) -> VoiceRecvClient | None:
-        """
-        Guaranteed to not be None inside write()
-        """
-        if self.parent is not None:
-            return self.parent.voice_client
-        else:
-            return self._voice_client
-
-    @property
     def parent(self) -> Optional[AudioSink]:
         return self._parent
 
     @property
     def child(self) -> Optional[AudioSink]:
         return self._child
 
     @property
-    def children(self) -> Sequence[AudioSink]:
+    def children(self) -> list[AudioSink]:
         return [self._child] if self._child else []
 
+    @property
+    def voice_client(self) -> Optional[VoiceRecvClient]:
+        """Guaranteed to not be None inside write()"""
+
+        if self.parent is not None:
+            return self.parent.voice_client
+        else:
+            return self._voice_client
+
+    @classmethod
+    def listener(cls, name: str=MISSING):
+        """Marks a function as an event listener."""
+
+        if name is not MISSING and not isinstance(name, str):
+            raise TypeError(f'AudioSink.listener expected str but received {type(name).__name__} instead.')
+
+        def decorator(func):
+            actual = func
+
+            if isinstance(actual, staticmethod):
+                actual = actual.__func__
+
+            if inspect.iscoroutinefunction(actual):
+                raise TypeError('Listener function must not be a coroutine function.')
+
+            actual.__sink_listener__ = True
+            to_assign = name or actual.__name__
+
+            try:
+                actual.__sink_listener_names__.append(to_assign)
+            except AttributeError:
+                actual.__sink_listener_names__ = [to_assign]
+
+            return func
+
+        return decorator
+
 
 class MultiAudioSink(AudioSink):
     def __init__(self, destinations: Sequence[AudioSink], /):
         # Intentionally not calling super().__init__ here
-        self._children = tuple(destinations)
+        self._children = list(destinations)
 
         if destinations is not None:
             for dest in destinations:
                 dest._parent = self
 
     @property
     def child(self) -> Optional[AudioSink]:
         return self._children[0] if self._children else None
 
     @property
-    def children(self) -> Sequence[AudioSink]:
-        return self._children
+    def children(self) -> list[AudioSink]:
+        return self._children.copy()
 
 
 class BasicSink(AudioSink):
     """Simple callback based sink."""
 
     def __init__(self,
         event: BasicSinkWriteCB,
@@ -300,7 +374,50 @@
         return self.start_time is not None and self.get_time() - self.start_time < self.duration
 
     def get_time(self) -> int | float:
         """Function to generate a timestamp.  Defaults to `time.perf_counter()`.
         Can be overridden.
         """
         return time.perf_counter()
+
+
+class SilencePaddingSink(AudioSink):
+    """docstring for SilencePaddingSink"""
+
+    def __init__(self, destination: AudioSink):
+        super().__init__(destination)
+
+        self.destination = destination
+        # self.silencegen = SilenceGenerator()
+
+    def wants_opus(self) -> bool:
+        return self.destination.wants_opus()
+
+    def write(self, user: Optional[User], data: VoiceData):
+        return super().write(user, data)
+
+    def write_rtcp(self, packet: RTCPPacket):
+        self.destination.write_rtcp(packet)
+
+    def cleanup(self):
+        pass
+
+
+class DejitterSink(AudioSink):
+    """docstring for DejitterSink"""
+
+    def __init__(self, destination: AudioSink):
+        super().__init__(destination)
+
+        self.destination = destination
+
+    def wants_opus(self) -> bool:
+        return self.destination.wants_opus()
+
+    def write(self, user: Optional[User], data: VoiceData):
+        ...
+
+    def write_rtcp(self, packet: RTCPPacket):
+        self.destination.write_rtcp(packet)
+
+    def cleanup(self):
+        ...
```

### Comparing `discord-ext-voice_recv-0.1.7a94/discord/ext/voice_recv/types.py` & `discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/types.py`

 * *Files identical despite different names*

### Comparing `discord-ext-voice_recv-0.1.7a94/discord/ext/voice_recv/utils.py` & `discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/utils.py`

 * *Files identical despite different names*

### Comparing `discord-ext-voice_recv-0.1.7a94/discord/ext/voice_recv/video.py` & `discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/video.py`

 * *Files identical despite different names*

### Comparing `discord-ext-voice_recv-0.1.7a94/discord/ext/voice_recv/voice_client.py` & `discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/voice_client.py`

 * *Files identical despite different names*

### Comparing `discord-ext-voice_recv-0.1.7a94/discord_ext_voice_recv.egg-info/PKG-INFO` & `discord-ext-voice_recv-0.1.8a99/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,69 @@
 Metadata-Version: 2.1
-Name: discord-ext-voice-recv
-Version: 0.1.7a94
+Name: discord-ext-voice_recv
+Version: 0.1.8a99
 Summary: Experimental voice receive extension for discord.py
 Home-page: https://github.com/imayhaveborkedit/discord-ext-voice-recv
 Author: Imayhaveborkedit
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
+Classifier: Topic :: Multimedia :: Sound/Audio :: Capture/Recording
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # discord-ext-voice-recv
 Voice receive extension package for discord.py
 
-### Warning
+## Warning
 **This extension should be more or less functional, but the code is not yet feature complete.  No guarantees are given for stability or random breaking changes.**
 
 ## Installing
-**Python 3.8 or higher is required**
+**Python 3.8 or higher is required**, preferably 3.11 or whatever is latest
 
-`python -m pip install git+https://github.com/imayhaveborkedit/discord-ext-voice-recv`
+```
+python -m pip install discord-ext-voice-recv
+```
 
-This package will be uploaded to pypi eventually.
+To install directly from github:
+```
+python -m pip install git+https://github.com/imayhaveborkedit/discord-ext-voice-recv
+```
 
-Naturally, this extension depends on `discord.py` being installed with voice support.
+Naturally, this extension depends on `discord.py` being installed with voice support (`pynacl`).
 
 ## Example
 See the [example script](examples/recv.py).
 
+## Feature overview
+### Custom VoiceProtocol client
+No monkey patching or bizarre hacks required.  Simply use the library feature to use `VoiceRecvClient` as the voice client class.  See [Usage](#usage).
+
+### Six new events
+This extension adds the unimplemented voice websocket events and one virtual event.  See [New Events](#new-events).
+
+### Simple and familiar API
+The overall API is designed to mirror the discord.py voice send API, with `AudioSink` being the counterpart to the existing `AudioSource`.  See [Sinks](#sinks).
+
+### Convenient included utilities
+Batteries included in the form of useful built in `AudioSinks`.  Some to match their `AudioSource` counterpart, some I merely considered useful.  See... uh... TODO.
+
+### More or less typed
+Its probably fine.
+
 ## Usage
 ### VoiceRecvClient
 The class `voice_recv.VoiceRecvClient` must be used in `VoiceChannel.connect()` to use voice receive functionality.
 ```python
 voice_client = await voice_channel.connect(cls=voice_recv.VoiceRecvClient)
 ```
 
@@ -85,61 +106,78 @@
 class MySink(voice_recv.AudioSink):
     def __init__(self):
         super().__init__()
 
     def wants_opus(self) -> bool:
         return False
 
-    def write(self, user: Optional[User | Member], data: VoiceData):
+    def write(self, user: User | Member | None, data: VoiceData):
         ...
 
     def cleanup(self):
         ...
 ```
 
 These are the main functions of a sink, names and purpose reflecting that of their source counterparts.  It is important to note that `super().__init__()` must be called when inheriting from `AudioSink`, in contrast to `AudioSource` which does not have a default `__init__` function.
 
 - The `wants_opus()` function determines if the sink should receive opus packets or decoded PCM packets.  Care should be taken not to unintentionally mix sinks that want different types.
 - The `write()` function is the main callback, where the sink logic takes place.  In a sink pipeline, this could alter, inspect, or log a packet, and then write it to a child sink.  `VoiceData` is a simple container class with attributes for the origin member, opus data, optionally pcm data, and raw audio packet.
 - The `cleanup()` function is identical to `AudioSource.cleanup()`, a finalizer to cleanup any loose ends when the sink has finished its job.
 
-In addition, sinks also have properties for their `voice_client`, as well as `parent` and `child`/`children` sinks.  Furthermore, sinks will be able to receive events in a similar manner to cogs, but this has not been implemented yet. (TODO)
+Additionally, sinks also have properties for their `voice_client`, as well as `parent` and `child`/`children` sinks.
 
 This extension comes with several useful built in sinks, which I will briefly explain another time.  For now just [source dive](discord/ext/voice_recv/sinks.py).  (TODO)
 
+### Sink event listeners
+With AudioSinks being potentially more complex and stateful than AudioSources and the addition of new events, it is sometimes necessary to handle events in the context of a sink.  It would be rather awkward to have to register a sink function with `commands.Bot.add_listener()` while dealing with thread safety, and even moreso using `discord.Client`.  To remedy this, listeners can be defined within sinks, similarly to how they work in Cogs.
+
+```python
+class MySink(AudioSink):
+    @AudioSink.listener()
+    def on_voice_member_disconnect(self, member: discord.Member, ssrc: int | None):
+        print(f"{member} has disconnected")
+        self.do_something_like_handle_disconnect(ssrc)
+```
+
+Note that these functions must be sync functions, as they are dispatched from a thread.  Trying to use a coroutine will result in an error.  This restriction only applies to sink listeners, and normal async event listeners will function as per usual.  The event listener dispatch thread is different from the one used to dispatch the `write()` callback so potential threadsafety issues should be considered.  A decorator argument to run the event callback in the other thread may be added later.
+
 ## New events
 ```python
 async def on_voice_member_speak(member: discord.Member, ssrc: int)
 ```
 Called when a member first speaks (transmits audio) in a voice channel.  This event is only called once per their voice session (ssrc assignment).  Any packets received from this member before this event fires can (probably) be safely ignored since they are likely just silence packets.  The main purpose of this event is to reveal the ssrc of a member, to map packets to their originating member.
 
 This is **NOT** a speaking indicator event.  The speaking indicator is determined by packet activity.  This functionality will be added in the future.
 
 ```python
-async def on_voice_member_disconnect(member: discord.Member, ssrc: int)
+async def on_voice_member_disconnect(member: discord.Member, ssrc: int | None)
 ```
 Called when a member disconnects from a voice channel. The `ssrc` parameter is the unique id a member has to identify which packets belong to them.  This is useful when using custom sinks, particularly those that handle packets from multiple members.
 
 ```python
 async def on_voice_member_video(member: discord.Member, data: voice_recv.VoiceVideoStreams)
 ```
 Called when a member in voice channel toggles their webcam on or off, NOT screenshare.  Screenshare status is only indicated in the `self_video` attribute of `discord.VoiceState`.
 
 ```python
-async def on_voice_member_flags(member: discord.Member, flags: Optional[int])
+async def on_voice_member_flags(member: discord.Member, flags: int | None)
 ```
 An undocumented event dispatched when a member joins a voice channel containing a flags bitfield.  Only values `0`, `2`, and `None` have been observed so far, but their meaning remains unknown.
 
 ```python
-async def on_voice_member_platform(member: discord.Member, platform: Optional[int | str])
+async def on_voice_member_platform(member: discord.Member, platform: int | str | None)
 ```
 An undocumented event dispatched when a member joins a voice channel containing a platform key, presumably with what platform the member joined on.  However, this field has only ever been seen to contain `None`.
 
+```python
+def on_rtcp_packet(packet: RTCPPacket, guild: discord.Guild)
+```
+A virtual event for when an RTCP packet is received.  This event only works inside of sinks, so it cannot be async.
+
 ## Currently missing features
-- Sink events (similar to cog event handlers)
 - Silence generation (will be implemented as an included AudioSink)
 - Member speaking state status/event (design not yet decided)
 - Various internal impl details to maintain audio stability and consistency
 
 ## Future plans
 - Muxer AudioSink (mixes multiple audio streams into a single stream)
 - Rust implementations of some components for improved performance
```

### Comparing `discord-ext-voice_recv-0.1.7a94/discord_ext_voice_recv.egg-info/SOURCES.txt` & `discord-ext-voice_recv-0.1.8a99/discord_ext_voice_recv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discord-ext-voice_recv-0.1.7a94/setup.py` & `discord-ext-voice_recv-0.1.8a99/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,17 +39,17 @@
       extras_require=None,
       zip_safe=False,
       classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Intended Audience :: Developers',
         'Natural Language :: English',
-        'Operating System :: OS Independent',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
-        "Operating System :: POSIX",
-        "Operating System :: Microsoft :: Windows",
-        "Operating System :: MacOS",
+        'Operating System :: POSIX',
+        'Operating System :: Microsoft :: Windows',
+        'Operating System :: MacOS',
+        'Topic :: Multimedia :: Sound/Audio :: Capture/Recording'
       ]
 )
```

