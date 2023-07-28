# Comparing `tmp/veilcord-0.0.3.1.tar.gz` & `tmp/veilcord-0.0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veilcord-0.0.3.1.tar", last modified: Wed Jul 26 02:27:07 2023, max compression
+gzip compressed data, was "veilcord-0.0.3.2.tar", last modified: Fri Jul 28 22:22:41 2023, max compression
```

## Comparing `veilcord-0.0.3.1.tar` & `veilcord-0.0.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 02:27:07.828716 veilcord-0.0.3.1/
--rw-rw-rw-   0        0        0     1085 2023-05-20 20:15:11.000000 veilcord-0.0.3.1/LICENSE
--rw-rw-rw-   0        0        0     3040 2023-07-26 02:27:07.828716 veilcord-0.0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1820 2023-07-26 01:58:21.000000 veilcord-0.0.3.1/README.md
--rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 veilcord-0.0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-26 02:27:07.829716 veilcord-0.0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1667 2023-07-26 02:26:31.000000 veilcord-0.0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 02:27:07.814480 veilcord-0.0.3.1/veilcord/
--rw-rw-rw-   0        0        0     9213 2023-07-26 02:26:47.000000 veilcord-0.0.3.1/veilcord/__init__.py
--rw-rw-rw-   0        0        0    10505 2023-07-26 02:25:10.000000 veilcord-0.0.3.1/veilcord/__main__.py
--rw-rw-rw-   0        0        0     5228 2023-07-26 02:26:23.000000 veilcord-0.0.3.1/veilcord/__session__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 02:27:07.827309 veilcord-0.0.3.1/veilcord.egg-info/
--rw-rw-rw-   0        0        0     3040 2023-07-26 02:27:07.000000 veilcord-0.0.3.1/veilcord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-07-26 02:27:07.000000 veilcord-0.0.3.1/veilcord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 02:27:07.000000 veilcord-0.0.3.1/veilcord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-07-26 02:27:07.000000 veilcord-0.0.3.1/veilcord.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-26 02:27:07.000000 veilcord-0.0.3.1/veilcord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-28 22:22:41.517614 veilcord-0.0.3.2/
+-rw-rw-rw-   0        0        0     1085 2023-05-20 20:15:11.000000 veilcord-0.0.3.2/LICENSE
+-rw-rw-rw-   0        0        0     3462 2023-07-28 22:22:41.516615 veilcord-0.0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2242 2023-07-28 22:11:38.000000 veilcord-0.0.3.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 veilcord-0.0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-28 22:22:41.517614 veilcord-0.0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1667 2023-07-28 20:52:56.000000 veilcord-0.0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 22:22:41.501150 veilcord-0.0.3.2/veilcord/
+-rw-rw-rw-   0        0        0     9215 2023-07-28 22:12:14.000000 veilcord-0.0.3.2/veilcord/__init__.py
+-rw-rw-rw-   0        0        0    11729 2023-07-28 22:20:51.000000 veilcord-0.0.3.2/veilcord/__main__.py
+-rw-rw-rw-   0        0        0     5313 2023-07-28 22:15:32.000000 veilcord-0.0.3.2/veilcord/__session__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 22:22:41.516615 veilcord-0.0.3.2/veilcord.egg-info/
+-rw-rw-rw-   0        0        0     3462 2023-07-28 22:22:41.000000 veilcord-0.0.3.2/veilcord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-07-28 22:22:41.000000 veilcord-0.0.3.2/veilcord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 22:22:41.000000 veilcord-0.0.3.2/veilcord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-07-28 22:22:41.000000 veilcord-0.0.3.2/veilcord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-28 22:22:41.000000 veilcord-0.0.3.2/veilcord.egg-info/top_level.txt
```

### Comparing `veilcord-0.0.3.1/LICENSE` & `veilcord-0.0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `veilcord-0.0.3.1/PKG-INFO` & `veilcord-0.0.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veilcord
-Version: 0.0.3.1
+Version: 0.0.3.2
 Summary: VeilCord // @imvast
 Home-page: http://pypi.python.org/pypi/veilcord
 Author: @imvast
 Author-email: dev@vast.sh
 License: MIT
 Project-URL: Homepage, https://github.com/imvast/veilcord
 Project-URL: Suggestions, https://github.com/imvast/veilcord/issues
@@ -62,27 +62,43 @@
 # GETTING ALL THE COOKIES AND FINGERPRINT
 fp, cookies = veilcord.getFingerprint(xsup, cookieType="json")
 print(f"(+) Retrieved Fingerprint: {fp}")
 print(f"(+) Retrieved Cookies: {cookies}")
 # returns a set.  [0] - Fingerprint  |  [1] - COOKIESJAR or JSON
 
 
-# GET THE NEW SESSION ID BS
+# GET THE NEW SESSION ID BS  || this can also be used for websocket connection but not recommended as of rn
 session = veilcord.openSession()
 
 token = ""
 sessionID = veilcord.getSession(
     session = session, # the session returned from veilcord.openSession()
     token = token, # obv the token
     keep_alive = False,  # keep the session alive | only needed if ur code is slow (avg. session is live for ~40 seconds.)
     show_hb = False # prints when it sends the heartbeat and when the next one is
 )
 print(f"(+) Got Session ID: {sessionID}")
 
 # close the session, if keepAlive is enabled.
 # veilcord.closeSession(session)
 
+
+## Extra Cool Stuff
+
+# get discord build number
+buildNum = VeilCord.getBuildNum()
+print(buildNum)
+
+# -- or with all the extra stats
+
+buildNum, buildTS, url, time_taken = VeilCord.getBuildNum(withStat=True)
+print("URL:", url)
+print("Build Number:", buildNum)
+print("Build Timestamp:", buildTS)
+print("Elapsed:", time_taken)
+
+
 ```
 
 ---
 
 ## * [imvast@discord](https://discord.com/users/1118654675898617891) | [imvast@github](https://github.com/imvast) | [vast.sh](https://vast.sh) *
