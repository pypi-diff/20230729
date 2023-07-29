# Comparing `tmp/tvolib-0.3.0.tar.gz` & `tmp/tvolib-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvolib-0.3.0.tar", max compression
+gzip compressed data, was "tvolib-0.4.0.tar", max compression
```

## Comparing `tvolib-0.3.0.tar` & `tvolib-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0    35149 2023-07-21 18:31:00.565627 tvolib-0.3.0/LICENSE
--rw-r--r--   0        0        0      307 2023-07-25 22:43:23.561333 tvolib-0.3.0/README.md
--rw-r--r--   0        0        0      714 2023-07-26 17:38:44.501523 tvolib-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       63 2023-07-26 17:38:14.079542 tvolib-0.3.0/src/tvolib/__init__.py
--rw-r--r--   0        0        0       61 2023-07-26 17:37:54.763558 tvolib-0.3.0/src/tvolib/models/__init__.py
--rw-r--r--   0        0        0     6085 2023-07-26 17:38:07.348547 tvolib-0.3.0/src/tvolib/models/lin10_magnetopause_model.py
--rw-r--r--   0        0        0      219 2023-07-25 19:48:55.445686 tvolib-0.3.0/src/tvolib/mpl_utils/__init__.py
--rw-r--r--   0        0        0     2103 2023-07-25 19:51:46.873557 tvolib-0.3.0/src/tvolib/mpl_utils/_draw.py
--rw-r--r--   0        0        0      526 2023-07-25 19:42:33.293735 tvolib-0.3.0/src/tvolib/mpl_utils/_format.py
--rw-r--r--   0        0        0      898 2023-07-25 19:48:29.873412 tvolib-0.3.0/src/tvolib/mpl_utils/_setup.py
--rw-r--r--   0        0        0    25742 2023-07-21 17:47:40.083899 tvolib-0.3.0/src/tvolib/mpl_utils/data/mpl_utils.mplstyle
--rw-r--r--   0        0        0      139 2023-07-26 05:27:27.100229 tvolib-0.3.0/src/tvolib/numeric/__init__.py
--rw-r--r--   0        0        0     1724 2023-07-26 00:08:22.418224 tvolib-0.3.0/src/tvolib/numeric/interpolate.py
--rw-r--r--   0        0        0     1488 2023-07-25 22:45:58.568398 tvolib-0.3.0/src/tvolib/numeric/moving.py
--rw-r--r--   0        0        0      572 2023-07-25 23:04:48.648666 tvolib-0.3.0/src/tvolib/numeric/timing.py
--rw-r--r--   0        0        0     1201 1970-01-01 00:00:00.000000 tvolib-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-21 18:31:00.565627 tvolib-0.4.0/LICENSE
+-rw-r--r--   0        0        0      398 2023-07-29 16:28:47.019683 tvolib-0.4.0/README.md
+-rw-r--r--   0        0        0      817 2023-07-29 16:26:42.944720 tvolib-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-07-29 16:27:19.159149 tvolib-0.4.0/src/tvolib/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 16:31:40.262695 tvolib-0.4.0/src/tvolib/models/__init__.py
+-rw-r--r--   0        0        0     6416 2023-07-29 16:32:46.269053 tvolib-0.4.0/src/tvolib/models/magnetopause_model.py
+-rw-r--r--   0        0        0      219 2023-07-29 16:27:19.169149 tvolib-0.4.0/src/tvolib/mpl_utils/__init__.py
+-rw-r--r--   0        0        0     2067 2023-07-29 16:27:20.045184 tvolib-0.4.0/src/tvolib/mpl_utils/_draw.py
+-rw-r--r--   0        0        0      526 2023-07-25 19:42:33.293735 tvolib-0.4.0/src/tvolib/mpl_utils/_format.py
+-rw-r--r--   0        0        0      899 2023-07-29 16:27:19.165149 tvolib-0.4.0/src/tvolib/mpl_utils/_setup.py
+-rw-r--r--   0        0        0    25742 2023-07-21 17:47:40.083899 tvolib-0.4.0/src/tvolib/mpl_utils/data/mpl_utils.mplstyle
+-rw-r--r--   0        0        0      174 2023-07-29 16:49:47.120339 tvolib-0.4.0/src/tvolib/numeric/__init__.py
+-rw-r--r--   0        0        0     1463 2023-07-29 16:49:26.036785 tvolib-0.4.0/src/tvolib/numeric/curlometer.py
+-rw-r--r--   0        0        0     2318 2023-07-29 16:38:52.332070 tvolib-0.4.0/src/tvolib/numeric/interpolate.py
+-rw-r--r--   0        0        0     2455 2023-07-29 16:42:20.822532 tvolib-0.4.0/src/tvolib/numeric/moving.py
+-rw-r--r--   0        0        0      572 2023-07-25 23:04:48.648666 tvolib-0.4.0/src/tvolib/numeric/timing.py
+-rw-r--r--   0        0        0     1292 1970-01-01 00:00:00.000000 tvolib-0.4.0/PKG-INFO
```

### Comparing `tvolib-0.3.0/LICENSE` & `tvolib-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tvolib-0.3.0/pyproject.toml` & `tvolib-0.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tvolib"
-version = "0.3.0"
+version = "0.4.0"
 description = "A personal collection of Python and IDL research tools in Space Plasma Physics."
 authors = ["Tien Vo <tien.a.vo@proton.me>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 packages = [
     { include = "tvolib", from = "src" }
 ]
