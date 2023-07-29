# Comparing `tmp/isabelle_client-0.4.0.tar.gz` & `tmp/isabelle_client-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isabelle_client-0.4.0.tar", max compression
+gzip compressed data, was "isabelle_client-0.4.1.tar", max compression
```

## Comparing `isabelle_client-0.4.0.tar` & `isabelle_client-0.4.1.tar`

### file list

```diff
@@ -1,13 +1,24 @@
--rw-r--r--   0        0        0    11358 2022-04-20 19:15:05.623546 isabelle_client-0.4.0/LICENSE
--rw-r--r--   0        0        0     4774 2023-05-29 14:48:08.562757 isabelle_client-0.4.0/README.rst
--rw-r--r--   0        0        0      897 2023-06-29 08:41:16.138251 isabelle_client-0.4.0/isabelle_client/__init__.py
--rw-r--r--   0        0        0     1862 2023-03-29 15:20:44.432379 isabelle_client-0.4.0/isabelle_client/conftest.py
--rw-r--r--   0        0        0    11629 2023-06-29 08:41:16.138251 isabelle_client-0.4.0/isabelle_client/isabelle__client.py
--rw-r--r--   0        0        0        0 2022-04-20 19:15:05.651546 isabelle_client-0.4.0/isabelle_client/py.typed
--rw-r--r--   0        0        0      295 2022-08-04 13:52:33.523169 isabelle_client-0.4.0/isabelle_client/resources/Cygwin-Isabelle.bat
--rw-r--r--   0        0        0     1247 2022-08-24 07:23:02.458778 isabelle_client-0.4.0/isabelle_client/resources/example.txt
--rwxr-xr-x   0        0        0       79 2022-04-20 19:15:05.651546 isabelle_client-0.4.0/isabelle_client/resources/isabelle
--rw-r--r--   0        0        0     5283 2023-06-29 08:41:16.142251 isabelle_client-0.4.0/isabelle_client/socket_communication.py
--rw-r--r--   0        0        0     6766 2023-04-29 10:14:23.981789 isabelle_client-0.4.0/isabelle_client/utils.py
--rw-r--r--   0        0        0     3354 2023-06-29 08:41:16.142251 isabelle_client-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     5840 1970-01-01 00:00:00.000000 isabelle_client-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2022-04-20 19:15:05.623546 isabelle_client-0.4.1/LICENSE
+-rw-r--r--   0        0        0     4774 2023-05-29 14:48:08.562757 isabelle_client-0.4.1/README.rst
+-rw-r--r--   0        0        0      897 2023-07-29 08:16:42.179327 isabelle_client-0.4.1/isabelle_client/__init__.py
+-rw-r--r--   0        0        0     1862 2023-03-29 15:20:44.432379 isabelle_client-0.4.1/isabelle_client/conftest.py
+-rw-r--r--   0        0        0    11834 2023-07-26 08:40:41.307844 isabelle_client-0.4.1/isabelle_client/isabelle__client.py
+-rw-r--r--   0        0        0     4694 2023-07-26 08:40:41.311845 isabelle_client-0.4.1/isabelle_client/isabelle_connector.py
+-rw-r--r--   0        0        0        0 2022-04-20 19:15:05.651546 isabelle_client-0.4.1/isabelle_client/py.typed
+-rw-r--r--   0        0        0      295 2022-08-04 13:52:33.523169 isabelle_client-0.4.1/isabelle_client/resources/Cygwin-Isabelle.bat
+-rw-r--r--   0        0        0     1247 2022-08-24 07:23:02.458778 isabelle_client-0.4.1/isabelle_client/resources/example.txt
+-rwxr-xr-x   0        0        0       79 2022-04-20 19:15:05.651546 isabelle_client-0.4.1/isabelle_client/resources/isabelle
+-rw-r--r--   0        0        0        4 2023-07-26 08:40:41.315846 isabelle_client-0.4.1/isabelle_client/resources/isabelle-responses/cancel
+-rw-r--r--   0        0        0      123 2023-07-26 08:40:41.323847 isabelle_client-0.4.1/isabelle_client/resources/isabelle-responses/help
+-rw-r--r--   0        0        0       90 2023-07-26 08:40:41.327848 isabelle_client-0.4.1/isabelle_client/resources/isabelle-responses/purge_theories
+-rw-r--r--   0        0        0      864 2023-07-26 08:40:41.331848 isabelle_client-0.4.1/isabelle_client/resources/isabelle-responses/session_build
+-rw-r--r--   0        0        0      337 2023-07-26 08:40:41.335849 isabelle_client-0.4.1/isabelle_client/resources/isabelle-responses/session_start
+-rw-r--r--   0        0        0      135 2023-07-26 08:40:41.339850 isabelle_client-0.4.1/isabelle_client/resources/isabelle-responses/session_stop
+-rw-r--r--   0        0        0        4 2023-07-26 08:40:41.339850 isabelle_client-0.4.1/isabelle_client/resources/isabelle-responses/shutdown
+-rw-r--r--   0        0        0       30 2023-07-26 08:40:41.343850 isabelle_client-0.4.1/isabelle_client/resources/isabelle-responses/unknown
+-rw-r--r--   0        0        0      699 2023-07-26 08:40:41.347851 isabelle_client-0.4.1/isabelle_client/resources/isabelle-responses/use_theories
+-rw-r--r--   0        0        0     1040 2023-07-26 08:40:41.347851 isabelle_client-0.4.1/isabelle_client/resources/isabelle-responses/use_theories.Fail
+-rw-r--r--   0        0        0     5443 2023-07-26 08:40:41.351851 isabelle_client-0.4.1/isabelle_client/socket_communication.py
+-rw-r--r--   0        0        0     7183 2023-07-26 08:40:41.351851 isabelle_client-0.4.1/isabelle_client/utils.py
+-rw-r--r--   0        0        0     3560 2023-07-29 08:16:42.187327 isabelle_client-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     5913 1970-01-01 00:00:00.000000 isabelle_client-0.4.1/PKG-INFO
```

### Comparing `isabelle_client-0.4.0/LICENSE` & `isabelle_client-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `isabelle_client-0.4.0/README.rst` & `isabelle_client-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `isabelle_client-0.4.0/isabelle_client/__init__.py` & `isabelle_client-0.4.1/isabelle_client/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # limitations under the License.
 # noqa: D205
 """A Python client to `Isabelle <https://isabelle.in.tum.de>`__ server."""
 from isabelle_client.isabelle__client import IsabelleClient
 from isabelle_client.socket_communication import IsabelleResponse
 from isabelle_client.utils import get_isabelle_client, start_isabelle_server
 
