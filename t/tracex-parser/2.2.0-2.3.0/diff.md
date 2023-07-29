# Comparing `tmp/tracex_parser-2.2.0.tar.gz` & `tmp/tracex_parser-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracex_parser-2.2.0.tar", max compression
+gzip compressed data, was "tracex_parser-2.3.0.tar", max compression
```

## Comparing `tracex_parser-2.2.0.tar` & `tracex_parser-2.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3266 2023-05-20 16:53:41.535213 tracex_parser-2.2.0/README.md
--rw-r--r--   0        0        0    32000 2023-05-20 16:53:41.535213 tracex_parser-2.2.0/demo_filex.trx
--rw-r--r--   0        0        0    32000 2023-05-20 16:53:41.535213 tracex_parser-2.2.0/demo_netx_tcp.trx
--rw-r--r--   0        0        0    32000 2023-05-20 16:53:41.535213 tracex_parser-2.2.0/demo_netx_udp.trx
--rw-r--r--   0        0        0    32768 2023-05-20 16:53:41.535213 tracex_parser-2.2.0/demo_threadx.trx
--rw-r--r--   0        0        0      889 2023-05-20 16:53:41.535213 tracex_parser-2.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-20 16:53:41.535213 tracex_parser-2.2.0/tracex_parser/__init__.py
--rw-r--r--   0        0        0    12117 2023-05-20 16:53:41.535213 tracex_parser-2.2.0/tracex_parser/events.py
--rwxr-xr-x   0        0        0     9640 2023-05-20 16:53:41.535213 tracex_parser-2.2.0/tracex_parser/file_parser.py
--rw-r--r--   0        0        0     2132 2023-05-20 16:53:41.535213 tracex_parser-2.2.0/tracex_parser/helpers.py
--rw-r--r--   0        0        0     3887 2023-05-20 16:53:53.340665 tracex_parser-2.2.0/setup.py
--rw-r--r--   0        0        0     4114 2023-05-20 16:53:53.341123 tracex_parser-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3266 2023-07-29 18:44:43.490208 tracex_parser-2.3.0/README.md
+-rw-r--r--   0        0        0    32000 2023-07-29 18:44:43.490208 tracex_parser-2.3.0/demo_filex.trx
+-rw-r--r--   0        0        0    32000 2023-07-29 18:44:43.490208 tracex_parser-2.3.0/demo_netx_tcp.trx
+-rw-r--r--   0        0        0    32000 2023-07-29 18:44:43.494208 tracex_parser-2.3.0/demo_netx_udp.trx
+-rw-r--r--   0        0        0    32768 2023-07-29 18:44:43.494208 tracex_parser-2.3.0/demo_threadx.trx
+-rw-r--r--   0        0        0      889 2023-07-29 18:44:43.494208 tracex_parser-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-29 18:44:43.494208 tracex_parser-2.3.0/tracex_parser/__init__.py
+-rw-r--r--   0        0        0    12246 2023-07-29 18:44:43.494208 tracex_parser-2.3.0/tracex_parser/events.py
+-rwxr-xr-x   0        0        0    10319 2023-07-29 18:44:43.494208 tracex_parser-2.3.0/tracex_parser/file_parser.py
+-rw-r--r--   0        0        0     2142 2023-07-29 18:44:43.494208 tracex_parser-2.3.0/tracex_parser/helpers.py
+-rw-r--r--   0        0        0     3887 2023-07-29 18:44:56.997723 tracex_parser-2.3.0/setup.py
+-rw-r--r--   0        0        0     4114 2023-07-29 18:44:56.998205 tracex_parser-2.3.0/PKG-INFO
```

### Comparing `tracex_parser-2.2.0/README.md` & `tracex_parser-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `tracex_parser-2.2.0/demo_filex.trx` & `tracex_parser-2.3.0/demo_filex.trx`

 * *Files identical despite different names*

