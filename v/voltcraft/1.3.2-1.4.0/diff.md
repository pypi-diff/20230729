# Comparing `tmp/voltcraft-1.3.2.tar.gz` & `tmp/voltcraft-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voltcraft-1.3.2.tar", last modified: Sat Jul  8 08:59:27 2023, max compression
+gzip compressed data, was "voltcraft-1.4.0.tar", last modified: Sat Jul 29 09:41:25 2023, max compression
```

## Comparing `voltcraft-1.3.2.tar` & `voltcraft-1.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:59:27.068759 voltcraft-1.3.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:59:27.064759 voltcraft-1.3.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-08 08:59:11.000000 voltcraft-1.3.2/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:59:27.064759 voltcraft-1.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-08 08:59:11.000000 voltcraft-1.3.2/.github/workflows/build_publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-08 08:59:11.000000 voltcraft-1.3.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-08 08:59:11.000000 voltcraft-1.3.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-08 08:59:11.000000 voltcraft-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-08 08:59:27.068759 voltcraft-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-08 08:59:11.000000 voltcraft-1.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-08 08:59:11.000000 voltcraft-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-08 08:59:27.068759 voltcraft-1.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:59:27.068759 voltcraft-1.3.2/voltcraft/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-08 08:59:11.000000 voltcraft-1.3.2/voltcraft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-08 08:59:27.000000 voltcraft-1.3.2/voltcraft/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-07-08 08:59:11.000000 voltcraft-1.3.2/voltcraft/pps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:59:27.068759 voltcraft-1.3.2/voltcraft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-08 08:59:27.000000 voltcraft-1.3.2/voltcraft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-08 08:59:27.000000 voltcraft-1.3.2/voltcraft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 08:59:27.000000 voltcraft-1.3.2/voltcraft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-08 08:59:27.000000 voltcraft-1.3.2/voltcraft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-08 08:59:27.000000 voltcraft-1.3.2/voltcraft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:41:25.057239 voltcraft-1.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:41:25.045239 voltcraft-1.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-29 09:41:13.000000 voltcraft-1.4.0/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:41:25.049239 voltcraft-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-29 09:41:13.000000 voltcraft-1.4.0/.github/workflows/build_publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-29 09:41:13.000000 voltcraft-1.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-29 09:41:13.000000 voltcraft-1.4.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-29 09:41:13.000000 voltcraft-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-29 09:41:25.057239 voltcraft-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-29 09:41:13.000000 voltcraft-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-29 09:41:13.000000 voltcraft-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-29 09:41:25.057239 voltcraft-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:41:25.053239 voltcraft-1.4.0/voltcraft/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-29 09:41:13.000000 voltcraft-1.4.0/voltcraft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-29 09:41:24.000000 voltcraft-1.4.0/voltcraft/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-07-29 09:41:13.000000 voltcraft-1.4.0/voltcraft/pps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:41:25.057239 voltcraft-1.4.0/voltcraft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-29 09:41:25.000000 voltcraft-1.4.0/voltcraft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-29 09:41:25.000000 voltcraft-1.4.0/voltcraft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 09:41:25.000000 voltcraft-1.4.0/voltcraft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-29 09:41:25.000000 voltcraft-1.4.0/voltcraft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-29 09:41:25.000000 voltcraft-1.4.0/voltcraft.egg-info/top_level.txt
```

### Comparing `voltcraft-1.3.2/.github/workflows/build_publish.yaml` & `voltcraft-1.4.0/.github/workflows/build_publish.yaml`

 * *Files identical despite different names*

### Comparing `voltcraft-1.3.2/.pre-commit-config.yaml` & `voltcraft-1.4.0/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -6,26 +6,26 @@
   - id: end-of-file-fixer
   - id: check-added-large-files
 - repo: https://github.com/pycqa/isort
   rev: 5.12.0
   hooks:
   - id: isort
 - repo: https://github.com/psf/black
-  rev: 23.3.0
+  rev: 23.7.0
   hooks:
   - id: black
-    language_version: python3
 - repo: https://github.com/pre-commit/mirrors-mypy
   rev: 'v1.4.1'
   hooks:
   - id: mypy
-    additional_dependencies: ["numpy"]
-    exclude: ^examples/
 - repo: https://github.com/PyCQA/flake8
   rev: '6.0.0'
   hooks:
   - id: flake8
     additional_dependencies:
-    - flake8-typing-imports==1.14.0
     - flake8-black==0.3.6
-    language_version: python3
     exclude: "^(build|docs|setup.py)|tests[/]"