@@ -18,11 +18,18 @@
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
 matplotlib = "*"
 numpy = "*"
 astropy = "*"
 scipy = "*"
 
+[tool.poetry.group.dev]
+optional = true
+
+[tool.poetry.group.dev.dependencies]
+black = "*"
+isort = "*"
+
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tvolib-0.3.0/src/tvolib/models/lin10_magnetopause_model.py` & `tvolib-0.4.0/src/tvolib/models/magnetopause_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-r"""3D asymmetric magnetopause model. For references consult
-    Lin+ (2010), "A three-dimensional asymmetric magnetopause model", JGR-SP, doi:10.1029/2009JA014235
-"""
-
 __all__ = ["Lin10MagnetopauseModel"]
 
 import numpy as np
 from scipy.interpolate import UnivariateSpline
 
 
 class Lin10MagnetopauseModel:
-    # Fit coefficients (see Table 9)
+    r"""
+    3D asymmetric magnetopause model. For references consult
+    Lin+ (2010), "A three-dimensional asymmetric magnetopause model",
+    JGR-Space Physics, doi:10.1029/2009JA014235
+    """
+
+    # Fit coefficients (see Table 9 in reference)
     a = np.zeros(22, dtype=np.float32)
     a[0] = 12.544
     a[1] = -0.194
     a[2] = 0.305
     a[3] = 0.0573
     a[4] = 2.178
     a[5] = 0.0571
@@ -32,64 +34,83 @@
     a[18] = -5.328
     a[19] = 1.103
     a[20] = -0.907
     a[21] = 1.450
 
     def __init__(self, pressure, bfield, tilt_angle):
         r"""
-        ----------
+
         Parameters
         ----------
         pressure: nPa
-            Total (dynamic and magnetic) solar wind pressure.
+            Total (dynamic and magnetic) solar wind pressure
         bfield: nT
-            z coordinate of the interplanetary magnetic field.
+            z coordinate of the interplanetary magnetic field
         tilt_angle: rad
-            Dipole tilt angle.
+            Dipole tilt angle
         """
 
         # Save
         self._P = pressure
         self._Bz = bfield
         self._phi = tilt_angle
 
         # Calculate other coefficients
         self.construct_model()
 
     def construct_model(self):
-        r"""Calculate the coefficients in eq. (20) and r(theta, varphi) in eq. (19)"""
+        r"""
+        Calculate the coefficients in eq. (20) and r(theta, varphi)
+        in eq. (19)
+        """
         # Unpack
         a = self.a
         P = self._P
         Bz = self._Bz
         phi = self._phi
 
         # Auxilliary coefficients
-        r0 = (a[0] * (P ** a[1]) * (1 + a[2] * (np.exp(a[3] * Bz) - 1) / (np.exp(a[4] * Bz) + 1)))
+        r0 = (
+            a[0]
+            * (P ** a[1])
+            * (1 + a[2] * (np.exp(a[3] * Bz) - 1) / (np.exp(a[4] * Bz) + 1))
+        )
         b0 = a[6] + a[7] * (np.exp(a[8] * Bz) - 1) / (np.exp(a[9] * Bz) + 1)
         b1 = a[10]
         b2 = a[11] + a[12] * phi
         b3 = a[13]
         cn = cs = a[14] * (P ** a[15])
         dn = a[16] + a[17] * phi + a[18] * (phi**2)
         ds = a[16] - a[17] * phi + a[18] * (phi**2)
         en = es = a[21]
         tn = a[19] + a[20] * phi
         ts = a[19] - a[20] * phi
 
         # Auxilliary functions
         def psi_n(varphi, theta):
-            return np.arccos(np.cos(theta) * np.cos(tn) + np.sin(theta) * np.sin(tn) * np.cos(varphi - np.pi / 2))
+            return np.arccos(
+                np.cos(theta) * np.cos(tn)
+                + np.sin(theta) * np.sin(tn) * np.cos(varphi - np.pi / 2)
+            )
 
         def psi_s(varphi, theta):
