# Comparing `tmp/captcha-0.4.tar.gz` & `tmp/captcha-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "captcha-0.4.tar", last modified: Tue Mar 15 10:34:10 2022, max compression
+gzip compressed data, was "captcha-0.5.0.tar", last modified: Sat Jul 29 01:46:25 2023, max compression
```

## Comparing `captcha-0.4.tar` & `captcha-0.5.0.tar`

### file list

```diff
@@ -1,41 +1,60 @@
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-03-15 10:34:10.940132 captcha-0.4/
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1475 2022-03-15 10:31:28.000000 captcha-0.4/LICENSE
--rw-r--r--   0 lepture   (1000) lepture   (1000)      109 2022-03-15 10:31:28.000000 captcha-0.4/MANIFEST.in
--rw-r--r--   0 lepture   (1000) lepture   (1000)     4214 2022-03-15 10:34:10.938138 captcha-0.4/PKG-INFO
--rw-r--r--   0 lepture   (1000) lepture   (1000)     2407 2022-03-15 10:31:28.000000 captcha-0.4/README.rst
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-03-15 10:34:10.634286 captcha-0.4/captcha/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      334 2022-03-15 10:31:49.000000 captcha-0.4/captcha/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     7597 2022-03-15 10:31:28.000000 captcha-0.4/captcha/audio.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-03-15 10:34:10.736132 captcha-0.4/captcha/data/
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-03-15 10:34:10.752132 captcha-0.4/captcha/data/0/
--rw-r--r--   0 lepture   (1000) lepture   (1000)     2791 2022-03-15 10:31:28.000000 captcha-0.4/captcha/data/0/default.wav
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-03-15 10:34:10.769132 captcha-0.4/captcha/data/1/
--rw-r--r--   0 lepture   (1000) lepture   (1000)     2018 2022-03-15 10:31:28.000000 captcha-0.4/captcha/data/1/default.wav
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-03-15 10:34:10.786132 captcha-0.4/captcha/data/2/
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1991 2022-03-15 10:31:28.000000 captcha-0.4/captcha/data/2/default.wav
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-03-15 10:34:10.805132 captcha-0.4/captcha/data/3/
--rw-r--r--   0 lepture   (1000) lepture   (1000)     2324 2022-03-15 10:31:28.000000 captcha-0.4/captcha/data/3/default.wav
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-03-15 10:34:10.824132 captcha-0.4/captcha/data/4/
--rw-r--r--   0 lepture   (1000) lepture   (1000)     2331 2022-03-15 10:31:28.000000 captcha-0.4/captcha/data/4/default.wav
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-03-15 10:34:10.844134 captcha-0.4/captcha/data/5/
--rw-r--r--   0 lepture   (1000) lepture   (1000)     2674 2022-03-15 10:31:28.000000 captcha-0.4/captcha/data/5/default.wav
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-03-15 10:34:10.865132 captcha-0.4/captcha/data/6/
--rw-r--r--   0 lepture   (1000) lepture   (1000)     2427 2022-03-15 10:31:28.000000 captcha-0.4/captcha/data/6/default.wav
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-03-15 10:34:10.884132 captcha-0.4/captcha/data/7/
--rw-r--r--   0 lepture   (1000) lepture   (1000)     2789 2022-03-15 10:31:28.000000 captcha-0.4/captcha/data/7/default.wav
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-03-15 10:34:10.903132 captcha-0.4/captcha/data/8/
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1851 2022-03-15 10:31:28.000000 captcha-0.4/captcha/data/8/default.wav
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-03-15 10:34:10.922132 captcha-0.4/captcha/data/9/
--rw-r--r--   0 lepture   (1000) lepture   (1000)     2385 2022-03-15 10:31:28.000000 captcha-0.4/captcha/data/9/default.wav
--rw-r--r--   0 lepture   (1000) lepture   (1000)   117072 2022-03-15 10:31:28.000000 captcha-0.4/captcha/data/DroidSansMono.ttf
--rw-r--r--   0 lepture   (1000) lepture   (1000)      940 2022-03-15 10:31:28.000000 captcha-0.4/captcha/data/beep.wav
--rw-r--r--   0 lepture   (1000) lepture   (1000)     7600 2022-03-15 10:31:28.000000 captcha-0.4/captcha/image.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-03-15 10:34:10.705132 captcha-0.4/captcha.egg-info/
--rw-r--r--   0 lepture   (1000) lepture   (1000)     4214 2022-03-15 10:34:10.000000 captcha-0.4/captcha.egg-info/PKG-INFO
--rw-r--r--   0 lepture   (1000) lepture   (1000)      600 2022-03-15 10:34:10.000000 captcha-0.4/captcha.egg-info/SOURCES.txt
--rw-r--r--   0 lepture   (1000) lepture   (1000)        1 2022-03-15 10:34:10.000000 captcha-0.4/captcha.egg-info/dependency_links.txt
--rw-r--r--   0 lepture   (1000) lepture   (1000)        1 2022-03-15 10:34:10.000000 captcha-0.4/captcha.egg-info/not-zip-safe
--rw-r--r--   0 lepture   (1000) lepture   (1000)        7 2022-03-15 10:34:10.000000 captcha-0.4/captcha.egg-info/requires.txt
--rw-r--r--   0 lepture   (1000) lepture   (1000)        8 2022-03-15 10:34:10.000000 captcha-0.4/captcha.egg-info/top_level.txt
--rw-r--r--   0 lepture   (1000) lepture   (1000)       38 2022-03-15 10:34:10.940132 captcha-0.4/setup.cfg
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1796 2022-03-15 10:31:28.000000 captcha-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:46:25.270702 captcha-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-29 01:46:16.000000 captcha-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-29 01:46:16.000000 captcha-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-29 01:46:25.270702 captcha-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-29 01:46:16.000000 captcha-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:46:25.266702 captcha-0.5.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:46:25.266702 captcha-0.5.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-07-29 01:46:16.000000 captcha-0.5.0/docs/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-29 01:46:16.000000 captcha-0.5.0/docs/_static/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-07-29 01:46:16.000000 captcha-0.5.0/docs/_static/image-demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-07-29 01:46:16.000000 captcha-0.5.0/docs/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-29 01:46:16.000000 captcha-0.5.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-29 01:46:16.000000 captcha-0.5.0/docs/audio.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-29 01:46:16.000000 captcha-0.5.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-29 01:46:16.000000 captcha-0.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-29 01:46:16.000000 captcha-0.5.0/docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-29 01:46:16.000000 captcha-0.5.0/docs/image.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-29 01:46:16.000000 captcha-0.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 01:46:16.000000 captcha-0.5.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-29 01:46:16.000000 captcha-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 01:46:25.270702 captcha-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 01:46:16.000000 captcha-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:46:25.262702 captcha-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:46:25.266702 captcha-0.5.0/src/captcha/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-29 01:46:16.000000 captcha-0.5.0/src/captcha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-29 01:46:16.000000 captcha-0.5.0/src/captcha/audio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:46:25.266702 captcha-0.5.0/src/captcha/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:46:25.266702 captcha-0.5.0/src/captcha/data/0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-29 01:46:16.000000 captcha-0.5.0/src/captcha/data/0/default.wav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:46:25.266702 captcha-0.5.0/src/captcha/data/1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-29 01:46:16.000000 captcha-0.5.0/src/captcha/data/1/default.wav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:46:25.266702 captcha-0.5.0/src/captcha/data/2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-29 01:46:16.000000 captcha-0.5.0/src/captcha/data/2/default.wav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:46:25.270702 captcha-0.5.0/src/captcha/data/3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-29 01:46:16.000000 captcha-0.5.0/src/captcha/data/3/default.wav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:46:25.270702 captcha-0.5.0/src/captcha/data/4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-29 01:46:16.000000 captcha-0.5.0/src/captcha/data/4/default.wav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:46:25.270702 captcha-0.5.0/src/captcha/data/5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-29 01:46:16.000000 captcha-0.5.0/src/captcha/data/5/default.wav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:46:25.270702 captcha-0.5.0/src/captcha/data/6/
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-07-29 01:46:16.000000 captcha-0.5.0/src/captcha/data/6/default.wav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:46:25.270702 captcha-0.5.0/src/captcha/data/7/
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-29 01:46:16.000000 captcha-0.5.0/src/captcha/data/7/default.wav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:46:25.270702 captcha-0.5.0/src/captcha/data/8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-29 01:46:16.000000 captcha-0.5.0/src/captcha/data/8/default.wav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:46:25.270702 captcha-0.5.0/src/captcha/data/9/
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-29 01:46:16.000000 captcha-0.5.0/src/captcha/data/9/default.wav
+-rw-r--r--   0 runner    (1001) docker     (123)   117072 2023-07-29 01:46:16.000000 captcha-0.5.0/src/captcha/data/DroidSansMono.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-29 01:46:16.000000 captcha-0.5.0/src/captcha/data/beep.wav
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-07-29 01:46:16.000000 captcha-0.5.0/src/captcha/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 01:46:16.000000 captcha-0.5.0/src/captcha/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:46:25.266702 captcha-0.5.0/src/captcha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-29 01:46:25.000000 captcha-0.5.0/src/captcha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-29 01:46:25.000000 captcha-0.5.0/src/captcha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 01:46:25.000000 captcha-0.5.0/src/captcha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-29 01:46:25.000000 captcha-0.5.0/src/captcha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-29 01:46:25.000000 captcha-0.5.0/src/captcha.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:46:25.270702 captcha-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-29 01:46:16.000000 captcha-0.5.0/tests/test_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-29 01:46:16.000000 captcha-0.5.0/tests/test_image.py
```

### Comparing `captcha-0.4/LICENSE` & `captcha-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `captcha-0.4/captcha/audio.py` & `captcha-0.5.0/src/captcha/audio.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,64 +4,61 @@
     ~~~~~~~~~~~~~
 
     Generate Audio CAPTCHAs, with built-in digits CAPTCHA.
 
     This module is totally inspired by https://github.com/dchest/captcha
 """
 
+import typing as t
 import os
 import copy
 import wave
 import struct
 import random
 import operator
-
-import sys
-if sys.version_info[0] != 2:
-    import functools
-    reduce = functools.reduce
+from functools import reduce
 
 
 __all__ = ['AudioCaptcha']
 
 WAVE_SAMPLE_RATE = 8000  # HZ
 WAVE_HEADER = bytearray(
     b'RIFF\x00\x00\x00\x00WAVEfmt \x10\x00\x00\x00\x01\x00\x01\x00'
     b'@\x1f\x00\x00@\x1f\x00\x00\x01\x00\x08\x00data'
 )
 WAVE_HEADER_LENGTH = len(WAVE_HEADER) - 4
 DATA_DIR = os.path.join(os.path.abspath(os.path.dirname(__file__)), 'data')
 
 
-def _read_wave_file(filepath):
+def _read_wave_file(filepath: str) -> bytearray:
     w = wave.open(filepath)
     data = w.readframes(-1)
     w.close()
     return bytearray(data)
 
 
-def change_speed(body, speed=1):
+def change_speed(body: bytearray, speed: float = 1) -> bytearray:
     """Change the voice speed of the wave body."""
     if speed == 1:
         return body
 
     length = int(len(body) * speed)
     rv = bytearray(length)
 
-    step = 0
+    step: float = 0
     for v in body:
         i = int(step)
         while i < int(step + speed) and i < length:
             rv[i] = v
             i += 1
         step += speed
     return rv
 
 
-def patch_wave_header(body):
+def patch_wave_header(body: bytearray) -> bytearray:
     """Patch header to the given wave body.
 
     :param body: the wave content body, it should be bytearray.
     """
     length = len(body)
 
     padded = length + length % 2
@@ -77,55 +74,55 @@
     # the total length is even
     if length != padded:
         data = data + bytearray([0])
 
     return data
 
 
-def create_noise(length, level=4):
+def create_noise(length: int, level: int = 4) -> bytearray:
     """Create white noise for background"""
     noise = bytearray(length)
     adjust = 128 - int(level / 2)
     i = 0
     while i < length:
         v = random.randint(0, 256)
         noise[i] = v % level + adjust
         i += 1
     return noise
 
 
-def create_silence(length):
+def create_silence(length: int) -> bytearray:
     """Create a piece of silence."""
     data = bytearray(length)
     i = 0
     while i < length:
         data[i] = 128
         i += 1
     return data
 
 
-def change_sound(body, level=1):
+def change_sound(body: bytearray, level: float = 1) -> bytearray:
     if level == 1:
         return body
 
     body = copy.copy(body)
     for i, v in enumerate(body):
         if v > 128:
-            v = (v - 128) * level + 128
-            v = max(int(v), 128)
+            v = int((v - 128) * level + 128)
+            v = max(v, 128)
             v = min(v, 255)
         elif v < 128:
-            v = 128 - (128 - v) * level
-            v = min(int(v), 128)
+            v = int(128 - (128 - v) * level)
+            v = min(v, 128)
             v = max(v, 0)
         body[i] = v
     return body
 
 
-def mix_wave(src, dst):
+def mix_wave(src: bytearray, dst: bytearray) -> bytearray:
     """Mix two wave body into one."""
     if len(src) > len(dst):
         # output should be longer
         dst, src = src, dst
 
     for i, sv in enumerate(src):
         dv = dst[i]
@@ -137,15 +134,15 @@
 
 
 BEEP = _read_wave_file(os.path.join(DATA_DIR, 'beep.wav'))
 END_BEEP = change_speed(BEEP, 1.4)
 SILENCE = create_silence(int(WAVE_SAMPLE_RATE / 5))
 
 
-class AudioCaptcha(object):
+class AudioCaptcha:
     """Create an audio CAPTCHA.
 
     Create an instance of AudioCaptcha is pretty simple::
 
         captcha = AudioCaptcha()
         captcha.write('1234', 'out.wav')
 
@@ -162,121 +159,121 @@
     the directory name. A charater directory can has many wave files, this
     AudioCaptcha will randomly choose one of them.
 
     You should always use your own voice library::
 
         captcha = AudioCaptcha(voicedir='/path/to/voices')
     """
-    def __init__(self, voicedir=None):
+    def __init__(self, voicedir: t.Optional[str] = None):
         if voicedir is None:
             voicedir = DATA_DIR
 
         self._voicedir = voicedir
-        self._cache = {}
-        self._choices = []
+        self._cache: t.Dict[str, t.List[bytearray]] = {}
+        self._choices: t.List[str] = []
 
     @property
-    def choices(self):
+    def choices(self) -> t.List[str]:
         """Available choices for characters to be generated."""
         if self._choices:
             return self._choices
         for n in os.listdir(self._voicedir):
             if len(n) == 1 and os.path.isdir(os.path.join(self._voicedir, n)):
                 self._choices.append(n)
         return self._choices
 
-    def random(self, length=6):
+    def random(self, length: int = 6) -> t.List[str]:
         """Generate a random string with the given length.
 
         :param length: the return string length.
         """
         return random.sample(self.choices, length)
 
-    def load(self):
+    def load(self) -> None:
         """Load voice data into memory."""
         for name in self.choices:
             self._load_data(name)
 
-    def _load_data(self, name):
+    def _load_data(self, name: str) -> None:
         dirname = os.path.join(self._voicedir, name)
-        data = []
+        data: t.List[bytearray] = []
         for f in os.listdir(dirname):
             filepath = os.path.join(dirname, f)
             if f.endswith('.wav') and os.path.isfile(filepath):
                 data.append(_read_wave_file(filepath))
         self._cache[name] = data
 
-    def _twist_pick(self, key):
+    def _twist_pick(self, key: str) -> bytearray:
         voice = random.choice(self._cache[key])
 
         # random change speed
         speed = random.randrange(90, 120) / 100.0
         voice = change_speed(voice, speed)
 
         # random change sound
         level = random.randrange(80, 120) / 100.0
         voice = change_sound(voice, level)
         return voice
 
-    def _noise_pick(self):
+    def _noise_pick(self) -> bytearray:
         key = random.choice(self.choices)
         voice = random.choice(self._cache[key])
         voice = copy.copy(voice)
         voice.reverse()
 
         speed = random.randrange(8, 16) / 10.0
         voice = change_speed(voice, speed)
 
         level = random.randrange(2, 6) / 10.0
         voice = change_sound(voice, level)
         return voice
 
-    def create_background_noise(self, length, chars):
+    def create_background_noise(self, length: int, chars: str) -> bytearray:
         noise = create_noise(length, 4)
         pos = 0
         while pos < length:
             sound = self._noise_pick()
             end = pos + len(sound) + 1
             noise[pos:end] = mix_wave(sound, noise[pos:end])
             pos = end + random.randint(0, int(WAVE_SAMPLE_RATE / 10))
         return noise
 
-    def create_wave_body(self, chars):
-        voices = []
-        inters = []
-        for key in chars:
-            voices.append(self._twist_pick(key))
-            v = random.randint(WAVE_SAMPLE_RATE, WAVE_SAMPLE_RATE * 3)
-            inters.append(v)
+    def create_wave_body(self, chars: str) -> bytearray:
+        voices: t.List[bytearray] = []
+        inters: t.List[int] = []
+        for c in chars:
+            voices.append(self._twist_pick(c))
+            i = random.randint(WAVE_SAMPLE_RATE, WAVE_SAMPLE_RATE * 3)
+            inters.append(i)
 
         durations = map(lambda a: len(a), voices)
         length = max(durations) * len(chars) + reduce(operator.add, inters)
         bg = self.create_background_noise(length, chars)
 
         # begin
-        pos = inters[0]
+        pos: int = inters[0]
         for i, v in enumerate(voices):
             end = pos + len(v) + 1
             bg[pos:end] = mix_wave(v, bg[pos:end])
             pos = end + inters[i]
 
         return BEEP + SILENCE + BEEP + SILENCE + BEEP + bg + END_BEEP
 
-    def generate(self, chars):
+    def generate(self, chars: str) -> bytearray:
         """Generate audio CAPTCHA data. The return data is a bytearray.
 
         :param chars: text to be generated.
         """
         if not self._cache:
             self.load()
         body = self.create_wave_body(chars)
         return patch_wave_header(body)
 
-    def write(self, chars, output):
+    def write(self, chars: str, output: str) -> None:
         """Generate and write audio CAPTCHA data to the output.
 
         :param chars: text to be generated.
         :param output: output destionation.
         """
         data = self.generate(chars)
         with open(output, 'wb') as f:
-            return f.write(data)
+            f.write(data)
```

