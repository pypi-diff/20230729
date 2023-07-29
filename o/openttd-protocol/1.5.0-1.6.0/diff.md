# Comparing `tmp/openttd-protocol-1.5.0.tar.gz` & `tmp/openttd-protocol-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openttd-protocol-1.5.0.tar", last modified: Sat Jul 15 11:11:45 2023, max compression
+gzip compressed data, was "openttd-protocol-1.6.0.tar", last modified: Sat Jul 29 14:05:21 2023, max compression
```

## Comparing `openttd-protocol-1.5.0.tar` & `openttd-protocol-1.6.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 11:11:45.925711 openttd-protocol-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    26521 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-07-15 11:11:45.921711 openttd-protocol-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-15 11:11:45.000000 openttd-protocol-1.5.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 11:11:45.921711 openttd-protocol-1.5.0/openttd_protocol/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/openttd_protocol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 11:11:45.921711 openttd-protocol-1.5.0/openttd_protocol/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/openttd_protocol/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/openttd_protocol/protocol/content.py
--rw-r--r--   0 runner    (1001) docker     (123)    20789 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/openttd_protocol/protocol/coordinator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/openttd_protocol/protocol/game.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/openttd_protocol/protocol/stun.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/openttd_protocol/protocol/turn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 11:11:45.921711 openttd-protocol-1.5.0/openttd_protocol/wire/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/openttd_protocol/wire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/openttd_protocol/wire/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/openttd_protocol/wire/read.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/openttd_protocol/wire/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/openttd_protocol/wire/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/openttd_protocol/wire/test_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/openttd_protocol/wire/test_tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/openttd_protocol/wire/test_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/openttd_protocol/wire/write.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 11:11:45.921711 openttd-protocol-1.5.0/openttd_protocol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-07-15 11:11:45.000000 openttd-protocol-1.5.0/openttd_protocol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-15 11:11:45.000000 openttd-protocol-1.5.0/openttd_protocol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 11:11:45.000000 openttd-protocol-1.5.0/openttd_protocol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-15 11:11:45.000000 openttd-protocol-1.5.0/openttd_protocol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 11:11:45.925711 openttd-protocol-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:05:21.661968 openttd-protocol-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    26521 2023-07-29 14:05:09.000000 openttd-protocol-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-29 14:05:09.000000 openttd-protocol-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-07-29 14:05:21.657968 openttd-protocol-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-29 14:05:09.000000 openttd-protocol-1.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-29 14:05:21.000000 openttd-protocol-1.6.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:05:21.657968 openttd-protocol-1.6.0/openttd_protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:05:09.000000 openttd-protocol-1.6.0/openttd_protocol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:05:21.657968 openttd-protocol-1.6.0/openttd_protocol/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:05:09.000000 openttd-protocol-1.6.0/openttd_protocol/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-07-29 14:05:09.000000 openttd-protocol-1.6.0/openttd_protocol/protocol/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20958 2023-07-29 14:05:09.000000 openttd-protocol-1.6.0/openttd_protocol/protocol/coordinator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-07-29 14:05:09.000000 openttd-protocol-1.6.0/openttd_protocol/protocol/game.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-29 14:05:09.000000 openttd-protocol-1.6.0/openttd_protocol/protocol/stun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-29 14:05:09.000000 openttd-protocol-1.6.0/openttd_protocol/protocol/turn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:05:21.657968 openttd-protocol-1.6.0/openttd_protocol/wire/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:05:09.000000 openttd-protocol-1.6.0/openttd_protocol/wire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 14:05:09.000000 openttd-protocol-1.6.0/openttd_protocol/wire/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-29 14:05:09.000000 openttd-protocol-1.6.0/openttd_protocol/wire/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-29 14:05:09.000000 openttd-protocol-1.6.0/openttd_protocol/wire/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-07-29 14:05:09.000000 openttd-protocol-1.6.0/openttd_protocol/wire/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-29 14:05:09.000000 openttd-protocol-1.6.0/openttd_protocol/wire/test_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-29 14:05:09.000000 openttd-protocol-1.6.0/openttd_protocol/wire/test_tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-29 14:05:09.000000 openttd-protocol-1.6.0/openttd_protocol/wire/test_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-29 14:05:09.000000 openttd-protocol-1.6.0/openttd_protocol/wire/write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:05:21.657968 openttd-protocol-1.6.0/openttd_protocol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-07-29 14:05:21.000000 openttd-protocol-1.6.0/openttd_protocol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-29 14:05:21.000000 openttd-protocol-1.6.0/openttd_protocol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 14:05:21.000000 openttd-protocol-1.6.0/openttd_protocol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-29 14:05:21.000000 openttd-protocol-1.6.0/openttd_protocol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 14:05:21.661968 openttd-protocol-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-29 14:05:09.000000 openttd-protocol-1.6.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-29 14:05:09.000000 openttd-protocol-1.6.0/version.py
```

### Comparing `openttd-protocol-1.5.0/LICENSE` & `openttd-protocol-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openttd-protocol-1.5.0/PKG-INFO` & `openttd-protocol-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openttd-protocol
-Version: 1.5.0
+Version: 1.6.0
 Summary: OpenTTD network protocol for Python
 Home-page: https://github.com/OpenTTD/py-protocol
 Author: OpenTTD Dev Team
 Author-email: info@openttd.org
 License: UNKNOWN
 Description: # openttd-protocol
