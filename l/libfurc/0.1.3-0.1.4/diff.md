# Comparing `tmp/libfurc-0.1.3.tar.gz` & `tmp/libfurc-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/libfurc-0.1.3.tar", last modified: Thu Nov 17 09:48:12 2022, max compression
+gzip compressed data, was "dist/libfurc-0.1.4.tar", last modified: Sat Jul 29 10:57:27 2023, max compression
```

## Comparing `libfurc-0.1.3.tar` & `libfurc-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 09:48:12.000000 libfurc-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (121)     2047 2022-11-17 09:48:12.000000 libfurc-0.1.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 09:48:12.000000 libfurc-0.1.3/libfurc/
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-11-17 09:48:04.000000 libfurc-0.1.3/libfurc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7805 2022-11-17 09:48:04.000000 libfurc-0.1.3/libfurc/account.py
--rw-r--r--   0 runner    (1001) docker     (121)     8144 2022-11-17 09:48:04.000000 libfurc-0.1.3/libfurc/archive.py
--rw-r--r--   0 runner    (1001) docker     (121)     2388 2022-11-17 09:48:04.000000 libfurc-0.1.3/libfurc/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    38323 2022-11-17 09:48:04.000000 libfurc-0.1.3/libfurc/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     4647 2022-11-17 09:48:04.000000 libfurc-0.1.3/libfurc/colors.py
--rw-r--r--   0 runner    (1001) docker     (121)     5951 2022-11-17 09:48:04.000000 libfurc-0.1.3/libfurc/dream.py
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-11-17 09:48:04.000000 libfurc-0.1.3/libfurc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    19203 2022-11-17 09:48:04.000000 libfurc-0.1.3/libfurc/fox5.py
--rw-r--r--   0 runner    (1001) docker     (121)     2412 2022-11-17 09:48:04.000000 libfurc-0.1.3/libfurc/furcbuffer.py
--rw-r--r--   0 runner    (1001) docker     (121)     7645 2022-11-17 09:48:04.000000 libfurc-0.1.3/libfurc/particles.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 09:48:12.000000 libfurc-0.1.3/libfurc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2047 2022-11-17 09:48:12.000000 libfurc-0.1.3/libfurc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-11-17 09:48:12.000000 libfurc-0.1.3/libfurc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-17 09:48:12.000000 libfurc-0.1.3/libfurc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-17 09:48:12.000000 libfurc-0.1.3/libfurc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-17 09:48:12.000000 libfurc-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      930 2022-11-17 09:48:04.000000 libfurc-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:57:27.000000 libfurc-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-29 10:57:27.000000 libfurc-0.1.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:57:27.000000 libfurc-0.1.4/libfurc/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-29 10:57:24.000000 libfurc-0.1.4/libfurc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8326 2023-07-29 10:57:24.000000 libfurc-0.1.4/libfurc/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-29 10:57:24.000000 libfurc-0.1.4/libfurc/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-29 10:57:24.000000 libfurc-0.1.4/libfurc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40791 2023-07-29 10:57:24.000000 libfurc-0.1.4/libfurc/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-07-29 10:57:24.000000 libfurc-0.1.4/libfurc/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-07-29 10:57:24.000000 libfurc-0.1.4/libfurc/dream.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-29 10:57:24.000000 libfurc-0.1.4/libfurc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19280 2023-07-29 10:57:24.000000 libfurc-0.1.4/libfurc/fox5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-07-29 10:57:24.000000 libfurc-0.1.4/libfurc/furcbuffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11844 2023-07-29 10:57:24.000000 libfurc-0.1.4/libfurc/particles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:57:27.000000 libfurc-0.1.4/libfurc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-29 10:57:27.000000 libfurc-0.1.4/libfurc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-29 10:57:27.000000 libfurc-0.1.4/libfurc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:57:27.000000 libfurc-0.1.4/libfurc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-29 10:57:27.000000 libfurc-0.1.4/libfurc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:57:27.000000 libfurc-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-29 10:57:24.000000 libfurc-0.1.4/setup.py
```

### Comparing `libfurc-0.1.3/PKG-INFO` & `libfurc-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libfurc
-Version: 0.1.3
+Version: 0.1.4
 Summary: A library for handling Furcadia things.
 Home-page: https://github.com/FelixWolf/libFurc
 Author: Félix
 Author-email: felix.wolfz@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `libfurc-0.1.3/libfurc/account.py` & `libfurc-0.1.4/libfurc/account.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,21 +56,35 @@
         self.messages = None
         self.time = None
         self.owner = None
         self.costumes = None
         self.type = self.TYPE_INI
     
     @classmethod
-    def fromINI(self, name, colors = None, password = None, desc = None,
+    def fromINI(cls, name, colors = None, password = None, desc = None,
                 logins = 0, lastLogin = 0, autoResponse = None,
                 autoResponseMessage = None, AFKTime = None, AFKMessage = None,
                 AFKDescription = None, AFKPortrait = None,
                 DefaultPortrait = None, AFKDisconnectTime = None):
         self = cls()
         self.type = self.TYPE_INI
+        self.name = name
+        self.colors = colors
+        self.password = password
+        self.desc = desc
+        self.logins = logins
+        self.lastLogin = lastLogin
+        self.autoResponse = autoResponse
+        self.autoResponseMessage = autoResponseMessage
+        self.AFKTime = AFKTime
+        self.AFKMessage = AFKMessage
+        self.AFKDescription = AFKDescription
+        self.AFKPortrait = AFKPortrait
+        self.DefaultPortrait = DefaultPortrait
+        self.AFKDisconnectTime = AFKDisconnectTime
         return self
     
     @classmethod
     def fromAccount(cls, account, id, name, species = None, colors = None,
                     flags = None, created = None, lastLogin = None,
                     lastItem = None, lastPort = None, lastScale = 100,
                     lastGloam = None, lastSpeci = None, messages = None,
```

