# Comparing `tmp/rateslib-0.3.0.tar.gz` & `tmp/rateslib-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rateslib-0.3.0.tar", last modified: Sat Jul 29 05:10:27 2023, max compression
+gzip compressed data, was "rateslib-0.3.1.tar", last modified: Sat Jul 29 08:26:01 2023, max compression
```

## Comparing `rateslib-0.3.0.tar` & `rateslib-0.3.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2023-07-29 05:10:27.082456 rateslib-0.3.0/
--rw-r--r--   0 Darbyshire   (501) staff       (20)    19126 2022-10-15 05:18:28.000000 rateslib-0.3.0/LICENSE
--rw-r--r--   0 Darbyshire   (501) staff       (20)    23901 2023-07-29 05:10:27.081979 rateslib-0.3.0/PKG-INFO
--rw-r--r--   0 Darbyshire   (501) staff       (20)     1186 2023-04-24 18:38:25.000000 rateslib-0.3.0/README.md
--rw-r--r--   0 Darbyshire   (501) staff       (20)      779 2023-07-29 05:05:23.000000 rateslib-0.3.0/pyproject.toml
-drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2023-07-29 05:10:27.016683 rateslib-0.3.0/rateslib/
--rw-r--r--   0 Darbyshire   (501) staff       (20)     4780 2023-07-28 22:06:51.000000 rateslib-0.3.0/rateslib/__init__.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)     2763 2023-07-27 17:04:54.000000 rateslib-0.3.0/rateslib/_swaptions.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    23379 2023-07-27 17:04:54.000000 rateslib-0.3.0/rateslib/calendars.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    87883 2023-07-27 17:04:54.000000 rateslib-0.3.0/rateslib/curves.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)     3965 2023-07-27 17:04:54.000000 rateslib-0.3.0/rateslib/default.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    26483 2023-07-27 17:04:54.000000 rateslib-0.3.0/rateslib/dual.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    65656 2023-05-26 18:54:31.000000 rateslib-0.3.0/rateslib/fx.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)   287187 2023-07-27 17:04:54.000000 rateslib-0.3.0/rateslib/instruments.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    95396 2023-07-29 04:57:38.000000 rateslib-0.3.0/rateslib/legs.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    76258 2023-07-27 17:04:54.000000 rateslib-0.3.0/rateslib/periods.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    49424 2023-07-27 17:04:54.000000 rateslib-0.3.0/rateslib/scheduling.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    71411 2023-07-27 17:04:54.000000 rateslib-0.3.0/rateslib/solver.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    17008 2023-05-15 17:34:14.000000 rateslib-0.3.0/rateslib/splines.py
-drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2023-07-29 05:10:27.025196 rateslib-0.3.0/rateslib.egg-info/
--rw-r--r--   0 Darbyshire   (501) staff       (20)    23901 2023-07-29 05:10:26.000000 rateslib-0.3.0/rateslib.egg-info/PKG-INFO
--rw-r--r--   0 Darbyshire   (501) staff       (20)      676 2023-07-29 05:10:26.000000 rateslib-0.3.0/rateslib.egg-info/SOURCES.txt
--rw-r--r--   0 Darbyshire   (501) staff       (20)        1 2023-07-29 05:10:26.000000 rateslib-0.3.0/rateslib.egg-info/dependency_links.txt
--rw-r--r--   0 Darbyshire   (501) staff       (20)      129 2023-07-29 05:10:26.000000 rateslib-0.3.0/rateslib.egg-info/requires.txt
--rw-r--r--   0 Darbyshire   (501) staff       (20)        9 2023-07-29 05:10:26.000000 rateslib-0.3.0/rateslib.egg-info/top_level.txt
--rw-r--r--   0 Darbyshire   (501) staff       (20)       38 2023-07-29 05:10:27.082548 rateslib-0.3.0/setup.cfg
--rw-r--r--   0 Darbyshire   (501) staff       (20)       37 2022-08-28 05:42:04.000000 rateslib-0.3.0/setup.py
-drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2023-07-29 05:10:27.080343 rateslib-0.3.0/tests/
--rw-r--r--   0 Darbyshire   (501) staff       (20)     8293 2023-07-27 17:04:54.000000 rateslib-0.3.0/tests/test_calendars.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    39559 2023-07-27 17:04:54.000000 rateslib-0.3.0/tests/test_curves.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    23278 2023-05-22 18:47:00.000000 rateslib-0.3.0/tests/test_dual.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    28890 2023-07-27 17:04:54.000000 rateslib-0.3.0/tests/test_fx.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)   118294 2023-07-27 17:04:54.000000 rateslib-0.3.0/tests/test_instruments.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    47895 2023-07-27 17:04:54.000000 rateslib-0.3.0/tests/test_legs.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    47058 2023-07-27 17:04:54.000000 rateslib-0.3.0/tests/test_periods.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    27914 2023-07-27 17:04:54.000000 rateslib-0.3.0/tests/test_scheduling.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    46380 2023-07-27 17:04:54.000000 rateslib-0.3.0/tests/test_solver.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)     5430 2023-03-29 17:12:48.000000 rateslib-0.3.0/tests/test_splines.py
+drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2023-07-29 08:26:01.159696 rateslib-0.3.1/
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    19126 2022-10-15 05:18:28.000000 rateslib-0.3.1/LICENSE
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    23901 2023-07-29 08:26:01.159180 rateslib-0.3.1/PKG-INFO
+-rw-r--r--   0 Darbyshire   (501) staff       (20)     1186 2023-04-24 18:38:25.000000 rateslib-0.3.1/README.md
+-rw-r--r--   0 Darbyshire   (501) staff       (20)      779 2023-07-29 08:23:09.000000 rateslib-0.3.1/pyproject.toml
+drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2023-07-29 08:26:01.041536 rateslib-0.3.1/rateslib/
+-rw-r--r--   0 Darbyshire   (501) staff       (20)     4780 2023-07-28 22:06:51.000000 rateslib-0.3.1/rateslib/__init__.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)     2763 2023-07-27 17:04:54.000000 rateslib-0.3.1/rateslib/_swaptions.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    23379 2023-07-27 17:04:54.000000 rateslib-0.3.1/rateslib/calendars.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    89015 2023-07-29 07:30:23.000000 rateslib-0.3.1/rateslib/curves.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)     3965 2023-07-27 17:04:54.000000 rateslib-0.3.1/rateslib/default.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    26483 2023-07-27 17:04:54.000000 rateslib-0.3.1/rateslib/dual.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    65656 2023-05-26 18:54:31.000000 rateslib-0.3.1/rateslib/fx.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)   287187 2023-07-27 17:04:54.000000 rateslib-0.3.1/rateslib/instruments.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    95396 2023-07-29 06:11:43.000000 rateslib-0.3.1/rateslib/legs.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    76479 2023-07-29 07:30:23.000000 rateslib-0.3.1/rateslib/periods.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    49424 2023-07-27 17:04:54.000000 rateslib-0.3.1/rateslib/scheduling.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    71532 2023-07-29 06:11:43.000000 rateslib-0.3.1/rateslib/solver.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    17008 2023-05-15 17:34:14.000000 rateslib-0.3.1/rateslib/splines.py
+drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2023-07-29 08:26:01.053516 rateslib-0.3.1/rateslib.egg-info/
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    23901 2023-07-29 08:26:00.000000 rateslib-0.3.1/rateslib.egg-info/PKG-INFO
+-rw-r--r--   0 Darbyshire   (501) staff       (20)      676 2023-07-29 08:26:00.000000 rateslib-0.3.1/rateslib.egg-info/SOURCES.txt
+-rw-r--r--   0 Darbyshire   (501) staff       (20)        1 2023-07-29 08:26:00.000000 rateslib-0.3.1/rateslib.egg-info/dependency_links.txt
+-rw-r--r--   0 Darbyshire   (501) staff       (20)      129 2023-07-29 08:26:00.000000 rateslib-0.3.1/rateslib.egg-info/requires.txt
+-rw-r--r--   0 Darbyshire   (501) staff       (20)        9 2023-07-29 08:26:00.000000 rateslib-0.3.1/rateslib.egg-info/top_level.txt
+-rw-r--r--   0 Darbyshire   (501) staff       (20)       38 2023-07-29 08:26:01.159766 rateslib-0.3.1/setup.cfg
+-rw-r--r--   0 Darbyshire   (501) staff       (20)       37 2022-08-28 05:42:04.000000 rateslib-0.3.1/setup.py
+drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2023-07-29 08:26:01.145947 rateslib-0.3.1/tests/
+-rw-r--r--   0 Darbyshire   (501) staff       (20)     8293 2023-07-27 17:04:54.000000 rateslib-0.3.1/tests/test_calendars.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    39559 2023-07-27 17:04:54.000000 rateslib-0.3.1/tests/test_curves.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    23826 2023-07-29 06:11:43.000000 rateslib-0.3.1/tests/test_dual.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    28890 2023-07-27 17:04:54.000000 rateslib-0.3.1/tests/test_fx.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)   118294 2023-07-27 17:04:54.000000 rateslib-0.3.1/tests/test_instruments.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    47895 2023-07-27 17:04:54.000000 rateslib-0.3.1/tests/test_legs.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    48443 2023-07-29 07:30:23.000000 rateslib-0.3.1/tests/test_periods.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    27914 2023-07-27 17:04:54.000000 rateslib-0.3.1/tests/test_scheduling.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    46380 2023-07-27 17:04:54.000000 rateslib-0.3.1/tests/test_solver.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)     5430 2023-03-29 17:12:48.000000 rateslib-0.3.1/tests/test_splines.py
```

### Comparing `rateslib-0.3.0/LICENSE` & `rateslib-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rateslib-0.3.0/PKG-INFO` & `rateslib-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rateslib
-Version: 0.3.0
+Version: 0.3.1
 Summary: A fixed income library for trading interest rates
 Author: J H M Darbyshire
 License: Attribution-NonCommercial-NoDerivatives 4.0 International
         
         =======================================================================
         
         Creative Commons Corporation ("Creative Commons") is not a law firm and