```

### Comparing `openttd-protocol-1.5.0/README.md` & `openttd-protocol-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `openttd-protocol-1.5.0/openttd_protocol/protocol/content.py` & `openttd-protocol-1.6.0/openttd_protocol/protocol/content.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,32 +221,33 @@
             write_uint32(data, dependency)
 
         write_uint8(data, len(tags))
         for tag in tags:
             write_string(data, tag)
 
         write_presend(data, SEND_TCP_COMPAT_MTU)
-        await self.send_packet(data)
+        return await self.send_packet(data)
 
     async def send_PACKET_CONTENT_SERVER_CONTENT(self, content_type, content_id, filesize, filename, stream):
         # First, send a packet to tell the client it will be receiving a file
         data = write_init(PacketContentType.PACKET_CONTENT_SERVER_CONTENT)
 
         write_uint8(data, content_type.value)
         write_uint32(data, content_id)
 
         write_uint32(data, filesize)
         write_string(data, filename)
 
         write_presend(data, SEND_TCP_COMPAT_MTU)
-        await self.send_packet(data)
+        length = await self.send_packet(data)
 
         # Next, send the content of the file over
         while not stream.eof():
             data = write_init(PacketContentType.PACKET_CONTENT_SERVER_CONTENT)
             data += stream.read(SEND_TCP_COMPAT_MTU - 3)
             write_presend(data, SEND_TCP_COMPAT_MTU)
-            await self.send_packet(data)
+            length += await self.send_packet(data)
 
         data = write_init(PacketContentType.PACKET_CONTENT_SERVER_CONTENT)
         write_presend(data, SEND_TCP_COMPAT_MTU)
-        await self.send_packet(data)
+        length += await self.send_packet(data)
+        return length
```

### Comparing `openttd-protocol-1.5.0/openttd_protocol/protocol/coordinator.py` & `openttd-protocol-1.6.0/openttd_protocol/protocol/coordinator.py`

 * *Files 2% similar despite different names*