-__version__ = "0.4.0"
+__version__ = "0.4.1"
```

### Comparing `isabelle_client-0.4.0/isabelle_client/conftest.py` & `isabelle_client-0.4.1/isabelle_client/conftest.py`

 * *Files identical despite different names*

### Comparing `isabelle_client-0.4.0/isabelle_client/isabelle__client.py` & `isabelle_client-0.4.1/isabelle_client/isabelle__client.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,26 +62,27 @@
         Execute a command and waits for results.
 
         >>> logger = getfixture("mock_logger")  # noqa: F821
         >>> isabelle_client = IsabelleClient(
         ...     "localhost", 9999, "test_password", logger
         ... )
         >>> test_response = asyncio.run(
-        ...     isabelle_client.execute_command("test_command")
+        ...     isabelle_client.execute_command("unknown command")
         ... )
         >>> print(test_response[-1].response_type)
-        FINISHED
+        ERROR
         >>> print(test_response[-1].response_body)
-        {"session_id": "test_session_id"}
+        "Bad command 'unknown'"
+        >>> # error messages don't return the response length
         >>> print(test_response[-1].response_length)
-        43
+        None
         >>> print(logger.info.mock_calls)
-        [call('test_password\ntest_command\n'),
-         call('OK "connection OK"'),
-         call('43\nFINISHED {"session_id": "test_session_id"}')]
+        [call('test_password\nunknown command\n'),
+         call('OK {"isabelle_id":"mock","isabelle_name":"Isabelle2022"}'),
+         call('ERROR "Bad command \'unknown\'"')]
 
         :param command: a full text of a command to Isabelle
         :param asynchronous: if ``False``, waits for ``OK``; else waits for
             ``FINISHED``
         :returns: a list of Isabelle server responses
         """
         final_message = (
@@ -110,16 +111,16 @@
 
         >>> isabelle_client = IsabelleClient(
         ...     "localhost", 9999, "test_password"
         ... )
         >>> print(isabelle_client.session_build(
         ...     session="test_session", dirs=["."], verbose=True, options=[]
         ... )[-1])
-        43
-        FINISHED {"session_id": "test_session_id"}
+        400
+        FINISHED {"ok":true,"return_code":0,"sessions":[{"session":"Pure",...}
 
         :param session: a name of the session from ROOT file
         :param dirs: where to look for ROOT files
         :param verbose: set to ``True`` for extra verbosity
         :param kwargs: additional arguments
             (see Isabelle System manual for details)
         :returns: an Isabelle response
@@ -132,26 +133,26 @@
             arguments["dirs"] = dirs
         arguments.update(kwargs)
         response = asyncio.run(
             self.execute_command(f"session_build {json.dumps(arguments)}")
         )
         return response
 
-    def session_start(self, session: str = "HOL", **kwargs) -> str:
+    def session_start(self, session: str = "Main", **kwargs) -> str:
         """
         Start a new session.
 
         >>> isabelle_client = IsabelleClient("localhost", 9998, "test")
         >>> print(isabelle_client.session_start(verbose=True))
         Traceback (most recent call last):
             ...