### Comparing `captcha-0.4/captcha/data/0/default.wav` & `captcha-0.5.0/src/captcha/data/0/default.wav`

 * *Files identical despite different names*

### Comparing `captcha-0.4/captcha/data/1/default.wav` & `captcha-0.5.0/src/captcha/data/1/default.wav`

 * *Files identical despite different names*

### Comparing `captcha-0.4/captcha/data/2/default.wav` & `captcha-0.5.0/src/captcha/data/2/default.wav`

 * *Files identical despite different names*

### Comparing `captcha-0.4/captcha/data/3/default.wav` & `captcha-0.5.0/src/captcha/data/3/default.wav`

 * *Files identical despite different names*

### Comparing `captcha-0.4/captcha/data/4/default.wav` & `captcha-0.5.0/src/captcha/data/4/default.wav`

 * *Files identical despite different names*

### Comparing `captcha-0.4/captcha/data/5/default.wav` & `captcha-0.5.0/src/captcha/data/5/default.wav`

 * *Files identical despite different names*

### Comparing `captcha-0.4/captcha/data/6/default.wav` & `captcha-0.5.0/src/captcha/data/6/default.wav`

 * *Files identical despite different names*

### Comparing `captcha-0.4/captcha/data/7/default.wav` & `captcha-0.5.0/src/captcha/data/7/default.wav`

 * *Files identical despite different names*