```diff
@@ -352,28 +352,28 @@
         ):
             error_no = NetworkCoordinatorErrorType.NETWORK_COORDINATOR_ERROR_REGISTRATION_FAILED
 
         write_uint8(data, error_no.value)
         write_string(data, error_detail)
 
         write_presend(data, SEND_TCP_MTU)
-        await self.send_packet(data)
+        return await self.send_packet(data)
 
     async def send_PACKET_COORDINATOR_GC_REGISTER_ACK(
         self, protocol_version, connection_type, invite_code, invite_code_secret
     ):
         data = write_init(PacketCoordinatorType.PACKET_COORDINATOR_GC_REGISTER_ACK)
 
         if protocol_version > 1:
             write_string(data, invite_code)
             write_string(data, invite_code_secret)
         write_uint8(data, connection_type.value)
 
         write_presend(data, SEND_TCP_MTU)
-        await self.send_packet(data)
+        return await self.send_packet(data)
 
     def _fill_NEWGRF_LOOKUP_PACKET(self, newgrf_lookup_table_cursor, newgrf_lookup_table):
         data = bytearray()
         count = 0
         for index, newgrf in newgrf_lookup_table.items():
             if index <= newgrf_lookup_table_cursor:
                 continue
@@ -397,29 +397,33 @@
             yield count, data
 
     async def send_PACKET_COORDINATOR_GC_NEWGRF_LOOKUP(
         self, protocol_version, newgrf_lookup_table_cursor, newgrf_lookup_table
     ):
         cursor = max(newgrf_lookup_table.keys())
 
+        length = 0
         for count, body in self._fill_NEWGRF_LOOKUP_PACKET(newgrf_lookup_table_cursor, newgrf_lookup_table):
             data = write_init(PacketCoordinatorType.PACKET_COORDINATOR_GC_NEWGRF_LOOKUP)
 
             # The cursor is the highest index in the table. Index only increases
             # (till a full database reset), so it is a pretty safe cursor to use.
             write_uint32(data, cursor)
             write_uint16(data, count)
             write_bytes(data, body)
 
             write_presend(data, SEND_TCP_MTU)
-            await self.send_packet(data)
+            length += await self.send_packet(data)
+
+        return length
 
     async def send_PACKET_COORDINATOR_GC_LISTING(
         self, protocol_version, game_info_version, servers, newgrf_lookup_table
     ):
+        length = 0
         for server in servers:
             if server.game_type != ServerGameType.SERVER_GAME_TYPE_PUBLIC:
                 continue
             if len(server.info) == 0:
                 continue
 
             data = write_init(PacketCoordinatorType.PACKET_COORDINATOR_GC_LISTING)
@@ -479,77 +483,78 @@
                 write_uint16(data, server.info["map_width"])
                 write_uint16(data, server.info["map_height"])
                 write_uint8(data, server.info["map_type"])
 
                 write_uint8(data, server.info["is_dedicated"])
 
             write_presend(data, SEND_TCP_MTU)
-            await self.send_packet(data)
+            length += await self.send_packet(data)
 
         # Send a final packet with 0 servers to indicate end-of-list.
         data = write_init(PacketCoordinatorType.PACKET_COORDINATOR_GC_LISTING)
         write_uint16(data, 0)
         write_presend(data, SEND_TCP_MTU)
-        await self.send_packet(data)
+        length += await self.send_packet(data)
+        return length
 
     async def send_PACKET_COORDINATOR_GC_CONNECTING(self, protocol_version, token, invite_code):
         data = write_init(PacketCoordinatorType.PACKET_COORDINATOR_GC_CONNECTING)
 
         write_string(data, token)
         write_string(data, invite_code)
 
         write_presend(data, SEND_TCP_MTU)
-        await self.send_packet(data)
+        return await self.send_packet(data)
 
     async def send_PACKET_COORDINATOR_GC_CONNECT_FAILED(self, protocol_version, token):
         data = write_init(PacketCoordinatorType.PACKET_COORDINATOR_GC_CONNECT_FAILED)
 
         write_string(data, token)
 
         write_presend(data, SEND_TCP_MTU)
-        await self.send_packet(data)
+        return await self.send_packet(data)
 
     async def send_PACKET_COORDINATOR_GC_DIRECT_CONNECT(self, protocol_version, token, tracking_number, hostname, port):
         data = write_init(PacketCoordinatorType.PACKET_COORDINATOR_GC_DIRECT_CONNECT)
 
         write_string(data, token)
         write_uint8(data, tracking_number)
         write_string(data, hostname)
         write_uint16(data, port)
 
         write_presend(data, SEND_TCP_MTU)
-        await self.send_packet(data)
+        return await self.send_packet(data)
 
     async def send_PACKET_COORDINATOR_GC_STUN_REQUEST(self, protocol_version, token):
         data = write_init(PacketCoordinatorType.PACKET_COORDINATOR_GC_STUN_REQUEST)
 
         write_string(data, token)
 
         write_presend(data, SEND_TCP_MTU)
-        await self.send_packet(data)
+        return await self.send_packet(data)
 
     async def send_PACKET_COORDINATOR_GC_STUN_CONNECT(
         self, protocol_version, token, tracking_number, interface_number, hostname, port
     ):
         data = write_init(PacketCoordinatorType.PACKET_COORDINATOR_GC_STUN_CONNECT)
 
         write_string(data, token)
         write_uint8(data, tracking_number)
         write_uint8(data, interface_number)
         write_string(data, hostname)
         write_uint16(data, port)
 
         write_presend(data, SEND_TCP_MTU)
-        await self.send_packet(data)
+        return await self.send_packet(data)
 
     async def send_PACKET_COORDINATOR_GC_TURN_CONNECT(
         self, protocol_version, token, tracking_number, ticket, connection_string
     ):
         data = write_init(PacketCoordinatorType.PACKET_COORDINATOR_GC_TURN_CONNECT)
 
         write_string(data, token)
         write_uint8(data, tracking_number)
         write_string(data, ticket)
         write_string(data, connection_string)
 
         write_presend(data, SEND_TCP_MTU)
-        await self.send_packet(data)
+        return await self.send_packet(data)
```