-        ValueError: Unexpected response type: FAILED
+        ValueError: Unexpected response type: ERROR
         >>> isabelle_client = IsabelleClient("localhost", 9999, "test")
         >>> print(isabelle_client.session_start())
-        test_session_id
+        167dd6d8-1eeb-4315-8022-c8c527d9bd87
 
         :param session: a name of a session to start
         :param kwargs: additional arguments
             (see Isabelle System manual for details)
         :returns: a ``session_id``
         :raises ValueError: if the server response is malformed
         """
@@ -192,15 +193,15 @@
         **kwargs,
     ) -> List[IsabelleResponse]:
         """
         Run the engine on theory files.
 
         >>> isabelle_client = IsabelleClient("localhost", 9999, "test")
         >>> test_response = isabelle_client.use_theories(
-        ...     ["test"], master_dir="test", watchdog_timeout=0
+        ...     ["Mock"], master_dir="test", watchdog_timeout=0
         ... )
         >>> print(test_response[-1].response_type)
         FINISHED
 
         :param theories: names of theory files (without extensions!)
         :param session_id: an ID of a session; if ``None``, a new session is
             created and then destroyed after trying to process theories
@@ -249,15 +250,15 @@
     def help(self) -> List[IsabelleResponse]:
         """
         Ask a server to display the list of available commands.
 
         >>> isabelle_client = IsabelleClient("localhost", 9999, "test")
         >>> test_response = isabelle_client.help()
         >>> print(test_response[-1].response_body)
-        ["echo", "help"]
+        ["cancel","echo","help","purge_theories","session_build",...]
 
         :returns: Isabelle server response
         """
         response = asyncio.run(
             self.execute_command("help", asynchronous=False)
         )
         return response
@@ -273,15 +274,15 @@
         Ask a server to purge listed theories from it.
 
         >>> isabelle_client = IsabelleClient("localhost", 9999, "test")
         >>> test_response = isabelle_client.purge_theories(
         ...     "test", [], "dir", True
         ... )
         >>> print(test_response[-1].response_body)
-        {"purged": [], "retained": []}
+        {"purged":[{"node_name":"/tmp/Mock.thy",...}],"retained":[]}
 
         :param session_id: an ID of the session from which to purge theories
         :param theories: a list of theory names to purge from the server
         :param master_dir:  the master directory as in ``use_theories``
         :param purge_all: set to ``True`` attempts to purge all presently
             loaded theories
         :returns: Isabelle server response
```

### Comparing `isabelle_client-0.4.0/isabelle_client/resources/example.txt` & `isabelle_client-0.4.1/isabelle_client/resources/example.txt`

 * *Files identical despite different names*

### Comparing `isabelle_client-0.4.0/isabelle_client/socket_communication.py` & `isabelle_client-0.4.1/isabelle_client/socket_communication.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,25 +69,25 @@
     * a fixed length message after a carriage-return delimited message with
       only one integer number denoting length
 
     >>> async def awaiter():
     ...     test_reader, test_writer = await asyncio.open_connection(
     ...     "localhost", 9999
     ... )
-    ...     test_writer.write(b"ping\n")
+    ...     test_writer.write(b"test_password\nhelp\n")
     ...     result = [str(await get_response_from_isabelle(test_reader))]
     ...     result += [str(await get_response_from_isabelle(test_reader))]
     ...     return result
     >>> print(asyncio.run(awaiter()))