### Comparing `libfurc-0.1.3/libfurc/archive.py` & `libfurc-0.1.4/libfurc/archive.py`

 * *Files identical despite different names*

### Comparing `libfurc-0.1.3/libfurc/base.py` & `libfurc-0.1.4/libfurc/base.py`

 * *Files identical despite different names*

### Comparing `libfurc-0.1.3/libfurc/client.py` & `libfurc-0.1.4/libfurc/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         fuid = msg.read220(4)
         x = msg.read220(2)
         y = msg.read220(2)
         direction = msg.read220(1)
         shape = msg.read220(1)
         await self.fire("AnimateAvatar", fuid, (x,y), direction, shape)
     
-    #"0" - Sync dream variables
+    #"0" - Set variables
     async def message_16(self, opcode, data):
         msg = FurcBuffer(data)
         variables = {}
         while msg.remaining >= 2:
             offset = msg.read95(2)
             while msg.remaining >= 6:
                 val = msg.read95(3)
@@ -96,15 +96,15 @@
                     offset += 1
                 else:
                     repeats = msg.read95(3) + 1
                     val = msg.read95(3)
                     for i in range(repeats):
                         variables[offset] = val
                         offset += 1
-        await self.fire("UpdateVariables", variables)
+        await self.fire("SetVariables", variables)
     
     #"1" - Set floors
     async def message_17(self, opcode, data):
         msg = FurcBuffer(data)
         result = []
         while msg.remaining >= 6:
             x = msg.read220(2)
@@ -141,22 +141,22 @@
             result.append({
                 "pos": (x, y),
                 "id": wallID,
                 "repeats": repeats
             })
         await self.fire("SetWall", result)
     
-    #"3" - Set all DS variables
+    #"3" - Set DS Variable stack
     async def message_19(self, opcode, data):
         msg = FurcBuffer(data)
         vals = []
         while msg.remaining >= 3:
             var = msg.read95(3)
             vals.append(var)
-        await self.fire("SetVariables", vals)
+        await self.fire("DSVariableStack", vals)
     
     #"4" - Set region
     async def message_20(self, opcode, data):
         msg = FurcBuffer(data)
         result = []
         while msg.remaining >= 6:
             x = msg.read220(2)
@@ -240,17 +240,25 @@
         msg = FurcBuffer(data)
         moveFlag = msg.read95(1)
         randSeed = msg.read95(5)
         try:
             saidNum = msg.read95(3)
         except ValueError:
             #TEMPORARY: Fix for server sending non-base95 numbers
+            msg.offset -= 3
+            print("INVALID saidNum", msg.read(3))
             saidNum = 0
         facingDir = msg.read95(1)
