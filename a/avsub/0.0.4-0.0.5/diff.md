# Comparing `tmp/avsub-0.0.4.tar.gz` & `tmp/avsub-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avsub-0.0.4.tar", last modified: Fri Jul  7 20:12:19 2023, max compression
+gzip compressed data, was "avsub-0.0.5.tar", last modified: Sat Jul 29 10:39:46 2023, max compression
```

## Comparing `avsub-0.0.4.tar` & `avsub-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 20:12:19.464959 avsub-0.0.4/
--rw-rw-rw-   0        0        0    35823 2023-04-18 01:59:47.000000 avsub-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      797 2023-07-07 20:12:19.464959 avsub-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       44 2023-04-18 01:59:47.000000 avsub-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 20:12:19.422742 avsub-0.0.4/avsub/
--rw-rw-rw-   0        0        0        0 2023-04-18 01:59:47.000000 avsub-0.0.4/avsub/__init__.py
--rw-rw-rw-   0        0        0     3850 2023-04-18 01:59:47.000000 avsub-0.0.4/avsub/__main__.py
--rw-rw-rw-   0        0        0       81 2023-07-06 21:02:32.000000 avsub-0.0.4/avsub/__version__.py
--rw-rw-rw-   0        0        0      433 2023-04-18 01:59:47.000000 avsub-0.0.4/avsub/actions.py
--rw-rw-rw-   0        0        0     6106 2023-07-07 19:47:45.000000 avsub-0.0.4/avsub/cli.py
--rw-rw-rw-   0        0        0      735 2023-07-07 19:34:42.000000 avsub-0.0.4/avsub/consts.py
--rw-rw-rw-   0        0        0     4112 2023-07-07 20:07:19.000000 avsub-0.0.4/avsub/ffmpeg.py
--rw-rw-rw-   0        0        0      211 2023-04-18 01:59:47.000000 avsub-0.0.4/avsub/globs.py
--rw-rw-rw-   0        0        0     1680 2023-04-18 01:59:47.000000 avsub-0.0.4/avsub/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-07 20:12:19.464959 avsub-0.0.4/avsub.egg-info/
--rw-rw-rw-   0        0        0      797 2023-07-07 20:12:19.000000 avsub-0.0.4/avsub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-07-07 20:12:19.000000 avsub-0.0.4/avsub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 20:12:19.000000 avsub-0.0.4/avsub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-07 20:12:19.000000 avsub-0.0.4/avsub.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-07-07 20:12:18.000000 avsub-0.0.4/avsub.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-07-07 20:12:19.000000 avsub-0.0.4/avsub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1049 2023-04-18 01:59:47.000000 avsub-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-07 20:12:19.464959 avsub-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-29 10:39:46.697640 avsub-0.0.5/
+-rw-rw-rw-   0        0        0    35823 2023-04-18 01:59:47.000000 avsub-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      797 2023-07-29 10:39:46.694247 avsub-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2023-07-18 19:40:13.000000 avsub-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 10:39:46.664408 avsub-0.0.5/avsub/
+-rw-rw-rw-   0        0        0        0 2023-04-18 01:59:47.000000 avsub-0.0.5/avsub/__init__.py
+-rw-rw-rw-   0        0        0     3861 2023-07-18 19:19:01.000000 avsub-0.0.5/avsub/__main__.py
+-rw-rw-rw-   0        0        0       81 2023-07-29 10:38:44.000000 avsub-0.0.5/avsub/__version__.py
+-rw-rw-rw-   0        0        0      421 2023-07-29 04:22:37.000000 avsub-0.0.5/avsub/actions.py
+-rw-rw-rw-   0        0        0     6056 2023-07-29 04:22:37.000000 avsub-0.0.5/avsub/cli.py
+-rw-rw-rw-   0        0        0      735 2023-07-07 19:34:42.000000 avsub-0.0.5/avsub/consts.py
+-rw-rw-rw-   0        0        0     4112 2023-07-18 19:36:58.000000 avsub-0.0.5/avsub/ffmpeg.py
+-rw-rw-rw-   0        0        0      211 2023-04-18 01:59:47.000000 avsub-0.0.5/avsub/globs.py
+-rw-rw-rw-   0        0        0     1717 2023-07-29 05:10:18.000000 avsub-0.0.5/avsub/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:39:46.690741 avsub-0.0.5/avsub.egg-info/
+-rw-rw-rw-   0        0        0      797 2023-07-29 10:39:46.000000 avsub-0.0.5/avsub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-07-29 10:39:46.000000 avsub-0.0.5/avsub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 10:39:46.000000 avsub-0.0.5/avsub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-29 10:39:46.000000 avsub-0.0.5/avsub.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-07-29 10:39:46.000000 avsub-0.0.5/avsub.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-07-29 10:39:46.000000 avsub-0.0.5/avsub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1049 2023-04-18 01:59:47.000000 avsub-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-29 10:39:46.697640 avsub-0.0.5/setup.cfg
```

### Comparing `avsub-0.0.4/LICENSE` & `avsub-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `avsub-0.0.4/PKG-INFO` & `avsub-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avsub
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simplified command-line interface for FFmpeg
 Author: Serhat Çelik
 License: GPLv3
 Keywords: avsub,audio,video,subtitle,ffmpeg
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `avsub-0.0.4/avsub/__main__.py` & `avsub-0.0.5/avsub/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 import tempfile
 from contextlib import suppress
 from datetime import datetime, timedelta
 from tkinter.filedialog import askdirectory, askopenfilename, askopenfilenames
 from typing import NoReturn
 
 from avsub.cli import parser
