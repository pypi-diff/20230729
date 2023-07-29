# Comparing `tmp/pyais-2.5.5.tar.gz` & `tmp/pyais-2.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyais-2.5.5.tar", last modified: Sat Jun 17 13:16:08 2023, max compression
+gzip compressed data, was "dist/pyais-2.5.6.tar", last modified: Sat Jul 29 10:37:55 2023, max compression
```

## Comparing `pyais-2.5.5.tar` & `pyais-2.5.6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:16:08.000000 pyais-2.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)    23826 2023-06-17 13:16:08.000000 pyais-2.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19303 2023-06-17 13:15:57.000000 pyais-2.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:16:08.000000 pyais-2.5.5/pyais/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-17 13:15:57.000000 pyais-2.5.5/pyais/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-17 13:15:57.000000 pyais-2.5.5/pyais/ais_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-06-17 13:15:57.000000 pyais-2.5.5/pyais/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-06-17 13:15:57.000000 pyais-2.5.5/pyais/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-06-17 13:15:57.000000 pyais-2.5.5/pyais/encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-17 13:15:57.000000 pyais-2.5.5/pyais/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-06-17 13:15:57.000000 pyais-2.5.5/pyais/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    64765 2023-06-17 13:15:57.000000 pyais-2.5.5/pyais/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 13:15:57.000000 pyais-2.5.5/pyais/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-06-17 13:15:57.000000 pyais-2.5.5/pyais/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-06-17 13:15:57.000000 pyais-2.5.5/pyais/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-06-17 13:15:57.000000 pyais-2.5.5/pyais/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:16:08.000000 pyais-2.5.5/pyais.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23826 2023-06-17 13:16:08.000000 pyais-2.5.5/pyais.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-17 13:16:08.000000 pyais-2.5.5/pyais.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 13:16:08.000000 pyais-2.5.5/pyais.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-17 13:16:08.000000 pyais-2.5.5/pyais.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-17 13:16:08.000000 pyais-2.5.5/pyais.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-17 13:16:08.000000 pyais-2.5.5/pyais.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 13:16:08.000000 pyais-2.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-17 13:15:57.000000 pyais-2.5.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:16:08.000000 pyais-2.5.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/mock_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/mock_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    58995 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/test_decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/test_decode_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    32404 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/test_encode.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/test_file_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/test_generic_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/test_nmea.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/test_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/test_tag_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/test_talker_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/test_tcp_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/test_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/test_udp_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:16:08.000000 pyais-2.5.5/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/utils/generate_msg_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/utils/skip.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/utils/timeout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:37:55.000000 pyais-2.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    23840 2023-07-29 10:37:55.000000 pyais-2.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19317 2023-07-29 10:37:43.000000 pyais-2.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:37:55.000000 pyais-2.5.6/pyais/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-29 10:37:43.000000 pyais-2.5.6/pyais/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-29 10:37:43.000000 pyais-2.5.6/pyais/ais_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-07-29 10:37:43.000000 pyais-2.5.6/pyais/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-07-29 10:37:43.000000 pyais-2.5.6/pyais/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-07-29 10:37:43.000000 pyais-2.5.6/pyais/encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-29 10:37:43.000000 pyais-2.5.6/pyais/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-07-29 10:37:43.000000 pyais-2.5.6/pyais/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64765 2023-07-29 10:37:43.000000 pyais-2.5.6/pyais/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:37:43.000000 pyais-2.5.6/pyais/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-07-29 10:37:43.000000 pyais-2.5.6/pyais/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-07-29 10:37:43.000000 pyais-2.5.6/pyais/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-07-29 10:37:43.000000 pyais-2.5.6/pyais/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:37:55.000000 pyais-2.5.6/pyais.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23840 2023-07-29 10:37:54.000000 pyais-2.5.6/pyais.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-29 10:37:55.000000 pyais-2.5.6/pyais.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:37:54.000000 pyais-2.5.6/pyais.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-29 10:37:54.000000 pyais-2.5.6/pyais.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-29 10:37:54.000000 pyais-2.5.6/pyais.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-29 10:37:54.000000 pyais-2.5.6/pyais.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:37:55.000000 pyais-2.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-29 10:37:43.000000 pyais-2.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:37:55.000000 pyais-2.5.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-29 10:37:43.000000 pyais-2.5.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-29 10:37:43.000000 pyais-2.5.6/tests/mock_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-29 10:37:43.000000 pyais-2.5.6/tests/mock_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-29 10:37:43.000000 pyais-2.5.6/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58995 2023-07-29 10:37:43.000000 pyais-2.5.6/tests/test_decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-29 10:37:43.000000 pyais-2.5.6/tests/test_decode_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32404 2023-07-29 10:37:43.000000 pyais-2.5.6/tests/test_encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-29 10:37:43.000000 pyais-2.5.6/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-07-29 10:37:43.000000 pyais-2.5.6/tests/test_file_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-29 10:37:43.000000 pyais-2.5.6/tests/test_generic_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-07-29 10:37:43.000000 pyais-2.5.6/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-07-29 10:37:43.000000 pyais-2.5.6/tests/test_nmea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-29 10:37:43.000000 pyais-2.5.6/tests/test_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-07-29 10:37:43.000000 pyais-2.5.6/tests/test_tag_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-29 10:37:43.000000 pyais-2.5.6/tests/test_talker_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-29 10:37:43.000000 pyais-2.5.6/tests/test_tcp_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-07-29 10:37:43.000000 pyais-2.5.6/tests/test_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-29 10:37:43.000000 pyais-2.5.6/tests/test_udp_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:37:55.000000 pyais-2.5.6/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:37:43.000000 pyais-2.5.6/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-29 10:37:43.000000 pyais-2.5.6/tests/utils/generate_msg_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-29 10:37:43.000000 pyais-2.5.6/tests/utils/skip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-29 10:37:43.000000 pyais-2.5.6/tests/utils/timeout.py
```

### Comparing `pyais-2.5.5/PKG-INFO` & `pyais-2.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyais
-Version: 2.5.5
+Version: 2.5.6
 Summary: Ais message decoding
 Home-page: https://github.com/M0r13n/pyais
 Author: Leon Morten Richter
 Author-email: leon.morten@gmail.com
 License: MIT
 Description: # pyais
         