-        entryCode = msg.read95(3)
+        try:
+            entryCode = msg.read95(3)
+        except ValueError:
+            #TEMPORARY: Fix for server sending non-base95 numbers
+            msg.offset -= 3
+            print("INVALID entryCode", msg.read(3))
+            entryCode = 0
         objPaws =  msg.read95(3)
         furreCount = msg.read95(2)
         userID = msg.read95(6)
         DSBtn = msg.read95(2)
         dreamCookies = msg.read95(3)
         triggererCookies = msg.read95(2)
         portalOpen = (msg.read95(2), msg.read95(2))
@@ -367,17 +375,17 @@
         await self.fire("MoveAvatar", fuid, (x,y), direction, shape)
     
     #"B" - Set avatar colors
     async def message_34(self, opcode, data):
         msg = FurcBuffer(data)
         furre = msg.read220(4)
         direction = msg.read220(1)
-        unk1 = msg.read220(1)
+        shape = msg.read220(1)
         colors = Colors.fromStream(msg)
-        await self.fire("SetAvatarColors", furre, direction, unk1, colors)
+        await self.fire("SetAvatarColors", furre, direction, shape, colors)
     
     #"C" - Hide avatar at position
     async def message_35(self, opcode, data):
         msg = FurcBuffer(data)
         furre = msg.read220(4)
         pos = (msg.read220(2), msg.read220(2))
         await self.fire("HideAvatar", furre, pos)
@@ -527,47 +535,72 @@
     #"]3" - Show user list
     async def message_61_19(self, opcode, data):
         msg = FurcBuffer(data)
         #0 = Show usercount + list, 1 = Only count
         enabled = not bool(int(msg.read(1)))
         await self.fire("EnableUserList", enabled)
     
-    #"]?" - Unknown, something related to pounce
-    #FIXME: Figure out wtf this is
+    #"]?" - Pounce
     async def message_61_31(self, opcode, data):
-        """Seen values:
-            char[1] "I" - Clear(?) and jump to func1
-            char[1] "A" - jump to func1
-            char[1] "S" - jump to func2
-            char[1] "o" - jump to func3
-            
-            func1:
-                Base220(4) unk1
-                Base220(4) unk2
-                char[1] unk3 #flag?
-                Base220(4) unk4 #Time?
-                Base220(4) unk5 #Time?
-                Base220(4) unk6 #Time?
-                Base220(1) unk7
-                Base220(1) unk8
-            
-            func2:
-                while(remaining > 3)
-                    Base220(4) unk1
-                    Base220(4) unk2
-                    char[1] unk3
-                    Base220(4) unk4
-                    Base220(4) unk5
-            
-            func3:
-                Base220(4) unk1
-                char[1] flag - "+" or "-"
-        """
-        #await self.fire("SetUserID", int(data.decode()))
-    
+        msg = FurcBuffer(data)
+        subop = msg.read(1)
+        if subop == b"I":
+            await self.fire("PounceInit")
+            #print("Pounce Initialize")
+        
+        if subop == b"I" or subop == b"A":
+            pounceList = []
+            while msg.remaining > 23: #Must be greater than this due to string
+                """
+                    Flags:
+                        1 = isFriendRequest #If set, we can accept, otherwise we sent and are waiting
+                        2 = isFriends #Only set if both parties accepted
+                        4 = unknown
+                    if 1 and 2 are unset, then we sent the FR and they haven't accepted
+                    if 1 is set and 2 is unset, then they sent the FR and we haven't accepted
+                """
+                entry = {
+                    "character": msg.read220(4), #our FUID
+                    "fuid": msg.read220(4), #their FUID
+                    "status": msg.read(1), #+ = online, - = offline
+                    "unk4": datetime.datetime.fromtimestamp(msg.read220(4) + 1505145789), #Magic numbers yay!
+                    "unk5": datetime.datetime.fromtimestamp(msg.read220(4) + 1505145789),
+                    "unk6": datetime.datetime.fromtimestamp(msg.read220(4) + 1505145789),
+                    "flags": msg.read220(1),
+                    "name": msg.read(msg.read220(1))
+                }
+                pounceList.append(entry)
+            
+            await self.fire("PounceList", pounceList)
+        
+        elif subop == "S": #No clue what this is
+            updateList = []
+            while msg.remaining >= 17: #Greater or equal to since no unknown length
+                entry = {
+                    "character": msg.read220(4), #our FUID
+                    "fuid": msg.read220(4), #their FUID
+                    "status": msg.read(1), #+ = online, - = offline
+                    "unk3": datetime.datetime.fromtimestamp(msg.read220(4) + 1505145789),
+                    "unk4": datetime.datetime.fromtimestamp(msg.read220(4) + 1505145789),
+                }
+                updateList.append(entry)
+        
+        elif subop == "o":
+            onlineList = []
+            while msg.remaining >= 5: #Greater or equal to since no unknown length
+                entry = {
+                    "fuid": msg.read220(4),
+                    "status": msg.read(1) #+ = online, - = offline
+                }
+                onlineList.append(entry)
+            
+            await self.fire("PounceUpdate", onlineList)
+        
+        else:
+            logging.warn("Received unknown 61:31 (Pounce) request from server!")
     
     #"]A" - Download guild tag command (DEPRECATED?)
     async def message_61_33(self, opcode, data):
         msg = FurcBuffer(data)
         checksum = int(msg.readUntil()) #Download it from file server using gt%i
         name = msg.readUntil()
         await self.fire("GuildTagDownload", checksum, name)