### Comparing `captcha-0.4/captcha/data/8/default.wav` & `captcha-0.5.0/src/captcha/data/8/default.wav`

 * *Files identical despite different names*

### Comparing `captcha-0.4/captcha/data/9/default.wav` & `captcha-0.5.0/src/captcha/data/9/default.wav`

 * *Files identical despite different names*

### Comparing `captcha-0.4/captcha/data/DroidSansMono.ttf` & `captcha-0.5.0/src/captcha/data/DroidSansMono.ttf`

 * *Files identical despite different names*

### Comparing `captcha-0.4/captcha/data/beep.wav` & `captcha-0.5.0/src/captcha/data/beep.wav`

 * *Files identical despite different names*

### Comparing `captcha-0.4/captcha/image.py` & `captcha-0.5.0/src/captcha/image.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,93 +4,31 @@
     ~~~~~~~~~~~~~
 
     Generate Image CAPTCHAs, just the normal image CAPTCHAs you are using.
 """
 
 import os
 import random
-from PIL import Image
-from PIL import ImageFilter
-from PIL.ImageDraw import Draw
-from PIL.ImageFont import truetype
-try:
-    from cStringIO import StringIO as BytesIO
-except ImportError:
-    from io import BytesIO
-try:
-    from wheezy.captcha import image as wheezy_captcha
-except ImportError:
-    wheezy_captcha = None
-
-DATA_DIR = os.path.join(os.path.abspath(os.path.dirname(__file__)), 'data')
-DEFAULT_FONTS = [os.path.join(DATA_DIR, 'DroidSansMono.ttf')]
-
-if wheezy_captcha:
-    __all__ = ['ImageCaptcha', 'WheezyCaptcha']
-else:
-    __all__ = ['ImageCaptcha']
+import typing as t
+from PIL.Image import new as createImage, Image, QUAD, BILINEAR
+from PIL.ImageDraw import Draw, ImageDraw
+from PIL.ImageFilter import SMOOTH
+from PIL.ImageFont import FreeTypeFont, truetype
+from io import BytesIO
 
+__all__ = ['ImageCaptcha']
 
-table  =  []
-for  i  in  range( 256 ):
-    table.append( int(i * 1.97) )
 
+ColorTuple = t.Union[t.Tuple[int, int, int], t.Tuple[int, int, int, int]]
 
-class _Captcha(object):
-    def generate(self, chars, format='png'):
-        """Generate an Image Captcha of the given characters.
-
-        :param chars: text to be generated.
-        :param format: image file format
-        """
-        im = self.generate_image(chars)
-        out = BytesIO()
-        im.save(out, format=format)
-        out.seek(0)
-        return out
-
-    def write(self, chars, output, format='png'):
-        """Generate and write an image CAPTCHA data to the output.
-
-        :param chars: text to be generated.
-        :param output: output destination.
-        :param format: image file format
-        """
-        im = self.generate_image(chars)
-        return im.save(output, format=format)
-
-
-class WheezyCaptcha(_Captcha):
-    """Create an image CAPTCHA with wheezy.captcha."""
-    def __init__(self, width=200, height=75, fonts=None):
-        self._width = width
-        self._height = height
-        self._fonts = fonts or DEFAULT_FONTS
-
-    def generate_image(self, chars):
-        text_drawings = [
-            wheezy_captcha.warp(),
-            wheezy_captcha.rotate(),
-            wheezy_captcha.offset(),
-        ]
-        fn = wheezy_captcha.captcha(
-            drawings=[
-                wheezy_captcha.background(),
-                wheezy_captcha.text(fonts=self._fonts, drawings=text_drawings),
-                wheezy_captcha.curve(),
-                wheezy_captcha.noise(),
-                wheezy_captcha.smooth(),
-            ],
-            width=self._width,
-            height=self._height,
-        )
-        return fn(chars)
+DATA_DIR = os.path.join(os.path.abspath(os.path.dirname(__file__)), 'data')
+DEFAULT_FONTS = [os.path.join(DATA_DIR, 'DroidSansMono.ttf')]
 
 
-class ImageCaptcha(_Captcha):
+class ImageCaptcha:
     """Create an image CAPTCHA.
 
     Many of the codes are borrowed from wheezy.captcha, with a modification
     for memory and developer friendly.
 
     ImageCaptcha has one built-in font, DroidSansMono, which is licensed under
     Apache License 2. You should always use your own fonts::