### Comparing `tracex_parser-2.2.0/demo_netx_tcp.trx` & `tracex_parser-2.3.0/demo_netx_tcp.trx`

 * *Files identical despite different names*

### Comparing `tracex_parser-2.2.0/demo_netx_udp.trx` & `tracex_parser-2.3.0/demo_netx_udp.trx`

 * *Files identical despite different names*

### Comparing `tracex_parser-2.2.0/demo_threadx.trx` & `tracex_parser-2.3.0/demo_threadx.trx`

 * *Files identical despite different names*

### Comparing `tracex_parser-2.2.0/pyproject.toml` & `tracex_parser-2.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "tracex_parser"
-version = "2.2.0"
+version = "2.3.0"
 description = "Parser for ThreadX RTOS's trace buffers (aka TraceX)"
 authors = ["Julianne Swinoga <julianneswinoga@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 include = [
     '*.trx',
 ]
```

### Comparing `tracex_parser-2.2.0/tracex_parser/events.py` & `tracex_parser-2.3.0/tracex_parser/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import *
+from typing import Optional, Dict, List, Union, Any, ClassVar
 
 from .helpers import TraceXEventException, CStruct, TextColour
 
 
 class CommonArg:
     """
     Holds string mappings for common arguments so that we can
@@ -89,17 +89,19 @@
                 obj_reg_name = self._map_ptr_to_obj_reg_name(obj_reg_map, self.mapped_args[arg_to_map])
                 if obj_reg_name is not None:
                     self.mapped_args[arg_to_map] = obj_reg_name
                 else:
                     print(f'Failed to map {arg_to_map} in {self.__class__.__name__}:{self.mapped_args}')
 
         # Make the thread names nicer
+        # @see https://docs.microsoft.com/en-us/azure/rtos/tracex/chapter11#thread-pointer
         if self.thread_ptr == 0xFFFFFFFF:
-            # @see https://docs.microsoft.com/en-us/azure/rtos/tracex/chapter11#thread-pointer
             self.thread_name = 'INTERRUPT'
+        elif self.thread_ptr == 0xF0F0F0F0:
+            self.thread_name = 'INITIALIZATION'
         else:
             # Try to find time slice thread_ptr in the registry
             obj_reg_name = self._map_ptr_to_obj_reg_name(obj_reg_map, self.thread_ptr)
             if obj_reg_name is not None:
                 self.thread_name = obj_reg_name
             else:
                 print(f'Failed to map thread_ptr in {self.__class__.__name__}:{self.mapped_args}')
```

### Comparing `tracex_parser-2.2.0/tracex_parser/file_parser.py` & `tracex_parser-2.3.0/tracex_parser/file_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/python3
 
 import struct
 import argparse
 import copy
 import sys
-from typing import *
+from typing import Tuple, Optional, Dict, List
+from collections import deque
 
 from .helpers import TraceXParseException, CStruct, TextColour
 from .events import TraceXEvent, convert_events
 
 parser = argparse.ArgumentParser(description="""
 TraceX parser module, intended as a library but can be used as a standalone script""")
 parser.add_argument('input_trxs', nargs='+', action='store',
@@ -109,15 +110,15 @@
 
 
 def get_event_entries(endian_str: str, buf: bytes, start_idx: int, control_header: CStruct) \
         -> Tuple[List[CStruct], int]:
     """
     @see https://docs.microsoft.com/en-us/azure/rtos/tracex/chapter11#event-trace-entries
     Unpacks the TraceX events into a list of dict-like CStructs.