@@ -636,15 +669,16 @@
         pass
     
     #"]M" - Dynamic Avatars Info
     async def message_61_45(self, opcode, data):
         avatars = {}
         msg = FurcBuffer(data)
         dataVersion = msg.read220(1)
-        if data == 2:
+        unk1 = msg.read(1)
+        if dataVersion == 2:
             while msg.remaining >= 8:
                 avatarVersion = msg.read220(1)
                 
                 flags = msg.read220(1)
                 
                 idP1 = msg.read220(1)
                 idP2 = msg.read220(1)
@@ -670,29 +704,26 @@
     async def message_61_47(self, opcode, data):
         msg = FurcBuffer(data)
         result = {}
         
         while msg.remaining >= 12:
             fuid = msg.read220(4)
             
-            color = 0
+            r, g, b = 0, 0, 0
             
-            for i in range(6):
-                #I still don't fully understand this but this seems to work
-                color = color << 4
-                fragment = msg.read(1)[0]
-                if fragment >= 48 and fragment <= 57:
-                    color = color | (fragment & 15)
-                elif fragment >= 65 and fragment <= 70:
-                    color = color | (fragment - 75)
+            try:
+                #BGR encoding
+                b, g, r = bytes.fromhex(msg.read(6).decode())
+            except ValueError:
+                pass #Just ignore it, it's malformed
             
-            intensity = msg.read220(2)
+            intensity = msg.read220(2) & 0xFF #0 to 254
             
             result[fuid] = {
-                "color": color,
+                "color": [r, g, b],
                 "intensity": intensity
             }
         
         await self.fire("Gloam", result)
     
     #"]P" - Prefix next line (Can be overridden by 61_13)
     async def message_61_48(self, opcode, data):
@@ -741,42 +772,49 @@
                     msg.read220(2),
                     msg.read220(1),
                 ))
         
         await self.fire("RegionSettings", result)
     
     #"]Z" - Art party(?)
-    #TODO: Implement
     async def message_61_58(self, opcode, data):
-        """
-            Format:
-                char[1] opcode # 0 - 7
-                
-            if opcode == 0: #End
-                #No params
-            
-            if opcode == 2: #Draw
-                #Probably base220 byte array
-            
-            if opcode == 3: #UNKNOWN
-                #unknown
-            
-            if opcode == 4: #Set shape
-                base220(4) shape
-                
-            if opcode == 5:
-                #unknown
-            
-            if opcode == 6: #Request data?
-                #no op
-            
-            if opcode == 7:
-                char(*) filename
-        """
-        pass
+        msg = FurcBuffer(data)
+        cmd = int(msg.read(1))
+        if cmd == 0:
+            await self.fire("ArtPartyEnd")
+        
+        elif cmd == 2:
+            pixels = []
+            while len(pixels) < 32 and msg.remaining >= 6:
+                pxPosA = msg.read220(2)
+                pxPosB = msg.read220(2)
+                pixelColor = pxPosB & 0xFF
+                pixelPos = pxPosA + ((pxPosB >> 8) * 0x8000) - 256
+                unk = msg.read220(2)
+                pixels.append({
+                    "pixel": pixelPos,
+                    "color": pixelColor,
+                    "unk": unk,
+                    "x": pixelPos & 0xFF,
+                    "y": 0xFE - (pixelPos >> 8)
+                })
+            
+            await self.fire("ArtPartyDraw", pixels)
+        
+        elif cmd == 4:
+            await self.fire("ArtPartySetShape", msg.read220(4))
+        
+        elif cmd == 6:
+            await self.fire("ArtPartyRequest")
+        
+        elif cmd == 7:
+            await self.fire("ArtPartyStart", msg.read())
+        
+        else:
+            logging.warn("Received unknown 61:58 (Art Party) request from server!")
     
     #"]]" - Login failure
     async def message_61_61(self, opcode, data):
         await self.fire("Login", False)
     
     #"]_" - Kitterdust
     async def message_61_63(self, opcode, data):