@@ -102,140 +40,187 @@
     many.
 
     :param width: The width of the CAPTCHA image.
     :param height: The height of the CAPTCHA image.
     :param fonts: Fonts to be used to generate CAPTCHA images.
     :param font_sizes: Random choose a font size from this parameters.
     """
-    def __init__(self, width=160, height=60, fonts=None, font_sizes=None):
+    lookup_table: t.List[int] = [int(i * 1.97) for i in range(256)]
+
+    def __init__(
+            self,
+            width: int = 160,
+            height: int = 60,
+            fonts: t.Optional[t.List[str]] = None,
+            font_sizes: t.Optional[t.Tuple[int]] = None):
         self._width = width
         self._height = height
         self._fonts = fonts or DEFAULT_FONTS
         self._font_sizes = font_sizes or (42, 50, 56)
-        self._truefonts = []
+        self._truefonts: t.List[FreeTypeFont] = []
 
     @property
-    def truefonts(self):
+    def truefonts(self) -> t.List[FreeTypeFont]:
         if self._truefonts:
             return self._truefonts
-        self._truefonts = tuple([
+        self._truefonts = [
             truetype(n, s)
             for n in self._fonts
             for s in self._font_sizes
-        ])
+        ]
         return self._truefonts
 
     @staticmethod
-    def create_noise_curve(image, color):
+    def create_noise_curve(image: Image, color: ColorTuple) -> Image:
         w, h = image.size
         x1 = random.randint(0, int(w / 5))
         x2 = random.randint(w - int(w / 5), w)
         y1 = random.randint(int(h / 5), h - int(h / 5))
         y2 = random.randint(y1, h - int(h / 5))
         points = [x1, y1, x2, y2]
         end = random.randint(160, 200)
         start = random.randint(0, 20)
         Draw(image).arc(points, start, end, fill=color)
         return image
 
     @staticmethod
-    def create_noise_dots(image, color, width=3, number=30):
+    def create_noise_dots(
+            image: Image,
+            color: ColorTuple,
+            width: int = 3,
+            number: int = 30) -> Image:
         draw = Draw(image)
         w, h = image.size
         while number:
             x1 = random.randint(0, w)
             y1 = random.randint(0, h)
             draw.line(((x1, y1), (x1 - 1, y1 - 1)), fill=color, width=width)
             number -= 1
         return image
 
-    def create_captcha_image(self, chars, color, background):
+    def _draw_character(
+            self,
+            c: str,
+            draw: ImageDraw,
+            color: ColorTuple) -> Image:
+        font = random.choice(self.truefonts)
+
+        left, top, right, bottom = draw.textbbox((0, 0), c, font=font)
+        w = int((right - left)*1.7) or 1
+        h = int((bottom - top)*1.7) or 1
+
+        dx1 = random.randint(0, 4)
+        dy1 = random.randint(0, 6)
+        im = createImage('RGBA', (w + dx1, h + dy1))
+        Draw(im).text((dx1, dy1), c, font=font, fill=color)
+
+        # rotate
+        im = im.crop(im.getbbox())
+        im = im.rotate(random.uniform(-30, 30), BILINEAR, expand=True)
+
+        # warp
+        dx2 = w * random.uniform(0.1, 0.3)
+        dy2 = h * random.uniform(0.2, 0.3)
+        x1 = int(random.uniform(-dx2, dx2))
+        y1 = int(random.uniform(-dy2, dy2))
+        x2 = int(random.uniform(-dx2, dx2))
+        y2 = int(random.uniform(-dy2, dy2))
+        w2 = w + abs(x1) + abs(x2)
+        h2 = h + abs(y1) + abs(y2)
+        data = (
+            x1, y1,
+            -x1, h2 - y2,
+            w2 + x2, h2 + y2,
+            w2 - x2, -y1,
+        )
+        im = im.resize((w2, h2))
+        im = im.transform((w, h), QUAD, data)
+        return im
+
+    def create_captcha_image(
+            self,
+            chars: str,
+            color: ColorTuple,
+            background: ColorTuple) -> Image:
         """Create the CAPTCHA image itself.
 
         :param chars: text to be generated.
         :param color: color of the text.
         :param background: color of the background.
 
         The color should be a tuple of 3 numbers, such as (0, 255, 255).
         """
-        image = Image.new('RGB', (self._width, self._height), background)
+        image = createImage('RGB', (self._width, self._height), background)
         draw = Draw(image)
 
-        def _draw_character(c):
-            font = random.choice(self.truefonts)
-            w, h = draw.textsize(c, font=font)
-
-            dx = random.randint(0, 4)
-            dy = random.randint(0, 6)
-            im = Image.new('RGBA', (w + dx, h + dy))
-            Draw(im).text((dx, dy), c, font=font, fill=color)
-
-            # rotate
-            im = im.crop(im.getbbox())
-            im = im.rotate(random.uniform(-30, 30), Image.BILINEAR, expand=1)
-
-            # warp
-            dx = w * random.uniform(0.1, 0.3)
-            dy = h * random.uniform(0.2, 0.3)
-            x1 = int(random.uniform(-dx, dx))
-            y1 = int(random.uniform(-dy, dy))
-            x2 = int(random.uniform(-dx, dx))
-            y2 = int(random.uniform(-dy, dy))
-            w2 = w + abs(x1) + abs(x2)
-            h2 = h + abs(y1) + abs(y2)
-            data = (
-                x1, y1,
-                -x1, h2 - y2,
-                w2 + x2, h2 + y2,
-                w2 - x2, -y1,
-            )
-            im = im.resize((w2, h2))
-            im = im.transform((w, h), Image.QUAD, data)
-            return im
-
-        images = []
+        images: t.List[Image] = []
         for c in chars:
             if random.random() > 0.5:
-                images.append(_draw_character(" "))
-            images.append(_draw_character(c))
+                images.append(self._draw_character(" ", draw, color))
+            images.append(self._draw_character(c, draw, color))
 
         text_width = sum([im.size[0] for im in images])
 
         width = max(text_width, self._width)
         image = image.resize((width, self._height))
 
         average = int(text_width / len(chars))
         rand = int(0.25 * average)
         offset = int(average * 0.1)
 
         for im in images:
             w, h = im.size
-            mask = im.convert('L').point(table)
+            mask = im.convert('L').point(self.lookup_table)
             image.paste(im, (offset, int((self._height - h) / 2)), mask)
             offset = offset + w + random.randint(-rand, 0)
 
         if width > self._width:
             image = image.resize((self._width, self._height))
 
         return image
 
-    def generate_image(self, chars):
+    def generate_image(self, chars: str) -> Image:
         """Generate the image of the given characters.
 
         :param chars: text to be generated.
         """
         background = random_color(238, 255)
         color = random_color(10, 200, random.randint(220, 255))
         im = self.create_captcha_image(chars, color, background)
         self.create_noise_dots(im, color)
         self.create_noise_curve(im, color)
-        im = im.filter(ImageFilter.SMOOTH)
+        im = im.filter(SMOOTH)
         return im
 
+    def generate(self, chars: str, format: str = 'png') -> BytesIO:
+        """Generate an Image Captcha of the given characters.
+
+        :param chars: text to be generated.
+        :param format: image file format
+        """
+        im = self.generate_image(chars)
+        out = BytesIO()
+        im.save(out, format=format)
+        out.seek(0)
+        return out
+
+    def write(self, chars: str, output: str, format: str = 'png') -> None:
+        """Generate and write an image CAPTCHA data to the output.
+
+        :param chars: text to be generated.
+        :param output: output destination.
+        :param format: image file format
+        """
+        im = self.generate_image(chars)
+        im.save(output, format=format)
+
 
-def random_color(start, end, opacity=None):
+def random_color(
+        start: int,
+        end: int,
+        opacity: t.Optional[int] = None) -> ColorTuple:
     red = random.randint(start, end)
     green = random.randint(start, end)
     blue = random.randint(start, end)
     if opacity is None:
         return (red, green, blue)
     return (red, green, blue, opacity)
```