-            return np.arccos(np.cos(theta) * np.cos(ts) + np.sin(theta) * np.sin(ts) * np.cos(varphi - 3 * np.pi / 2))
+            return np.arccos(
+                np.cos(theta) * np.cos(ts)
+                + np.sin(theta) * np.sin(ts) * np.cos(varphi - 3 * np.pi / 2)
+            )
 
         def f(varphi, theta):
-            return (np.cos(theta / 2) + a[5] * np.sin(theta * 2) * (1 - np.exp(-theta))) ** (
-                b0 + b1 * np.cos(varphi) + b2 * np.sin(varphi) + b3 * (np.sin(varphi) ** 2)
+            return (
+                np.cos(theta / 2)
+                + a[5] * np.sin(theta * 2) * (1 - np.exp(-theta))
+            ) ** (
+                b0
+                + b1 * np.cos(varphi)
+                + b2 * np.sin(varphi)
+                + b3 * (np.sin(varphi) ** 2)
             )
 
         # Radial function
         def r(varphi, theta):
             return (
                 r0 * f(varphi, theta)
                 + cn * np.exp(dn * (psi_n(varphi, theta) ** en))
@@ -151,15 +172,17 @@
         else:
             raise NotImplementedError
 
         idx = np.argsort(T)
         return UnivariateSpline(T[idx], R[idx], s=0)
 
     def add_mpause_model(self, ax, which="XY", rotation_angle=0, **kw):
-        ax.plot(*self.shape_N(which=which, rotation_angle=rotation_angle), **kw)
+        ax.plot(
+            *self.shape_N(which=which, rotation_angle=rotation_angle), **kw
+        )
 
     @property
     def pressure(self):
         return self._P
 
     @property
     def bfield(self):
@@ -179,24 +202,25 @@
 
     @tilt_angle.setter
     def tilt_angle(self, new_tilt_angle):
         self._phi = new_tilt_angle
 
 
 if __name__ == "__main__":
-    import matplotlib.pyplot as plt
+    from tvolib import mpl_utils as mu
 
     model = Lin10MagnetopauseModel(pressure=1, bfield=0, tilt_angle=0)
     X_gsm, Y_gsm = model.shape_N(which="XY")
     T = np.linspace(-np.pi, np.pi, 1000)
     f = model.shape_F(which="XY", rotation_angle=np.radians(0))
     R = f(T)
 
-    fig, ax = plt.subplots(1, 1)
+    fig, ax = mu.plt.subplots(1, 1)
 
+    mu.draw_earth(ax)
     ax.plot(X_gsm, Y_gsm, "-k")
     ax.plot(R * np.cos(T), R * np.sin(T), "--r")
     ax.set_xlim(-40, 20)
     ax.set_ylim(-35, 35)
     ax.set_aspect("equal")
 
-    plt.show()
+    mu.plt.show()
```

### Comparing `tvolib-0.3.0/src/tvolib/mpl_utils/_draw.py` & `tvolib-0.4.0/src/tvolib/mpl_utils/_draw.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,20 @@
     "draw_arrows",
     "draw_earth",
     "draw_multicolored_line",
 ]
 
 import numpy as np
 from matplotlib.collections import LineCollection
-from matplotlib.patches import FancyArrowPatch
 from matplotlib.colors import Normalize
+from matplotlib.patches import FancyArrowPatch
 
 
 def draw_arrows(axis, x, y, N=None, color="k"):
-    r"""Draws arrows along a path on the axis
-    """
+    r"""Draws arrows along a path on the axis"""
     N = len(x) // 5 if N is None else N
     d = len(x) // (N + 1)
 
     idx = np.arange(d, len(x), d)
     for i in idx:
         ar = FancyArrowPatch(
             (x[i - 1], y[i - 1]),
@@ -25,16 +24,15 @@
             mutation_scale=20,
             color=color,
         )
         axis.add_patch(ar)
 
 
 def draw_earth(axis, R=1, N=50, zorder=999):
-    r"""Draws the Earth on the axis (with shading indicating day/night)
-    """
+    r"""Draws the Earth on the axis (with shading indicating day/night)"""
     # Nightside
     theta = np.linspace(np.pi / 2, 3 * np.pi / 2, N)
     Xn = R * np.cos(theta)
     Yn = R * np.sin(theta)
     Xn = np.append(Xn, Xn[0])
     Yn = np.append(Yn, Yn[0])
     # Dayside
@@ -46,18 +44,18 @@
     # Plot
     axis.plot(Xd, Yd, "-k", zorder=zorder)
     axis.plot(Xn, Yn, "-k", zorder=zorder)
     axis.fill(Xd, Yd, color="w")
     axis.fill(Xn, Yn, color="k")
 
 
-def draw_multicolored_line(axis, x, y, c, cmap="jet",
-                           vmin=None, vmax=None, set_lim=False, **kwargs):
-    r"""Draws a line with colors on a scale determined by c
-    """
+def draw_multicolored_line(
+    axis, x, y, c, cmap="jet", vmin=None, vmax=None, set_lim=False, **kwargs
+):
+    r"""Draws a line with colors on a scale determined by c"""
 
     vmin = c.min() if vmin is None else vmin
     vmax = c.max() if vmax is None else vmax
 
     points = np.array([x, y]).T.reshape(-1, 1, 2)
     segments = np.concatenate([points[:-1], points[1:]], axis=1)
     norm = Normalize(vmin, vmax)
```

### Comparing `tvolib-0.3.0/src/tvolib/mpl_utils/_format.py` & `tvolib-0.4.0/src/tvolib/mpl_utils/_format.py`

 * *Files identical despite different names*

### Comparing `tvolib-0.3.0/src/tvolib/mpl_utils/_setup.py` & `tvolib-0.4.0/src/tvolib/mpl_utils/_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 __all__ = ["setup"]
 
-import tempfile
 import atexit
-import shutil
 import os
-import matplotlib.pyplot as plt
-import matplotlib as mpl
+import shutil
+import tempfile
 from importlib.resources import files
 
+import matplotlib as mpl
+import matplotlib.pyplot as plt
+
 
 def _checkdep_usetex(s):
     return s and shutil.which("tex")
 
 
 def setup(tex=False, cache=False, **kw):
     plt.style.use(files("tvolib.mpl_utils") / "data" / "mpl_utils.mplstyle")
```

### Comparing `tvolib-0.3.0/src/tvolib/mpl_utils/data/mpl_utils.mplstyle` & `tvolib-0.4.0/src/tvolib/mpl_utils/data/mpl_utils.mplstyle`

 * *Files identical despite different names*

### Comparing `tvolib-0.3.0/src/tvolib/numeric/interpolate.py` & `tvolib-0.4.0/src/tvolib/numeric/interpolate.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,43 @@
 __all__ = ["interpol"]
 
 import astropy.units as u
 import numpy as np
 from scipy.interpolate import interp1d
-from .timing import sampling_period
+
 from .moving import move_avg
+from .timing import sampling_period
 
 
 def interpol(y, x, xout, window=None, kind="linear"):
     r"""Interpolate a signal onto a new temporal grid.
 
     This function mimics IDL's interpol routine. When downsampling, the
     window argument can be set to apply a moving average over the
     original temporal grid. Additionally, astropy.Quantity are preserved
     from this function.
+
+    Parameters
+    ----------
+    y: array_like, shape (N, ...)
+        Signal to interpolate, first axis is implicitly time (N)
+    x: datetime64 array, shape (N,)
+        Time corresponding to the signal `y`
+    xout: datetime64 array, shape (M,)
+        Output time to interpolate on
+    window: "box", "gauss"
+        Type of window if applying a moving average on `y` before
+            interpolating is desired
+    kind: "linear", "cubic", etc
+        See scipy.interpolate.interp1d documentation.
+
+    Return
+    ------
+    yout: array_like, shape (M, ...)
+        Interpolated signal
     """
 
     if not (
         (
             np.issubdtype(x.dtype, np.datetime64)
             and np.issubdtype(xout.dtype, np.datetime64)
         )
```

### Comparing `tvolib-0.3.0/src/tvolib/numeric/timing.py` & `tvolib-0.4.0/src/tvolib/numeric/timing.py`

 * *Files identical despite different names*

### Comparing `tvolib-0.3.0/PKG-INFO` & `tvolib-0.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvolib
-Version: 0.3.0
+Version: 0.4.0
 Summary: A personal collection of Python and IDL research tools in Space Plasma Physics.
 Home-page: https://github.com/tien-vo/tvolib
 License: GPL-3.0-or-later
 Author: Tien Vo
 Author-email: tien.a.vo@proton.me
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -25,12 +25,18 @@
 
 This is a personal collection of Python and IDL routines for my research
 in Space Plasma Physics, organized into packages. Some are more
 well-documented than others. Please use them at your discretion.
 
 ## Installation
 
-Ensure `micromamba` is recognized in PATH. Then just run
+The Python codes are published on PyPI. For installation run
 ```
-make install
+pip install tvolib
 ```
 
+To use the IDL code, run
+```
+source idlrc
+```
+to put `src/idl` into `IDL_PATH`.
+
```