@@ -12,15 +12,15 @@
         [![license](https://img.shields.io/pypi/l/pyais)](https://github.com/M0r13n/pyais/blob/master/LICENSE)
         [![codecov](https://codecov.io/gh/M0r13n/pyais/branch/master/graph/badge.svg)](https://codecov.io/gh/M0r13n/pyais)
         [![downloads](https://img.shields.io/pypi/dm/pyais)](https://pypi.org/project/pyais/)
         ![CI](https://github.com/M0r13n/pyais/workflows/CI/badge.svg)
         [![Documentation Status](https://readthedocs.org/projects/pyais/badge/?version=latest)](https://pyais.readthedocs.io/en/latest/?badge=latest)
         
         AIS message encoding and decoding. 100% pure Python. Supports AIVDM/AIVDO messages. Supports single messages, files and
-        TCP/UDP sockets. This library has been used and tested extensively in representative real-world scenarios. This includes tests with live feeds from [Spire](https://spire.com/maritime/), the [Norwegian Coastal Administration](https://kystverket.no/navigasjonstjenester/ais/tilgang-pa-ais-data/) and others. I test each major release against a selection of public and non-public data sources to ensure the broadest possible compatibility.
+        TCP/UDP sockets. This library has been used and tested extensively in representative real-world scenarios. This includes tests with live feeds from [Spire](https://spire.com/maritime/), the [Norwegian Coastal Administration](https://kystverket.no/en/navigation-and-monitoring/ais/access-to-ais-data/) and others. I test each major release against a selection of public and non-public data sources to ensure the broadest possible compatibility.
         
         You can find the full documentation on [readthedocs](https://pyais.readthedocs.io/en/latest/).
         
         I also wrote a [blog post about AIS decoding](https://leonrichter.de/posts/pyais/) and this lib.
         
         # Acknowledgements
         
@@ -133,15 +133,15 @@
         ]
         for msg in IterMessages(fake_stream):
             print(msg.decode())
         ```
         
         ## Live feed
         
-        The [Norwegian Coastal Administration](https://kystverket.no/navigasjonstjenester/ais/tilgang-pa-ais-data/) offers real-time AIS data.
+        The [Norwegian Coastal Administration](https://kystverket.no/en/navigation-and-monitoring/ais/access-to-ais-data/) offers real-time AIS data.
         This live feed can be accessed via TCP/IP without prior registration.
         The AIS data is freely available under the [norwegian license for public data](https://data.norge.no/nlod/no/1.0):
         
         Data can be read from a TCP/IP socket and is encoded according to IEC 62320-1:
         
         - IP:   153.44.253.27
         - Port: 5631
```

### Comparing `pyais-2.5.5/README.md` & `pyais-2.5.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![license](https://img.shields.io/pypi/l/pyais)](https://github.com/M0r13n/pyais/blob/master/LICENSE)
 [![codecov](https://codecov.io/gh/M0r13n/pyais/branch/master/graph/badge.svg)](https://codecov.io/gh/M0r13n/pyais)
 [![downloads](https://img.shields.io/pypi/dm/pyais)](https://pypi.org/project/pyais/)
 ![CI](https://github.com/M0r13n/pyais/workflows/CI/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/pyais/badge/?version=latest)](https://pyais.readthedocs.io/en/latest/?badge=latest)
 
 AIS message encoding and decoding. 100% pure Python. Supports AIVDM/AIVDO messages. Supports single messages, files and
-TCP/UDP sockets. This library has been used and tested extensively in representative real-world scenarios. This includes tests with live feeds from [Spire](https://spire.com/maritime/), the [Norwegian Coastal Administration](https://kystverket.no/navigasjonstjenester/ais/tilgang-pa-ais-data/) and others. I test each major release against a selection of public and non-public data sources to ensure the broadest possible compatibility.
+TCP/UDP sockets. This library has been used and tested extensively in representative real-world scenarios. This includes tests with live feeds from [Spire](https://spire.com/maritime/), the [Norwegian Coastal Administration](https://kystverket.no/en/navigation-and-monitoring/ais/access-to-ais-data/) and others. I test each major release against a selection of public and non-public data sources to ensure the broadest possible compatibility.
 
 You can find the full documentation on [readthedocs](https://pyais.readthedocs.io/en/latest/).
 
 I also wrote a [blog post about AIS decoding](https://leonrichter.de/posts/pyais/) and this lib.
 
 # Acknowledgements
 
@@ -125,15 +125,15 @@
 ]
 for msg in IterMessages(fake_stream):
     print(msg.decode())
 ```
 
 ## Live feed
 
-The [Norwegian Coastal Administration](https://kystverket.no/navigasjonstjenester/ais/tilgang-pa-ais-data/) offers real-time AIS data.
+The [Norwegian Coastal Administration](https://kystverket.no/en/navigation-and-monitoring/ais/access-to-ais-data/) offers real-time AIS data.
 This live feed can be accessed via TCP/IP without prior registration.
 The AIS data is freely available under the [norwegian license for public data](https://data.norge.no/nlod/no/1.0):
 
 Data can be read from a TCP/IP socket and is encoded according to IEC 62320-1:
 
 - IP:   153.44.253.27
 - Port: 5631
```

### Comparing `pyais-2.5.5/pyais/__init__.py` & `pyais-2.5.6/pyais/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pyais.messages import NMEAMessage, ANY_MESSAGE, AISSentence
 from pyais.stream import TCPConnection, FileReaderStream, IterMessages
 from pyais.encode import encode_dict, encode_msg, ais_to_nmea_0183
 from pyais.decode import decode
 from pyais.tracker import AISTracker, AISTrack
 
 __license__ = 'MIT'
-__version__ = '2.5.5'
+__version__ = '2.5.6'
 __author__ = 'Leon Morten Richter'
 
 __all__ = (
     'encode_dict',
     'encode_msg',
     'ais_to_nmea_0183',
     'NMEAMessage',
```

### Comparing `pyais-2.5.5/pyais/ais_types.py` & `pyais-2.5.6/pyais/ais_types.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.5/pyais/constants.py` & `pyais-2.5.6/pyais/constants.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.5/pyais/decode.py` & `pyais-2.5.6/pyais/decode.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.5/pyais/encode.py` & `pyais-2.5.6/pyais/encode.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.5/pyais/exceptions.py` & `pyais-2.5.6/pyais/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.5/pyais/main.py` & `pyais-2.5.6/pyais/main.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.5/pyais/messages.py` & `pyais-2.5.6/pyais/messages.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.5/pyais/stream.py` & `pyais-2.5.6/pyais/stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
 class BinaryIOStream(Stream[BinaryIO]):
     """Read messages from a file-like object"""
 
     def __init__(self, file: BinaryIO) -> None:
         super().__init__(file)
 
     def read(self) -> Generator[bytes, None, None]:
-        yield from self._fobj.readlines()
+        yield from self._fobj
 
 
 class FileReaderStream(BinaryIOStream):
     """
     Read NMEA messages from file
     """
```

### Comparing `pyais-2.5.5/pyais/tracker.py` & `pyais-2.5.6/pyais/tracker.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.5/pyais/util.py` & `pyais-2.5.6/pyais/util.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.5/pyais.egg-info/PKG-INFO` & `pyais-2.5.6/pyais.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyais
-Version: 2.5.5
+Version: 2.5.6
 Summary: Ais message decoding
 Home-page: https://github.com/M0r13n/pyais
 Author: Leon Morten Richter
 Author-email: leon.morten@gmail.com
 License: MIT
 Description: # pyais
         
@@ -12,15 +12,15 @@
         [![license](https://img.shields.io/pypi/l/pyais)](https://github.com/M0r13n/pyais/blob/master/LICENSE)
         [![codecov](https://codecov.io/gh/M0r13n/pyais/branch/master/graph/badge.svg)](https://codecov.io/gh/M0r13n/pyais)
         [![downloads](https://img.shields.io/pypi/dm/pyais)](https://pypi.org/project/pyais/)
         ![CI](https://github.com/M0r13n/pyais/workflows/CI/badge.svg)
         [![Documentation Status](https://readthedocs.org/projects/pyais/badge/?version=latest)](https://pyais.readthedocs.io/en/latest/?badge=latest)
         
         AIS message encoding and decoding. 100% pure Python. Supports AIVDM/AIVDO messages. Supports single messages, files and
-        TCP/UDP sockets. This library has been used and tested extensively in representative real-world scenarios. This includes tests with live feeds from [Spire](https://spire.com/maritime/), the [Norwegian Coastal Administration](https://kystverket.no/navigasjonstjenester/ais/tilgang-pa-ais-data/) and others. I test each major release against a selection of public and non-public data sources to ensure the broadest possible compatibility.
+        TCP/UDP sockets. This library has been used and tested extensively in representative real-world scenarios. This includes tests with live feeds from [Spire](https://spire.com/maritime/), the [Norwegian Coastal Administration](https://kystverket.no/en/navigation-and-monitoring/ais/access-to-ais-data/) and others. I test each major release against a selection of public and non-public data sources to ensure the broadest possible compatibility.
         
         You can find the full documentation on [readthedocs](https://pyais.readthedocs.io/en/latest/).
         
         I also wrote a [blog post about AIS decoding](https://leonrichter.de/posts/pyais/) and this lib.
         
         # Acknowledgements
         
@@ -133,15 +133,15 @@
         ]
         for msg in IterMessages(fake_stream):
             print(msg.decode())
         ```
         
         ## Live feed
         
-        The [Norwegian Coastal Administration](https://kystverket.no/navigasjonstjenester/ais/tilgang-pa-ais-data/) offers real-time AIS data.
+        The [Norwegian Coastal Administration](https://kystverket.no/en/navigation-and-monitoring/ais/access-to-ais-data/) offers real-time AIS data.
         This live feed can be accessed via TCP/IP without prior registration.
         The AIS data is freely available under the [norwegian license for public data](https://data.norge.no/nlod/no/1.0):
         
         Data can be read from a TCP/IP socket and is encoded according to IEC 62320-1:
         
         - IP:   153.44.253.27
         - Port: 5631
```

### Comparing `pyais-2.5.5/pyais.egg-info/SOURCES.txt` & `pyais-2.5.6/pyais.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyais-2.5.5/setup.py` & `pyais-2.5.6/setup.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.5/tests/mock_sender.py` & `pyais-2.5.6/tests/mock_sender.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.5/tests/mock_server.py` & `pyais-2.5.6/tests/mock_server.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.5/tests/test_constants.py` & `pyais-2.5.6/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.5/tests/test_decode.py` & `pyais-2.5.6/tests/test_decode.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.5/tests/test_decode_raw.py` & `pyais-2.5.6/tests/test_decode_raw.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.5/tests/test_encode.py` & `pyais-2.5.6/tests/test_encode.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.5/tests/test_examples.py` & `pyais-2.5.6/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.5/tests/test_file_stream.py` & `pyais-2.5.6/tests/test_file_stream.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.5/tests/test_generic_stream.py` & `pyais-2.5.6/tests/test_generic_stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,24 +18,19 @@
         """
         Read a single line of a file. Empty string if file is empty.
         """
         if not len(self.buffer):
             return b""
         return self.buffer.pop(0)
 
-    def readlines(self) -> List[bytes]:
-        """
-        Read until EOF using readline() and return a list containing the lines thus read.
-        """
-        buf = []
+    def __iter__(self) -> List[bytes]:
         line = self.readline()
         while line:
-            buf.append(line)
+            yield line
             line = self.readline()
-        return buf
 
 
 class TestGenericStream(unittest.TestCase):
 
     def test_empty_stream(self):
         """
         If the stream does not contain any data, nothing should happen.
```

### Comparing `pyais-2.5.5/tests/test_main.py` & `pyais-2.5.6/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.5/tests/test_nmea.py` & `pyais-2.5.6/tests/test_nmea.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.5/tests/test_socket.py` & `pyais-2.5.6/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.5/tests/test_tag_block.py` & `pyais-2.5.6/tests/test_tag_block.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.5/tests/test_talker_ids.py` & `pyais-2.5.6/tests/test_talker_ids.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.5/tests/test_tcp_stream.py` & `pyais-2.5.6/tests/test_tcp_stream.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.5/tests/test_tracker.py` & `pyais-2.5.6/tests/test_tracker.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.5/tests/test_udp_stream.py` & `pyais-2.5.6/tests/test_udp_stream.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.5/tests/utils/generate_msg_interface.py` & `pyais-2.5.6/tests/utils/generate_msg_interface.py`

 * *Files identical despite different names*

