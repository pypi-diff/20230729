# Comparing `tmp/nclib-1.0.3.tar.gz` & `tmp/nclib-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nclib-1.0.3.tar", last modified: Wed Jul 26 22:49:13 2023, max compression
+gzip compressed data, was "nclib-1.0.5.tar", last modified: Sat Jul 29 13:47:39 2023, max compression
```

## Comparing `nclib-1.0.3.tar` & `nclib-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxr-x   0 audrey    (1000) audrey    (1000)        0 2023-07-26 22:49:13.997812 nclib-1.0.3/
--rw-r--r--   0 audrey    (1000) audrey    (1000)     1082 2020-06-08 20:54:44.000000 nclib-1.0.3/LICENSE
--rw-rw-r--   0 audrey    (1000) audrey    (1000)     1541 2023-07-26 22:49:13.997812 nclib-1.0.3/PKG-INFO
--rw-r--r--   0 audrey    (1000) audrey    (1000)     1169 2020-06-08 20:54:44.000000 nclib-1.0.3/README.rst
-drwxrwxr-x   0 audrey    (1000) audrey    (1000)        0 2023-07-26 22:49:13.997812 nclib-1.0.3/nclib/
--rw-r--r--   0 audrey    (1000) audrey    (1000)      302 2020-06-08 20:54:44.000000 nclib-1.0.3/nclib/__init__.py
--rw-r--r--   0 audrey    (1000) audrey    (1000)      154 2020-06-08 20:54:44.000000 nclib-1.0.3/nclib/errors.py
--rw-r--r--   0 audrey    (1000) audrey    (1000)    10614 2020-06-08 20:54:44.000000 nclib-1.0.3/nclib/logger.py
--rw-rw-r--   0 audrey    (1000) audrey    (1000)    33617 2023-07-25 17:49:03.000000 nclib-1.0.3/nclib/netcat.py
--rw-r--r--   0 audrey    (1000) audrey    (1000)     6506 2020-06-08 20:54:44.000000 nclib-1.0.3/nclib/process.py
--rw-r--r--   0 audrey    (1000) audrey    (1000)     1951 2020-06-08 20:54:44.000000 nclib-1.0.3/nclib/select.py
--rw-r--r--   0 audrey    (1000) audrey    (1000)     3342 2023-07-25 17:37:26.000000 nclib-1.0.3/nclib/server.py
--rw-rw-r--   0 audrey    (1000) audrey    (1000)    11485 2021-05-03 09:37:29.000000 nclib-1.0.3/nclib/simplesock.py
-drwxrwxr-x   0 audrey    (1000) audrey    (1000)        0 2023-07-26 22:49:13.997812 nclib-1.0.3/nclib.egg-info/
--rw-r--r--   0 audrey    (1000) audrey    (1000)     1541 2023-07-26 22:49:13.000000 nclib-1.0.3/nclib.egg-info/PKG-INFO
--rw-r--r--   0 audrey    (1000) audrey    (1000)      290 2023-07-26 22:49:13.000000 nclib-1.0.3/nclib.egg-info/SOURCES.txt
--rw-r--r--   0 audrey    (1000) audrey    (1000)        1 2023-07-26 22:49:13.000000 nclib-1.0.3/nclib.egg-info/dependency_links.txt
--rw-r--r--   0 audrey    (1000) audrey    (1000)        6 2023-07-26 22:49:13.000000 nclib-1.0.3/nclib.egg-info/top_level.txt
--rwxr-xr-x   0 audrey    (1000) audrey    (1000)     1906 2020-06-08 20:54:44.000000 nclib-1.0.3/serve-stdio
--rw-rw-r--   0 audrey    (1000) audrey    (1000)       38 2023-07-26 22:49:13.997812 nclib-1.0.3/setup.cfg
--rw-rw-r--   0 audrey    (1000) audrey    (1000)     1796 2023-07-26 22:48:41.000000 nclib-1.0.3/setup.py
+drwxrwxr-x   0 audrey    (1000) audrey    (1000)        0 2023-07-29 13:47:39.060313 nclib-1.0.5/
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)     1082 2023-05-26 21:45:16.000000 nclib-1.0.5/LICENSE
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)       17 2023-07-27 20:39:30.000000 nclib-1.0.5/MANIFEST.in
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)     1541 2023-07-29 13:47:39.060313 nclib-1.0.5/PKG-INFO
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)     1169 2023-05-26 21:45:16.000000 nclib-1.0.5/README.rst
+drwxrwxr-x   0 audrey    (1000) audrey    (1000)        0 2023-07-29 13:47:39.060313 nclib-1.0.5/nclib/
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)      464 2023-07-27 20:55:53.000000 nclib-1.0.5/nclib/__init__.py
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)      154 2023-05-26 21:45:16.000000 nclib-1.0.5/nclib/errors.py
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)    10614 2023-05-26 21:45:16.000000 nclib-1.0.5/nclib/logger.py
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)    33759 2023-07-29 13:46:42.000000 nclib-1.0.5/nclib/netcat.py
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)     6506 2023-05-26 21:45:16.000000 nclib-1.0.5/nclib/process.py
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)        0 2023-07-27 20:38:48.000000 nclib-1.0.5/nclib/py.typed
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)     2380 2023-07-29 13:46:29.000000 nclib-1.0.5/nclib/select.py
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)     3389 2023-07-27 20:55:03.000000 nclib-1.0.5/nclib/server.py
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)    11485 2023-05-26 21:45:16.000000 nclib-1.0.5/nclib/simplesock.py
+drwxrwxr-x   0 audrey    (1000) audrey    (1000)        0 2023-07-29 13:47:39.060313 nclib-1.0.5/nclib.egg-info/
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)     1541 2023-07-29 13:47:39.000000 nclib-1.0.5/nclib.egg-info/PKG-INFO
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)      317 2023-07-29 13:47:39.000000 nclib-1.0.5/nclib.egg-info/SOURCES.txt
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)        1 2023-07-29 13:47:39.000000 nclib-1.0.5/nclib.egg-info/dependency_links.txt
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)        6 2023-07-29 13:47:39.000000 nclib-1.0.5/nclib.egg-info/top_level.txt
+-rwxrwxr-x   0 audrey    (1000) audrey    (1000)     1906 2023-05-26 21:45:16.000000 nclib-1.0.5/serve-stdio
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)       38 2023-07-29 13:47:39.060313 nclib-1.0.5/setup.cfg
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)     1841 2023-07-29 13:47:24.000000 nclib-1.0.5/setup.py
```

### Comparing `nclib-1.0.3/LICENSE` & `nclib-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nclib-1.0.3/PKG-INFO` & `nclib-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nclib
-Version: 1.0.3
+Version: 1.0.5
 Summary: Netcat as a library: convienent socket interfaces
 Home-page: https://github.com/rhelmot/nclib
 Author: rhelmot
 Author-email: audrey@rhelmot.io
 License: MIT
 Keywords: netcat nc socket sock file pipe tcp udp recv until logging interact handle listen connect server serve stdio process gdb
 Requires-Python: >=3.5