-from avsub.consts import X
+from avsub.consts import (
+    X,
+)
 from avsub.ffmpeg import FFmpeg
 from avsub.globs import completed, controller, corrupted, untouched
 from avsub.utils import exit_if_not, separate, splitext
 
 
 def start() -> tuple[int | None, bool]:
     """Start the program."""
@@ -108,16 +110,16 @@
     except OverflowError as err:
         print('[!]', err)
         return
 
     message = f'AVsub has scheduled a shutdown for {schedule}.'
 
     shutdown = {
-        'linux': (['shutdown', '-P', str(sec), message], '-c'),
-        'win32': (['shutdown', '/t', str(sec), '/s', '/c', message], '/a'),
+        'linux': (('shutdown', '-P', str(sec), message), '-c'),
+        'win32': (('shutdown', '/t', str(sec), '/s', '/c', message), '/a'),
     }
 
     if sys.platform not in shutdown:
         print('[!]', 'Cannot schedule shutdown on this platform.')
         return
 
     cmd, cancel = shutdown[sys.platform]
```

### Comparing `avsub-0.0.4/avsub/cli.py` & `avsub-0.0.5/avsub/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,31 +11,30 @@
     CHOICES_SUB_BGR_CHART,
     X,
 )
 from avsub.utils import check_for_updates
 
 parser = argparse.ArgumentParser(
     prog='avsub',
-    usage='%(prog)s <extension> [<option> ...]',
     description='%(prog)s — a simplified command-line interface for ffmpeg',
     epilog='https://github.com/serhatcelik/avsub',
     formatter_class=argparse.RawTextHelpFormatter,
     allow_abbrev=False,
 )
 
 parser.register('action', 'exit', ExitAction)
 
-burn = parser.add_argument_group('options embed')
+burn = parser.add_argument_group('hardsub')
 misc = parser.add_argument_group('miscellaneous')
 
 mutual = parser.add_mutually_exclusive_group()
 
-########################
-# Positional Arguments #
-########################
+###############
+# Positionals #
+###############
 parser.add_argument(
     'extension',
     help=f'output extension or {X}',
     metavar='extension',
 )
 
 ###########
@@ -76,16 +75,16 @@
     help='set %(metavar)s as crf value for compression (const: %(const)s)',
     metavar='VALUE',
     dest='compress',
 )
 parser.add_argument(
     '--copy', '-c',
     nargs='+',
-    default=[],
-    choices=[X, 'audio', 'subtitle', 'video'],
+    default=(),
+    choices=(X, 'audio', 'subtitle', 'video'),
     help='use copy codec for output %(metavar)s stream (choices: %(choices)s)',
     metavar='STREAM',
     dest='copy',
 )
 parser.add_argument(
     '--disable-select',
     action='store_true',
@@ -104,40 +103,40 @@
     help='set %(metavar)s as frame rate',
     metavar='VALUE',
     dest='frame',
 )
 mutual.add_argument(
     '--only-audio', '-A',
     action='store_const',
-    const=['-dn', '-sn', '-vn'],
-    default=[],
+    const=('-dn', '-sn', '-vn'),
+    default=(),
     help='choose audio stream only',
     dest='only_a',
 )
 mutual.add_argument(
     '--only-subtitle', '-S',
     action='store_const',
-    const=['-an', '-dn', '-vn'],
-    default=[],
+    const=('-an', '-dn', '-vn'),
+    default=(),
     help='choose subtitle stream only',
     dest='only_s',
 )
 mutual.add_argument(
     '--only-video', '-V',
     action='store_const',
-    const=['-an', '-dn', '-sn'],
-    default=[],
+    const=('-an', '-dn', '-sn'),
+    default=(),
     help='choose video stream only',
     dest='only_v',
 )
 parser.add_argument(
     '--remove', '-r',
     nargs='+',
-    default=[],
-    choices=['audio', 'data', 'subtitle', 'video'],
+    default=(),
+    choices=('audio', 'data', 'subtitle', 'video'),
     help='do not copy %(metavar)s stream to output (choices: %(choices)s)',
     metavar='STREAM',
     dest='remove',
 )
 parser.add_argument(
     '--remove-chapters',
     action='store_true',
@@ -164,17 +163,17 @@
     type=int,
     choices=range(0, 60),
     help='extract a part of a video',
     metavar=('H:', 'M:', 'S:', ':H', ':M', ':S'),
     dest='trim',
 )
 