-    Events are sorted by their timestamp.
+    Events are sorted by their place in the buffer.
     """
     event_entry = CStruct(endian_str, [
         ('L', 'thread_ptr'),
         ('L', 'thread_priority'),
         ('L', 'event_id'),
         ('L', 'time_stamp'),
         ('L', 'info_field_1'),
@@ -135,19 +136,29 @@
 
     event_entry_start_idx = start_idx
     raw_events = []
     for event_idx in range(num_entries):
         event_entry.clear()
         object_entry_end_idx = event_entry_start_idx + event_size
         event_entry.unpack(buf[event_entry_start_idx:object_entry_end_idx])
+
+        # Apply the timer valid mask to the timestamp
+        event_entry['time_stamp'] = control_header['timer_valid_mask'] & event_entry['time_stamp']
+
         if event_entry['event_id'] != 0:
             raw_events.append(copy.deepcopy(event_entry))
         event_entry_start_idx += event_size
-    raw_events.sort(key=lambda t: t['time_stamp'])
-    return raw_events, event_entry_start_idx
+
+    # Even though we have a timestamp, events are ordered in the way they were placed in the buffer
+    oldest_event_idx = (control_header['buf_end_ptr'] - control_header['buf_cur_ptr']) // event_size
+    raw_events_deque = deque(raw_events)
+    raw_events_deque.rotate(oldest_event_idx)
+    raw_events_sorted = list(raw_events_deque)
+
+    return raw_events_sorted, event_entry_start_idx
 
 
 def parse_tracex_buffer(filepath: str, custom_events_map: Optional[Dict[int, TraceXEvent]] = None) \
         -> Tuple[List[TraceXEvent], Dict[int, CStruct]]:
     """
     Parse a TraceX binary dump (canonically .trx) into a list of TraceXEvent classes
     :param filepath: Path to where the TraceX file is
@@ -185,22 +196,24 @@
         total_ticks = tracex_events[-1].timestamp - tracex_events[0].timestamp
         print(f'{colour.wte}delta ticks: {total_ticks}{colour.rst}')
 
         if args.verbose > 0:
             print(f'{colour.grn}Event Histogram:{colour.rst}')
             events_histogram = {}
             for tracex_event in tracex_events:
-                event_id = tracex_event.fn_name if tracex_event.fn_name else tracex_event.id
+                event_id = tracex_event.fn_name if tracex_event.fn_name else str(tracex_event.id)
                 if event_id in events_histogram:
                     events_histogram[event_id] += 1
                 else:
                     events_histogram[event_id] = 1
-            for event_id in sorted(events_histogram, key=lambda k: events_histogram[k], reverse=True):
+            sorted_event_names = sorted(events_histogram.keys(), key=lambda k: events_histogram[k], reverse=True)
+            max_event_name_len = max(len(e_id) for e_id in sorted_event_names)
+            for event_id in sorted_event_names:
                 event_colour = colour.blu if isinstance(event_id, str) else colour.yel
-                print(f'{event_colour}{event_id:<20}{events_histogram[event_id]}{colour.rst}')
+                print(f'{event_colour}{event_id:<{max_event_name_len + 1}}{events_histogram[event_id]}{colour.rst}')
 
         if args.verbose > 1:
             print(f'{colour.grn}All events:{colour.rst}')
             for tracex_event in tracex_events:
                 print(tracex_event.as_str(colour))
```

### Comparing `tracex_parser-2.2.0/tracex_parser/helpers.py` & `tracex_parser-2.3.0/tracex_parser/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import struct
-from typing import *
+from typing import Tuple, List
 
 
 class TraceXBaseException(Exception):
     pass
 
 
 class TraceXParseException(TraceXBaseException):