+-   repo: https://github.com/asottile/pyupgrade
+    rev: v3.9.0
+    hooks:
+    - id: pyupgrade
+      args: [--py38-plus]
```

### Comparing `voltcraft-1.3.2/LICENSE.md` & `voltcraft-1.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `voltcraft-1.3.2/PKG-INFO` & `voltcraft-1.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: voltcraft
-Version: 1.3.2
+Version: 1.4.0
 Summary: library for controlling Voltcraft PPS power supplies
 Home-page: https://github.com/ap--/voltcraft.git
 Download-URL: https://github.com/ap--/voltcraft
 Author: Andreas Poehlmann
 Author-email: andreas@poehlmann.io
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # voltcraft.pps
 
 [![PyPI](https://img.shields.io/pypi/v/voltcraft)](https://pypi.org/project/voltcraft/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/voltcraft?label=pypi)](https://pypi.org/project/voltcraft/)
```

### Comparing `voltcraft-1.3.2/README.md` & `voltcraft-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `voltcraft-1.3.2/setup.cfg` & `voltcraft-1.4.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -11,33 +11,31 @@
 author = Andreas Poehlmann
 author_email = andreas@poehlmann.io
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python
-	Programming Language :: Python :: 2
 	Programming Language :: Python :: 3
 	Topic :: Scientific/Engineering
 	Topic :: Utilities
 	Operating System :: Microsoft :: Windows
 	Operating System :: POSIX
 	Operating System :: Unix
 	Operating System :: MacOS
 
 [options]
 packages = find:
 install_requires = 
 	pyserial
+python_requires = >=3.8
 
 [bdist_wheel]
 universal = 1
 
 [flake8]
 max-line-length = 88
