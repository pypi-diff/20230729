# Comparing `tmp/reolink_aio-0.7.5.tar.gz` & `tmp/reolink_aio-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reolink_aio-0.7.5.tar", last modified: Thu Jul 27 20:43:57 2023, max compression
+gzip compressed data, was "reolink_aio-0.7.6.tar", last modified: Sat Jul 29 19:20:27 2023, max compression
```

## Comparing `reolink_aio-0.7.5.tar` & `reolink_aio-0.7.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 20:43:57.823860 reolink_aio-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-07-27 20:43:44.000000 reolink_aio-0.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     4720 2023-07-27 20:43:57.823860 reolink_aio-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3912 2023-07-27 20:43:44.000000 reolink_aio-0.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 20:43:57.823860 reolink_aio-0.7.5/reolink_aio/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-27 20:43:44.000000 reolink_aio-0.7.5/reolink_aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   194199 2023-07-27 20:43:44.000000 reolink_aio-0.7.5/reolink_aio/api.py
--rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-07-27 20:43:44.000000 reolink_aio-0.7.5/reolink_aio/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)     1379 2023-07-27 20:43:44.000000 reolink_aio-0.7.5/reolink_aio/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     9403 2023-07-27 20:43:44.000000 reolink_aio-0.7.5/reolink_aio/software_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     7935 2023-07-27 20:43:44.000000 reolink_aio-0.7.5/reolink_aio/templates.py
--rw-r--r--   0 runner    (1001) docker     (122)    15330 2023-07-27 20:43:44.000000 reolink_aio-0.7.5/reolink_aio/typings.py
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-27 20:43:44.000000 reolink_aio-0.7.5/reolink_aio/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 20:43:57.823860 reolink_aio-0.7.5/reolink_aio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4720 2023-07-27 20:43:57.000000 reolink_aio-0.7.5/reolink_aio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      439 2023-07-27 20:43:57.000000 reolink_aio-0.7.5/reolink_aio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-27 20:43:57.000000 reolink_aio-0.7.5/reolink_aio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-27 20:43:57.000000 reolink_aio-0.7.5/reolink_aio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-07-27 20:43:57.000000 reolink_aio-0.7.5/reolink_aio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-07-27 20:43:57.000000 reolink_aio-0.7.5/reolink_aio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-27 20:43:57.823860 reolink_aio-0.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1399 2023-07-27 20:43:44.000000 reolink_aio-0.7.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 20:43:57.823860 reolink_aio-0.7.5/tests/
--rw-r--r--   0 runner    (1001) docker     (122)    15443 2023-07-27 20:43:44.000000 reolink_aio-0.7.5/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 19:20:27.817567 reolink_aio-0.7.6/
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-07-29 19:20:13.000000 reolink_aio-0.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4720 2023-07-29 19:20:27.817567 reolink_aio-0.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3912 2023-07-29 19:20:13.000000 reolink_aio-0.7.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 19:20:27.813567 reolink_aio-0.7.6/reolink_aio/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-29 19:20:13.000000 reolink_aio-0.7.6/reolink_aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   194628 2023-07-29 19:20:13.000000 reolink_aio-0.7.6/reolink_aio/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-07-29 19:20:13.000000 reolink_aio-0.7.6/reolink_aio/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1379 2023-07-29 19:20:13.000000 reolink_aio-0.7.6/reolink_aio/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9403 2023-07-29 19:20:13.000000 reolink_aio-0.7.6/reolink_aio/software_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7935 2023-07-29 19:20:13.000000 reolink_aio-0.7.6/reolink_aio/templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15330 2023-07-29 19:20:13.000000 reolink_aio-0.7.6/reolink_aio/typings.py
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-29 19:20:13.000000 reolink_aio-0.7.6/reolink_aio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 19:20:27.817567 reolink_aio-0.7.6/reolink_aio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4720 2023-07-29 19:20:27.000000 reolink_aio-0.7.6/reolink_aio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      439 2023-07-29 19:20:27.000000 reolink_aio-0.7.6/reolink_aio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-29 19:20:27.000000 reolink_aio-0.7.6/reolink_aio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-29 19:20:27.000000 reolink_aio-0.7.6/reolink_aio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-07-29 19:20:27.000000 reolink_aio-0.7.6/reolink_aio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-07-29 19:20:27.000000 reolink_aio-0.7.6/reolink_aio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-29 19:20:27.817567 reolink_aio-0.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1399 2023-07-29 19:20:13.000000 reolink_aio-0.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 19:20:27.817567 reolink_aio-0.7.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    15443 2023-07-29 19:20:13.000000 reolink_aio-0.7.6/tests/test.py
```

### Comparing `reolink_aio-0.7.5/LICENSE` & `reolink_aio-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.5/PKG-INFO` & `reolink_aio-0.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reolink_aio
-Version: 0.7.5
+Version: 0.7.6
 Summary: Reolink NVR/cameras API package
 Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG
 Author-email: starkiller.og@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reolink_aio Version: 0.7.5 Summary: Reolink NVR/
