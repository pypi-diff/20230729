# Comparing `tmp/ydl-ipc-0.1.0.tar.gz` & `tmp/ydl_ipc-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ydl-ipc-0.1.0.tar", last modified: Sat Oct 29 20:56:22 2022, max compression
+gzip compressed data, was "ydl_ipc-0.2.0.tar", max compression
```

## Comparing `ydl-ipc-0.1.0.tar` & `ydl_ipc-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,8 @@
-drwxr-xr-x   0 qiwen      (501) staff       (20)        0 2022-10-29 20:56:22.984730 ydl-ipc-0.1.0/
--rw-r--r--   0 qiwen      (501) staff       (20)     1080 2022-09-24 20:30:02.000000 ydl-ipc-0.1.0/LICENSE
--rw-r--r--   0 qiwen      (501) staff       (20)      367 2022-10-29 20:56:22.984561 ydl-ipc-0.1.0/PKG-INFO
--rw-r--r--   0 qiwen      (501) staff       (20)      369 2022-09-24 20:30:02.000000 ydl-ipc-0.1.0/README.md
--rw-r--r--   0 qiwen      (501) staff       (20)       38 2022-10-29 20:56:22.984792 ydl-ipc-0.1.0/setup.cfg
--rw-r--r--   0 qiwen      (501) staff       (20)      522 2022-09-24 20:30:02.000000 ydl-ipc-0.1.0/setup.py
-drwxr-xr-x   0 qiwen      (501) staff       (20)        0 2022-10-29 20:56:22.983457 ydl-ipc-0.1.0/ydl/
--rw-r--r--   0 qiwen      (501) staff       (20)      525 2022-09-24 20:30:02.000000 ydl-ipc-0.1.0/ydl/__init__.py
--rw-r--r--   0 qiwen      (501) staff       (20)      960 2022-09-24 20:30:02.000000 ydl-ipc-0.1.0/ydl/__main__.py
--rw-r--r--   0 qiwen      (501) staff       (20)     7996 2022-09-24 20:30:02.000000 ydl-ipc-0.1.0/ydl/_core.py
--rw-r--r--   0 qiwen      (501) staff       (20)     4430 2022-09-24 20:30:02.000000 ydl-ipc-0.1.0/ydl/_header.py
-drwxr-xr-x   0 qiwen      (501) staff       (20)        0 2022-10-29 20:56:22.984260 ydl-ipc-0.1.0/ydl_ipc.egg-info/
--rw-r--r--   0 qiwen      (501) staff       (20)      367 2022-10-29 20:56:22.000000 ydl-ipc-0.1.0/ydl_ipc.egg-info/PKG-INFO
--rw-r--r--   0 qiwen      (501) staff       (20)      240 2022-10-29 20:56:22.000000 ydl-ipc-0.1.0/ydl_ipc.egg-info/SOURCES.txt
--rw-r--r--   0 qiwen      (501) staff       (20)        1 2022-10-29 20:56:22.000000 ydl-ipc-0.1.0/ydl_ipc.egg-info/dependency_links.txt
--rw-r--r--   0 qiwen      (501) staff       (20)       10 2022-10-29 20:56:22.000000 ydl-ipc-0.1.0/ydl_ipc.egg-info/requires.txt
--rw-r--r--   0 qiwen      (501) staff       (20)        4 2022-10-29 20:56:22.000000 ydl-ipc-0.1.0/ydl_ipc.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1080 2023-07-29 11:02:40.527595 ydl_ipc-0.2.0/LICENSE
+-rw-r--r--   0        0        0      307 2023-07-29 11:02:40.527595 ydl_ipc-0.2.0/README.md
+-rw-r--r--   0        0        0      477 2023-07-29 11:02:40.527595 ydl_ipc-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      518 2023-07-29 11:02:40.527595 ydl_ipc-0.2.0/ydl/__init__.py
+-rw-r--r--   0        0        0      998 2023-07-29 11:02:40.527595 ydl_ipc-0.2.0/ydl/__main__.py
+-rw-r--r--   0        0        0     7929 2023-07-29 11:02:40.527595 ydl_ipc-0.2.0/ydl/_core.py
+-rw-r--r--   0        0        0     2937 2023-07-29 11:02:40.527595 ydl_ipc-0.2.0/ydl/_header.py
+-rw-r--r--   0        0        0     1178 1970-01-01 00:00:00.000000 ydl_ipc-0.2.0/PKG-INFO
```

### Comparing `ydl-ipc-0.1.0/LICENSE` & `ydl_ipc-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ydl-ipc-0.1.0/ydl/__main__.py` & `ydl_ipc-0.2.0/ydl/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Run a YDL server, which clients can use to communicate.
 """
 
 import argparse
 import signal
 import sys
-from ._core import run_ydl_server
+from ._core import run_server, DEFAULT_HOST, DEFAULT_PORT
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(prog='python3 -m ydl', description=__doc__)
     parser.add_argument("-s", "--silent", action='store_true',
         help="do not print client connections")
-    parser.add_argument("-a", "--address", default=None, type=str,
-        help="run server on specified ip address, such as 0.0.0.0")
-    parser.add_argument("-p", "--port", default=None, type=int,
+    parser.add_argument("-a", "--address", default=DEFAULT_HOST, type=str,
+        help="run server on specified host address, such as 0.0.0.0")
+    parser.add_argument("-p", "--port", default=DEFAULT_PORT, type=int,
         help="run server on specified port")
 
     args = parser.parse_args()
     verbose = not args.silent
     def sigint_handler(_signum, _frame):
         '''gracefully shuts down server on sigint (ctrl-c)'''
         if verbose:
             print("\nShutting down YDL server")
         sys.exit(0)
 
     signal.signal(signal.SIGINT, sigint_handler)
-    run_ydl_server(args.address, args.port, verbose)
+    run_server(args.address, args.port, verbose)
```

### Comparing `ydl-ipc-0.1.0/ydl/_core.py` & `ydl_ipc-0.2.0/ydl/_core.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,40 +7,41 @@
 
 
 
 # Default address for the YDL server. Also used as default arg for client.
 # A network of clients should communicate through one server on a designated address.
 # if all clients are on one computer, 127.0.0.1 works; if distributed across a local
 # network, use 0.0.0.0 instead.
-DEFAULT_YDL_ADDR = ('127.0.0.1', 5001) # doesn't need to be available on network
+DEFAULT_HOST = '127.0.0.1' # doesn't need to be available on network
+DEFAULT_PORT = 5001
 
-
-class YDLClient():
+class Client():
     '''
     A client to the YDL network. Listens to a set of channels, and may send messages to
     any channel. Will automatically try to connect to YDL network.
     '''
-    def __init__(self, *receive_channels: str, socket_address: Tuple[str, int] = DEFAULT_YDL_ADDR):
+    def __init__(self, *receive_channels: str, host: str = DEFAULT_HOST, port: int = DEFAULT_PORT):
         '''
         Waits for connection to open, then subscribes to given receive_channels
         '''
         self._receive_channels = receive_channels
-        self._socket_address = socket_address
+        self._socket_address = (host, port)
         self._lock = threading.Lock() # protects all local variables
         self._conn = None    # set in _new_connection()
         self._selobj = None  # set in _new_connection()
         with self._lock:
             self._new_connection()
 
     def send(self, message: Tuple):
         '''
-        The input message is a tuple of (target_channel, stuff...)
-        target_channel: str, which channel you want to send to
-        stuff: any other stuff you want to send. Must be json serializable.
-        May block if disconnected and waiting for a new connection.
+        The input message is a tuple of `(target_channel, stuff...)`.
+        `target_channel` is a string which identifies the channel you want to
+        send to. `stuff` can be any other stuff you want to send. `stuff` must
+        be json serializable. This method may block if disconnected and 
+        waiting for a new connection.
         '''
         target_channel = message[0]
         json_str = json.dumps(message[1:])
         while True:
             try:
                 send_message(self._conn, target_channel, json_str)
                 break
@@ -177,30 +178,25 @@
                 # an empty string is a special message that means "subscribe to channel"
                 subscriptions[target_channel].append(conn)
             else:
                 # forward message to correct subscribers
                 for chan in subscriptions[target_channel]:
                     send_message(chan, target_channel, message)
 
-def run_ydl_server(address=None, port=None, verbose=False):
+def run_server(host: str = DEFAULT_HOST, port: int = DEFAULT_PORT, verbose: bool = False):
     '''
-    (server method - internal use only)
     Runs the YDL server that processes will use
     to communicate with each other
     '''
-    if address is None:
-        address = DEFAULT_YDL_ADDR[0]
-    if port is None:
-        port = DEFAULT_YDL_ADDR[1]
     if verbose:
-        print("Starting YDL server at address:", (address, port))
+        print("Starting YDL server at address:", (host, port))
     subscriptions = {} # a mapping of target names -> list of socket objects
     sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-    sock.bind((address, port))
+    sock.bind((host, port))
     sock.listen()
     sock.setblocking(False)
     sel = selectors.DefaultSelector()
     sel.register(sock, selectors.EVENT_READ, None)
     while True:
         events = sel.select(timeout=1) #Windows is bad and needs a timeout here.
         for key, _mask in events:
```