-extend-ignore = 
-	E203,
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `voltcraft-1.3.2/voltcraft/pps.py` & `voltcraft-1.4.0/voltcraft/pps.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 """voltcraft.pps"""
+from __future__ import annotations
+
 import functools
 import sys
+from typing import Literal
 
 import serial
 
 # The model can be identified by the maximum voltage and maximum current.
 # But this is probably one of the weirdest naming-schemes I've seen...
 # It just doesn't really make sense...
 PPS_MODELS = {
@@ -18,24 +21,30 @@
     (32.2, 21.5): "DPPS3220",  # added tykling 2019-03-26
     (60.5, 11.0): "DPPS6010",
 }
 
 PPS_TIMEOUT = 1.00
 
 
-def _pps_debug(s, debug=True):
+def _pps_debug(s: str, debug: bool = True) -> None:
     """debug printing for PPS"""
     if debug:
         sys.stdout.write(s)
         sys.stdout.flush()
 
 
 # noinspection PyPep8Naming
-class PPS(object):
-    def __init__(self, port="/dev/ttyUSB0", reset=True, prom=None, debug=False):
+class PPS:
+    def __init__(
+        self,
+        port: str = "/dev/ttyUSB0",
+        reset: bool = True,
+        prom: int | None = None,
+        debug: bool = False,
+    ):
         """PPS(port, reset, prom)
 
         Parameters
         ----------
         port : str
             default '/dev/ttyUSB0'
         reset : bool
@@ -69,144 +78,149 @@
             )
 
         if bool(reset):
             self.output(0)
             self.voltage(0)
             self.current(0)
 
-        if not (prom is None):
+        if prom is not None:
             self.use_preset(prom)
 
     @property
-    def VMAX(self):
+    def VMAX(self) -> float:
         """maximum output voltage"""
         return self._vmax
 
     @property
-    def IMAX(self):
+    def IMAX(self) -> float:
         """maximum output current"""
         return self._imax
 
     @property
-    def MODEL(self):
+    def MODEL(self) -> str:
         """PS model number"""
         return self._model
 
     @property
-    def IMULT(self):
+    def IMULT(self) -> float:
         """current multiplier"""
         return self._imult
 
-    def _query(self, cmd):
+    def _query(self, cmd: str) -> str:
         """tx/rx to/from PS"""
         self._debug("PPS <- %s<CR>\n" % cmd)
         self._serial.write((cmd + "\r").encode())
-        b = []
+        b: list[bytes] = []
         self._debug("PPS -> ")
         while True:
             b.append(self._serial.read(1))
             self._debug(b[-1].replace(b"\r", b"<CR>").decode())
             if b[-1] in {b"", b"\x00"}:
                 raise serial.SerialTimeoutException()
             if b"".join(b[-3:]) == b"OK\r":
                 break
         self._debug("\n")
         return (b"".join(b[:-4])).decode()
 
-    def limits(self):
+    def limits(self) -> tuple[float, float]:
         """get maximum voltage and current from PS"""
         return self._vmax, self._imax
 
-    def output(self, state):
+    def output(self, state: int) -> None:
         """enable/disable the PS output"""
         state = 1 if not state else 0
         self._query("SOUT%d" % state)
 
-    def voltage(self, voltage):
+    def voltage(self, voltage: float) -> None:
         """set voltage: silently saturates at 0 and VMAX"""
         voltage = min(max(0, int(voltage * 10)), int(self._vmax * 10))
         self._query("VOLT%03d" % voltage)
 
-    def current(self, current):
+    def current(self, current: float) -> None:
         """set current: silently saturates at 0 and IMAX"""
         current = min(max(0, int(current * self._imult)), int(self._imax * self._imult))
         self._query("CURR%03d" % current)
 
-    def reading(self):
+    def reading(self) -> tuple[float, float, Literal["CC", "CV"]]:
         """read applied output voltage and current and if PS is in "CV" or "CC" mode"""
         getd = self._query("GETD")
         voltage = int(getd[0:4]) / 100.0
         current = int(getd[4:8]) / 100.0
-        mode = "CC" if int(getd[8]) else "CV"
+        mode: Literal["CC", "CV"] = "CC" if int(getd[8]) else "CV"
         return voltage, current, mode
 
-    def store_presets(self, VC0, VC1, VC2):
+    def store_presets(
+        self,
+        VC0: tuple[float, float],
+        VC1: tuple[float, float],
+        VC2: tuple[float, float],
+    ) -> None:
         """
         store preset value tuples (voltage, current)
         """
-        vcs = []
+        vcs: list[tuple[float, float]] = []
         for voltage, current in [VC0, VC1, VC2]:
             vcs.append(
                 (
                     min(max(0.0, voltage), self._vmax) * 10,
                     min(max(0.0, current), self._imax) * self._imult,
                 )
             )
         self._query("PROM%s" % "".join("%03d%03d" % s for s in vcs))
 
-    def load_presets(self):
+    def load_presets(self) -> list[tuple[float, float]]:
         """load preset value tuples (voltage, current)"""
         getm = self._query("GETM")
         v0 = int(getm[0:3]) / 10.0
         i0 = int(getm[3:6]) / self._imult
         v1 = int(getm[7:10]) / 10.0
         i1 = int(getm[10:13]) / self._imult
         v2 = int(getm[14:17]) / 10.0
         i2 = int(getm[17:20]) / self._imult
         return [(v0, i0), (v1, i1), (v2, i2)]
 
-    def use_preset(self, nbr):
+    def use_preset(self, nbr: int) -> None:
         """use specified preset"""
         nbr = min(max(0, int(nbr)), 2)
         self._query("RUNM%d" % nbr)
 
     @property
-    def preset(self):
+    def preset(self) -> tuple[float, float]:
         """preset values: (voltage, current)"""
         gets = self._query("GETS")
         voltage = int(gets[0:3]) / 10.0
         current = int(gets[3:6]) / self._imult
         return voltage, current
 
     @preset.setter
-    def preset(self, VC):
+    def preset(self, VC: tuple[float, float]) -> None:
         self.preset_voltage = VC[0]
         self.preset_current = VC[1]
 
     @property
-    def preset_voltage(self):
+    def preset_voltage(self) -> float:
         """preset voltage"""
         govp = self._query("GOVP")
         voltage = int(govp[0:3]) / 10.0
         return voltage
 
     @preset_voltage.setter
-    def preset_voltage(self, voltage):
+    def preset_voltage(self, voltage: float) -> None:
         voltage = min(max(0.0, float(voltage)), self._vmax) * 10
         self._query("SOVP%03d" % int(voltage))
 
     @property
-    def preset_current(self):
+    def preset_current(self) -> float:
         """preset current"""
         gocp = self._query("GOCP")
         current = int(gocp[0:3]) / self._imult
         return current
 
     @preset_current.setter
-    def preset_current(self, current):
+    def preset_current(self, current: float) -> None:
         current = min(max(0.0, float(current)), self._imax) * self._imult
         self._query("SOCP%03d" % int(current))
 
-    def power_dissipation(self):
+    def power_dissipation(self) -> float:
         """return current power dissipation"""
         voltage, current, _ = self.reading()
         return voltage * current
```

### Comparing `voltcraft-1.3.2/voltcraft.egg-info/PKG-INFO` & `voltcraft-1.4.0/voltcraft.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: voltcraft
-Version: 1.3.2
+Version: 1.4.0
 Summary: library for controlling Voltcraft PPS power supplies
 Home-page: https://github.com/ap--/voltcraft.git
 Download-URL: https://github.com/ap--/voltcraft
 Author: Andreas Poehlmann
 Author-email: andreas@poehlmann.io
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # voltcraft.pps
 
 [![PyPI](https://img.shields.io/pypi/v/voltcraft)](https://pypi.org/project/voltcraft/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/voltcraft?label=pypi)](https://pypi.org/project/voltcraft/)
```