```

### Comparing `tracex_parser-2.2.0/setup.py` & `tracex_parser-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['tracex_parser']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'tracex-parser',
-    'version': '2.2.0',
+    'version': '2.3.0',
     'description': "Parser for ThreadX RTOS's trace buffers (aka TraceX)",
     'long_description': "# TraceX Parser\n[![Documentation Status](https://readthedocs.org/projects/tracex_parser/badge/?version=latest)](https://tracex_parser.readthedocs.io/en/latest/?badge=latest)\n[![CircleCI](https://circleci.com/gh/julianneswinoga/tracex_parser.svg?style=shield)](https://circleci.com/gh/julianneswinoga/tracex_parser)\n[![Coverage Status](https://coveralls.io/repos/github/julianneswinoga/tracex_parser/badge.svg?branch=master)](https://coveralls.io/github/julianneswinoga/tracex_parser?branch=master)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tracex_parser)](https://pypi.org/project/tracex_parser/)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/tracex_parser)\n\nThis python package parses ThreadX trace buffers into both human and machine-readable formats.\nDon't know where to begin? Check out the [quick-start](https://tracex-parser.readthedocs.io/en/latest/quickstart.html) documentation.\nMore documentation about ThreadX trace buffers can be found [here](https://docs.microsoft.com/en-us/azure/rtos/tracex/chapter5).\n\n## Install\n`pip3 install tracex-parser`\n\n## Example trace buffers\nIn the repository source there are a couple example TraceX traces which can be used to verify that things are working correctly.\n### As a python module\n[documentation](https://tracex-parser.readthedocs.io/en/latest/py-interface.html)\n```pycon\n>>> from tracex_parser.file_parser import parse_tracex_buffer\n>>> events, obj_map = parse_tracex_buffer('./demo_threadx.trx')\n>>> events\n[4265846278:thread 7 threadResume(thread_ptr=thread 6,prev_state=0xd,stack_ptr=0x12980,next_thread=), 4265846441:thread 7 mtxPut(obj_id=mutex 0,owning_thread=0x6adc,own_cnt=0x1,stack_ptr=0x129a0), 4265846566:thread 7 mtxPut(obj_id=mutex 0,owning_thread=0x6adc,own_cnt=0x2,stack_ptr=0x129a0)]\n>>> obj_map[0xeea4]\n{'obj_reg_entry_obj_available **': '0x0', 'obj_reg_entry_obj_type **': '0x1', 'thread_reg_entry_obj_ptr': '0xeea4', 'obj_reg_entry_obj_parameter_1': '0xef4c', 'obj_reg_entry_obj_parameter_2': '0x3fc', 'thread_reg_entry_obj_name': b'System Timer Thread'}\n```\n\n### As a command line utility\n[documentation](https://tracex-parser.readthedocs.io/en/latest/cli-interface.html)\nThe `file_parser` module can also be run as a script, which will provide simple statistics on the trace as well as dumping all the events in the trace:\n```console\n$ python3 -m tracex_parser.file_parser -vvv ./demo_threadx.trx\nParsing ./demo_threadx.trx\ntotal events: 974\nobject registry size: 16\ndelta ticks: 156206\nEvent Histogram:\nqueueSend           493\nqueueReceive        428\nthreadResume        19\nthreadSuspend       16\nmtxPut              4\nisrExit             3\nisrEnter            3\nsemGet              2\nsemPut              2\nthreadSleep         2\nmtxGet              2\nAll events:\n4265846278:thread 7 threadResume(thread_ptr=thread 6,prev_state=0xd,stack_ptr=0x12980,next_thread=)\n4265846441:thread 7 mtxPut(obj_id=mutex 0,owning_thread=0x6adc,own_cnt=0x1,stack_ptr=0x129a0)\n4265846566:thread 7 mtxPut(obj_id=mutex 0,owning_thread=0x6adc,own_cnt=0x2,stack_ptr=0x129a0)\n4265846825:thread 4 threadSuspend(thread_ptr=thread 4,new_state=0x6,stack_ptr=0x11d70,next_thread=thread 7)\n4265846953:thread 4 semGet(obj_id=semaphore 0,timeout=WaitForever,cur_cnt=0x0,stack_ptr=0x11d98)\n...\n",
     'author': 'Julianne Swinoga',
     'author_email': 'julianneswinoga@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `tracex_parser-2.2.0/PKG-INFO` & `tracex_parser-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracex-parser
-Version: 2.2.0
+Version: 2.3.0
 Summary: Parser for ThreadX RTOS's trace buffers (aka TraceX)
 License: MIT
 Author: Julianne Swinoga
 Author-email: julianneswinoga@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