```

### Comparing `nclib-1.0.3/README.rst` & `nclib-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `nclib-1.0.3/nclib/logger.py` & `nclib-1.0.5/nclib/logger.py`

 * *Files identical despite different names*

### Comparing `nclib-1.0.3/nclib/netcat.py` & `nclib-1.0.5/nclib/netcat.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     if type(b) is str:
         return b.encode()
     elif type(b) is bytes:
         return b
     else:
         raise ValueError("Value must be str or bytes (preferably bytes)")
 
-def _is_ipv6_addr(addr):
+def _is_ipv6_addr(addr) -> bool:
     try:
         socket.inet_pton(socket.AF_INET6, addr)
     except socket.error:
         return False
     else:
         return True
 
@@ -170,15 +170,15 @@
                  loggers=None,
 
                  # canned options
                  verbose=0,
                  log_send=None, log_recv=None, log_yield=False,
                  echo_headers=True, echo_perline=True, echo_hex=False,
                  echo_send_prefix='>> ', echo_recv_prefix='<< ',
-            ):
+            ) -> None:
 
         # handle canned logger options
         if loggers is None:
             loggers = []
         if verbose:
             l = logger.StandardLogger(
                     _xwrap(sys.stderr),
@@ -423,37 +423,37 @@
                         raise errors.NetcatError('Could not connect to %r:' \
                                 % (target,)) from exc
                 else:
                     break
             self.peer = target
         self.logger.connected(self.peer)
 
-    def __enter__(self):
+    def __enter__(self) -> "Netcat":
         return self
 
-    def __exit__(self, ty, val, tb):
+    def __exit__(self, ty, val, tb) -> None:
         self.close()
 
-    def add_logger(self, l):
+    def add_logger(self, l) -> None:
         """
         Add the given logger to the list of current loggers
         """
         self.logger.children.append(l)
 
-    def remove_logger(self, l):
+    def remove_logger(self, l) -> None:
         """
         Remove the given logger from the list of current loggers
         """
         self.logger.children.remove(l)
 
     #
     # Socket metadata functionality
     #
 
-    def close(self):
+    def close(self) -> None:
         """
         Close the socket.
         """
         return self.sock.close()
 
     # inconsistent between sockets and files. support both
     @property
@@ -463,15 +463,15 @@
         """
         return self.sock.closed
 
     @property
     def _closed(self) -> bool:
         return self.closed
 
-    def shutdown(self, how=socket.SHUT_RDWR):
+    def shutdown(self, how=socket.SHUT_RDWR) -> None:
         """
         Send a shutdown signal for one or both of reading and writing. Valid
         arguments are ``socket.SHUT_RDWR``, ``socket.SHUT_RD``, and
         ``socket.SHUT_WR``.
 
         Shutdown differs from closing in that it explicitly changes the state of
         the socket resource to closed, whereas closing will only decrement the
@@ -481,49 +481,49 @@
         still need to call close. (except that this is python and close is
         automatically called on the deletion of the socket)
 
         http://stackoverflow.com/questions/409783/socket-shutdown-vs-socket-close
         """
         return self.sock.shutdown(how)
 
-    def shutdown_rd(self):
+    def shutdown_rd(self) -> None:
         """
         Send a shutdown signal for reading - you may no longer read from this
         socket.
         """
         return self.shutdown(socket.SHUT_RD)
 
-    def shutdown_wr(self):
+    def shutdown_wr(self) -> None:
         """
         Send a shutdown signal for writing - you may no longer write to this
         socket.
         """
         return self.shutdown(socket.SHUT_WR)
 
     def fileno(self) -> int:
         """
         Return the file descriptor associated with this socket
         """
         return self.sock.fileno()
 
-    def settimeout(self, timeout):
+    def settimeout(self, timeout) -> None:
         """
         Set the default timeout in seconds to use for subsequent socket
         operations. Set to None to wait forever, or 0 to be effectively
         nonblocking.
         """
         self._timeout = timeout
 
     def gettimeout(self) -> Optional[float]:
         """
         Retrieve the timeout currently associated with the socket
         """
         return self._timeout
 
-    def flush(self):
+    def flush(self) -> None:
         # no output buffering
         pass
 
     def _prep_select(self):
         return self.sock._prep_select()
 
     #
@@ -702,15 +702,15 @@
         self.logger.requesting_send(s)
 
         out = len(s)
         while s:
             s = s[self._send(s):]
         return out
 
-    def interact(self, insock=sys.stdin, outsock=sys.stdout):
+    def interact(self, insock=sys.stdin, outsock=sys.stdout) -> None:
         """
         Connects the socket to the terminal for user interaction.
         Alternate input and output files may be specified.
 
         This method cannot be used with a timeout.
 
         Aliases: interactive, interaction
@@ -723,27 +723,27 @@
     #
     # Public socket data functionality
     # (implemented with other public socket data functions)
     #
 
     LINE_ENDING = b'\n'
 
-    def recv_line(self, max_size: Optional[int]=None, timeout: DFLOAT = 'default', ending: Optional[BYTESISH]=None):
+    def recv_line(self, max_size: Optional[int]=None, timeout: DFLOAT = 'default', ending: Optional[BYTESISH]=None) -> bytes:
         """
         Recieve until the next newline , default "\\n". The newline string can
         be changed by changing ``nc.LINE_ENDING``. The newline will be returned
         as part of the string.
 
         Aliases: recvline, readline, read_line, readln, recvln
         """
         if ending is None:
             ending = self.LINE_ENDING
         return self.recv_until(ending, max_size, timeout)
 
-    def send_line(self, line: BYTESISH, ending: Optional[BYTESISH]=None):
+    def send_line(self, line: BYTESISH, ending: Optional[BYTESISH]=None) -> int:
         """
         Write the string to the wire, followed by a newline. The newline string
         can be changed by specifying the ``ending`` param or changing
         ``nc.LINE_ENDING``.
 
         Aliases: sendline, writeline, write_line, writeln, sendln
         """
@@ -792,15 +792,15 @@
 
     sendline = send_line
     writeline = send_line
     write_line = send_line
     writeln = send_line
     sendln = send_line
 
-def merge(children, **kwargs):
+def merge(children, **kwargs) -> Netcat:
     """
     Return a Netcat object whose receives will be the merged stream of all the
     given children sockets.
 
     :param children:    A list of socks of any kind to receive from
     :param kwargs:      Any additional keyword arguments will be passed on to
                         the Netcat constructor. Notably, you might want to
@@ -815,15 +815,15 @@
     like simplesock.wrap but will also *unwrap* Netcat objects into their
     constituent sockets. Be warned that this will discard buffers.
     """
     return sock.sock if isinstance(sock, Netcat) else simplesock.wrap(sock)
 
 
 def ferry(left, right, ferry_left=True, ferry_right=True,
-        suppress_timeout=True, suppress_raise_eof=False):
+        suppress_timeout=True, suppress_raise_eof=False) -> None:
     """
     Establish a linkage between two socks, automatically copying any data
     that becomes available between the two.
 
     :param left:                A netcat sock
     :param right:               Another netcat sock
     :param ferry_left:          Whether to copy data leftward, i.e. from the
```

### Comparing `nclib-1.0.3/nclib/process.py` & `nclib-1.0.5/nclib/process.py`

 * *Files identical despite different names*

### Comparing `nclib-1.0.3/nclib/select.py` & `nclib-1.0.5/nclib/select.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,32 @@
+from typing import Tuple, List, TYPE_CHECKING, Iterable, Union, Optional
 import select as _select
 
+if TYPE_CHECKING:
+    from .netcat import Netcat
+
 # hey!!! did you know that you can have nested loops in list/dict/generator comprehensions????
 # GUESS WHAT WE'RE DOING HERE
-def select(select_read, select_write=(), select_exc=(), timeout=None):
+def select(
+        select_read: Iterable["Netcat"],
+        select_write: Optional[Iterable["Netcat"]]=None,
+        select_exc: Optional[Iterable["Netcat"]]=None,
+        timeout: Union[None, int, float]=None
+) -> Tuple[List["Netcat"], List["Netcat"], List["Netcat"]]:
     """
     A select function which works for any netcat or simplesock object.
     This function is a drop-in replacement for python's ``select.select``.
 
     The main advantage is that sockets with multiple backing file descriptors
     are handled cleanly.
     """
+    if select_write is None:
+        select_write = []
+    if select_exc is None:
+        select_exc = []
     allsocks = set(sock for sockset in (select_read, select_write, select_exc) for sock in sockset)
     sock_mapping = {sock: sock._prep_select() for sock in allsocks}
 
     reverse_read = {base: sock for sock, (baselist, _, _) in sock_mapping.items() for base in baselist}
     reverse_write = {base: sock for sock, (_, baselist, _) in sock_mapping.items() for base in baselist}
     reverse_exc = {base: sock for sock, (_, _, baselist) in sock_mapping.items() for base in baselist}
```

### Comparing `nclib-1.0.3/nclib/server.py` & `nclib-1.0.5/nclib/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Tuple
 import socket
 import select
 
 from . import Netcat
 
 class TCPServer:
     """