### Comparing `openttd-protocol-1.5.0/openttd_protocol/protocol/game.py` & `openttd-protocol-1.6.0/openttd_protocol/protocol/game.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,8 +163,8 @@
             raise PacketInvalidData("more bytes than expected in SERVER_SHUTDOWN; remaining: ", len(data))
 
         return {}
 
     async def send_PACKET_CLIENT_GAME_INFO(self):
         data = write_init(PacketGameType.PACKET_CLIENT_GAME_INFO)
         write_presend(data, SEND_TCP_MTU)
-        await self.send_packet(data)
+        return await self.send_packet(data)
```

### Comparing `openttd-protocol-1.5.0/openttd_protocol/protocol/stun.py` & `openttd-protocol-1.6.0/openttd_protocol/protocol/stun.py`

 * *Files identical despite different names*

### Comparing `openttd-protocol-1.5.0/openttd_protocol/protocol/turn.py` & `openttd-protocol-1.6.0/openttd_protocol/protocol/turn.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,8 +44,8 @@
 
     async def send_PACKET_TURN_TURN_CONNECTED(self, protocol_version, hostname):
         data = write_init(PacketTurnType.PACKET_TURN_TURN_CONNECTED)
 
         write_string(data, hostname)
 
         write_presend(data, SEND_TCP_MTU)
-        await self.send_packet(data)
+        return await self.send_packet(data)
```

### Comparing `openttd-protocol-1.5.0/openttd_protocol/wire/exceptions.py` & `openttd-protocol-1.6.0/openttd_protocol/wire/exceptions.py`

 * *Files identical despite different names*

### Comparing `openttd-protocol-1.5.0/openttd_protocol/wire/read.py` & `openttd-protocol-1.6.0/openttd_protocol/wire/read.py`

 * *Files identical despite different names*

### Comparing `openttd-protocol-1.5.0/openttd_protocol/wire/source.py` & `openttd-protocol-1.6.0/openttd_protocol/wire/source.py`

 * *Files identical despite different names*

### Comparing `openttd-protocol-1.5.0/openttd_protocol/wire/tcp.py` & `openttd-protocol-1.6.0/openttd_protocol/wire/tcp.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,7 +213,9 @@
             raise SocketClosed
 
         res = self.transport.write(data)
         # For websockets, the return of the write is a coroutine. For
         # everything else, it is a non-blocking normal function.
         if iscoroutine(res):
             await res
+
+        return len(data)
```

### Comparing `openttd-protocol-1.5.0/openttd_protocol/wire/test_read.py` & `openttd-protocol-1.6.0/openttd_protocol/wire/test_read.py`

 * *Files identical despite different names*

### Comparing `openttd-protocol-1.5.0/openttd_protocol/wire/test_tcp.py` & `openttd-protocol-1.6.0/openttd_protocol/wire/test_tcp.py`

 * *Files identical despite different names*

### Comparing `openttd-protocol-1.5.0/openttd_protocol/wire/test_write.py` & `openttd-protocol-1.6.0/openttd_protocol/wire/test_write.py`

 * *Files identical despite different names*

### Comparing `openttd-protocol-1.5.0/openttd_protocol/wire/write.py` & `openttd-protocol-1.6.0/openttd_protocol/wire/write.py`

 * *Files identical despite different names*

### Comparing `openttd-protocol-1.5.0/openttd_protocol.egg-info/PKG-INFO` & `openttd-protocol-1.6.0/openttd_protocol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openttd-protocol
-Version: 1.5.0
+Version: 1.6.0
 Summary: OpenTTD network protocol for Python
 Home-page: https://github.com/OpenTTD/py-protocol
 Author: OpenTTD Dev Team
 Author-email: info@openttd.org
 License: UNKNOWN
 Description: # openttd-protocol
```

### Comparing `openttd-protocol-1.5.0/openttd_protocol.egg-info/SOURCES.txt` & `openttd-protocol-1.6.0/openttd_protocol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openttd-protocol-1.5.0/setup.py` & `openttd-protocol-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `openttd-protocol-1.5.0/version.py` & `openttd-protocol-1.6.0/version.py`

 * *Files identical despite different names*