```

### Comparing `rateslib-0.3.0/README.md` & `rateslib-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `rateslib-0.3.0/pyproject.toml` & `rateslib-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rateslib"
-version = "0.3.0"
+version = "0.3.1"
 description = "A fixed income library for trading interest rates"
 readme = "README.md"
 authors = [{ name = "J H M Darbyshire"}]
 license = { file = "LICENSE" }
 keywords = ["interest rate", "derivatives", "swaps", "bonds", "fixed income"]
 dependencies = [
     "numpy>=1.21.5",
```

### Comparing `rateslib-0.3.0/rateslib/__init__.py` & `rateslib-0.3.1/rateslib/__init__.py`

 * *Files identical despite different names*

### Comparing `rateslib-0.3.0/rateslib/_swaptions.py` & `rateslib-0.3.1/rateslib/_swaptions.py`

 * *Files identical despite different names*

### Comparing `rateslib-0.3.0/rateslib/calendars.py` & `rateslib-0.3.1/rateslib/calendars.py`

 * *Files identical despite different names*

### Comparing `rateslib-0.3.0/rateslib/curves.py` & `rateslib-0.3.1/rateslib/curves.py`

 * *Files 2% similar despite different names*

```diff
@@ -2164,14 +2164,41 @@
 
         Returns
         -------
         CompositeCurve
         """
         return CompositeCurve(curves=[curve.roll(tenor) for curve in self.curves])
 
+    def index_value(self, date: datetime, interpolation: str = "daily"):
+        """
+        Calculate the accrued value of the index from the ``index_base``.
+
+        See :meth:`IndexCurve.index_value()<rateslib.curves.IndexCurve.index_value>`
+        """
+        # TODO: DRY inherit this method from IndexCurve.index_value.
+        if not isinstance(self.curves[0], IndexCurve):
+            raise TypeError("`index_value` not available on non `IndexCurve` types.")
+
+        if interpolation.lower() == "daily":
+            date_ = date
+        elif interpolation.lower() == "monthly":
+            date_ = datetime(date.year, date.month, 1)
+        else:
+            raise ValueError(
+                "`interpolation` for `index_value` must be in {'daily', 'monthly'}."
+            )
+        if date_ < self.node_dates[0]:
+            return 0.0
+            # return zero for index dates in the past
+            # the proper way for instruments to deal with this is to supply i_fixings
+        elif date_ == self.node_dates[0]:
+            return self.index_base
+        else:
+            return self.index_base * 1 / self[date_]
+
 
 def average_rate(effective, termination, convention, rate):
     """
     Return the geometric, 1 calendar day, average rate for the rate in a period.
 
     This is used for approximations usually in combination with floating periods.
```