-    ['OK "connection OK"', '43\nFINISHED {"session_id": "test_session_id"}']
+    ['OK {"isabelle_id":"mock","isabelle_name":"Isabelle2022"}', '118\nOK [...]
     >>> async def awaiter():
     ...     test_reader, test_writer = await asyncio.open_connection(
     ...     "localhost", 9998
     ... )
-    ...     test_writer.write(b"ping\n")
+    ...     test_writer.write(b"test_password\nhelp\n")
     ...     result = [str(await get_response_from_isabelle(test_reader))]
     ...     result += [str(await get_response_from_isabelle(test_reader))]
     ...     return result
     >>> print(asyncio.run(awaiter()))
     Traceback (most recent call last):
       ...
     ValueError: Unexpected response from Isabelle: # !!!
@@ -118,27 +118,27 @@
     (until a message of specified 'final' type arrives)
 
     >>> test_logger = getfixture("mock_logger")  # noqa: F821
     >>> async def awaiter():
     ...     test_reader, test_writer = await asyncio.open_connection(
     ...     "localhost", 9999
     ... )
-    ...     test_writer.write(b"ping\n")
+    ...     test_writer.write(b"test_password\nhelp\n")
     ...     result = await get_final_message(
-    ...         test_reader, {"FINISHED"}, test_logger
+    ...         test_reader, {"OK"}, test_logger
     ...     )
     ...     return result
     >>> for response in asyncio.run(awaiter()):
     ...     print(response)
-    OK "connection OK"
-    43
-    FINISHED {"session_id": "test_session_id"}
+    OK {"isabelle_id":"mock","isabelle_name":"Isabelle2022"}
+    118
+    OK ["cancel","echo","help","purge_theories","session_build",...]
     >>> print(test_logger.info.mock_calls)
-    [call('OK "connection OK"'),
-     call('43\nFINISHED {"session_id": "test_session_id"}')]
+    [call('OK {"isabelle_id":"mock","isabelle_name":"Isabelle2022"}'),
+     call('118\nOK ["cancel","echo","help","purge_theories","session_buil...')]
 
     :param reader: a ``StreamReader`` connected to Isabelle server
     :param final_message: a set of possible final message types
     :param logger: a logger where to send all server replies
     :returns: the final response from Isabelle server
     """
     response_list = []
```

### Comparing `isabelle_client-0.4.0/isabelle_client/utils.py` & `isabelle_client-0.4.1/isabelle_client/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 """
 Utilities
 ==========
 
 A collection of different useful functions.
 """
 import asyncio
+import json
 import os
 import re
 import socketserver
 import sys
 from typing import Optional, Tuple
 
 from isabelle_client.isabelle__client import IsabelleClient
@@ -64,15 +65,14 @@
     log_file: Optional[str] = None,
     name: Optional[str] = None,
     port: Optional[int] = None,
 ) -> Tuple[str, asyncio.subprocess.Process]:
     """
     Start Isabelle server.
 
-    >>> import os
     >>> os.environ["PATH"] = "isabelle_client/resources:$PATH"
     >>> print(start_isabelle_server()[0])
     server "isabelle" = 127.0.0.1:9999 (password "test_password")
     <BLANKLINE>
 
     :param log_file: a log file for exceptional output of internal server and
         session operations
@@ -153,47 +153,55 @@
 
 
 class BuggyDummyTCPHandler(socketserver.BaseRequestHandler):
     """A dummy handler to mock bugs in Isabelle server response."""
 
     def handle(self):
         """Return something weird."""
-        request = self.request.recv(1024).decode("utf-8").split("\n")[0]
-        if request == "ping":
+        request = self.request.recv(4096).decode("utf-8").split("\n")[1]
+        if request == "help":
             self.request.sendall(b"5\n")
             self.request.sendall(b"# !!!")
         else:
-            self.request.sendall(b'OK "connection OK"\n')
-            self.request.sendall(b"7\n")
-            self.request.sendall(b"FAILED\n")
+            self.request.sendall(
+                b'OK {"isabelle_id":"mock","isabelle_name":"Isabelle2022"}\n'
+            )
+            self.request.sendall(b"ERROR UNEXPECTED\n")
 
 
 class DummyTCPHandler(socketserver.BaseRequestHandler):
     """A dummy handler to mock Isabelle server."""
 
-    _request_response = {
-        "shutdown": b"OK",
-        "cancel": b"OK",
-        "purge_theories": b'OK {"purged": [], "retained": []}',
-        "help": b'OK ["echo", "help"]',
-    }
+    def _mock_command_execution(self, command: str, arguments: str):
+        filename = command
+        if command == "use_theories":
+            theory_name = json.loads(arguments)["theories"][0]
+            if theory_name != "Mock":
+                filename += f".{theory_name}"
+        with open(
+            str(
+                files("isabelle_client").joinpath(
+                    os.path.join("resources", "isabelle-responses", filename)
+                )
+            ),
+            encoding="utf8",
+        ) as mock_response_file:
+            self.request.sendall(mock_response_file.read().encode())
 
     def handle(self):
         """Return something similar to what Isabelle server does."""
-        request = self.request.recv(1024).decode("utf-8").split("\n")[1]
+        request = self.request.recv(4096).decode("utf-8").split("\n")[1]
         command = request.split(" ")[0]
-        self.request.sendall(b'OK "connection OK"\n')
-        if command == "echo":
-            self.request.sendall(
-                f"OK{request.split(' ')[1]}\n".encode("utf-8")
-            )
+        arguments = request[len(command) :]
         self.request.sendall(
-            self._request_response.get(
-                command, b'43\nFINISHED {"session_id": "test_session_id"}\n'
-            )
+            b'OK {"isabelle_id":"mock","isabelle_name":"Isabelle2022"}\n'
         )
+        if command == "echo":
+            self.request.sendall(f"OK {arguments[1:]}\n".encode())
+        else:
+            self._mock_command_execution(command, arguments)
 
 
 class ReusableDummyTCPServer(socketserver.TCPServer):
     """Ignore TIME-WAIT during testing."""
 
     allow_reuse_address = True
```

### Comparing `isabelle_client-0.4.0/pyproject.toml` & `isabelle_client-0.4.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "isabelle-client"
-version = "0.4.0"
+version = "0.4.1"
 description = "A client to Isabelle proof assistant server"
 authors = ["Boris Shminke <boris@shminke.ml>"]
 license = "Apache-2.0"
 repository = "https://github.com/inpefess/isabelle-client"
 readme = "README.rst"
 classifiers=[
 	"Programming Language :: Python :: 3.11",
@@ -16,14 +16,15 @@
 	"Intended Audience :: Science/Research",
 	"Development Status :: 4 - Beta",
 	"Environment :: Console",
 	"Natural Language :: English",
 	"Topic :: Scientific/Engineering :: Artificial Intelligence",
 	"Typing :: Typed"
 ]
+keywords = ["TCP client", "Isabelle proof assistant", "interactive theorem prover"]
 include = ["isabelle_client/py.typed"]
 
 [tool.poetry.dependencies]
 python = ">= 3.8.1, < 3.12"
 importlib-resources = {version = "*", markers = "python_version < \"3.9\""}
 
 [tool.poetry.group.dev.dependencies]
@@ -38,14 +39,17 @@
 pydocstyle = "*"
 tox = "*"
 pyenchant = "*"
 tbump = "*"
 toml = "*"
 furo = "*"
 jedi = "*"
+pyroma = "*"
+pyupgrade = "*"
+bandit = "*"
 
 [tool.black]
 line-length=79
 
 [tool.isort]
 profile = "black"
 src_paths = ["isabelle_client"]
@@ -115,27 +119,31 @@
     pytest-cov
     flake8
     pydocstyle
     pylint
     mypy
     toml
     pyenchant
+    pyroma
+    bandit
 commands =
     pydocstyle isabelle_client examples
     flake8 isabelle_client examples
     pylint isabelle_client examples
     mypy isabelle_client examples
+    pyroma -n 10 .
+    bandit -r isabelle_client examples
     pytest
 """
 
 [tool.tbump]
 github_url = "https://github.com/inpfess/isabelle-client/"
 
 [tool.tbump.version]
-current = "0.4.0"
+current = "0.4.1"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   '''
```

### Comparing `isabelle_client-0.4.0/PKG-INFO` & `isabelle_client-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: isabelle-client
-Version: 0.4.0
+Version: 0.4.1
 Summary: A client to Isabelle proof assistant server
 Home-page: https://github.com/inpefess/isabelle-client
 License: Apache-2.0
+Keywords: TCP client,Isabelle proof assistant,interactive theorem prover
 Author: Boris Shminke
 Author-email: boris@shminke.ml
 Requires-Python: >=3.8.1,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
```