+Metadata-Version: 2.1 Name: reolink_aio Version: 0.7.6 Summary: Reolink NVR/
 cameras API package Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG Author-email: starkiller.og@gmail.com License: MIT
 Platform: any Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier: Topic
 :: Software Development :: Libraries Classifier: Topic :: Home Automation
 Classifier: Programming Language :: Python Classifier: Programming Language ::
```

### Comparing `reolink_aio-0.7.5/README.md` & `reolink_aio-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.5/reolink_aio/api.py` & `reolink_aio-0.7.6/reolink_aio/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 )
 from .software_version import SoftwareVersion, NewSoftwareVersion, MINIMUM_FIRMWARE
 from .utils import datetime_to_reolink_time, reolink_time_to_datetime
 
 MANUFACTURER = "Reolink"
 DEFAULT_STREAM = "sub"
 DEFAULT_PROTOCOL = "rtmp"
-DEFAULT_TIMEOUT = 60
+DEFAULT_TIMEOUT = 30
 RETRY_ATTEMPTS = 3
 MAX_CHUNK_ITEMS = 40
 DEFAULT_RTMP_AUTH_METHOD = "PASSWORD"
 SUBSCRIPTION_TERMINATION_TIME = 15  # minutes
 LONG_POLL_TIMEOUT = 5  # minutes
 
 MOTION_DETECTION_TYPE = "motion"
@@ -88,14 +88,15 @@
         stream: str = DEFAULT_STREAM,
         timeout: int = DEFAULT_TIMEOUT,
         rtmp_auth_method: str = DEFAULT_RTMP_AUTH_METHOD,
         aiohttp_get_session_callback=None,
     ):
         self._send_mutex = asyncio.Lock()
         self._login_mutex = asyncio.Lock()
+        self._long_poll_mutex = asyncio.Lock()
 
         ##############################################################################
         # Host
         self._url: str = ""
         self._use_https: Optional[bool] = use_https
         self._host: str = host
         self._port: Optional[int] = port
@@ -376,15 +377,17 @@
     @property
     def session_active(self) -> bool:
         if self._token is not None and self._lease_time is not None and self._lease_time > (datetime.now() + timedelta(seconds=5)):
             return True
         return False
 
     @property
-    def timeout(self) -> Optional[float]:
+    def timeout(self) -> float:
+        if self._timeout.total is None:
+            return DEFAULT_TIMEOUT
         return self._timeout.total
 
     @property
     def user_level(self) -> str:
         """Check if the user has admin authorisation."""
         if self._users is None or len(self._users) < 1:
             return "unknown"
@@ -3709,81 +3712,82 @@
 
             if expected_response_type == "application/octet-stream":
                 # response needs to be read or released from the calling function
                 return response
 
             response.release()
             raise InvalidContentTypeError(f"Expected {expected_response_type}, unexpected data received: {data!r}")
-        except aiohttp.ClientConnectorError as err:
+        except (aiohttp.ClientConnectorError, aiohttp.ServerConnectionError) as err:
             if retry <= 0:
+                _LOGGER.debug("Host %s:%s: connection error: %s", self._host, self._port, str(err))
                 await self.expire_session()
-                _LOGGER.error("Host %s:%s: connection error: %s", self._host, self._port, str(err))
                 raise ReolinkConnectionError(f"Host {self._host}:{self._port}: connection error: {str(err)}") from err
             _LOGGER.debug("Host %s:%s: connection error, trying again: %s", self._host, self._port, str(err))
             return await self.send(body, param, expected_response_type, retry)
         except asyncio.TimeoutError as err:
             if retry <= 0:
-                await self.expire_session()
-                _LOGGER.error(
-                    "Host %s:%s: connection timeout exception. Please check the connection to this host.",
+                _LOGGER.debug(
+                    "Host %s:%s: connection timeout. Please check the connection to this host.",
                     self._host,
                     self._port,
                 )
+                await self.expire_session()
                 raise ReolinkTimeoutError(f"Host {self._host}:{self._port}: Timeout error: {str(err)}") from err
             _LOGGER.debug(
-                "Host %s:%s: connection timeout exception, trying again.",
+                "Host %s:%s: connection timeout, trying again.",
                 self._host,
                 self._port,
             )
             return await self.send(body, param, expected_response_type, retry)
         except ApiError as err:
-            await self.expire_session(unsubscribe=False)
             _LOGGER.error("Host %s:%s: API error: %s.", self._host, self._port, str(err))
+            await self.expire_session(unsubscribe=False)
             raise err
         except CredentialsInvalidError as err:
-            await self.expire_session()
             _LOGGER.error("Host %s:%s: login attempt failed.", self._host, self._port)
+            await self.expire_session()
             raise err
         except InvalidContentTypeError as err:
-            await self.expire_session(unsubscribe=False)
             _LOGGER.debug("Host %s:%s: content type error: %s.", self._host, self._port, str(err))
+            await self.expire_session(unsubscribe=False)
             raise err
         except Exception as err:
-            await self.expire_session()
             _LOGGER.error('Host %s:%s: unknown exception "%s" occurred, traceback:\n%s\n', self._host, self._port, str(err), traceback.format_exc())
+            await self.expire_session()
             raise err
 
     async def send_reolink_com(
         self,
         URL: str,
         expected_response_type: Literal["application/json"] = "application/json",
     ) -> dict[str, Any]:
         """Generic send method for reolink.com site."""
 
         if self._aiohttp_session.closed:
             self._aiohttp_session = self._get_aiohttp_session()
 
+        com_timeout = aiohttp.ClientTimeout(total=2 * self.timeout)
         try:
-            response = await self._aiohttp_session.get(url=URL)
-        except aiohttp.ClientConnectorError as err:
+            response = await self._aiohttp_session.get(url=URL, timeout=com_timeout)
+        except (aiohttp.ClientConnectorError, aiohttp.ServerConnectionError) as err:
             raise ReolinkConnectionError(f"Connetion error to {URL}: {str(err)}") from err
         except asyncio.TimeoutError as err:
             raise ReolinkTimeoutError(f"Timeout requesting {URL}: {str(err)}") from err
 
         if response.status != 200:
             response.release()
             raise ApiError(f"Request to {URL} returned HTTP status ERROR code {response.status}/{response.reason}")
 
         if response.content_type != expected_response_type:
             response.release()
             raise InvalidContentTypeError(f"Request to {URL}, expected type '{expected_response_type}' but received '{response.content_type}'")
 
         try:
             data = await response.text()
-        except aiohttp.ClientConnectorError as err:
+        except (aiohttp.ClientConnectorError, aiohttp.ServerConnectionError) as err:
             raise ReolinkConnectionError(f"Connetion error reading response from {URL}: {str(err)}") from err
         except asyncio.TimeoutError as err:
             raise ReolinkTimeoutError(f"Timeout reading response from {URL}: {str(err)}") from err
 
         try:
             json_data = json_loads(data)
         except (TypeError, JSONDecodeError) as err:
@@ -3847,15 +3851,15 @@
             "UsernameToken": str(uuid.uuid4()),
             "Username": self._username,
             "PasswordDigest": digest_pwd.decode("utf8"),
             "Nonce": nonce.decode("utf8"),
             "Created": time_created,
         }
 
-    async def subscription_send(self, headers, data, timeout: aiohttp.ClientTimeout | None = None) -> str:
+    async def subscription_send(self, headers, data, timeout: aiohttp.ClientTimeout | None = None, mutex: asyncio.Lock | None = None) -> str:
         """Send subscription data to the camera."""
         if self._subscribe_url is None:
             await self.get_state("GetNetPort")
 
         if self._subscribe_url is None:
             raise NotSupportedError(f"subscription_send: failed to retrieve subscribe_url from {self._host}:{self._port}")
 