-#################
-# Options Embed #
-#################
+####################
+# Options: Hardsub #
+####################
 burn.add_argument(
     '--burn',
     action='store_true',
     help='burn a subtitle into a video',
     dest='burn',
 )
 burn.add_argument(
@@ -213,22 +212,22 @@
     default='bottom',
     choices=CHOICES_SUB_ALIGNMENT,
     help='set %(metavar)s as subtitle position (choices: %(choices)s)',
     metavar='POSITION',
     dest='alignment',
 )
 
-#################
-# Miscellaneous #
-#################
+##########################
+# Options: Miscellaneous #
+##########################
 misc.add_argument(
     '-?',
     action='exit',
     help='check for program updates and exit',
-    func=check_for_updates,
+    f=check_for_updates,
     args=(__version__,),
 )
 misc.add_argument(
     '--shutdown',
     nargs='?',
     const=0,
     type=int,
```

### Comparing `avsub-0.0.4/avsub/consts.py` & `avsub-0.0.5/avsub/consts.py`

 * *Files identical despite different names*

### Comparing `avsub-0.0.4/avsub/ffmpeg.py` & `avsub-0.0.5/avsub/ffmpeg.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,25 +41,25 @@
         if opts.codec_s:
             cmd += ['-codec:s', opts.codec_s]
         if opts.codec_v:
             cmd += ['-codec:v', opts.codec_v]
 
         cmd += ['-crf', str(opts.compress)]
 
-        cmd += chain(*(['-codec:' + _[0].strip(X), 'copy'] for _ in opts.copy))
+        cmd += chain(*(['-codec:' + s[0].strip(X), 'copy'] for s in opts.copy))
 
         if not opts.disable:
             cmd += ['-map', '0']
 
         if opts.frame is not None:
             cmd += ['-r', str(opts.frame)]
 
         cmd += opts.only_a + opts.only_s + opts.only_v
 
-        cmd += [f'-{_[0]}n' for _ in opts.remove]
+        cmd += [f'-{s[0]}n' for s in opts.remove]
 
         cmd += ['-map_chapters', str(-int(opts.chapters))]
         cmd += ['-map_metadata', str(-int(opts.metadata))]
 
         if opts.speed is not None:
             speed_a, speed_v = opts.speed
             by_a, by_v = float(Fraction(speed_a)), float(Fraction(speed_v))
```

### Comparing `avsub-0.0.4/avsub/utils.py` & `avsub-0.0.5/avsub/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """General utilities."""
 
+import functools
 import os
 import sys
 import webbrowser
 from tkinter.messagebox import askokcancel
 from typing import Any, NoReturn
 from urllib.error import URLError
 from urllib.request import urlopen
@@ -11,53 +12,54 @@
 
 def check_for_updates(current: str):
     """Check for program updates."""
     file = 'https://raw.githubusercontent.com/serhatcelik/avsub/main/VERSION'
 
     try:
         with urlopen(file, timeout=9) as answer:  # nosec
-            latest = answer.readline().rstrip().decode()
+            latest = answer.readline().decode().rstrip()
     except URLError as err:
         print('[!]', err)
         return
 
     if current == latest:
         print('[*]', 'Up to date!')
         return
 
     print('[*]', message := 'Update available. Download?')
 
     if not askokcancel(message=message, icon='warning'):
         return
 
-    zip_ = 'https://github.com/serhatcelik/avsub/archive/refs/heads/main.zip'
+    zipp = 'https://github.com/serhatcelik/avsub/archive/refs/heads/main.zip'
 
-    webbrowser.open_new_tab(zip_)
+    webbrowser.open_new_tab(zipp)
 
 
 def exit_if_not(thing: Any, /, status: int | str = 0) -> Any | NoReturn:
     """Conditional exit: if not."""
     if not thing:
         sys.exit(status)
     return thing
 
 
-def separate(func):
+def separate(f):
     """Draw a horizontal line before and after the given function."""
 
+    @functools.wraps(f)
     def wrapper(*args, **kwargs):
         print('-' * os.get_terminal_size().columns)
-        func(*args, **kwargs)
+        f(*args, **kwargs)
         print('-' * os.get_terminal_size().columns)
 
     return wrapper
 
 
 def splitext(path: str) -> tuple[str, str]:
     """Split the pathname `path` into a pair."""
     tail = os.path.split(path)[1]
 
-    extension = ''.join(_[1:]) if (_ := tail.rpartition('.'))[1] else _[1]
+    extension = ''.join(t[1:]) if (t := tail.rpartition('.'))[1] else t[1]
 
     filename = path.removesuffix(extension)
 
     return filename, extension
```

### Comparing `avsub-0.0.4/avsub.egg-info/PKG-INFO` & `avsub-0.0.5/avsub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avsub
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simplified command-line interface for FFmpeg
 Author: Serhat Çelik
 License: GPLv3
 Keywords: avsub,audio,video,subtitle,ffmpeg
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `avsub-0.0.4/pyproject.toml` & `avsub-0.0.5/pyproject.toml`

 * *Files identical despite different names*