### Comparing `rateslib-0.3.0/rateslib/default.py` & `rateslib-0.3.1/rateslib/default.py`

 * *Files identical despite different names*

### Comparing `rateslib-0.3.0/rateslib/dual.py` & `rateslib-0.3.1/rateslib/dual.py`

 * *Files identical despite different names*

### Comparing `rateslib-0.3.0/rateslib/fx.py` & `rateslib-0.3.1/rateslib/fx.py`

 * *Files identical despite different names*

### Comparing `rateslib-0.3.0/rateslib/instruments.py` & `rateslib-0.3.1/rateslib/instruments.py`

 * *Files identical despite different names*

### Comparing `rateslib-0.3.0/rateslib/legs.py` & `rateslib-0.3.1/rateslib/legs.py`

 * *Files identical despite different names*

### Comparing `rateslib-0.3.0/rateslib/periods.py` & `rateslib-0.3.1/rateslib/periods.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 import numpy as np
 from pandas.tseries.offsets import CustomBusinessDay
 from pandas import DataFrame, date_range, Series, NA, isna
 
 from rateslib import defaults
 from rateslib.calendars import add_tenor, get_calendar, dcf, _get_eom
-from rateslib.curves import Curve, LineCurve, IndexCurve, average_rate
+from rateslib.curves import Curve, LineCurve, IndexCurve, average_rate, CompositeCurve
 from rateslib.dual import Dual, Dual2, DualTypes
 from rateslib.fx import FXForwards, FXRates
 
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
@@ -1723,15 +1723,21 @@
         i_date: datetime,
         i_curve: Optional[IndexCurve],
         i_lag: int,
         i_method: str,
     ) -> Optional[DualTypes]:
         if i_curve is None:
             return None