@@ -18,15 +19,15 @@
 
     >>> from nclib import TCPServer
     >>> server = TCPServer(('0.0.0.0', 1337))
     >>> for client in server:
     ...     client.send(client.recv()) # or submit to a thread pool for async handling...
 
     """
-    def __init__(self, bindto, kernel_backlog=5, **kwargs):
+    def __init__(self, bindto: Tuple[str, int], kernel_backlog: int=5, **kwargs):
         self.addr = bindto
         self.kwargs = kwargs
 
         self.sock = socket.socket(type=socket.SOCK_STREAM)
         self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         self.sock.bind(bindto)
         self.sock.listen(kernel_backlog)
```

### Comparing `nclib-1.0.3/nclib/simplesock.py` & `nclib-1.0.5/nclib/simplesock.py`

 * *Files identical despite different names*

### Comparing `nclib-1.0.3/nclib.egg-info/PKG-INFO` & `nclib-1.0.5/nclib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nclib
-Version: 1.0.3
+Version: 1.0.5
 Summary: Netcat as a library: convienent socket interfaces
 Home-page: https://github.com/rhelmot/nclib
 Author: rhelmot
 Author-email: audrey@rhelmot.io
 License: MIT
 Keywords: netcat nc socket sock file pipe tcp udp recv until logging interact handle listen connect server serve stdio process gdb
 Requires-Python: >=3.5
```

### Comparing `nclib-1.0.3/serve-stdio` & `nclib-1.0.5/serve-stdio`

 * *Files identical despite different names*

### Comparing `nclib-1.0.3/setup.py` & `nclib-1.0.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,19 +29,20 @@
 '''
 
 if bytes is str:
   raise Exception("nclib is python 3 only now :(")
 
 from setuptools import setup
 setup(name='nclib',
-      version='1.0.3',
+      version='1.0.5',
       python_requires='>=3.5',
       packages=['nclib'],
       scripts=['serve-stdio'],
       description='Netcat as a library: convienent socket interfaces',
       long_description=long_description,
       url='https://github.com/rhelmot/nclib',
       author='rhelmot',
       author_email='audrey@rhelmot.io',
       license='MIT',
-      keywords='netcat nc socket sock file pipe tcp udp recv until logging interact handle listen connect server serve stdio process gdb'
+      keywords='netcat nc socket sock file pipe tcp udp recv until logging interact handle listen connect server serve stdio process gdb',
+      package_data={'nclib': ['py.typed']},
       )
```