@@ -822,16 +860,23 @@
     
     #"]c" - Set marbled
     async def message_61_67(self, opcode, data):
         #This has a "c" prefixed to it
         msg = FurcBuffer(data)
         
         #t is Type
-        #type 0 and 1 are unknown
+        #type 0 is invalid (?)
+        #type 1 is probably the loading screen
         #type 2 is normal mode
+        #type 3 is character creator (?)
+        #type 4, 5, 6, 7, 8 are related to the message center
+        #type 9 isn't implemented
+        #type 10 is the pink text box screen
+        #everything else isn't defined
+        
         t = msg.read(1)[0]
         if t > 96 and t < 123:
             t = t - 97
         else:
             t = 0
         
         background = msg.readUntil()
@@ -899,56 +944,51 @@
         version = msg.read220(1)
         channelUpdateType = msg.read220(1)
         unk1 = msg.read220(1)
         while msg.remaining >= 9:
             nameLength = msg.read220(1)
             name = msg.read(nameLength)
             bitpack = msg.read220(4)
-            canJoin = bitpack >> 7 & 1
+            canJoin = bitpack >> 7 & 1 == 1
             maturity = (bitpack >> 8 & 0xf) * 100
             peopleCount = bitpack >> 25 & 0x1f
-            canTell = bitpack & 0x4000
-            canListen = bitpack & 0x20000
-            canBroadcast = bitpack & 0x40000
+            canTell = bitpack & 0x4000 == 0x4000
+            canListen = bitpack & 0x20000 == 0x20000
+            canBroadcast = bitpack & 0x40000 == 0x40000
             channelImage = msg.read220(4)
             await self.fire("ChannelInfo", channelUpdateType == "@", name, maturity, peopleCount, canTell, canListen, canBroadcast, channelImage)
     
     #"]o" - Dream owner name
     async def message_61_79(self, opcode, data):
         msg = FurcBuffer(data)
         owner = msg.read()
         await self.fire("DreamOwner", owner.decode())
     
     #"]q" - Load dream with custom patches
     async def message_61_81(self, opcode, data):
         msg = FurcBuffer(data)
+        msg.readUntil() #NOP
         patchName = msg.readUntil()
         crc32 = msg.readUntil()
         unk1 = msg.readUntil()
         unk2 = msg.readUntil()
         modern = msg.readUntil()
         if modern == "modern":
             modern = True
         else:
             modern = False
         await self.fire("Dream", True, patchName, crc32, modern)
     
     #"]r" - Load dream with default patches
     async def message_61_82(self, opcode, data):
         msg = FurcBuffer(data)
+        msg.readUntil() #NOP
         patchName = msg.readUntil()
         crc32 = msg.readUntil()
-        unk1 = msg.readUntil()
-        unk2 = msg.readUntil()
-        modern = msg.readUntil()
-        if modern == "modern":
-            modern = True
-        else:
-            modern = False
-        await self.fire("Dream", False, patchName, crc32, modern)
+        await self.fire("Dream", False, patchName, crc32, False)
     
     #"]s" - Place text at location
     async def message_61_83(self, opcode, data):
         msg = FurcBuffer(data)
         x = msg.read95(2)
         y = msg.read95(2)
         textType = int(msg.readUntil()) #Text type: 0 = None, 1 = Normal, 2 = Lower
@@ -1066,15 +1106,15 @@
         try:
             await getattr(
                 self,
                 "message_" + str(data[0]-32),
                 self.message_unhandled
             )(data[0]-32, data[1:])
         except ValueError as e:
-            print("DECODE FAILED ")
+            print("DECODE FAILED ", data)
 
 #Outgoing message definitions
 class Commands:
     def login(self, character, machineid = None):
         if machineid == None:
             machineid = ""
         else:
@@ -1159,16 +1199,16 @@
                 return motd
             else:
                 motd += data.decode()
         
         return None
     
     async def disconnect(self):
-        writer.close()
-        await writer.wait_closed()
+        self.writer.close()
+        await self.writer.wait_closed()
         self.reader = None
         self.writer = None
     
     async def send(self, data):
         if self.connected:
             self.writer.write(data)
             await self.writer.drain()
```

### Comparing `libfurc-0.1.3/libfurc/colors.py` & `libfurc-0.1.4/libfurc/colors.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python3
+from .furcbuffer import FurcBuffer
 
 class Colors:
     def __init__(self, version = 116):
         self.version = version
         self.fur = 0
         self.markings = 0
         self.hair = 0
@@ -32,14 +33,97 @@
         if self.species:
             values += "; S: {}".format(self.species)
         if self.avatar:
             values += "; Av: {}".format(self.avatar)
         
         return "<Colors({}) {}>".format(self.version, values)
     
+    def toString(self, full = True, version = None):
+        version = version or self.version
+        
+        data = FurcBuffer()
+        
+        if version == 116: #t
+            data.write220(self.fur)
+            data.write220(self.markings)
+            data.write220(self.hair)
+            data.write220(self.eye)
+            data.write220(self.badge)
+            data.write220(self.vest)
+            data.write220(self.bracer)
+            data.write220(self.cape)
+            data.write220(self.boot)
+            data.write220(self.trousers)
+            
+            if full:
+                data.write220(self.gender or 0)
+                data.write220(self.species or 0)
+                data.write220(self.avatar or 0)
+            
+        elif version == 117: #u
+            #TODO: Implement this
+            #http://dev.furcadia.com/docs/new_color_code_format.pdf
+            if data.remaining < 2:
+                raise ValueError("Invalid color code length!")
+            
+            bitmask = (data.read220()&63) | (data.read220() << 6)
+            
+            for i in range(0, 10):
+                if bitmask >> i & 1:
+                    data.read(3)
+                else:
+                    data.read(1)
+            
+            if data.remaining >= 1:
+                self.gender = data.read220()
+            
+            if data.remaining >= 1:
+                self.species = data.read220()
+            
+            if data.remaining >= 1:
+                self.avatar = data.read220()
+        
+        elif version == 118: #v
+            #TODO: Implement this
+            #http://dev.furcadia.com/docs/new_color_code_format.pdf
+            if data.remaining < 27:
+                raise ValueError("Invalid color code length!")
+            
+            data.read(27) # 9 * 3
+            
+            if data.remaining >= 1:
+                self.gender = data.read220()
+            
+            if data.remaining >= 1:
+                self.species = data.read220()
+            
+            if data.remaining >= 1:
+                self.avatar = data.read220()
+        
+        elif version == 119: #w
+            data.write220(self.fur)
+            data.write220(self.markings)
+            data.write220(self.hair)
+            data.write220(self.eye)
+            data.write220(self.badge)
+            data.write220(self.vest)
+            data.write220(self.bracer)
+            data.write220(self.cape)
+            data.write220(self.boot)
+            data.write220(self.trousers)
+            data.write220(self.wings)
+            data.write220(self.accent)
+            
+            if full:
+                data.write220(self.gender or 0)
+                data.write220(self.species or 0)
+                data.write220(self.avatar or 0)
+        
+        return data
+    
     @classmethod
     def fromCode(cls, data):
         self = cls()
         
         return self
     
     @classmethod
```

### Comparing `libfurc-0.1.3/libfurc/dream.py` & `libfurc-0.1.4/libfurc/dream.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,24 +48,25 @@
     'sfxopacity': int,
     'name': str,
     'patchs': str,
     'noload': bool,
     'allowjs': bool,
     'allowlf': bool,
     'allowfurl': bool,
+    'allowshouts': bool,
+    'allowlarge': bool,
     'swearfilter': bool,
     'nowho': bool,
     'forcesittable': bool,
-    'allowshouts': bool,
-    'allowlarge': bool,
     'notab': bool,
     'nonovelty': bool,
     'rating': str,
     'allow32bitart': bool,
-    'ismodern': bool
+    'ismodern': bool,
+    'parentalcontrols': bool
 }
 
 class Dream:
     def __init__(self, version = 1.5, **parameters):
         self.properties = {}
         for parameter in parameters:
             if parameter.lower() not in DreamTypeCast:
@@ -104,20 +105,20 @@
             self._lighting = TileAccessor(self, "_lighting")
             self._ambient = TileAccessor(self, "_ambient")
     
     def coordinateToIndex(self, x, y):
         return (self.height * x) + y
     
     def __getitem__(self, key):
-        self.parameters[key]
+        self.properties[key]
 
     def __setitem__(self, key, value):
         if parameter.lower() not in DreamTypeCast:
-            raise ValueError("Unknown parameter {}".format(parameter))
-        self.parameters[key] = value
+            print("[WARN] Unknown dream parameter {}".format(parameter))
+        self.properties[key] = value
     
     @property
     def width(self):
         return self.properties["width"]
     
     @width.setter
     def width(self, value):
```

### Comparing `libfurc-0.1.3/libfurc/fox5.py` & `libfurc-0.1.4/libfurc/fox5.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,55 +25,60 @@
 def Decompress(data):
     return lzma.decompress(data, format=lzma.FORMAT_ALONE)
     
 class Fox5Error(Exception):
     pass
 
 class Fox5Image:
-    def __init__(self, width = 0, height = 0, format = 0, data = None):
+    def __init__(self, width = 0, height = 0, format = 0, data = None, compressed = False):
         self.width = width
         self.height = height
         self.format = format
         self.__data__ = data
-        self.compressed = None
+        self.compressed = compressed
     
     def __repr__(self):
         return "<{} Width={}; Height={}; Format={}>".format(self.__class__.__name__, self.width, self.height, self.format)
     
     def __len__(self):
         return len(self.__data__)
     
     @property
     def data(self):
         return self.__data__
     
     @data.setter
     def data(self, value):
-        self.__data__ = data
-        self.compressed = None
+        self.__data__ = value
+        self.compressed = False
     
     def compress(self):
         if not self.compressed:
-            self.compressed = Compress(self.data)
-        return self.compressed
+            self.data = Compress(self.data)
+            self.compressed = True
+        return self.data
+    
+    def decompress(self):
+        if self.compressed:
+            self.data = Decompress(self.data)
+            self.compressed = False
+        return self.data
     
     @classmethod
     def fromPIL(cls, im):
         data = b""
         for pixel in im.getdata():
             data += bytes((pixel[3], pixel[0], pixel[1], pixel[2]))
         
-        return cls(im.width, im.height, 1, data)
+        return cls(im.width, im.height, 1, data, False)
     
     def toPIL(self):
+        self.decompress()
         if self.format == 1:
-            data = b""
-            for pixel in range(0, len(self.data), 4):
-                data += bytes((self.data[pixel+1], self.data[pixel+2], self.data[pixel+3], self.data[pixel]))
-            return Image.frombytes('RGBA', (self.width, self.height), data)
+            return Image.frombytes('RGBA', (self.width, self.height), self.data, "raw", "ARGB")
         elif self.format == 2:
             return Image.frombytes('L', (self.width, self.height), self.data)
 
 sList = struct.Struct(">BI")
 sUInt8 = struct.Struct(">B")
 sUInt16 = struct.Struct(">H")
 sInt16 = struct.Struct(">h")
@@ -477,15 +482,15 @@
                 data = foxhandle.read(compressedSize)
                 
                 #Decrypt if needed
                 if self.parent.encryption == 1:
                     uncompressedSize = width * height * (4 if fmt == 1 else 1)
                     data = Fox5Cipher(data, uncompressedSize, self.parent.seed)
                 
-                im = Fox5Image(width, height, fmt, Decompress(data))
+                im = Fox5Image(width, height, fmt, data, True)
                 self["ImageList"].append(im)
             return True
 
 sFox5Footer = struct.Struct(">BBxxII8s")
 class Fox5File(Fox5List):
     __level__ = -1
     __childtype__ = Fox5Body
```

### Comparing `libfurc-0.1.3/libfurc.egg-info/PKG-INFO` & `libfurc-0.1.4/libfurc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libfurc
-Version: 0.1.3
+Version: 0.1.4
 Summary: A library for handling Furcadia things.
 Home-page: https://github.com/FelixWolf/libFurc
 Author: Félix
 Author-email: felix.wolfz@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `libfurc-0.1.3/setup.py` & `libfurc-0.1.4/setup.py`

 * *Files identical despite different names*