-        elif not isinstance(i_curve, IndexCurve):
+        elif (
+            not isinstance(i_curve, IndexCurve)
+            and not isinstance(i_curve, CompositeCurve)
+        ) or (
+            isinstance(i_curve, CompositeCurve)
+            and not isinstance(i_curve.curves[0], IndexCurve)
+        ):
             raise TypeError("`index_value` must be forecast from an `IndexCurve`.")
         elif i_lag != i_curve.index_lag:
             return None  # TODO decide if RolledCurve to correct index lag be attemoted
         else:
             return i_curve.index_value(i_date, i_method)
 
     @staticmethod
```

### Comparing `rateslib-0.3.0/rateslib/scheduling.py` & `rateslib-0.3.1/rateslib/scheduling.py`

 * *Files identical despite different names*

### Comparing `rateslib-0.3.0/rateslib/solver.py` & `rateslib-0.3.1/rateslib/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1709,15 +1709,18 @@
         idx_tuples = [c + l for c in all_keys for l in inst_keys + fx_keys]
         ridx = MultiIndex.from_tuples(
             [key for key in idx_tuples],
             names=["local_ccy", "display_ccy", "type", "solver", "label"],
         )
         if base is not None:
             ridx = ridx.append(
-                MultiIndex.from_tuples([("all", base) + l for l in inst_keys + fx_keys])
+                MultiIndex.from_tuples(
+                    [("all", base) + l for l in inst_keys + fx_keys],
+                    names=["local_ccy", "display_ccy", "type", "solver", "label"]
+                )
             )
         cidx = MultiIndex.from_tuples(
             [l for l in inst_keys + fx_keys], names=["type", "solver", "label"]
         )
         df = DataFrame(None, index=ridx, columns=cidx)
         for key, d in container.items():
             array = np.block(
```

### Comparing `rateslib-0.3.0/rateslib/splines.py` & `rateslib-0.3.1/rateslib/splines.py`

 * *Files identical despite different names*

### Comparing `rateslib-0.3.0/rateslib.egg-info/PKG-INFO` & `rateslib-0.3.1/rateslib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rateslib
-Version: 0.3.0
+Version: 0.3.1
 Summary: A fixed income library for trading interest rates
 Author: J H M Darbyshire
 License: Attribution-NonCommercial-NoDerivatives 4.0 International
         
         =======================================================================
         
         Creative Commons Corporation ("Creative Commons") is not a law firm and
```

### Comparing `rateslib-0.3.0/rateslib.egg-info/SOURCES.txt` & `rateslib-0.3.1/rateslib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rateslib-0.3.0/tests/test_calendars.py` & `rateslib-0.3.1/tests/test_calendars.py`

 * *Files identical despite different names*

### Comparing `rateslib-0.3.0/tests/test_curves.py` & `rateslib-0.3.1/tests/test_curves.py`

 * *Files identical despite different names*

### Comparing `rateslib-0.3.0/tests/test_dual.py` & `rateslib-0.3.1/tests/test_dual.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
 import math
 import numpy as np
+from packaging import version
 
 import context
 from rateslib.dual import (
     Dual,
     Dual2,
     dual_exp,
     dual_log,
@@ -776,21 +777,36 @@
 def test_numpy_matmul(y_2, y_1):
     a = np.array([y_2, y_1])
     result = np.matmul(a[:, np.newaxis], a[np.newaxis, :])
     expected = np.array([[y_2 * y_2, y_2 * y_1], [y_2 * y_1, y_1 * y_1]])
     assert np.all(result == expected)
 
 
+@pytest.mark.skipif(
+    version.parse(np.__version__) >= version.parse("1.25.0"),
+    reason="Object dtypes accepted by NumPy in 1.25.0+"
+)
 def test_numpy_einsum(y_2, y_1):
     # einsum does not work with object dtypes
     a = np.array([y_2, y_1])
     with pytest.raises(TypeError):
         _ = np.einsum("i,j", a, a, optimize=True)
 
 
+@pytest.mark.skipif(
+    version.parse(np.__version__) < version.parse("1.25.0"),
+    reason="Object dtypes not accepted by NumPy in <1.25.0"
+)
+def test_numpy_einsum_works(y_2, y_1):
+    a = np.array([y_2, y_1])
+    result = np.einsum("i,j", a, a, optimize=True)
+    expected = np.array([[y_2 * y_2, y_2 * y_1], [y_2 * y_1, y_1 * y_1]])
+    assert np.all(result == expected)
+
+
 @pytest.mark.parametrize("z", [
     Dual(2., "y"),
     Dual2(3., "x", np.array([1]), np.array([[2]])),
 ])
 @pytest.mark.parametrize("dtype", [
     np.int8,
     np.int16,
```

### Comparing `rateslib-0.3.0/tests/test_fx.py` & `rateslib-0.3.1/tests/test_fx.py`

 * *Files identical despite different names*

### Comparing `rateslib-0.3.0/tests/test_instruments.py` & `rateslib-0.3.1/tests/test_instruments.py`

 * *Files identical despite different names*

### Comparing `rateslib-0.3.0/tests/test_legs.py` & `rateslib-0.3.1/tests/test_legs.py`

 * *Files identical despite different names*

### Comparing `rateslib-0.3.0/tests/test_periods.py` & `rateslib-0.3.1/tests/test_periods.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import context
 from rateslib.periods import (
     Cashflow, FixedPeriod, FloatPeriod, IndexFixedPeriod, IndexCashflow, IndexMixin
 )
 from rateslib.fx import FXRates
 from rateslib.default import Defaults
-from rateslib.curves import Curve, LineCurve, IndexCurve
+from rateslib.curves import Curve, LineCurve, IndexCurve, CompositeCurve
 
 
 @pytest.fixture()
 def curve():
     nodes = {
         dt(2022, 1, 1): 1.00,
         dt(2022, 4, 1): 0.99,
@@ -1228,14 +1228,54 @@
             i_date=dt(2001, 7, 20),
             i_lag=3,
             i_method="daily"
         )
         expected = 173.1 + 19/31 * (174.2 - 173.1)
         assert abs(result - expected) < 1e-6
 
+    def test_composite_curve(self):
+        index_period = IndexFixedPeriod(
+            start=dt(2022, 1, 3),
+            end=dt(2022, 4, 3),
+            payment=dt(2022, 4, 3),
+            notional=1e9,
+            convention="Act360",
+            termination=dt(2022, 4, 3),
+            frequency="Q",
+            fixed_rate=4.00,
+            currency="usd",
+            index_base=100.,
+        )
+        index_curve = IndexCurve(
+            nodes={dt(2022, 1, 1): 1.0, dt(2022, 4, 3): 0.995},
+            index_base=200.,
+        )
+        composite_curve = CompositeCurve([index_curve])
+        _, result, _ = index_period.index_ratio(composite_curve)
+
+    def test_composite_curve_raises(self):
+        index_period = IndexFixedPeriod(
+            start=dt(2022, 1, 3),
+            end=dt(2022, 4, 3),
+            payment=dt(2022, 4, 3),
+            notional=1e9,
+            convention="Act360",
+            termination=dt(2022, 4, 3),
+            frequency="Q",
+            fixed_rate=4.00,
+            currency="usd",
+            index_base=100.,
+        )
+        curve = Curve(
+            nodes={dt(2022, 1, 1): 1.0, dt(2022, 4, 3): 0.995},
+        )
+        composite_curve = CompositeCurve([curve])
+        with pytest.raises(TypeError, match="`index_value` must be forecast from"):
+            _, result, _ = index_period.index_ratio(composite_curve)
+
 
 class TestIndexCashflow:
 
     def test_cashflow_analytic_delta(self, curve):
         cashflow = IndexCashflow(
             notional=1e6, payment=dt(2022, 1, 1), index_base=100
         )
```

### Comparing `rateslib-0.3.0/tests/test_scheduling.py` & `rateslib-0.3.1/tests/test_scheduling.py`

 * *Files identical despite different names*

### Comparing `rateslib-0.3.0/tests/test_solver.py` & `rateslib-0.3.1/tests/test_solver.py`

 * *Files identical despite different names*

### Comparing `rateslib-0.3.0/tests/test_splines.py` & `rateslib-0.3.1/tests/test_splines.py`

 * *Files identical despite different names*