@@ -3867,17 +3871,19 @@
         )
 
         if self._aiohttp_session.closed:
             self._aiohttp_session = self._get_aiohttp_session()
 
         if timeout is None:
             timeout = self._timeout
+        if mutex is None:
+            mutex = self._send_mutex
 
         try:
-            async with self._send_mutex:
+            async with mutex:
                 response = await self._aiohttp_session.post(
                     url=self._subscribe_url,
                     data=data,
                     headers=headers,
                     allow_redirects=False,
                     timeout=timeout,
                 )
@@ -3892,15 +3898,15 @@
             )
 
             if response.status != 200:
                 raise ApiError(f"Host {self._host}:{self._port}: subscription request got a response with wrong HTTP status {response.status}: {response.reason}")
 
             return response_text
 
-        except aiohttp.ClientConnectorError as err:
+        except (aiohttp.ClientConnectorError, aiohttp.ServerConnectionError) as err:
             raise ReolinkConnectionError(f"Host {self._host}:{self._port}: connection error: {str(err)}.") from err
         except asyncio.TimeoutError as err:
             raise ReolinkTimeoutError(f"Host {self._host}:{self._port}: connection timeout exception.") from err
 
     async def subscribe(self, webhook_url: str | None = None, sub_type: Literal[SubType.push, SubType.long_poll] = SubType.push, retry: bool = False):
         """Subscribe to ONVIF events."""
         headers = templates.HEADERS
@@ -4066,15 +4072,15 @@
 
         xml = template.format(**parameters)
         _LOGGER.debug("Reolink %s requesting ONVIF pull point message", self.nvr_name)
 
         timeout = aiohttp.ClientTimeout(total=LONG_POLL_TIMEOUT * 60 + 30, connect=self.timeout)
 
         try:
-            response = await self.subscription_send(headers, xml, timeout)
+            response = await self.subscription_send(headers, xml, timeout, mutex=self._long_poll_mutex)
         except ReolinkError as err:
             raise SubscriptionError(f"Failed to request pull point message: {str(err)}") from err
 
         root = XML.fromstring(response)
         if root.find(".//{http://docs.oasis-open.org/wsn/b-2}NotificationMessage") is None:
             _LOGGER.debug("Reolink %s received ONVIF pull point message without event", self.nvr_name)
             return []
```

### Comparing `reolink_aio-0.7.5/reolink_aio/enums.py` & `reolink_aio-0.7.6/reolink_aio/enums.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.5/reolink_aio/exceptions.py` & `reolink_aio-0.7.6/reolink_aio/exceptions.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.5/reolink_aio/software_version.py` & `reolink_aio-0.7.6/reolink_aio/software_version.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.5/reolink_aio/templates.py` & `reolink_aio-0.7.6/reolink_aio/templates.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.5/reolink_aio/typings.py` & `reolink_aio-0.7.6/reolink_aio/typings.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.5/reolink_aio/utils.py` & `reolink_aio-0.7.6/reolink_aio/utils.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.5/reolink_aio.egg-info/PKG-INFO` & `reolink_aio-0.7.6/reolink_aio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reolink-aio
-Version: 0.7.5
+Version: 0.7.6
 Summary: Reolink NVR/cameras API package
 Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG
 Author-email: starkiller.og@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reolink-aio Version: 0.7.5 Summary: Reolink NVR/
+Metadata-Version: 2.1 Name: reolink-aio Version: 0.7.6 Summary: Reolink NVR/
 cameras API package Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG Author-email: starkiller.og@gmail.com License: MIT
 Platform: any Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier: Topic
 :: Software Development :: Libraries Classifier: Topic :: Home Automation
 Classifier: Programming Language :: Python Classifier: Programming Language ::
```

### Comparing `reolink_aio-0.7.5/setup.py` & `reolink_aio-0.7.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(name='reolink_aio',
-      version='0.7.5',
+      version='0.7.6',
       description='Reolink NVR/cameras API package',
       long_description=README,
       long_description_content_type="text/markdown",
       url='https://github.com/starkillerOG/reolink_aio',
       author='starkillerOG',
       author_email='starkiller.og@gmail.com',
       license='MIT',
```

### Comparing `reolink_aio-0.7.5/tests/test.py` & `reolink_aio-0.7.6/tests/test.py`

 * *Files identical despite different names*