```

### Comparing `veilcord-0.0.3.1/setup.py` & `veilcord-0.0.3.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/env python
 
 from setuptools import setup, find_packages
 
-vers = "0.0.3.1"
+vers = "0.0.3.2"
 
 setup(
     name="veilcord",
     version=vers,
     description="VeilCord // @imvast",
     long_description_content_type="text/markdown",
     long_description=open("README.md", encoding="utf-8").read(),
```

### Comparing `veilcord-0.0.3.1/veilcord/__init__.py` & `veilcord-0.0.3.2/veilcord/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+__author__  = "github.com/imvast"                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   ;_0110001001101111011011110110110001110101011100110110010101100100011000100110010101100110011011110111001001100101=False
+__title__   = 'VeilCord'                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           ;print("MADE BY VAST DONT CHANGE CREDITS U QUEER") if __author__ != "github.com/imvast" else None                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     
+__version__ = '0.0.3.3'
+
 from .__main__    import *
 
 from terminut     import printf as print
 from colorama     import Fore
 from os           import system
 from sys          import executable
 from requests     import get
 
 
-__author__  = "github.com/imvast"                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   ;_0110001001101111011011110110110001110101011100110110010101100100011000100110010101100110011011110111001001100101=False
-__title__   = 'VeilCord'                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           ;print("MADE BY VAST DONT CHANGE CREDITS U QUEER") if __author__ != "github.com/imvast" else None                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     
-__version__ = '0.0.3.1'
 
 CURRENT_VERSION = str(get('https://pypi.org/project/veilcord/').text.split('<h1 class="package-header__name">\n        veilcord ')[1].split('\n')[0])
 
 
 if __version__ < CURRENT_VERSION:
     print(
         f"[VeilCord] Version Out-of-Date. Please upgrade by using: \"python.exe -m pip install -U veilcord\"",
```

### Comparing `veilcord-0.0.3.1/veilcord/__main__.py` & `veilcord-0.0.3.2/veilcord/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,59 +3,80 @@
 from base64       import b64encode
 from json         import dumps
 from tls_client   import Session
 from typing       import Optional, Literal, List, Union
 from json         import dumps, loads
 from time         import sleep, time
 from httpx        import get
-from re           import search
+from re           import search, findall
 from asyncio      import run
 
 
-
 class HTTPClient:
     def __init__(self):
-        self.session = Session(client_identifier="firefox_113", random_tls_extension_order=True)
-
-
-class Globals:
-    session_id = None
-    sessionThread = None
-    sessionOn = True
+        self.session = Session(client_identifier="firefox_115", random_tls_extension_order=True)
 
 
 class VeilCord:
     def __init__(
         self, 
         session:        Optional[Session] = HTTPClient().session,
         device_type:    Literal["browser", "mobile", "app"] = "browser", 
         user_agent:     Optional[str] = None,
         device_version: Optional[str] = None
     ) -> None:
         self.session = HTTPClient().session if session is None else session
-        self.user_agent_browser = "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/113.0"
+        self.user_agent_browser = "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/115.0"
         self.user_agent_mobile  = "Discord-Android/170014;RNA"
-        self.user_agent_app     = "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) discord/1.0.9013 Chrome/108.0.5359.215 Electron/22.3.2 Safari/537.36"
+        self.user_agent_app     = "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) discord/1.0.9015 Chrome/108.0.5359.215 Electron/22.3.12 Safari/537.36"
         self.device_type_browser = "Windows"
         self.device_type_mobile  = "Android"
-        self.currentBuildNUM = 199933
+        
+        self.currentBuildNUM = VeilCord.getBuildNum()
+        self.currentCapNum = VeilCord.getCapabilitiesNum()
+        
         if user_agent and not device_version:
-            raise SyntaxError("If using custom useragent you must provide the version. Such as: 113.0")
+            raise SyntaxError("If using custom useragent you must provide the version. Such as: 115.0")
         if device_type == "browser":
             self.device_type = "browser"
             self.user_agent = self.user_agent_browser if user_agent is None else user_agent
         elif device_type == "mobile":
             self.device_type = "mobile"
             self.user_agent = self.user_agent_mobile if user_agent is None else user_agent
         elif device_type == "app":
             self.device_type = "app"
             self.user_agent = self.user_agent_app if user_agent is None else user_agent
         else:
             raise ValueError("An invalid device_type was provided. Acceptable values: ['browser', 'mobile', 'app']")
         
+    # session mg
+        
+    def openSession(self):
+        session_manager = SessionManager(self.user_agent, self.currentBuildNUM, self.device_type, self.currentCapNum)
+        return session_manager
+        
+    def getSession(
+        self, 
+        session, 
+        token: str, 
+        keep_alive: bool = False, 
+        show_hb: bool = False
+    ) -> Union[str, None]:
+        if session is None:
+            session = SessionManager(self.user_agent, self.currentBuildNUM, self.device_type, self.currentCapNum)
+            if keep_alive:
+                raise SyntaxError("Session cannot be null with keepAlive enabled.")
+        session_id = run(session.get_session(token, keep_alive, show_hb))
+        return session_id
+
+    def closeSession(self, session):
+        session.close_session()
+        return True
+    
+
     
     def generateXProp(
         self,
         browser_name: Optional[str] = None, 
         browser_vers: Optional[str] = None,
         build_num:    Optional[int] = None
     ):
@@ -73,25 +94,25 @@
             }
         elif self.device_type == "browser":
             xsup = {
                 "os": self.device_type_browser,
                 "browser": browser_name if browser_name else "Firefox",
                 "system_locale": "en-US",
                 "browser_user_agent": self.user_agent,
-                "browser_version": browser_vers if browser_vers else "113.0.0.0",
+                "browser_version": browser_vers if browser_vers else "115.0.0.0",
                 "os_version": "10",
                 "release_channel": "stable",
                 "client_build_number": build_num if build_num else self.currentBuildNUM,
             }
         elif self.device_type == "app":
             xsup = {
                 "os": self.device_type_browser,
                 "browser": "Discord Client",
                 "release_channel": "stable",
-                "client_version": browser_vers if browser_vers else "1.0.9013",
+                "client_version": browser_vers if browser_vers else "1.0.9015",
                 "os_version": "10.0.22621",
                 "os_arch": "x64",
                 "system_locale": "en-US",
                 "browser_user_agent": self.user_agent_app,
                 "browser_version": "22.3.2",
                 "client_build_number": build_num if build_num else self.currentBuildNUM,
                 "native_build_number": 32266,
@@ -168,88 +189,91 @@
         response = self.session.get('https://discord.com/api/v9/experiments', headers=headers)
         if withCookies:
             cookies = response.cookies if cookieType == "cookiejar" else dumps(response.cookies.get_dict())
             return response.json().get("fingerprint"), cookies
         return response.json().get("fingerprint")
 
 
-    
     # non self #
     
-    def getBuildNum():
-        headers = {
-            'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/113.0',
-            'Accept': '*/*',
-            'Accept-Language': 'en-US,en;q=0.5',
-            'Accept-Encoding': 'gzip, deflate, br',
-            'Alt-Used': 'discord.com',
-            'Connection': 'keep-alive',
-            'Referer': 'https://discord.com/',
-            'Sec-Fetch-Dest': 'script',
-            'Sec-Fetch-Mode': 'no-cors',
-            'Sec-Fetch-Site': 'same-origin',
-            'Pragma': 'no-cache',
-            'Cache-Control': 'no-cache',
-            'TE': 'trailers',
-        }
-        html = get(f"https://discord.com/app?_={(time() * 1000)}", headers=headers).text
-
-        last_index = html.rfind('/assets/')
-        closing_quote_index = html.find('"', last_index)
-        prefetched_script = html[last_index:closing_quote_index]
-
-        response = get(f'https://discord.com{prefetched_script}', headers=headers).text
+    def getBuildNum(withStat: bool = False):
+        def scrape():
+            html_content = get('https://discord.com/channels/@me').text
+            script_tags = findall(r'<script\s+src="(.*?)".*?>', html_content)
+
+            # print(f"Searching {len(script_tags)} scripts...\n")
+
+            for url in script_tags:
+                input_string = get(f"https://discord.com{url}").text
+                if "buildnum" not in input_string.lower():
+                    continue
+
+                build_number_match = search(r'"buildNumber",null!==\(t="(\d+)"\)', input_string)
+                build_timestamp_match = search(r'\("builtAt",String\("(\d+)"\)\);', input_string)
+
+                build_number = build_number_match.group(1) if build_number_match else None
+                build_timestamp = build_timestamp_match.group(1) if build_timestamp_match else None
+
+                if build_number is not None:
+                    return build_number, build_timestamp, url
+
+            return 216114, build_timestamp, url
+
+        start = time()
+        build_number, build_timestamp, url = scrape()
+        time_taken = round(time() - start, 2), "s"
+        if withStat:
+            return build_number, build_timestamp, url, time_taken
+        return build_number
 
-        buildnum = response.split("buildNumber:\"")[1].split("\"")[0]
-        
-        return buildnum
-    
     
+    def getCapabilitiesNum():
+        try:
+            headers = {
+                "cookie": "OptanonConsent=isIABGlobal=false&datestamp=Thu+Jul+27+2023+21%3A05%3A10+GMT-0400+(Eastern+Daylight+Time)&version=6.33.0&hosts=&landingPath=https%3A%2F%2Fdiscord.com%2F&groups=C0001%3A1%2CC0002%3A1%2CC0003%3A1",
+            }
+
+            resp_welcome = get("https://discord.com/welcome/", headers=headers)
+
+            pattern = r'src="([^"]+)"'
+            matches = findall(pattern, resp_welcome.text)
+
+            if not matches:
+                return 16381
+
+            last_script_link = matches[-1]
+            resp_script = get("https://discord.com" + last_script_link)
+
+            cappattern = r'capabilities:(\d+)'
+            match = search(cappattern, resp_script.text)
+
+            if match:
+                capabilities_number = match.group(1)
+                return int(capabilities_number)
+            else:
+                return 16381
+        except:
+            return 16381 # last known version
+
     def extractCode(invite):
         """Extracts the invite code from a Discord invite link"""
         code_regex = r"(?:(?:http:\/\/|https:\/\/)?discord\.gg\/|discordapp\.com\/invite\/|discord\.com\/invite\/)?([a-zA-Z0-9-]+)"
         match = search(code_regex, invite)
         if match:
             try:
                 return match.group(1)
             except:
                 return match.group(0)
         else:
             return None
         
-        
-        
-    def openSession(self):
-        session_manager = SessionManager(self.user_agent, self.currentBuildNUM, self.device_type)
-        return session_manager
-        
-    def getSession(
-        self, 
-        session, 
-        token: str, 
-        keep_alive: bool = False, 
-        show_hb: bool = False
-    ) -> Union[str, None]:
-        if session is None:
-            session = SessionManager(self.user_agent, self.currentBuildNUM, self.device_type)
-            if keep_alive:
-                raise SyntaxError("Session cannot be null with keepAlive enabled.")
-        session_id = run(session.get_session(token, keep_alive, show_hb))
-        return session_id
 
-    def closeSession(self, session):
-        session.close_session()
-        return True
-    
-    
 
-      
-        
-        
-        
+
+
         
 ## out of the class for old projects use
 
 def extractCode(invite):
     """Extracts the invite code from a Discord invite link"""
     code_regex = r"(?:(?:http:\/\/|https:\/\/)?discord\.gg\/|discordapp\.com\/invite\/|discord\.com\/invite\/)?([a-zA-Z0-9-]+)"
     match = search(code_regex, invite)
```

### Comparing `veilcord-0.0.3.1/veilcord/__session__.py` & `veilcord-0.0.3.2/veilcord/__session__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from websocket import WebSocket
 from json      import dumps, loads
 from terminut  import printf as print
 from asyncio   import sleep, create_task
 
 
 class SessionManager:
-    def __init__(self, user_agent, build_num, device_type):
+    def __init__(self, user_agent, build_num, device_type, capabilities_num):
         self.session_id = None
         self.session_task = None
         self.session_on = False
         self.ws = WebSocket()
         
         self.user_agent = user_agent
         self.build_num = build_num
         self.device_type = device_type
+        self.capabilities_num = capabilities_num
         
 
     async def _wsconn(self, token):
         self.ws.connect("wss://gateway.discord.gg/?encoding=json&v=9")
         message = {
             "op": 2,
             "d": {
                 "token": token,
-                "capabilities": 8189,
+                "capabilities": self.capabilities_num,
                 "properties": {
                     "os": "Windows",
                     "browser_user_agent": self.user_agent,
                     "device": "",
                     "system_locale": "en-US",
                     "release_channel": "stable",
                     "client_build_number": self.build_num,
```

### Comparing `veilcord-0.0.3.1/veilcord.egg-info/PKG-INFO` & `veilcord-0.0.3.2/veilcord.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veilcord
-Version: 0.0.3.1
+Version: 0.0.3.2
 Summary: VeilCord // @imvast
 Home-page: http://pypi.python.org/pypi/veilcord
 Author: @imvast
 Author-email: dev@vast.sh
 License: MIT
 Project-URL: Homepage, https://github.com/imvast/veilcord
 Project-URL: Suggestions, https://github.com/imvast/veilcord/issues
@@ -62,27 +62,43 @@
 # GETTING ALL THE COOKIES AND FINGERPRINT
 fp, cookies = veilcord.getFingerprint(xsup, cookieType="json")
 print(f"(+) Retrieved Fingerprint: {fp}")
 print(f"(+) Retrieved Cookies: {cookies}")
 # returns a set.  [0] - Fingerprint  |  [1] - COOKIESJAR or JSON
 
 
-# GET THE NEW SESSION ID BS
+# GET THE NEW SESSION ID BS  || this can also be used for websocket connection but not recommended as of rn
 session = veilcord.openSession()
 
 token = ""
 sessionID = veilcord.getSession(
     session = session, # the session returned from veilcord.openSession()
     token = token, # obv the token
     keep_alive = False,  # keep the session alive | only needed if ur code is slow (avg. session is live for ~40 seconds.)
     show_hb = False # prints when it sends the heartbeat and when the next one is
 )
 print(f"(+) Got Session ID: {sessionID}")
 
 # close the session, if keepAlive is enabled.
 # veilcord.closeSession(session)
 
+
+## Extra Cool Stuff
+
+# get discord build number
+buildNum = VeilCord.getBuildNum()
+print(buildNum)
+
+# -- or with all the extra stats
+
+buildNum, buildTS, url, time_taken = VeilCord.getBuildNum(withStat=True)
+print("URL:", url)
+print("Build Number:", buildNum)
+print("Build Timestamp:", buildTS)
+print("Elapsed:", time_taken)
+
+
 ```
 
 ---
 
 ## * [imvast@discord](https://discord.com/users/1118654675898617891) | [imvast@github](https://github.com/imvast) | [vast.sh](https://vast.sh) *
```

