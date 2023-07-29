# Comparing `tmp/rateslib-0.2.0.tar.gz` & `tmp/rateslib-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rateslib-0.2.0.tar", last modified: Mon May 15 18:25:25 2023, max compression
+gzip compressed data, was "rateslib-0.3.0.tar", last modified: Sat Jul 29 05:10:27 2023, max compression
```

## Comparing `rateslib-0.2.0.tar` & `rateslib-0.3.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2023-05-15 18:25:25.126181 rateslib-0.2.0/
--rw-r--r--   0 Darbyshire   (501) staff       (20)    19126 2022-10-15 05:18:28.000000 rateslib-0.2.0/LICENSE
--rw-r--r--   0 Darbyshire   (501) staff       (20)    23901 2023-05-15 18:25:25.125729 rateslib-0.2.0/PKG-INFO
--rw-r--r--   0 Darbyshire   (501) staff       (20)     1186 2023-04-24 18:38:25.000000 rateslib-0.2.0/README.md
--rw-r--r--   0 Darbyshire   (501) staff       (20)      779 2023-05-15 17:52:21.000000 rateslib-0.2.0/pyproject.toml
-drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2023-05-15 18:25:25.008758 rateslib-0.2.0/rateslib/
--rw-r--r--   0 Darbyshire   (501) staff       (20)     4459 2023-05-15 17:34:14.000000 rateslib-0.2.0/rateslib/__init__.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    23171 2023-05-15 17:59:17.000000 rateslib-0.2.0/rateslib/calendars.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    57996 2023-05-15 17:34:14.000000 rateslib-0.2.0/rateslib/curves.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)     3536 2023-05-15 17:34:14.000000 rateslib-0.2.0/rateslib/default.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    25348 2023-05-15 17:34:14.000000 rateslib-0.2.0/rateslib/dual.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    65162 2023-05-15 17:34:14.000000 rateslib-0.2.0/rateslib/fx.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)   234743 2023-05-15 18:06:24.000000 rateslib-0.2.0/rateslib/instruments.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    71323 2023-05-15 17:34:14.000000 rateslib-0.2.0/rateslib/legs.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    62756 2023-05-15 17:34:14.000000 rateslib-0.2.0/rateslib/periods.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    47001 2023-05-15 17:34:14.000000 rateslib-0.2.0/rateslib/scheduling.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    67841 2023-05-15 17:34:14.000000 rateslib-0.2.0/rateslib/solver.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    17008 2023-05-15 17:34:14.000000 rateslib-0.2.0/rateslib/splines.py
-drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2023-05-15 18:25:25.026673 rateslib-0.2.0/rateslib.egg-info/
--rw-r--r--   0 Darbyshire   (501) staff       (20)    23901 2023-05-15 18:25:24.000000 rateslib-0.2.0/rateslib.egg-info/PKG-INFO
--rw-r--r--   0 Darbyshire   (501) staff       (20)      653 2023-05-15 18:25:24.000000 rateslib-0.2.0/rateslib.egg-info/SOURCES.txt
--rw-r--r--   0 Darbyshire   (501) staff       (20)        1 2023-05-15 18:25:24.000000 rateslib-0.2.0/rateslib.egg-info/dependency_links.txt
--rw-r--r--   0 Darbyshire   (501) staff       (20)      129 2023-05-15 18:25:24.000000 rateslib-0.2.0/rateslib.egg-info/requires.txt
--rw-r--r--   0 Darbyshire   (501) staff       (20)        9 2023-05-15 18:25:24.000000 rateslib-0.2.0/rateslib.egg-info/top_level.txt
--rw-r--r--   0 Darbyshire   (501) staff       (20)       38 2023-05-15 18:25:25.126276 rateslib-0.2.0/setup.cfg
--rw-r--r--   0 Darbyshire   (501) staff       (20)       37 2022-08-28 05:42:04.000000 rateslib-0.2.0/setup.py
-drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2023-05-15 18:25:25.118447 rateslib-0.2.0/tests/
--rw-r--r--   0 Darbyshire   (501) staff       (20)     8187 2023-03-05 18:52:18.000000 rateslib-0.2.0/tests/test_calendars.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    25127 2023-05-15 17:34:14.000000 rateslib-0.2.0/tests/test_curves.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    23147 2023-05-06 20:57:27.000000 rateslib-0.2.0/tests/test_dual.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    28832 2023-04-24 16:35:20.000000 rateslib-0.2.0/tests/test_fx.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    88567 2023-05-15 17:34:14.000000 rateslib-0.2.0/tests/test_instruments.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    31919 2023-05-15 17:34:14.000000 rateslib-0.2.0/tests/test_legs.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    43128 2023-05-15 17:34:14.000000 rateslib-0.2.0/tests/test_periods.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    24515 2023-05-15 17:34:14.000000 rateslib-0.2.0/tests/test_scheduling.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    34007 2023-05-15 17:34:14.000000 rateslib-0.2.0/tests/test_solver.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)     5430 2023-03-29 17:12:48.000000 rateslib-0.2.0/tests/test_splines.py
+drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2023-07-29 05:10:27.082456 rateslib-0.3.0/
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    19126 2022-10-15 05:18:28.000000 rateslib-0.3.0/LICENSE
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    23901 2023-07-29 05:10:27.081979 rateslib-0.3.0/PKG-INFO
+-rw-r--r--   0 Darbyshire   (501) staff       (20)     1186 2023-04-24 18:38:25.000000 rateslib-0.3.0/README.md
+-rw-r--r--   0 Darbyshire   (501) staff       (20)      779 2023-07-29 05:05:23.000000 rateslib-0.3.0/pyproject.toml
+drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2023-07-29 05:10:27.016683 rateslib-0.3.0/rateslib/
+-rw-r--r--   0 Darbyshire   (501) staff       (20)     4780 2023-07-28 22:06:51.000000 rateslib-0.3.0/rateslib/__init__.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)     2763 2023-07-27 17:04:54.000000 rateslib-0.3.0/rateslib/_swaptions.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    23379 2023-07-27 17:04:54.000000 rateslib-0.3.0/rateslib/calendars.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    87883 2023-07-27 17:04:54.000000 rateslib-0.3.0/rateslib/curves.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)     3965 2023-07-27 17:04:54.000000 rateslib-0.3.0/rateslib/default.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    26483 2023-07-27 17:04:54.000000 rateslib-0.3.0/rateslib/dual.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    65656 2023-05-26 18:54:31.000000 rateslib-0.3.0/rateslib/fx.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)   287187 2023-07-27 17:04:54.000000 rateslib-0.3.0/rateslib/instruments.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    95396 2023-07-29 04:57:38.000000 rateslib-0.3.0/rateslib/legs.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    76258 2023-07-27 17:04:54.000000 rateslib-0.3.0/rateslib/periods.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    49424 2023-07-27 17:04:54.000000 rateslib-0.3.0/rateslib/scheduling.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    71411 2023-07-27 17:04:54.000000 rateslib-0.3.0/rateslib/solver.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    17008 2023-05-15 17:34:14.000000 rateslib-0.3.0/rateslib/splines.py
+drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2023-07-29 05:10:27.025196 rateslib-0.3.0/rateslib.egg-info/
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    23901 2023-07-29 05:10:26.000000 rateslib-0.3.0/rateslib.egg-info/PKG-INFO
+-rw-r--r--   0 Darbyshire   (501) staff       (20)      676 2023-07-29 05:10:26.000000 rateslib-0.3.0/rateslib.egg-info/SOURCES.txt
+-rw-r--r--   0 Darbyshire   (501) staff       (20)        1 2023-07-29 05:10:26.000000 rateslib-0.3.0/rateslib.egg-info/dependency_links.txt
+-rw-r--r--   0 Darbyshire   (501) staff       (20)      129 2023-07-29 05:10:26.000000 rateslib-0.3.0/rateslib.egg-info/requires.txt
+-rw-r--r--   0 Darbyshire   (501) staff       (20)        9 2023-07-29 05:10:26.000000 rateslib-0.3.0/rateslib.egg-info/top_level.txt
+-rw-r--r--   0 Darbyshire   (501) staff       (20)       38 2023-07-29 05:10:27.082548 rateslib-0.3.0/setup.cfg
+-rw-r--r--   0 Darbyshire   (501) staff       (20)       37 2022-08-28 05:42:04.000000 rateslib-0.3.0/setup.py
+drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2023-07-29 05:10:27.080343 rateslib-0.3.0/tests/
+-rw-r--r--   0 Darbyshire   (501) staff       (20)     8293 2023-07-27 17:04:54.000000 rateslib-0.3.0/tests/test_calendars.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    39559 2023-07-27 17:04:54.000000 rateslib-0.3.0/tests/test_curves.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    23278 2023-05-22 18:47:00.000000 rateslib-0.3.0/tests/test_dual.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    28890 2023-07-27 17:04:54.000000 rateslib-0.3.0/tests/test_fx.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)   118294 2023-07-27 17:04:54.000000 rateslib-0.3.0/tests/test_instruments.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    47895 2023-07-27 17:04:54.000000 rateslib-0.3.0/tests/test_legs.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    47058 2023-07-27 17:04:54.000000 rateslib-0.3.0/tests/test_periods.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    27914 2023-07-27 17:04:54.000000 rateslib-0.3.0/tests/test_scheduling.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    46380 2023-07-27 17:04:54.000000 rateslib-0.3.0/tests/test_solver.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)     5430 2023-03-29 17:12:48.000000 rateslib-0.3.0/tests/test_splines.py
```

### Comparing `rateslib-0.2.0/LICENSE` & `rateslib-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rateslib-0.2.0/PKG-INFO` & `rateslib-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rateslib
-Version: 0.2.0
+Version: 0.3.0
 Summary: A fixed income library for trading interest rates
 Author: J H M Darbyshire
 License: Attribution-NonCommercial-NoDerivatives 4.0 International
         
         =======================================================================
         
         Creative Commons Corporation ("Creative Commons") is not a law firm and
```

### Comparing `rateslib-0.2.0/README.md` & `rateslib-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `rateslib-0.2.0/pyproject.toml` & `rateslib-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rateslib"
-version = "0.2.0"
+version = "0.3.0"
 description = "A fixed income library for trading interest rates"
 readme = "README.md"
 authors = [{ name = "J H M Darbyshire"}]
 license = { file = "LICENSE" }
 keywords = ["interest rate", "derivatives", "swaps", "bonds", "fixed income"]
 dependencies = [
     "numpy>=1.21.5",
```

### Comparing `rateslib-0.2.0/rateslib/__init__.py` & `rateslib-0.3.0/rateslib/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -55,44 +55,65 @@
 
 from rateslib.calendars import create_calendar, get_calendar, add_tenor, dcf
 
 from rateslib.splines import bsplev_single, bspldnev_single, PPSpline
 
 from rateslib.scheduling import Schedule
 
-from rateslib.curves import Curve, LineCurve, interpolate, index_left
+from rateslib.curves import (
+    Curve,
+    LineCurve,
+    interpolate,
+    index_left,
+    IndexCurve,
+    CompositeCurve,
+)
 
 from rateslib.fx import (
     FXRates,
     FXForwards,
     ProxyCurve,
 )
 
 from rateslib.solver import Solver
 
-from rateslib.periods import FixedPeriod, FloatPeriod, Cashflow
+from rateslib.periods import (
+    FixedPeriod,
+    FloatPeriod,
+    Cashflow,
+    IndexFixedPeriod,
+    IndexCashflow,
+)
 
 from rateslib.legs import (
     FixedLeg,
     FixedLegExchange,
     FixedLegExchangeMtm,
     FloatLeg,
     FloatLegExchange,
     FloatLegExchangeMtm,
     ZeroFloatLeg,
+    ZeroFixedLeg,
+    ZeroIndexLeg,
+    IndexFixedLeg,
+    IndexFixedLegExchange,
     CustomLeg,
 )
 
 from rateslib.instruments import (
     Value,
     Bill,
     FixedRateBond,
+    IndexFixedRateBond,
     FloatRateBond,
+    BondFuture,
     IRS,
+    IIRS,
     ZCS,
+    ZCIS,
     FRA,
     Swap,
     SBS,
     FXSwap,
     NonMtmXCS,
     NonMtmFixedFixedXCS,
     NonMtmFixedFloatXCS,
@@ -111,21 +132,14 @@
 ==========================================================================
 
 **rateslib** is a Python package providing fast, flexible, and accurate
 fixed income instrument configuration and calculation.
 It aims to be the fundamental high-level building block for practical analysis of
 fixed income securities, derivatives, FX representation and curve construction
 in Python.
-
-Main Features
--------------
-Here are just a few of the things that pandas does well:
-
-  - Easy handling of missing data in floating point as well as non-floating
-    point data.
 """
 
 # Use __all__ to let type checkers know what is part of the public API.
 # Rateslib is not (yet) a py.typed library: the public API is determined
 # based on the documentation.
 __all__ = [
     "dt",
@@ -146,44 +160,56 @@
     "add_tenor",
     "dcf",
     # scheduling.py
     "Schedule",
     # curves.py
     "Curve",
     "LineCurve",
+    "IndexCurve",
+    "CompositeCurve",
     "interpolate",
     "index_left",
     # solver.py
     "Solver",
     # fx.py
     "FXRates",
     "FXForwards",
     "ProxyCurve",
     # periods.py,
     "FixedPeriod",
     "FloatPeriod",
     "Cashflow",
+    "IndexCashflow",
+    "IndexFixedPeriod",
     # legs.py
     "FixedLeg",
     "FloatLeg",
     "ZeroFloatLeg",
+    "ZeroFixedLeg",
     "FixedLegExchange",
     "FixedLegExchangeMtm",
     "FloatLegExchange",
     "FloatLegExchangeMtm",
+    "IndexFixedLeg",
+    "ZeroIndexLeg",
+    "IndexFixedLegExchange",
     "CustomLeg",
     # instruments.py
     "FixedRateBond",
+    "IndexFixedRateBond",
     "FloatRateBond",
+    "BondFuture",
     "FRA",
     "Value",
     "Bill",
     "IRS",
+    "IIRS",
     "Swap",
     "ZCS",
+    "ZCIS",
     "SBS",
     "FXSwap",
     "NonMtmXCS",
     "NonMtmFixedFixedXCS",
     "NonMtmFixedFloatXCS",
     "XCS",
     "FixedFixedXCS",
```

### Comparing `rateslib-0.2.0/rateslib/calendars.py` & `rateslib-0.3.0/rateslib/calendars.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,15 +338,15 @@
        :suppress:
 
        from rateslib.calendars import add_tenor, get_calendar, create_calendar, dcf
        from rateslib.curves import Curve, LineCurve, interpolate, index_left, IndexCurve
        from rateslib.dual import Dual, Dual2
        from rateslib.periods import FixedPeriod, FloatPeriod, Cashflow
        from rateslib.legs import FixedLeg, FloatLeg, CustomLeg, FloatLegExchange, FixedLegExchange, FloatLegExchangeMtm, FixedLegExchangeMtm
-       from rateslib.instruments import FixedRateBond, FloatRateBond, Value, IRS, SBS, FRA, forward_fx, Spread, Fly, BondFuture
+       from rateslib.instruments import FixedRateBond, FloatRateBond, Value, IRS, SBS, FRA, forward_fx, Spread, Fly, BondFuture, Bill, ZCS, FXSwap, ZCIS, IIRS
        from rateslib.solver import Solver
        from rateslib.splines import bspldnev_single, PPSpline
        from datetime import datetime as dt
        from pandas import date_range, Series, DataFrame
 
     .. ipython:: python
 
@@ -539,14 +539,15 @@
     float
 
     Notes
     -----
     Permitted values for the convention are:
 
     - `"1"`: Returns 1 for any period.
+    - `"1+"`: Returns the number of months between dates divided by 12.
     - `"Act365F"`: Returns actual number of days divided by a fixed 365 denominator.
     - `"Act360"`: Returns actual number of days divided by a fixed 360 denominator.
     - `"30E360"`, `"EuroBondBasis"`: Months are treated as having 30 days and start
       and end dates are converted under the rule:
 
       * start day is minimum of (30, start day),
       * end day is minimum of (30, end day).
@@ -583,16 +584,14 @@
        dcf(dt(2000, 1, 1), dt(2000, 4, 3), "ActActICMA", dt(2010, 1, 1), 3, False)
        dcf(dt(2000, 1, 1), dt(2000, 4, 3), "ActActICMA", dt(2010, 1, 1), 3, True)
 
     """
     convention = convention.upper()
     if convention == "ACT365F":
         return (end - start) / timedelta(days=365)
-    elif convention == "1":
-        return 1.0
     elif convention == "ACT360":
         return (end - start) / timedelta(days=360)
     elif convention in ["30360", "360360", "BONDBASIS"]:
         ds = min(30, start.day)
         de = min(ds, end.day) if ds == 30 else end.day
         y, m = end.year - start.year, (end.month - start.month) / 12
         return y + m + (de - ds) / 360
@@ -666,17 +665,21 @@
                     fraction += 1
                     fraction += (prev_start - start) / (
                         prev_start - _add_months(end, -2 * frequency_months, None, None)
                     )
                 else:
                     fraction += (end - start) / (end - prev_start)
                 return fraction * frequency_months / 12
+    elif convention == "1":
+        return 1.0
+    elif convention == "1+":
+        return end.year - start.year + (end.month - start.month) / 12
     else:
         raise ValueError(
-            "`convention` must be in {'Act365f', '1', 'Act360', "
+            "`convention` must be in {'Act365f', '1', '1+', 'Act360', "
             "'30360' '360360', 'BondBasis', '30E360', 'EuroBondBasis', "
             "'30E360ISDA', 'ActAct', 'ActActISDA', 'ActActICMA', "
             "'ActActISMA', 'ActActBond'}"
         )
 
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
```

### Comparing `rateslib-0.2.0/rateslib/curves.py` & `rateslib-0.3.0/rateslib/curves.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 from datetime import datetime, timedelta
 from typing import Optional, Union, Callable, Any
 from pandas.tseries.offsets import CustomBusinessDay
 from pandas.tseries.holiday import Holiday
 from uuid import uuid4
 import numpy as np
 import json
-from math import floor
+from math import floor, comb
 from rateslib import defaults
-from rateslib.dual import Dual, Dual2, dual_log, dual_exp
+from rateslib.dual import Dual, Dual2, dual_log, dual_exp, set_order_convert
 from rateslib.splines import PPSpline
 from rateslib.default import plot
 from rateslib.calendars import create_calendar, get_calendar, add_tenor, dcf
 
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
@@ -145,27 +145,20 @@
 
     def _set_ad_order(self, order):
         """
         Change the node values to float, Dual or Dual2 based on input parameter.
         """
         if order == getattr(self, "ad", None):
             return None
-        if order == 0:
-            self.ad = 0
-            self.nodes = {k: float(v) for i, (k, v) in enumerate(self.nodes.items())}
-            self.csolve()
-            return None
-        elif order == 1:
-            self.ad, DualType = 1, Dual
-        elif order == 2:
-            self.ad, DualType = 2, Dual2
-        else:
+        elif order not in [0, 1, 2]:
             raise ValueError("`order` can only be in {0, 1, 2} for auto diff calcs.")
+
+        self.ad = order
         self.nodes = {
-            k: DualType(float(v), f"{self.id}{i}")
+            k: set_order_convert(v, order, f"{self.id}{i}")
             for i, (k, v) in enumerate(self.nodes.items())
         }
         self.csolve()
         return None
 
 
 class PlotCurve:
@@ -268,61 +261,130 @@
         x = [left + timedelta(days=i) for i in range(points)]
         rates = [forward_fx(_, self, curve_foreign, fx_rate, fx_settlement) for _ in x]
         return plot(x, [rates])
 
 
 class Curve(Serialize, PlotCurve):
     """
-    Object to return DFs parametrised by DFs at given node dates and interpolation.
+    Curve based on DF parametrisation at given node dates with interpolation.
 
     Parameters
     ----------
     nodes : dict[datetime: float]
-        Degrees of freedom of the curve denoted by a node date and a corresponding
+        Parameters of the curve denoted by a node date and a corresponding
         DF at that point.
-    interpolation : str in {"log_linear", "linear", "linear_zero_rate"} or callable
+    interpolation : str or callable
         The interpolation used in the non-spline section of the curve. That is the part
         of the curve between the first node in ``nodes`` and the first knot in ``t``.
         If a callable, this allows a user-defined interpolation scheme, and this must
         have the signature ``method(date, nodes)``, where ``date`` is the datetime
         whose DF will be returned and ``nodes`` is as above and is passed to the
         callable.
     t : list[datetime], optional
         The knot locations for the B-spline log-cubic interpolation section of the
         curve. If *None* all interpolation will be done by the local method specified in
         ``interpolation``.
     c : list[float], optional
-        The B-spline coefficients used to define the log-cubic spline. If not given
-        will use :meth:`csolve`.
+        The B-spline coefficients used to define the log-cubic spline. If not given,
+        which is the expected case, uses :meth:`csolve` to calculate these
+        automatically.
     endpoints : str or list, optional
         The left and right endpoint constraint for the spline solution. Valid values are
         in {"natural", "not_a_knot"}. If a list, supply the left endpoint then the
         right endpoint.
     id : str, optional, set by Default
         The unique identifier to distinguish between curves in a multicurve framework.
     convention : str, optional, set by Default
         The convention of the curve for determining rates.
     modifier : str, optional
         The modification rule, in {"F", "MF", "P", "MP"}, for determining rates.
     calendar : calendar or str, optional
         The holiday calendar object to use. If str, looks up named calendar from
         static data. Used for determining rates.
-    index_base : float, optional
-        Set the initial, known value of the index. For typical use with RFR indexes and
-        inflation indexes, and if the :meth:`Curve.index_value` method is to be used.
     ad : int in {0, 1, 2}, optional
         Sets the automatic differentiation order. Defines whether to convert node
         values to float, :class:`~rateslib.dual.Dual` or
         :class:`~rateslib.dual.Dual2`. It is advised against
         using this setting directly. It is mainly used internally.
+
+    Notes
+    -----
+
+    This curve type is **discount factor (DF)** based and is parametrised by a set of
+    (date, DF) pairs set as ``nodes``. The initial node date of the curve is defined
+    to be today and should **always** have a DF of precisely 1.0. The initial DF
+    will **not** be affected by a :class:`~rateslib.solver.Solver`.
+
+    Intermediate DFs are determined through ``interpolation``. If local interpolation
+    is adopted a DF for an arbitrary date is dependent only on its immediately
+    neighbouring nodes via the interpolation routine. Available options are:
+
+    - *"log_linear"* (default for this curve type)
+    - *"linear_index"*
+
+    And also the following which are not recommended for this curve type:
+
+    - *"linear"*,
+    - *"linear_zero_rate"*,
+    - *"flat_forward"*,
+    - *"flat_backward"*,
+
+    Global interpolation in the form of a **log-cubic** spline is also configurable
+    with the parameters ``t``, ``c`` and ``endpoints``. See
+    :ref:`splines<splines-doc>` for instruction of knot sequence calibration.
+    Values before the first knot in ``t`` will be determined through the local
+    interpolation method.
+
+    For defining rates by a given tenor, the ``modifier`` and ``calendar`` arguments
+    will be used. For correct scaling of the rate a ``convention`` is attached to the
+    curve, which is usually one of "Act360" or "Act365F".
+
+    Examples
+    --------
+
+    .. ipython:: python
+
+       curve = Curve(
+           nodes={
+               dt(2022,1,1): 1.0,  # <- initial DF should always be 1.0
+               dt(2023,1,1): 0.99,
+               dt(2024,1,1): 0.979,
+               dt(2025,1,1): 0.967,
+               dt(2026,1,1): 0.956,
+               dt(2027,1,1): 0.946,
+           },
+           interpolation="log_linear",
+       )
+       curve.plot("1d")
+
+    .. plot::
+
+       from rateslib.curves import *
+       import matplotlib.pyplot as plt
+       from datetime import datetime as dt
+       import numpy as np
+       curve = Curve(
+           nodes={
+               dt(2022,1,1): 1.0,
+               dt(2023,1,1): 0.99,
+               dt(2024,1,1): 0.979,
+               dt(2025,1,1): 0.967,
+               dt(2026,1,1): 0.956,
+               dt(2027,1,1): 0.946,
+           },
+           interpolation="log_linear",
+       )
+       fig, ax, line = curve.plot("1D")
+       plt.show()
     """
 
     _op_exp = staticmethod(dual_exp)  # Curve is DF based: log-cubic spline is exp'ed
     _op_log = staticmethod(dual_log)  # Curve is DF based: spline is applied over log
     _ini_solve = 1  # Curve is assumed to have initial DF node at 1.0 as constraint
+    _base_type = "dfs"
 
     def __init__(
         self,
         nodes: dict,
         interpolation: Optional[Union[str, Callable]] = None,
         t: Optional[list[datetime]] = None,
         c: Optional[list[float]] = None,
@@ -403,14 +465,16 @@
     def rate(
         self,
         effective: datetime,
         termination: Union[datetime, str],
         modifier: Optional[Union[str, bool]] = False,
         # calendar: Optional[Union[CustomBusinessDay, str, bool]] = False,
         # convention: Optional[str] = None,
+        float_spread: float = None,
+        spread_compound_method: str = None,
     ):
         """
         Calculate the rate on the `Curve` using DFs.
 
         If rates are sought for dates prior to the initial node of the curve `None`
         will be returned.
 
@@ -425,14 +489,20 @@
             determined from the `Curve` modifier.
         # calendar : CustomBusinessDay, str, None, optional
         #     The business day calendar to determine valid business days from which to
         #     determine rates. If `False` is determined from the `Curve` calendar.
         # convention : str, optional
         #     The day count convention used for calculating rates. If `None` is
         #     determined from the `Curve` convention.
+        float_spread : float, optional
+            A float spread can be added to the rate in certain cases.
+        spread_compound_method : str in {"none_simple", "isda_compounding"}
+            The method if adding a float spread.
+            If *"none_simple"* is used this results in an exact calculation.
+            If *"isda_compounding"* is used this results in an approximation.
 
         Returns
         -------
         Dual, Dual2 or float
 
         Notes
         -----
@@ -442,41 +512,85 @@
 
         ``modifier`` is only used if a tenor is given as the termination.
 
         Major indexes, such as legacy IBORs, and modern RFRs typically use a
         ``convention`` which is either `"Act365F"` or `"Act360"`. These conventions
         do not need additional parameters, such as the `termination` of a leg,
         the `frequency` or a leg or whether it is a `stub` to calculate a DCF.
+
+        **Adding Floating Spreads**
+
+        An optimised method for adding floating spreads to a curve rate is provided.
+        This is quite restrictive and mainly used internally to facilitate other parts
+        of the library.
+
+        - When ``spread_compound_method`` is *"none_simple"* the spread is a simple
+          linear addition.
+        - When using *"isda_compounding"* the curve is assumed to be comprised of RFR
+          rates and an approximation is used to derive to total rate.
+        - The *"isda_flat_compounding"* method is not suitable for this optimisation.
+
         """
         modifier = self.modifier if modifier is False else modifier
         # calendar = self.calendar if calendar is False else calendar
         # convention = self.convention if convention is None else convention
 
         if isinstance(termination, str):
             termination = add_tenor(effective, termination, modifier, self.calendar)
         try:
             df_ratio = self[effective] / self[termination]
         except ZeroDivisionError:
             return None
-        rate = (df_ratio - 1) / dcf(effective, termination, self.convention)
-        return rate * 100
+
+        try:
+            _ = (df_ratio - 1) / dcf(effective, termination, self.convention) * 100
+        except ZeroDivisionError:
+            raise ZeroDivisionError(
+                f"effective: {effective}, termination: {termination}"
+            )
+
+        if float_spread is not None and abs(float_spread) > 1e-9:
+            if spread_compound_method == "none_simple":
+                return _ + float_spread / 100
+            elif spread_compound_method == "isda_compounding":
+                # this provides an approximated rate
+                r_bar, d, n = average_rate(effective, termination, self.convention, _)
+                _ = ((1 + (r_bar + float_spread / 100) / 100 * d) ** n - 1) / (n * d)
+                return 100 * _
+            elif spread_compound_method == "isda_flat_compounding":
+                # this provides an approximated rate
+                r_bar, d, n = average_rate(effective, termination, self.convention, _)
+                rd = r_bar / 100 * d
+                _ = (
+                    (r_bar + float_spread / 100)
+                    / n
+                    * (comb(n, 1) + comb(n, 2) * rd + comb(n, 3) * rd**2)
+                )
+                return _
+            else:
+                raise ValueError(
+                    "Must supply a valid `spread_compound_method`, when `float_spread` "
+                    " is not `None`."
+                )
+
+        return _
 
     def csolve(self):
         """
-        Solve the coefficients, ``c``, of the :class:`PPSpline`.
-
-        Only impacts curves which have a knot sequence, ``t``, and a ``PPSpline``.
-        Only solves if ``c`` not given at ``Curve`` initialisation.
+        Solves **and sets** the coefficients, ``c``, of the :class:`PPSpline`.
 
         Returns
         -------
-        Set the coefficients for the PPSpline : None
+        None
 
         Notes
         -----
+        Only impacts curves which have a knot sequence, ``t``, and a ``PPSpline``.
+        Only solves if ``c`` not given at curve initialisation.
+
         Uses the ``spline_endpoints`` attribute on the class to determine the solving
         method.
         """
         if self.spline is None or self.c_init:
             return None
 
         self.spline = PPSpline(4, self.t, None)
@@ -620,17 +734,20 @@
         return _
 
     def _translate_nodes(self, start: datetime):
         scalar = 1 / self[start]
         new_nodes = {k: scalar * v for k, v in self.nodes.items()}
 
         # re-organise the nodes on the new curve
-        if start == self.node_dates[1]:
-            del new_nodes[self.node_dates[1]]
         del new_nodes[self.node_dates[0]]
+        flag, i = (start >= self.node_dates[1]), 1
+        while flag:
+            del new_nodes[self.node_dates[i]]
+            flag, i = (start >= self.node_dates[i + 1]), i + 1
+
         new_nodes = {start: 1.0, **new_nodes}
         return new_nodes
 
     def translate(self, start: datetime, t: bool = False):
         """
         Create a new curve with an initial node date moved forward keeping all else
         constant.
@@ -699,14 +816,15 @@
                },
                t = [
                    dt(2024, 1, 1), dt(2024, 1, 1), dt(2024, 1, 1), dt(2024, 1, 1),
                    dt(2025, 1, 1),
                    dt(2026, 1, 1),
                    dt(2027, 1, 1), dt(2027, 1, 1), dt(2027, 1, 1), dt(2027, 1, 1),
                ],
+               interpolation="log_linear",
            )
            translated_curve = curve.translate(dt(2022, 12, 1))
            fig, ax, line = curve.plot("1d", comparators=[translated_curve], labels=["orig", "translated"], left=dt(2022, 12, 1))
            plt.show()
            plt.close()
 
         .. ipython:: python
@@ -756,18 +874,16 @@
            )
            translated = curve.translate(dt(2022, 1, 15))
            translated2 = curve.translate(dt(2022, 1, 15), t=True)
            fig, ax, line = curve.plot("1d", left=dt(2022, 1, 15), comparators=[translated, translated2], labels=["orig", "translated", "translated2"])
            plt.show()
 
         """
-        if start <= self.node_dates[0] or self.node_dates[1] < start:
-            raise ValueError(
-                "Cannot translate exactly for the given `start`, review the docs."
-            )
+        if start <= self.node_dates[0]:
+            raise ValueError("Cannot translate into the past. Review the docs.")
 
         new_nodes = self._translate_nodes(start)
 
         # re-organise the t-knot sequence
         # TODO: shift the t knot sequence if the first knot begins at t-0.
         new_t = None if self.t is None else self.t.copy()
         if self.t and start <= self.t[0]:
@@ -829,15 +945,16 @@
 
     # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
     # Commercial use of this code, and/or copying and redistribution is prohibited.
     # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
     def roll(self, tenor: Union[datetime, str]):
         """
-        Create a new curve with its shape translated in time
+        Create a new curve with its shape translated in time but an identical initial
+        node date.
 
         This curve adjustment is a simulation of a future state of the market where
         forward rates are assumed to have moved so that the present day's curve shape
         is reflected in the future (or the past). This is often used in trade
         strategy analysis.
 
         Parameters
@@ -917,87 +1034,169 @@
 
         if tenor == self.node_dates[0]:
             return self.copy()
 
         days = (tenor - self.node_dates[0]).days
         new_nodes = self._roll_nodes(tenor, days)
         new_t = [_ + timedelta(days=days) for _ in self.t] if self.t else None
+        if type(self) is IndexCurve:
+            xtra = dict(index_lag=self.index_lag, index_base=self.index_base)
+        else:
+            xtra = {}
         new_curve = type(self)(
             nodes=new_nodes,
             interpolation=self.interpolation,
             t=new_t,
             c=None,
             endpoints=self.spline_endpoints,
             modifier=self.modifier,
             calendar=self.calendar,
             convention=self.convention,
             id=None,
-            # TODO: design how to adjust the index_base on a rolled curve.
             ad=self.ad,
+            **xtra,
         )
         if tenor > self.node_dates[0]:
             return new_curve
         else:  # tenor < self.node_dates[0]
             return new_curve.translate(self.node_dates[0])
 
 
 class LineCurve(Curve):
     """
-    Object to return values parametrised by values at node dates and interpolation.
+    Curve based on value parametrisation at given node dates with interpolation.
 
     Parameters
     ----------
     nodes : dict[datetime: float]
-        Degrees of freedom of the curve denoted by a node date and a corresponding
+        Parameters of the curve denoted by a node date and a corresponding
         value at that point.
     interpolation : str in {"log_linear", "linear"} or callable
         The interpolation used in the non-spline section of the curve. That is the part
         of the curve between the first node in ``nodes`` and the first knot in ``t``.
         If a callable, this allows a user-defined interpolation scheme, and this must
         have the signature ``method(date, nodes)``, where ``date`` is the datetime
         whose DF will be returned and ``nodes`` is as above and is passed to the
         callable.
     t : list[datetime], optional
         The knot locations for the B-spline cubic interpolation section of the
         curve. If *None* all interpolation will be done by the method specified in
         ``interpolation``.
     c : list[float], optional
-        The B-spline coefficients used to define the cubic spline. If not given
-        will use :meth:`csolve`.
+        The B-spline coefficients used to define the log-cubic spline. If not given,
+        which is the expected case, uses :meth:`csolve` to calculate these
+        automatically.
     endpoints : str or list, optional
         The left and right endpoint constraint for the spline solution. Valid values are
         in {"natural", "not_a_knot"}. If a list, supply the left endpoint then the
         right endpoint.
     id : str, optional, set by Default
-        The unique identifier to distinguish between curves in a multicurve framework.
+        The unique identifier to distinguish between curves in a multi-curve framework.
     convention : str, optional,
-        **This parameter is not used by :class:`LineCurve`**. It is included for
+        This argument is **not used** by :class:`LineCurve`. It is included for
         signature consistency with :class:`Curve`.
     modifier : str, optional
-        **This parameter is not used by :class:`LineCurve`**. It is included for
+        This argument is **not used** by :class:`LineCurve`. It is included for
         signature consistency with :class:`Curve`.
     calendar : calendar or str, optional
-        **This parameter is not used by :class:`LineCurve`**. It is included for
-        signature consistency with :class:`Curve`.
-    index_base : float, optional
-        **This parameter is not used by :class:`LineCurve`**. It is included for
+        This argument is **not used** by :class:`LineCurve`. It is included for
         signature consistency with :class:`Curve`.
     ad : int in {0, 1, 2}, optional
         Sets the automatic differentiation order. Defines whether to convert node
         values to float, :class:`Dual` or :class:`Dual2`. It is advised against
         using this setting directly. It is mainly used internally.
+
+    Notes
+    -----
+
+    This curve type is **value** based and it is parametrised by a set of
+    (date, value) pairs set as ``nodes``. The initial node date of the curve is defined
+    to be today, and can take a general value. The initial value
+    will be affected by a :class:`~rateslib.solver.Solver`.
+
+    .. note::
+
+       This curve type can only ever be used for **forecasting** rates and projecting
+       cashflow calculations. It cannot be used to discount cashflows becuase it is
+       not DF based and there is no mathematical one-to-one conversion available to
+       imply DFs.
+
+    Intermediate values are determined through ``interpolation``. If local interpolation
+    is adopted a value for an arbitrary date is dependent only on its immediately
+    neighbouring nodes via the interpolation routine. Available options are:
+
+    - *"linear"* (default for this curve type)
+    - *"log_linear"* (useful for values that exponential, e.g. stock indexes or GDP)
+    - *"flat_forward"*, (useful for replicating a DF based log-linear type curve)
+    - *"flat_backward"*,
+
+    And also the following which are not recommended for this curve type:
+
+    - *"linear_index"*
+    - *"linear_zero_rate"*,
+
+    Global interpolation in the form of a **cubic** spline is also configurable
+    with the parameters ``t``, ``c`` and ``endpoints``. See
+    :ref:`splines<splines-doc>` for instruction of knot sequence calibration.
+    Values before the first knot in ``t`` will be determined through the local
+    interpolation method.
+
+    This curve type cannot return arbitrary tenor rates. It will only return a single
+    value which is applicable to that date. It is recommended to review
+    :ref:`RFR and IBOR Indexing<c-curves-ibor-rfr>` to ensure indexing is done in a
+    way that is consistent with internal instrument configuration.
+
+    Examples
+    --------
+
+    .. ipython:: python
+
+       line_curve = LineCurve(
+           nodes={
+               dt(2022,1,1): 0.975,  # <- initial value is general
+               dt(2023,1,1): 1.10,
+               dt(2024,1,1): 1.22,
+               dt(2025,1,1): 1.14,
+               dt(2026,1,1): 1.03,
+               dt(2027,1,1): 1.03,
+           },
+           interpolation="linear",
+       )
+       line_curve.plot("1d")
+
+    .. plot::
+
+       from rateslib.curves import *
+       import matplotlib.pyplot as plt
+       from datetime import datetime as dt
+       import numpy as np
+       line_curve = LineCurve(
+           nodes={
+               dt(2022,1,1): 0.975,  # <- initial value is general
+               dt(2023,1,1): 1.10,
+               dt(2024,1,1): 1.22,
+               dt(2025,1,1): 1.14,
+               dt(2026,1,1): 1.03,
+               dt(2027,1,1): 1.03,
+           },
+           interpolation="linear",
+       )
+       fig, ax, line = line_curve.plot("1D")
+       plt.show()
+
     """
 
     _op_exp = staticmethod(
         lambda x: x
     )  # LineCurve spline is not log based so no exponent needed
     _op_log = staticmethod(
         lambda x: x
     )  # LineCurve spline is not log based so no log needed
     _ini_solve = 0  # No constraint placed on initial node in Solver
+    _base_type = "values"
 
     def __init__(
         self,
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
@@ -1106,20 +1305,23 @@
             calendar=self.calendar,
             ad=self.ad,
         )
         return _
 
     def _translate_nodes(self, start: datetime):
         new_nodes = self.nodes.copy()
+
         # re-organise the nodes on the new curve
         del new_nodes[self.node_dates[0]]
-        if start == self.node_dates[1]:
-            pass
-        else:
-            new_nodes = {start: self[start], **new_nodes}
+        flag, i = (start >= self.node_dates[1]), 1
+        while flag:
+            del new_nodes[self.node_dates[i]]
+            flag, i = (start >= self.node_dates[i + 1]), i + 1
+
+        new_nodes = {start: self[start], **new_nodes}
         return new_nodes
 
     # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
     # Commercial use of this code, and/or copying and redistribution is prohibited.
     # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
     def translate(self, start: datetime, t: bool = False):
@@ -1338,22 +1540,24 @@
 
         """
         return super().roll(tenor)
 
 
 class IndexCurve(Curve):
     """
-    A :class:`Curve` designed for use with inflation secuities and derivatives.
+    A subclass of :class:`~rateslib.curves.Curve` with an ``index_base`` value for
+    index calculations.
 
     Parameters
     ----------
     args : tuple
         Position arguments required by :class:`Curve`.
-    inf_lag : int
-        Number of months of inflation lag this curve adopts. For example if the initial
+    index_base: float
+    index_lag : int
+        Number of months of by which the index lags the date. For example if the initial
         curve node date is 1st Sep 2021 based on the inflation index published
         17th June 2023 then the lag is 3 months.
     kwargs : dict
         Keyword arguments required by :class:`Curve`.
     """
 
     def __init__(
@@ -1363,15 +1567,15 @@
         index_lag: Optional[int] = None,
         **kwargs,
     ):
         self.index_lag = defaults.index_lag if index_lag is None else index_lag
         self.index_base = index_base
         if self.index_base is None:
             raise ValueError("`index_base` must be given for IndexCurve.")
-        super().__init__(*args, **kwargs)
+        super().__init__(*args, **{**{"interpolation": "linear_index"}, **kwargs})
 
     def index_value(self, date: datetime, interpolation: str = "daily"):
         """
         Calculate the accrued value of the index from the ``index_base``.
 
         Parameters
         ----------
@@ -1410,15 +1614,592 @@
             date_ = date
         elif interpolation.lower() == "monthly":
             date_ = datetime(date.year, date.month, 1)
         else:
             raise ValueError(
                 "`interpolation` for `index_value` must be in {'daily', 'monthly'}."
             )
-        return self.index_base * 1 / self[date_]
+        if date_ < self.node_dates[0]:
+            return 0.0
+            # return zero for index dates in the past
+            # the proper way for instruments to deal with this is to supply i_fixings
+        else:
+            return self.index_base * 1 / self[date_]
+
+    def plot_index(
+        self,
+        right: Optional[Union[datetime, str]] = None,
+        left: Optional[Union[datetime, str]] = None,
+        comparators: list[Curve] = [],
+        difference: bool = False,
+        labels: list[str] = [],
+    ):
+        """
+        Plot given forward tenor rates from the curve.
+
+        Parameters
+        ----------
+        tenor : str
+            The tenor of the forward rates to plot, e.g. "1D", "3M".
+        right : datetime or str, optional
+            The right bound of the graph. If given as str should be a tenor format
+            defining a point measured from the initial node date of the curve.
+            Defaults to the final node of the curve minus the ``tenor``.
+        left : datetime or str, optional
+            The left bound of the graph. If given as str should be a tenor format
+            defining a point measured from the initial node date of the curve.
+            Defaults to the initial node of the curve.
+        comparators: list[Curve]
+            A list of curves which to include on the same plot as comparators.
+        difference : bool
+            Whether to plot as comparator minus base curve or outright curve levels in
+            plot. Default is `False`.
+        labels : list[str]
+            A list of strings associated with the plot and comparators. Must be same
+            length as number of plots.
+
+        Returns
+        -------
+        (fig, ax, line) : Matplotlib.Figure, Matplotplib.Axes, Matplotlib.Lines2D
+        """
+        if left is None:
+            left_: datetime = self.node_dates[0]
+        elif isinstance(left, str):
+            left_ = add_tenor(self.node_dates[0], left, None, None)
+        elif isinstance(left, datetime):
+            left_ = left
+        else:
+            raise ValueError("`left` must be supplied as datetime or tenor string.")
+
+        if right is None:
+            right_: datetime = self.node_dates[-1]
+        elif isinstance(right, str):
+            right_ = add_tenor(self.node_dates[0], right, None, None)
+        elif isinstance(right, datetime):
+            right_ = right
+        else:
+            raise ValueError("`right` must be supplied as datetime or tenor string.")
+
+        points: int = (right_ - left_).days + 1
+        x = [left_ + timedelta(days=i) for i in range(points)]
+        rates = [self.index_value(_) for _ in x]
+        if not difference:
+            y = [rates]
+            if comparators is not None:
+                for comparator in comparators:
+                    y.append([comparator.index_value(_) for _ in x])
+        elif difference and len(comparators) > 0:
+            y = []
+            for comparator in comparators:
+                diff = [comparator.index_value(_) - rates[i] for i, _ in enumerate(x)]
+                y.append(diff)
+        return plot(x, y, labels)
+
+
+class CompositeCurve(PlotCurve):
+    """
+    A dynamic composition of a sequence of other curves.
+
+    .. note::
+       Can only composite curves of the same type: :class:`Curve`, :class:`IndexCurve`
+       or :class:`LineCurve`. Other curve parameters such as ``modifier``, ``calendar``
+       and ``convention`` must also match.
+
+    Parameters
+    ----------
+    curves : sequence of :class:`Curve`, :class:`LineCurve` or :class:`IndexCurve`
+        The curves to be composited.
+    id : str, optional, set by Default
+        The unique identifier to distinguish between curves in a multi-curve framework.
+
+    Examples
+    --------
+    Composite two :class:`LineCurve` s. Here, simulating the effect of adding
+    quarter-end turns to a cubic spline interpolator, which is otherwise difficult to
+    mathematically derive.
+
+    .. ipython:: python
+
+       from rateslib.curves import LineCurve, CompositeCurve
+       line_curve1 = LineCurve(
+           nodes={
+               dt(2022, 1, 1): 2.5,
+               dt(2023, 1, 1): 3.5,
+               dt(2024, 1, 1): 3.0,
+           },
+           t=[dt(2022, 1, 1), dt(2022, 1, 1), dt(2022, 1, 1), dt(2022, 1, 1),
+              dt(2023, 1, 1),
+              dt(2024, 1, 1), dt(2024, 1, 1), dt(2024, 1, 1), dt(2024, 1, 1)],
+       )
+       line_curve2 = LineCurve(
+           nodes={
+               dt(2022, 1, 1): 0,
+               dt(2022, 3, 31): -0.2,
+               dt(2022, 4, 1): 0,
+               dt(2022, 6, 30): -0.2,
+               dt(2022, 7, 1): 0,
+               dt(2022, 9, 30): -0.2,
+               dt(2022, 10, 1): 0,
+               dt(2022, 12, 31): -0.2,
+               dt(2023, 1, 1): 0,
+               dt(2023, 3, 31): -0.2,
+               dt(2023, 4, 1): 0,
+               dt(2023, 6, 30): -0.2,
+               dt(2023, 7, 1): 0,
+               dt(2023, 9, 30): -0.2,
+           },
+           interpolation="flat_forward",
+       )
+       curve = CompositeCurve([line_curve1, line_curve2])
+       curve.plot("1d")
+
+    .. plot::
+
+       from rateslib.curves import LineCurve, CompositeCurve
+       import matplotlib.pyplot as plt
+       from datetime import datetime as dt
+       line_curve1 = LineCurve(
+           nodes={
+               dt(2022, 1, 1): 2.5,
+               dt(2023, 1, 1): 3.5,
+               dt(2024, 1, 1): 3.0,
+           },
+           t=[dt(2022, 1, 1), dt(2022, 1, 1), dt(2022, 1, 1), dt(2022, 1, 1),
+              dt(2023, 1, 1),
+              dt(2024, 1, 1), dt(2024, 1, 1), dt(2024, 1, 1), dt(2024, 1, 1)],
+       )
+       line_curve2 = LineCurve(
+           nodes={
+               dt(2022, 1, 1): 0,
+               dt(2022, 3, 31): -0.2,
+               dt(2022, 4, 1): 0,
+               dt(2022, 6, 30): -0.2,
+               dt(2022, 7, 1): 0,
+               dt(2022, 9, 30): -0.2,
+               dt(2022, 10, 1): 0,
+               dt(2022, 12, 31): -0.2,
+               dt(2023, 1, 1): 0,
+               dt(2023, 3, 31): -0.2,
+               dt(2023, 4, 1): 0,
+               dt(2023, 6, 30): -0.2,
+               dt(2023, 7, 1): 0,
+               dt(2023, 9, 30): -0.2,
+           },
+           interpolation="flat_forward",
+       )
+       curve = CompositeCurve([line_curve1, line_curve2])
+       fig, ax, line = curve.plot("1D")
+       plt.show()
+
+    We can also composite DF based curves by using a fast approximation or an
+    exact match.
+
+    .. ipython:: python
+
+       from rateslib.curves import Curve, CompositeCurve
+       curve1 = Curve(
+           nodes={
+               dt(2022, 1, 1): 1.0,
+               dt(2023, 1, 1): 0.98,
+               dt(2024, 1, 1): 0.965,
+               dt(2025, 1, 1): 0.955
+           },
+           t=[dt(2023, 1, 1), dt(2023, 1, 1), dt(2023, 1, 1), dt(2023, 1, 1),
+              dt(2024, 1, 1),
+              dt(2025, 1, 1), dt(2025, 1, 1), dt(2025, 1, 1), dt(2025, 1, 1)],
+       )
+       curve2 =Curve(
+           nodes={
+               dt(2022, 1, 1): 1.0,
+               dt(2022, 6, 30): 1.0,
+               dt(2022, 7, 1): 0.999992,
+               dt(2022, 12, 31): 0.999992,
+               dt(2023, 1, 1): 0.999984,
+               dt(2023, 6, 30): 0.999984,
+               dt(2023, 7, 1): 0.999976,
+               dt(2023, 12, 31): 0.999976,
+               dt(2024, 1, 1): 0.999968,
+               dt(2024, 6, 30): 0.999968,
+               dt(2024, 7, 1): 0.999960,
+               dt(2025, 1, 1): 0.999960,
+           },
+       )
+       curve = CompositeCurve([curve1, curve2])
+       curve.plot("1D", comparators=[curve1, curve2], labels=["Composite", "C1", "C2"])
+
+    .. plot::
+
+       from rateslib.curves import Curve, CompositeCurve
+       import matplotlib.pyplot as plt
+       from datetime import datetime as dt
+       curve1 = Curve(
+           nodes={
+               dt(2022, 1, 1): 1.0,
+               dt(2023, 1, 1): 0.98,
+               dt(2024, 1, 1): 0.965,
+               dt(2025, 1, 1): 0.955
+           },
+           t=[dt(2023, 1, 1), dt(2023, 1, 1), dt(2023, 1, 1), dt(2023, 1, 1),
+              dt(2024, 1, 1),
+              dt(2025, 1, 1), dt(2025, 1, 1), dt(2025, 1, 1), dt(2025, 1, 1)],
+       )
+       curve2 =Curve(
+           nodes={
+               dt(2022, 1, 1): 1.0,
+               dt(2022, 6, 30): 1.0,
+               dt(2022, 7, 1): 0.999992,
+               dt(2022, 12, 31): 0.999992,
+               dt(2023, 1, 1): 0.999984,
+               dt(2023, 6, 30): 0.999984,
+               dt(2023, 7, 1): 0.999976,
+               dt(2023, 12, 31): 0.999976,
+               dt(2024, 1, 1): 0.999968,
+               dt(2024, 6, 30): 0.999968,
+               dt(2024, 7, 1): 0.999960,
+               dt(2025, 1, 1): 0.999960,
+           },
+       )
+       curve = CompositeCurve([curve1, curve2])
+       fig, ax, line = curve.plot("1D", comparators=[curve1, curve2], labels=["Composite", "C1", "C2"])
+       plt.show()
+
+    The :meth:`~rateslib.curves.CompositeCurve.rate` method of a :class:`CompositeCurve`
+    composed of either :class:`Curve` or :class:`IndexCurve` s
+    accepts an ``approximate`` argument. When *True* by default it used a geometric mean
+    approximation to determine composite period rates.
+    Below we demonstrate this is more than 1000x faster and within 1e-8 of the true
+    value.
+
+    .. ipython:: python
+
+       curve.rate(dt(2022, 6, 1), "1y")
+       %timeit curve.rate(dt(2022, 6, 1), "1y")
+
+    .. ipython:: python
+
+       curve.rate(dt(2022, 6, 1), "1y", approximate=False)
+       %timeit curve.rate(dt(2022, 6, 1), "1y", approximate=False)
+
+    """
+
+    def __init__(
+        self,
+        curves: Union[list, tuple],
+        id: Optional[str] = None,
+        multi_csa: bool = False,
+        multi_csa_min_step: Optional[int] = 1,
+        multi_csa_max_step: Optional[int] = 1825,
+    ) -> None:
+        self.id = id or uuid4().hex[:5] + "_"  # 1 in a million clash
+
+        if multi_csa and isinstance(curves[0], (LineCurve, IndexCurve)):
+            raise TypeError("Multi-CSA curves must be of type `Curve`.")
+        self.multi_csa = multi_csa
+        self.multi_csa_min_step = max(1, multi_csa_min_step)
+        self.multi_csa_max_step = min(1825, multi_csa_max_step)
+        if self.multi_csa_min_step > self.multi_csa_max_step:
+            raise ValueError("`multi_csa_max_step` cannot be less than `min_step`.")
+
+        # validate
+        self._base_type = curves[0]._base_type
+        for i in range(1, len(curves)):
+            if not type(curves[0]) == type(curves[i]):
+                raise TypeError(
+                    "`curves` must be a list of similar type curves, got "
+                    f"{type(curves[0])} and {type(curves[i])}."
+                )
+            if not curves[0].node_dates[0] == curves[i].node_dates[0]:
+                raise ValueError(
+                    "`curves` must share the same initial node date, got "
+                    f"{curves[0].node_dates[0]} and {curves[i].node_dates[0]}"
+                )
+
+        if not self.multi_csa:  # for multi_csa DF curve do not check calendars
+            for attr in [
+                "calendar",
+            ]:
+                for i in range(1, len(curves)):
+                    if getattr(curves[i], attr, None) != getattr(curves[0], attr, None):
+                        raise ValueError(
+                            "Cannot composite curves with different attributes, "
+                            f"got {attr}s, '{getattr(curves[i], attr, None)}' and "
+                            f"'{getattr(curves[0], attr, None)}'."
+                        )
+        self.calendar = curves[0].calendar
+
+        if self._base_type == "dfs":
+            for attr in ["modifier", "convention"]:
+                for i in range(1, len(curves)):
+                    if getattr(curves[i], attr, None) != getattr(curves[0], attr, None):
+                        raise ValueError(
+                            "Cannot composite curves with different attributes, "
+                            f"got {attr}s, '{getattr(curves[i], attr, None)}' and "
+                            f"'{getattr(curves[0], attr, None)}'."
+                        )
+            self.modifier = curves[0].modifier
+            self.convention = curves[0].convention
+        if isinstance(curves[0], IndexCurve):
+            for attr in ["index_base", "index_lag"]:
+                for i in range(1, len(curves)):
+                    if getattr(curves[i], attr, None) != getattr(curves[0], attr, None):
+                        raise ValueError(
+                            "Cannot composite curves with different attributes, "
+                            f"got {attr}s, '{getattr(curves[i], attr, None)}' and "
+                            f"'{getattr(curves[0], attr, None)}'."
+                        )
+            self.index_lag = curves[0].index_lag
+            self.index_base = curves[0].index_base
+
+        self.curves = tuple(curves)
+        self.node_dates = self.curves[0].node_dates
+
+    def rate(
+        self,
+        effective: datetime,
+        termination: Optional[Union[datetime, str]] = None,
+        modifier: Optional[Union[str, bool]] = False,
+        approximate: bool = True,
+    ):
+        """
+        Calculate the composited rate on the curve.
+
+        If rates are sought for dates prior to the initial node of the curve `None`
+        will be returned.
+
+        Parameters
+        ----------
+        effective : datetime
+            The start date of the period for which to calculate the rate.
+        termination : datetime or str
+            The end date of the period for which to calculate the rate.
+        modifier : str, optional
+            The day rule if determining the termination from tenor. If `False` is
+            determined from the `Curve` modifier.
+        approximate : bool, optional
+            When compositing :class:`Curve` or :class:`IndexCurve` calculating many
+            individual rates is expensive. This uses an approximation typically with
+            error less than 1/100th of basis point. Not used if ``multi_csa`` is True.
+
+        Returns
+        -------
+        Dual, Dual2 or float
+        """
+        if self._base_type == "values":
+            _ = 0.0
+            for i in range(0, len(self.curves)):
+                _ += self.curves[i].rate(effective, termination, modifier)
+            return _
+        elif self._base_type == "dfs":
+            modifier = self.modifier if modifier is False else modifier
+            if isinstance(termination, str):
+                termination = add_tenor(effective, termination, modifier, self.calendar)
+
+            d = 1.0 / 360 if "360" in self.convention else 1.0 / 365
+
+            if self.multi_csa:
+                n = (termination - effective).days
+                # TODO when these discount factors are looked up the curve repeats
+                # the lookup could be vectorised to return two values at once.
+                df_num = self[effective]
+                df_den = self[termination]
+                _ = (df_num / df_den - 1) * 100 / (d * n)
+
+            elif approximate:
+                # calculates the geometric mean overnight rates in periods and adds
+                _, n = 0.0, (termination - effective).days
+                for curve_ in self.curves:
+                    r = curve_.rate(effective, termination)
+                    _ += ((1 + r * n * d / 100) ** (1 / n) - 1) / d
+
+                _ = ((1 + d * _) ** n - 1) * 100 / (d * n)
+
+            else:
+                _, dcf_ = 1.0, 0.0
+                date_ = effective
+                while date_ < termination:
+                    term_ = add_tenor(date_, "1B", None, self.calendar)
+                    __, d_ = 0.0, (term_ - date_).days * d
+                    dcf_ += d_
+                    for curve in self.curves:
+                        __ += curve.rate(date_, term_)
+                    _ *= 1 + d_ * __ / 100
+                    date_ = term_
+                _ = 100 * (_ - 1) / dcf_
+        else:
+            raise TypeError(  # pragma: no cover
+                f"Base curve type is unrecognised: {self._base_type}"
+            )
+
+        return _
+
+    def __getitem__(self, date: datetime):
+        if self._base_type == "dfs":
+            # will return a composited discount factor
+            days = (date - self.curves[0].node_dates[0]).days
+            d = 1.0 / 360 if self.convention == "ACT360" else 1.0 / 365
+
+            if not self.multi_csa:
+                total_rate = 0.0
+                for curve in self.curves:
+                    avg_rate = ((1.0 / curve[date]) ** (1.0 / days) - 1) / d
+                    total_rate += avg_rate
+                _ = 1.0 / (1 + total_rate * d) ** days
+                return _
+            else:
+                # method uses the step and picks the highest (cheapest rate)
+                # in each period
+                _ = 1.0
+                d1 = self.curves[0].node_dates[0]
+
+                def _get_step(step):
+                    return min(
+                        max(step, self.multi_csa_min_step), self.multi_csa_max_step
+                    )
+
+                d2 = d1 + timedelta(days=_get_step(defaults.multi_csa_steps[0]))
+                # cache stores looked up DF values to next loop, avoiding double calc
+                cache, k = {i: 1.0 for i in range(len(self.curves))}, 1
+                while d2 < date:
+                    min_ratio = 1e5
+                    for i, curve in enumerate(self.curves):
+                        d2_df = curve[d2]
+                        ratio_ = d2_df / cache[i]
+                        min_ratio = ratio_ if ratio_ < min_ratio else min_ratio
+                        cache[i] = d2_df
+                    _ *= min_ratio
+                    try:
+                        step = _get_step(defaults.multi_csa_steps[k])
+                    except IndexError:
+                        step = self.multi_csa_max_step
+                    d1, d2, k = d2, d2 + timedelta(days=step), k + 1
+
+                # finish the loop on the correct date
+                if date == d1:
+                    return _
+                else:
+                    min_ratio = 1e5
+                    for i, curve in enumerate(self.curves):
+                        ratio_ = curve[date] / cache[i]  # cache[i] = curve[d1]
+                        min_ratio = ratio_ if ratio_ < min_ratio else min_ratio
+                    _ *= min_ratio
+                    return _
+
+        elif self._base_type == "values":
+            # will return a composited rate
+            _ = 0.0
+            for curve in self.curves:
+                _ += curve[date]
+            return _
+
+        else:
+            raise TypeError(  # pragma: no cover
+                f"Base curve type is unrecognised: {self._base_type}"
+            )
+
+    def shift(self, spread: float) -> CompositeCurve:
+        """
+        Create a new curve by vertically adjusting the curve by a set number of basis
+        points.
+
+        This curve adjustment preserves the shape of the curve but moves it up or
+        down as a translation.
+        This method is suitable as a way to assess value changes of instruments when
+        a parallel move higher or lower in yields is predicted.
+
+        Parameters
+        ----------
+        spread : float, Dual, Dual2
+            The number of basis points added to the existing curve.
+
+        Returns
+        -------
+        CompositeCurve
+        """
+        curves = (self.curves[0].shift(spread),)
+        curves += self.curves[1:]
+        return CompositeCurve(curves=curves)
+
+    def translate(self, start: datetime, t: bool = False) -> CompositeCurve:
+        """
+        Create a new curve with an initial node date moved forward keeping all else
+        constant.
+
+        This curve adjustment preserves forward curve expectations as time evolves.
+        This method is suitable as a way to create a subsequent *opening* curve from a
+        previous day's *closing* curve.
+
+        Parameters
+        ----------
+        start : datetime
+            The new initial node date for the curve, must be in the domain:
+            (node_date[0], node_date[1]]
+        t : bool
+            Set to *True* if the initial knots of the knot sequence should be
+            translated forward.
+
+        Returns
+        -------
+        CompositeCurve
+        """
+        return CompositeCurve(
+            curves=[curve.translate(start, t) for curve in self.curves]
+        )
+
+    def roll(self, tenor: Union[datetime, str]) -> CompositeCurve:
+        """
+        Create a new curve with its shape translated in time
+
+        This curve adjustment is a simulation of a future state of the market where
+        forward rates are assumed to have moved so that the present day's curve shape
+        is reflected in the future (or the past). This is often used in trade
+        strategy analysis.
+
+        Parameters
+        ----------
+        tenor : datetime or str
+            The date or tenor by which to roll the curve. If a tenor, as str, will
+            derive the datetime as measured from the initial node date. If supplying a
+            negative tenor, or a past datetime, there is a limit to how far back the
+            curve can be rolled - it will first roll backwards and then attempt to
+            :meth:`translate` forward to maintain the initial node date.
+
+        Returns
+        -------
+        CompositeCurve
+        """
+        return CompositeCurve(curves=[curve.roll(tenor) for curve in self.curves])
+
+
+def average_rate(effective, termination, convention, rate):
+    """
+    Return the geometric, 1 calendar day, average rate for the rate in a period.
+
+    This is used for approximations usually in combination with floating periods.
+
+    Parameters
+    ----------
+    effective : datetime
+        The effective date of the rate.
+    termination : datetime
+        The termination date of the rate.
+    convention : str
+        The day count convention of the curve rate.
+    rate : float, Dual, Dual2
+        The rate to decompose to average, in percentage terms, e.g. 0.04 = 4% rate.
+
+    Returns
+    -------
+    tuple : The rate, the 1-day DCF, and the number of calendar days
+    """
+    # TODO decide if the one-day DCF is properly accounted for here, e.g. 30e360?
+    # maybe just provide a static mapping instead.
+    d = 1.0 / 360 if "360" in convention else 1.0 / 365
+    n = (termination - effective).days
+    _ = ((1 + rate / 100 * n * d) ** (1 / n) - 1) / d
+    return _ * 100, d, n
 
 
 def interpolate(x, x_1, y_1, x_2, y_2, interpolation, start=None):
     """
     Perform local interpolation between two data points.
 
     Parameters
@@ -1468,19 +2249,19 @@
         y_2 = dual_log(y_2) / ((start - x_2) / timedelta(days=365))
         if start == x_1:
             y_1 = y_2
         else:
             y_1 = dual_log(y_1) / ((start - x_1) / timedelta(days=365))
         op = lambda z: dual_exp((start - x) / timedelta(days=365) * z)
     elif interpolation == "flat_forward":
-        if x == x_2:
+        if x >= x_2:
             return y_2
         return y_1
     elif interpolation == "flat_backward":
-        if x == x_1:
+        if x <= x_1:
             return y_1
         return y_2
     ret = op(y_1 + (y_2 - y_1) * ((x - x_1) / (x_2 - x_1)))
     return ret
 
 
 def index_left(
```

### Comparing `rateslib-0.2.0/rateslib/default.py` & `rateslib-0.3.0/rateslib/default.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,30 +12,34 @@
 
     convention = "ACT360"
     notional = 1.0e6
     stub = "SHORTFRONT"
     stub_length = "SHORT"
     modifier = "MF"
     index_lag = 3
+    index_method = "daily"
     payment_lag = 2
     payment_lag_exchange = 0
     payment_lag_specific = {
         "IRS": 2,
+        "IIRS": 2,
         "ZCS": 2,
+        "ZCIS": 0,
         "FXSwap": 0,
         "SBS": 2,
         "Swap": 2,
         "NonMtmXCS": 2,
         "NonMtmFixedFloatXCS": 2,
         "NonMtmFixedFixedXCS": 2,
         "XCS": 2,
         "FixedFloatXCS": 2,
         "FixedFixedXCS": 2,
         "FloatFixedXCS": 2,
         "FixedRateBond": 0,
+        "IndexFixedRateBond": 0,
         "FloatRateBond": 0,
         "Bill": 0,
         "FRA": 0,
     }
     calendar = BusinessDay()
     interpolation = {
         "Curve": "log_linear",
@@ -83,17 +87,28 @@
         "npv": "NPV",
         "cashflow": "Cashflow",
         "fx": "FX Rate",
         "npv_fx": "NPV Ccy",
         "real_cashflow": "Real Cashflow",
         "index_value": "Index Val",
         "index_ratio": "Index Ratio",
+        "index_base": "Index Base",
     }
+    algorithm = "gauss_newton"
     curve_not_in_solver = "ignore"
     no_fx_fixings_for_xcs = "warn"
+    pool = 1
+
+    # fmt: off
+    multi_csa_steps = [
+       2, 5, 10, 20, 30, 50, 77, 81, 86, 91, 96, 103, 110, 119, 128, 140, 153,
+       169, 188, 212, 242, 281, 332, 401, 498, 636, 835, 1104, 1407, 1646, 1766,
+       1808, 1821, 1824, 1825,
+    ]
+    # fmt: on
 
     # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
     # Commercial use of this code, and/or copying and redistribution is prohibited.
     # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
     def reset_defaults(self):
         base = Defaults()
```

### Comparing `rateslib-0.2.0/rateslib/dual.py` & `rateslib-0.3.0/rateslib/dual.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,18 @@
     """
     Base class for dual number implementation.
     """
 
     dual: np.ndarray = np.zeros(0)
     dual2: np.ndarray = np.zeros(0)
 
-    def __init__(self, real: float, vars: tuple[str, ...] = tuple()):
+    def __init__(
+        self, real: float, vars: tuple[str, ...] = tuple()
+    ) -> None:  # pragma: no cover
+        # each dual overloads init
         self.real: float = real
         self.vars: tuple[str, ...] = vars
 
     def __float__(self):
         return float(self.real)
 
     def __abs__(self):
@@ -69,27 +72,29 @@
             return False
         elif not np.all(np.isclose(self.dual, argument.dual, atol=PRECISION)):
             return False
         if type(self) is Dual2 and type(argument) is Dual2:
             if not np.all(np.isclose(self.dual2, argument.dual2, atol=PRECISION)):
                 return False
         elif type(self) is Dual2 or type(argument) is Dual2:
-            return False  # cannot compare Dual with Dual2
+            # this line should not be hit TypeError should raise earlier
+            # cannot compare Dual with Dual2
+            return False  # pragma: no cover
         return True
 
     def __upcast_combined__(self, arg):
         """Combines, and inserts, the vars of two Dual numbers to match each other."""
         new_vars = sorted(list(set(self.vars).union(set(arg.vars))))
         new_self = self if new_vars == self.vars else self.__upcast_vars__(new_vars)
         new_arg = arg if new_vars == arg.vars else arg.__upcast_vars__(new_vars)
         return new_self, new_arg
 
     @abstractmethod
     def __upcast_vars__(self, new_vars: list[str]):
-        pass
+        pass  # pragma: no cover
 
     def gradient(self, vars=None, order=1, keep_manifold=False):
         """
         Return derivatives of a dual number.
 
         Parameters
         ----------
@@ -711,12 +716,45 @@
     """
     if isinstance(val, (*FLOATS, *INTS)):
         return val
     elif isinstance(val, (Dual, Dual2)):
         return val._set_order(order)
 
 
+def set_order_convert(val, order, tag):
+    """
+    Convert a float, :class:`Dual` or :class:`Dual2` type to a specified alternate type.
+
+    Parameters
+    ----------
+    val : float, Dual or Dual2
+        The value to convert.
+    order : int
+        The AD order to convert the value to if necessary.
+    tag : str
+        The variable name if upcasting a float to a Dual or Dual2
+
+    Returns
+    -------
+    float, Dual, Dual2
+    """
+    if isinstance(val, (*FLOATS, *INTS)):
+        if order == 0:
+            return val
+        elif order == 1:
+            return Dual(val, tag)
+        elif order == 2:
+            return Dual2(val, tag)
+    elif isinstance(val, (Dual, Dual2)):
+        if order == 0:
+            return float(val)
+        elif (order == 1 and isinstance(val, Dual)) \
+                or (order == 2 and isinstance(val, Dual2)):
+            return val
+        else:
+            return val._set_order(order)
+
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
 DualTypes = Union[float, Dual, Dual2]
```

### Comparing `rateslib-0.2.0/rateslib/fx.py` & `rateslib-0.3.0/rateslib/fx.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import numpy as np
 from pandas import DataFrame, Series
 from pandas.tseries.offsets import CustomBusinessDay
 from itertools import product
 import warnings
 from datetime import timedelta, datetime
 import json
+from uuid import uuid4
 
 from rateslib import defaults
 from rateslib.dual import Dual, dual_solve, set_order, DualTypes
 from rateslib.default import plot
 from rateslib.calendars import add_tenor, CalInput
 from rateslib.curves import Curve, LineCurve
 
@@ -1427,14 +1428,15 @@
     def curve(
         self,
         cashflow: str,
         collateral: str,
         convention: Optional[str] = None,
         modifier: Optional[Union[str, bool]] = False,
         calendar: Optional[Union[CustomBusinessDay, str, bool]] = False,
+        id: Optional[str] = None,
     ):
         """
         Return a cash collateral curve.
 
         Parameters
         ----------
         cashflow : str
@@ -1448,14 +1450,16 @@
         modifier : str, optional
             The modification rule, in {"F", "MF", "P", "MP"}, for determining rates.
             If `False` will default to the modifier in the local cashflow currency.
         calendar : calendar or str, optional
             The holiday calendar object to use. If str, lookups named calendar
             from static data. Used for determining rates. If `False` will
             default to the calendar in the local cashflow currency.
+        id : str, optional
+            The identifier attached to any constructed :class:`~rateslib.fx.ProxyCurve`.
 
         Returns
         -------
         Curve or ProxyCurve
 
         Notes
         -----
@@ -1481,14 +1485,15 @@
         return ProxyCurve(
             cashflow=cash_ccy,
             collateral=coll_ccy,
             fx_forwards=self,
             convention=convention,
             modifier=modifier,
             calendar=calendar,
+            id=id,
         )
 
     def plot(
         self,
         pair: str,
         right: Optional[Union[datetime, str]] = None,
         left: Optional[Union[datetime, str]] = None,
@@ -1643,16 +1648,16 @@
         An FXForwards copy creates a new object with copied references.
         """
         return self.from_json(self.to_json())
 
 
 class ProxyCurve(Curve):
     """
-    Create a curve which is defined by other curves and related via
-    :class:`~rateslib.fx.FXForwards`.
+    A subclass of :class:`~rateslib.curves.Curve` which returns dynamic DFs based on
+    other curves related via :class:`~rateslib.fx.FXForwards` parity.
 
     Parameters
     ----------
     cashflow : str
         The currency in which cashflows are represented (3-digit code).
     collateral : str
         The currency of the CSA against which cashflows are collateralised (3-digit
@@ -1666,14 +1671,16 @@
     modifier : str, optional
         The modification rule, in {"F", "MF", "P", "MP"}, for determining rates.
         If `False` will default to the modifier in the local cashflow currency.
     calendar : calendar or str, optional
         The holiday calendar object to use. If str, lookups named calendar
         from static data. Used for determining rates. If `False` will
         default to the calendar in the local cashflow currency.
+    id : str, optional, set by Default
+        The unique identifier to distinguish between curves in a multi-curve framework.
 
     Notes
     -----
     The DFs returned are calculated via the chaining method and the below formula,
     relating the DF curve in the local collateral currency and FX forward rates.
 
     .. math::
@@ -1681,23 +1688,27 @@
        w_{dom:for,i} = \\frac{f_{DOMFOR,i}}{F_{DOMFOR,0}} v_{for:for,i}
 
     The returned curve contains contrived methods to calculate this dynamically and
     efficiently from the combination of curves and FX rates that are available within
     the given :class:`FXForwards` instance.
     """
 
+    _base_type = "dfs"
+
     def __init__(
         self,
         cashflow: str,
         collateral: str,
         fx_forwards: FXForwards,
         convention: Optional[str] = None,
         modifier: Optional[Union[str, bool]] = False,
         calendar: Optional[Union[CalInput, bool]] = False,
+        id: Optional[str]=None,
     ):
+        self.id = id or uuid4().hex[:5] + "_"  # 1 in a million clash
         cash_ccy, coll_ccy = cashflow.lower(), collateral.lower()
         self._is_proxy = True
         self.fx_forwards = fx_forwards
         self.cash_currency = cash_ccy
         self.cash_pair = f"{cash_ccy}{cash_ccy}"
         self.cash_idx = self.fx_forwards.currencies[cash_ccy]
         self.coll_currency = coll_ccy
```

### Comparing `rateslib-0.2.0/rateslib/instruments.py` & `rateslib-0.3.0/rateslib/instruments.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,28 +32,32 @@
 # from scipy.optimize import brentq
 from pandas.tseries.offsets import CustomBusinessDay
 from pandas import DataFrame, concat, date_range, Series
 
 from rateslib import defaults
 from rateslib.calendars import add_tenor, _add_days, get_calendar, dcf
 from rateslib.scheduling import Schedule
-from rateslib.curves import Curve, index_left, LineCurve
+from rateslib.curves import Curve, index_left, LineCurve, CompositeCurve, IndexCurve
 from rateslib.solver import Solver
-from rateslib.periods import Cashflow, FixedPeriod, FloatPeriod, _get_fx_and_base
+from rateslib.periods import Cashflow, FixedPeriod, FloatPeriod, _get_fx_and_base, IndexMixin
 from rateslib.legs import (
     FixedLeg,
     FixedLegExchange,
     FloatLeg,
     FloatLegExchange,
     FloatLegExchangeMtm,
     FixedLegExchangeMtm,
     ZeroFloatLeg,
+    ZeroFixedLeg,
+    ZeroIndexLeg,
+    IndexFixedLeg,
+    IndexFixedLegExchange,
     CustomLeg,
 )
-from rateslib.dual import Dual, Dual2, set_order
+from rateslib.dual import Dual, Dual2, set_order, DualTypes
 from rateslib.fx import FXForwards, FXRates
 
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
@@ -131,15 +135,15 @@
         fx_ = fx
 
     if curves is None and curves_attr is None:
         return (None, None, None, None), fx_
     elif curves is None:
         curves = curves_attr
 
-    if isinstance(curves, (Curve, str)):
+    if isinstance(curves, (Curve, str, CompositeCurve)):
         curves = [curves]
     if solver is None:
 
         def check_curve(curve):
             if isinstance(curve, str):
                 raise ValueError(
                     "`curves` must contain Curve, not str, if `solver` not given."
@@ -283,14 +287,15 @@
         Returns
         -------
         DataFrame
         """
         if solver is None:
             raise ValueError("`solver` is required for delta/gamma methods.")
         npv = self.npv(curves, solver, fx, base, local=True)
+        _, fx = _get_curves_and_fx_maybe_from_solver(None, solver, None, fx)
         return solver.delta(npv, base, fx)
 
     def gamma(
         self,
         curves: Optional[Union[Curve, str, list]] = None,
         solver: Optional[Solver] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
@@ -326,27 +331,42 @@
 
         Returns
         -------
         DataFrame
         """
         if solver is None:
             raise ValueError("`solver` is required for delta/gamma methods.")
-        _ = solver._ad  # store original order
+        _, fx_ = _get_curves_and_fx_maybe_from_solver(None, solver, None, fx)
+
+        # store original order
+        if fx_ is not None:
+            _ad2 = fx_._ad
+            fx_._set_ad_order(2)
+
+        _ad1 = solver._ad
         solver._set_ad_order(2)
-        npv = self.npv(curves, solver, fx, base, local=True)
-        grad_s_sT_P = solver.gamma(npv, base, fx)
-        solver._set_ad_order(_)  # reset original order
+
+        npv = self.npv(curves, solver, fx_, base, local=True)
+        grad_s_sT_P = solver.gamma(npv, base, fx_)
+
+        # reset original order
+        if fx_ is not None:
+            fx_._set_ad_order(_ad2)
+        solver._set_ad_order(_ad1)
+
         return grad_s_sT_P
 
 
 class BaseMixin:
     _fixed_rate_mixin = False
     _float_spread_mixin = False
     _leg2_fixed_rate_mixin = False
     _leg2_float_spread_mixin = False
+    _index_base_mixin = False
+    _leg2_index_base_mixin = False
     _rate_scalar = 1.0
 
     @property
     def fixed_rate(self):
         """
         float or None : If set will also set the ``fixed_rate`` of the contained
         leg1.
@@ -414,14 +434,60 @@
     @leg2_float_spread.setter
     def leg2_float_spread(self, value):
         if not self._leg2_float_spread_mixin:
             raise AttributeError("Cannot set `leg2_float_spread` for this Instrument.")
         self._leg2_float_spread = value
         self.leg2.float_spread = value
 
+    @property
+    def index_base(self):
+        """
+        float or None : If set will also set the ``index_base`` of the contained
+        leg1.
+
+        .. note::
+           ``fixed_rate``, ``float_spread``, ``leg2_fixed_rate`` and
+           ``leg2_float_spread`` are attributes only applicable to certain
+           ``Instruments``. *AttributeErrors* are raised if calling or setting these
+           is invalid.
+
+        """
+        # TODO: re-write these docstrings to include index base mixin
+        return self._index_base
+
+    @index_base.setter
+    def index_base(self, value):
+        if not self._index_base_mixin:
+            raise AttributeError("Cannot set `index_base` for this Instrument.")
+        self._index_base = value
+        self.leg1.index_base = value
+
+    @property
+    def leg2_index_base(self):
+        """
+        float or None : If set will also set the ``index_base`` of the contained
+        leg1.
+
+        .. note::
+           ``fixed_rate``, ``float_spread``, ``leg2_fixed_rate`` and
+           ``leg2_float_spread`` are attributes only applicable to certain
+           ``Instruments``. *AttributeErrors* are raised if calling or setting these
+           is invalid.
+
+        """
+        # TODO: re-write these docstrings to include index base mixin
+        return self._leg2_index_base
+
+    @leg2_index_base.setter
+    def leg2_index_base(self, value):
+        if not self._leg2_index_base_mixin:
+            raise AttributeError("Cannot set `leg2_index_base` for this Instrument.")
+        self._leg2_index_base = value
+        self.leg2.index_base = value
+
 
 class Value(BaseMixin):
     """
     A null instrument which can be used within a :class:`~rateslib.solver.Solver`
     to directly parametrise a node.
 
     Parameters
@@ -482,14 +548,20 @@
         return curves[0][self.effective]
 
 
 ### Securities
 
 
 class BondMixin:
+    def _set_base_index_if_none(self, curve: IndexCurve):
+        if self._index_base_mixin and self.index_base is None:
+            self.leg1.index_base = curve.index_value(
+                self.leg1.schedule.effective, self.leg1.index_method
+            )
+
     def ex_div(self, settlement: datetime):
         """
         Return a boolean whether the security is ex-div on the settlement.
 
         Parameters
         ----------
         settlement : datetime
@@ -518,21 +590,19 @@
         coupon period left index
         """
         acc_idx = index_left(
             self.leg1.schedule.aschedule,
             len(self.leg1.schedule.aschedule),
             settlement,
         )
-        return (
-            (settlement - self.leg1.schedule.aschedule[acc_idx])
-            / (
-                self.leg1.schedule.aschedule[acc_idx + 1]
-                - self.leg1.schedule.aschedule[acc_idx]
-            )
-        ), acc_idx
+        _ = (settlement - self.leg1.schedule.aschedule[acc_idx]) / (
+            self.leg1.schedule.aschedule[acc_idx + 1]
+            - self.leg1.schedule.aschedule[acc_idx]
+        )
+        return _, acc_idx
 
     def _npv_local(
         self,
         curve: Union[Curve, LineCurve],
         disc_curve: Curve,
         fx: Optional[Union[float, FXRates, FXForwards]],
         base: Optional[str],
@@ -572,14 +642,15 @@
         -----
         The cashflows for determination (excluding an ``ex_div`` cashflow) are
         evaluated by ``settlement``.
 
         The date for which the PV is returned is by ``projection``, and not the
         initial node date of the ``disc_curve``.
         """
+        self._set_base_index_if_none(curve)
         npv = self.leg1.npv(curve, disc_curve, fx, base)
 
         # now must systematically deduct any cashflow between the initial node date
         # and the settlement date, including the cashflow after settlement if ex_div.
         initial_idx = index_left(
             self.leg1.schedule.aschedule,
             self.leg1.schedule.n_periods + 1,
@@ -600,341 +671,14 @@
             npv -= self.leg1.periods[settle_idx].npv(curve, disc_curve, fx, base)
 
         if projection is None:
             return npv
         else:
             return npv / disc_curve[projection]
 
-    def npv(
-        self,
-        curves: Optional[Union[Curve, str, list]] = None,
-        solver: Optional[Solver] = None,
-        fx: Optional[Union[float, FXRates, FXForwards]] = None,
-        base: Optional[str] = None,
-        local: bool = False,
-    ):
-        """
-        Return the NPV of the security by summing cashflow valuations.
-
-        Parameters
-        ----------
-        curves : Curve, str or list of such
-            A single :class:`Curve` or id or a list of such. A list defines the
-            following curves in the order:
-
-              - Forecasting :class:`Curve` for ``leg1``.
-              - Discounting :class:`Curve` for ``leg1``.
-        solver : Solver, optional
-            The numerical :class:`Solver` that constructs ``Curves`` from calibrating
-            instruments.
-        fx : float, FXRates, FXForwards, optional
-            The immediate settlement FX rate that will be used to convert values
-            into another currency. A given `float` is used directly. If giving a
-            ``FXRates`` or ``FXForwards`` object, converts from local currency
-            into ``base``.
-        base : str, optional
-            The base currency to convert cashflows into (3-digit code), set by default.
-            Only used if ``fx`` is an ``FXRates`` or ``FXForwards`` object.
-        local : bool, optional
-            If `True` will ignore the ``base`` request and return a dict identifying
-            local currency NPV.
-
-        Returns
-        -------
-        float, Dual, Dual2 or dict of such
-
-        Notes
-        -----
-        The ``settlement`` date of the bond is inferred from the objects ``settle``
-        days parameter and the initial date of the supplied ``curves``.
-        The NPV returned is for immediate settlement.
-
-        If **only one curve** is given this is used as all four curves.
-
-        If **two curves** are given the forecasting curve is used as the forecasting
-        curve on both legs and the discounting curve is used as the discounting
-        curve for both legs.
-        """
-        curves, fx = _get_curves_and_fx_maybe_from_solver(
-            self.curves, solver, curves, fx
-        )
-        settlement = add_tenor(
-            curves[1].node_dates[0],
-            f"{self.settle}B",
-            None,
-            self.leg1.schedule.calendar,
-        )
-        base = self.leg1.currency if local else base
-        npv = self._npv_local(curves[0], curves[1], fx, base, settlement, None)
-        if local:
-            return {self.leg1.currency: npv}
-        else:
-            return npv
-
-    def analytic_delta(
-        self,
-        curve: Optional[Curve] = None,
-        disc_curve: Optional[Curve] = None,
-        fx: Union[float, FXRates, FXForwards] = 1.0,
-        base: Optional[str] = None,
-    ):
-        """
-        Return the analytic delta of the security via summing all periods.
-
-        Parameters
-        ----------
-        curve : Curve
-            The forecasting curve object. Not used unless it is set equal to
-            ``disc_curve``.
-        disc_curve : Curve, optional
-            The discounting curve object used in calculations.
-            Set equal to ``curve`` if not given.
-        fx : float, FXRates, FXForwards, optional
-            The immediate settlement FX rate that will be used to convert values
-            into another currency. A given `float` is used directly. If giving a
-            :class:`~rateslib.fx.FXRates` or :class:`~rateslib.fx.FXForwards`
-            object, converts from local currency into ``base``.
-        base : str, optional
-            The base currency to convert cashflows into (3-digit code), set by default.
-            Only used if ``fx`` is an :class:`~rateslib.fx.FXRates` or
-            :class:`~rateslib.fx.FXForwards` object.
-
-        Returns
-        -------
-        float, Dual, Dual2
-        """
-        disc_curve = disc_curve or curve
-        settlement = add_tenor(
-            disc_curve.node_dates[0],
-            f"{self.settle}B",
-            None,
-            self.leg1.schedule.calendar,
-        )
-        a_delta = self.leg1.analytic_delta(curve, disc_curve, fx, base)
-        if self.ex_div(settlement):
-            # deduct the next coupon which has otherwise been included in valuation
-            current_period = index_left(
-                self.leg1.schedule.aschedule,
-                self.leg1.schedule.n_periods + 1,
-                settlement,
-            )
-            a_delta -= self.leg1.periods[current_period].analytic_delta(
-                curve, disc_curve, fx, base
-            )
-        return a_delta
-
-    def cashflows(
-        self,
-        curves: Optional[Union[Curve, str, list]] = None,
-        solver: Optional[Solver] = None,
-        fx: Optional[Union[float, FXRates, FXForwards]] = None,
-        base: Optional[str] = None,
-        settlement: datetime = None,
-    ):
-        """
-        Return the properties of the security used in calculating cashflows.
-
-        Parameters
-        ----------
-        curves : Curve, str or list of such
-            A single :class:`Curve` or id or a list of such. A list defines the
-            following curves in the order:
-
-              - Forecasting :class:`Curve` for ``leg1``.
-              - Discounting :class:`Curve` for ``leg1``.
-        solver : Solver, optional
-            The numerical :class:`Solver` that constructs ``Curves`` from calibrating
-            instruments.
-        fx : float, FXRates, FXForwards, optional
-            The immediate settlement FX rate that will be used to convert values
-            into another currency. A given `float` is used directly. If giving a
-            ``FXRates`` or ``FXForwards`` object, converts from local currency
-            into ``base``.
-        base : str, optional
-            The base currency to convert cashflows into (3-digit code), set by default.
-            Only used if ``fx_rate`` is an ``FXRates`` or ``FXForwards`` object.
-        settlement : datetime, optional
-            The settlement date of the security. If *None* adds the regular ``settle``
-            time to the initial node date of the given discount ``curves``.
-
-        Returns
-        -------
-        DataFrame
-        """
-        curves, fx = _get_curves_and_fx_maybe_from_solver(
-            self.curves, solver, curves, fx
-        )
-        if settlement is None:
-            settlement = add_tenor(
-                curves[1].node_dates[0],
-                f"{self.settle}B",
-                None,
-                self.leg1.schedule.calendar,
-            )
-        cashflows = self.leg1.cashflows(curves[0], curves[1], fx, base)
-        if self.ex_div(settlement):
-            # deduct the next coupon which has otherwise been included in valuation
-            current_period = index_left(
-                self.leg1.schedule.aschedule,
-                self.leg1.schedule.n_periods + 1,
-                settlement,
-            )
-            cashflows.loc[current_period, defaults.headers["npv"]] = 0
-            cashflows.loc[current_period, defaults.headers["npv_fx"]] = 0
-        return cashflows
-
-
-class FixedRateBond(Sensitivities, BondMixin, BaseMixin):
-    # TODO ensure calculations work for amortizing bonds.
-    """
-    Create a fixed rate bond security.
-
-    Parameters
-    ----------
-    effective : datetime
-        The adjusted or unadjusted effective date.
-    termination : datetime or str
-        The adjusted or unadjusted termination date. If a string, then a tenor must be
-        given expressed in days (`"D"`), months (`"M"`) or years (`"Y"`), e.g. `"48M"`.
-    frequency : str in {"M", "B", "Q", "T", "S", "A"}, optional
-        The frequency of the schedule. "Z" is not permitted.
-    stub : str combining {"SHORT", "LONG"} with {"FRONT", "BACK"}, optional
-        The stub type to enact on the swap. Can provide two types, for
-        example "SHORTFRONTLONGBACK".
-    front_stub : datetime, optional
-        An adjusted or unadjusted date for the first stub period.
-    back_stub : datetime, optional
-        An adjusted or unadjusted date for the back stub period.
-        See notes for combining ``stub``, ``front_stub`` and ``back_stub``
-        and any automatic stub inference.
-    roll : int in [1, 31] or str in {"eom", "imm", "som"}, optional
-        The roll day of the schedule. Inferred if not given.
-    eom : bool, optional
-        Use an end of month preference rather than regular rolls for inference. Set by
-        default. Not required if ``roll`` is specified.
-    modifier : str, optional
-        The modification rule, in {"F", "MF", "P", "MP"}
-    calendar : calendar or str, optional
-        The holiday calendar object to use. If str, looks up named calendar from
-        static data.
-    payment_lag : int, optional
-        The number of business days to lag payments by.
-    notional : float, optional
-        The leg notional, which is applied to each period.
-    currency : str, optional
-        The currency of the leg (3-digit code).
-    amortization: float, optional
-        The amount by which to adjust the notional each successive period. Should have
-        sign equal to that of notional if the notional is to reduce towards zero.
-    convention: str, optional
-        The day count convention applied to calculations of period accrual dates.
-        See :meth:`~rateslib.calendars.dcf`.
-    fixed_rate : float, optional
-        The **coupon** rate applied to determine cashflows. Can be set
-        to `None` and designated
-        later, perhaps after a mid-market rate for all periods has been calculated.
-    ex_div : int
-        The number of days prior to a cashflow during which the bond is considered
-        ex-dividend.
-    settle : int
-        The number of business days for regular settlement time, i.e, 1 is T+1.
-
-    Attributes
-    ----------
-    ex_div_days : int
-    leg1 : FixedLegExchange
-    """
-    _fixed_rate_mixin = True
-
-    def __init__(
-        self,
-        effective: datetime,
-        termination: Union[datetime, str] = None,
-        frequency: str = None,
-        stub: Optional[str] = None,
-        front_stub: Optional[datetime] = None,
-        back_stub: Optional[datetime] = None,
-        roll: Optional[Union[str, int]] = None,
-        eom: Optional[bool] = None,
-        modifier: Optional[str] = False,
-        calendar: Optional[Union[CustomBusinessDay, str]] = None,
-        payment_lag: Optional[int] = None,
-        notional: Optional[float] = None,
-        currency: Optional[str] = None,
-        amortization: Optional[float] = None,
-        convention: Optional[str] = None,
-        fixed_rate: Optional[float] = None,
-        ex_div: int = 0,
-        settle: int = 1,
-        curves: Optional[Union[list, str, Curve]] = None,
-    ):
-        self.curves = curves
-        if frequency.lower() == "z":
-            raise ValueError("FixedRateBond `frequency` must be in {M, B, Q, T, S, A}.")
-        if payment_lag is None:
-            payment_lag = defaults.payment_lag_specific[type(self).__name__]
-        self._fixed_rate = fixed_rate
-        self.ex_div_days = ex_div
-        self.settle = settle
-        self.leg1 = FixedLegExchange(
-            effective=effective,
-            termination=termination,
-            frequency=frequency,
-            stub=stub,
-            front_stub=front_stub,
-            back_stub=back_stub,
-            roll=roll,
-            eom=eom,
-            modifier=modifier,
-            calendar=calendar,
-            payment_lag=payment_lag,
-            payment_lag_exchange=payment_lag,
-            notional=notional,
-            currency=currency,
-            amortization=amortization,
-            convention=convention,
-            fixed_rate=fixed_rate,
-            initial_exchange=False,
-        )
-        if self.leg1.amortization != 0:
-            # Note if amortization is added to FixedRateBonds must systematically
-            # go through and update all methods. Many rely on the quantity
-            # self.notional which is currently assumed to be a fixed quantity
-            raise NotImplementedError("`amortization` for FixedRateBond must be zero.")
-
-    def accrued(self, settlement: datetime):
-        """
-        Calculate the accrued amount per nominal par value of 100.
-
-        Parameters
-        ----------
-        settlement : datetime
-            The settlement date which to measure accrued interest against.
-
-        Notes
-        -----
-        Fractionally apportions the coupon payment based on calendar days.
-
-        .. math::
-
-           \\text{Accrued} = \\text{Coupon} \\times \\frac{\\text{Settle - Last Coupon}}{\\text{Next Coupon - Last Coupon}}
-
-        """
-        # TODO validate against effective and termination?
-        frac, acc_idx = self._accrued_frac(settlement)
-        if self.ex_div(settlement):
-            frac = frac - 1  # accrued is negative in ex-div period
-        return frac * self.leg1.periods[acc_idx].cashflow / -self.leg1.notional * 100
-
-    # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
-    # Commercial use of this code, and/or copying and redistribution is prohibited.
-    # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
-
-    # Analogue Methods
-
     def _price_from_ytm(self, ytm: float, settlement: datetime, dirty: bool = False):
         """
         Loop through all future cashflows and discount them with ``ytm`` to achieve
         correct price.
         """
         # TODO note this formula does not account for back stubs
         # this is also mentioned in Coding IRs
@@ -947,22 +691,23 @@
             # is a stub so must account for discounting in a different way.
             fd0 = self.leg1.periods[acc_idx].dcf * f * (1 - acc_frac)
         else:
             fd0 = 1 - acc_frac
 
         d = 0
         for i, p_idx in enumerate(
-            range(acc_idx, len(self.leg1.schedule.aschedule) - 1)
+                range(acc_idx, len(self.leg1.schedule.aschedule) - 1)
         ):
             if i == 0 and self.ex_div(settlement):
                 continue
             else:
-                d += self.leg1.periods[p_idx].cashflow * v**i
-        d += self.leg1.periods[-1].cashflow * v**i
-        p = v**fd0 * d / -self.leg1.notional * 100
+                d += getattr(self.leg1.periods[p_idx], self._ytm_attribute) * v ** i
+                # d += self.leg1.periods[p_idx].cashflow * v ** i
+        d += getattr(self.leg1.periods[-1], self._ytm_attribute) * v ** i
+        p = v ** fd0 * d / -self.leg1.notional * 100
         return p if dirty else p - self.accrued(settlement)
 
     def price(self, ytm: float, settlement: datetime, dirty: bool = False):
         """
         Calculate the price of the security per nominal value of 100, given
         yield-to-maturity.
 
@@ -1217,29 +962,29 @@
             d2ydP2 = -p.gradient("y", order=2)[0][0] * p.gradient("y")[0] ** -3
             return Dual2(
                 x,
                 price.vars,
                 dydP * price.dual,
                 0.5
                 * (
-                    dydP * price.gradient(price.vars, order=2)
-                    + d2ydP2 * np.matmul(price.dual[:, None], price.dual[None, :])
+                        dydP * price.gradient(price.vars, order=2)
+                        + d2ydP2 * np.matmul(price.dual[:, None], price.dual[None, :])
                 ),
             )
         else:
             return x
 
     def fwd_from_repo(
-        self,
-        price: Union[float, Dual, Dual2],
-        settlement: datetime,
-        forward_settlement: datetime,
-        repo_rate: Union[float, Dual, Dual2],
-        convention: Optional[str] = None,
-        dirty: bool = False,
+            self,
+            price: Union[float, Dual, Dual2],
+            settlement: datetime,
+            forward_settlement: datetime,
+            repo_rate: Union[float, Dual, Dual2],
+            convention: Optional[str] = None,
+            dirty: bool = False,
     ):
         """
         Return a forward price implied by a given repo rate.
 
         Parameters
         ----------
         price : float, Dual, or Dual2
@@ -1294,32 +1039,32 @@
         # deduct final coupon if received within period
         fwd_settlement_idx += 1 if self.ex_div(forward_settlement) else 0
 
         for p_idx in range(settlement_idx, fwd_settlement_idx):
             # deduct accrued coupon from dirty price
             dcf_ = dcf(self.leg1.periods[p_idx].payment, forward_settlement, convention)
             accrued_coup = self.leg1.periods[p_idx].cashflow * (
-                1 + dcf_ * repo_rate / 100
+                    1 + dcf_ * repo_rate / 100
             )
             total_rtn -= accrued_coup
 
         forward_price = total_rtn / -self.leg1.notional * 100
         if dirty:
             return forward_price
         else:
             return forward_price - self.accrued(forward_settlement)
 
     def repo_from_fwd(
-        self,
-        price: Union[float, Dual, Dual2],
-        settlement: datetime,
-        forward_settlement: datetime,
-        forward_price: Union[float, Dual, Dual2],
-        convention: Optional[str] = None,
-        dirty: bool = False,
+            self,
+            price: Union[float, Dual, Dual2],
+            settlement: datetime,
+            forward_settlement: datetime,
+            forward_price: Union[float, Dual, Dual2],
+            convention: Optional[str] = None,
+            dirty: bool = False,
     ):
         """
         Return an implied repo rate from a forward price.
 
         Parameters
         ----------
         price : float, Dual, or Dual2
@@ -1375,19 +1120,435 @@
         fwd_settlement_idx += 1 if self.ex_div(forward_settlement) else 0
 
         for p_idx in range(settlement_idx, fwd_settlement_idx):
             # deduct accrued coupon from dirty price
             dcf_ = dcf(self.leg1.periods[p_idx].payment, forward_settlement, convention)
             numerator += 100 * self.leg1.periods[p_idx].cashflow / -self.leg1.notional
             denominator -= (
-                100 * dcf_ * self.leg1.periods[p_idx].cashflow / -self.leg1.notional
+                    100 * dcf_ * self.leg1.periods[p_idx].cashflow / -self.leg1.notional
             )
 
         return numerator / denominator * 100
 
+    def accrued(self, settlement: datetime):
+        """
+        Calculate the accrued amount per nominal par value of 100.
+
+        Parameters
+        ----------
+        settlement : datetime
+            The settlement date which to measure accrued interest against.
+
+        Notes
+        -----
+        Fractionally apportions the coupon payment based on calendar days.
+
+        .. math::
+
+           \\text{Accrued} = \\text{Coupon} \\times \\frac{\\text{Settle - Last Coupon}}{\\text{Next Coupon - Last Coupon}}
+
+        """
+        # TODO validate against effective and termination?
+        frac, acc_idx = self._accrued_frac(settlement)
+        if self.ex_div(settlement):
+            frac = frac - 1  # accrued is negative in ex-div period
+        _ = getattr(self.leg1.periods[acc_idx], self._ytm_attribute)
+        return frac * _ / -self.leg1.notional * 100
+
+    def npv(
+        self,
+        curves: Optional[Union[Curve, str, list]] = None,
+        solver: Optional[Solver] = None,
+        fx: Optional[Union[float, FXRates, FXForwards]] = None,
+        base: Optional[str] = None,
+        local: bool = False,
+    ):
+        """
+        Return the NPV of the security by summing cashflow valuations.
+
+        Parameters
+        ----------
+        curves : Curve, str or list of such
+            A single :class:`Curve` or id or a list of such. A list defines the
+            following curves in the order:
+
+              - Forecasting :class:`Curve` for ``leg1``.
+              - Discounting :class:`Curve` for ``leg1``.
+        solver : Solver, optional
+            The numerical :class:`Solver` that constructs ``Curves`` from calibrating
+            instruments.
+        fx : float, FXRates, FXForwards, optional
+            The immediate settlement FX rate that will be used to convert values
+            into another currency. A given `float` is used directly. If giving a
+            ``FXRates`` or ``FXForwards`` object, converts from local currency
+            into ``base``.
+        base : str, optional
+            The base currency to convert cashflows into (3-digit code), set by default.
+            Only used if ``fx`` is an ``FXRates`` or ``FXForwards`` object.
+        local : bool, optional
+            If `True` will ignore the ``base`` request and return a dict identifying
+            local currency NPV.
+
+        Returns
+        -------
+        float, Dual, Dual2 or dict of such
+
+        Notes
+        -----
+        The ``settlement`` date of the bond is inferred from the objects ``settle``
+        days parameter and the initial date of the supplied ``curves``.
+        The NPV returned is for immediate settlement.
+
+        If **only one curve** is given this is used as all four curves.
+
+        If **two curves** are given the forecasting curve is used as the forecasting
+        curve on both legs and the discounting curve is used as the discounting
+        curve for both legs.
+        """
+        curves, fx = _get_curves_and_fx_maybe_from_solver(
+            self.curves, solver, curves, fx
+        )
+        settlement = add_tenor(
+            curves[1].node_dates[0],
+            f"{self.settle}B",
+            None,
+            self.leg1.schedule.calendar,
+        )
+        base = self.leg1.currency if local else base
+        npv = self._npv_local(curves[0], curves[1], fx, base, settlement, None)
+        if local:
+            return {self.leg1.currency: npv}
+        else:
+            return npv
+
+    def analytic_delta(
+        self,
+        curve: Optional[Curve] = None,
+        disc_curve: Optional[Curve] = None,
+        fx: Union[float, FXRates, FXForwards] = 1.0,
+        base: Optional[str] = None,
+    ):
+        """
+        Return the analytic delta of the security via summing all periods.
+
+        For arguments see :meth:`~rateslib.periods.BasePeriod.analytic_delta`.
+        """
+        disc_curve = disc_curve or curve
+        settlement = add_tenor(
+            disc_curve.node_dates[0],
+            f"{self.settle}B",
+            None,
+            self.leg1.schedule.calendar,
+        )
+        a_delta = self.leg1.analytic_delta(curve, disc_curve, fx, base)
+        if self.ex_div(settlement):
+            # deduct the next coupon which has otherwise been included in valuation
+            current_period = index_left(
+                self.leg1.schedule.aschedule,
+                self.leg1.schedule.n_periods + 1,
+                settlement,
+            )
+            a_delta -= self.leg1.periods[current_period].analytic_delta(
+                curve, disc_curve, fx, base
+            )
+        return a_delta
+
+    def cashflows(
+        self,
+        curves: Optional[Union[Curve, str, list]] = None,
+        solver: Optional[Solver] = None,
+        fx: Optional[Union[float, FXRates, FXForwards]] = None,
+        base: Optional[str] = None,
+        settlement: datetime = None,
+    ):
+        """
+        Return the properties of the security used in calculating cashflows.
+
+        Parameters
+        ----------
+        curves : Curve, str or list of such
+            A single :class:`Curve` or id or a list of such. A list defines the
+            following curves in the order:
+
+              - Forecasting :class:`Curve` for ``leg1``.
+              - Discounting :class:`Curve` for ``leg1``.
+        solver : Solver, optional
+            The numerical :class:`Solver` that constructs ``Curves`` from calibrating
+            instruments.
+        fx : float, FXRates, FXForwards, optional
+            The immediate settlement FX rate that will be used to convert values
+            into another currency. A given `float` is used directly. If giving a
+            ``FXRates`` or ``FXForwards`` object, converts from local currency
+            into ``base``.
+        base : str, optional
+            The base currency to convert cashflows into (3-digit code), set by default.
+            Only used if ``fx_rate`` is an ``FXRates`` or ``FXForwards`` object.
+        settlement : datetime, optional
+            The settlement date of the security. If *None* adds the regular ``settle``
+            time to the initial node date of the given discount ``curves``.
+
+        Returns
+        -------
+        DataFrame
+        """
+        curves, fx = _get_curves_and_fx_maybe_from_solver(
+            self.curves, solver, curves, fx
+        )
+        self._set_base_index_if_none(curves[0])
+
+        if settlement is None:
+            settlement = add_tenor(
+                curves[1].node_dates[0],
+                f"{self.settle}B",
+                None,
+                self.leg1.schedule.calendar,
+            )
+        cashflows = self.leg1.cashflows(curves[0], curves[1], fx, base)
+        if self.ex_div(settlement):
+            # deduct the next coupon which has otherwise been included in valuation
+            current_period = index_left(
+                self.leg1.schedule.aschedule,
+                self.leg1.schedule.n_periods + 1,
+                settlement,
+            )
+            cashflows.loc[current_period, defaults.headers["npv"]] = 0
+            cashflows.loc[current_period, defaults.headers["npv_fx"]] = 0
+        return cashflows
+
+
+class FixedRateBond(Sensitivities, BondMixin, BaseMixin):
+    # TODO ensure calculations work for amortizing bonds.
+    """
+    Create a fixed rate bond security.
+
+    Parameters
+    ----------
+    effective : datetime
+        The adjusted or unadjusted effective date.
+    termination : datetime or str
+        The adjusted or unadjusted termination date. If a string, then a tenor must be
+        given expressed in days (`"D"`), months (`"M"`) or years (`"Y"`), e.g. `"48M"`.
+    frequency : str in {"M", "B", "Q", "T", "S", "A"}, optional
+        The frequency of the schedule. "Z" is not permitted.
+    stub : str combining {"SHORT", "LONG"} with {"FRONT", "BACK"}, optional
+        The stub type to enact on the swap. Can provide two types, for
+        example "SHORTFRONTLONGBACK".
+    front_stub : datetime, optional
+        An adjusted or unadjusted date for the first stub period.
+    back_stub : datetime, optional
+        An adjusted or unadjusted date for the back stub period.
+        See notes for combining ``stub``, ``front_stub`` and ``back_stub``
+        and any automatic stub inference.
+    roll : int in [1, 31] or str in {"eom", "imm", "som"}, optional
+        The roll day of the schedule. Inferred if not given.
+    eom : bool, optional
+        Use an end of month preference rather than regular rolls for inference. Set by
+        default. Not required if ``roll`` is specified.
+    modifier : str, optional
+        The modification rule, in {"F", "MF", "P", "MP"}
+    calendar : calendar or str, optional
+        The holiday calendar object to use. If str, looks up named calendar from
+        static data.
+    payment_lag : int, optional
+        The number of business days to lag payments by.
+    notional : float, optional
+        The leg notional, which is applied to each period.
+    currency : str, optional
+        The currency of the leg (3-digit code).
+    amortization: float, optional
+        The amount by which to adjust the notional each successive period. Should have
+        sign equal to that of notional if the notional is to reduce towards zero.
+    convention: str, optional
+        The day count convention applied to calculations of period accrual dates.
+        See :meth:`~rateslib.calendars.dcf`.
+    fixed_rate : float, optional
+        The **coupon** rate applied to determine cashflows. Can be set
+        to `None` and designated
+        later, perhaps after a mid-market rate for all periods has been calculated.
+    ex_div : int
+        The number of days prior to a cashflow during which the bond is considered
+        ex-dividend.
+    settle : int
+        The number of business days for regular settlement time, i.e, 1 is T+1.
+    curves : CurveType, str or list of such, optional
+        A single *Curve* or string id or a list of such.
+
+        A list defines the following curves in the order:
+
+        - Forecasting *Curve* for ``leg1``.
+        - Discounting :class:`~rateslib.curves.Curve` for ``leg1``.
+
+    Attributes
+    ----------
+    ex_div_days : int
+    settle : int
+    curves : str, list, CurveType
+    leg1 : FixedLegExchange
+
+    Examples
+    --------
+    This example is taken from the UK debt management office (DMO) website. A copy of
+    which is available :download:`here<_static/ukdmoyldconv.pdf>`.
+
+    We demonstrate the use of **analogue methods** which do not need *Curves* or
+    *Solvers*,
+    :meth:`~rateslib.instruments.FixedRateBond.price`,
+    :meth:`~rateslib.instruments.FixedRateBond.ytm`,
+    :meth:`~rateslib.instruments.FixedRateBond.ex_div`,
+    :meth:`~rateslib.instruments.FixedRateBond.accrued`,
+    :meth:`~rateslib.instruments.FixedRateBond.repo_from_fwd`
+    :meth:`~rateslib.instruments.FixedRateBond.fwd_from_repo`
+    :meth:`~rateslib.instruments.FixedRateBond.duration`,
+    :meth:`~rateslib.instruments.FixedRateBond.convexity`.
+
+    .. ipython:: python
+
+       gilt = FixedRateBond(
+           effective=dt(1998, 12, 7),
+           termination=dt(2015, 12, 7),
+           frequency="S",
+           calendar="ldn",
+           currency="gbp",
+           convention="ActActICMA",
+           ex_div=7,
+           settle=1,
+           fixed_rate=8.0,
+           notional=-1e6,  # negative notional receives fixed, i.e. buys a bond
+           curves="gilt_curve",
+       )
+       gilt.ex_div(dt(1999, 5, 27))
+       gilt.price(ytm=4.445, settlement=dt(1999, 5, 27), dirty=True)
+       gilt.ytm(price=141.070132, settlement=dt(1999, 5, 27), dirty=True)
+       gilt.accrued(dt(1999, 5, 27))
+       gilt.fwd_from_repo(
+           price=141.070132,
+           settlement=dt(1999, 5, 27),
+           forward_settlement=dt(2000, 2, 27),
+           repo_rate=4.5,
+           convention="Act365F",
+           dirty=True,
+       )
+       gilt.repo_from_fwd(
+           price=141.070132,
+           settlement=dt(1999, 5, 27),
+           forward_settlement=dt(2000, 2, 27),
+           forward_price=141.829943,
+           convention="Act365F",
+           dirty=True,
+       )
+       gilt.duration(settlement=dt(1999, 5, 27), ytm=4.445, metric="risk")
+       gilt.duration(settlement=dt(1999, 5, 27), ytm=4.445, metric="modified")
+       gilt.convexity(settlement=dt(1999, 5, 27), ytm=4.445)
+
+
+    The following **digital methods** consistent with the library's ecosystem are
+    also available,
+    :meth:`~rateslib.instruments.FixedRateBond.analytic_delta`,
+    :meth:`~rateslib.instruments.FixedRateBond.rate`,
+    :meth:`~rateslib.instruments.FixedRateBond.npv`,
+    :meth:`~rateslib.instruments.FixedRateBond.cashflows`,
+    :meth:`~rateslib.instruments.FixedRateBond.delta`,
+    :meth:`~rateslib.instruments.FixedRateBond.gamma`.
+
+    .. ipython:: python
+
+       gilt_curve = Curve({dt(1999, 5, 26): 1.0, dt(2019, 5, 26): 1.0}, id="gilt_curve")
+       instruments = [
+           (gilt, (), {"metric": "ytm"}),
+       ]
+       solver = Solver(
+           curves=[gilt_curve],
+           instruments=instruments,
+           s=[4.445],
+           instrument_labels=["8% Dec15"],
+           id="gilt_solver",
+       )
+       gilt.npv(solver=solver)
+       gilt.analytic_delta(disc_curve=gilt_curve)
+       gilt.rate(solver=solver, metric="clean_price")
+
+    The sensitivities are also available. In this case the *Solver* is calibrated
+    with *instruments* priced in yield terms so sensitivities are measured in basis
+    points (bps).
+
+    .. ipython:: python
+
+       gilt.delta(solver=solver)
+       gilt.gamma(solver=solver)
+
+    The DataFrame of cashflows.
+
+    .. ipython:: python
+
+       gilt.cashflows(solver=solver)
+
+    """
+    _fixed_rate_mixin = True
+    _ytm_attribute = "cashflow"  # nominal bonds use cashflows in YTM calculation
+
+    def __init__(
+        self,
+        effective: datetime,
+        termination: Union[datetime, str] = None,
+        frequency: str = None,
+        stub: Optional[str] = None,
+        front_stub: Optional[datetime] = None,
+        back_stub: Optional[datetime] = None,
+        roll: Optional[Union[str, int]] = None,
+        eom: Optional[bool] = None,
+        modifier: Optional[str] = False,
+        calendar: Optional[Union[CustomBusinessDay, str]] = None,
+        payment_lag: Optional[int] = None,
+        notional: Optional[float] = None,
+        currency: Optional[str] = None,
+        amortization: Optional[float] = None,
+        convention: Optional[str] = None,
+        fixed_rate: Optional[float] = None,
+        ex_div: int = 0,
+        settle: int = 1,
+        curves: Optional[Union[list, str, Curve]] = None,
+    ):
+        self.curves = curves
+        if frequency.lower() == "z":
+            raise ValueError("FixedRateBond `frequency` must be in {M, B, Q, T, S, A}.")
+        if payment_lag is None:
+            payment_lag = defaults.payment_lag_specific[type(self).__name__]
+        self._fixed_rate = fixed_rate
+        self.ex_div_days = ex_div
+        self.settle = settle
+        self.leg1 = FixedLegExchange(
+            effective=effective,
+            termination=termination,
+            frequency=frequency,
+            stub=stub,
+            front_stub=front_stub,
+            back_stub=back_stub,
+            roll=roll,
+            eom=eom,
+            modifier=modifier,
+            calendar=calendar,
+            payment_lag=payment_lag,
+            payment_lag_exchange=payment_lag,
+            notional=notional,
+            currency=currency,
+            amortization=amortization,
+            convention=convention,
+            fixed_rate=fixed_rate,
+            initial_exchange=False,
+        )
+        if self.leg1.amortization != 0:
+            # Note if amortization is added to FixedRateBonds must systematically
+            # go through and update all methods. Many rely on the quantity
+            # self.notional which is currently assumed to be a fixed quantity
+            raise NotImplementedError("`amortization` for FixedRateBond must be zero.")
+
+    # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
+    # Commercial use of this code, and/or copying and redistribution is prohibited.
+    # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
+
     # Digital Methods
 
     def rate(
         self,
         curves: Optional[Union[Curve, str, list]] = None,
         solver: Optional[Solver] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
@@ -1491,18 +1652,228 @@
     #     kwargs : dict
     #         Keyword arguments to :meth:`~rateslib.periods.BasePeriod.npv`.
     #
     #     Returns
     #     -------
     #     float, Dual, Dual2
     #     """
-    #     TODO: calculte this formula.
+    #     TODO: calculate this par_spread formula.
     #     return (self.notional - self.npv(*args, **kwargs)) / self.analytic_delta(*args, **kwargs)
 
 
+class IndexFixedRateBond(Sensitivities, BondMixin, BaseMixin):
+    _fixed_rate_mixin = True
+    _ytm_attribute = "real_cashflow"  # index linked bonds use real cashflows
+    _index_base_mixin = True
+
+    def __init__(
+        self,
+        effective: datetime,
+        termination: Union[datetime, str] = None,
+        frequency: str = None,
+        stub: Optional[str] = None,
+        front_stub: Optional[datetime] = None,
+        back_stub: Optional[datetime] = None,
+        roll: Optional[Union[str, int]] = None,
+        eom: Optional[bool] = None,
+        modifier: Optional[str] = False,
+        calendar: Optional[Union[CustomBusinessDay, str]] = None,
+        payment_lag: Optional[int] = None,
+        notional: Optional[float] = None,
+        currency: Optional[str] = None,
+        amortization: Optional[float] = None,
+        convention: Optional[str] = None,
+        fixed_rate: Optional[float] = None,
+        index_base: Optional[Union[float, Series]] = None,
+        index_fixings: Optional[Union[float, Series]] = None,
+        index_method: Optional[str] = None,
+        index_lag: Optional[int] = None,
+        ex_div: int = 0,
+        settle: int = 1,
+        curves: Optional[Union[list, str, Curve]] = None,
+    ):
+        self.curves = curves
+        if frequency.lower() == "z":
+            raise ValueError(
+                "IndexFixedRateBond `frequency` must be in {M, B, Q, T, S, A}."
+            )
+        if payment_lag is None:
+            payment_lag = defaults.payment_lag_specific[type(self).__name__]
+        self._fixed_rate = fixed_rate
+        self._index_base = index_base
+        self.ex_div_days = ex_div
+        self.settle = settle
+        self.leg1 = IndexFixedLegExchange(
+            effective=effective,
+            termination=termination,
+            frequency=frequency,
+            stub=stub,
+            front_stub=front_stub,
+            back_stub=back_stub,
+            roll=roll,
+            eom=eom,
+            modifier=modifier,
+            calendar=calendar,
+            payment_lag=payment_lag,
+            payment_lag_exchange=payment_lag,
+            notional=notional,
+            currency=currency,
+            amortization=amortization,
+            convention=convention,
+            fixed_rate=fixed_rate,
+            initial_exchange=False,
+            index_base=index_base,
+            index_method=index_method,
+            index_lag=index_lag,
+            index_fixings=index_fixings,
+        )
+        if self.leg1.amortization != 0:
+            # Note if amortization is added to FixedRateBonds must systematically
+            # go through and update all methods. Many rely on the quantity
+            # self.notional which is currently assumed to be a fixed quantity
+            raise NotImplementedError("`amortization` for FixedRateBond must be zero.")
+
+    def index_ratio(self, settlement: datetime, curve: Optional[IndexCurve]):
+        if self.leg1.index_fixings is not None \
+                and not isinstance(self.leg1.index_fixings, Series):
+            raise ValueError(
+                "Must provide `index_fixings` as a Series for inter-period settlement."
+            )
+        # TODO: this indexing of periods assumes no amortization
+        index_val = IndexMixin._index_value(
+            i_fixings=self.leg1.index_fixings,
+            i_curve=curve,
+            i_lag=self.leg1.index_lag,
+            i_method=self.leg1.index_method,
+            i_date=settlement,
+        )
+        index_base = IndexMixin._index_value(
+            i_fixings=self.index_base,
+            i_date=self.leg1.schedule.effective,
+            i_lag=self.leg1.index_lag,
+            i_method=self.leg1.index_method,
+            i_curve=curve
+        )
+        return index_val / index_base
+
+    def rate(
+        self,
+        curves: Optional[Union[Curve, str, list]] = None,
+        solver: Optional[Solver] = None,
+        fx: Optional[Union[float, FXRates, FXForwards]] = None,
+        base: Optional[str] = None,
+        metric: str = "clean_price",
+        forward_settlement: Optional[datetime] = None,
+    ):
+        """
+        Return various pricing metrics of the security calculated from
+        :class:`~rateslib.curves.Curve` s.
+
+        Parameters
+        ----------
+        curves : Curve, str or list of such
+            A single :class:`Curve` or id or a list of such. A list defines the
+            following curves in the order:
+
+              - Forecasting :class:`Curve` for ``leg1``.
+              - Discounting :class:`Curve` for ``leg1``.
+        solver : Solver, optional
+            The numerical :class:`Solver` that constructs ``Curves`` from calibrating
+            instruments.
+        fx : float, FXRates, FXForwards, optional
+            The immediate settlement FX rate that will be used to convert values
+            into another currency. A given `float` is used directly. If giving a
+            ``FXRates`` or ``FXForwards`` object, converts from local currency
+            into ``base``.
+        base : str, optional
+            The base currency to convert cashflows into (3-digit code), set by default.
+            Only used if ``fx`` is an ``FXRates`` or ``FXForwards`` object.
+        metric : str, optional
+            Metric returned by the method. Available options are {"clean_price",
+            "dirty_price", "ytm", "fwd_clean_price", "fwd_dirty_price"}
+        forward_settlement : datetime
+            The forward settlement date, required if the metric is in
+            {"fwd_clean_price", "fwd_dirty_price"}.
+
+        Returns
+        -------
+        float, Dual, Dual2
+        """
+
+        curves, fx = _get_curves_and_fx_maybe_from_solver(
+            self.curves, solver, curves, fx
+        )
+
+        metric = metric.lower()
+        if metric in [
+            "clean_price",
+            "dirty_price",
+            "index_clean_price",
+            "ytm",
+            "index_dirty_price",
+        ]:
+            settlement = add_tenor(
+                curves[1].node_dates[0],
+                f"{self.settle}B",
+                None,
+                self.leg1.schedule.calendar,
+            )
+            npv = self._npv_local(
+                curves[0], curves[1], fx, base, settlement, settlement
+            )
+            # scale price to par 100 (npv is already projected forward to settlement)
+            index_dirty_price = npv * 100 / -self.leg1.notional
+            index_ratio = self.index_ratio(settlement, curves[0])
+            dirty_price = index_dirty_price / index_ratio
+
+            if metric == "dirty_price":
+                return dirty_price
+            elif metric == "clean_price":
+                return dirty_price - self.accrued(settlement)
+            elif metric == "ytm":
+                return self.ytm(dirty_price, settlement, True)
+            elif metric == "index_dirty_price":
+                return index_dirty_price
+            elif metric == "index_clean_price":
+                return index_dirty_price - self.accrued(settlement) * index_ratio
+
+        elif metric in [
+            "fwd_clean_price",
+            "fwd_dirty_price",
+            "fwd_index_clean_price",
+            "fwd_index_dirty_price",
+        ]:
+            if forward_settlement is None:
+                raise ValueError(
+                    "`forward_settlement` needed to determine forward price."
+                )
+            npv = self._npv_local(
+                curves[0], curves[1], fx, base, forward_settlement, forward_settlement
+            )
+            index_dirty_price = npv / -self.leg1.notional * 100
+            index_ratio = self.index_ratio(forward_settlement, curves[0])
+            dirty_price = index_dirty_price / index_ratio
+            if metric == "fwd_dirty_price":
+                return dirty_price
+            elif metric == "fwd_clean_price":
+                return dirty_price - self.accrued(forward_settlement)
+            elif metric == "fwd_index_dirty_price":
+                return index_dirty_price
+            elif metric == "fwd_index_clean_price":
+                return (
+                    index_dirty_price - self.accrued(forward_settlement) * index_ratio
+                )
+
+        raise ValueError(
+            "`metric` must be in {'dirty_price', 'clean_price', 'ytm', "
+            "'fwd_clean_price', 'fwd_dirty_price', 'index_dirty_price', "
+            "'index_clean_price', 'fwd_index_dirty_price', 'fwd_index_clean_price'}."
+        )
+
+
 class Bill(FixedRateBond):
     """
     Create a discount security.
 
     Parameters
     ----------
     effective : datetime
@@ -1525,31 +1896,127 @@
         The currency of the leg (3-digit code).
     convention: str, optional
         The day count convention applied to calculations of period accrual dates.
         See :meth:`~rateslib.calendars.dcf`.
     settle : int
         The number of business days for regular settlement time, i.e, 1 is T+1.
 
-    Attributes
-    ----------
-    leg1 : FixedLegExchange
+    Examples
+    --------
+    This example is taken from the US Treasury Federal website. A copy of
+    which is available :download:`here<_static/ofcalc6decTbill.pdf>`.
+
+    We demonstrate the use of **analogue methods** which do not need *Curves* or
+    *Solvers*,
+    :meth:`~rateslib.instruments.Bill.price`,
+    :meth:`~rateslib.instruments.Bill.simple_rate`,
+    :meth:`~rateslib.instruments.Bill.discount_rate`,
+    :meth:`~rateslib.instruments.FixedRateBond.ytm`,
+    :meth:`~rateslib.instruments.FixedRateBond.ex_div`,
+    :meth:`~rateslib.instruments.FixedRateBond.accrued`,
+    :meth:`~rateslib.instruments.FixedRateBond.repo_from_fwd`
+    :meth:`~rateslib.instruments.FixedRateBond.fwd_from_repo`
+    :meth:`~rateslib.instruments.FixedRateBond.duration`,
+    :meth:`~rateslib.instruments.FixedRateBond.convexity`.
+
+    .. ipython:: python
+
+       bill = Bill(
+           effective=dt(2004, 1, 22),
+           termination=dt(2004, 2, 19),
+           frequency="M",
+           calendar="nyc",
+           modifier="MF",
+           currency="usd",
+           convention="Act360",
+           settle=1,
+           notional=-1e6,  # negative notional receives fixed, i.e. buys a bill
+           curves="bill_curve",
+       )
+       bill.ex_div(dt(2004, 1, 22))
+       bill.price(discount_rate=0.80, settlement=dt(2004, 1, 22))
+       bill.simple_rate(price=99.937778, settlement=dt(2004, 1, 22))
+       bill.discount_rate(price=99.937778, settlement=dt(2004, 1, 22))
+       bill.ytm(price=99.937778, settlement=dt(2004, 1, 22))
+       bill.accrued(dt(2004, 1, 22))
+       bill.fwd_from_repo(
+           price=99.937778,
+           settlement=dt(2004, 1, 22),
+           forward_settlement=dt(2004, 2, 19),
+           repo_rate=0.8005,
+           convention="Act360",
+       )
+       bill.repo_from_fwd(
+           price=99.937778,
+           settlement=dt(2004, 1, 22),
+           forward_settlement=dt(2004, 2, 19),
+           forward_price=100.00,
+           convention="Act360",
+       )
+       bill.duration(settlement=dt(2004, 1, 22), ytm=0.8005, metric="risk")
+       bill.duration(settlement=dt(2004, 1, 22), ytm=0.8005, metric="modified")
+       bill.convexity(settlement=dt(2004, 1, 22), ytm=0.8005)
+
+
+    The following **digital methods** consistent with the library's ecosystem are
+    also available,
+    :meth:`~rateslib.instruments.Bill.rate`,
+    :meth:`~rateslib.instruments.FixedRateBond.npv`,
+    :meth:`~rateslib.instruments.FixedRateBond.analytic_delta`,
+    :meth:`~rateslib.instruments.FixedRateBond.cashflows`,
+    :meth:`~rateslib.instruments.FixedRateBond.delta`,
+    :meth:`~rateslib.instruments.FixedRateBond.gamma`,
+
+    .. ipython:: python
+
+       bill_curve = Curve({dt(2004, 1, 21): 1.0, dt(2004, 3, 21): 1.0}, id="bill_curve")
+       instruments = [
+           (bill, (), {"metric": "ytm"}),
+       ]
+       solver = Solver(
+           curves=[bill_curve],
+           instruments=instruments,
+           s=[0.8005],
+           instrument_labels=["Feb04 Tbill"],
+           id="bill_solver",
+       )
+       bill.npv(solver=solver)
+       bill.analytic_delta(disc_curve=bill_curve)
+       bill.rate(solver=solver, metric="price")
+
+    The sensitivities are also available. In this case the *Solver* is calibrated
+    with *instruments* priced in yield terms so sensitivities are measured in basis
+    points (bps).
+
+    .. ipython:: python
+
+       bill.delta(solver=solver)
+       bill.gamma(solver=solver)
+
+    The DataFrame of cashflows.
+
+    .. ipython:: python
+
+       bill.cashflows(solver=solver)
+
     """
 
     def __init__(
         self,
         effective: datetime,
         termination: Union[datetime, str] = None,
         frequency: str = None,
         modifier: Optional[str] = False,
         calendar: Optional[Union[CustomBusinessDay, str]] = None,
         payment_lag: Optional[int] = None,
         notional: Optional[float] = None,
         currency: Optional[str] = None,
         convention: Optional[str] = None,
         settle: int = 1,
+        curves: Optional[Union[list, str, Curve]] = None,
     ):
         if payment_lag is None:
             payment_lag = defaults.payment_lag_specific[type(self).__name__]
         super().__init__(
             effective=effective,
             termination=termination,
             frequency=frequency,
@@ -1564,19 +2031,20 @@
             notional=notional,
             currency=currency,
             amortization=None,
             convention=convention,
             fixed_rate=0,
             ex_div=0,
             settle=settle,
+            curves=curves,
         )
 
     def rate(
         self,
-        curves: Union[Curve, str, list],
+        curves: Optional[Union[Curve, str, list]] = None,
         solver: Optional[Solver] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
         metric="price",
     ):
         """
         Return various pricing metrics of the security calculated from
@@ -1619,45 +2087,79 @@
         )
         # scale price to par 100 and make a fwd adjustment according to curve
         price = (
             self.npv(curves, solver, fx, base)
             * 100
             / (-self.leg1.notional * curves[1][settlement])
         )
-        if metric == "price":
+        if metric in ["price", "clean_price"]:
             return price
         elif metric == "discount_rate":
             return self.discount_rate(price, settlement)
         elif metric == "simple_rate":
             return self.simple_rate(price, settlement)
         elif metric == "ytm":
             return self.ytm(price, settlement, False)
         raise ValueError(
             "`metric` must be in {'price', 'discount_rate', 'ytm', 'simple_rate'}"
         )
 
-    def simple_rate(self, price, settlement):
+    def simple_rate(self, price: DualTypes, settlement: datetime) -> DualTypes:
+        """
+        Return the simple rate of the security from its ``price``.
+
+        Parameters
+        ----------
+        price : float, Dual, or Dual2
+            The price of the security.
+        settlement : datetime
+            The settlement date of the security.
+
+        Returns
+        -------
+        float, Dual, or Dual2
+        """
         dcf = (1 - self._accrued_frac(settlement)[0]) * self.leg1.periods[0].dcf
         return ((100 / price - 1) / dcf) * 100
 
-    def discount_rate(self, price, settlement):
+    def discount_rate(self, price: DualTypes, settlement: datetime) -> DualTypes:
+        """
+        Return the discount rate of the security from its ``price``.
+
+        Parameters
+        ----------
+        price : float, Dual, or Dual2
+            The price of the security.
+        settlement : datetime
+            The settlement date of the security.
+
+        Returns
+        -------
+        float, Dual, or Dual2
+        """
         dcf = (1 - self._accrued_frac(settlement)[0]) * self.leg1.periods[0].dcf
         rate = ((1 - price / 100) / dcf) * 100
         return rate
 
-    def price(self, discount_rate, settlement):
+    def price(
+        self, discount_rate: DualTypes, settlement: datetime, dirty: bool = False
+    ) -> DualTypes:
         """
         Return the price of the bill given the ``discount_rate``.
 
         Parameters
         ----------
         discount_rate : float
             The rate used by the pricing formula.
         settlement : datetime
             The settlement date.
+        dirty : bool, not required
+            Discount securities have no coupon, the concept of clean or dirty is not
+            relevant. Argument is included for signature consistency with
+            :meth:`FixedRateBond.price<rateslib.instruments.FixedRateBond.price>`.
 
         Returns
         -------
         float, Dual, Dual2
         """
         dcf = (1 - self._accrued_frac(settlement)[0]) * self.leg1.periods[0].dcf
         return 100 - discount_rate * dcf
@@ -2068,74 +2570,17 @@
             dirty_price = npv * 100 / -self.leg1.notional
 
             if metric == "dirty_price":
                 return dirty_price
             elif metric == "clean_price":
                 return dirty_price - self.accrued(settlement)
             elif metric == "spread":
-                if (
-                    "rfr" in self.leg1.fixing_method
-                    and self.leg1.spread_compound_method != "none_simple"
-                ):
-                    # This code replicates BaseLeg._spread for an FRN accounting for ex-div
-                    # via FRN.npv().
-
-                    _fs = self.float_spread
-                    self.float_spread = Dual2(
-                        0.0 if _fs is None else float(_fs), "spread_z"
-                    )
-
-                    fore_curve, disc_curve = curves[0], curves[1]
-
-                    fore_ad = fore_curve.ad
-                    fore_curve._set_ad_order(2)
-
-                    disc_ad = disc_curve.ad
-                    disc_curve._set_ad_order(2)
-
-                    if isinstance(fx, (FXRates, FXForwards)):
-                        _fx = None if fx is None else fx._ad
-                        fx._set_ad_order(2)
-
-                    npv = self.npv([fore_curve, disc_curve], None, fx, base, False)
-                    b = npv.gradient("spread_z", order=1)[0]
-                    a = 0.5 * npv.gradient("spread_z", order=2)[0][0]
-                    c = npv + self.leg1.notional
-
-                    _1 = -c / b
-                    if abs(a) > 1e-14:
-                        _2a = (-b - (b**2 - 4 * a * c) ** 0.5) / (2 * a)
-                        _2b = (-b + (b**2 - 4 * a * c) ** 0.5) / (2 * a)  # alt soln
-                        if abs(_1 - _2a) < abs(_1 - _2b):
-                            _ = _2a
-                        else:
-                            _ = _2b  # select quadratic soln
-                    else:  # pragma: no cover
-                        # this is to avoid div by zero err and return an approximation
-                        _ = _1
-                        warnings.warn(
-                            "Divide by zero encountered and the spread is approximated "
-                            "to first order.",
-                            UserWarning,
-                        )
-                    _ += 0.0 if _fs is None else _fs
-
-                    self.float_spread = _fs
-                    fore_curve._set_ad_order(fore_ad)
-                    disc_curve._set_ad_order(disc_ad)
-                    if isinstance(fx, (FXRates, FXForwards)):
-                        fx._set_ad_order(_fx)
-                    return set_order(_, disc_ad)  # use disc_ad: cred spd from disc crv
-                else:
-                    # NPV calc is efficient and requires no additional ingenuity.
-                    _ = (npv + self.leg1.notional) / self.analytic_delta(
-                        curves[0], curves[1], fx, base
-                    )
-                    _ += self.float_spread
-                    return _
+                _ = self.leg1._spread(-(npv + self.leg1.notional), curves[0], curves[1])
+                z = 0.0 if self.float_spread is None else self.float_spread
+                return _ + z
 
         elif metric in ["fwd_clean_price", "fwd_dirty_price"]:
             if forward_settlement is None:
                 raise ValueError(
                     "`forward_settlement` needed to determine forward price."
                 )
             npv = self._npv_local(
@@ -2163,21 +2608,153 @@
     ----------
     coupon: float
         The nominal coupon rate set on the contract specifications.
     delivery: datetime or 2-tuple of datetimes
         The delivery window first and last delivery day, or a single delivery day.
     basket: tuple of FixedRateBond
         The bonds that are available as deliverables.
-    last_trading: int, optional
-        The number of business days before the final delivery day when trading
-        will cease.
     nominal: float, optional
         The nominal amount of the contract.
+    contracts: int, optional
+        The number of contracts owned or short.
     calendar: str, optional
         The calendar to define delivery days within the delivery window.
+    currency: str, optional
+        The currency (3-digit code) of the settlement contract.
+
+    Examples
+    --------
+    The :meth:`~rateslib.instruments.BondFuture.dlv` method is a summary method which
+    displays many attributes simultaneously in a DataFrame.
+    This example replicates the Bloomberg screen print in the publication
+    *The Futures Bond Basis: Second Edition (p77)* by Moorad Choudhry. To replicate
+    that publication exactly no calendar has been provided. A more modern
+    Bloomberg would probably consider the London business day calendar and
+    this would affect the metrics of the third bond to a small degree (i.e.
+    set `calendar="ldn"`)
+
+    .. ipython:: python
+
+       kws = dict(
+           frequency="S",
+           ex_div=7,
+           convention="ActActICMA",
+           calendar=None,
+           currency="gbp",
+           settle=1,
+           curves="gilt_curve"
+       )
+       bonds = [
+           FixedRateBond(dt(1999, 1, 1), dt(2009, 12, 7), fixed_rate=5.75, **kws),
+           FixedRateBond(dt(1999, 1, 1), dt(2011, 7, 12), fixed_rate=9.00, **kws),
+           FixedRateBond(dt(1999, 1, 1), dt(2010, 11, 25), fixed_rate=6.25, **kws),
+           FixedRateBond(dt(1999, 1, 1), dt(2012, 8, 6), fixed_rate=9.00, **kws),
+       ]
+       prices=[102.732, 131.461, 107.877, 134.455]
+       ytms=[bond.ytm(price, dt(2000, 3, 16)) for bond, price in zip(bonds, prices)]
+       future = BondFuture(
+           delivery=(dt(2000, 6, 1), dt(2000, 6, 30)),
+           coupon=7.0,
+           basket=bonds,
+           nominal=100000,
+           contracts=10,
+           currency="gbp",
+       )
+       future.dlv(
+           future_price=112.98,
+           prices=[102.732, 131.461, 107.877, 134.455],
+           repo_rate=6.24,
+           settlement=dt(2000, 3, 16),
+           convention="Act365f",
+       )
+
+    Various other metrics can be extracted in isolation including,
+    ``notional``, and conversion factors (``cfs``),
+    :meth:`~rateslib.instruments.BondFuture.gross_basis`,
+    :meth:`~rateslib.instruments.BondFuture.net_basis`,
+    :meth:`~rateslib.instruments.BondFuture.implied_repo`,
+    :meth:`~rateslib.instruments.BondFuture.ytm`,
+    :meth:`~rateslib.instruments.BondFuture.duration`,
+    :meth:`~rateslib.instruments.BondFuture.convexity`,
+    :meth:`~rateslib.instruments.BondFuture.ctd_index`,
+
+    .. ipython:: python
+
+        future.cfs
+        future.notional
+        future.gross_basis(
+            future_price=112.98,
+            prices=prices,
+        )
+        future.net_basis(
+            future_price=112.98,
+            prices=prices,
+            repo_rate=6.24,
+            settlement=dt(2000, 3, 16),
+            delivery=dt(2000, 6, 30),
+            convention="Act365f"
+        )
+        future.implied_repo(
+            future_price=112.98,
+            prices=prices,
+            settlement=dt(2000, 3, 16)
+        )
+        future.ytm(future_price=112.98)
+        future.duration(future_price=112.98)
+        future.convexity(future_price=112.98)
+        future.ctd_index(
+            future_price=112.98,
+            prices=prices,
+            settlement=dt(2000, 3, 16)
+        )
+
+    As opposed to the **analogue methods** above, we can also use
+    the **digital methods**,
+    :meth:`~rateslib.instruments.BondFuture.npv`,
+    :meth:`~rateslib.instruments.BondFuture.rate`,
+    but we need to create *Curves* and a *Solver* in the usual way.
+
+    .. ipython:: python
+
+       gilt_curve = Curve(
+           nodes={
+               dt(2000, 3, 15): 1.0,
+               dt(2009, 12, 7): 1.0,
+               dt(2010, 11, 25): 1.0,
+               dt(2011, 7, 12): 1.0,
+               dt(2012, 8, 6): 1.0,
+           },
+           id="gilt_curve",
+       )
+       solver = Solver(
+           curves=[gilt_curve],
+           instruments=[(b, (), {"metric": "ytm"}) for b in bonds],
+           s=ytms,
+           id="gilt_solver",
+           instrument_labels=["5.75% '09", "9% '11", "6.25% '10", "9% '12"],
+       )
+
+    Sensitivities are also available;
+    :meth:`~rateslib.instruments.BondFuture.delta`
+    :meth:`~rateslib.instruments.BondFuture.gamma`.
+
+    .. ipython:: python
+
+       future.delta(solver=solver)
+
+    The delta of a *BondFuture* is individually assigned to the CTD. If the CTD changes
+    the delta is reassigned.
+
+    .. ipython:: python
+
+       solver.s = [5.3842, 5.2732, 5.2755, 5.52]
+       solver.iterate()
+       future.delta(solver=solver)
+       future.gamma(solver=solver)
+
     """
 
     def __init__(
         self,
         coupon: float,
         delivery: Union[datetime, tuple[datetime, datetime]],
         basket: tuple[FixedRateBond],
@@ -2307,43 +2884,14 @@
             The day count convention applied to the repo rates.
         dirty: bool
             Whether the bond prices are given including accrued interest.
 
         Returns
         -------
         DataFrame
-
-        Examples
-        --------
-        This example replicates the Bloomberg screen print in the publication
-        *The Futures Bond Basis: Second Edition (p77)* by Moorad Choudhry. To replicate
-        that publication exactly no calendar has been provided. A more modern
-        Bloomberg would probably consider the London business day calendar and
-        this would affect the metrics of the third bond to a small degree (i.e.
-        set `calendar="ldn"`)
-
-        .. ipython:: python
-
-           kws = dict(ex_div=7, frequency="S", convention="ActActICMA", calendar=None)
-           bonds = [
-               FixedRateBond(dt(1999, 1, 1), dt(2009, 12, 7), fixed_rate=5.75, **kws),
-               FixedRateBond(dt(1999, 1, 1), dt(2011, 7, 12), fixed_rate=9.00, **kws),
-               FixedRateBond(dt(1999, 1, 1), dt(2010, 11, 25), fixed_rate=6.25, **kws),
-               FixedRateBond(dt(1999, 1, 1), dt(2012, 8, 6), fixed_rate=9.00, **kws),
-           ]
-           future = BondFuture(
-               delivery=(dt(2000, 6, 1), dt(2000, 6, 30)), coupon=7.0, basket=bonds
-           )
-           future.dlv(
-               future_price=112.98,
-               prices=[102.732, 131.461, 107.877, 134.455],
-               repo_rate=6.24,
-               settlement=dt(2000, 3, 16),
-               convention="Act365f",
-           )
         """
         if not isinstance(repo_rate, (tuple, list)):
             r_ = (repo_rate,) * len(self.basket)
         else:
             r_ = tuple(repo_rate)
 
         df = DataFrame(
@@ -2386,16 +2934,15 @@
         self,
         future_price: Union[float, Dual, Dual2],
         prices: list[float, Dual, Dual2],
         settlement: datetime = None,
         dirty: bool = False,
     ):
         """
-        Calculate the implied repo of each bond in the basket using the proceeds
-        method.
+        Calculate the gross basis of each bond in the basket.
 
         Parameters
         ----------
         future_price: float, Dual, Dual2
             The price of the future.
         prices: sequence of float, Dual, Dual2
             The prices of the bonds in the deliverable basket (ordered).
@@ -2403,21 +2950,14 @@
             The settlement date of the bonds, required only if ``dirty`` is *True*.
         dirty: bool
             Whether the bond prices are given including accrued interest.
 
         Returns
         -------
         tuple
-
-        Examples
-        --------
-
-        .. ipython:: python
-
-           future.gross_basis(112.98, [102.732, 131.461, 107.877, 134.455])
         """
         if dirty:
             prices_ = tuple(
                 prices[i] - bond.accrued(settlement)
                 for i, bond in enumerate(self.basket)
             )
         else:
@@ -2433,16 +2973,16 @@
         repo_rate: Union[float, Dual, Dual2, list, tuple],
         settlement: datetime,
         delivery: Optional[datetime] = None,
         convention: Optional[str] = None,
         dirty: bool = False,
     ):
         """
-        Calculate the implied repo of each bond in the basket using the proceeds
-        method.
+        Calculate the net basis of each bond in the basket via the proceeds
+        method of repo.
 
         Parameters
         ----------
         future_price: float, Dual, Dual2
             The price of the future.
         prices: sequence of float, Dual, Dual2
             The prices of the bonds in the deliverable basket (ordered).
@@ -2457,28 +2997,14 @@
             The day count convention applied to the repo rates.
         dirty: bool
             Whether the bond prices are given including accrued interest.
 
         Returns
         -------
         tuple
-
-        Examples
-        --------
-
-        .. ipython:: python
-
-           future.net_basis(
-               future_price=112.98,
-               prices=[102.732, 131.461, 107.877, 134.455],
-               repo_rate=6.24,
-               settlement=dt(2000, 3, 16),
-               delivery=dt(2000, 6, 30),
-               convention="Act365f"
-           )
         """
         if delivery is None:
             f_settlement = self.delivery[1]
         else:
             f_settlement = delivery
 
         if not isinstance(repo_rate, (list, tuple)):
@@ -2523,23 +3049,14 @@
             The day count convention used in the rate.
         dirty: bool
             Whether the bond prices are given including accrued interest.
 
         Returns
         -------
         tuple
-
-        Examples
-        --------
-
-        .. ipython:: python
-
-           future.implied_repo(
-               112.98, [102.732, 131.461, 107.877, 134.455], dt(2000, 3, 16)
-           )
         """
         if delivery is None:
             f_settlement = self.delivery[1]
         else:
             f_settlement = delivery
 
         implied_repos = tuple()
@@ -2572,21 +3089,14 @@
         delivery : datetime, optional
             The future delivery day on which to calculate the yield. If not given aligns
             with the last delivery day specified on the future.
 
         Returns
         -------
         tuple
-
-        Examples
-        --------
-
-        .. ipython:: python
-
-           future.ytm(112.98)
         """
         if delivery is None:
             settlement = self.delivery[1]
         else:
             settlement = delivery
         adjusted_prices = [future_price * cf for cf in self.cfs]
         yields = tuple(
@@ -2598,15 +3108,15 @@
     def duration(
         self,
         future_price: float,
         metric: str = "risk",
         delivery: Optional[datetime] = None,
     ):
         """
-        Return the (negated) derivative of ``price`` w.r.t. ``ytm``.
+        Return the (negated) derivative of ``price`` w.r.t. ``ytm`` .
 
         Parameters
         ----------
         future_price : float
             The price of the future.
         metric : str
             The specific duration calculation to return. See notes.
@@ -2653,15 +3163,15 @@
 
     def convexity(
         self,
         future_price: float,
         delivery: Optional[datetime] = None,
     ):
         """
-        Return the second derivative of ``price`` w.r.t. ``ytm``.
+        Return the second derivative of ``price`` w.r.t. ``ytm`` .
 
         Parameters
         ----------
         future_price : float
             The price of the future.
         delivery : datetime, optional
             The delivery date of the contract. If not given uses the last delivery day
@@ -2721,15 +3231,15 @@
             The prices of the bonds to determine the CTD. Not used is ``ctd_index``
             is given.
         settlement : datetime
             The settlement date of the bonds' ``prices``. Only required if ``prices``
             are given.
         delivery : datetime, optional
             The delivery date of the contract.
-        dirty : bool
+        dirty : bool, optional
             Whether the ``prices`` given include accrued interest or not.
 
         Returns
         -------
         int
         """
         implied_repo = self.implied_repo(
@@ -3013,15 +3523,15 @@
         -------
         float, Dual, Dual2
 
         Examples
         --------
         .. ipython:: python
 
-           curve = Curve({dt(2021,1,1): 1.00, dt(2025,1,1): 0.83}, "log_linear", id="SONIA")
+           curve = Curve({dt(2021,1,1): 1.00, dt(2025,1,1): 0.83}, id="SONIA")
            fxr = FXRates({"gbpusd": 1.25}, base="usd")
 
         .. ipython:: python
 
            irs = IRS(
                effective=dt(2022, 1, 1),
                termination="6M",
@@ -3045,15 +3555,15 @@
         base: Optional[str] = None,
     ):
         """
         Return the properties of all legs used in calculating cashflows.
 
         Parameters
         ----------
-        curves : Curve, LineCurve, str or list of such, optional
+        curves : CurveType, str or list of such, optional
             A single :class:`~rateslib.curves.Curve`,
             :class:`~rateslib.curves.LineCurve` or id or a
             list of such. A list defines the following curves in the order:
 
             - Forecasting :class:`~rateslib.curves.Curve` or
               :class:`~rateslib.curves.LineCurve` for ``leg1``.
             - Discounting :class:`~rateslib.curves.Curve` for ``leg1``.
@@ -3254,14 +3764,85 @@
         and derive the rest from the ``curve``.
     leg2_fixing_method : str, optional
         The method by which floating rates are determined, set by default. See notes.
     leg2_method_param : int, optional
         A parameter that is used for the various ``fixing_method`` s. See notes.
     kwargs : dict
         Required keyword arguments to :class:`BaseDerivative`.
+
+    Examples
+    --------
+    Construct a curve to price the example.
+
+    .. ipython:: python
+
+       usd = Curve(
+           nodes={
+               dt(2022, 1, 1): 1.0,
+               dt(2023, 1, 1): 0.965,
+               dt(2024, 1, 1): 0.94
+           },
+           id="usd"
+       )
+
+    Create the IRS, and demonstrate the :meth:`~rateslib.instruments.IRS.rate`,
+    :meth:`~rateslib.instruments.IRS.npv`,
+    :meth:`~rateslib.instruments.IRS.analytic_delta`, and
+    :meth:`~rateslib.instruments.IRS.spread`.
+
+    .. ipython:: python
+
+       irs = IRS(
+           effective=dt(2022, 1, 1),
+           termination="18M",
+           frequency="A",
+           calendar="nyc",
+           currency="usd",
+           fixed_rate=3.269,
+           convention="Act360",
+           notional=100e6,
+           curves=["usd"],
+       )
+       irs.rate(curves=usd)
+       irs.npv(curves=usd)
+       irs.analytic_delta(curve=usd)
+       irs.spread(curves=usd)
+
+    A DataFrame of :meth:`~rateslib.instruments.IRS.cashflows`.
+
+    .. ipython:: python
+
+       irs.cashflows(curves=usd)
+
+    For accurate sensitivity calculations; :meth:`~rateslib.instruments.IRS.delta`
+    and :meth:`~rateslib.instruments.IRS.gamma`, construct a curve model.
+
+    .. ipython:: python
+
+       sofr_kws = dict(
+           effective=dt(2022, 1, 1),
+           frequency="A",
+           convention="Act360",
+           calendar="nyc",
+           currency="usd",
+           curves=["usd"]
+       )
+       instruments = [
+           IRS(termination="1Y", **sofr_kws),
+           IRS(termination="2Y", **sofr_kws),
+       ]
+       solver = Solver(
+           curves=[usd],
+           instruments=instruments,
+           s=[3.65, 3.20],
+           instrument_labels=["1Y", "2Y"],
+           id="sofr",
+       )
+       irs.delta(solver=solver)
+       irs.gamma(solver=solver)
     """
 
     _fixed_rate_mixin = True
     _leg2_float_spread_mixin = True
 
     def __init__(
         self,
@@ -3314,42 +3895,27 @@
             payment_lag=self.leg2_payment_lag,
             notional=self.leg2_notional,
             currency=self.leg2_currency,
             amortization=self.leg2_amortization,
             convention=self.leg2_convention,
         )
 
+    def _set_pricing_mid(
+        self,
+        curves: Optional[Union[Curve, str, list]] = None,
+        solver: Optional[Solver] = None,
+    ):
+        mid_market_rate = self.rate(curves, solver)
+        self.leg1.fixed_rate = float(mid_market_rate)
+
     def analytic_delta(self, *args, **kwargs):
         """
         Return the analytic delta of a leg of the derivative object.
 
         See :meth:`BaseDerivative.analytic_delta`.
-
-        Examples
-        --------
-        .. ipython:: python
-
-           forecasting_curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.98})
-           discounting_curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.985})
-
-        .. ipython:: python
-
-           irs = IRS(
-               effective=dt(2022, 2, 15),
-               termination=dt(2022, 8, 15),
-               frequency="Q",
-               convention="30e360",
-               leg2_convention="Act360",
-               leg2_fixing_method="rfr_payment_delay",
-               payment_lag=2,
-               fixed_rate=2.50,
-               notional=1e9,
-               currency="gbp",
-           )
-           irs.analytic_delta(forecasting_curve, discounting_curve, leg=1)
         """
         return super().analytic_delta(*args, **kwargs)
 
     def npv(
         self,
         curves: Optional[Union[Curve, str, list]] = None,
         solver: Optional[Solver] = None,
@@ -3357,30 +3923,18 @@
         base: Optional[str] = None,
         local: bool = False,
     ):
         """
         Return the NPV of the derivative by summing legs.
 
         See :meth:`BaseDerivative.npv`.
-
-        Examples
-        --------
-        .. ipython:: python
-
-           irs.npv([forecasting_curve, discounting_curve])
-
-        .. ipython:: python
-
-           fxr = FXRates({"gbpusd": 2.0})
-           irs.npv([forecasting_curve, discounting_curve], None, fxr, "usd")
         """
         if self.fixed_rate is None:
             # set a fixed rate for the purpose of pricing NPV, which should be zero.
-            mid_market_rate = self.rate(curves, solver)
-            self.leg1.fixed_rate = mid_market_rate.real
+            self._set_pricing_mid(curves, solver)
         return super().npv(curves, solver, fx, base, local)
 
     def rate(
         self,
         curves: Optional[Union[Curve, str, list]] = None,
         solver: Optional[Solver] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
@@ -3410,20 +3964,14 @@
         -------
         float, Dual or Dual2
 
         Notes
         -----
         The arguments ``fx`` and ``base`` are unused by single currency derivatives
         rates calculations.
-
-        Examples
-        --------
-        .. ipython:: python
-
-           irs.rate([forecasting_curve, discounting_curve])
         """
         curves, _ = _get_curves_and_fx_maybe_from_solver(
             self.curves, solver, curves, fx
         )
         leg2_npv = self.leg2.npv(curves[2], curves[3])
         return self.leg1._spread(-leg2_npv, curves[0], curves[1]) / 100
         # leg1_analytic_delta = self.leg1.analytic_delta(curves[0], curves[1])
@@ -3436,21 +3984,14 @@
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
     ):
         """
         Return the properties of all legs used in calculating cashflows.
 
         See :meth:`BaseDerivative.cashflows`.
-
-        Examples
-        --------
-        .. ipython:: python
-
-           fxr = FXRates({"gbpusd": 2.0})
-           irs.cashflows([forecasting_curve, discounting_curve], None, fxr, "usd")
         """
         return super().cashflows(curves, solver, fx, base)
 
     # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
     # Commercial use of this code, and/or copying and redistribution is prohibited.
     # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
@@ -3494,17 +4035,17 @@
 
         Examples
         --------
         For the most common parameters this method will be exact.
 
         .. ipython:: python
 
-           irs.spread([forecasting_curve, discounting_curve])
-           irs.leg2_float_spread = 48.867036358702
-           irs.npv([forecasting_curve, discounting_curve])
+           irs.spread(curves=usd)
+           irs.leg2_float_spread = -6.948753
+           irs.npv(curves=usd)
 
         When a non-linear spread compound method is used for float RFR legs this is
         an approximation, via second order Taylor expansion.
 
         .. ipython:: python
 
            irs = IRS(
@@ -3515,25 +4056,26 @@
                leg2_convention="Act360",
                leg2_fixing_method="rfr_payment_delay",
                leg2_spread_compound_method="isda_compounding",
                payment_lag=2,
                fixed_rate=2.50,
                leg2_float_spread=0,
                notional=50000000,
-               currency="gbp",
+               currency="usd",
            )
-           irs.spread([forecasting_curve, discounting_curve])
-           irs.leg2_float_spread = 48.59613590683196
-           irs.npv([forecasting_curve, discounting_curve])
-           irs.spread([forecasting_curve, discounting_curve])
+           irs.spread(curves=usd)
+           irs.leg2_float_spread = -111.060143
+           irs.npv(curves=usd)
+           irs.spread(curves=usd)
 
         The ``leg2_float_spread`` is determined through NPV differences. If the difference
         is small since the defined spread is already quite close to the solution the
         approximation is much more accurate. This is shown above where the second call
-        to ``irs.spread`` is different to the previous call.
+        to ``irs.spread`` is different to the previous call, albeit the difference
+        is 1/10000th of a basis point.
         """
         irs_npv = self.npv(curves, solver)
         specified_spd = 0 if self.leg2.float_spread is None else self.leg2.float_spread
         curves, _ = _get_curves_and_fx_maybe_from_solver(
             self.curves, solver, curves, fx
         )
         return self.leg2._spread(-irs_npv, curves[2], curves[3]) + specified_spd
@@ -3543,56 +4085,213 @@
 
 class Swap(IRS):
     """
     Alias for :class:`~rateslib.instruments.IRS`.
     """
 
 
-class ZCS(BaseDerivative):
+class IIRS(BaseDerivative):
+    """
+    Create an indexed interest rate swap (IIRS) composing an
+    :class:`~rateslib.legs.IndexFixedLeg` and a :class:`~rateslib.legs.FloatLeg`.
+
+    If ``notional_exchange``, the legs are :class:`~rateslib.legs.IndexFixedLegExchange`
+    and :class:`~rateslib.legs.FloatLegExchange`.
+
+    Parameters
+    ----------
+    args : dict
+       Required positional args to :class:`BaseDerivative`.
+    fixed_rate : float or None
+       The fixed rate applied to the :class:`~rateslib.legs.ZeroFixedLeg`. If `None`
+       will be set to mid-market when curves are provided.
+    index_base : float or None, optional
+       The base index applied to all periods.
+    index_fixings : float, or Series, optional
+       If a float scalar, will be applied as the index fixing for the first
+       period.
+       If a list of *n* fixings will be used as the index fixings for the first *n*
+       periods.
+       If a datetime indexed ``Series`` will use the fixings that are available in
+       that object, and derive the rest from the ``curve``.
+    index_method : str
+       Whether the indexing uses a daily measure for settlement or the most recently
+       monthly data taken from the first day of month.
+    index_lag : int, optional
+       The number of months by which the index value is lagged. Used to ensure
+       consistency between curves and forecast values. Defined by default.
+    notional_exchange : bool, optional
+       Whether the legs include final notional exchanges and interim
+       amortization notional exchanges.
+    kwargs : dict
+       Required keyword arguments to :class:`BaseDerivative`.
+
+    Examples
+    --------
+    Construct a curve to price the example.
+
+    .. ipython:: python
+
+      usd = Curve(
+          nodes={
+              dt(2022, 1, 1): 1.0,
+              dt(2027, 1, 1): 0.85,
+              dt(2032, 1, 1): 0.65,
+          },
+          id="usd",
+      )
+      us_cpi = IndexCurve(
+          nodes={
+              dt(2022, 1, 1): 1.0,
+              dt(2027, 1, 1): 0.85,
+              dt(2032, 1, 1): 0.70,
+          },
+          id="us_cpi",
+          index_base=100,
+          index_lag=3,
+      )
+
+    Create the ZCIS, and demonstrate the :meth:`~rateslib.instruments.ZCIS.rate`,
+    :meth:`~rateslib.instruments.ZCIS.npv`,
+    :meth:`~rateslib.instruments.ZCIS.analytic_delta`, and
+
+    .. ipython:: python
+
+      iirs = IIRS(
+          effective=dt(2022, 1, 1),
+          termination="4Y",
+          frequency="A",
+          calendar="nyc",
+          currency="usd",
+          fixed_rate=2.05,
+          convention="1+",
+          notional=100e6,
+          index_base=100.0,
+          index_method="monthly",
+          index_lag=3,
+          index_fixings=None,
+          notional_exchange=True,
+          leg2_convention="Act360",
+          curves=["us_cpi", "usd", "usd", "usd"],
+      )
+      iirs.rate(curves=[us_cpi, usd, usd, usd])
+      iirs.npv(curves=[us_cpi, usd, usd, usd])
+
+    A DataFrame of :meth:`~rateslib.instruments.IIRS.cashflows`.
+
+    .. ipython:: python
+
+      iirs.cashflows(curves=[us_cpi, usd, usd, usd])
+
+    For accurate sensitivity calculations; :meth:`~rateslib.instruments.IIRS.delta`
+    and :meth:`~rateslib.instruments.IIRS.gamma`, construct a curve model.
+
+    .. ipython:: python
+
+      sofr_kws = dict(
+          effective=dt(2022, 1, 1),
+          frequency="A",
+          convention="Act360",
+          calendar="nyc",
+          currency="usd",
+          curves=["usd"]
+      )
+      cpi_kws = dict(
+          effective=dt(2022, 1, 1),
+          frequency="A",
+          convention="1+",
+          calendar="nyc",
+          leg2_index_method="monthly",
+          currency="usd",
+          curves=["usd", "usd", "us_cpi", "usd"]
+      )
+      instruments = [
+          IRS(termination="5Y", **sofr_kws),
+          IRS(termination="10Y", **sofr_kws),
+          ZCIS(termination="5Y", **cpi_kws),
+          ZCIS(termination="10Y", **cpi_kws),
+      ]
+      solver = Solver(
+          curves=[usd, us_cpi],
+          instruments=instruments,
+          s=[3.40, 3.60, 2.2, 2.05],
+          instrument_labels=["5Y", "10Y", "5Yi", "10Yi"],
+          id="us",
+      )
+      iirs.delta(solver=solver)
+      iirs.gamma(solver=solver)
+    """
+
     _fixed_rate_mixin = True
+    _index_base_mixin = True
     _leg2_float_spread_mixin = True
 
     def __init__(
         self,
         *args,
         fixed_rate: Optional[float] = None,
+        index_base: Optional[Union[float, Series]] = None,
+        index_fixings: Optional[Union[float, Series]] = None,
+        index_method: Optional[str] = None,
+        index_lag: Optional[int] = None,
+        notional_exchange: Optional[bool] = False,
+        payment_lag_exchange: Optional[int] = None,
         leg2_float_spread: Optional[float] = None,
-        leg2_spread_compound_method: Optional[str] = None,
-        leg2_fixings: Optional[Union[float, list, Series]] = None,
+        leg2_fixings: Optional[Union[float, list]] = None,
         leg2_fixing_method: Optional[str] = None,
         leg2_method_param: Optional[int] = None,
+        leg2_spread_compound_method: Optional[str] = None,
+        leg2_payment_lag_exchange: Optional[int] = "inherit",
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
+        self._index_base = index_base
         self._fixed_rate = fixed_rate
-        self._leg2_float_spread = leg2_float_spread
-        self.leg1 = FixedLeg(
+        if leg2_payment_lag_exchange == "inherit":
+            leg2_payment_lag_exchange = payment_lag_exchange
+
+        self.notional_exchange = notional_exchange
+        if not notional_exchange:
+            L1, L2 = IndexFixedLeg, FloatLeg
+            l1_args, l2_args = {}, {}
+        else:
+            L1, L2 = IndexFixedLegExchange, FloatLegExchange
+            l1_args = dict(
+                payment_lag_exchange=payment_lag_exchange,
+                initial_exchange=False,
+            )
+            l2_args = dict(
+                payment_lag_exchange=leg2_payment_lag_exchange,
+                initial_exchange=False,
+            )
+
+        self.leg1 = L1(
             fixed_rate=fixed_rate,
             effective=self.effective,
             termination=self.termination,
-            frequency="Z",
+            frequency=self.frequency,
             stub=self.stub,
             front_stub=self.front_stub,
             back_stub=self.back_stub,
             roll=self.roll,
             eom=self.eom,
             modifier=self.modifier,
             calendar=self.calendar,
             payment_lag=self.payment_lag,
             notional=self.notional,
             currency=self.currency,
             amortization=self.amortization,
             convention=self.convention,
+            index_base=index_base,
+            index_method=index_method,
+            index_lag=index_lag,
+            index_fixings=index_fixings,
+            **l1_args,
         )
-        self.leg2 = ZeroFloatLeg(
-            float_spread=leg2_float_spread,
-            spread_compound_method=leg2_spread_compound_method,
-            fixings=leg2_fixings,
-            fixing_method=leg2_fixing_method,
-            method_param=leg2_method_param,
+        self.leg2 = L2(
             effective=self.leg2_effective,
             termination=self.leg2_termination,
             frequency=self.leg2_frequency,
             stub=self.leg2_stub,
             front_stub=self.leg2_front_stub,
             back_stub=self.leg2_back_stub,
             roll=self.leg2_roll,
@@ -3600,75 +4299,397 @@
             modifier=self.leg2_modifier,
             calendar=self.leg2_calendar,
             payment_lag=self.leg2_payment_lag,
             notional=self.leg2_notional,
             currency=self.leg2_currency,
             amortization=self.leg2_amortization,
             convention=self.leg2_convention,
+            float_spread=leg2_float_spread,
+            fixings=leg2_fixings,
+            fixing_method=leg2_fixing_method,
+            method_param=leg2_method_param,
+            spread_compound_method=leg2_spread_compound_method,
+            **l2_args,
         )
 
-    def analytic_delta(self, *args, **kwargs):
+    def _set_pricing_mid(
+        self,
+        curves: Optional[Union[Curve, str, list]] = None,
+        solver: Optional[Solver] = None,
+    ):
+        mid_market_rate = self.rate(curves, solver)
+        self.leg1.fixed_rate = float(mid_market_rate)
+
+    def npv(
+        self,
+        curves: Optional[Union[Curve, str, list]] = None,
+        solver: Optional[Solver] = None,
+        fx: Optional[Union[float, FXRates, FXForwards]] = None,
+        base: Optional[str] = None,
+        local: bool = False,
+    ):
+        curves, _ = _get_curves_and_fx_maybe_from_solver(
+            self.curves, solver, curves, fx
+        )
+        if self.index_base is None:
+            # must forecast for the leg
+            self.leg1.index_base = curves[0].index_value(
+                self.leg1.schedule.effective, self.leg1.index_method
+            )
+        if self.fixed_rate is None:
+            # set a fixed rate for the purpose of pricing NPV, which should be zero.
+            self._set_pricing_mid(curves, solver)
+        return super().npv(curves, solver, fx, base, local)
+
+    def cashflows(
+        self,
+        curves: Optional[Union[Curve, str, list]] = None,
+        solver: Optional[Solver] = None,
+        fx: Optional[Union[float, FXRates, FXForwards]] = None,
+        base: Optional[str] = None,
+    ):
+        curves, _ = _get_curves_and_fx_maybe_from_solver(
+            self.curves, solver, curves, fx
+        )
+        if self.index_base is None:
+            # must forecast for the leg
+            self.leg1.index_base = curves[0].index_value(
+                self.leg1.schedule.effective, self.leg1.index_method
+            )
+        return super().cashflows(curves, solver, fx, base)
+
+    def rate(
+        self,
+        curves: Optional[Union[Curve, str, list]] = None,
+        solver: Optional[Solver] = None,
+        fx: Optional[Union[float, FXRates, FXForwards]] = None,
+        base: Optional[str] = None,
+    ):
         """
-        Return the analytic delta of a leg of the derivative object.
+        Return the mid-market rate of the IRS.
 
-        See :meth:`BaseDerivative.analytic_delta`.
+        Parameters
+        ----------
+        curves : Curve, str or list of such
+            A single :class:`~rateslib.curves.Curve` or id or a list of such.
+            A list defines the following curves in the order:
+
+            - Forecasting :class:`~rateslib.curves.Curve` for floating leg.
+            - Discounting :class:`~rateslib.curves.Curve` for both legs.
+        solver : Solver, optional
+            The numerical :class:`~rateslib.solver.Solver` that
+            constructs :class:`~rateslib.curves.Curve` from calibrating instruments.
+
+            .. note::
+
+               The arguments ``fx`` and ``base`` are unused by single currency
+               derivatives rates calculations.
+
+        Returns
+        -------
+        float, Dual or Dual2
+
+        Notes
+        -----
+        The arguments ``fx`` and ``base`` are unused by single currency derivatives
+        rates calculations.
+        """
+        curves, _ = _get_curves_and_fx_maybe_from_solver(
+            self.curves, solver, curves, fx
+        )
+        if self.index_base is None:
+            # must forecast for the leg
+            self.leg1.index_base = curves[0].index_value(
+                self.leg1.schedule.effective, self.leg1.index_method
+            )
+        leg2_npv = self.leg2.npv(curves[2], curves[3])
+
+        if self.fixed_rate is None:
+            self.leg1.fixed_rate = 0.0
+        _existing = self.leg1.fixed_rate
+        leg1_npv = self.leg1.npv(curves[0], curves[1])
+
+        _ = self.leg1._spread(-leg2_npv - leg1_npv, curves[0], curves[1]) / 100
+        return _ + _existing
+
+    def spread(
+        self,
+        curves: Optional[Union[Curve, str, list]] = None,
+        solver: Optional[Solver] = None,
+        fx: Optional[Union[float, FXRates, FXForwards]] = None,
+        base: Optional[str] = None,
+    ):
+        """
+        Return the mid-market float spread (bps) required to equate to the fixed rate.
+
+        Parameters
+        ----------
+        curves : Curve, str or list of such
+            A single :class:`~rateslib.curves.Curve` or id or a list of such.
+            A list defines the following curves in the order:
+
+            - Forecasting :class:`~rateslib.curves.Curve` for floating leg.
+            - Discounting :class:`~rateslib.curves.Curve` for both legs.
+        solver : Solver, optional
+            The numerical :class:`~rateslib.solver.Solver` that constructs
+            :class:`~rateslib.curves.Curve` from calibrating instruments.
+
+            .. note::
+
+               The arguments ``fx`` and ``base`` are unused by single currency
+               derivatives rates calculations.
+
+        Returns
+        -------
+        float, Dual or Dual2
+
+        Notes
+        -----
+        If the :class:`IRS` is specified without a ``fixed_rate`` this should always
+        return the current ``leg2_float_spread`` value or zero since the fixed rate used
+        for calculation is the implied rate including the current ``leg2_float_spread``
+        parameter.
 
         Examples
         --------
+        For the most common parameters this method will be exact.
+
         .. ipython:: python
 
-           forecasting_curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.98})
-           discounting_curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.985})
+           irs.spread(curves=usd)
+           irs.leg2_float_spread = -6.948753
+           irs.npv(curves=usd)
+
+        When a non-linear spread compound method is used for float RFR legs this is
+        an approximation, via second order Taylor expansion.
 
         .. ipython:: python
 
            irs = IRS(
                effective=dt(2022, 2, 15),
                termination=dt(2022, 8, 15),
                frequency="Q",
                convention="30e360",
                leg2_convention="Act360",
                leg2_fixing_method="rfr_payment_delay",
+               leg2_spread_compound_method="isda_compounding",
                payment_lag=2,
                fixed_rate=2.50,
-               notional=1e9,
-               currency="gbp",
+               leg2_float_spread=0,
+               notional=50000000,
+               currency="usd",
            )
-           irs.analytic_delta(forecasting_curve, discounting_curve, leg=1)
+           irs.spread(curves=usd)
+           irs.leg2_float_spread = -111.060143
+           irs.npv(curves=usd)
+           irs.spread(curves=usd)
+
+        The ``leg2_float_spread`` is determined through NPV differences. If the difference
+        is small since the defined spread is already quite close to the solution the
+        approximation is much more accurate. This is shown above where the second call
+        to ``irs.spread`` is different to the previous call, albeit the difference
+        is 1/10000th of a basis point.
+        """
+        irs_npv = self.npv(curves, solver)
+        specified_spd = 0 if self.leg2.float_spread is None else self.leg2.float_spread
+        curves, _ = _get_curves_and_fx_maybe_from_solver(
+            self.curves, solver, curves, fx
+        )
+        return self.leg2._spread(-irs_npv, curves[2], curves[3]) + specified_spd
+
+
+class ZCS(BaseDerivative):
+    """
+    Create a zero coupon swap (ZCS) composing a :class:`~rateslib.legs.ZeroFixedLeg`
+    and a :class:`~rateslib.legs.ZeroFloatLeg`.
+
+    Parameters
+    ----------
+    args : dict
+        Required positional args to :class:`BaseDerivative`.
+    fixed_rate : float or None
+        The fixed rate applied to the :class:`~rateslib.legs.ZeroFixedLeg`. If `None`
+        will be set to mid-market when curves are provided.
+    leg2_float_spread : float, optional
+        The spread applied to the :class:`~rateslib.legs.FloatLeg`. Can be set to
+        `None` and designated
+        later, perhaps after a mid-market spread for all periods has been calculated.
+    leg2_spread_compound_method : str, optional
+        The method to use for adding a floating spread to compounded rates. Available
+        options are `{"none_simple", "isda_compounding", "isda_flat_compounding"}`.
+    leg2_fixings : float, list, or Series optional
+        If a float scalar, will be applied as the determined fixing for the first
+        period. If a list of *n* fixings will be used as the fixings for the first *n*
+        periods. If any sublist of length *m* is given, is used as the first *m* RFR
+        fixings for that :class:`~rateslib.periods.FloatPeriod`. If a datetime
+        indexed ``Series`` will use the fixings that are available in that object,
+        and derive the rest from the ``curve``.
+    leg2_fixing_method : str, optional
+        The method by which floating rates are determined, set by default. See notes.
+    leg2_method_param : int, optional
+        A parameter that is used for the various ``fixing_method`` s. See notes.
+    kwargs : dict
+        Required keyword arguments to :class:`BaseDerivative`.
+
+    Examples
+    --------
+    Construct a curve to price the example.
+
+    .. ipython:: python
+
+       usd = Curve(
+           nodes={
+               dt(2022, 1, 1): 1.0,
+               dt(2027, 1, 1): 0.85,
+               dt(2032, 1, 1): 0.70,
+           },
+           id="usd"
+       )
+
+    Create the ZCS, and demonstrate the :meth:`~rateslib.instruments.ZCS.rate`,
+    :meth:`~rateslib.instruments.ZCS.npv`,
+    :meth:`~rateslib.instruments.ZCS.analytic_delta`, and
+
+    .. ipython:: python
+
+       zcs = ZCS(
+           effective=dt(2022, 1, 1),
+           termination="10Y",
+           frequency="Q",
+           calendar="nyc",
+           currency="usd",
+           fixed_rate=4.0,
+           convention="Act360",
+           notional=100e6,
+           curves=["usd"],
+       )
+       zcs.rate(curves=usd)
+       zcs.npv(curves=usd)
+       zcs.analytic_delta(curve=usd)
+
+    A DataFrame of :meth:`~rateslib.instruments.ZCS.cashflows`.
+
+    .. ipython:: python
+
+       zcs.cashflows(curves=usd)
+
+    For accurate sensitivity calculations; :meth:`~rateslib.instruments.ZCS.delta`
+    and :meth:`~rateslib.instruments.ZCS.gamma`, construct a curve model.
+
+    .. ipython:: python
+
+       sofr_kws = dict(
+           effective=dt(2022, 1, 1),
+           frequency="A",
+           convention="Act360",
+           calendar="nyc",
+           currency="usd",
+           curves=["usd"]
+       )
+       instruments = [
+           IRS(termination="5Y", **sofr_kws),
+           IRS(termination="10Y", **sofr_kws),
+       ]
+       solver = Solver(
+           curves=[usd],
+           instruments=instruments,
+           s=[3.40, 3.60],
+           instrument_labels=["5Y", "10Y"],
+           id="sofr",
+       )
+       zcs.delta(solver=solver)
+       zcs.gamma(solver=solver)
+    """
+
+    _fixed_rate_mixin = True
+    _leg2_float_spread_mixin = True
+
+    def __init__(
+        self,
+        *args,
+        fixed_rate: Optional[float] = None,
+        leg2_float_spread: Optional[float] = None,
+        leg2_spread_compound_method: Optional[str] = None,
+        leg2_fixings: Optional[Union[float, list, Series]] = None,
+        leg2_fixing_method: Optional[str] = None,
+        leg2_method_param: Optional[int] = None,
+        **kwargs,
+    ):
+        super().__init__(*args, **kwargs)
+        self._fixed_rate = fixed_rate
+        self._leg2_float_spread = leg2_float_spread
+        self.leg1 = ZeroFixedLeg(
+            fixed_rate=fixed_rate,
+            effective=self.effective,
+            termination=self.termination,
+            frequency=self.frequency,
+            stub=self.stub,
+            front_stub=self.front_stub,
+            back_stub=self.back_stub,
+            roll=self.roll,
+            eom=self.eom,
+            modifier=self.modifier,
+            calendar=self.calendar,
+            payment_lag=self.payment_lag,
+            notional=self.notional,
+            currency=self.currency,
+            amortization=self.amortization,
+            convention=self.convention,
+        )
+        self.leg2 = ZeroFloatLeg(
+            float_spread=leg2_float_spread,
+            spread_compound_method=leg2_spread_compound_method,
+            fixings=leg2_fixings,
+            fixing_method=leg2_fixing_method,
+            method_param=leg2_method_param,
+            effective=self.leg2_effective,
+            termination=self.leg2_termination,
+            frequency=self.leg2_frequency,
+            stub=self.leg2_stub,
+            front_stub=self.leg2_front_stub,
+            back_stub=self.leg2_back_stub,
+            roll=self.leg2_roll,
+            eom=self.leg2_eom,
+            modifier=self.leg2_modifier,
+            calendar=self.leg2_calendar,
+            payment_lag=self.leg2_payment_lag,
+            notional=self.leg2_notional,
+            currency=self.leg2_currency,
+            amortization=self.leg2_amortization,
+            convention=self.leg2_convention,
+        )
+
+    def analytic_delta(self, *args, **kwargs):
+        """
+        Return the analytic delta of a leg of the derivative object.
+
+        See :meth:`BaseDerivative.analytic_delta<rateslib.instruments.BaseDerivative.analytic_delta>`.
         """
         return super().analytic_delta(*args, **kwargs)
 
+    def _set_pricing_mid(self, curves, solver):
+        mid_market_rate = self.rate(curves, solver)
+        self.leg1.fixed_rate = float(mid_market_rate)
+
     def npv(
         self,
         curves: Optional[Union[Curve, str, list]] = None,
         solver: Optional[Solver] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
         local: bool = False,
     ):
         """
         Return the NPV of the derivative by summing legs.
 
         See :meth:`BaseDerivative.npv`.
-
-        Examples
-        --------
-        .. ipython:: python
-
-           irs.npv([forecasting_curve, discounting_curve])
-
-        .. ipython:: python
-
-           fxr = FXRates({"gbpusd": 2.0})
-           irs.npv([forecasting_curve, discounting_curve], None, fxr, "usd")
         """
         if self.fixed_rate is None:
             # set a fixed rate for the purpose of pricing NPV, which should be zero.
-            mid_market_rate = self.rate(curves, solver)
-            self.leg1.fixed_rate = mid_market_rate.real
+            self._set_pricing_mid(curves, solver)
         return super().npv(curves, solver, fx, base, local)
 
     def rate(
         self,
         curves: Optional[Union[Curve, str, list]] = None,
         solver: Optional[Solver] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
@@ -3698,43 +4719,294 @@
         -------
         float, Dual or Dual2
 
         Notes
         -----
         The arguments ``fx`` and ``base`` are unused by single currency derivatives
         rates calculations.
+
+        The *'irr'* ``fixed_rate`` defines a cashflow by:
+
+        .. math::
+
+           -notional * ((1 + irr / f)^{f \\times dcf} - 1)
+
+        where :math:`f` is associated with the compounding frequency.
         """
         curves, _ = _get_curves_and_fx_maybe_from_solver(
             self.curves, solver, curves, fx
         )
         leg2_npv = self.leg2.npv(curves[2], curves[3])
-        return self.leg1._spread(-leg2_npv, curves[0], curves[1]) / 100
-        # leg1_analytic_delta = self.leg1.analytic_delta(curves[0], curves[1])
-        # return leg2_npv / (leg1_analytic_delta * 100)
+        _ = self.leg1._spread(-leg2_npv, curves[0], curves[1]) / 100
+        return _
 
     def cashflows(
         self,
         curves: Optional[Union[Curve, str, list]] = None,
         solver: Optional[Solver] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
     ):
         """
         Return the properties of all legs used in calculating cashflows.
 
         See :meth:`BaseDerivative.cashflows`.
+        """
+        return super().cashflows(curves, solver, fx, base)
 
-        Examples
-        --------
-        .. ipython:: python
 
-           fxr = FXRates({"gbpusd": 2.0})
-           irs.cashflows([forecasting_curve, discounting_curve], None, fxr, "usd")
+class ZCIS(BaseDerivative):
+    """
+    Create a zero coupon index swap (ZCIS) composing an
+    :class:`~rateslib.legs.ZeroFixedLeg`
+    and a :class:`~rateslib.legs.ZeroIndexLeg`.
+
+    Parameters
+    ----------
+    args : dict
+        Required positional args to :class:`BaseDerivative`.
+    fixed_rate : float or None
+        The fixed rate applied to the :class:`~rateslib.legs.ZeroFixedLeg`. If `None`
+        will be set to mid-market when curves are provided.
+    index_base : float or None, optional
+        The base index applied to all periods.
+    index_fixings : float, or Series, optional
+        If a float scalar, will be applied as the index fixing for the first
+        period.
+        If a list of *n* fixings will be used as the index fixings for the first *n*
+        periods.
+        If a datetime indexed ``Series`` will use the fixings that are available in
+        that object, and derive the rest from the ``curve``.
+    index_method : str
+        Whether the indexing uses a daily measure for settlement or the most recently
+        monthly data taken from the first day of month.
+    index_lag : int, optional
+        The number of months by which the index value is lagged. Used to ensure
+        consistency between curves and forecast values. Defined by default.
+    kwargs : dict
+        Required keyword arguments to :class:`BaseDerivative`.
+
+    Examples
+    --------
+    Construct a curve to price the example.
+
+    .. ipython:: python
+
+       usd = Curve(
+           nodes={
+               dt(2022, 1, 1): 1.0,
+               dt(2027, 1, 1): 0.85,
+               dt(2032, 1, 1): 0.65,
+           },
+           id="usd",
+       )
+       us_cpi = IndexCurve(
+           nodes={
+               dt(2022, 1, 1): 1.0,
+               dt(2027, 1, 1): 0.85,
+               dt(2032, 1, 1): 0.70,
+           },
+           id="us_cpi",
+           index_base=100,
+           index_lag=3,
+       )
+
+    Create the ZCIS, and demonstrate the :meth:`~rateslib.instruments.ZCIS.rate`,
+    :meth:`~rateslib.instruments.ZCIS.npv`,
+    :meth:`~rateslib.instruments.ZCIS.analytic_delta`, and
+
+    .. ipython:: python
+
+       zcis = ZCIS(
+           effective=dt(2022, 1, 1),
+           termination="10Y",
+           frequency="A",
+           calendar="nyc",
+           currency="usd",
+           fixed_rate=2.05,
+           convention="1+",
+           notional=100e6,
+           leg2_index_base=100.0,
+           leg2_index_method="monthly",
+           leg2_index_lag=3,
+           leg2_index_fixings=None,
+           curves=["usd", "usd", "us_cpi", "usd"],
+       )
+       zcis.rate(curves=[usd, usd, us_cpi, usd])
+       zcis.npv(curves=[usd, usd, us_cpi, usd])
+       zcis.analytic_delta(usd, usd)
+
+    A DataFrame of :meth:`~rateslib.instruments.ZCIS.cashflows`.
+
+    .. ipython:: python
+
+       zcis.cashflows(curves=[usd, usd, us_cpi, usd])
+
+    For accurate sensitivity calculations; :meth:`~rateslib.instruments.ZCIS.delta`
+    and :meth:`~rateslib.instruments.ZCIS.gamma`, construct a curve model.
+
+    .. ipython:: python
+
+       sofr_kws = dict(
+           effective=dt(2022, 1, 1),
+           frequency="A",
+           convention="Act360",
+           calendar="nyc",
+           currency="usd",
+           curves=["usd"]
+       )
+       cpi_kws = dict(
+           effective=dt(2022, 1, 1),
+           frequency="A",
+           convention="1+",
+           calendar="nyc",
+           leg2_index_method="monthly",
+           currency="usd",
+           curves=["usd", "usd", "us_cpi", "usd"]
+       )
+       instruments = [
+           IRS(termination="5Y", **sofr_kws),
+           IRS(termination="10Y", **sofr_kws),
+           ZCIS(termination="5Y", **cpi_kws),
+           ZCIS(termination="10Y", **cpi_kws),
+       ]
+       solver = Solver(
+           curves=[usd, us_cpi],
+           instruments=instruments,
+           s=[3.40, 3.60, 2.2, 2.05],
+           instrument_labels=["5Y", "10Y", "5Yi", "10Yi"],
+           id="us",
+       )
+       zcis.delta(solver=solver)
+       zcis.gamma(solver=solver)
+    """
+
+    _fixed_rate_mixin = True
+    _leg2_index_base_mixin = True
+
+    def __init__(
+        self,
+        *args,
+        fixed_rate: Optional[float] = None,
+        leg2_index_base: Optional[Union[float, Series]] = None,
+        leg2_index_fixings: Optional[Union[float, Series]] = None,
+        leg2_index_method: Optional[str] = None,
+        leg2_index_lag: Optional[int] = None,
+        **kwargs,
+    ):
+        super().__init__(*args, **kwargs)
+        self._fixed_rate = fixed_rate
+        self._leg2_index_base = leg2_index_base
+        self.leg1 = ZeroFixedLeg(
+            fixed_rate=fixed_rate,
+            effective=self.effective,
+            termination=self.termination,
+            frequency=self.frequency,
+            stub=self.stub,
+            front_stub=self.front_stub,
+            back_stub=self.back_stub,
+            roll=self.roll,
+            eom=self.eom,
+            modifier=self.modifier,
+            calendar=self.calendar,
+            payment_lag=self.payment_lag,
+            notional=self.notional,
+            currency=self.currency,
+            amortization=self.amortization,
+            convention=self.convention,
+        )
+        self.leg2 = ZeroIndexLeg(
+            index_base=leg2_index_base,
+            index_method=leg2_index_method,
+            index_lag=leg2_index_lag,
+            index_fixings=leg2_index_fixings,
+            effective=self.leg2_effective,
+            termination=self.leg2_termination,
+            frequency=self.leg2_frequency,
+            stub=self.leg2_stub,
+            front_stub=self.leg2_front_stub,
+            back_stub=self.leg2_back_stub,
+            roll=self.leg2_roll,
+            eom=self.leg2_eom,
+            modifier=self.leg2_modifier,
+            calendar=self.leg2_calendar,
+            payment_lag=self.leg2_payment_lag,
+            notional=self.leg2_notional,
+            currency=self.leg2_currency,
+            amortization=self.leg2_amortization,
+            convention=self.leg2_convention,
+        )
+
+    def _set_pricing_mid(self, curves, solver):
+        mid_market_rate = self.rate(curves, solver)
+        self.leg1.fixed_rate = float(mid_market_rate)
+
+    def cashflows(self, *args, **kwargs):
+        return super().cashflows(*args, **kwargs)
+
+    def npv(
+            self,
+            curves: Optional[Union[Curve, str, list]] = None,
+            solver: Optional[Solver] = None,
+            fx: Optional[Union[float, FXRates, FXForwards]] = None,
+            base: Optional[str] = None,
+            local: bool = False,
+    ):
+        if self.fixed_rate is None:
+            # set a fixed rate for the purpose of pricing NPV, which should be zero.
+            self._set_pricing_mid(curves, solver)
+        return super().npv(curves, solver, fx, base, local)
+
+    def rate(
+        self,
+        curves: Optional[Union[Curve, str, list]] = None,
+        solver: Optional[Solver] = None,
+        fx: Optional[Union[float, FXRates, FXForwards]] = None,
+        base: Optional[str] = None,
+    ):
         """
-        return super().cashflows(curves, solver, fx, base)
+        Return the mid-market IRR rate of the ZCIS.
+
+        Parameters
+        ----------
+        curves : Curve, str or list of such
+            A single :class:`~rateslib.curves.Curve` or id or a list of such.
+            A list defines the following curves in the order:
+
+            - Forecasting :class:`~rateslib.curves.Curve` for floating leg.
+            - Discounting :class:`~rateslib.curves.Curve` for both legs.
+        solver : Solver, optional
+            The numerical :class:`~rateslib.solver.Solver` that
+            constructs :class:`~rateslib.curves.Curve` from calibrating instruments.
+
+            .. note::
+
+               The arguments ``fx`` and ``base`` are unused by single currency
+               derivatives rates calculations.
+
+        Returns
+        -------
+        float, Dual or Dual2
+
+        Notes
+        -----
+        The arguments ``fx`` and ``base`` are unused by single currency derivatives
+        rates calculations.
+        """
+        curves, _ = _get_curves_and_fx_maybe_from_solver(
+            self.curves, solver, curves, fx
+        )
+        if self.leg2_index_base is None:
+            # must forecast for the leg
+            self.leg2.index_base = curves[2].index_value(
+                self.leg2.schedule.effective, self.leg2.index_method
+            )
+        leg2_npv = self.leg2.npv(curves[2], curves[3])
+
+        return self.leg1._spread(-leg2_npv, curves[0], curves[1]) / 100
 
 
 class SBS(BaseDerivative):
     """
     Create a single currency basis swap composing two
     :class:`~rateslib.legs.FloatLeg` s.
 
@@ -3779,14 +5051,115 @@
         and derive the rest from the ``curve``.
     leg2_fixing_method : str, optional
         The method by which floating rates are determined, set by default. See notes.
     leg2_method_param : int, optional
         A parameter that is used for the various ``fixing_method`` s. See notes.
     kwargs : dict
         Required keyword arguments to :class:`BaseDerivative`.
+
+    Examples
+    --------
+    Construct curves to price the example.
+
+    .. ipython:: python
+
+       eur3m = Curve(
+           nodes={
+               dt(2022, 1, 1): 1.0,
+               dt(2023, 1, 1): 0.965,
+               dt(2024, 1, 1): 0.94
+           },
+           id="eur3m",
+       )
+       eur6m = Curve(
+           nodes={
+               dt(2022, 1, 1): 1.0,
+               dt(2023, 1, 1): 0.962,
+               dt(2024, 1, 1): 0.936
+           },
+           id="eur6m",
+       )
+
+    Create the SBS, and demonstrate the :meth:`~rateslib.instruments.SBS.rate`,
+    :meth:`~rateslib.instruments.SBS.npv`,
+    :meth:`~rateslib.instruments.SBS.analytic_delta`, and
+    :meth:`~rateslib.instruments.SBS.spread`.
+
+    .. ipython:: python
+
+       sbs = SBS(
+           effective=dt(2022, 1, 1),
+           termination="18M",
+           frequency="Q",
+           leg2_frequency="S",
+           calendar="tgt",
+           currency="eur",
+           fixing_method="ibor",
+           method_param=2,
+           convention="Act360",
+           leg2_float_spread=-22.9,
+           notional=100e6,
+           curves=["eur3m", "eur3m", "eur6m", "eur3m"],
+       )
+       sbs.rate(curves=[eur3m, eur3m, eur6m, eur3m])
+       sbs.npv(curves=[eur3m, eur3m, eur6m, eur3m])
+       sbs.analytic_delta(curve=eur6m, disc_curve=eur3m, leg=2)
+       sbs.spread(curves=[eur3m, eur3m, eur6m, eur3m], leg=2)
+
+    A DataFrame of :meth:`~rateslib.instruments.SBS.cashflows`.
+
+    .. ipython:: python
+
+       sbs.cashflows(curves=[eur3m, eur3m, eur6m, eur3m])
+
+    For accurate sensitivity calculations; :meth:`~rateslib.instruments.SBS.delta`
+    and :meth:`~rateslib.instruments.SBS.gamma`, construct a curve model.
+
+    .. ipython:: python
+
+       irs_kws = dict(
+           effective=dt(2022, 1, 1),
+           frequency="A",
+           leg2_frequency="Q",
+           convention="30E360",
+           leg2_convention="Act360",
+           leg2_fixing_method="ibor",
+           leg2_method_param=2,
+           calendar="tgt",
+           currency="eur",
+           curves=["eur3m", "eur3m"],
+       )
+       sbs_kws = dict(
+           effective=dt(2022, 1, 1),
+           frequency="Q",
+           leg2_frequency="S",
+           convention="Act360",
+           fixing_method="ibor",
+           method_param=2,
+           leg2_convention="Act360",
+           calendar="tgt",
+           currency="eur",
+           curves=["eur3m", "eur3m", "eur6m", "eur3m"]
+       )
+       instruments = [
+           IRS(termination="1Y", **irs_kws),
+           IRS(termination="2Y", **irs_kws),
+           SBS(termination="1Y", **sbs_kws),
+           SBS(termination="2Y", **sbs_kws),
+       ]
+       solver = Solver(
+           curves=[eur3m, eur6m],
+           instruments=instruments,
+           s=[1.55, 1.6, 5.5, 6.5],
+           instrument_labels=["1Y", "2Y", "1Y 3s6s", "2Y 3s6s"],
+           id="eur",
+       )
+       sbs.delta(solver=solver)
+       sbs.gamma(solver=solver)
+
     """
 
     _float_spread_mixin = True
     _leg2_float_spread_mixin = True
     _rate_scalar = 100.0
 
     def __init__(
@@ -3848,61 +5221,37 @@
             payment_lag=self.leg2_payment_lag,
             notional=self.leg2_notional,
             currency=self.leg2_currency,
             amortization=self.leg2_amortization,
             convention=self.leg2_convention,
         )
 
+    def _set_pricing_mid(self, curves, solver):
+        rate = self.rate(curves, solver)
+        self.leg1.float_spread = float(rate)
+
     def analytic_delta(self, *args, **kwargs):
         """
         Return the analytic delta of a leg of the derivative object.
 
         See :meth:`BaseDerivative.analytic_delta`.
-
-        Examples
-        --------
-        .. ipython:: python
-
-           forecasting_curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.98})
-           forecasting_curve2 = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.97})
-           discounting_curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.985})
-
-        .. ipython:: python
-
-           sbs = SBS(
-               effective=dt(2022, 2, 15),
-               termination=dt(2022, 8, 15),
-               frequency="Q",
-               leg2_frequency="S",
-               leg2_float_spread=-50.0,
-               convention="Act360",
-               payment_lag=2,
-               notional=1e9,
-           )
-           sbs.analytic_delta(forecasting_curve, discounting_curve, leg=1)
         """
         return super().analytic_delta(*args, **kwargs)
 
     def cashflows(
         self,
         curves: Optional[Union[Curve, str, list]] = None,
         solver: Optional[Solver] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
     ):
         """
         Return the properties of all legs used in calculating cashflows.
 
         See :meth:`BaseDerivative.cashflows`.
-
-        Examples
-        --------
-        .. ipython:: python
-
-           sbs.cashflows([forecasting_curve, discounting_curve, forecasting_curve2])
         """
         return super().cashflows(curves, solver, fx, base)
 
     def npv(
         self,
         curves: Optional[Union[Curve, str, list]] = None,
         solver: Optional[Solver] = None,
@@ -3910,21 +5259,18 @@
         base: Optional[str] = None,
         local: bool = False,
     ):
         """
         Return the NPV of the derivative object by summing legs.
 
         See :meth:`BaseDerivative.npv`.
-
-        Examples
-        --------
-        .. ipython:: python
-
-           sbs.npv([forecasting_curve, discounting_curve, forecasting_curve2])
         """
+        if self.float_spread is None and self.leg2_float_spread is None:
+            # set a pricing parameter for the purpose of pricing NPV at zero.
+            self._set_pricing_mid(curves, solver)
         return super().npv(curves, solver, fx, base, local)
 
     def rate(
         self,
         curves: Optional[Union[Curve, str, list]] = None,
         solver: Optional[Solver] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
@@ -3948,33 +5294,26 @@
             instruments.
         leg: int in [1, 2]
             Specify which leg the spread calculation is applied to.
 
         Returns
         -------
         float, Dual or Dual2
-
-        Examples
-        --------
-        .. ipython:: python
-
-           sbs.rate([forecasting_curve, discounting_curve, forecasting_curve2], leg=1)
-           sbs.rate([forecasting_curve, discounting_curve, forecasting_curve2], leg=2)
         """
-        irs_npv = self.npv(curves, solver)
+        core_npv = super().npv(curves, solver)
         curves, _ = _get_curves_and_fx_maybe_from_solver(
             self.curves, solver, curves, fx
         )
         if leg == 1:
             leg_obj, args = self.leg1, (curves[0], curves[1])
         else:
             leg_obj, args = self.leg2, (curves[2], curves[3])
 
         specified_spd = 0 if leg_obj.float_spread is None else leg_obj.float_spread
-        return leg_obj._spread(-irs_npv, *args) + specified_spd
+        return leg_obj._spread(-core_npv, *args) + specified_spd
 
         # irs_npv = self.npv(curves, solver)
         # curves, _ = self._get_curves_and_fx_maybe_from_solver(solver, curves, None)
         # if leg == 1:
         #     args = (curves[0], curves[1])
         # else:
         #     args = (curves[2], curves[3])
@@ -4001,39 +5340,105 @@
     Parameters
     ----------
     args : dict
         Required positional args to :class:`BaseDerivative`.
     fixed_rate : float or None
         The fixed rate applied to the :class:`~rateslib.legs.FixedLeg`. If `None`
         will be set to mid-market when curves are provided.
-    float_spread : float, optional
-        The spread applied to the :class:`~rateslib.legs.FloatLeg`. Can be set to
-        `None` and designated
-        later, perhaps after a mid-market spread for all periods has been calculated.
-    spread_compound_method : str, optional
-        The method to use for adding a floating spread to compounded rates. Available
-        options are `{"none_simple", "isda_compounding", "isda_flat_compounding"}`.
     fixings : float or list, optional
         If a float scalar, will be applied as the determined fixing for the first
         period. If a list of *n* fixings will be used as the fixings for the first *n*
         periods. If any sublist of length *m* is given as the first *m* RFR fixings
         within individual curve and composed into the overall rate.
-    fixing_method : str, optional
-        The method by which floating rates are determined, set by default. See notes.
     method_param : int, optional
         A parameter that is used for the various ``fixing_method`` s. See notes.
     kwargs : dict
         Required keyword arguments to :class:`BaseDerivative`.
 
     Notes
     -----
     FRAs are a legacy derivative whose ``fixing_method`` is set to *"ibor"*.
 
     ``effective`` and ``termination`` are not adjusted prior to initialising
     ``Periods``. Care should be taken to enter these exactly.
+
+    Examples
+    --------
+    Construct curves to price the example.
+
+    .. ipython:: python
+
+       eur3m = Curve(
+           nodes={
+               dt(2022, 1, 1): 1.0,
+               dt(2023, 1, 1): 0.965,
+               dt(2024, 1, 1): 0.94
+           },
+           id="eur3m",
+       )
+
+    Create the FRA, and demonstrate the :meth:`~rateslib.instruments.FRA.rate`,
+    :meth:`~rateslib.instruments.FRA.npv`,
+    :meth:`~rateslib.instruments.FRA.analytic_delta`.
+
+    .. ipython:: python
+
+       fra = FRA(
+           effective=dt(2023, 2, 15),
+           termination="3M",
+           frequency="Q",
+           calendar="tgt",
+           currency="eur",
+           method_param=2,
+           convention="Act360",
+           notional=100e6,
+           fixed_rate=2.617,
+           curves=["eur3m"],
+       )
+       fra.rate(curves=eur3m)
+       fra.npv(curves=eur3m)
+       fra.analytic_delta(curve=eur3m)
+
+    A DataFrame of :meth:`~rateslib.instruments.FRA.cashflows`.
+
+    .. ipython:: python
+
+       fra.cashflows(curves=eur3m)
+
+    For accurate sensitivity calculations; :meth:`~rateslib.instruments.FRA.delta`
+    and :meth:`~rateslib.instruments.FRA.gamma`, construct a curve model.
+
+    .. ipython:: python
+
+       irs_kws = dict(
+           effective=dt(2022, 1, 1),
+           frequency="A",
+           leg2_frequency="Q",
+           convention="30E360",
+           leg2_convention="Act360",
+           leg2_fixing_method="ibor",
+           leg2_method_param=2,
+           calendar="tgt",
+           currency="eur",
+           curves=["eur3m", "eur3m"],
+       )
+       instruments = [
+           IRS(termination="1Y", **irs_kws),
+           IRS(termination="2Y", **irs_kws),
+       ]
+       solver = Solver(
+           curves=[eur3m],
+           instruments=instruments,
+           s=[1.55, 1.6],
+           instrument_labels=["1Y", "2Y"],
+           id="eur",
+       )
+       fra.delta(solver=solver)
+       fra.gamma(solver=solver)
+
     """
 
     _fixed_rate_mixin = True
 
     def __init__(
         self,
         effective: datetime,
@@ -4045,15 +5450,15 @@
         convention: Optional[str] = None,
         method_param: Optional[int] = None,
         payment_lag: Optional[int] = None,
         fixed_rate: Optional[float] = None,
         fixings: Optional[Union[float, Series]] = None,
         currency: Optional[str] = None,
         curves: Optional[Union[str, list, Curve]] = None,
-    ):
+    ) -> None:
         self.curves = curves
         self.currency = defaults.base_currency if currency is None else currency.lower()
 
         if isinstance(modifier, bool):  # then get default
             modifier_: Optional[str] = defaults.modifier
         else:
             modifier_ = modifier.upper()
@@ -4097,96 +5502,58 @@
             fixing_method="ibor",
             method_param=method_param,
             fixings=fixings,
             convention=convention,
             frequency=frequency,
             stub=False,
             currency=self.currency,
-            notional=self.notional,
+            notional=-self.notional,
         )  # FloatPeriod is used only to access the rate method for calculations.
 
+    def _set_pricing_mid(
+        self,
+        curves: Optional[Union[Curve, str, list]] = None,
+        solver: Optional[Solver] = None,
+    ) -> None:
+        mid_market_rate = self.rate(curves, solver)
+        self.leg1.fixed_rate = mid_market_rate.real
+
     def analytic_delta(
         self,
         curve: Curve,
         disc_curve: Optional[Curve] = None,
         fx: Union[float, FXRates, FXForwards] = 1.0,
         base: Optional[str] = None,
-    ):
+    ) -> DualTypes:
         """
         Return the analytic delta of the FRA.
 
-        Parameters
-        ----------
-        curve : Curve
-            The forecasting curve object.
-        disc_curve : Curve, optional
-            The discounting curve object. Set equal to ``curve`` if not given.
-        fx : float, FXRates, FXForwards, optional
-            The immediate settlement FX rate that will be used to convert values
-            into another currency. A given `float` is used directly. If giving a
-            ``FXRates`` or ``FXForwards`` object, converts from local currency
-            into ``base``.
-        base : str, optional
-            The base currency to convert cashflows into (3 digit code), set by default.
-            Only used if ``fx_rate`` is an ``FXRates`` or ``FXForwards`` object.
-
-        Returns
-        -------
-        flaat, Dual or Dual2
-
-        Examples
-        --------
-        .. ipython:: python
-
-           forecasting_curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.98})
-           discounting_curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.985})
-
-        .. ipython:: python
-
-           fra = FRA(
-               effective=dt(2022, 3, 15),
-               termination=dt(2022, 6, 15),
-               frequency="Q",
-               convention="Act360",
-               fixed_rate=2.50,
-               notional=1000000,
-               currency="gbp"
-           )
-           fra.analytic_delta(forecasting_curve, discounting_curve)
+        For arguments see :meth:`~rateslib.periods.BasePeriod.analytic_delta`.
         """
         disc_curve = disc_curve or curve
         fx, base = _get_fx_and_base(self.currency, fx, base)
         rate = self.rate([curve])
         _ = self.notional * self.leg1.dcf * disc_curve[self.payment] / 10000
         return fx * _ / (1 + self.leg1.dcf * rate / 100)
 
     def npv(
         self,
         curves: Optional[Union[str, list, Curve]] = None,
         solver: Optional[Solver] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
         local: bool = False,
-    ):
+    ) -> DualTypes:
         """
         Return the NPV of the derivative.
 
         See :meth:`BaseDerivative.npv`.
-
-        Examples
-        --------
-        .. ipython:: python
-
-           fra.npv([forecasting_curve, discounting_curve])
-
-        .. ipython:: python
-
-           fxr = FXRates({"gbpusd": 2.0})
-           fra.npv([forecasting_curve, discounting_curve], None, fxr, "usd")
         """
+        if self.fixed_rate is None:
+            self._set_pricing_mid(curves, solver)
         curves, fx = _get_curves_and_fx_maybe_from_solver(
             self.curves, solver, curves, fx
         )
         fx, base = _get_fx_and_base(self.currency, fx, base)
         value = self.cashflow(curves[0]) * curves[1][self.payment]
         if local:
             return {self.currency: value}
@@ -4195,15 +5562,15 @@
 
     def rate(
         self,
         curves: Optional[Union[str, list, Curve]] = None,
         solver: Optional[Solver] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
-    ):
+    ) -> DualTypes:
         """
         Return the mid-market rate of the FRA.
 
         Only the forecasting curve is required to price an FRA.
 
         Parameters
         ----------
@@ -4218,20 +5585,14 @@
             constructs :class:`~rateslib.curves.Curve` from calibrating instruments.
         fx : unused
         base : unused
 
         Returns
         -------
         float, Dual or Dual2
-
-        Examples
-        --------
-        .. ipython:: python
-
-           fra.rate(forecasting_curve)
         """
         curves, _ = _get_curves_and_fx_maybe_from_solver(
             self.curves, solver, curves, fx
         )
         return self.leg2.rate(curves[0])
 
     def cashflow(self, curve: Union[Curve, LineCurve]):
@@ -4243,70 +5604,64 @@
         ----------
         curve : Curve or LineCurve,
             The forecasting curve for determining the floating rate.
 
         Returns
         -------
         float, Dual or Dual2
-
-        Examples
-        --------
-        .. ipython:: python
-
-           fra.cashflow(forecasting_curve)
         """
-        if self.fixed_rate is None:
-            return 0  # set the fixed rate = to floating rate netting to zero
-        rate = self.leg2.rate(curve)
-        cf = self.notional * self.leg1.dcf * (rate - self.fixed_rate) / 100
+        cf1 = self.leg1.cashflow
+        cf2 = self.leg2.cashflow(curve)
+        cf = cf1 + cf2
+        rate = None if curve is None else 100 * cf2 / (self.notional * self.leg2.dcf)
         cf /= 1 + self.leg1.dcf * rate / 100
+
+        # if self.fixed_rate is None:
+        #     return 0  # set the fixed rate = to floating rate netting to zero
+        # rate = self.leg2.rate(curve)
+        # cf = self.notional * self.leg1.dcf * (rate - self.fixed_rate) / 100
+        # cf /= 1 + self.leg1.dcf * rate / 100
         return cf
 
     def cashflows(
         self,
         curves: Optional[Union[str, list, Curve]] = None,
         solver: Optional[Solver] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
-    ):
+    ) -> DataFrame:
         """
         Return the properties of the leg used in calculating cashflows.
 
         Parameters
         ----------
         args :
             Positional arguments supplied to :meth:`~rateslib.periods.BasePeriod.cashflows`.
         kwargs :
             Keyword arguments supplied to :meth:`~rateslib.periods.BasePeriod.cashflows`.
 
         Returns
         -------
         DataFrame
-
-        Examples
-        --------
-        .. ipython:: python
-
-           fxr = FXRates({"gbpusd": 2.0})
-           fra.cashflows([forecasting_curve, discounting_curve], None, fxr, "usd")
         """
         curves, _ = _get_curves_and_fx_maybe_from_solver(
             self.curves, solver, curves, fx
         )
         fx, base = _get_fx_and_base(self.currency, fx, base)
         cf = float(self.cashflow(curves[0]))
         npv_local = self.cashflow(curves[0]) * curves[1][self.payment]
 
-        _spread = None if self.fixed_rate is None else -float(self.fixed_rate) * 100
+        _fix = None if self.fixed_rate is None else -float(self.fixed_rate)
+        _spd = None if curves[1] is None else -float(self.rate(curves[1])) * 100
         cfs = self.leg1.cashflows(curves[0], curves[1], fx, base)
         cfs[defaults.headers["type"]] = "FRA"
         cfs[defaults.headers["payment"]] = self.payment
         cfs[defaults.headers["cashflow"]] = cf
-        cfs[defaults.headers["rate"]] = float(self.rate(curves[1]))
-        cfs[defaults.headers["spread"]] = _spread
+        cfs[defaults.headers["rate"]] = _fix
+        cfs[defaults.headers["spread"]] = _spd
         cfs[defaults.headers["npv"]] = npv_local
         cfs[defaults.headers["fx"]] = float(fx)
         cfs[defaults.headers["npv_fx"]] = npv_local * float(fx)
         return DataFrame.from_records([cfs])
 
 
 ### Multi-currency derivatives
@@ -4408,14 +5763,66 @@
             self.leg2_notional = self.leg2.notional
         else:
             self.leg2_notional = self.leg1.notional * -fx_arg
             self.leg2.notional = self.leg2_notional
             self.leg2_amortization = self.leg1.amortization * -fx_arg
             self.leg2.amortization = self.leg2_amortization
 
+    @property
+    def _is_unpriced(self):
+        if getattr(self, "_unpriced", None) is True:
+            return True
+        if self._fixed_rate_mixin and self._leg2_fixed_rate_mixin:
+            # Fixed/Fixed where one leg is unpriced.
+            if self.fixed_rate is None or self.leg2_fixed_rate is None:
+                return True
+            return False
+        elif self._fixed_rate_mixin and self.fixed_rate is None:
+            # Fixed/Float where fixed leg is unpriced
+            return True
+        elif self._float_spread_mixin and self.float_spread is None:
+            # Float leg1 where leg1 is
+            pass  # goto 2)
+        else:
+            return False
+
+        # 2) leg1 is Float
+        if self._leg2_fixed_rate_mixin and self.leg2_fixed_rate is None:
+            return True
+        elif self._leg2_float_spread_mixin and self.leg2_float_spread is None:
+            return True
+        else:
+            return False
+
+    def _set_pricing_mid(
+        self,
+        curves: Optional[Union[Curve, str, list]] = None,
+        solver: Optional[Solver] = None,
+        fx: Optional[FXForwards] = None,
+    ):
+        leg: int = 1
+        lookup = {
+            1: ["_fixed_rate_mixin", "_float_spread_mixin"],
+            2: ["_leg2_fixed_rate_mixin", "_leg2_float_spread_mixin"],
+        }
+        if self._leg2_fixed_rate_mixin and self.leg2_fixed_rate is None:
+            # Fixed/Fixed or Float/Fixed
+            leg = 2
+
+        rate = self.rate(curves, solver, fx, leg=leg)
+        if getattr(self, lookup[leg][0]):
+            getattr(self, f"leg{leg}").fixed_rate = float(rate)
+        elif getattr(self, lookup[leg][1]):
+            getattr(self, f"leg{leg}").float_spread = float(rate)
+        else:
+            # this line should not be hit: internal code check
+            raise AttributeError(
+                "BaseXCS leg1 must be defined fixed or float."
+            )  # pragma: no cover
+
     def npv(
         self,
         curves: Optional[Union[Curve, str, list]] = None,
         solver: Optional[Solver] = None,
         fx: Optional[FXForwards] = None,
         base: Optional[str] = None,
         local: bool = False,
@@ -4430,28 +5837,22 @@
 
         See :meth:`BaseDerivative.npv`.
         """
         curves, fx = _get_curves_and_fx_maybe_from_solver(
             self.curves, solver, curves, fx
         )
         base = self.leg1.currency if base is None else base
+
+        if self._is_unpriced:
+            self._set_pricing_mid(curves, solver, fx)
+
         self._set_fx_fixings(fx)
         if self._is_mtm:
             self.leg2._do_not_repeat_set_periods = True
 
-        if "Fixed" in type(self.leg1).__name__ and self.fixed_rate is None:
-            mid_market_rate = self.rate(curves, solver, fx, leg=1)
-            self.leg1.fixed_rate = mid_market_rate
-        if "Fixed" in type(self.leg2).__name__ and self.leg2_fixed_rate is None:
-            if type(self).__name__ == "FXSwap":
-                mid_market_rate = self.rate(curves, solver, fx, fixed_rate=True)
-            else:
-                mid_market_rate = self.rate(curves, solver, fx, leg=2)
-            self.leg2.fixed_rate = mid_market_rate
-
         ret = super().npv(curves, solver, fx, base, local)
         if self._is_mtm:
             self.leg2._do_not_repeat_set_periods = False  # reset for next calculation
         return ret
 
     def rate(
         self,
@@ -4514,60 +5915,49 @@
         leg2 = 1 if leg == 2 else 2
         tgt_str, alt_str = "" if leg == 1 else "leg2_", "" if leg2 == 1 else "leg2_"
         tgt_leg, alt_leg = getattr(self, f"leg{leg}"), getattr(self, f"leg{leg2}")
         base = tgt_leg.currency
 
         _is_float_tgt_leg = "Float" in type(tgt_leg).__name__
         _is_float_alt_leg = "Float" in type(alt_leg).__name__
-        if not _is_float_alt_leg and getattr(self, f"{alt_str}fixed_rate") is None:
+        if not _is_float_alt_leg and getattr(alt_leg, f"fixed_rate") is None:
             raise ValueError(
                 "Cannot solve for a `fixed_rate` or `float_spread` where the "
                 "`fixed_rate` on the non-solvable leg is None."
             )
 
         # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
         # Commercial use of this code, and/or copying and redistribution is prohibited.
         # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
-        if tgt_leg._is_linear:
-            if not _is_float_tgt_leg and getattr(self, f"{tgt_str}fixed_rate") is None:
-                # set the target fixed leg to a null fixed rate for calculation
-                tgt_leg.fixed_rate = 0.0
-
-            self._set_fx_fixings(fx)
-            if self._is_mtm:
-                self.leg2._do_not_repeat_set_periods = True
-
-            tgt_leg_npv = tgt_leg.npv(tgt_fore_curve, tgt_disc_curve, fx, base)
-            alt_leg_npv = alt_leg.npv(alt_fore_curve, alt_disc_curve, fx, base)
-            fx_a_delta = 1.0 if not tgt_leg._is_mtm else fx
-            _ = tgt_leg._spread(
-                -(tgt_leg_npv + alt_leg_npv), tgt_fore_curve, tgt_disc_curve, fx_a_delta
-            )
-
-            specified_spd = 0.0
-            if _is_float_tgt_leg and not (
-                getattr(self, f"{tgt_str}float_spread") is None
-            ):
-                specified_spd = tgt_leg.float_spread
-            elif not _is_float_tgt_leg:
-                specified_spd = tgt_leg.fixed_rate * 100
-
-            _ += specified_spd
-
-            if self._is_mtm:
-                self.leg2._do_not_repeat_set_periods = False  # reset the mtm calc
-
-        else:
-            # need to set_order(2) for XCS.
-            # npv = self.npv(curves, solver, fx, leg_.currency)
-            raise NotImplementedError("Dual and Dual2 upcasting not complete.")
-            # the problem here is that spread requires Dual2 but fx_fixing
-            # calculates a Dual by default. Needs a manual overwrite.
-            # set_order(1) for XCS
+        if not _is_float_tgt_leg and getattr(tgt_leg, f"fixed_rate") is None:
+            # set the target fixed leg to a null fixed rate for calculation
+            tgt_leg.fixed_rate = 0.0
+
+        self._set_fx_fixings(fx)
+        if self._is_mtm:
+            self.leg2._do_not_repeat_set_periods = True
+
+        tgt_leg_npv = tgt_leg.npv(tgt_fore_curve, tgt_disc_curve, fx, base)
+        alt_leg_npv = alt_leg.npv(alt_fore_curve, alt_disc_curve, fx, base)
+        fx_a_delta = 1.0 if not tgt_leg._is_mtm else fx
+        _ = tgt_leg._spread(
+            -(tgt_leg_npv + alt_leg_npv), tgt_fore_curve, tgt_disc_curve, fx_a_delta
+        )
+
+        specified_spd = 0.0
+        if _is_float_tgt_leg and not (getattr(tgt_leg, f"float_spread") is None):
+            specified_spd = tgt_leg.float_spread
+        elif not _is_float_tgt_leg:
+            specified_spd = tgt_leg.fixed_rate * 100
+
+        _ += specified_spd
+
+        if self._is_mtm:
+            self.leg2._do_not_repeat_set_periods = False  # reset the mtm calc
 
         return _ if _is_float_tgt_leg else _ * 0.01
 
     def spread(self, *args, **kwargs):
         """
         Alias for :meth:`~rateslib.instruments.BaseXCS.rate`
         """
@@ -4731,14 +6121,23 @@
             notional=self.leg2_notional,
             currency=self.leg2_currency,
             amortization=self.leg2_amortization,
             convention=self.leg2_convention,
         )
         self._initialise_fx_fixings(fx_fixing)
 
+    # def _set_pricing_mid(
+    #     self,
+    #     curves: Optional[Union[Curve, str, list]] = None,
+    #     solver: Optional[Solver] = None,
+    #     fx: Optional[FXForwards] = None,
+    # ):
+    #     rate = self.rate(curves, solver, fx, leg=1)
+    #     self.leg1.float_spread = float(rate)
+
     def _rate2(
         self,
         curve_domestic: Curve,
         disc_curve_domestic: Curve,
         curve_foreign: Curve,
         disc_curve_foreign: Curve,
         fx_rate: Union[float, Dual],
@@ -5264,14 +6663,23 @@
             alt_currency=self.currency,
             alt_notional=-self.notional,
             fx_fixings=fx_fixings,
             amortization=self.leg2_amortization,
             convention=self.leg2_convention,
         )
 
+    # def _set_pricing_mid(
+    #     self,
+    #     curves: Optional[Union[Curve, str, list]] = None,
+    #     solver: Optional[Solver] = None,
+    #     fx: Optional[FXForwards] = None,
+    # ):
+    #     rate = self.rate(curves, solver, fx, leg=1)
+    #     self.leg1.float_spread = float(rate)
+
     def _npv2(
         self,
         curve_domestic: Curve,
         disc_curve_domestic: Curve,
         curve_foreign: Curve,
         disc_curve_foreign: Curve,
         fx_rate: Union[float, Dual],
@@ -5653,60 +7061,122 @@
             fx_fixings=fx_fixings,
             amortization=self.leg2_amortization,
             convention=self.leg2_convention,
         )
 
 
 class FXSwap(BaseXCS):
-    _fixed_rate_mixin = True
-    _leg2_fixed_rate_mixin = True
-
     """
-    Create n FX swap simulated via a :class:`NonMtmFixedFixedXCS`.
+    Create an FX swap simulated via a :class:`NonMtmFixedFixedXCS`.
 
     Parameters
     ----------
     args : dict
         Required positional args to :class:`BaseDerivative`.
     fx_fixing : float, FXForwards or None
         The initial FX fixing where leg 1 is considered the domestic currency. For
         example for an ESTR/SOFR XCS in 100mm EUR notional a value of 1.10 for `fx0`
         implies the notional on leg 2 is 110m USD. If `None` determines this
         dynamically.
+    points : float, optional
+        The pricing parameter for the FX Swap, which will determine the implicit
+        fixed rate on leg2.
     payment_lag_exchange : int
         The number of business days by which to delay notional exchanges, aligned with
-        the accrual schedule.
-    leg2_fixed_rate : float or None
-        The fixed rate applied to leg 2.
-        If `None` will be set to mid-market when curves are provided.
-        Must set the ``fixed_rate`` on at least one leg.
+        the accrual schedule. Defaults to 0 for *FXSwaps*.
     leg2_payment_lag_exchange : int
         The number of business days by which to delay notional exchanges, aligned with
-        the accrual schedule.
+        the accrual schedule. Defaults to 0 for *FXSwaps*.
     kwargs : dict
         Required keyword arguments to :class:`BaseDerivative`.
 
     Notes
     -----
-    TODO XXXXXXX
+    ``leg2_notional`` is determined by the ``fx_fixing`` either initialised or at price
+    time and the value of ``notional``. The argument value of ``leg2_notional`` does
+    not impact calculations.
+
+    .. note::
+
+       *FXSwaps* can be initialised either *priced* or *unpriced*. Priced derivatives
+       represent traded contracts with defined ``fx_fixing`` and ``points`` values.
+       This is usual for valuing *npv* against current market conditions. Unpriced
+       derivatives do not have a set ``fx_fixing`` nor ``points`` values. Any *rate*
+       calculation should return the mid-market rate and an *npv* of zero.
+
+    Examples
+    --------
+    To value the *FXSwap* we create *Curves* and :class:`~rateslib.fx.FXForwards`
+    objects.
+
+    .. ipython:: python
+
+       usd = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.95}, id="usd")
+       eur = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.97}, id="eur")
+       eurusd = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.971}, id="eurusd")
+       fxr = FXRates({"eurusd": 1.10}, settlement=dt(2022, 1, 3))
+       fxf = FXForwards(
+           fx_rates=fxr,
+           fx_curves={"usdusd": usd, "eureur": eur, "eurusd": eurusd},
+       )
+
+    Then we define the *FXSwap*. This in an unpriced instrument.
+
+    .. ipython:: python
+
+       fxs = FXSwap(
+           effective=dt(2022, 1, 17),
+           termination=dt(2022, 4, 19),
+           calendar="nyc",
+           currency="usd",
+           notional=1000000,
+           leg2_currency="eur",
+           curves=["usd", "usd", "eur", "eurusd"],
+       )
+
+    Now demonstrate the :meth:`~rateslib.instruments.FXSwap.npv` and
+    :meth:`~rateslib.instruments.FXSwap.rate` methods:
+
+    .. ipython:: python
+
+       fxs.npv(curves=[usd, usd, eur, eurusd], fx=fxf)
+       fxs.rate(curves=[usd, usd, eur, eurusd], fx=fxf)
+
+    In the case of *FXSwaps*, whose mid-market price is the difference between two
+    forward FX rates we can also derive this quantity using the independent
+    :meth:`FXForwards.swap<rateslib.fx.FXForwards.swap>` method. In this example
+    the numerical differences are caused by different calculation methods. The
+    difference here equates to a tolerance of 1e-8, or $1 per $100mm.
+
+    .. ipython:: python
+
+       fxf.swap("usdeur", [dt(2022, 1, 17), dt(2022, 4, 19)])
+
     """
 
+    _fixed_rate_mixin = True
+    _leg2_fixed_rate_mixin = True
+    _unpriced = True
+
     def __init__(
         self,
         *args,
         fx_fixing: Optional[Union[float, FXRates, FXForwards]] = None,
+        points: Optional[float] = None,
         payment_lag_exchange: Optional[int] = None,
-        leg2_fixed_rate: Optional[float] = None,
         leg2_payment_lag_exchange: Optional[int] = "inherit",
         **kwargs,
     ):
+        if fx_fixing is None and points is not None:
+            raise ValueError(
+                "Cannot set `points` on FXSwap without giving an `fx_fixing`."
+            )
         super().__init__(*args, **kwargs)
         if leg2_payment_lag_exchange == "inherit":
             leg2_payment_lag_exchange = payment_lag_exchange
-        self._leg2_fixed_rate = leg2_fixed_rate
         self._fixed_rate = 0.0
         self.leg1 = FixedLegExchange(
             fixed_rate=0.0,
             effective=self.effective,
             termination=self.termination,
             frequency="Z",
             modifier=self.modifier,
@@ -5714,32 +7184,61 @@
             payment_lag=payment_lag_exchange,
             payment_lag_exchange=payment_lag_exchange,
             notional=self.notional,
             currency=self.currency,
             convention=self.convention,
         )
         self.leg2 = FixedLegExchange(
-            fixed_rate=leg2_fixed_rate,
+            fixed_rate=None,
             effective=self.leg2_effective,
             termination=self.leg2_termination,
             frequency="Z",
             modifier=self.leg2_modifier,
             calendar=self.leg2_calendar,
             payment_lag=leg2_payment_lag_exchange,
             payment_lag_exchange=leg2_payment_lag_exchange,
             notional=self.leg2_notional,
             currency=self.leg2_currency,
             convention=self.leg2_convention,
         )
         self._initialise_fx_fixings(fx_fixing)
+        self.points = points
+
+    @property
+    def points(self):
+        return self._points
+
+    @points.setter
+    def points(self, value):
+        self._unpriced = False
+        self._points = value
+        self._leg2_fixed_rate = None
+        if value is not None:
+            fixed_rate = (
+                value
+                * -self.notional
+                / (self.leg2.periods[1].dcf * 100 * self.leg2.periods[1].notional)
+            )
+            self.leg2_fixed_rate = fixed_rate
+
+        # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 
-    # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
     # Commercial use of this code, and/or copying and redistribution is prohibited.
     # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
+    def _set_pricing_mid(
+        self,
+        curves: Optional[Union[Curve, str, list]] = None,
+        solver: Optional[Solver] = None,
+        fx: Optional[FXForwards] = None,
+    ):
+        points = self.rate(curves, solver, fx)
+        self.points = points
+        self._unpriced = True  # setting pricing mid does not define a priced instrument
+
     def rate(
         self,
         curves: Union[Curve, str, list],
         solver: Optional[Solver] = None,
         fx: Optional[FXForwards] = None,
         fixed_rate: bool = False,
     ):
@@ -5758,41 +7257,29 @@
         solver : Solver, optional
             The numerical :class:`~rateslib.solver.Solver` that
             constructs :class:`~rateslib.curves.Curve` from calibrating instruments.
         fx : FXForwards, optional
             The FX forwards object that is used to determine the initial FX fixing for
             determining ``leg2_notional``, if not specified at initialisation, and for
             determining mark-to-market exchanges on mtm XCSs.
+        fixed_rate : bool
+            Whether to return the fixed rate for the leg or the FX swap points price.
 
         Returns
         -------
         float, Dual or Dual2
-
-        Notes
-        -----
-        Fixed legs have pricing parameter returned in percentage terms, and
-        float legs have pricing parameter returned in basis point (bp) terms.
-
-        If the ``XCS`` type is specified without a ``fixed_rate`` on any leg then an
-        implied ``float_spread`` will return as its originaly value or zero since
-        the fixed rate used
-        for calculation is the implied mid-market rate including the
-        current ``float_spread`` parameter.
-
-        Examples
-        --------
         """
         leg2_fixed_rate = super().rate(curves, solver, fx, leg=2)
         if fixed_rate:
             return leg2_fixed_rate
         cf = self.leg2.notional * leg2_fixed_rate * 0.01 * self.leg2.periods[1].dcf
         # fwd_fx = (cf + self.leg2.notional) / -self.leg1.notional
         # ini_fx = self.leg2.notional / -self.leg1.notional
         ## TODO decide how to price mid-market rates when ini fx is struck but
-        ## there is no fixed points, i,e the FXswap is sem-determined, which is
+        ## there is no fixed points, i,e the FXswap is semi-determined, which is
         ## not a real instrument.
         return (cf / -self.leg1.notional) * 10000
 
 
 ### Generic Instruments
 
 
@@ -5863,14 +7350,21 @@
         kwargs :
             Keyword arguments required for the ``npv`` method of both of the underlying
             ``Instruments``.
 
         Returns
         -------
         float, Dual or Dual2
+
+        Notes
+        -----
+
+        If the argument ``local`` is added to return a dict of currencies, ensure
+        that this is added as a **keyword** argument and not a positional argument.
+        I.e. use `local=True`.
         """
         leg1_npv = self.instrument1.npv(*args, **kwargs)
         leg2_npv = self.instrument2.npv(*args, **kwargs)
         if kwargs.get("local", False):
             return {
                 k: leg1_npv.get(k, 0) + leg2_npv.get(k, 0)
                 for k in set(leg1_npv) | set(leg2_npv)
@@ -5984,16 +7478,16 @@
         float, Dual or Dual2
         """
         leg1_npv = self.instrument1.npv(*args, **kwargs)
         leg2_npv = self.instrument2.npv(*args, **kwargs)
         leg3_npv = self.instrument3.npv(*args, **kwargs)
         if kwargs.get("local", False):
             return {
-                k: leg1_npv.get(k, 0) + leg2_npv.get(k, 0)
-                for k in set(leg1_npv) | set(leg2_npv)
+                k: leg1_npv.get(k, 0) + leg2_npv.get(k, 0) + leg3_npv.get(k, 0)
+                for k in set(leg1_npv) | set(leg2_npv) | set(leg3_npv)
             }
         else:
             return leg1_npv + leg2_npv + leg3_npv
 
     def rate(self, *args, **kwargs):
         """
         Return the mid-market rate of the composited via the difference of instrument
@@ -6056,35 +7550,69 @@
 #         else:
 #             args1 = args
 #             args2 = args
 #             args3 = args
 #         return 2 * self.instrument2.rate(*args2) - self.instrument1.rate(*args1) - self.instrument3.rate(*args3)
 
 
+def _instrument_npv(instrument, *args, **kwargs):
+    return instrument.npv(*args, **kwargs)
+
+
 class Portfolio(Sensitivities):
+    # TODO document portfolio
+
     def __init__(self, instruments):
         self.instruments = instruments
 
     def npv(self, *args, **kwargs):
         # TODO do not permit a mixing of currencies.
         # TODO look at legs.npv where args len is used.
+
+        if defaults.pool == 1:
+            return self._npv_single_core(*args, **kwargs)
+
+        from multiprocessing import Pool
+        from functools import partial
+        func = partial(_instrument_npv, *args, **kwargs)
+        p = Pool(defaults.pool)
+        results = p.map(func, self.instruments)
+
+        if kwargs.get("local", False):
+            _ = DataFrame(results).fillna(0.0)
+            _ = _.sum()
+            ret = _.to_dict()
+
+            # ret = {}
+            # for result in results:
+            #     for ccy in result:
+            #         if ccy in ret:
+            #             ret[ccy] += result[ccy]
+            #         else:
+            #             ret[ccy] = result[ccy]
+
+        else:
+            ret = sum(results)
+
+        return ret
+
+    def _npv_single_core(self, *args, **kwargs):
         if kwargs.get("local", False):
             ret = {}
             for instrument in self.instruments:
                 i_npv = instrument.npv(*args, **kwargs)
                 for ccy in i_npv:
                     if ccy in ret:
                         ret[ccy] += i_npv[ccy]
                     else:
                         ret[ccy] = i_npv[ccy]
         else:
             ret = 0
             for instrument in self.instruments:
                 ret += instrument.npv(*args, **kwargs)
-
         return ret
 
 
 def forward_fx(
     date: datetime,
     curve_domestic: Curve,
     curve_foreign: Curve,
@@ -6255,17 +7783,18 @@
     _A = np.array([[f0**2, f0, 1], [f1**2, f1, 1], [f2**2, f2, 1]])
     c = np.linalg.solve(_A, _b)
     y = c[2, 0]
     f_ = f(y)
 
     pad = min(tol * 1e8, 0.0001, abs(f_ * 1e4))  # avoids singular matrix error
     if y <= y0:
+        # line not hit due to reassessment of initial vars?
         return _ytm_quadratic_converger2(
             f, 2 * y - y0 - pad, y, y0 + pad, None, f_, None, tol
-        )
+        )  # pragma: no cover
     elif y0 < y <= y1:
         if (y - y0) < (y1 - y):
             return _ytm_quadratic_converger2(
                 f, y0 - pad, y, 2 * y - y0 + pad, None, f_, None, tol
             )
         else:
             return _ytm_quadratic_converger2(
@@ -6277,68 +7806,77 @@
                 f, y1 - pad, y, 2 * y - y1 + pad, None, f_, None, tol
             )
         else:
             return _ytm_quadratic_converger2(
                 f, 2 * y - y2 - pad, y, y2 + pad, None, f_, None, tol
             )
     else:  # y2 < y:
+        # line not hit due to reassessmemt of initial vars?
         return _ytm_quadratic_converger2(
             f, y2 - pad, y, 2 * y - y2 + pad, None, f_, None, tol
+        )  # pragma: no cover
+
+
+def _brents(f, x0, x1, max_iter=50, tolerance=1e-9):  # pragma: no cover
+    """
+    Alternative yield converger as an alternative to ytm_converger
+
+    Unused currently within the library
+    """
+    fx0 = f(x0)
+    fx1 = f(x1)
+
+    if float(fx0 * fx1) > 0:
+        raise ValueError(
+            "`brents` must initiate from function values with opposite signs."
         )
 
+    if abs(fx0) < abs(fx1):
+        x0, x1 = x1, x0
+        fx0, fx1 = fx1, fx0
 
-# def _brents(f, x0, x1, max_iter=50, tolerance=1e-9):
-#     fx0 = f(x0)
-#     fx1 = f(x1)
-#
-#     if float(fx0 * fx1) > 0:
-#         raise ValueError(
-#             "`brents` must initiate from function values with opposite signs.")
-#
-#     if abs(fx0) < abs(fx1):
-#         x0, x1 = x1, x0
-#         fx0, fx1 = fx1, fx0
-#
-#     x2, fx2 = x0, fx0
-#
-#     mflag = True
-#     steps_taken = 0
-#
-#     while steps_taken < max_iter and abs(x1 - x0) > tolerance:
-#         fx0 = f(x0)
-#         fx1 = f(x1)
-#         fx2 = f(x2)
-#
-#         if fx0 != fx2 and fx1 != fx2:
-#             L0 = (x0 * fx1 * fx2) / ((fx0 - fx1) * (fx0 - fx2))
-#             L1 = (x1 * fx0 * fx2) / ((fx1 - fx0) * (fx1 - fx2))
-#             L2 = (x2 * fx1 * fx0) / ((fx2 - fx0) * (fx2 - fx1))
-#             new = L0 + L1 + L2
-#
-#         else:
-#             new = x1 - ((fx1 * (x1 - x0)) / (fx1 - fx0))
-#
-#         if ((float(new) < float((3 * x0 + x1) / 4) or float(new) > float(x1)) or
-#                 (mflag == True and (abs(new - x1)) >= (abs(x1 - x2) / 2)) or
-#                 (mflag == False and (abs(new - x1)) >= (abs(x2 - d) / 2)) or
-#                 (mflag == True and (abs(x1 - x2)) < tolerance) or
-#                 (mflag == False and (abs(x2 - d)) < tolerance)):
-#             new = (x0 + x1) / 2
-#             mflag = True
-#
-#         else:
-#             mflag = False
-#
-#         fnew = f(new)
-#         d, x2 = x2, x1
-#
-#         if float(fx0 * fnew) < 0:
-#             x1 = new
-#         else:
-#             x0 = new
-#
-#         if abs(fx0) < abs(fx1):
-#             x0, x1 = x1, x0
-#
-#         steps_taken += 1
-#
-#     return x1, steps_taken
+    x2, fx2 = x0, fx0
+
+    mflag = True
+    steps_taken = 0
+
+    while steps_taken < max_iter and abs(x1 - x0) > tolerance:
+        fx0 = f(x0)
+        fx1 = f(x1)
+        fx2 = f(x2)
+
+        if fx0 != fx2 and fx1 != fx2:
+            L0 = (x0 * fx1 * fx2) / ((fx0 - fx1) * (fx0 - fx2))
+            L1 = (x1 * fx0 * fx2) / ((fx1 - fx0) * (fx1 - fx2))
+            L2 = (x2 * fx1 * fx0) / ((fx2 - fx0) * (fx2 - fx1))
+            new = L0 + L1 + L2
+
+        else:
+            new = x1 - ((fx1 * (x1 - x0)) / (fx1 - fx0))
+
+        if (
+            (float(new) < float((3 * x0 + x1) / 4) or float(new) > float(x1))
+            or (mflag == True and (abs(new - x1)) >= (abs(x1 - x2) / 2))
+            or (mflag == False and (abs(new - x1)) >= (abs(x2 - d) / 2))
+            or (mflag == True and (abs(x1 - x2)) < tolerance)
+            or (mflag == False and (abs(x2 - d)) < tolerance)
+        ):
+            new = (x0 + x1) / 2
+            mflag = True
+
+        else:
+            mflag = False
+
+        fnew = f(new)
+        d, x2 = x2, x1
+
+        if float(fx0 * fnew) < 0:
+            x1 = new
+        else:
+            x0 = new
+
+        if abs(fx0) < abs(fx1):
+            x0, x1 = x1, x0
+
+        steps_taken += 1
+
+    return x1, steps_taken
```

### Comparing `rateslib-0.2.0/rateslib/legs.py` & `rateslib-0.3.0/rateslib/legs.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,25 +27,26 @@
 import pandas as pd
 from pandas.tseries.offsets import CustomBusinessDay
 from pandas import DataFrame, Series
 
 from rateslib import defaults
 from rateslib.calendars import add_tenor
 from rateslib.scheduling import Schedule
-from rateslib.curves import Curve
+from rateslib.curves import Curve, IndexCurve
 from rateslib.periods import (
     IndexFixedPeriod,
     FixedPeriod,
     FloatPeriod,
     Cashflow,
     IndexCashflow,
+    IndexMixin,
     _validate_float_args,
     _get_fx_and_base,
 )
-from rateslib.dual import Dual, Dual2, set_order
+from rateslib.dual import Dual, Dual2, set_order, DualTypes
 from rateslib.fx import FXForwards, FXRates
 
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
@@ -109,14 +110,18 @@
     convention : str
     periods : list
 
     See Also
     --------
     FixedLeg : Create a fixed leg composed of :class:`~rateslib.periods.FixedPeriod` s.
     FloatLeg : Create a floating leg composed of :class:`~rateslib.periods.FloatPeriod` s.
+    IndexFixedLeg : Create a fixed leg composed of :class:`~rateslib.periods.IndexFixedPeriod` s.
+    ZeroFixedLeg : Create a zero coupon leg composed of a :class:`~rateslib.periods.FixedPeriod`.
+    ZeroFloatLeg : Create a zero coupon leg composed of a :class:`~rateslib.periods.FloatPeriod` s.
+    ZeroIndexLeg : Create a zero coupon leg composed of :class:`~rateslib.periods.IndexFixedPeriod`.
     BaseLegExchange : Abstract base class for ``Legs`` with notional exchanges.
     CustomLeg : Create a leg composed of user specified periods.
     """
 
     @abc.abstractmethod
     def __init__(
         self,
@@ -159,69 +164,40 @@
             self._amortization = 0 if amortization is None else amortization
         else:
             self.amortization = 0 if amortization is None else amortization
         self.periods = []
 
     def analytic_delta(self, *args, **kwargs):
         """
-        Return the analytic delta of the leg object via summing all periods.
+        Return the analytic delta of the *Leg* via summing all periods.
 
-        Parameters
-        ----------
-        args :
-            Positional arguments supplied to
-            :meth:`BasePeriod.analytic_delta()<rateslib.periods.BasePeriod.analytic_delta>`.
-        kwargs :
-            Keyword arguments supplied to
-            :meth:`BasePeriod.analytic_delta()<rateslib.periods.BasePeriod.analytic_delta>`.
-
-        Returns
-        -------
-        float, Dual, Dual2
+        For arguments see
+        :meth:`BasePeriod.analytic_delta()<rateslib.periods.BasePeriod.analytic_delta>`.
         """
         sum = 0
         for period in self.periods:
             sum += period.analytic_delta(*args, **kwargs)
         return sum
 
-    def cashflows(self, *args, **kwargs):
+    def cashflows(self, *args, **kwargs) -> DataFrame:
         """
-        Return the properties of the leg used in calculating cashflows.
+        Return the properties of the *Leg* used in calculating cashflows.
 
-        Parameters
-        ----------
-        args :
-            Positional arguments supplied to :meth:`~rateslib.periods.BasePeriod.cashflows`.
-        kwargs :
-            Keyword arguments supplied to :meth:`~rateslib.periods.BasePeriod.cashflows`.
-
-        Returns
-        -------
-        DataFrame
+        For arguments see
+        :meth:`BasePeriod.cashflows()<rateslib.periods.BasePeriod.cashflows>`.
         """
         seq = [period.cashflows(*args, **kwargs) for period in self.periods]
         return DataFrame.from_records(seq)
 
     def npv(self, *args, **kwargs):
         """
-        Return the NPV of the leg object via summing all periods.
-
-        Calculates the cashflow for the all periods and multiplies them by the
-        DF associated with each payment date.
-
-        Parameters
-        ----------
-        args :
-            Positional arguments supplied to :meth:`~rateslib.periods.BasePeriod.npv`.
-        kwargs :
-            Keyword arguments supplied to :meth:`~rateslib.periods.BasePeriod.npv`.
+        Return the NPV of the *Leg* via summing all periods.
 
-        Returns
-        -------
-        Dual
+        For arguments see
+        :meth:`BasePeriod.npv()<rateslib.periods.BasePeriod.npv>`.
         """
         sum = 0
         _is_local = (len(args) == 5 and args[4]) or kwargs.get("local", False)
         if _is_local:
             for period in self.periods:
                 sum += period.npv(*args, **kwargs)[self.currency]
             return {self.currency: sum}
@@ -247,14 +223,109 @@
             if (
                 "rfr" in self.fixing_method
                 and self.spread_compound_method != "none_simple"
             ):
                 return False
         return True
 
+    def _spread_isda_approximated_rate(self, target_npv, fore_curve, disc_curve):
+        """
+        Use approximated derivatives through geometric averaged 1day rates to derive the
+        spread
+        """
+        a, b = 0.0, 0.0
+        for period in self.periods:
+            try:
+                a_, b_ = period._get_analytic_delta_quadratic_coeffs(
+                    fore_curve, disc_curve
+                )
+                a += a_
+                b += b_
+            except AttributeError:
+                pass
+        c = -target_npv
+
+        # perform the quadratic solution
+        _1 = -c / b
+        if abs(a) > 1e-14:
+            _2a = (-b - (b**2 - 4 * a * c) ** 0.5) / (2 * a)
+            _2b = (-b + (b**2 - 4 * a * c) ** 0.5) / (2 * a)  # alt quadratic soln
+            if abs(_1 - _2a) < abs(_1 - _2b):
+                _ = _2a
+            else:
+                _ = _2b  # select quadratic soln
+        else:
+            # this is to avoid divide by zero errors and return an approximation
+            # also isda_flat_compounding has a=0
+            _ = _1
+
+        return _
+
+    def _spread_isda_dual2(
+        self, target_npv, fore_curve, disc_curve, fx=None
+    ):  # pragma: no cover
+        # This method is unused and untested, superseded by _spread_isda_approx_rate
+
+        # This method creates a dual2 variable for float spread and obtains derivatives automatically
+        _fs = self.float_spread
+        self.float_spread = Dual2(0.0 if _fs is None else float(_fs), "spread_z")
+
+        # This method uses ad-hoc AD to solve a specific problem for which
+        # there is no closed form solution. Calculating NPV is very inefficient
+        # so, we only do this once as opposed to using a root solver algo
+        # which would otherwise converge to the exact solution but is
+        # practically not workable.
+
+        # This method is more accurate than the 'spread through approximated
+        # derivatives' method, but it is a more costly and less robust method
+        # due to its need to work in second order mode.
+
+        fore_ad = fore_curve.ad
+        fore_curve._set_ad_order(2)
+
+        disc_ad = disc_curve.ad
+        disc_curve._set_ad_order(2)
+
+        if isinstance(fx, (FXRates, FXForwards)):
+            _fx = None if fx is None else fx._ad
+            fx._set_ad_order(2)
+
+        npv = self.npv(fore_curve, disc_curve, fx, self.currency)
+        b = npv.gradient("spread_z", order=1)[0]
+        a = 0.5 * npv.gradient("spread_z", order=2)[0][0]
+        c = -target_npv
+
+        # Perform quadratic solution
+        _1 = -c / b
+        if abs(a) > 1e-14:
+            _2a = (-b - (b**2 - 4 * a * c) ** 0.5) / (2 * a)
+            _2b = (-b + (b**2 - 4 * a * c) ** 0.5) / (2 * a)  # alt quadratic soln
+            if abs(_1 - _2a) < abs(_1 - _2b):
+                _ = _2a
+            else:
+                _ = _2b  # select quadratic soln
+        else:  # pragma: no cover
+            # this is to avoid divide by zero errors and return an approximation
+            _ = _1
+            warnings.warn(
+                "Divide by zero encountered and the spread is approximated to "
+                "first order.",
+                UserWarning,
+            )
+
+        # This is required by the Dual2 AD approach to revert to original order.
+        self.float_spread = _fs
+        fore_curve._set_ad_order(fore_ad)
+        disc_curve._set_ad_order(disc_ad)
+        if isinstance(fx, (FXRates, FXForwards)):
+            fx._set_ad_order(_fx)
+        _ = set_order(_, disc_ad)  # use disc_ad: credit spread from disc curve
+
+        return _
+
     def _spread(self, target_npv, fore_curve, disc_curve, fx=None):
         """
         Calculates an adjustment to the ``fixed_rate`` or ``float_spread`` to match
         a specific target NPV.
 
         Parameters
         ----------
@@ -288,62 +359,17 @@
         Examples
         --------
         """
         if self._is_linear:
             a_delta = self.analytic_delta(fore_curve, disc_curve, fx, self.currency)
             return -target_npv / a_delta
         else:
-            # This method creates a dual2 variable for float spread.
-            _fs = self.float_spread
-            self.float_spread = Dual2(0.0 if _fs is None else float(_fs), "spread_z")
-
-            # This method uses ad-hoc AD to solve a specific problem for which
-            # there is no closed form solution. Calculating NPV is very inefficient
-            # so, we only do this once as opposed to using a root solver algo
-            # which would otherwise converge to the exact solution but is
-            # practically not workable.
-
-            fore_ad = fore_curve.ad
-            fore_curve._set_ad_order(2)
-
-            disc_ad = disc_curve.ad
-            disc_curve._set_ad_order(2)
-
-            if isinstance(fx, (FXRates, FXForwards)):
-                _fx = None if fx is None else fx._ad
-                fx._set_ad_order(2)
-
-            npv = self.npv(fore_curve, disc_curve, fx, self.currency)
-            b = npv.gradient("spread_z", order=1)[0]
-            a = 0.5 * npv.gradient("spread_z", order=2)[0][0]
-            c = -target_npv
-
-            _1 = -c / b
-            if abs(a) > 1e-14:
-                _2a = (-b - (b**2 - 4 * a * c) ** 0.5) / (2 * a)
-                _2b = (-b + (b**2 - 4 * a * c) ** 0.5) / (2 * a)  # alt quadratic soln
-                if abs(_1 - _2a) < abs(_1 - _2b):
-                    _ = _2a
-                else:
-                    _ = _2b  # select quadratic soln
-            else:  # pragma: no cover
-                # this is to avoid divide by zero errors and return an approximation
-                _ = _1
-                warnings.warn(
-                    "Divide by zero encountered and the spread is approximated to "
-                    "first order.",
-                    UserWarning,
-                )
-
-            self.float_spread = _fs
-            fore_curve._set_ad_order(fore_ad)
-            disc_curve._set_ad_order(disc_ad)
-            if isinstance(fx, (FXRates, FXForwards)):
-                fx._set_ad_order(_fx)
-            return set_order(_, disc_ad)  # use disc_ad: credit spread from disc curve
+            _ = self._spread_isda_approximated_rate(target_npv, fore_curve, disc_curve)
+            # _ = self._spread_isda_dual2(target_npv, fore_curve, disc_curve, fx)
+            return _
 
 
 class FixedLegMixin:
     """
     Add the functionality to add and retrieve ``fixed_rate`` on
     :class:`~rateslib.periods.FixedPeriod` s.
     """
@@ -367,21 +393,36 @@
 
 class FixedLeg(BaseLeg, FixedLegMixin):
     """
     Create a fixed leg composed of :class:`~rateslib.periods.FixedPeriod` s.
 
     Parameters
     ----------
-    args : dict
+    args : tuple
         Required positional args to :class:`BaseLeg`.
     fixed_rate : float, optional
         The rate applied to determine cashflows. Can be set to `None` and designated
         later, perhaps after a mid-market rate for all periods has been calculated.
     kwargs : dict
         Required keyword arguments to :class:`BaseLeg`.
+
+    Notes
+    -----
+    The NPV of a fixed leg is the sum of the period NPVs.
+
+    .. math::
+
+       P = - R \\sum_{i=1}^n {N_i d_i v_i(m_i)}
+
+    The analytic delta is the sum of the period analytic deltas.
+
+    .. math::
+
+       A = -\\frac{\\partial P}{\\partial R} = \\sum_{i=1}^n {N_i d_i v_i(m_i)}
+
     """
 
     def __init__(self, *args, fixed_rate: Optional[float] = None, **kwargs):
         self._fixed_rate = fixed_rate
         super().__init__(*args, **kwargs)
         self.periods = [
             FixedPeriod(
@@ -395,14 +436,41 @@
                 termination=self.schedule.termination,
                 frequency=self.schedule.frequency,
                 stub=True if period[defaults.headers["stub_type"]] == "Stub" else False,
             )
             for i, period in self.schedule.table.to_dict(orient="index").items()
         ]
 
+    def analytic_delta(self, *args, **kwargs):
+        """
+        Return the analytic delta of the *FixedLeg* via summing all periods.
+
+        For arguments see
+        :meth:`BasePeriod.analytic_delta()<rateslib.periods.BasePeriod.analytic_delta>`.
+        """
+        return super().analytic_delta(*args, **kwargs)
+
+    def cashflows(self, *args, **kwargs) -> DataFrame:
+        """
+        Return the properties of the *FixedLeg* used in calculating cashflows.
+
+        For arguments see
+        :meth:`BasePeriod.cashflows()<rateslib.periods.BasePeriod.cashflows>`.
+        """
+        return super().cashflows(*args, **kwargs)
+
+    def npv(self, *args, **kwargs):
+        """
+        Return the NPV of the *FixedLeg* via summing all periods.
+
+        For arguments see
+        :meth:`BasePeriod.npv()<rateslib.periods.BasePeriod.npv>`.
+        """
+        return super().npv(*args, **kwargs)
+
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
 
 class FloatLegMixin:
@@ -484,51 +552,44 @@
     #     all RFR calculations.
     #     """
     #     df = self.periods[0].fixings_table(curve)
     #     for i in range(1, self.schedule.n_periods):
     #         df = pd.concat([df, self.periods[i].fixings_table(curve)])
     #     return df
 
-    def fixings_table(self, curve: Curve):
+    def _fixings_table(self, *args, **kwargs):
         """
         Return a DataFrame of fixing exposures on a :class:`~rateslib.legs.FloatLeg`.
 
-        See :meth:`~rateslib.periods.FloatPeriod.fixings_table` for more info.
-
-        Parameters
-        ----------
-        curve : Curve
-            The forecast :class:`~rateslib.curves.Curve` or
-            :class:`~rateslib.curves.LineCurve` needed to calculate rates which
-            affect compounding and dependent notional exposure.
+        See :meth:`~rateslib.periods.FloatPeriod.fixings_table` for arguments.
 
         Returns
         -------
         DataFrame
         """
         df, _ = None, 0
         while df is None:
             if type(self.periods[_]) is FloatPeriod:
-                df = self.periods[_].fixings_table(curve)
+                df = self.periods[_].fixings_table(*args, **kwargs)
             _ += 1
 
         n = len(self.periods)
         for _ in range(_, n):
             if type(self.periods[_]) is FloatPeriod:
-                df = pd.concat([df, self.periods[_].fixings_table(curve)])
+                df = pd.concat([df, self.periods[_].fixings_table(*args, **kwargs)])
         return df
 
 
 class FloatLeg(BaseLeg, FloatLegMixin):
     """
     Create a floating leg composed of :class:`~rateslib.periods.FloatPeriod` s.
 
     Parameters
     ----------
-    args : dict
+    args : tuple
         Required positional args to :class:`BaseLeg`.
     float_spread : float, optional
         The spread applied to determine cashflows. Can be set to `None` and designated
         later, perhaps after a mid-market spread for all periods has been calculated.
     spread_compound_method : str, optional
         The method to use for adding a floating spread to compounded rates. Available
         options are `{"none_simple", "isda_compounding", "isda_flat_compounding"}`.
@@ -544,22 +605,38 @@
     method_param : int, optional
         A parameter that is used for the various ``fixing_method`` s. See notes.
     kwargs : dict
         Required keyword arguments to :class:`BaseLeg`.
 
     Notes
     -----
-    ... warn::
+    The NPV of a *FloatLeg* is the sum of the period NPVs.
+
+    .. math::
+
+       P = - \\sum_{i=1}^n {N_i r_i(r_j, z) d_i v_i(m_i)}
+
+    The analytic delta is the sum of the period analytic deltas.
+
+    .. math::
+
+       A = -\\frac{\\partial P}{\\partial z} = \\sum_{i=1}^n {\\frac{\\partial r_i}{\\partial z} N_i d_i v_i(m_i)}
+
+
+    .. warning::
+
+       When floating rates are determined from historical fixings the forecast
+       ``Curve`` ``calendar`` will be used to determine fixing dates.
+       If this calendar does not align with the ``Leg`` ``calendar`` then
+       spurious results or errors may be generated.
 
-        When floating rates are determined from historical fixings the forecast
-        ``Curve`` ``calendar`` will be used to determine fixing dates.
-        If this calendar does not align with the leg ``calendar`` then
-        spurious results or errors may be generated. Including the curve calendar in
-        the leg is acceptable, i.e. a leg calendar of *"nyc,ldn,tgt"* and a curve
-        calendar of *"ldn"* is valid, whereas only *"nyc,tgt"* may give errors.
+       Including the curve calendar within a *Leg* multi-holiday calendar
+       is acceptable, i.e. a *Leg* calendar of *"nyc,ldn,tgt"* and a curve
+       calendar of *"ldn"* is valid. A *Leg* calendar of just *"nyc,tgt"* may
+       give errors.
 
     Examples
     --------
     Set the first fixing on an historic IBOR leg.
 
     .. ipython:: python
 
@@ -582,15 +659,15 @@
            frequency="Q",
            fixing_method="ibor",
            fixings=[1.00, 2.00],
        )
        float_leg.cashflows(curve)
 
     Set the initial RFR fixings in the first period of an RFR leg (notice the sublist
-    and the implied -10% year end turn).
+    and the implied -10% year end turn spread).
 
     .. ipython:: python
 
        float_leg = FloatLeg(
            effective=dt(2022, 12, 28),
            termination="2M",
            frequency="M",
@@ -637,14 +714,50 @@
                 fixings=self.fixings[i],
                 method_param=self.method_param,
                 spread_compound_method=self.spread_compound_method,
             )
             for i, period in self.schedule.table.to_dict(orient="index").items()
         ]
 
+    def analytic_delta(self, *args, **kwargs):
+        """
+        Return the analytic delta of the *FloatLeg* via summing all periods.
+
+        For arguments see
+        :meth:`BasePeriod.analytic_delta()<rateslib.periods.BasePeriod.analytic_delta>`.
+        """
+        return super().analytic_delta(*args, **kwargs)
+
+    def cashflows(self, *args, **kwargs) -> DataFrame:
+        """
+        Return the properties of the *FloatLeg* used in calculating cashflows.
+
+        For arguments see
+        :meth:`BasePeriod.cashflows()<rateslib.periods.BasePeriod.cashflows>`.
+        """
+        return super().cashflows(*args, **kwargs)
+
+    def npv(self, *args, **kwargs):
+        """
+        Return the NPV of the *FloatLeg* via summing all periods.
+
+        For arguments see
+        :meth:`BasePeriod.npv()<rateslib.periods.BasePeriod.npv>`.
+        """
+        return super().npv(*args, **kwargs)
+
+    def fixings_table(self, *args, **kwargs) -> DataFrame:
+        """
+        Return a DataFrame of fixing exposures on a :class:`~rateslib.legs.FloatLeg`.
+
+        For arguments see
+        :meth:`FloatPeriod.fixings_table()<rateslib.periods.FloatPeriod.fixings_table>`.
+        """
+        return super()._fixings_table(*args, **kwargs)
+
     # @property
     # def _is_complex(self):
     #     """
     #     A complex float leg is one which is RFR based and for which each individual
     #     RFR fixing is required is order to calculate correctly. This occurs in the
     #     following cases:
     #
@@ -670,14 +783,206 @@
     #         else:
     #             return True
     #     elif self.fixing_method == "ibor":
     #         return False
     #     return True
 
 
+class IndexLegMixin:
+    schedule = None
+    index_method = None
+    _index_fixings = None
+    _index_base = None
+
+    # def _set_index_fixings_on_periods(self):
+    #     """
+    #     Re-organises the fixings input to list structure for each period.
+    #     Requires a ``schedule`` object and ``float_args``.
+    #     """
+    #     if self.index_fixings is None:
+    #         pass  # do nothing
+    #     elif isinstance(self.index_fixings, Series):
+    #         for period in self.periods:
+    #             period.index_fixings = IndexMixin._index_value(
+    #                 i_method=self.index_method,
+    #                 i_lag=self.index_lag,
+    #                 i_curve=None,
+    #                 i_date=period.end,
+    #                 i_fixings=self.index_fixings,
+    #             )
+    #     elif isinstance(self.index_fixings, list):
+    #         for i in range(len(self.index_fixings)):
+    #             self.periods[i].index_fixings = self.index_fixings[i]
+    #     else:  # index_fixings is float
+    #         if type(self) is ZeroFixedLeg:
+    #             self.periods[0].index_fixings = self.index_fixings
+    #             self.periods[1].index_fixings = self.index_fixings
+    #         elif type(self) is IndexFixedLegExchange and self.inital_exchange is False:
+    #             self.periods[0].index_fixings = self.index_fixings
+    #         else:
+    #             self.periods[0].index_fixings = self.index_fixings
+    #         # TODO index_fixings as a list cannot handle amortization. Use a Series.
+
+    @property
+    def index_fixings(self):
+        return self._index_fixings
+
+    @index_fixings.setter
+    def index_fixings(self, value):
+        self._index_fixings = value
+        # if value is not None:
+        for i, period in enumerate(self.periods):
+
+            if isinstance(period, (IndexFixedPeriod, IndexCashflow)):
+                if isinstance(value, Series):
+                    _ = IndexMixin._index_value(
+                        i_fixings=value,
+                        i_method=self.index_method,
+                        i_lag=self.index_lag,
+                        i_date=period.end,
+                        i_curve=None,  # not required because i_fixings is Series
+                    )
+                elif isinstance(value, list):
+                    if i >= len(value):
+                        _ = None  # some fixings are unknown, list size is limited
+                    else:
+                        _ = value[i]
+                else:
+                    # value is float or None
+                    _ = value if i == 0 else None
+                period.index_fixings = _
+
+    @property
+    def index_base(self):
+        return self._index_base
+
+    @index_base.setter
+    def index_base(self, value):
+        if isinstance(value, Series):
+            value = IndexMixin._index_value(
+                i_fixings=value,
+                i_method=self.index_method,
+                i_lag=self.index_lag,
+                i_date=self.schedule.effective,
+                i_curve=None,  # not required becuase i_fixings is Series
+            )
+        self._index_base = value
+        # if value is not None:
+        for period in self.periods:
+            if isinstance(period, (IndexFixedPeriod, IndexCashflow)):
+                period.index_base = value
+
+
+class IndexFixedLeg(IndexLegMixin, FixedLeg):
+    """
+    Create a fixed leg composed of :class:`~rateslib.periods.IndexFixedPeriod` s.
+
+    Parameters
+    ----------
+    args : tuple
+        Required positional args to :class:`BaseLeg`.
+    fixed_rate : float, optional
+        The rate applied to determine cashflows. Can be set to `None` and designated
+        later, perhaps after a mid-market rate for all periods has been calculated.
+    index_base : float or None, optional
+        The base index applied to all periods.
+    index_fixings : float, or Series, optional
+        If a float scalar, will be applied as the index fixing for the first
+        period.
+        If a list of *n* fixings will be used as the index fixings for the first *n*
+        periods.
+        If a datetime indexed ``Series`` will use the fixings that are available in
+        that object, and derive the rest from the ``curve``.
+    index_method : str, optional
+        Whether the indexing uses a daily measure for settlement or the most recently
+        monthly data taken from the first day of month.
+    index_lag : int, optional
+        The number of months by which the index value is lagged. Used to ensure
+        consistency between curves and forecast values. Defined by default.
+    kwargs : dict
+        Required keyword arguments to :class:`BaseLeg`.
+
+    Notes
+    -----
+    The NPV of an *IndexFixedLeg* is the sum of the period NPVs.
+
+    .. math::
+
+       P = - R \\sum_{i=1}^n {N_i d_i v_i(m_i) I(m_i)}
+
+    The analytic delta is the sum of the period analytic deltas.
+
+    .. math::
+
+       A = -\\frac{\\partial P}{\\partial R} = \\sum_{i=1}^n {N_i d_i v_i(m_i) I(m_i)}
+    """
+
+    def __init__(
+        self,
+        *args,
+        fixed_rate: Optional[float] = None,
+        index_base: float,
+        index_fixings: Optional[Union[float, Series]] = None,
+        index_method: Optional[str] = None,
+        index_lag: Optional[int] = None,
+        **kwargs,
+    ):
+
+        super().__init__(*args, fixed_rate=fixed_rate, **kwargs)
+        self.index_method = defaults.index_method if index_method is None else index_method.lower()
+        self.index_lag = defaults.index_lag if index_lag is None else index_lag
+        self.periods = [
+            IndexFixedPeriod(
+                fixed_rate=self.fixed_rate,
+                start=period[defaults.headers["a_acc_start"]],
+                end=period[defaults.headers["a_acc_end"]],
+                payment=period[defaults.headers["payment"]],
+                notional=self.notional - self.amortization * i,
+                currency=self.currency,
+                convention=self.convention,
+                termination=self.schedule.termination,
+                frequency=self.schedule.frequency,
+                stub=True if period[defaults.headers["stub_type"]] == "Stub" else False,
+                index_base=index_base,
+                index_fixings=self.index_fixings,
+                index_method=index_method,
+            )
+            for i, period in self.schedule.table.to_dict(orient="index").items()
+        ]
+        self.index_fixings = index_fixings  # set index fixings after periods init
+        self.index_base = index_base  # set after periods initialised
+
+    def analytic_delta(self, *args, **kwargs):
+        """
+        Return the analytic delta of the *IndexFixedLeg* via summing all periods.
+
+        For arguments see
+        :meth:`BasePeriod.analytic_delta()<rateslib.periods.BasePeriod.analytic_delta>`.
+        """
+        return super().analytic_delta(*args, **kwargs)
+
+    def cashflows(self, *args, **kwargs) -> DataFrame:
+        """
+        Return the properties of the *IndexFixedLeg* used in calculating cashflows.
+
+        For arguments see
+        :meth:`BasePeriod.cashflows()<rateslib.periods.BasePeriod.cashflows>`.
+        """
+        return super().cashflows(*args, **kwargs)
+
+    def npv(self, *args, **kwargs):
+        """
+        Return the NPV of the *IndexFixedLeg* via summing all periods.
+
+        For arguments see
+        :meth:`BasePeriod.npv()<rateslib.periods.BasePeriod.npv>`.
+        """
+        return super().npv(*args, **kwargs)
+
+
 class ZeroFloatLeg(BaseLeg, FloatLegMixin):
     """
     Create a zero coupon floating leg composed of
     :class:`~rateslib.periods.FloatPeriod` s.
 
     Parameters
     ----------
@@ -701,26 +1006,35 @@
     method_param : int, optional
         A parameter that is used for the various ``fixing_method`` s. See notes.
     kwargs : dict
         Required keyword arguments to :class:`BaseLeg`.
 
     Notes
     -----
+    The NPV of a *ZeroFloatLeg* is:
+
+    .. math::
+
+       P = -N v(m_n) \\left ( \\prod_{i=1}^n (1 + d_i r_i(r_j, z)) - 1 \\right )
+
+    The analytic delta of a *ZeroFloatLeg* is:
+
+    .. math::
+
+      A = N v(m_n) \\sum_{k=1}^n d_k \\frac{\\partial r_k}{\\partial z} \\prod_{i=1, i \\ne k}^n (1 + d_i r_i(r_j, z))
+
     .. warning::
 
        When floating rates are determined from historical fixings the forecast
        ``Curve`` ``calendar`` will be used to determine fixing dates.
        If this calendar does not align with the leg ``calendar`` then
        spurious results or errors may be generated. Including the curve calendar in
        the leg is acceptable, i.e. a leg calendar of *"nyc,ldn,tgt"* and a curve
        calendar of *"ldn"* is valid, whereas only *"nyc,tgt"* may give errors.
 
-    Examples
-    --------
-    TODO
     """
 
     def __init__(
         self,
         *args,
         float_spread: Optional[float] = None,
         fixings: Optional[Union[float, list, Series]] = None,
@@ -766,15 +1080,15 @@
         _ = 0.0
         for period in self.periods:
             _ += period.dcf
         return _
 
     def rate(self, curve):
         """
-        Calculating the floating rate for the zero coupon leg.
+        Calculating a period type floating rate for the zero coupon leg.
 
         Parameters
         ----------
         curve : Curve, LineCurve
             The forecasting curve object.
 
         Returns
@@ -791,68 +1105,77 @@
         self,
         curve: Curve,
         disc_curve: Optional[Curve] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
         local: bool = False,
     ):
+        """
+        Return the NPV of the *ZeroFloatLeg* via summing all periods.
+
+        For arguments see
+        :meth:`BasePeriod.npv()<rateslib.periods.BasePeriod.npv>`.
+        """
         disc_curve = disc_curve or curve
         fx, base = _get_fx_and_base(self.currency, fx, base)
         value = (
             self.rate(curve)
             / 100
             * self.dcf
             * disc_curve[self.schedule.pschedule[-1]]
             * -self.notional
         )
         if local:
             return {self.currency: value}
         else:
             return fx * value
 
-    def fixings_table(self, curve: Curve):
+    def fixings_table(self, curve: Curve):  # pragma: no cover
         # TODO: fixing table for ZeroFloatLeg
         raise NotImplementedError("fixings table on ZeroFloatLeg.")
 
-    def analytic_delta(self, *args, **kwargs):
-        # TODO: a delta for ZeroFloatLeg
-        raise NotImplementedError("analytic delta on ZeroFloatLeg.")
+    def analytic_delta(
+        self,
+        curve: Optional[Curve] = None,
+        disc_curve: Optional[Curve] = None,
+        fx: Union[float, FXRates, FXForwards] = 1.0,
+        base: Optional[str] = None,
+    ):
+        """
+        Return the analytic delta of the *ZeroFloatLeg* from all periods.
+
+        For arguments see
+        :meth:`BasePeriod.analytic_delta()<rateslib.periods.BasePeriod.analytic_delta>`.
+        """
+        disc_curve_: Curve = disc_curve or curve
+        fx, base = _get_fx_and_base(self.currency, fx, base)
+        compounded_rate, total_dcf = 1.0, 0.0
+        for period in self.periods:
+            compounded_rate *= 1 + period.dcf * period.rate(curve) / 100
+
+        a_sum = 0.0
+        for period in self.periods:
+            _ = period.analytic_delta(curve, disc_curve_, fx, base) / disc_curve_[period.payment]
+            _ *= compounded_rate / (1 + period.dcf * period.rate(curve) / 100)
+            a_sum += _
+        a_sum *= disc_curve_[self.schedule.pschedule[-1]] * fx
+        return a_sum
 
     def cashflows(
         self,
         curve: Optional[Curve] = None,
         disc_curve: Optional[Curve] = None,
         fx: Union[float, FXRates, FXForwards] = 1.0,
         base: Optional[str] = None,
     ):
         """
-        Return the properties of the leg used in calculating cashflows.
+        Return the properties of the *ZeroFloatLeg* used in calculating cashflows.
 
-        Parameters
-        ----------
-        curve : Curve, optional
-            The forecasting curve object. Not used unless it is set equal to
-            ``disc_curve``, or if a rate in a :class:`FloatPeriod` is required.
-        disc_curve : Curve, optional
-            The discounting curve object used in calculations.
-            Set equal to ``curve`` if not given.
-        fx : float, FXRates, FXForwards, optional
-            The immediate settlement FX rate that will be used to convert values
-            into another currency. A given `float` is used directly. If giving a
-            :class:`~rateslib.fx.FXRates` or :class:`~rateslib.fx.FXForwards`
-            object, converts from local currency into ``base``.
-        base : str, optional
-            The base currency to convert cashflows into (3-digit code).
-            Only used if ``fx`` is an :class:`~rateslib.fx.FXRates` or
-            :class:`~rateslib.fx.FXForwards` object. If not given defaults to
-            ``fx.base``.
-
-        Returns
-        -------
-        DataFrame
+        For arguments see
+        :meth:`BasePeriod.npv()<rateslib.periods.BasePeriod.npv>`.
         """
         disc_curve = disc_curve or curve
         fx, base = _get_fx_and_base(self.currency, fx, base)
         rate = None if curve is None else float(self.rate(curve))
         cashflow = (
             None if rate is None else -float(self.notional * self.dcf * rate / 100)
         )
@@ -883,14 +1206,340 @@
                 defaults.headers["fx"]: float(fx),
                 defaults.headers["npv_fx"]: npv_fx,
             }
         ]
         return DataFrame.from_records(seq)
 
 
+class ZeroFixedLeg(BaseLeg, FixedLegMixin):
+    """
+    Create a zero coupon fixed leg composed of a single
+    :class:`~rateslib.periods.FixedPeriod` .
+
+    Parameters
+    ----------
+    args : dict
+        Required positional args to :class:`BaseLeg`.
+    fixed_rate : float, optional
+        The IRR rate applied to determine cashflows. Can be set to `None` and designated
+        later, perhaps after a mid-market rate for all periods has been calculated.
+    kwargs : dict
+        Required keyword arguments to :class:`BaseLeg`.
+
+    Notes
+    -----
+    .. warning::
+
+       The ``fixed_rate`` in this calculation is not a period rate but an IRR
+       defining the cashflow as follows,
+
+       .. math::
+
+          C = -N \\left ( \\left (1 + \\frac{R^{irr}}{f} \\right ) ^ {df} - 1 \\right )
+
+    The NPV of a *ZeroFixedLeg* is:
+
+    .. math::
+
+       P = -N v(m) \\left ( \\left (1+\\frac{R^{irr}}{f} \\right )^{df} - 1 \\right )
+
+    The analytic delta of a *ZeroFixedLeg* is:
+
+    .. math::
+
+      A = N d v(m) \\left ( 1+ \\frac{R^{irr}}{f} \\right )^{df -1}
+
+    """
+
+    def __init__(self, *args, fixed_rate: Optional[float] = None, **kwargs):
+
+        super().__init__(*args, **kwargs)
+        self.periods = [
+            FixedPeriod(
+                fixed_rate=None,
+                start=self.schedule.effective,
+                end=self.schedule.termination,
+                payment=self.schedule.pschedule[-1],
+                notional=self.notional,
+                currency=self.currency,
+                convention=self.convention,
+                termination=self.schedule.termination,
+                frequency=self.schedule.frequency,
+                stub=False,
+            )
+        ]
+        self.fixed_rate = fixed_rate
+
+    @property
+    def fixed_rate(self):
+        """
+        float or None : If set will also set the ``fixed_rate`` of
+            contained :class:`FixedPeriod` s.
+        """
+        return self._fixed_rate
+
+    @fixed_rate.setter
+    def fixed_rate(self, value):
+        # overload the setter for a zero coupon to convert from irr to period rate
+        self._fixed_rate = value
+        f = 12 / defaults.frequency_months[self.schedule.frequency]
+        if value is not None:
+            period_rate = 100 * (1 / self.dcf) * ((1 + value / (100 * f)) ** (self.dcf * f) - 1)
+        else:
+            period_rate = None
+
+        for period in self.periods:
+            if isinstance(period, FixedPeriod):
+                period.fixed_rate = period_rate
+
+    @property
+    def dcf(self):
+        """
+        The DCF of a *ZeroFixedLeg* is defined as DCF of the single *FixedPeriod*
+        spanning the *Leg*.
+        """
+        _ = 0.0
+        for period in self.periods:
+            _ += period.dcf
+        return _
+
+    def cashflows(
+        self,
+        curve: Optional[Curve] = None,
+        disc_curve: Optional[Curve] = None,
+        fx: Union[float, FXRates, FXForwards] = 1.0,
+        base: Optional[str] = None,
+    ):
+        """
+        Return the cashflows of the *ZeroFixedLeg* from all periods.
+
+        For arguments see
+        :meth:`BasePeriod.cashflows()<rateslib.periods.BasePeriod.cashflows>`.
+        """
+        disc_curve = disc_curve or curve
+        fx, base = _get_fx_and_base(self.currency, fx, base)
+        rate = self.fixed_rate
+        cashflow = self.periods[0].cashflow
+        if disc_curve is None or rate is None:
+            npv, npv_fx = None, None
+        else:
+            npv = float(self.npv(curve, disc_curve))
+            npv_fx = npv * float(fx)
+        seq = [
+            {
+                defaults.headers["type"]: type(self).__name__,
+                defaults.headers["stub_type"]: None,
+                defaults.headers["currency"]: self.currency.upper(),
+                defaults.headers["a_acc_start"]: self.schedule.effective,
+                defaults.headers["a_acc_end"]: self.schedule.termination,
+                defaults.headers["payment"]: self.schedule.pschedule[-1],
+                defaults.headers["convention"]: self.convention,
+                defaults.headers["dcf"]: self.dcf,
+                defaults.headers["notional"]: float(self.notional),
+                defaults.headers["df"]: None
+                if disc_curve is None
+                else float(disc_curve[self.schedule.pschedule[-1]]),
+                defaults.headers["rate"]: self.fixed_rate,
+                defaults.headers["spread"]: None,
+                defaults.headers["cashflow"]: cashflow,
+                defaults.headers["npv"]: npv,
+                defaults.headers["fx"]: float(fx),
+                defaults.headers["npv_fx"]: npv_fx,
+            }
+        ]
+        return DataFrame.from_records(seq)
+
+    def analytic_delta(
+        self,
+        curve: Optional[Curve] = None,
+        disc_curve: Optional[Curve] = None,
+        fx: Union[float, FXRates, FXForwards] = 1.0,
+        base: Optional[str] = None,
+    ) -> DualTypes:
+        """
+        Return the analytic delta of the *ZeroFixedLeg* from all periods.
+
+        For arguments see
+        :meth:`BasePeriod.analytic_delta()<rateslib.periods.BasePeriod.analytic_delta>`.
+        """
+        disc_curve_: Curve = disc_curve or curve
+        if self.fixed_rate is None:
+            return None
+
+        f = 12 / defaults.frequency_months[self.schedule.frequency]
+        _ = self.notional * self.dcf * disc_curve_[self.periods[0].payment]
+        _ *= (1 + self.fixed_rate / (100*f)) ** (self.dcf * f - 1)
+        return _ / 10000
+
+    def _analytic_delta(self, *args, **kwargs) -> DualTypes:
+        """
+        Analytic delta based on period rate and not IRR.
+        """
+        _ = 0.0
+        for period in self.periods:
+            _ += period.analytic_delta(*args, **kwargs)
+        return _
+
+    def _spread(self, target_npv, fore_curve, disc_curve, fx=None):
+        """
+        Overload the _spread calc to use analytic delta based on period rate
+        """
+        a_delta = self._analytic_delta(fore_curve, disc_curve, fx, self.currency)
+        period_rate = -target_npv / (a_delta * 100)
+        f = 12 / defaults.frequency_months[self.schedule.frequency]
+        _ = f * ((1 + period_rate * self.dcf/ 100)**(1/(self.dcf*f)) - 1)
+        return _ * 10000
+
+    def npv(self, *args, **kwargs):
+        """
+        Return the NPV of the *ZeroFixedLeg* via summing all periods.
+
+        For arguments see
+        :meth:`BasePeriod.npv()<rateslib.periods.BasePeriod.npv>`.
+        """
+        return super().npv(*args, **kwargs)
+
+
+class ZeroIndexLeg(BaseLeg, IndexLegMixin):
+    """
+    Create a zero coupon index leg composed of a single
+    :class:`~rateslib.periods.IndexFixedPeriod` and
+    a :class:`~rateslib.periods.Cashflow`.
+
+    Parameters
+    ----------
+    args : dict
+        Required positional args to :class:`BaseLeg`.
+    index_base : float or None, optional
+        The base index applied to all periods.
+    index_fixings : float, or Series, optional
+        If a float scalar, will be applied as the index fixing for the first
+        period.
+        If a list of *n* fixings will be used as the index fixings for the first *n*
+        periods.
+        If a datetime indexed ``Series`` will use the fixings that are available in
+        that object, and derive the rest from the ``curve``.
+    index_method : str
+        Whether the indexing uses a daily measure for settlement or the most recently
+        monthly data taken from the first day of month.
+    index_lag : int, optional
+        The number of months by which the index value is lagged. Used to ensure
+        consistency between curves and forecast values. Defined by default.
+    kwargs : dict
+        Required keyword arguments to :class:`BaseLeg`.
+
+    Notes
+    -----
+    The fixed rate of the *IndexFixedPeriod* is set to 100% to index up the
+    complete the notional. The offsetting *Cashflow* deducts the real notional.
+
+    The NPV of a *ZeroIndexLeg* is the sum of the period NPVs.
+
+    .. math::
+
+       P = - v(m_n) N \\left ( I(m_n) - 1 \\right )
+
+    The analytic delta is defined as zero due to the lack of rates related attributes.
+
+    .. math::
+
+       A = 0
+
+    """
+
+    def __init__(
+        self,
+        *args,
+        index_base: Optional[Union[float, Series]] = None,
+        index_fixings: Optional[Union[float, Series]] = None,
+        index_method: Optional[str] = None,
+        index_lag: Optional[int] = None,
+        **kwargs
+    ):
+        super().__init__(*args, **kwargs)
+        self.index_method = defaults.index_method if index_method is None else index_method.lower()
+        self.index_lag = defaults.index_lag if index_lag is None else index_lag
+        # The first period indexes up the complete notional amount.
+        # The second period deducts the un-indexed notional amount.
+        self.periods = [
+            IndexFixedPeriod(
+                fixed_rate=100.0,
+                start=self.schedule.effective,
+                end=self.schedule.termination,
+                payment=self.schedule.pschedule[-1],
+                convention="1",
+                frequency=self.schedule.frequency,
+                notional=self.notional,
+                currency=self.currency,
+                termination=self.schedule.termination,
+                stub=False,
+                index_base=self.index_base,
+                index_fixings=self.index_fixings,
+                index_lag=self.index_lag,
+                index_method=self.index_method,
+            ),
+            Cashflow(
+                notional=-self.notional,
+                payment=self.schedule.pschedule[-1],
+                currency=self.currency,
+                stub_type=None,
+                rate=None,
+            )
+        ]
+        self.index_fixings = index_fixings  # set index fixings after periods init
+        self.index_base = index_base  # set after periods initialised
+
+    def cashflow(self, curve: Optional[IndexCurve] = None):
+        """Aggregate the cashflows on the *IndexFixedPeriod* and *Cashflow* period."""
+        _ = self.periods[0].cashflow(curve) + self.periods[1].cashflow
+        return _
+
+    def cashflows(self, *args, **kwargs):
+        """
+        Return the properties of the *IndexFixedLeg* used in calculating cashflows.
+
+        For arguments see
+        :meth:`BasePeriod.cashflows()<rateslib.periods.BasePeriod.cashflows>`.
+        """
+        cfs = super().cashflows(*args, **kwargs)
+        _ = cfs.iloc[[0]].copy()
+        for attr in ["Cashflow", "NPV", "NPV Ccy"]:
+            _[attr] += cfs.iloc[1][attr]
+        _["Type"] = "ZeroIndexLeg"
+        _["Period"] = None
+        return _
+
+    def analytic_delta(self, *args, **kwargs):
+        """
+        Return the analytic delta of the *ZeroIndexLeg* via summing all periods.
+
+        For arguments see
+        :meth:`BasePeriod.analytic_delta()<rateslib.periods.BasePeriod.analytic_delta>`.
+        """
+        return 0.0
+
+    def cashflows(self, *args, **kwargs) -> DataFrame:
+        """
+        Return the properties of the *ZeroIndexLeg* used in calculating cashflows.
+
+        For arguments see
+        :meth:`BasePeriod.cashflows()<rateslib.periods.BasePeriod.cashflows>`.
+        """
+        return super().cashflows(*args, **kwargs)
+
+    def npv(self, *args, **kwargs):
+        """
+        Return the NPV of the *ZeroIndexLeg* via summing all periods.
+
+        For arguments see
+        :meth:`BasePeriod.npv()<rateslib.periods.BasePeriod.npv>`.
+        """
+        return super().npv(*args, **kwargs)
+
+
 class BaseLegExchange(BaseLeg):
     """
     Abstract base class with common parameters for all ``LegExchange`` subclasses.
 
     Parameters
     ----------
     args : dict
@@ -903,14 +1552,15 @@
     kwargs : dict
         Required keyword arguments to :class:`BaseLeg`.
 
     See Also
     --------
     FixedLegExchange : Create a fixed leg with additional notional exchanges.
     FloatLegExchange : Create a floating leg with additional notional exchanges.
+    IndexFixedLegExchange : Create a fixed leg indexed with additional indexed notional exchanges.
     BaseLegExchangeMtm : Base class for legs with additional MTM notional exchanges.
     """
 
     _is_mtm = False
 
     def __init__(
         self,
@@ -946,14 +1596,22 @@
         self._amortization = value
         self._set_periods()
 
     @abstractmethod
     def _set_periods(self):
         pass  # pragma: no cover
 
+    def npv(self, *args, **kwargs):
+        return super().npv(*args, **kwargs)
+
+    def cashflows(self, *args, **kwargs):
+        return super().cashflows(*args, **kwargs)
+
+    def analytic_delta(self, *args, **kwargs):
+        return super().analytic_delta(*args, **kwargs)
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
 
 class FixedLegExchange(FixedLegMixin, BaseLegExchange):
@@ -1055,186 +1713,184 @@
                     self.schedule.calendar,
                 ),
                 self.currency,
                 "Exchange",
             )
         )
 
+    def npv(self, *args, **kwargs):
+        return super().npv(*args, **kwargs)
+
+    def cashflows(self, *args, **kwargs):
+        return super().cashflows(*args, **kwargs)
+
+    def analytic_delta(self, *args, **kwargs):
+        return super().analytic_delta(*args, **kwargs)
+
 
-class IndexFixedLegExchange(FixedLegMixin, BaseLegExchange):
+class IndexFixedLegExchange(IndexLegMixin, FixedLegMixin, BaseLegExchange):
     """
     Create a leg of :class:`~rateslib.periods.IndexFixedPeriod` s and initial and
     final :class:`~rateslib.periods.IndexCashflow` s.
 
     Parameters
     ----------
     args : dict
         Required positional args to :class:`BaseLegExchange`.
     index_base : float or None, optional
         The base index to determine the cashflow.
-    index_fixings : float, or Series, optional
-        If a float scalar, will be applied as the index fixing for the whole
-        period. If a datetime indexed ``Series`` will use the
-        fixings that are available in that object, and derive the rest from the
-        ``curve``.
+    index_fixings : float, list or Series, optional
+        If a float scalar, will be applied as the index fixing for the first period.
+        If a datetime indexed ``Series``, will use the fixings that are available
+        in that object for relevant periods, and derive the rest from the ``curve``.
+        If a list, will apply those values as the fixings for the first set of periods
+        and derive the rest from the ``curve``.
     index_method : str
         Whether the indexing uses a daily measure for settlement or the most recently
         monthly data taken from the first day of month.
     fixed_rate : float or None
         The fixed rate applied to determine cashflows. Can be set to `None` and
         designated later, perhaps after a mid-market rate for all periods has been
         calculated.
     kwargs : dict
         Required keyword arguments to :class:`BaseLegExchange`.
 
     Notes
     -----
-    The initial cashflow notional is set as the negative of the notional. The payment
-    date is set equal to the accrual start date adjusted by
-    the ``payment_lag_exchange``.
+    An initial exchange is not currently implement for this leg.
 
     The final cashflow notional is set as the notional. The payment date is set equal
     to the final accrual date adjusted by ``payment_lag_exchange``.
 
     If ``amortization`` is specified an exchanged notional equivalent to the
     amortization amount is added to the list of periods. For similar examples see
     :class:`~rateslib.legs.FloatLegExchange`.
     """
 
+    # TODO: spread calculations to determine the fixed rate on this leg do not work.
     def __init__(
         self,
         *args,
         index_base: float,
         index_fixings: Optional[Union[float, Series]] = None,
-        index_method: str = "daily",
+        index_method: Optional[str] = None,
+        index_lag: Optional[int] = None,
         fixed_rate: Optional[float] = None,
-        **kwargs
+        **kwargs,
     ) -> None:
         self._fixed_rate = fixed_rate
-        self.index_base = index_base
-        self.index_method = index_method.lower()
+        self.index_lag = defaults.index_lag if index_lag is None else index_lag
+        self.index_method = defaults.index_method if index_method is None else index_method.lower()
         if self.index_method not in ["daily", "monthly"]:
             raise ValueError("`index_method` must be in {'daily', 'monthly'}.")
         super().__init__(*args, **kwargs)
-        self._set_index_fixings(index_fixings)
+        if self.initial_exchange:
+            raise NotImplementedError(
+                "Cannot construct `IndexFixedLegExchange` with `initial_exchange` "
+                "due to not implemented `index_fixings` input argument applicable to "
+                "the indexing-up the initial exchange."
+            )
         self._set_periods()
-
-    def _set_index_fixings(
-        self,
-        index_fixings: Optional[Union[float, list, Series]]
-    ) -> None:
-        """
-        Re-organises the ``index_fixings`` input to list structure for each period.
-        Requires a ``schedule`` object and ``index_args``.
-        """
-        if index_fixings is None:
-            index_fixings_: list = []
-        elif isinstance(index_fixings, Series):
-            last_fixing = index_fixings.index[-1]
-            required_day = self.schedule.pschedule[:self.schedule.n_periods]
-            if self.index_method == "monthly":
-                required_day = [
-                    datetime(d.year, d.month, 1) for d in required_day
-                ]
-            index_fixings_ = [
-                index_fixings if last_fixing >= d else None for d in required_day
-            ]
-        elif not isinstance(index_fixings, list):
-            index_fixings_ = [index_fixings]
-        else:
-            index_fixings_ = index_fixings
-
-        self.index_fixings = (
-            index_fixings_ + [None] * (self.schedule.n_periods - len(index_fixings_))
-        )
-        return None
+        self.index_fixings = index_fixings  # set index fixings after periods init
+        self.index_base = index_base  # set after periods initialised
 
     def _set_periods(self) -> None:
+        self.periods = []
+
         # initial exchange
-        self.periods = (
-            [
+        if self.initial_exchange:
+            # TODO this conflicts with the error on initialisation regarding initial exc
+            self.periods.append(
                 IndexCashflow(
                     notional=-self.notional,
                     payment=add_tenor(
                         self.schedule.aschedule[0],
                         f"{self.payment_lag_exchange}B",
                         None,
                         self.schedule.calendar,
                     ),
                     currency=self.currency,
                     stub_type="Exchange",
                     rate=None,
                     index_base=self.index_base,
-                    index_fixings=self.index_fixings[0],
-                    index_method=self.index_method
+                    index_fixings=self.index_fixings,
+                    index_method=self.index_method,
                 )
-            ]
-            if self.initial_exchange
-            else []
-        )
+            )
 
+        # regular periods
         regular_periods = [
             IndexFixedPeriod(
                 fixed_rate=self.fixed_rate,
                 start=period[defaults.headers["a_acc_start"]],
                 end=period[defaults.headers["a_acc_end"]],
                 payment=period[defaults.headers["payment"]],
                 notional=self.notional - self.amortization * i,
                 convention=self.convention,
                 currency=self.currency,
                 termination=self.schedule.termination,
                 frequency=self.schedule.frequency,
                 stub=True if period[defaults.headers["stub_type"]] == "Stub" else False,
                 index_base=self.index_base,
                 index_method=self.index_method,
-                index_fixings=self.index_fixings[i]
+                index_fixings=self.index_fixings,
             )
             for i, period in self.schedule.table.to_dict(orient="index").items()
         ]
         if self.amortization != 0:
             amortization = [
                 IndexCashflow(
                     notional=self.amortization,
                     payment=self.schedule.pschedule[1 + i],
                     currency=self.currency,
                     stub_type="Amortization",
                     rate=None,
                     index_base=self.index_base,
-                    index_fixings=self.index_fixings[1 + i],
-                    index_method=self.index_method
+                    index_fixings=self.index_fixings,
+                    index_method=self.index_method,
                 )
                 for i in range(self.schedule.n_periods - 1)
             ]
             interleaved_periods = [
                 val for pair in zip(regular_periods, amortization) for val in pair
             ]
             interleaved_periods.append(regular_periods[-1])  # add last regular period
         else:
             interleaved_periods = regular_periods
         self.periods.extend(interleaved_periods)
 
         # final cashflow
         self.periods.append(
             IndexCashflow(
-                notional=self.notional - self.amortization * (self.schedule.n_periods - 1),
+                notional=self.notional
+                - self.amortization * (self.schedule.n_periods - 1),
                 payment=add_tenor(
                     self.schedule.aschedule[-1],
                     f"{self.payment_lag_exchange}B",
                     None,
                     self.schedule.calendar,
                 ),
                 currency=self.currency,
                 stub_type="Exchange",
                 rate=None,
                 index_base=self.index_base,
-                index_fixings=self.index_fixings[-1],
-                index_method=self.index_method
+                index_fixings=self.index_fixings,
+                index_method=self.index_method,
             )
         )
 
+    def npv(self, *args, **kwargs):
+        return super().npv(*args, **kwargs)
+
+    def cashflows(self, *args, **kwargs):
+        return super().cashflows(*args, **kwargs)
+
+    def analytic_delta(self, *args, **kwargs):
+        return super().analytic_delta(*args, **kwargs)
+
 
 class FloatLegExchange(BaseLegExchange, FloatLegMixin):
     """
     Create a leg of :class:`~rateslib.periods.FloatPeriod` s and initial and
     final :class:`~rateslib.periods.Cashflow` s.
 
     Parameters
@@ -1379,19 +2035,35 @@
                     self.schedule.calendar,
                 ),
                 self.currency,
                 "Exchange",
             )
         )
 
+    def fixings_table(self, *args, **kwargs) -> DataFrame:
+        """
+        Return a DataFrame of fixing exposures
+        on a :class:`~rateslib.legs.FloatLegExchange`.
 
-class BaseLegExchangeMtm(BaseLegExchange, metaclass=ABCMeta):
-    _do_not_repeat_set_periods = False
-    _is_mtm = True
+        For arguments see
+        :meth:`FloatPeriod.fixings_table()<rateslib.periods.FloatPeriod.fixings_table>`.
+        """
+        return super()._fixings_table(*args, **kwargs)
+
+    def npv(self, *args, **kwargs):
+        return super().npv(*args, **kwargs)
+
+    def cashflows(self, *args, **kwargs):
+        return super().cashflows(*args, **kwargs)
+
+    def analytic_delta(self, *args, **kwargs):
+        return super().analytic_delta(*args, **kwargs)
 
+
+class BaseLegExchangeMtm(BaseLegExchange, metaclass=ABCMeta):
     """
     Abstract base class with common parameters for all ``LegExchangeMtm``
     subclasses.
 
     Parameters
     ----------
     args : dict
@@ -1412,14 +2084,17 @@
 
     See Also
     --------
     FixedLegExchangeMtm: Create a fixed leg with notional and Mtm exchanges.
     FloatLegExchangeMtm : Create a floating leg with notional and Mtm exchanges.
     """
 
+    _do_not_repeat_set_periods = False
+    _is_mtm = True
+
     def __init__(
         self,
         *args,
         fx_fixings: Optional[Union[list, float, Dual, Dual2]] = None,
         alt_currency: str = None,
         alt_notional: Optional[float] = None,
         **kwargs,
@@ -1605,31 +2280,14 @@
         self,
         curve: Curve,
         disc_curve: Optional[Curve] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
         local: bool = False,
     ):
-        """
-        Return the NPV of the leg object via summing all periods.
-
-        Calculates the cashflow for the all periods and multiplies them by the
-        DF associated with each payment date.
-
-        Parameters
-        ----------
-        args :
-            Positional arguments supplied to :meth:`BasePeriod.npv`.
-        kwargs :
-            Keyword arguments supplied to :meth:`BasePeriod.npv`.
-
-        Returns
-        -------
-        float, Dual, Dual2 or dict of such
-        """
         if not self._do_not_repeat_set_periods:
             self._set_periods(fx)
         ret = super().npv(curve, disc_curve, fx, base, local)
         # self._is_set_periods_fx = False
         return ret
 
     def cashflows(
```

### Comparing `rateslib-0.2.0/rateslib/periods.py` & `rateslib-0.3.0/rateslib/periods.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This module is a dependent of legs.py
 
-# TODO float spread averaging
+# TODO v2.0 Add float rate averaging to the available fixing_method (e.g. RIBAs and monthly fed funds futures)
 
 """
 .. ipython:: python
    :suppress:
 
    from rateslib.periods import *
    from rateslib.curves import Curve
@@ -20,22 +20,23 @@
    )
 """
 
 from abc import abstractmethod, ABCMeta
 from datetime import datetime
 from typing import Optional, Union
 import warnings
+from math import comb
 
 import numpy as np
 from pandas.tseries.offsets import CustomBusinessDay
 from pandas import DataFrame, date_range, Series, NA, isna
 
 from rateslib import defaults
-from rateslib.calendars import add_tenor, get_calendar, dcf
-from rateslib.curves import Curve, LineCurve, IndexCurve
+from rateslib.calendars import add_tenor, get_calendar, dcf, _get_eom
+from rateslib.curves import Curve, LineCurve, IndexCurve, average_rate
 from rateslib.dual import Dual, Dual2, DualTypes
 from rateslib.fx import FXForwards, FXRates
 
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
@@ -87,14 +88,16 @@
         convention calculations.
 
     See Also
     --------
     FixedPeriod : Create a period defined with a fixed rate.
     FloatPeriod : Create a period defined with a floating rate index.
     Cashflow : Create a period defined by a single cashflow.
+    IndexFixedPeriod : Create a period defined with a fixed rate and an index.
+    IndexCashflow : Create a period defined by a single cashflow and an index.
     """
 
     @abstractmethod
     def __init__(
         self,
         start: datetime,
         end: datetime,
@@ -140,15 +143,15 @@
     @abstractmethod
     def analytic_delta(
         self,
         curve: Optional[Curve] = None,
         disc_curve: Optional[Curve] = None,
         fx: Union[float, FXRates, FXForwards] = 1.0,
         base: Optional[str] = None,
-    ):
+    ) -> DualTypes:
         """
         Return the analytic delta of the period object.
 
         Parameters
         ----------
         curve : Curve
             The forecasting curve object. Not used unless it is set equal to
@@ -166,53 +169,14 @@
             Only used if ``fx`` is an :class:`~rateslib.fx.FXRates` or
             :class:`~rateslib.fx.FXForwards` object.
 
         Returns
         -------
         float, Dual, Dual2
 
-        Notes
-        -----
-        For a :class:`FixedPeriod` this gives the sensitivity to the fixed rate.
-
-        .. math::
-
-           C = v N d R, \\quad A = \\frac{\\partial C}{\\partial R} = v N d
-
-        For a :class:`FloatPeriod` this gives the sensitivity to the float spread, which
-        under a ``spread_compound_method`` of *"none_simple"* (or if the
-        ``float_spread`` is zero) is equivalent to :class:`FixedPeriod` analytic delta.
-        If other compounding methods are applied the figure is usually slightly higher.
-
-        .. math::
-
-           C = v N d r(r_i, z), \\quad A = \\frac{\\partial C}{\\partial z} = v N d \\frac{\\partial r}{\\partial z}
-
-        where,
-
-        .. math::
-
-           d =& \\text{DCF of period} \\\\
-           v =& \\text{DF of period payment date}\\\\
-           N =& \\text{Notional of period}\\\\
-           R =& \\text{Fixed rate of period}\\\\
-           r =& \\text{Float period rate as a function of fixings and spread}\\\\
-           z =& \\text{Float period spread}\\\\
-
-        The sign, or direction, of analytic delta is ignorant of whether a period is
-        fixed rate or floating rate, and thus, dependent upon the context of calculating
-        either fixed rates or floating spreads, requires different interpretation.
-
-        For a **positive notional**, which assumes paying a cashflow, this method
-        returns a **positive value**. The resultant usage of analytic delta should then
-        assign a proper sign for its context in post-processing.
-
-        The analytic delta of a :class:`Cashflow` is set to zero to be compatible with
-        inherited :class:`~rateslib.instruments.BaseDerivative` methods.
-
         Examples
         --------
         .. ipython:: python
 
            curve = Curve({dt(2021,1,1): 1.00, dt(2025,1,1): 0.83}, "log_linear", id="SONIA")
            fxr = FXRates({"gbpusd": 1.25}, base="usd")
 
@@ -238,15 +202,15 @@
     @abstractmethod
     def cashflows(
         self,
         curve: Optional[Curve] = None,
         disc_curve: Optional[Curve] = None,
         fx: Union[float, FXRates, FXForwards] = 1.0,
         base: Optional[str] = None,
-    ):
+    ) -> dict:
         """
         Return the properties of the period used in calculating cashflows.
 
         Parameters
         ----------
         curve : Curve, optional
             The forecasting curve object. Not used unless it is set equal to
@@ -295,15 +259,15 @@
     def npv(
         self,
         curve: Curve,
         disc_curve: Optional[Curve] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
         local: bool = False,
-    ):
+    ) -> Union[DualTypes, dict[str, DualTypes]]:
         """
         Return the NPV of the period object.
 
         Calculates the cashflow for the period and multiplies it by the DF associated
         with the payment date.
 
         Parameters
@@ -351,25 +315,50 @@
     args : dict
         Required positional args to :class:`BasePeriod`.
     fixed_rate : float or None, optional
         The rate applied to determine the cashflow. If `None`, can be set later,
         typically after a mid-market rate for all periods has been calculated.
     kwargs : dict
         Required keyword arguments to :class:`BasePeriod`.
+
+    Notes
+    -----
+    The ``cashflow`` is defined as follows;
+
+    .. math::
+
+       C = -NdR
+
+    The :meth:`~rateslib.periods.BasePeriod.npv` is defined as;
+
+    .. math::
+
+       P = Cv = -NdRv(m)
+
+    The :meth:`~rateslib.periods.BasePeriod.analytic_delta` is defined as;
+
+    .. math::
+
+       A = - \\frac{\\partial P}{\\partial R} = Ndv(m)
     """
 
     def __init__(self, *args, fixed_rate: Union[float, None] = None, **kwargs):
         self.fixed_rate = fixed_rate
         super().__init__(*args, **kwargs)
 
-    def analytic_delta(self, *args, **kwargs):
+    def analytic_delta(self, *args, **kwargs) -> DualTypes:
+        """
+        Return the analytic delta of the *FixedPeriod*.
+        See
+        :meth:`BasePeriod.analytic_delta()<rateslib.periods.BasePeriod.analytic_delta>`
+        """
         return super().analytic_delta(*args, **kwargs)
 
     @property
-    def cashflow(self):
+    def cashflow(self) -> Union[float, None]:
         """
         float, Dual or Dual2 : The calculated value from rate, dcf and notional.
         """
         return (
             None
             if self.fixed_rate is None
             else -self.notional * self.dcf * self.fixed_rate / 100
@@ -382,15 +371,19 @@
     def npv(
         self,
         curve: Curve,
         disc_curve: Optional[Curve] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
         local: bool = False,
-    ):
+    ) -> DualTypes:
+        """
+        Return the NPV of the *FixedPeriod*.
+        See :meth:`BasePeriod.npv()<rateslib.periods.BasePeriod.npv>`
+        """
         disc_curve = disc_curve or curve
         if disc_curve is None:
             raise TypeError(
                 "`curves` have not been supplied correctly. NoneType has been detected."
             )
         fx, base = _get_fx_and_base(self.currency, fx, base)
         value = self.cashflow * disc_curve[self.payment]
@@ -401,15 +394,19 @@
 
     def cashflows(
         self,
         curve: Optional[Curve] = None,
         disc_curve: Optional[Curve] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
-    ):
+    ) -> dict:
+        """
+        Return the cashflows of the *FixedPeriod*.
+        See :meth:`BasePeriod.cashflows()<rateslib.periods.BasePeriod.cashflows>`
+        """
         disc_curve = disc_curve or curve
         fx, base = _get_fx_and_base(self.currency, fx, base)
 
         if disc_curve is None or self.fixed_rate is None:
             npv = None
             npv_fx = None
         else:
@@ -518,14 +515,31 @@
     method_param : int, optional
         A parameter that is used for the various ``fixing_method`` s. See notes.
     kwargs : dict
         Required keyword arguments to :class:`BasePeriod`.
 
     Notes
     -----
+    The ``cashflow`` is defined as follows;
+
+    .. math::
+
+       C = -Ndr(r_i, z)
+
+    The :meth:`~rateslib.periods.BasePeriod.npv` is defined as;
+
+    .. math::
+
+       P = Cv(m) = -Ndr(r_i, z)v(m)
+
+    The :meth:`~rateslib.periods.BasePeriod.analytic_delta` is defined as;
+
+    .. math::
+
+       A = - \\frac{\\partial P}{\\partial z} = Ndv(m) \\frac{\\partial r}{\\partial z}
 
     **Fixing Methods**
 
     Floating period rates depend on different ``fixing_method`` to determine their
     rates. For further info see
     :download:`ISDA RFR Compounding Memo (2006)<_static/isda-memo-rfrs-2006.pdf>`.
     The available options provided here are:
@@ -562,15 +576,14 @@
       and then everything is compounded.
     - **"isda_flat_compounding"**: the spread is added to each rate but is not used
       when compounding each previously calculated component.
 
     The first is the most efficient and most encountered. The second and third are
     rarely encountered in modern financial instruments.
     For further info see
-    :download:`Swap Compounding Formulae<_static/SSRN-id3882163(compounding).pdf>` and
     :download:`ISDA Compounding Memo (2009)<_static/isda-compounding-memo.pdf>`.
 
     .. _float fixings:
 
     **Fixings**
 
     .. warning::
@@ -748,14 +761,19 @@
     def analytic_delta(
         self,
         curve: Optional[Curve] = None,
         disc_curve: Optional[Curve] = None,
         fx: Union[float, FXRates, FXForwards] = 1.0,
         base: Optional[str] = None,
     ):
+        """
+        Return the analytic delta of the *FloatPeriod*.
+        See
+        :meth:`BasePeriod.analytic_delta()<rateslib.periods.BasePeriod.analytic_delta>`
+        """
         if self.spread_compound_method == "none_simple" or self.float_spread == 0:
             # then analytic_delta is not impacted by float_spread compounding
             dr_dz = 1.0
         elif isinstance(curve, Curve):
             _ = self.float_spread
             DualType = Dual if curve.ad in [0, 1] else Dual2
             self.float_spread = DualType(float(_), "z_float_spread")
@@ -772,26 +790,29 @@
     def cashflows(
         self,
         curve: Optional[Curve] = None,
         disc_curve: Optional[Curve] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
     ):
+        """
+        Return the cashflows of the *FloatPeriod*.
+        See
+        :meth:`BasePeriod.cashflows()<rateslib.periods.BasePeriod.cashflows>`
+        """
         disc_curve = disc_curve or curve
         fx, base = _get_fx_and_base(self.currency, fx, base)
 
-        rate = None if curve is None else float(self.rate(curve))
+        cashflow = None if curve is None else float(self.cashflow(curve))
+        rate = None if curve is None else float(100 * cashflow / (-self.notional * self.dcf))
         if disc_curve is None or rate is None:
             npv, npv_fx = None, None
         else:
             npv = float(self.npv(curve, disc_curve))
             npv_fx = npv * float(fx)
-        cashflow = (
-            None if rate is None else -float(self.notional * self.dcf * rate / 100)
-        )
 
         return {
             **super().cashflows(curve, disc_curve, fx, base),
             defaults.headers["rate"]: rate,
             defaults.headers["spread"]: float(self.float_spread),
             defaults.headers["cashflow"]: cashflow,
             defaults.headers["npv"]: npv,
@@ -803,14 +824,19 @@
         self,
         curve: Curve,
         disc_curve: Optional[Curve] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
         local: bool = False,
     ):
+        """
+        Return the cashflows of the *FloatPeriod*.
+        See
+        :meth:`BasePeriod.npv()<rateslib.periods.BasePeriod.npv>`
+        """
         disc_curve = disc_curve or curve
         if disc_curve is None or curve is None:
             raise TypeError(
                 "`curves` have not been supplied correctly. NoneType has been detected."
             )
         if self.payment < disc_curve.node_dates[0]:
             return 0.0  # payment date is in the past avoid issues with fixings or rates
@@ -823,14 +849,22 @@
             * -self.notional
         )
         if local:
             return {self.currency: value}
         else:
             return fx * value
 
+    def cashflow(self, curve: Union[Curve, LineCurve]) -> Union[None, DualTypes]:
+        if curve is None:
+            return None
+        else:
+            rate = None if curve is None else self.rate(curve)
+            _ = -self.notional * self.dcf * rate / 100
+            return _
+
     def rate(self, curve: Union[Curve, LineCurve]):
         """
         Calculating the floating rate for the period.
 
         Parameters
         ----------
         curve : Curve, LineCurve
@@ -862,39 +896,40 @@
                     UserWarning,
                 )
 
             # this ignores spread_compound_type
             return self.fixings + self.float_spread / 100
         # else next calculations made based on fixings in (None, list, Series)
 
-        if type(curve) is Curve:
+        if curve._base_type == "dfs":
             if "rfr" in self.fixing_method:
                 return self._rfr_rate_from_df_curve(curve)
             elif "ibor" in self.fixing_method:
                 return self._ibor_rate_from_df_curve(curve)
-        elif type(curve) is LineCurve:
+        elif curve._base_type == "values":
             if "rfr" in self.fixing_method:
                 return self._rfr_rate_from_line_curve(curve)
             elif "ibor" in self.fixing_method:
                 return self._ibor_rate_from_line_curve(curve)
         else:
-            raise TypeError("`curve` must be of type `Curve` or `LineCurve`.")
+            raise TypeError(  # pragma: no cover
+                f"Base curve type is unrecognised: {curve._base_type}"
+            )
 
     def _rfr_rate_from_df_curve(self, curve: Curve):
-        if self.fixing_method == "rfr_payment_delay" and not self._is_complex:
+        if self.fixing_method == "rfr_payment_delay" and not self._is_inefficient:
             return curve.rate(self.start, self.end) + self.float_spread / 100
 
-        elif self.fixing_method == "rfr_observation_shift" and not self._is_complex:
+        elif self.fixing_method == "rfr_observation_shift" and not self._is_inefficient:
             start = add_tenor(self.start, f"-{self.method_param}b", "P", curve.calendar)
             end = add_tenor(self.end, f"-{self.method_param}b", "P", curve.calendar)
             return curve.rate(start, end) + self.float_spread / 100
-
             # TODO: semi-efficient method for lockout under certain conditions
         else:
-            # return complex calculation
+            # return inefficient calculation
             return self._rfr_fixings_array(curve, fixing_exposure=False)[0]
 
     def _ibor_rate_from_df_curve(self, curve: Curve):
         # the compounding method has no effect on single rate (ibor) fixings.
         if isinstance(self.fixings, Series):
             # check if we return published IBOR rate
             fixing_date = add_tenor(
@@ -932,76 +967,46 @@
         self,
         curve: Union[Curve, LineCurve],
         fixing_exposure: bool = False,
     ):
         """
         Calculate the rate of a period via extraction and combination of every fixing.
 
-        This method of calculation is used when either:
+        This method of calculation is inefficient and used when either:
 
         - known fixings needs to be combined with unknown fixings,
         - the fixing_method is of a type that needs individual fixing data,
         - the spread compound method is of a type that needs individual fixing data.
 
         Parameters
         ----------
         curve : Curve or LineCurve
             The forecasting curve used to extract the fixing data.
         fixing_exposure : bool
             Whether to calculate sensitivities to the fixings additionally.
+        fixing_exposure_approx : bool
+            Whether to use an approximation, if available, for fixing exposure calcs.
 
         Returns
         -------
         tuple
             The compounded rate, DataFrame of the calculation data.
 
         Notes
         -----
         ``start_obs`` and ``end_obs`` define the observation period for fixing rates.
         ``start_dcf`` and ``end_dcf`` define the period for day count fractions.
         Unless *"lookback"* is used which mis-aligns the obs and dcf periods these
         will be aligned.
+
+        The ``fixing_exposure_approx`` is available only for ``spread_compound_method``
+        that is either *"none_simple"* or *"isda_compounding"*.
         """
-        if self.fixing_method in ["rfr_payment_delay", "rfr_lockout"]:
-            start_obs, end_obs = self.start, self.end
-            start_dcf, end_dcf = self.start, self.end
-        elif self.fixing_method == "rfr_observation_shift":
-            start_obs = add_tenor(
-                self.start, f"-{self.method_param}b", "P", curve.calendar
-            )
-            end_obs = add_tenor(self.end, f"-{self.method_param}b", "P", curve.calendar)
-            start_dcf, end_dcf = start_obs, end_obs
-        elif self.fixing_method == "rfr_lookback":
-            start_obs = add_tenor(
-                self.start, f"-{self.method_param}b", "P", curve.calendar
-            )
-            end_obs = add_tenor(self.end, f"-{self.method_param}b", "P", curve.calendar)
-            start_dcf, end_dcf = self.start, self.end
-        else:
-            raise NotImplementedError(
-                "`fixing_method` should be in {'rfr_payment_delay', 'rfr_lockout', "
-                "'rfr_lookback', 'rfr_observation_shift'}"
-            )
 
-        obs_dates = Series(
-            date_range(  # dates of the fixing observation period
-                start=start_obs, end=end_obs, freq=curve.calendar
-            )
-        )
-        dcf_dates = Series(
-            date_range(  # dates for the dcf weights period
-                start=start_dcf, end=end_dcf, freq=curve.calendar
-            )
-        )
-        if len(dcf_dates) != len(obs_dates):
-            # this should never be true since dates should be adjusted under the
-            # curve calendar which is consistent in all above execution statements.
-            raise ValueError(  # pragma: no cover
-                "Observation and dcf dates do not align, possible `calendar` issue."
-            )
+        obs_dates, dcf_dates = self._get_method_dcf_markers(curve)
 
         dcf_vals = Series(
             [  # calculate the dcf values from the dcf dates
                 dcf(dcf_dates[i], dcf_dates[i + 1], curve.convention)
                 for i in range(len(dcf_dates.index) - 1)
             ]
         )
@@ -1037,15 +1042,15 @@
             else:
                 raise TypeError(  # pragma: no cover
                     "`fixings` should be of type scalar, None, list or Series."
                 )
 
         # reindex the rates series getting missing values from the curves
         rates = Series(
-            {k: curve.rate(k, "1b") if isna(v) else v for k, v in rates.items()}
+            {k: curve.rate(k, "1b", "F") if isna(v) else v for k, v in rates.items()}
         )
 
         if fixing_exposure:
             # need to calculate the dcfs associated with the rates (unshifted)
             if self.fixing_method in [
                 "rfr_payment_delay",
                 "rfr_observation_shift",
@@ -1138,34 +1143,35 @@
             return (
                 ((1 + dcf_vals * (rates / 100 + self.float_spread / 10000)).prod() - 1)
                 * 100
                 / dcf_vals.sum()
             )
         elif self.spread_compound_method == "isda_flat_compounding":
             sub_cashflows = (rates / 100 + self.float_spread / 10000) * dcf_vals
+            C_i = 0.0
             for i in range(1, len(sub_cashflows)):
-                k, k_ = rates.index[i], rates.index[i - 1]
-                sub_cashflows[k] += sub_cashflows[k_] * rates[k] / 100 * dcf_vals[k]
+                C_i += sub_cashflows.iloc[i-1]
+                sub_cashflows.iloc[i] += C_i * rates.iloc[i] / 100 * dcf_vals.iloc[i]
             total_cashflow = sub_cashflows.sum()
             return total_cashflow * 100 / dcf_vals.sum()
         else:
             # this path not generally hit due to validation at initialisation
             raise ValueError(
                 "`spread_compound_method` must be in {'none_simple', "
                 "'isda_compounding', 'isda_flat_compounding'}."
             )
 
     # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
     # Commercial use of this code, and/or copying and redistribution is prohibited.
     # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
     @property
-    def _is_complex(self):
+    def _is_inefficient(self):
         """
-        A complex float leg is one which is RFR based and for which each individual
+        An inefficient float period is one which is RFR based and for which each individual
         RFR fixing is required is order to calculate correctly. This occurs in the
         following cases:
 
         1) The ``fixing_method`` is lookback - since fixing have arbitrary weightings
            misaligned with their standard weightings due to arbitrary shifts.
         2) The ``spread_compound_method`` is not *"none_simple"* - this is because the
            float spread is compounded alongside the rates so there is a non-linear
@@ -1180,25 +1186,33 @@
                 return True
             elif self.float_spread == 0 or self.spread_compound_method == "none_simple":
                 return False
             else:
                 return True
         elif self.fixing_method == "ibor":
             return False
+        # else fixing method in ["rfr_lookback", "rfr_lockout"]
         return True
 
-    def fixings_table(self, curve: Union[Curve, LineCurve]):
+    def fixings_table(
+        self,
+        curve: Union[Curve, LineCurve],
+        approximate: bool = False
+    ):
         """
         Return a DataFrame of fixing exposures.
 
         Parameters
         ----------
         curve : Curve, LineCurve
             The forecast needed to calculate rates which affect compounding and
             dependent notional exposure.
+        approximate : bool, optional
+            Perform a calculation that is broadly 10x faster but potentially loses
+            precision upto 0.1%.
 
         Returns
         -------
         DataFrame
 
         Notes
         -----
@@ -1293,16 +1307,106 @@
            period = FloatPeriod(**{
                **constants,
                "fixing_method": "ibor",
                "method_param": 2,
             })
            period.fixings_table(ibor_curve)
         """
+        if approximate:
+            return self._fixings_table_fast(curve)
+        if "rfr" in self.fixing_method:
+            rate, table = self._rfr_fixings_array(
+                curve,
+                fixing_exposure=True,
+            )
+            table = table.iloc[:-1]
+            return table[["obs_dates", "notional", "dcf", "rates"]].set_index(
+                "obs_dates"
+            )
+        elif "ibor" in self.fixing_method:
+            fixing_date = add_tenor(
+                self.start, f"-{self.method_param}b", "P", curve.calendar
+            )
+            return DataFrame(
+                {
+                    "obs_dates": [fixing_date],
+                    "notional": -self.notional,
+                    "dcf": [None],
+                    "rates": [self.rate(curve)],
+                }
+            ).set_index("obs_dates")
+
+    def _fixings_table_fast(self, curve: Union[Curve, LineCurve]):
+        """
+        Return a DataFrame of **approximate** fixing exposures.
+
+        For arguments see :meth:`~rateslib.periods.FloatPeriod.fixings_table`.
+        """
         if "rfr" in self.fixing_method:
-            rate, table = self._rfr_fixings_array(curve, fixing_exposure=True)
+            # Depending upon method get the observation dates and dcf dates
+            obs_dates, dcf_dates = self._get_method_dcf_markers(curve)
+
+            # TODO this calculation could be vectorised by a 360 or 365 multiplier
+            dcf_vals = Series(
+                [  # calculate the dcf values from the dcf dates
+                    dcf(dcf_dates[i], dcf_dates[i + 1], curve.convention)
+                    for i in range(len(dcf_dates.index) - 1)
+                ]
+            )
+            obs_vals = Series(
+                [  # calculate the dcf values from the dcf dates
+                    dcf(obs_dates[i], obs_dates[i + 1], curve.convention)
+                    for i in range(len(obs_dates.index) - 1)
+                ]
+            )
+            scalar = dcf_vals.values / obs_vals.values
+            if self.fixing_method == "rfr_lockout":
+                scalar[-self.method_param:] = 0.0
+                scalar[-(self.method_param+1)] = (
+                    obs_vals.iloc[-(self.method_param+1):].sum() /
+                    obs_vals.iloc[-(self.method_param+1)]
+                )
+
+            # perform an efficient rate approximation
+            rate = curve.rate(
+                effective=obs_dates.iloc[0],
+                termination=obs_dates.iloc[-1],
+            )
+            r_bar, d, n = average_rate(
+                obs_dates.iloc[0], obs_dates.iloc[-1], curve.convention, rate
+            )
+            # approximate sensitivity to each fixing
+            z = self.float_spread / 10000
+            if self.spread_compound_method == "none_simple":
+                drdri = (1 / n) * (1 + (rate / 100) * d) ** (n-1)
+            elif self.spread_compound_method == "isda_compounding":
+                drdri = (1 / n) * (1 + (r_bar / 100 + z) * d) ** (n-1)
+            elif self.spread_compound_method == "isda_flat_compounding":
+                dr = d * r_bar / 100
+                drdri = (1 / n) * (
+                    ((1/n) * (comb(n, 1) + comb(n, 2) * dr + comb(n, 3) * dr**2))
+                    +
+                    ((r_bar / 100 + z)/n) * (comb(n, 2) * d + 2 * comb(n, 3) * dr * d)
+                )
+
+            notional_exposure = Series(
+                -self.notional * self.dcf * drdri / d * scalar, index=obs_vals.index
+            )
+
+            table = DataFrame(
+                {
+                    "obs_dates": obs_dates,
+                    "obs_dcf": obs_vals,
+                    "dcf_dates": dcf_dates,
+                    "dcf": dcf_vals,
+                    "notional": notional_exposure.apply(float, convert_dtype=float),
+                    "rates": Series(rate, index=obs_dates.index),
+                }
+            )
+
             table = table.iloc[:-1]
             return table[["obs_dates", "notional", "dcf", "rates"]].set_index(
                 "obs_dates"
             )
         elif "ibor" in self.fixing_method:
             fixing_date = add_tenor(
                 self.start, f"-{self.method_param}b", "P", curve.calendar
@@ -1312,14 +1416,87 @@
                     "obs_dates": [fixing_date],
                     "notional": -self.notional,
                     "dcf": [None],
                     "rates": [self.rate(curve)],
                 }
             ).set_index("obs_dates")
 
+    def _get_method_dcf_markers(self, curve: Union[Curve, LineCurve], endpoints=False):
+        # Depending upon method get the observation dates and dcf dates
+        if self.fixing_method in ["rfr_payment_delay", "rfr_lockout"]:
+            start_obs, end_obs = self.start, self.end
+            start_dcf, end_dcf = self.start, self.end
+        elif self.fixing_method == "rfr_observation_shift":
+            start_obs = add_tenor(
+                self.start, f"-{self.method_param}b", "P", curve.calendar
+            )
+            end_obs = add_tenor(self.end, f"-{self.method_param}b", "P", curve.calendar)
+            start_dcf, end_dcf = start_obs, end_obs
+        elif self.fixing_method == "rfr_lookback":
+            start_obs = add_tenor(
+                self.start, f"-{self.method_param}b", "P", curve.calendar
+            )
+            end_obs = add_tenor(self.end, f"-{self.method_param}b", "P", curve.calendar)
+            start_dcf, end_dcf = self.start, self.end
+        else:
+            raise NotImplementedError(
+                "`fixing_method` should be in {'rfr_payment_delay', 'rfr_lockout', "
+                "'rfr_lookback', 'rfr_observation_shift'}"
+            )
+
+        if endpoints:
+            # return just the edges without the computation of creating Series
+            return start_obs, end_obs, start_dcf, end_dcf
+
+        # dates of the fixing observation period
+        obs_dates = Series(
+            date_range(start=start_obs, end=end_obs, freq=curve.calendar)
+        )
+        # dates for the dcf weight for each observation towards the calculation
+        dcf_dates = Series(
+            date_range(start=start_dcf, end=end_dcf, freq=curve.calendar)
+        )
+        if len(dcf_dates) != len(obs_dates):
+            # this should never be true since dates should be adjusted under the
+            # curve calendar which is consistent in all above execution statements.
+            raise ValueError(  # pragma: no cover
+                "Observation and dcf dates do not align, possible `calendar` issue."
+            )
+
+        return obs_dates, dcf_dates
+
+    def _get_analytic_delta_quadratic_coeffs(self, fore_curve, disc_curve):
+        """
+        For use in the Leg._spread calculation get the 'a' and 'b' coefficients
+        """
+        os, oe, _, _ = self._get_method_dcf_markers(fore_curve, True)
+        rate = fore_curve.rate(
+            effective=os,
+            termination=oe,
+            float_spread=0.0,
+            spread_compound_method=self.spread_compound_method
+        )
+        r, d, n = average_rate(os, oe, fore_curve.convention, rate)
+        # approximate sensitivity to each fixing
+        z = 0.0 if self.float_spread is None else self.float_spread
+        if self.spread_compound_method == "isda_compounding":
+            d2rdz2 = d * (n - 1) * (1 + (r / 100 + z / 10000) * d) ** (n - 2) / 1e8
+            drdz = (1 + (r / 100 + z / 10000) * d) ** (n - 1) / 1e4
+            Nvd = -self.notional * disc_curve[self.payment] * self.dcf
+            a, b = 0.5 * Nvd * d2rdz2, Nvd * drdz
+        elif self.spread_compound_method == "isda_flat_compounding":
+            # d2rdz2 = 0.0
+            drdz = (
+                1 + comb(n, 2)/n * r/100 * d + comb(n, 3)/n * (r/100 * d) ** 2
+            ) / 1e4
+            Nvd = -self.notional * disc_curve[self.payment] * self.dcf
+            a, b = 0.0, Nvd * drdz
+
+        return a, b
+
 
 class Cashflow:
     """
     Create a single cashflow amount on a payment date (effectively a CustomPeriod).
 
     Parameters
     ----------
@@ -1340,14 +1517,32 @@
     payment : Datetime
     stub_type : str
 
     Notes
     -----
     Other common :class:`BasePeriod` parameters not required for single cashflows are
     set to *None*.
+
+    The ``cashflow`` is defined as follows;
+
+    .. math::
+
+       C = -N
+
+    The :meth:`~rateslib.periods.BasePeriod.npv` is defined as;
+
+    .. math::
+
+       P = Cv(m) = -Nv(m)
+
+    The :meth:`~rateslib.periods.BasePeriod.analytic_delta` is defined as;
+
+    .. math::
+
+       A = 0
     """
 
     def __init__(
         self,
         notional: float,
         payment: datetime,
         currency: Optional[str] = None,
@@ -1357,26 +1552,31 @@
         self.notional, self.payment = notional, payment
         self.currency = defaults.base_currency if currency is None else currency.lower()
         self.stub_type = stub_type
         self.rate_ = rate if rate is None else float(rate)
 
     def rate(self):
         """
-        The rate of the cashflow (nominal only - not used in calculations)
+        Return the associated rate initialised with the *Cashflow*. Not used for calculations.
         """
         return self.rate_
 
     def npv(
         self,
         curve: Curve,
         disc_curve: Optional[Curve] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
         local: bool = False,
     ):
+        """
+        Return the NPV of the *Cashflow*.
+        See
+        :meth:`BasePeriod.npv()<rateslib.periods.BasePeriod.npv>`
+        """
         disc_curve = disc_curve or curve
         if disc_curve is None:
             raise TypeError(
                 "`curves` have not been supplied correctly. NoneType has been detected."
             )
         fx, base = _get_fx_and_base(self.currency, fx, base)
         value = self.cashflow * disc_curve[self.payment]
@@ -1388,14 +1588,19 @@
     def cashflows(
         self,
         curve: Optional[Curve] = None,
         disc_curve: Optional[Curve] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
     ) -> dict:
+        """
+        Return the cashflows of the *Cashflow*.
+        See
+        :meth:`BasePeriod.cashflows()<rateslib.periods.BasePeriod.cashflows>`
+        """
         disc_curve = disc_curve or curve
         fx, base = _get_fx_and_base(self.currency, fx, base)
 
         if disc_curve is None:
             npv, npv_fx = None, None
         else:
             npv = float(self.npv(curve, disc_curve))
@@ -1434,82 +1639,173 @@
     def analytic_delta(
         self,
         curve: Optional[Curve] = None,
         disc_curve: Optional[Curve] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
     ):
+        """
+        Return the analytic delta of the *Cashflow*.
+        See
+        :meth:`BasePeriod.analytic_delta()<rateslib.periods.BasePeriod.analytic_delta>`
+        """
         return 0
 
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
 
 class IndexMixin(metaclass=ABCMeta):
-    index_base: float = 0.0
+    """
+    Abstract base class to include methods and properties related to indexed *Periods*.
+    """
+
+    index_base: Optional[Union[float, Series]] = None
     index_method: str = ""
     index_fixings: Optional[Union[float, Series]] = None
+    index_lag: Optional[int] = None
     payment: datetime = datetime(1990, 1, 1)
     currency: str = ""
 
     def cashflow(self, curve: Optional[IndexCurve] = None) -> Optional[DualTypes]:
         """
         float, Dual or Dual2 : The calculated value from rate, dcf and notional,
         adjusted for the index.
         """
         if self.real_cashflow is None:
             return None
-        if self.rate(curve) is None:
+        index_ratio, _, _ = self.index_ratio(curve)
+        if index_ratio is None:
             return None
-        _ = self.real_cashflow * self.rate(curve) / self.index_base
+        else:
+            _ = self.real_cashflow * index_ratio
         return _
 
-    def rate(self, curve: Optional[IndexCurve] = None) -> Optional[DualTypes]:
+    def index_ratio(self, curve: Optional[IndexCurve]) -> tuple:
         """
-        Project an index rate for the cashflow payment date.
+        Calculate the index ratio for the end date of the *IndexPeriod*.
+
+        .. math::
+
+           I(m) = \\frac{I_{val}(m)}{I_{base}}
 
         Parameters
         ----------
         curve : IndexCurve
+            The index curve from which index values are forecast.
 
         Returns
         -------
         float, Dual, Dual2
         """
-        if self.index_fixings is None:
-            if curve is None:
-                return None
-            # forecast inflation index from curve
-            return curve.index_value(self.payment, self.index_method)
-        else:
-            if isinstance(self.index_fixings, Series):
-                if self.index_method == "daily":
-                    adj_date = self.payment
-                else:  # index_method == "monthly"
-                    adj_date = datetime(self.payment.year, self.payment.month, 1)
+        denominator = self._index_value(
+            i_fixings=self.index_base,
+            i_date=getattr(self, "start", None),  # IndexCashflow has no start
+            i_curve=curve,
+            i_lag=self.index_lag,
+            i_method=self.index_method
+        )
+        numerator = self._index_value(
+            i_fixings=self.index_fixings,
+            i_date=self.end,
+            i_curve=curve,
+            i_lag=self.index_lag,
+            i_method=self.index_method
+        )
+        if numerator is None or denominator is None:
+            return None, numerator, denominator
+        else:
+            return numerator / denominator, numerator, denominator
 
-                try:
-                    return self.index_fixings[adj_date]
-                except KeyError:
-                    s = self.index_fixings.copy()
-                    s.loc[adj_date] = np.NaN  # type: ignore[call-overload]
-                    return s.sort_index().interpolate("linear")[adj_date]
+    @staticmethod
+    def _index_value_from_curve(
+        i_date: datetime,
+        i_curve: Optional[IndexCurve],
+        i_lag: int,
+        i_method: str,
+    ) -> Optional[DualTypes]:
+        if i_curve is None:
+            return None
+        elif not isinstance(i_curve, IndexCurve):
+            raise TypeError("`index_value` must be forecast from an `IndexCurve`.")
+        elif i_lag != i_curve.index_lag:
+            return None  # TODO decide if RolledCurve to correct index lag be attemoted
+        else:
+            return i_curve.index_value(i_date, i_method)
+
+    @staticmethod
+    def _index_value(
+        i_fixings: Optional[Union[float, Series]],
+        i_date: datetime,
+        i_curve: Optional[IndexCurve],
+        i_lag: int,
+        i_method: str
+    ) -> Optional[DualTypes]:
+        """
+        Project an index rate, or lookup from provided fixings, for a given date.
+
+        If ``index_fixings`` are set on the period this will be used instead of
+        the ``curve``.
+
+        Parameters
+        ----------
+        curve : IndexCurve
+
+        Returns
+        -------
+        float, Dual, Dual2
+        """
+        if i_fixings is None:
+            return IndexMixin._index_value_from_curve(i_date, i_curve, i_lag, i_method)
+        else:
+            if isinstance(i_fixings, Series):
+                if i_method == "daily":
+                    adj_date = i_date
+                    unavailable_date = i_fixings.index[-1]
+                else:
+                    adj_date = datetime(i_date.year, i_date.month, 1)
+                    _ = i_fixings.index[-1]
+                    unavailable_date = _get_eom(_.month, _.year)
+
+                if i_date > unavailable_date:
+                    if i_curve is None:
+                        return None
+                    else:
+                        return IndexMixin._index_value_from_curve(
+                            i_date, i_curve, i_lag, i_method
+                        )
+                    # raise ValueError(
+                    #     "`index_fixings` cannot forecast the index value. "
+                    #     f"There are no fixings available after date: {unavailable_date}"
+                    # )
+                else:
+                    try:
+                        return i_fixings[adj_date]
+                    except KeyError:
+                        s = i_fixings.copy()
+                        s.loc[adj_date] = np.NaN  # type: ignore[call-overload]
+                        _ = s.sort_index().interpolate("time")[adj_date]
+                        return _
             else:
-                return self.index_fixings
+                return i_fixings
 
     def npv(
         self,
         curve: IndexCurve,
         disc_curve: Optional[Curve] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
         local: bool = False,
     ):
+        """
+        Return the cashflows of the *IndexPeriod*.
+        See :meth:`BasePeriod.npv()<rateslib.periods.BasePeriod.npv>`
+        """
         disc_curve = disc_curve or curve
         if disc_curve is None:
             raise TypeError(
                 "`curves` have not been supplied correctly. NoneType has been detected."
             )
         fx, base = _get_fx_and_base(self.currency, fx, base)
         value = self.cashflow(curve) * disc_curve[self.payment]
@@ -1524,59 +1820,98 @@
         pass  # pragma: no cover
 
 
 class IndexFixedPeriod(IndexMixin, FixedPeriod):  # type: ignore[misc]
     """
     Create a period defined with a real rate adjusted by an index.
 
-    When used with inflation products this defines a real coupon period with a
+    When used with an inflation index this defines a real coupon period with a
     cashflow adjusted upwards by the inflation index.
 
     Parameters
     ----------
     args : dict
         Required positional args to :class:`FixedPeriod`.
     index_base : float or None, optional
         The base index to determine the cashflow.
     index_fixings : float, or Series, optional
-        If a float scalar, will be applied as the index fixing for the whole
-        period. If a datetime indexed ``Series`` will use the
-        fixings that are available in that object, and derive the rest from the
-        ``curve``.
-    index_method : str
+        If a float scalar, will be applied as the index fixing for the settlement, or
+        payment, date.
+        If a datetime indexed ``Series`` will use the
+        fixings that are available in that object, using linear interpolation if
+        necessary.
+    index_method : str, optional
         Whether the indexing uses a daily measure for settlement or the most recently
-        monthly data taken from the first day of month.
+        monthly data taken from the first day of month. Defined by default.
+    index_lag : int
+        The number of months by which the index value is lagged. Used to ensure
+        consistency between curves and forecast values. Defined by default.
     kwargs : dict
         Required keyword arguments to :class:`FixedPeriod`.
+
+    Notes
+    -----
+    The ``real_cashflow`` is defined as follows;
+
+    .. math::
+
+       C_{real} = -NdR
+
+    The ``cashflow`` is defined as follows;
+
+    .. math::
+
+       C = C_{real}I(m) = -NdRI(m)
+
+    The :meth:`~rateslib.periods.BasePeriod.npv` is defined as;
+
+    .. math::
+
+       P = Cv = -NdRv(m)I(m)
+
+    The :meth:`~rateslib.periods.BasePeriod.analytic_delta` is defined as;
+
+    .. math::
+
+       A = - \\frac{\\partial P}{\\partial R} = Ndv(m)I(m)
     """
 
     def __init__(
         self,
         *args,
-        index_base: float,
+        index_base: Optional[Union[float, Series]],
         index_fixings: Optional[Union[float, Series]] = None,
-        index_method: str = "daily",
+        index_method: Optional[str] = None,
+        index_lag: Optional[int] = None,
         **kwargs,
     ):
+        # if index_base is None:
+        #     raise ValueError("`index_base` cannot be None.")
         self.index_base = index_base
         self.index_fixings = index_fixings
-        self.index_method = index_method.lower()
+        self.index_method = defaults.index_method if index_method is None else index_method.lower()
+        self.index_lag = defaults.index_lag if index_lag is None else index_lag
         if self.index_method not in ["daily", "monthly"]:
             raise ValueError("`index_method` must be in {'daily', 'monthly'}.")
         super(IndexMixin, self).__init__(*args, **kwargs)
 
     def analytic_delta(
         self,
         curve: Optional[Curve] = None,
         disc_curve: Optional[Curve] = None,
         fx: Union[float, FXRates, FXForwards] = 1.0,
         base: Optional[str] = None,
     ):
+        """
+        Return the analytic delta of the *IndexFixedPeriod*.
+        See :meth:`BasePeriod.analytic_delta()<rateslib.periods.BasePeriod.analytic_delta>`
+        """
         real_a_delta = super().analytic_delta(curve, disc_curve, fx, base)
-        _ = real_a_delta * self.rate(curve) / self.index_base
+        index_ratio, _, _ = self.index_ratio(curve)
+        _ = None if index_ratio is None else real_a_delta * index_ratio
         return _
 
     @property
     def real_cashflow(self):
         """
         float, Dual or Dual2 : The calculated real value from rate, dcf and notional.
         """
@@ -1593,52 +1928,57 @@
     def cashflows(
         self,
         curve: Optional[IndexCurve] = None,
         disc_curve: Optional[Curve] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
     ):
+        """
+        Return the cashflows of the *IndexFixedPeriod*.
+        See :meth:`BasePeriod.cashflows()<rateslib.periods.BasePeriod.cashflows>`
+        """
         disc_curve = disc_curve or curve
         fx, base = _get_fx_and_base(self.currency, fx, base)
 
         if disc_curve is None or self.fixed_rate is None:
             npv = None
             npv_fx = None
         else:
             npv = float(self.npv(curve, disc_curve))
             npv_fx = npv * float(fx)
 
-        cashflow_ = self.cashflow(curve)
-        cashflow_ = None if cashflow_ is None else float(cashflow_)
-
-        index_ = self.rate(curve)
-        if index_ is None:
-            index_ratio_ = None
-        else:
-            index_ratio_ = index_ /self.index_base
+        index_ratio_, index_val_, index_base_ = self.index_ratio(curve)
 
         return {
             **super(FixedPeriod, self).cashflows(curve, disc_curve, fx, base),
             defaults.headers["rate"]: self.fixed_rate,
             defaults.headers["spread"]: None,
             defaults.headers["real_cashflow"]: self.real_cashflow,
-            defaults.headers["index_value"]: index_,
-            defaults.headers["index_ratio"]: index_ratio_,
-            defaults.headers["cashflow"]: cashflow_,
+            defaults.headers["index_base"]: _float_or_none(index_base_),
+            defaults.headers["index_value"]: _float_or_none(index_val_),
+            defaults.headers["index_ratio"]: _float_or_none(index_ratio_),
+            defaults.headers["cashflow"]: _float_or_none(self.cashflow(curve)),
             defaults.headers["npv"]: npv,
             defaults.headers["fx"]: float(fx),
             defaults.headers["npv_fx"]: npv_fx,
         }
 
+    def npv(self, *args, **kwargs):
+        """
+        Return the cashflows of the *IndexFixedPeriod*.
+        See :meth:`BasePeriod.npv()<rateslib.periods.BasePeriod.npv>`
+        """
+        return super().npv(*args, **kwargs)
+
 
 class IndexCashflow(IndexMixin, Cashflow):  # type: ignore[misc]
     """
     Create a cashflow defined with a real rate adjusted by an index.
 
-    When used with inflation products this defines a real redemption with a
+    When used with an inflation index this defines a real redemption with a
     cashflow adjusted upwards by the inflation index.
 
     Parameters
     ----------
     args : dict
         Required positional args to :class:`Cashflow`.
     index_base : float or None, optional
@@ -1646,49 +1986,102 @@
     index_fixings : float, or Series, optional
         If a float scalar, will be applied as the index fixing for the whole
         period. If a datetime indexed ``Series`` will use the
         fixings that are available in that object, and derive the rest from the
         ``curve``.
     index_method : str
         Whether the indexing uses a daily measure for settlement or the most recently
-        monthly data taken from the first day of month.
+        monthly data taken from the first day of month. Defined by default.
+    index_lag : int
+        The number of months by which the index value is lagged. Used to ensure
+        consistency between curves and forecast values. Defined by default.
     kwargs : dict
         Required keyword arguments to :class:`Cashflow`.
+
+    Notes
+    -----
+    The ``real_cashflow`` is defined as follows;
+
+    .. math::
+
+       C_{real} = -N
+
+    The ``cashflow`` is defined as follows;
+
+    .. math::
+
+       C = C_{real}I(m) = -NI(m)
+
+    The :meth:`~rateslib.periods.BasePeriod.npv` is defined as;
+
+    .. math::
+
+       P = Cv(m) = -Nv(m)I(m)
+
+    The :meth:`~rateslib.periods.BasePeriod.analytic_delta` is defined as;
+
+    .. math::
+
+       A = 0
     """
     def __init__(
         self,
         *args,
         index_base: float,
         index_fixings: Optional[Union[float, Series]] = None,
-        index_method: str = "daily",
+        index_method: Optional[str] = None,
+        index_lag: Optional[int] = None,
         **kwargs,
     ):
         self.index_base = index_base
         self.index_fixings = index_fixings
-        self.index_method = index_method.lower()
+        self.index_method = defaults.index_method if index_method is None else index_method.lower()
+        self.index_lag = defaults.index_lag if index_lag is None else index_lag
         super(IndexMixin, self).__init__(*args, **kwargs)
+        self.end = self.payment
 
     @property
     def real_cashflow(self):
         return -self.notional
 
     def cashflows(
         self,
         curve: Optional[Curve] = None,
         disc_curve: Optional[Curve] = None,
         fx: Optional[Union[float, FXRates, FXForwards]] = None,
         base: Optional[str] = None,
     ) -> dict:
-
-        index_ = self.rate(curve)
-        if index_ is None:
-            index_ratio_ = None
-        else:
-            index_ratio_ = index_ / self.index_base
-
+        """
+        Return the cashflows of the *IndexCashflow*.
+        See :meth:`BasePeriod.cashflows()<rateslib.periods.BasePeriod.cashflows>`
+        """
+        index_ratio_, index_val_, index_base_ = self.index_ratio(curve)
         return {
             **super(IndexMixin, self).cashflows(curve, disc_curve, fx, base),
             defaults.headers["real_cashflow"]: self.real_cashflow,
-            defaults.headers["index_value"]: index_,
-            defaults.headers["index_ratio"]: index_ratio_,
+            defaults.headers["index_base"]: _float_or_none(index_base_),
+            defaults.headers["index_value"]: _float_or_none(index_val_),
+            defaults.headers["index_ratio"]: _float_or_none(index_ratio_),
             defaults.headers["cashflow"]: self.cashflow(curve),
         }
+
+    def npv(self, *args, **kwargs):
+        """
+        Return the NPV of the *IndexCashflow*.
+        See :meth:`BasePeriod.npv()<rateslib.periods.BasePeriod.npv>`
+        """
+        return super().npv(*args, **kwargs)
+
+    def analytic_delta(self, *args, **kwargs):
+        """
+        Return the analytic delta of the *IndexCashflow*.
+        See
+        :meth:`BasePeriod.analytic_delta()<rateslib.periods.BasePeriod.analytic_delta>`
+        """
+        return 0.0
+
+
+def _float_or_none(val):
+    if val is None:
+        return None
+    else:
+        return float(val)
```

### Comparing `rateslib-0.2.0/rateslib/scheduling.py` & `rateslib-0.3.0/rateslib/scheduling.py`

 * *Files 5% similar despite different names*

```diff
@@ -653,19 +653,19 @@
     ----------
     ueffective : Datetime
         The unadjusted effective date.
     utermination: Datetime
         The unadjusted termination date.
     frequency : str
         The frequency of the leg.
-    roll : int in [1, 31] or str in {"eom", "imm", "som"}, optional
-        The roll day of the schedule. Inferred if not given.
     eom : bool
         Use an end of month preference rather than regular rolls for inference. Set by
         default.
+    roll : int in [1, 31] or str in {"eom", "imm", "som"}, optional
+        The roll day of the schedule. Inferred if not given.
 
     Returns
     -------
     tuple : bool, and either kwargs or error message.
 
     Notes
     -----
@@ -791,14 +791,41 @@
 
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
 
+def _is_invalid_very_short_stub(
+    date_to_modify: datetime,
+    date_fixed: datetime,
+    modifier: str,
+    calendar: CustomBusinessDay,
+):
+    """
+    This tests that a very short, i.e. 1 to a few days, stub has not been erroneously
+    generated. Short stubs are invalid if there is one genuine business day in the
+    window.
+    """
+    # _ = date_range(start=date1, end=date2, freq=calendar)
+    if _is_holiday(date_to_modify, calendar):
+        date1_ = add_tenor(date_to_modify, "1b", modifier, calendar)
+    else:
+        date1_ = date_to_modify
+
+    if _is_holiday(date_fixed, calendar):
+        date2_ = add_tenor(date_fixed, "1b", modifier, calendar)
+    else:
+        date2_ = date_fixed
+
+    if date1_ == date2_:
+        return True  # date range created by stubs is too small and is invalid
+    return False
+
+
 def _infer_stub_date(
     effective: datetime,
     termination: datetime,
     frequency: str,
     stub: str,
     front_stub: Optional[datetime],
     back_stub: Optional[datetime],
@@ -846,14 +873,15 @@
 
       - ``front_stub``: when ``stub`` is front sided only and ``back_stub`` is *None*.
       - ``front_stub``: when ``stub`` is dual sided and ``back_stub`` is specified.
       - ``back_stub``: when ``stub`` is back sided only and ``front_stub`` is *None*.
       - ``back_stub``: when ``stub`` is dual sided and ``front_stub`` is specified.
     """
     if "FRONT" in stub and "BACK" in stub:  # stub is dual sided
+        dead_front_stub, dead_back_stub = False, False
         if front_stub is None:
             assert isinstance(back_stub, datetime)
             valid, parsed_args = _check_regular_swap(
                 effective, back_stub, frequency, modifier, eom, roll, calendar
             )
             if valid:  # no front stub is required
                 return True, {
@@ -866,14 +894,17 @@
                     "eom": parsed_args["eom"],
                 }
             else:
                 stub_ = _get_default_stub("FRONT", stub)
                 front_stub = _get_unadjusted_stub_date(
                     effective, back_stub, frequency, stub_, eom, roll
                 )
+                dead_front_stub = _is_invalid_very_short_stub(
+                    effective, front_stub, modifier, calendar
+                )
         else:
             valid, parsed_args = _check_regular_swap(
                 front_stub, termination, frequency, modifier, eom, roll, calendar
             )
             if valid:  # no back stub is required
                 return True, {
                     "ueffective": effective,
@@ -885,25 +916,28 @@
                     "eom": parsed_args["eom"],
                 }
             else:
                 stub_ = _get_default_stub("BACK", stub)
                 back_stub = _get_unadjusted_stub_date(
                     front_stub, termination, frequency, stub_, eom, roll
                 )
+                dead_back_stub = _is_invalid_very_short_stub(
+                    back_stub, termination, modifier, calendar
+                )
         valid, parsed_args = _check_regular_swap(
             front_stub, back_stub, frequency, modifier, eom, roll, calendar
         )
         if not valid:
             return valid, parsed_args
         else:
             return True, {
-                "ueffective": effective,
-                "utermination": termination,
-                "front_stub": parsed_args["ueffective"],
-                "back_stub": parsed_args["utermination"],
+                "ueffective": effective if not dead_front_stub else parsed_args["ueffective"],
+                "utermination": termination if not dead_back_stub else parsed_args["utermination"],
+                "front_stub": parsed_args["ueffective"] if not dead_front_stub else None,
+                "back_stub": parsed_args["utermination"] if not dead_back_stub else None,
                 "roll": parsed_args["roll"],
                 "frequency": parsed_args["frequency"],
                 "eom": parsed_args["eom"],
             }
     elif "FRONT" in stub:
         valid, parsed_args = _check_regular_swap(
             effective, termination, frequency, modifier, eom, roll, calendar
@@ -919,24 +953,31 @@
                 "eom": parsed_args["eom"],
             }
         else:
             stub_ = _get_default_stub("FRONT", stub)
             front_stub = _get_unadjusted_stub_date(
                 effective, termination, frequency, stub_, eom, roll
             )
+
+            # The following check prohibits stubs that are too short under calendar,
+            # e.g. 2 May 27 is a Sunday and 3 May 27 is a Monday => dead_stub is True
+            dead_stub = _is_invalid_very_short_stub(
+                effective, front_stub, modifier, calendar
+            )
+
             valid, parsed_args = _check_regular_swap(
                 front_stub, termination, frequency, modifier, eom, roll, calendar
             )
             if not valid:
                 return valid, parsed_args
             else:
                 return True, {
-                    "ueffective": effective,
+                    "ueffective": effective if not dead_stub else parsed_args["ueffective"],
                     "utermination": parsed_args["utermination"],
-                    "front_stub": parsed_args["ueffective"],
+                    "front_stub": parsed_args["ueffective"] if not dead_stub else None,
                     "back_stub": None,
                     "roll": parsed_args["roll"],
                     "frequency": parsed_args["frequency"],
                     "eom": parsed_args["eom"],
                 }
     else:  # schedule is "BACK" sided
         valid, parsed_args = _check_regular_swap(
@@ -953,25 +994,32 @@
                 "eom": parsed_args["eom"],
             }
         else:
             stub_ = _get_default_stub("BACK", stub)
             back_stub = _get_unadjusted_stub_date(
                 effective, termination, frequency, stub_, eom, roll
             )
+
+            # The following check prohibits stubs that are too short under calendar,
+            # 19 Oct 47 is a Saturday and 20 Oct 47 is a Sunday => dead_stub is True
+            dead_stub = _is_invalid_very_short_stub(
+                back_stub, termination, modifier, calendar
+            )
+
             valid, parsed_args = _check_regular_swap(
                 effective, back_stub, frequency, modifier, eom, roll, calendar
             )
             if not valid:
                 return valid, parsed_args
             else:
                 return True, {
                     "ueffective": parsed_args["ueffective"],
-                    "utermination": termination,
+                    "utermination": termination if not dead_stub else parsed_args["utermination"],
                     "front_stub": None,
-                    "back_stub": parsed_args["utermination"],
+                    "back_stub": parsed_args["utermination"] if not dead_stub else None,
                     "roll": parsed_args["roll"],
                     "frequency": parsed_args["frequency"],
                     "eom": parsed_args["eom"],
                 }
 
 
 def _get_default_stub(side: str, stub: str) -> str:
@@ -1009,28 +1057,27 @@
     roll : int in [1, 31] or str in {"eom", "imm", "som"}, optional
         The roll day for the schedule.
 
     Returns
     -------
     datetime
     """
-    frequency_months = defaults.frequency_months[frequency]
+    # frequency_months = defaults.frequency_months[frequency]
+    stub_side = "FRONT" if "FRONT" in stub else "BACK"
     if "LONG" in stub:
+        _ = _get_unadjusted_short_stub_date(
+            ueffective, utermination, frequency, stub_side, eom, roll
+        )
         if "FRONT" in stub:
-            ueffective = _add_months(ueffective, frequency_months, None, None)
+            ueffective = _ + timedelta(days=1)
         else:  # "BACK" in stub
-            utermination = _add_months(utermination, -frequency_months, None, None)
+            utermination = _ - timedelta(days=1)
 
     return _get_unadjusted_short_stub_date(
-        ueffective,
-        utermination,
-        frequency,
-        "FRONT" if "FRONT" in stub else "BACK",
-        eom,
-        roll,
+        ueffective, utermination, frequency, stub_side, eom, roll,
     )
 
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
@@ -1070,36 +1117,42 @@
     else:  # stub_side == "BACK":
         stub_side_dt, reg_side_dt, direction = utermination, ueffective, -1
 
     if roll is None:
         roll = "eom" if (eom and _is_eom(reg_side_dt)) else reg_side_dt.day
 
     frequency_months = defaults.frequency_months[frequency]
-    if (
-        _is_divisible_months(ueffective, utermination, frequency_months)
-        and ueffective.day < utermination.day
-    ):
+
+    if _is_divisible_months(ueffective, utermination, frequency_months):
         if stub_side == "FRONT":
-            stub_date = _get_roll(ueffective.month, ueffective.year, roll)
-        else:
-            stub_date = _get_roll(utermination.month, utermination.year, roll)
-    elif (
-        _is_divisible_months(ueffective, utermination, frequency_months)
-        and ueffective.day >= utermination.day
-    ):
-        stub_date = _add_months(stub_side_dt, frequency_months * direction, None, None)
-        stub_date = _get_roll(stub_date.month, stub_date.year, roll)
+            comparison = _get_roll(ueffective.month, ueffective.year, roll)
+            if ueffective.day > comparison.day:
+                _ = _add_months(ueffective, frequency_months * direction, None, None)
+                _ = _get_roll(_.month, _.year, roll)
+            else:
+                _ = ueffective
+                _ = _get_roll(_.month, _.year, roll)
+
+        else:  # stub_side == "BACK"
+            comparison = _get_roll(utermination.month, utermination.year, roll)
+            if utermination.day < comparison.day:
+                _ = _add_months(utermination, frequency_months * direction, None, None)
+                _ = _get_roll(_.month, _.year, roll)
+            else:
+                _ = utermination
+                _ = _get_roll(_.month, _.year, roll)
+
     else:
         for month_offset in range(1, 12):
             stub_date = _add_months(stub_side_dt, month_offset * direction, None, None)
             if _is_divisible_months(stub_date, reg_side_dt, frequency_months):
                 break
-        stub_date = _get_roll(stub_date.month, stub_date.year, roll)
+        _ = _get_roll(stub_date.month, stub_date.year, roll)
 
-    return stub_date
+    return _
 
 
 # Book coded - This defines all the unadjusted date scheduling - no inference
 
 # The code below this line should be tested and is confident that it functions
 
 
@@ -1193,15 +1246,15 @@
 ):
     """
     Return all possible unadjusted dates that result in given date under modifier/cal.
 
     Parameters
     ----------
     date : Datetime
-        Date to test.
+        Adjusted date for which unadjusted dates can be modified to.
     modifier : str, optional
         |modifier|
     calendar : Calendar
         |calendar|
 
     Returns
     -------
```

### Comparing `rateslib-0.2.0/rateslib/solver.py` & `rateslib-0.3.0/rateslib/solver.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,19 @@
 from itertools import combinations
 from uuid import uuid4
 from time import time
 import numpy as np
 import warnings
 from pandas import DataFrame, MultiIndex, concat, Series
 
+from rateslib import defaults
 from rateslib.dual import Dual, Dual2, dual_log, dual_solve
-from rateslib.fx import FXForwards
+from rateslib.fx import FXForwards, ProxyCurve
+from rateslib.curves import CompositeCurve
+
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
 
 class Gradients:
@@ -39,15 +42,15 @@
         return self._J
 
     @property
     def grad_v_rT(self):
         """
         Alias of ``J``.
         """
-        return self.J  # pragma: no cover
+        return self.J
 
     @property
     def J2(self):
         """
         3d array of second derivatives of calibrating instrument rates with
         respect to curve variables, of size (n, n, m);
 
@@ -193,19 +196,15 @@
            [\\nabla_\mathbf{f}\mathbf{r^T}]_{i,j} = \\frac{\\partial r_j}{\\partial f_i}
 
         Parameters
         ----------
         fx_vars : list or tuple of str
             The variable name tags for the FX rate sensitivities.
         """
-        rates_pre = []
-        for solver in self.pre_solvers:
-            rates_pre += [rate for rate in solver.r]
-        rates_pre += [rate for rate in self.r]
-        grad_f_rT = np.array([rate.gradient(fx_vars) for rate in rates_pre]).T
+        grad_f_rT = np.array([rate.gradient(fx_vars) for rate in self.r_pre]).T
         return grad_f_rT
 
     @property
     def J2_pre(self):
         """
         3d array of second derivatives of calibrating instrument rates with
         respect to curve variables for all ``Solvers`` including ``pre_solvers``,
@@ -255,23 +254,18 @@
 
         Parameters
         ----------
         fx_vars : list or tuple of str
             The variable name tags for the FX rate sensitivities.
         """
         # FX sensitivity requires reverting through all pre-solvers rates.
-        rates_pre = []
-        for solver in self.pre_solvers:
-            rates_pre += [rate for rate in solver.r]
-        rates_pre += [rate for rate in self.r]
-
         all_gradients = np.array(
             [
                 rate.gradient(self.pre_variables + tuple(fx_vars), order=2)
-                for rate in rates_pre
+                for rate in self.r_pre
             ]
         ).swapaxes(0, 2)
 
         grad_f_v_rT = all_gradients[self.pre_n :, : self.pre_n, :]
         return grad_f_v_rT
 
     def grad_f_f_rT_pre(self, fx_vars):
@@ -285,21 +279,16 @@
 
         Parameters
         ----------
         fx_vars : list or tuple of str
             The variable name tags for the FX rate sensitivities.
         """
         # FX sensitivity requires reverting through all pre-solvers rates.
-        rates_pre = []
-        for solver in self.pre_solvers:
-            rates_pre += [rate for rate in solver.r]
-        rates_pre += [rate for rate in self.r]
-
         grad_f_f_rT = np.array(
-            [rate.gradient(fx_vars, order=2) for rate in rates_pre]
+            [rate.gradient(fx_vars, order=2) for rate in self.r_pre]
         ).swapaxes(0, 2)
         return grad_f_f_rT
 
     @property
     def grad_s_s_vT_pre(self):
         """
         3d array of second derivatives of curve variables with respect to
@@ -380,19 +369,15 @@
 
         Parameters
         ----------
         fx_vars : list or tuple of str
             The variable name tags for the FX rate sensitivities
         """
         # FX sensitivity requires reverting through all pre-solvers rates.
-        rates_pre = []
-        for solver in self.pre_solvers:
-            rates_pre += [rate for rate in solver.r]
-        rates_pre += [rate for rate in self.r]
-        grad_f_rT = np.array([rate.gradient(fx_vars) for rate in rates_pre]).T
+        grad_f_rT = np.array([rate.gradient(fx_vars) for rate in self.r_pre]).T
         return -np.matmul(grad_f_rT, self.grad_s_vT_pre)
 
     def grad_f_f(self, f, fx_vars):
         """
         1d array of total derivatives of FX conversion rate with respect to
         FX rate variables, of size (len(fx_vars));
 
@@ -954,24 +939,25 @@
 
     def __init__(
         self,
         curves: Union[list, tuple] = (),
         instruments: Union[tuple[tuple], list[tuple]] = (),
         s: list[float] = [],
         weights: Optional[list] = None,
-        algorithm: str = "gauss_newton",
+        algorithm: Optional[str] = None,
         fx: Optional[FXForwards] = None,
         instrument_labels: Optional[tuple[str], list[str]] = None,
         id: Optional[str] = None,
         pre_solvers: Union[tuple[Solver], list[Solver]] = (),
         max_iter: int = 100,
         func_tol: float = 1e-11,
         conv_tol: float = 1e-14,
     ) -> None:
-        self.algorithm, self.m = algorithm, len(instruments)
+        self.algorithm = algorithm if algorithm is not None else defaults.algorithm
+        self.m = len(instruments)
         self.func_tol, self.conv_tol, self.max_iter = func_tol, conv_tol, max_iter
         self.id = id or uuid4().hex[:5] + "_"  # 1 in a million clash
         self.pre_solvers = tuple(pre_solvers)
 
         # validate `id`s so that DataFrame indexing does not share duplicated keys.
         if len(set([self.id] + [p.id for p in self.pre_solvers])) < 1 + len(
             self.pre_solvers
@@ -999,15 +985,19 @@
             self.weights = np.ones(len(instruments))
         else:
             if len(weights) != self.m:
                 raise ValueError("`weights` must be same length as `instruments`.")
             self.weights = np.asarray(weights)
         self.W = np.diag(self.weights)
 
-        self.curves = {curve.id: curve for curve in curves}
+        self.curves = {
+            curve.id: curve for curve in curves
+            if not type(curve) in [ProxyCurve, CompositeCurve]
+            # Proxy and Composite curves have no parameters of their own
+        }
         self.variables = ()
         for curve in self.curves.values():
             curve._set_ad_order(1)  # solver uses gradients in optimisation
             curve_vars = tuple(
                 (f"{curve.id}{i}" for i in range(curve._ini_solve, curve.n))
             )
             self.variables += curve_vars
@@ -1025,14 +1015,19 @@
             self.pre_instrument_labels += pre_solver.pre_instrument_labels
             self.pre_rate_scalars.extend(pre_solver.pre_rate_scalars)
             self.pre_m += pre_solver.pre_m
             self.pre_n += pre_solver.pre_n
             self.pre_curves.update(pre_solver.pre_curves)
             curve_collection.extend(pre_solver.pre_curves.values())
         self.pre_curves.update(self.curves)
+        self.pre_curves.update({
+            curve.id: curve for curve in curves
+            if type(curve) in [ProxyCurve, CompositeCurve]
+            # Proxy and Composite curves added to the collection without variables
+        })
         curve_collection.extend(curves)
         for curve1, curve2 in combinations(curve_collection, 2):
             if curve1.id == curve2.id:
                 raise ValueError(
                     "`curves` must each have their own unique `id`. If using "
                     "pre-solvers as part of a dependency chain a curve can only be "
                     "specified as a variable in one solver."
@@ -1121,14 +1116,15 @@
         Returns
         -------
         None
         """
         if not dual2_only:
             self._v = None  # depends on self.curves
             self._r = None  # depends on self.pre_curves and self.instruments
+            self._r_pre = None  # depends on pre_solvers and self.r
             self._x = None  # depends on self.r, self.s
             self._g = None  # depends on self.x, self.weights
             self._J = None  # depends on self.r
             self._grad_s_vT = None  # final_iter_dual: depends on self.s and iteration
             # fixed_point_iter: depends on self.f
             # final_iter_anal: depends on self.J
             self._grad_s_vT_pre = None  # depends on self.grad_s_vT and pre_solvers.
@@ -1167,14 +1163,34 @@
         """
         if self._r is None:
             self._r = np.array([_[0].rate(*_[1], **_[2]) for _ in self.instruments])
             # solver and fx are passed by default via parse_args to get string curves
         return self._r
 
     @property
+    def r_pre(self):
+        if len(self.pre_solvers) == 0:
+            return self.r
+
+        if self._r_pre is None:
+            r_pre = np.empty(self.pre_m, dtype="object")
+
+            i = 0
+            for pre_solver in self.pre_solvers:
+
+                m = pre_solver.pre_m
+                r_pre[i : i + m] = pre_solver.r_pre
+                i = i + m
+
+            # create bottom right block
+            r_pre[-self.m :] = self.r
+            self._r_pre = r_pre
+        return self._r_pre
+
+    @property
     def x(self):
         """
         1d array of error in each calibrating instrument rate, of size (m,).
 
         .. math::
 
            \\mathbf{x} = \\mathbf{r-S}
@@ -1193,24 +1209,18 @@
 
         Returns
         -------
         Series
         """
         s = None
         for pre_solver in self.pre_solvers:
-            _ = Series(
-                pre_solver.x.astype(float) * 100 / self.rate_scalars,
-                index=MultiIndex.from_tuples(
-                    [(pre_solver.id, inst) for inst in pre_solver.instrument_labels]
-                ),
-            )
             if s is None:
-                s = _
+                s = pre_solver.error
             else:
-                s = concat([s, _])
+                s = concat([pre_solver.error, s])
 
         _ = Series(
             self.x.astype(float) * 100 / self.rate_scalars,
             index=MultiIndex.from_tuples(
                 [(self.id, inst) for inst in self.instrument_labels]
             ),
         )
@@ -1479,15 +1489,15 @@
 
         if base is not None:
             df.loc[r_idx, ("all", base)] = df.loc[r_idx, (slice(None), base)].sum(
                 axis=1
             )
 
         sorted_cols = df.columns.sort_values()
-        return df.loc[:, sorted_cols]
+        return df.loc[:, sorted_cols].astype("float64")
 
     def _get_base_and_fx(self, base, fx):
         if base is not None and self.fx is None and fx is None:
             raise ValueError(
                 "`base` is given but `fx` is not and Solver does not "
                 "contain an attached FXForwards object."
             )
@@ -1527,15 +1537,17 @@
         DataFrame
 
         Notes
         -----
         .. note::
 
            *Instrument* values are scaled to 1bp (1/10000th of a unit) when they are
-           rate based. *FX* values are scaled to pips (1/10000th of an FX unit).
+           rate based.
+
+           *FX* values are scaled to pips (1/10000th of an FX unit).
 
         The output ``DataFrame`` has the following structure:
 
         - A 5-level index by *'local_ccy'*, *'display_ccy'*, *'type'*, *'solver'*,
           and *'label'*;
 
           - **local_ccy** displays the currency for which cashflows are payable, and
@@ -1550,14 +1562,89 @@
             ``instrument_labels``.
 
         - A 3-level column header index using the last three levels of the above;
 
         Converting a gamma/delta from a local currency to another ``base`` currency also
         introduces FX risk to the NPV of the instrument, which is included in the
         output.
+
+        Examples
+        --------
+        This example replicates the analytical calculations demonstrated in
+        *Pricing and Trading Interest Rate Derivatives (2022)*, derived from
+        first principles.
+        The results are stated in the cross-gamma grid in figure 22.1.
+
+        .. ipython:: python
+
+           curve_r = Curve(
+               nodes={
+                   dt(2022, 1, 1): 1.0,
+                   dt(2023, 1, 1): 0.99,
+                   dt(2024, 1, 1): 0.98,
+                   dt(2025, 1, 1): 0.97,
+                   dt(2026, 1, 1): 0.96,
+                   dt(2027, 1, 1): 0.95,
+               },
+               id="r"
+           )
+           curve_z = Curve(
+               nodes={
+                   dt(2022, 1, 1): 1.0,
+                   dt(2023, 1, 1): 0.99,
+                   dt(2024, 1, 1): 0.98,
+                   dt(2025, 1, 1): 0.97,
+                   dt(2026, 1, 1): 0.96,
+                   dt(2027, 1, 1): 0.95,
+               },
+               id="z"
+           )
+           curve_s = Curve(
+               nodes={
+                   dt(2022, 1, 1): 1.0,
+                   dt(2023, 1, 1): 0.99,
+                   dt(2024, 1, 1): 0.98,
+                   dt(2025, 1, 1): 0.97,
+                   dt(2026, 1, 1): 0.96,
+                   dt(2027, 1, 1): 0.95,
+               },
+               id="s"
+           )
+           args = dict(termination="1Y", frequency="A", fixing_method="ibor", leg2_fixing_method="ibor")
+           instruments = [
+               SBS(dt(2022, 1, 1), curves=["r", "s", "s", "s"], **args),
+               SBS(dt(2023, 1, 1), curves=["r", "s", "s", "s"], **args),
+               SBS(dt(2024, 1, 1), curves=["r", "s", "s", "s"], **args),
+               SBS(dt(2025, 1, 1), curves=["r", "s", "s", "s"], **args),
+               SBS(dt(2026, 1, 1), curves=["r", "s", "s", "s"], **args),
+               SBS(dt(2022, 1, 1), curves=["r", "s", "z", "s"], **args),
+               SBS(dt(2023, 1, 1), curves=["r", "s", "z", "s"], **args),
+               SBS(dt(2024, 1, 1), curves=["r", "s", "z", "s"], **args),
+               SBS(dt(2025, 1, 1), curves=["r", "s", "z", "s"], **args),
+               SBS(dt(2026, 1, 1), curves=["r", "s", "z", "s"], **args),
+               IRS(dt(2022, 1, 1), "1Y", "A", curves=["r", "s"], leg2_fixing_method="ibor"),
+               IRS(dt(2023, 1, 1), "1Y", "A", curves=["r", "s"], leg2_fixing_method="ibor"),
+               IRS(dt(2024, 1, 1), "1Y", "A", curves=["r", "s"], leg2_fixing_method="ibor"),
+               IRS(dt(2025, 1, 1), "1Y", "A", curves=["r", "s"], leg2_fixing_method="ibor"),
+               IRS(dt(2026, 1, 1), "1Y", "A", curves=["r", "s"], leg2_fixing_method="ibor"),
+           ]
+           solver = Solver(
+               curves=[curve_r, curve_s, curve_z],
+               instruments=instruments,
+               s=[0.]*5 + [0.]*5 + [1.5]*5,
+               id="sonia",
+               instrument_labels=[
+                   "s1", "s2", "s3", "s4", "s5",
+                   "z1", "z2", "z3", "z4", "z5",
+                   "r1", "r2", "r3", "r4", "r5",
+               ],
+           )
+           irs = IRS(dt(2022, 1, 1), "5Y", "A", notional=-8.3e8, curves=["z", "s"], leg2_fixing_method="ibor", fixed_rate=25.0)
+           irs.delta(solver=solver)
+           irs.gamma(solver=solver)
         """
         if self._ad != 2:
             raise ValueError("`Solver` must be in ad order 2 to use `gamma` method.")
 
         # new
         base, fx = self._get_base_and_fx(base, fx)
         fx_vars = tuple() if fx is None else fx.variables
@@ -1648,15 +1735,15 @@
                 df.loc[(currencies, base, slice(None), slice(None), slice(None)), :]
                 .groupby(level=[2, 3, 4])
                 .sum()
             )
             gdf.index = MultiIndex.from_tuples([("all", base) + l for l in gdf.index])
             df.loc[("all", base, slice(None), slice(None), slice(None))] = gdf
 
-        return df
+        return df.astype("float64")
 
     def _pnl_explain(self, npv, ds, dfx=None, base=None, fx=None, order=1):
         """
         Calculate PnL from market movements over delta and, optionally, gamma.
 
         Parameters
         ----------
```

### Comparing `rateslib-0.2.0/rateslib/splines.py` & `rateslib-0.3.0/rateslib/splines.py`

 * *Files identical despite different names*

### Comparing `rateslib-0.2.0/rateslib.egg-info/PKG-INFO` & `rateslib-0.3.0/rateslib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rateslib
-Version: 0.2.0
+Version: 0.3.0
 Summary: A fixed income library for trading interest rates
 Author: J H M Darbyshire
 License: Attribution-NonCommercial-NoDerivatives 4.0 International
         
         =======================================================================
         
         Creative Commons Corporation ("Creative Commons") is not a law firm and
```

### Comparing `rateslib-0.2.0/rateslib.egg-info/SOURCES.txt` & `rateslib-0.3.0/rateslib.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 rateslib/__init__.py
+rateslib/_swaptions.py
 rateslib/calendars.py
 rateslib/curves.py
 rateslib/default.py
 rateslib/dual.py
 rateslib/fx.py
 rateslib/instruments.py
 rateslib/legs.py
```

### Comparing `rateslib-0.2.0/tests/test_calendars.py` & `rateslib-0.3.0/tests/test_calendars.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,15 +211,17 @@
 @pytest.mark.parametrize("start, end, conv, expected", [
     (dt(2022, 1, 1), dt(2022, 4, 1), "ACT365F", 0.2465753424657534),
     (dt(2022, 1, 1), dt(2022, 4, 1), "1", 1.0),
     (dt(2022, 1, 1), dt(2022, 4, 1), "ACT360", 0.2465753424657534 * 365 / 360),
     (dt(2022, 1, 1), dt(2022, 4, 1), "30360", 0.250),
     (dt(2022, 1, 1), dt(2022, 4, 1), "30E360", 0.250),
     (dt(2022, 1, 1), dt(2022, 4, 1), "ACTACT", 0.2465753424657534),
-    (dt(2022, 1, 1), dt(2022, 1, 1), "ACTACT", 0.0)
+    (dt(2022, 1, 1), dt(2022, 1, 1), "ACTACT", 0.0),
+    (dt(2022, 1, 1), dt(2023, 1, 31), "1+", 1.0),
+    (dt(2022, 1, 1), dt(2024, 2, 28), "1+", 2 + 1/12),
 ])
 def test_dcf(start, end, conv, expected):
     result = dcf(start, end, conv)
     assert result == expected
 
 
 @pytest.mark.parametrize("start, end, conv, expected, freq_m, term, stub", [
```

### Comparing `rateslib-0.2.0/tests/test_curves.py` & `rateslib-0.3.0/tests/test_curves.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 import pytest
 from datetime import datetime as dt
 from pandas import DataFrame
 import numpy as np
 from math import log, exp
+from matplotlib import pyplot as plt
 
 import context
-from rateslib.curves import Curve, LineCurve, index_left, interpolate, IndexCurve
+from rateslib.curves import (
+    Curve,
+    LineCurve,
+    index_left,
+    interpolate,
+    IndexCurve,
+    CompositeCurve,
+)
+from rateslib import default_context
 from rateslib.dual import Dual, Dual2
 from rateslib.calendars import get_calendar
 
 
 @pytest.fixture()
 def curve():
     return Curve(
@@ -89,14 +98,32 @@
 
 
 def test_line_curve_rate(line_curve):
     expected = Dual(2.005, ["v0", "v1"], np.array([0.5, 0.5]))
     assert line_curve.rate(effective=dt(2022, 3, 16)) == expected
 
 
+@pytest.mark.parametrize("scm, exp", [
+    ("none_simple", 5.56617834937),
+    ("isda_flat_compounding", 5.57234801943),
+    ("isda_compounding", 5.58359355318),
+])
+def test_curve_rate_floating_spread(scm, exp):
+    curve = Curve({dt(2022, 1, 1): 1.0, dt(2022, 2, 1): 0.9985, dt(2022, 3, 1): 0.995})
+    result = curve.rate(dt(2022, 1, 1), dt(2022, 3, 1), None, 250, scm)
+    assert (result - exp) < 1e-8
+
+
+def test_curve_rate_raises(curve):
+    with pytest.raises(ValueError, match="Must supply a valid `spread_compound"):
+        curve.rate(
+            dt(2022, 3, 3), "7d", float_spread=10.0, spread_compound_method="bad"
+        )
+
+
 @pytest.mark.parametrize("li, ll, val, expected", [
     ([0, 1, 2, 3, 4], 5, 0, 0),
     ([0, 1, 2, 3, 4], 5, 0.5, 0),
     ([0, 1, 2, 3, 4], 5, 1, 0),
     ([0, 1, 2, 3, 4], 5, 1.5, 1),
     ([0, 1, 2, 3, 4], 5, 2, 1),
     ([0, 1, 2, 3, 4], 5, 2.5, 2),
@@ -115,14 +142,15 @@
     # test calcs without raise
     curve_zero = Curve(
         nodes={dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99,
                dt(2024, 1, 1): 0.979, dt(2025, 1, 1): 0.967},
         interpolation="linear_zero_rate",
     )
     curve_zero.plot("1d")
+    plt.close("all")
 
 
 def test_curve_equality_type_differ(curve, line_curve):
     assert curve != line_curve
 
 
 def test_serialization(curve):
@@ -474,14 +502,23 @@
         result_curve.rate(_, "1D") - curve.rate(_, "1D") - 0.25 for _ in [
             dt(2022, 1, 10), dt(2023, 3, 24), dt(2024, 11, 11), dt(2026, 4, 5)
         ]
     ])
     assert np.all(np.abs(diff) < 1e-7)
 
 
+def test_composite_curve_shift():
+    c1 = Curve({dt(2022, 1, 1): 1.0, dt(2022, 2, 1): 0.999})
+    c2 = Curve({dt(2022, 1, 1): 1.0, dt(2022, 2, 1): 0.998})
+    cc = CompositeCurve([c1, c2])
+    result = cc.shift(20).rate(dt(2022, 1, 1), "1d")
+    expected = c1.rate(dt(2022, 1, 1), "1d") + c2.rate(dt(2022, 1, 1), "1d") + 0.2
+    assert abs(result - expected) < 1e-3
+
+
 @pytest.mark.parametrize("ad_order", [0, 1, 2])
 def test_linecurve_shift(ad_order):
     curve = LineCurve(
         nodes={
             dt(2022, 1, 1): 1.0,
             dt(2023, 1, 1): 0.988,
             dt(2024, 1, 1): 0.975,
@@ -728,103 +765,456 @@
 
 
 def test_curve_roll_copy(curve):
     result = curve.roll("0d")
     assert result == curve
 
 
-def test_curve_translate_raises(curve):
-    with pytest.raises(ValueError, match="Cannot translate exactly for the given"):
-        curve.translate(dt(2022, 4, 1))
-
-
-def test_curve_translate_knots_raises(curve):
-    curve = Curve(
+def test_index_curve_roll():
+    crv = IndexCurve(
         nodes={
             dt(2022, 1, 1): 1.0,
             dt(2023, 1, 1): 0.988,
             dt(2024, 1, 1): 0.975,
             dt(2025, 1, 1): 0.965,
             dt(2026, 1, 1): 0.955,
-            dt(2027, 1, 1): 0.9475
+            dt(2027, 1, 1): 0.9475,
         },
-        t=[dt(2022, 1, 1), dt(2022, 1, 1), dt(2022, 1, 1), dt(2022, 1, 1),
-           dt(2022, 12, 1),
-           dt(2024, 1, 1),
-           dt(2025, 1, 1),
-           dt(2026, 1, 1),
-           dt(2027, 1, 1), dt(2027, 1, 1), dt(2027, 1, 1), dt(2027, 1, 1),
+        t=[
+            dt(2024, 1, 1), dt(2024, 1, 1), dt(2024, 1, 1), dt(2024, 1, 1),
+            dt(2025, 1, 1),
+            dt(2026, 1, 1),
+            dt(2027, 1, 1), dt(2027, 1, 1), dt(2027, 1, 1), dt(2027, 1, 1),
         ],
+        index_base=110.0,
+        interpolation="log_linear",
     )
-    with pytest.raises(ValueError, match="Cannot translate spline knots for given"):
-        curve.translate(dt(2022, 12, 15))
+    rolled_curve = crv.roll("10d")
+    rolled_curve2 = crv.roll("-10d")
+
+    expected = np.array([crv.rate(_, "1D") for _ in [
+        dt(2023, 1, 15), dt(2023, 3, 15), dt(2024, 11, 15), dt(2026, 4, 15)
+    ]
+                         ])
+    result = np.array([rolled_curve.rate(_, "1D") for _ in [
+        dt(2023, 1, 25), dt(2023, 3, 25), dt(2024, 11, 25), dt(2026, 4, 25)
+    ]
+                       ])
+    result2 = np.array([rolled_curve2.rate(_, "1D") for _ in [
+        dt(2023, 1, 5), dt(2023, 3, 5), dt(2024, 11, 5), dt(2026, 4, 5)
+    ]
+                        ])
+    assert np.all(np.abs(result - expected) < 1e-7)
+    assert np.all(np.abs(result2 - expected) < 1e-7)
+    assert rolled_curve.index_base == crv.index_base
 
 
-def test_curve_index_linear_daily_interp():
-    curve = IndexCurve(
-        nodes={dt(2022, 1, 1): 1.0, dt(2022, 1, 5): 0.9999},
-        index_base=200.0,
-    )
-    result = curve.index_value(dt(2022, 1, 5))
-    expected = 200.020002002
-    assert abs(result - expected) < 1e-7
+def test_curve_translate_raises(curve):
+    with pytest.raises(ValueError, match="Cannot translate into the past."):
+        curve.translate(dt(2020, 4, 1))
+
+
+class TestIndexCurve:
+
+    def test_curve_translate_knots_raises(self, curve):
+        curve = Curve(
+            nodes={
+                dt(2022, 1, 1): 1.0,
+                dt(2023, 1, 1): 0.988,
+                dt(2024, 1, 1): 0.975,
+                dt(2025, 1, 1): 0.965,
+                dt(2026, 1, 1): 0.955,
+                dt(2027, 1, 1): 0.9475
+            },
+            t=[dt(2022, 1, 1), dt(2022, 1, 1), dt(2022, 1, 1), dt(2022, 1, 1),
+               dt(2022, 12, 1),
+               dt(2024, 1, 1),
+               dt(2025, 1, 1),
+               dt(2026, 1, 1),
+               dt(2027, 1, 1), dt(2027, 1, 1), dt(2027, 1, 1), dt(2027, 1, 1),
+            ],
+        )
+        with pytest.raises(ValueError, match="Cannot translate spline knots for given"):
+            curve.translate(dt(2022, 12, 15))
+
+    def test_curve_index_linear_daily_interp(self):
+        curve = IndexCurve(
+            nodes={dt(2022, 1, 1): 1.0, dt(2022, 1, 5): 0.9999},
+            index_base=200.0,
+        )
+        result = curve.index_value(dt(2022, 1, 5))
+        expected = 200.020002002
+        assert abs(result - expected) < 1e-7
+
+        result = curve.index_value(dt(2022, 1, 3))
+        expected = 200.010001001  # value is linearly interpolated between index values.
+        assert abs(result - expected) < 1e-7
+
+    def test_indexcurve_raises(self):
+        with pytest.raises(ValueError, match="`index_base` must be given"):
+            curve = IndexCurve({dt(2022, 1, 1): 1.0})
+
+    def test_index_value_raises(self):
+        curve = IndexCurve({dt(2022, 1, 1): 1.0}, index_base=100.0)
+        with pytest.raises(ValueError, match="`interpolation` for `index_value`"):
+            curve.index_value(dt(2022, 1, 1), interpolation="BAD")
+
+    def test_roll_preserves_ad(self):
+        curve = IndexCurve(
+            {dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99},
+            index_base=100.0,
+            index_lag=3,
+            id="tags_",
+            ad=1,
+        )
+        new_curve = curve.roll("1m")
+        pass
+
+
+class TestCompositeCurve:
+
+    def test_curve_df_based(self):
+        curve1 = Curve(
+            nodes={
+                dt(2022, 1, 1): 1.0,
+                dt(2023, 1, 1): 0.98,
+                dt(2024, 1, 1): 0.965,
+                dt(2025, 1, 1): 0.955
+            },
+            t=[dt(2023, 1, 1), dt(2023, 1, 1), dt(2023, 1, 1), dt(2023, 1, 1),
+               dt(2024, 1, 1),
+               dt(2025, 1, 1), dt(2025, 1, 1), dt(2025, 1, 1), dt(2025, 1, 1)],
+        )
+        curve2 = Curve(
+            nodes={
+                dt(2022, 1, 1): 1.0,
+                dt(2022, 6, 30): 1.0,
+                dt(2022, 7, 1): 0.999992,
+                dt(2022, 12, 31): 0.999992,
+                dt(2023, 1, 1): 0.999984,
+                dt(2023, 6, 30): 0.999984,
+                dt(2023, 7, 1): 0.999976,
+                dt(2023, 12, 31): 0.999976,
+                dt(2024, 1, 1): 0.999968,
+                dt(2024, 6, 30): 0.999968,
+                dt(2024, 7, 1): 0.999960,
+                dt(2025, 1, 1): 0.999960,
+            },
+        )
+        curve = CompositeCurve([curve1, curve2])
+
+        result1 = curve.rate(dt(2022, 12, 30), "1d")
+        result2 = curve.rate(dt(2022, 12, 31), "1d")
+        result3 = curve.rate(dt(2023, 1, 1), "1d")
+
+        expected1 = curve.rate(dt(2022, 12, 30), "1d", approximate=False)
+        expected2 = curve.rate(dt(2022, 12, 31), "1d", approximate=False)
+        expected3 = curve.rate(dt(2023, 1, 1), "1d", approximate=False)
+
+        assert abs(result1 - expected1) < 1e-9
+        assert abs(result2 - expected2) < 1e-9
+        assert abs(result3 - expected3) < 1e-9
+
+        result = curve.rate(dt(2022, 6, 1), "1Y")
+        expected = curve.rate(dt(2022, 6, 1), "1Y", approximate=False)
+        assert abs(result - expected) < 1e-4
+
+    def test_composite_curve_translate(self):
+        curve1 = Curve(
+            nodes={
+                dt(2022, 1, 1): 1.0,
+                dt(2023, 1, 1): 0.98,
+                dt(2024, 1, 1): 0.965,
+                dt(2025, 1, 1): 0.955
+            },
+            t=[dt(2023, 1, 1), dt(2023, 1, 1), dt(2023, 1, 1), dt(2023, 1, 1),
+               dt(2024, 1, 1),
+               dt(2025, 1, 1), dt(2025, 1, 1), dt(2025, 1, 1), dt(2025, 1, 1)],
+        )
+        curve2 = Curve(
+            nodes={
+                dt(2022, 1, 1): 1.0,
+                dt(2022, 6, 30): 1.0,
+                dt(2022, 7, 1): 0.999992,
+                dt(2022, 12, 31): 0.999992,
+                dt(2023, 1, 1): 0.999984,
+                dt(2023, 6, 30): 0.999984,
+                dt(2023, 7, 1): 0.999976,
+                dt(2023, 12, 31): 0.999976,
+                dt(2024, 1, 1): 0.999968,
+                dt(2024, 6, 30): 0.999968,
+                dt(2024, 7, 1): 0.999960,
+                dt(2025, 1, 1): 0.999960,
+            },
+        )
+        crv = CompositeCurve([curve1, curve2])
+
+        result_curve = crv.translate(dt(2022, 3, 1))
+        diff = np.array([
+            result_curve.rate(_, "1D") - crv.rate(_, "1D") for _ in [
+                dt(2023, 1, 25), dt(2023, 3, 24), dt(2024, 11, 11), dt(2026, 4, 5)
+            ]
+        ])
+        assert np.all(np.abs(diff) < 1e-5)
+
+    def test_composite_curve_roll(self):
+        curve1 = Curve(
+            nodes={
+                dt(2022, 1, 1): 1.0,
+                dt(2023, 1, 1): 0.98,
+                dt(2024, 1, 1): 0.965,
+                dt(2025, 1, 1): 0.955
+            },
+            t=[dt(2023, 1, 1), dt(2023, 1, 1), dt(2023, 1, 1), dt(2023, 1, 1),
+               dt(2024, 1, 1),
+               dt(2025, 1, 1), dt(2025, 1, 1), dt(2025, 1, 1), dt(2025, 1, 1)],
+        )
+        curve2 = Curve(
+            nodes={
+                dt(2022, 1, 1): 1.0,
+                dt(2022, 6, 30): 1.0,
+                dt(2022, 7, 1): 0.999992,
+                dt(2022, 12, 31): 0.999992,
+                dt(2023, 1, 1): 0.999984,
+                dt(2023, 6, 30): 0.999984,
+                dt(2023, 7, 1): 0.999976,
+                dt(2023, 12, 31): 0.999976,
+                dt(2024, 1, 1): 0.999968,
+                dt(2024, 6, 30): 0.999968,
+                dt(2024, 7, 1): 0.999960,
+                dt(2025, 1, 1): 0.999960,
+            },
+        )
+        crv = CompositeCurve([curve1, curve2])
+
+        rolled_curve = crv.roll("10d")
+        expected = np.array([crv.rate(_, "1D") for _ in [
+            dt(2023, 1, 15), dt(2023, 3, 15), dt(2024, 11, 15), dt(2026, 4, 15)
+        ]
+                             ])
+        result = np.array([rolled_curve.rate(_, "1D") for _ in [
+            dt(2023, 1, 25), dt(2023, 3, 25), dt(2024, 11, 25), dt(2026, 4, 25)
+        ]
+        ])
+
+        assert np.all(np.abs(result - expected) < 1e-7)
+
+    def test_isinstance_raises(self):
+        curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99})
+        line_curve = LineCurve({dt(2022, 1, 1): 10.0, dt(2023, 1, 1): 12.0})
+        with pytest.raises(TypeError, match="`curves` must be a list of"):
+            CompositeCurve([curve, line_curve])
+
+    @pytest.mark.parametrize("attribute, val", [
+        ("modifier", ["MF", "MP"]),
+        ("calendar", ["ldn", "tgt"]),
+        ("convention", ["act360", "act365f"])
+    ])
+    def test_attribute_error_raises(self, attribute, val):
+        c1 = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99}, **{attribute: val[0]})
+        c2 = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99}, **{attribute: val[1]})
+        with pytest.raises(ValueError, match="Cannot composite curves with dif"):
+            CompositeCurve([c1, c2])
+
+    def test_line_based(self):
+        c1 = LineCurve({dt(2022, 1, 1): 1.5, dt(2022, 1, 3): 1.0})
+        c2 = LineCurve({dt(2022, 1, 1): 2.0, dt(2022, 1, 3): 3.0})
+        cc = CompositeCurve([c1, c2])
+        expected = 3.75
+        result = cc.rate(dt(2022, 1, 2))
+        assert abs(result - expected) < 1e-8
+
+        result = cc[dt(2022, 1, 2)]
+        assert abs(result - expected) < 1e-8
+
+    def test_initial_node_raises(self):
+        c1 = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99})
+        c2 = Curve({dt(2022, 1, 2): 1.0, dt(2023, 1, 1): 0.99})
+        with pytest.raises(ValueError, match="`curves` must share the same ini"):
+            CompositeCurve([c1, c2])
+
+    @pytest.mark.parametrize("lag, base", [
+        ([2, 3], [100.0, 100.0]),
+        ([3, 3], [100.0, 100.001])
+    ])
+    def test_index_curves_raises(self, lag, base):
+        ic1 = IndexCurve(
+            {dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99},
+            index_lag=lag[0],
+            index_base=base[0]
+        )
+        ic2 = IndexCurve(
+            {dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99},
+            index_lag=lag[1],
+            index_base=base[1]
+        )
+        with pytest.raises(ValueError, match="Cannot composite curves with different"):
+            CompositeCurve([ic1, ic2])
 
-    result = curve.index_value(dt(2022, 1, 3))
-    expected = 200.010001001  # value is linearly interpolated between index values.
-    assert abs(result - expected) < 1e-7
+    def test_index_curves_attributes(self):
+        ic1 = IndexCurve(
+            {dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99},
+            index_lag=3,
+            index_base=101.1
+        )
+        ic2 = IndexCurve(
+            {dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99},
+            index_lag=3,
+            index_base=101.1
+        )
+        cc = CompositeCurve([ic1, ic2])
+        assert cc.index_lag == 3
+        assert cc.index_base == 101.1
+
+    def test_multi_csa(self):
+        c1 = Curve(
+            {
+                dt(2022, 1, 1): 1.0,
+                dt(2022, 1, 2): 0.99997260,  # 1%
+                dt(2022, 1, 3): 0.99991781,  # 2%
+                dt(2022, 1, 4): 0.99983564,  # 3%
+                dt(2022, 1, 5): 0.99972608,  # 4%
+             },
+            convention="Act365F",
+        )
+        c2 = Curve(
+            {
+                dt(2022, 1, 1): 1.0,
+                dt(2022, 1, 2): 0.99989042,  # 4%
+                dt(2022, 1, 3): 0.99980825,  # 3%
+                dt(2022, 1, 4): 0.99975347,  # 2%
+                dt(2022, 1, 5): 0.99972608,  # 1%
+            },
+            convention="Act365F",
+        )
+        c3 = Curve(
+            {
+                dt(2022, 1, 1): 1.0,
+                dt(2022, 1, 2): 0.99989042,  # 4%
+                dt(2022, 1, 3): 0.99979455,  # 3.5%
+                dt(2022, 1, 4): 0.99969869,  # 3.5%
+                dt(2022, 1, 5): 0.99958915,  # 4%
+            },
+            convention="Act365F",
+        )
+        cc = CompositeCurve([c1, c2, c3], multi_csa=True)
+        with default_context("multi_csa_granularity", 1):
+            r1 = cc.rate(dt(2022, 1, 1), "1d")
+            r2 = cc.rate(dt(2022, 1, 2), "1d")
+            r3 = cc.rate(dt(2022, 1, 3), "1d")
+            r4 = cc.rate(dt(2022, 1, 4), "1d")
+
+        assert abs(r1 - 4.0) < 1e-3
+        assert abs(r2 - 3.5) < 1e-3
+        assert abs(r3 - 3.5) < 1e-3
+        assert abs(r4 - 4.0) < 1e-3
+
+    def test_multi_csa_granularity(self):
+        c1 = Curve({dt(2022, 1, 1): 1.0, dt(2032, 1, 1): 0.9, dt(2072, 1, 1): 0.5})
+        c2 = Curve({dt(2022, 1, 1): 1.0, dt(2032, 1, 1): 0.8, dt(2072, 1, 1): 0.7})
+        cc = CompositeCurve(
+            [c1, c2], multi_csa=True, multi_csa_max_step=182, multi_csa_min_step=182
+        )
 
+        r1 = cc.rate(dt(2052, 5, 24), "1d")
+        r2 = cc.rate(dt(2052, 5, 25), "1d")
+        r3 = cc.rate(dt(2052, 5, 26), "1d")
 
-def test_indexcurve_raises():
-    with pytest.raises(ValueError, match="`index_base` must be given"):
-        curve = IndexCurve({dt(2022, 1, 1): 1.0})
+        assert abs(r1 - 1.448374) < 1e-3
 
 
 class TestPlotCurve:
 
     def test_plot_curve(self, curve):
         fig, ax, lines = curve.plot("1d")
         result = lines[0].get_data()
         assert result[0][0] == dt(2022, 3, 1)
         assert abs(result[1][0].real - 12.004001333774994) < 1e-6
+        plt.close("all")
 
     def test_plot_linecurve(self, line_curve):
         fig, ax, lines = line_curve.plot("0d")
         result = lines[0].get_data()
         assert result[0][0] == dt(2022, 3, 1)
         assert abs(result[1][0].real - 2.0) < 1e-6
+        plt.close("all")
 
     @pytest.mark.parametrize("left", ["1d", dt(2022, 3, 2)])
     def test_plot_curve_left(self, curve, left):
         fig, ax, lines = curve.plot("1d", left=left)
         result = lines[0].get_data()
         assert result[0][0] == dt(2022, 3, 2)
         assert abs(result[1][0].real - 12.008005336896055) < 1e-6
+        plt.close("all")
 
     def test_plot_curve_left_raise(self, curve):
         with pytest.raises(ValueError, match="`left` must be supplied as"):
             fig, ax, lines = curve.plot("1d", left=100.3)
+        plt.close("all")
 
     @pytest.mark.parametrize("right", ["2d", dt(2022, 3, 3)])
     def test_plot_curve_right(self, curve, right):
         fig, ax, lines = curve.plot("1d", right=right)
         result = lines[0].get_data()
         assert result[0][-1] == dt(2022, 3, 2)
         assert abs(result[1][-1].real - 12.008005336896055) < 1e-6
+        plt.close("all")
 
     def test_plot_curve_right_raise(self, curve):
         with pytest.raises(ValueError, match="`right` must be supplied as"):
             fig, ax, lines = curve.plot("1d", right=100.3)
+        plt.close("all")
 
     def test_plot_comparators(self, curve):
         fig, ax, lines = curve.plot("1d", comparators=[curve])
         assert len(lines) == 2
         res1 = lines[0].get_data()
         res2 = lines[1].get_data()
         assert res1[0][0] == res2[0][0]
         assert res1[1][0] == res2[1][0]
+        plt.close("all")
 
     def test_plot_diff(self, curve):
         fig, ax, lines = curve.plot("1d", comparators=[curve], difference=True)
         assert len(lines) == 1
         result = lines[0].get_data()
         assert result[0][0] == dt(2022, 3, 1)
-        assert result[1][0] == 0
+        assert result[1][0] == 0
+        plt.close("all")
+
+    @pytest.mark.parametrize("left", [None, dt(2022, 1, 1), "0d"])
+    @pytest.mark.parametrize("right", [None, dt(2022, 2, 1), "0d"])
+    def test_plot_index(self, left, right):
+        i_curve = IndexCurve({dt(2022, 1, 1): 1.0, dt(2022, 2, 1): 1.0}, index_base=2.0)
+        fig, ax, lines = i_curve.plot_index(left=left, right=right)
+        result = lines[0].get_data()
+        assert result[0][0] == dt(2022, 1, 1)
+        assert abs(result[1][0].real - 2.0) < 1e-6
+        plt.close("all")
+
+    def test_plot_index_comparators(self):
+        i_curve = IndexCurve({dt(2022, 1, 1): 1.0, dt(2022, 2, 1): 1.0}, index_base=2.0)
+        i_curv2 = IndexCurve({dt(2022, 1, 1): 1.0, dt(2022, 2, 1): 1.0}, index_base=2.0)
+        fig, ax, lines = i_curve.plot_index(comparators=[i_curv2])
+        assert len(lines) == 2
+        res1 = lines[0].get_data()
+        res2 = lines[1].get_data()
+        assert res1[0][0] == res2[0][0]
+        assert res1[1][0] == res2[1][0]
+        plt.close("all")
+
+    def test_plot_index_diff(self):
+        i_curv = IndexCurve({dt(2022, 1, 1): 1.0, dt(2022, 2, 1): 1.0}, index_base=2.0)
+        i_curv2 = IndexCurve({dt(2022, 1, 1): 1.0, dt(2022, 2, 1): 1.0}, index_base=2.0)
+        fig, ax, lines = i_curv.plot_index("1d", comparators=[i_curv2], difference=True)
+        assert len(lines) == 1
+        result = lines[0].get_data()
+        assert result[0][0] == dt(2022, 1, 1)
+        assert result[1][0] == 0
+        plt.close("all")
+
+    def test_plot_index_raises(self):
+        i_curve = IndexCurve({dt(2022, 1, 1): 1.0, dt(2022, 2, 1): 1.0}, index_base=2.0)
+        with pytest.raises(ValueError, match="`left` must be supplied as"):
+            i_curve.plot_index(left=2.0)
+        with pytest.raises(ValueError, match="`right` must be supplied as"):
+            i_curve.plot_index(right=2.0)
```

### Comparing `rateslib-0.2.0/tests/test_dual.py` & `rateslib-0.3.0/tests/test_dual.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,14 +223,19 @@
 
 @pytest.mark.parametrize("op", ["__add__", "__sub__", "__mul__", "__truediv__"])
 def test_dual_immutable(x_1, op):
     _ = getattr(x_1, op)(Dual(2, vars=["new"], dual=np.array([4])))
     assert x_1 == Dual(1, vars=["v0", "v1"], dual=np.array([1, 2]))
 
 
+def test_dual_raises(x_1):
+    with pytest.raises(ValueError, match="`Dual` variable cannot possess `dual2`"):
+        x_1.dual2
+
+
 @pytest.mark.parametrize("op, expected", [
     ("__add__", Dual(3, vars=["v0", "v1", "v2"], dual=np.array([1, 2, 3]))),
     ("__sub__", Dual(-1, vars=["v0", "v1", "v2"], dual=np.array([1, 2, -3]))),
     ("__mul__", Dual(2, vars=["v0", "v1", "v2"], dual=np.array([2, 4, 3]))),
     ("__truediv__", Dual(0.5, vars=["v0", "v1", "v2"], dual=np.array([0.5, 1, -0.75]))),
 ])
 def test_ops(x_1, x_2, op, expected):
```

### Comparing `rateslib-0.2.0/tests/test_fx.py` & `rateslib-0.3.0/tests/test_fx.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytest
 from datetime import datetime as dt
+from matplotlib import pyplot as plt
 from pandas import DataFrame
 from pandas.testing import assert_frame_equal
 import numpy as np
 
 import context
 from rateslib.fx import (
     FXForwards,
@@ -532,14 +533,15 @@
             "eurusd": eurusd,
         }
     )
     result = fxf.plot("eurusd", left=left, right=right)
     assert len(result) == 3
     y_data = result[2][0].get_data()[1]
     assert abs(float(y_data[8]) - 0.9520631477714822) < 1e-10
+    plt.close("all")
 
 
 def test_delta_risk_equivalence():
     start, end = dt(2022, 1, 1), dt(2023, 1, 1)
     fx_curves = {
         "usdusd": Curve({start: 1.0, end: 0.96}, id="uu", ad=1),
         "eureur": Curve({start: 1.0, end: 0.99}, id="ee", ad=1),
```

### Comparing `rateslib-0.2.0/tests/test_instruments.py` & `rateslib-0.3.0/tests/test_instruments.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,45 +3,68 @@
 from pandas import DataFrame, date_range, Series, Index, MultiIndex
 from pandas.testing import assert_frame_equal
 import numpy as np
 
 import context
 from rateslib import defaults, default_context
 from rateslib.instruments import (
-    IRS, forward_fx, SBS, FXSwap, NonMtmXCS, FixedRateBond, Bill, Value,
-    _get_curve_from_solver, BaseMixin, FloatRateBond, FRA, BondFuture,
-    NonMtmFixedFloatXCS, NonMtmFixedFixedXCS, XCS, FixedFloatXCS, FixedFixedXCS, FloatFixedXCS,
-    Portfolio, Spread, Fly, _get_curves_and_fx_maybe_from_solver
+    IRS,
+    IIRS,
+    forward_fx,
+    SBS,
+    FXSwap,
+    NonMtmXCS,
+    FixedRateBond,
+    Bill,
+    Value,
+    ZCS,
+    ZCIS,
+    _get_curve_from_solver,
+    BaseMixin,
+    FloatRateBond,
+    FRA,
+    BondFuture,
+    IndexFixedRateBond,
+    NonMtmFixedFloatXCS,
+    NonMtmFixedFixedXCS,
+    XCS,
+    FixedFloatXCS,
+    FixedFixedXCS,
+    FloatFixedXCS,
+    Portfolio,
+    Spread,
+    Fly,
+    _get_curves_and_fx_maybe_from_solver,
 )
 from rateslib.dual import Dual, Dual2
 from rateslib.calendars import dcf
-from rateslib.curves import Curve
+from rateslib.curves import Curve, IndexCurve, LineCurve
 from rateslib.fx import FXRates, FXForwards
 from rateslib.solver import Solver
 
 
 @pytest.fixture()
 def curve():
     nodes = {
         dt(2022, 1, 1): 1.00,
         dt(2022, 4, 1): 0.99,
         dt(2022, 7, 1): 0.98,
-        dt(2022, 10, 1): 0.97
+        dt(2022, 10, 1): 0.97,
     }
     convention = "Act360"
     return Curve(nodes=nodes, interpolation="log_linear")
 
 
 @pytest.fixture()
 def curve2():
     nodes = {
         dt(2022, 1, 1): 1.00,
         dt(2022, 4, 1): 0.98,
         dt(2022, 7, 1): 0.97,
-        dt(2022, 10, 1): 0.95
+        dt(2022, 10, 1): 0.95,
     }
     return Curve(nodes=nodes, interpolation="log_linear")
 
 
 @pytest.fixture()
 def usdusd():
     nodes = {dt(2022, 1, 1): 1.00, dt(2022, 4, 1): 0.99}
@@ -58,19 +81,18 @@
 def usdeur():
     nodes = {dt(2022, 1, 1): 1.00, dt(2022, 4, 1): 0.996}
     return Curve(nodes=nodes, interpolation="log_linear")
 
 
 def test_get_curve_from_solver():
     from rateslib.solver import Solver
+
     curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 1.0}, id="tagged")
     inst = [(Value(dt(2023, 1, 1)), ("tagged",), {})]
-    solver = Solver(
-        [curve], inst, [0.975]
-    )
+    solver = Solver([curve], inst, [0.975])
 
     result = _get_curve_from_solver("tagged", solver)
     assert result == curve
 
     result = _get_curve_from_solver(curve, solver)
     assert result == curve
 
@@ -95,23 +117,19 @@
 @pytest.mark.parametrize("fx", [None, 2.0])
 @pytest.mark.parametrize("crv", [True, False])
 def test_get_curves_and_fx_from_solver(usdusd, usdeur, eureur, solver, fxf, fx, crv):
     curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 1.0}, id="tagged")
     inst = [(Value(dt(2023, 1, 1)), ("tagged",), {})]
     fxfs = FXForwards(
         FXRates({"eurusd": 1.05}, settlement=dt(2022, 1, 3)),
-        {
-            "usdusd": usdusd,
-            "usdeur": usdeur,
-            "eureur": eureur
-        }
+        {"usdusd": usdusd, "usdeur": usdeur, "eureur": eureur},
+    )
+    solver = (
+        Solver([curve], inst, [0.975], fx=fxfs if fxf else None) if solver else None
     )
-    solver = Solver(
-        [curve], inst, [0.975], fx=fxfs if fxf else None
-    ) if solver else None
     curve = curve if crv else None
 
     crv_result, fx_result = _get_curves_and_fx_maybe_from_solver(
         None, solver, curve, fx
     )
 
     # check the fx results. If fx is specified directly it is returned
@@ -149,25 +167,177 @@
 @pytest.mark.parametrize("num", [1, 2, 3, 4])
 def test_get_curves_from_solver_multiply(num):
     from rateslib.solver import Solver
 
     curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 1.0}, id="tagged")
     inst = [(Value(dt(2023, 1, 1)), ("tagged",), {})]
     solver = Solver([curve], inst, [0.975])
-    result, _ = _get_curves_and_fx_maybe_from_solver(None, solver, ["tagged"] * num, None)
+    result, _ = _get_curves_and_fx_maybe_from_solver(
+        None, solver, ["tagged"] * num, None
+    )
     assert result == (curve, curve, curve, curve)
 
 
-class TestIRS:
+def test_get_proxy_curve_from_solver(usdusd, usdeur, eureur):
+    # TODO: check whether curves in fxf but not is solver should be allowed???
+    curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 1.0}, id="tagged")
+    inst = [(Value(dt(2023, 1, 1)), ("tagged",), {})]
+    fxf = FXForwards(
+        FXRates({"eurusd": 1.05}, settlement=dt(2022, 1, 3)),
+        {"usdusd": usdusd, "usdeur": usdeur, "eureur": eureur},
+    )
+    solver = Solver([curve], inst, [0.975], fx=fxf)
+    curve = fxf.curve("eur", "usd")
+    irs = IRS(dt(2022, 1, 1), "3m", "Q")
+
+    # test the curve will return even though it is not included within the solver
+    # because it is a proxy curve.
+    irs.npv(curves=curve, solver=solver)
+
+
+class TestNullPricing:
+    # test instruments can be priced without defining a pricing parameter.
+
+    @pytest.mark.parametrize(
+        "inst",
+        [
+            IRS(dt(2022, 7, 1), "3M", "A", curves="eureur", notional=1e6),
+            FRA(dt(2022, 7, 1), "3M", "A", curves="eureur", notional=1e6),
+            SBS(
+                dt(2022, 7, 1),
+                "3M",
+                "A",
+                curves=["eureur", "eureur", "eurusd", "eureur"],
+                notional=-1e6,
+            ),
+            ZCS(dt(2022, 7, 1), "3M", "A", curves="eureur", notional=1e6),
+            IIRS(dt(2022, 7, 1), "3M", "A", curves=["eu_cpi", "eureur", "eureur", "eureur"], notional=1e6),
+            IIRS(dt(2022, 7, 1), "3M", "A",
+                 curves=["eu_cpi", "eureur", "eureur", "eureur"], notional=1e6, notional_exchange=True),
+            # TODO add a null price test for ZCIS
+            XCS(
+                dt(2022, 7, 1),
+                "3M",
+                "A",
+                currency="usd",
+                leg2_currency="eur",
+                curves=["usdusd", "usdusd", "eureur", "eurusd"],
+                notional=1e6,
+            ),
+            NonMtmXCS(
+                dt(2022, 7, 1),
+                "3M",
+                "A",
+                currency="usd",
+                leg2_currency="eur",
+                curves=["usdusd", "usdusd", "eureur", "eurusd"],
+                notional=1e6,
+            ),
+            NonMtmFixedFloatXCS(
+                dt(2022, 7, 1),
+                "3M",
+                "A",
+                currency="eur",
+                leg2_currency="usd",
+                curves=["eureur", "eureur", "usdusd", "usdusd"],
+                notional=1e6,
+            ),
+            NonMtmFixedFixedXCS(
+                dt(2022, 7, 1),
+                "3M",
+                "A",
+                currency="eur",
+                leg2_currency="usd",
+                fixed_rate=1.2,
+                curves=["eureur", "eureur", "usdusd", "usdusd"],
+                notional=1e6,
+            ),
+            FixedFloatXCS(
+                dt(2022, 7, 1),
+                "3M",
+                "A",
+                currency="eur",
+                leg2_currency="usd",
+                curves=["eureur", "eureur", "usdusd", "usdusd"],
+                notional=1e6,
+            ),
+            FixedFixedXCS(
+                dt(2022, 7, 1),
+                "3M",
+                "A",
+                currency="eur",
+                leg2_currency="usd",
+                leg2_fixed_rate=1.3,
+                curves=["eureur", "eureur", "usdusd", "usdusd"],
+                notional=1e6,
+            ),
+            FloatFixedXCS(
+                dt(2022, 7, 1),
+                "3M",
+                "A",
+                currency="usd",
+                leg2_currency="eur",
+                curves=["usdusd", "usdusd", "eureur", "eureur"],
+                notional=-1e6,
+            ),
+            FXSwap(
+                dt(2022, 7, 1),
+                "3M",
+                "A",
+                currency="eur",
+                leg2_currency="usd",
+                curves=["eureur", "eureur", "usdusd", "usdusd"],
+                notional=1e6,
+            ),
+        ],
+    )
+    def test_null_priced_delta(self, inst):
+        c1 = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99}, id="usdusd")
+        c2 = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.98}, id="eureur")
+        c3 = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.982}, id="eurusd")
+        c4 = IndexCurve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.995}, id="eu_cpi", index_base=100.0)
+        fxf = FXForwards(
+            FXRates({"eurusd": 1.0}, settlement=dt(2022, 1, 1)),
+            {"usdusd": c1, "eureur": c2, "eurusd": c3},
+        )
+        ins = [
+            IRS(dt(2022, 1, 1), "1y", "A", curves="eureur"),
+            IRS(dt(2022, 1, 1), "1y", "A", curves="usdusd"),
+            IRS(dt(2022, 1, 1), "1y", "A", curves="eurusd"),
+            ZCIS(dt(2022, 1, 1), "1y", "A", curves=["eureur", "eureur", "eu_cpi", "eureur"])
+        ]
+        solver = Solver(
+            curves=[c1, c2, c3, c4],
+            instruments=ins,
+            s=[1.2, 1.3, 1.33, 0.5],
+            id="solver",
+            instrument_labels=["eur 1y", "usd 1y", "eur 1y xcs adj.", "1y cpi"],
+            fx=fxf,
+        )
+        result = inst.delta(solver=solver)
+        assert abs((result.iloc[0, 0] - 25.0)) < 1.0
+        result2 = inst.npv(solver=solver)
+        assert abs(result2) < 1e-3
+
+        # test that instruments have not been set by the previous pricing action
+        solver.s = [1.3, 1.4, 1.36, 0.55]
+        solver.iterate()
+        result3 = inst.npv(solver=solver)
+        assert abs(result3) < 1e-3
 
-    @pytest.mark.parametrize("float_spread, fixed_rate, expected", [
-        (0, 4.03, 4.03637780),
-        (3, 4.03, 4.06637780),
-        (0, 5.10, 4.03637780),
-    ])
+
+class TestIRS:
+    @pytest.mark.parametrize(
+        "float_spread, fixed_rate, expected",
+        [
+            (0, 4.03, 4.03637780),
+            (3, 4.03, 4.06637780),
+            (0, 5.10, 4.03637780),
+        ],
+    )
     def test_irs_rate(self, curve, float_spread, fixed_rate, expected):
         # test the mid-market rate ignores the given fixed_rate and reacts to float_spread
         irs = IRS(
             effective=dt(2022, 1, 1),
             termination=dt(2022, 6, 1),
             payment_lag=2,
             notional=1e9,
@@ -176,19 +346,23 @@
             fixed_rate=4.03,
             stub="ShortFront",
             leg2_float_spread=float_spread,
         )
         result = irs.rate(curve)
         assert abs(result - expected) < 1e-7
 
-    @pytest.mark.parametrize("float_spread, fixed_rate, expected", [
-        (0, 4.03, -0.63777963),
-        (10, 4.03, -0.63777963),
-        (0, 4.01, -2.63777963),
-    ])
+    @pytest.mark.parametrize(
+        "float_spread, fixed_rate, expected",
+        [
+            (0, 4.03, -0.63777963),
+            (200, 4.03, -0.63777963),
+            (500, 4.03, -0.63777963),
+            (0, 4.01, -2.63777963),
+        ],
+    )
     def test_irs_spread_none_simple(self, curve, float_spread, fixed_rate, expected):
         # test the mid-market float spread ignores the given float_spread and react to fixed
         irs = IRS(
             effective=dt(2022, 1, 1),
             termination=dt(2022, 6, 1),
             payment_lag=2,
             notional=1e9,
@@ -203,20 +377,27 @@
         result = irs.spread(curve)
         assert abs(result - expected) < 1e-7
 
         irs.leg2_float_spread = result
         validate = irs.npv(curve)
         assert abs(validate) < 1e-8
 
-    @pytest.mark.parametrize("float_spread, fixed_rate, expected", [
-        # (0, 4.03, -0.6322524949759807),  # note this is the closest solution
-        # (200, 4.03, -0.632906212667),  # note this is 0.0007bp inaccurate
-        # (500, 4.03, -0.64246185393653),  # note this is 0.0102bp inaccurate
-        (0, 4.01, -2.61497625534),
-    ])
+    @pytest.mark.parametrize(
+        "float_spread, fixed_rate, expected",
+        [
+            (0, 4.03, -0.6322524949759807),  # note this is the closest solution
+            (
+                200,
+                4.03,
+                -0.632906212667,
+            ),  # note this is 0.0006bp inaccurate due to approx
+            (500, 4.03, -0.64246185),  # note this is 0.0102bp inaccurate due to approx
+            (0, 4.01, -2.61497625534),
+        ],
+    )
     def test_irs_spread_isda_compound(self, curve, float_spread, fixed_rate, expected):
         # test the mid-market float spread ignores the given float_spread and react to fixed
         irs = IRS(
             effective=dt(2022, 1, 1),
             termination=dt(2022, 6, 1),
             payment_lag=2,
             notional=1e9,
@@ -225,19 +406,60 @@
             fixed_rate=fixed_rate,
             leg2_float_spread=float_spread,
             leg2_fixing_method="rfr_payment_delay",
             leg2_spread_compound_method="isda_compounding",
             stub="ShortFront",
         )
         result = irs.spread(curve)
-        assert abs(result - expected) < 1e-7
+        assert abs(result - expected) < 1e-2
+
+        irs.leg2_float_spread = result
+        validate = irs.npv(curve)
+        assert abs(validate) < 5e2
 
-        # irs.float_spread = result
-        # validate = irs.npv(curve)
-        # assert abs(validate) < 1e-4
+    @pytest.mark.parametrize(
+        "float_spread, fixed_rate, expected",
+        [
+            (0, 4.03, -0.63500600),  # note this is the closest solution
+            (
+                200,
+                4.03,
+                -0.6348797243,
+            ),  # note this is 0.0001bp inaccurate due to approx
+            (
+                500,
+                4.03,
+                -0.6346903026,
+            ),  # note this is 0.0003bp inaccurate due to approx
+            (0, 4.01, -2.626308241),
+        ],
+    )
+    def test_irs_spread_isda_flat_compound(
+        self, curve, float_spread, fixed_rate, expected
+    ):
+        # test the mid-market float spread ignores the given float_spread and react to fixed
+        irs = IRS(
+            effective=dt(2022, 1, 1),
+            termination=dt(2022, 6, 1),
+            payment_lag=2,
+            notional=1e9,
+            convention="Act360",
+            frequency="Q",
+            fixed_rate=fixed_rate,
+            leg2_float_spread=float_spread,
+            leg2_fixing_method="rfr_payment_delay",
+            leg2_spread_compound_method="isda_flat_compounding",
+            stub="ShortFront",
+        )
+        result = irs.spread(curve)
+        assert abs(result - expected) < 1e-2
+
+        irs.leg2_float_spread = result
+        validate = irs.npv(curve)
+        assert abs(validate) < 20
 
     def test_irs_npv(self, curve):
         irs = IRS(
             effective=dt(2022, 1, 1),
             termination=dt(2022, 6, 1),
             payment_lag=2,
             notional=1e9,
@@ -295,14 +517,142 @@
         assert abs(irs.npv(curve)) < 1e-8
 
     def test_sbs_float_spread_raises(self, curve):
         irs = IRS(dt(2022, 1, 1), "9M", "Q")
         with pytest.raises(AttributeError, match="Cannot set `float_spread`"):
             irs.float_spread = 1.0
 
+    def test_index_base_raises(self):
+        irs = IRS(dt(2022, 1, 1), "9M", "Q")
+        with pytest.raises(AttributeError, match="Cannot set `index_base`"):
+            irs.index_base = 1.0
+
+        with pytest.raises(AttributeError, match="Cannot set `leg2_index_base`"):
+            irs.leg2_index_base = 1.0
+
+
+class TestIIRS:
+
+    def test_index_base_none_populated(self, curve):
+        i_curve = IndexCurve(
+            {dt(2022, 1, 1): 1.0, dt(2022, 2, 1): 0.5, dt(2034, 1, 1): 0.4},
+            index_lag=3,
+            index_base=100.0
+        )
+        iirs = IIRS(
+            effective=dt(2022, 2, 1),
+            termination="1y",
+            frequency="Q",
+            index_lag=3,
+            notional_exchange=False,
+        )
+        for period in iirs.leg1.periods:
+            assert period.index_base is None
+        iirs.rate(curves=[i_curve, curve])
+        for period in iirs.leg1.periods:
+            assert period.index_base == 200.0
+
+    def test_iirs_npv_mid_mkt_zero(self, curve):
+        i_curve = IndexCurve(
+            {dt(2022, 1, 1): 1.0, dt(2022, 2, 1): 0.5, dt(2034, 1, 1): 0.4},
+            index_lag=3,
+            index_base=100.0
+        )
+        iirs = IIRS(
+            effective=dt(2022, 2, 1),
+            termination=dt(2022, 7, 1),
+            payment_lag=0,
+            notional=1e9,
+            convention="Act360",
+            frequency="Q",
+            stub="ShortFront",
+        )
+        result = iirs.npv([i_curve, curve])
+        assert abs(result) < 1e-8
+
+        iirs.fixed_rate = iirs.rate([i_curve, curve])
+        iirs.index_base = 1000.0  # high index base implies positive NPV
+        assert iirs.npv([i_curve, curve]) > 1
+
+        iirs.index_base = None  # index_base set back to initial
+        iirs.fixed_rate = None
+        assert abs(iirs.npv([i_curve, curve])) < 1e-8
+
+        mid_fixed = float(iirs.rate([i_curve, curve]))
+        iirs.base_index = 200.0  # this is index_base from i_curve
+        new_mid = float(iirs.rate([i_curve, curve]))
+        assert abs(mid_fixed - new_mid) < 1e-6
+
+    def test_cashflows(self, curve):
+        i_curve = IndexCurve(
+            {dt(2022, 1, 1): 1.0, dt(2023, 2, 1): 0.99},
+            index_lag=3,
+            index_base=100.0
+        )
+        iirs = IIRS(
+            effective=dt(2022, 2, 1),
+            termination="9M",
+            frequency="Q",
+            index_base=Series([90, 110], index=[dt(2022, 1, 31), dt(2022, 2, 2)]),
+            index_fixings=[110, 115],
+            index_lag=3,
+            index_method="daily",
+            fixed_rate=1.0
+        )
+        result = iirs.cashflows([i_curve, curve, curve, curve])
+        expected = DataFrame({
+            "Index Val": [110.0, 115.0, 100.7754, np.nan, np.nan, np.nan],
+            "Index Ratio": [1.10, 1.15, 1.00775, np.nan, np.nan, np.nan],
+            "NPV": [
+                -2682.655, -2869.534, -2488.937, 9849.93, 10070.85, 9963.277
+            ],
+            "Type": ["IndexFixedPeriod"] * 3 + ["FloatPeriod"] * 3
+        }, index= MultiIndex.from_tuples([
+            ("leg1", 0), ("leg1", 1), ("leg1", 2), ("leg2", 0), ("leg2", 1), ("leg2", 2)
+        ]))
+        assert_frame_equal(
+            expected, result[["Index Val", "Index Ratio", "NPV", "Type"]], rtol=1e-3,
+        )
+
+    def test_npv_no_index_base(self, curve):
+        i_curve = IndexCurve(
+            {dt(2022, 1, 1): 1.0, dt(2022, 2, 1): 0.5, dt(2034, 1, 1): 0.4},
+            index_lag=3,
+            index_base=100.0
+        )
+        iirs = IIRS(
+            effective=dt(2022, 2, 1),
+            termination="1y",
+            frequency="Q",
+            fixed_rate=2.0,
+            index_lag=3,
+            notional_exchange=False,
+        )
+        result = iirs.npv([i_curve, curve, curve, curve])
+        expected = 19792.08369745
+        assert abs(result - expected) < 1e-6
+
+    def test_cashflows_no_index_base(self, curve):
+        i_curve = IndexCurve(
+            {dt(2022, 1, 1): 1.0, dt(2022, 2, 1): 0.5, dt(2034, 1, 1): 0.4},
+            index_lag=3,
+            index_base=100.0
+        )
+        iirs = IIRS(
+            effective=dt(2022, 2, 1),
+            termination="1y",
+            frequency="Q",
+            fixed_rate=2.0,
+            index_lag=3,
+            notional_exchange=False,
+        )
+        result = iirs.cashflows([i_curve, curve, curve, curve])
+        for i in range(4):
+            assert result.iloc[i]["Index Base"] == 200.0
+
 
 class TestSBS:
     def test_sbs_npv(self, curve):
         sbs = SBS(dt(2022, 1, 1), "9M", "Q", float_spread=3.0)
         a_delta = sbs.analytic_delta(curve, curve, leg=1)
         npv = sbs.npv(curve)
         assert abs(npv + 3.0 * a_delta) < 1e-9
@@ -322,19 +672,22 @@
         alias = sbs.rate([curve], leg=2)
         assert abs(result - 3.0) < 1e-8
         assert abs(alias - 3.0) < 1e-8
 
     def test_sbs_cashflows(self, curve):
         sbs = SBS(dt(2022, 1, 1), "9M", "Q", float_spread=3.0)
         result = sbs.cashflows(curve)
-        expected = DataFrame({
-            "Type": ["FloatPeriod", "FloatPeriod"],
-            "Period": ["Regular", "Regular"],
-            "Spread": [3.0, 0.0],
-        }, index=MultiIndex.from_tuples([("leg1", 0), ("leg2", 2)]))
+        expected = DataFrame(
+            {
+                "Type": ["FloatPeriod", "FloatPeriod"],
+                "Period": ["Regular", "Regular"],
+                "Spread": [3.0, 0.0],
+            },
+            index=MultiIndex.from_tuples([("leg1", 0), ("leg2", 2)]),
+        )
         assert_frame_equal(
             result.loc[[("leg1", 0), ("leg2", 2)], ["Type", "Period", "Spread"]],
             expected,
         )
 
     def test_sbs_fixed_rate_raises(self, curve):
         sbs = SBS(dt(2022, 1, 1), "9M", "Q", float_spread=3.0)
@@ -342,15 +695,14 @@
             sbs.fixed_rate = 1.0
 
         with pytest.raises(AttributeError, match="Cannot set `leg2_fixed_rate`"):
             sbs.leg2_fixed_rate = 1.0
 
 
 class TestFRA:
-
     def test_fra_rate(self, curve):
         # test the mid-market rate ignores the given fixed_rate and reacts to float_spread
         fra = FRA(
             effective=dt(2022, 1, 1),
             termination=dt(2022, 7, 1),
             notional=1e9,
             convention="Act360",
@@ -370,15 +722,15 @@
             convention="Act360",
             modifier="mf",
             frequency="S",
             fixed_rate=4.035,
         )
         result = fra.npv(curve)
         expected = fra.analytic_delta(curve) * (4.035 - fra.rate(curve)) * -100
-        assert abs(result - expected) < 1e-9
+        assert abs(result - expected) < 1e-8
         assert abs(result - 118631.8350458332) < 1e-7
 
     def test_fra_cashflows(self, curve):
         fra = FRA(
             effective=dt(2022, 1, 1),
             termination=dt(2022, 7, 1),
             payment_lag=2,
@@ -406,28 +758,93 @@
         fra.fixed_rate = 1.0  # pay fixed low rate implies positive NPV
         assert fra.npv(curve) > 1
 
         fra.fixed_rate = None  # fixed rate set back to initial
         assert abs(fra.npv(curve)) < 1e-9
 
 
+class TestZCS:
+    @pytest.mark.parametrize("freq, exp", [("Q", 3.52986327830), ("S", 3.54543819675)])
+    def test_zcs_rate(self, freq, exp):
+        usd = Curve(
+            nodes={dt(2022, 1, 1): 1.0, dt(2027, 1, 1): 0.85, dt(2032, 1, 1): 0.70},
+            id="usd",
+        )
+        zcs = ZCS(
+            effective=dt(2022, 1, 1),
+            termination="10Y",
+            frequency=freq,
+            leg2_frequency="Q",
+            calendar="nyc",
+            currency="usd",
+            fixed_rate=4.0,
+            convention="Act360",
+            notional=100e6,
+            curves=["usd"],
+        )
+        result = zcs.rate(usd)
+        assert abs(result - exp) < 1e-7
+
+    def test_zcs_analytic_delta(self):
+        usd = Curve(
+            nodes={dt(2022, 1, 1): 1.0, dt(2027, 1, 1): 0.85, dt(2032, 1, 1): 0.70},
+            id="usd",
+        )
+        zcs = ZCS(
+            effective=dt(2022, 1, 1),
+            termination="10Y",
+            frequency="Q",
+            leg2_frequency="Q",
+            calendar="nyc",
+            currency="usd",
+            fixed_rate=4.0,
+            convention="Act360",
+            notional=100e6,
+            curves=["usd"],
+        )
+        result = zcs.analytic_delta(usd, usd)
+        expected = 105226.66099084
+        assert abs(result - expected) < 1e-7
+
+
+class TestZCIS:
+
+    def test_leg2_index_base(self, curve):
+        i_curve = IndexCurve(
+            {dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99},
+            index_base=200.0
+        )
+        zcis = ZCIS(
+            effective=dt(2022, 1, 1),
+            termination="9m",
+            frequency="Q",
+        )
+        prior = zcis.rate(curves=[curve, curve, i_curve, curve])
+
+        zcis.leg2_index_base = 100.0  # index base is lower
+        result = zcis.rate(curves=[curve, curve, i_curve, curve])
+        assert result > (prior + 100)
+
+
 def test_forward_fx_immediate():
-    d_curve = Curve(nodes={dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99},
-                    interpolation="log_linear")
+    d_curve = Curve(
+        nodes={dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99}, interpolation="log_linear"
+    )
     f_curve = Curve(nodes={dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.95})
     result = forward_fx(dt(2022, 4, 1), d_curve, f_curve, 10.0)
     assert abs(result - 10.102214) < 1e-6
 
     result = forward_fx(dt(2022, 1, 1), d_curve, f_curve, 10.0, dt(2022, 1, 1))
     assert abs(result - 10.0) < 1e-6
 
 
 def test_forward_fx_spot_equivalent():
-    d_curve = Curve(nodes={dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99},
-                    interpolation="log_linear")
+    d_curve = Curve(
+        nodes={dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99}, interpolation="log_linear"
+    )
     f_curve = Curve(nodes={dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.95})
     result = forward_fx(dt(2022, 7, 1), d_curve, f_curve, 10.102214, dt(2022, 4, 1))
     assert abs(result - 10.206626) < 1e-6
 
 
 # test the commented out FXSwap variant
 # def test_fx_swap(curve, curve2):
@@ -457,81 +874,127 @@
 #     )
 #     points2 = fxs.rate(fxf)
 #     npv2 = fxs.npv(fxf, None, "eur")
 #     assert abs(npv2) < 1e-9
 
 
 class TestNonMtmXCS:
-
     def test_nonmtmxcs_npv(self, curve, curve2):
         fxf = FXForwards(
             FXRates({"eurusd": 1.1}, settlement=dt(2022, 1, 3)),
-            {"usdusd": curve, "eurusd": curve2, "eureur": curve2}
+            {"usdusd": curve, "eurusd": curve2, "eureur": curve2},
         )
 
-        xcs = NonMtmXCS(dt(2022, 2, 1), "8M", "M",
-                        payment_lag=0, currency="eur", leg2_currency="usd",
-                        payment_lag_exchange=0)
+        xcs = NonMtmXCS(
+            dt(2022, 2, 1),
+            "8M",
+            "M",
+            payment_lag=0,
+            currency="eur",
+            leg2_currency="usd",
+            payment_lag_exchange=0,
+        )
         npv2 = xcs._npv2(curve2, curve2, curve, curve, 1.10)
         npv = xcs.npv([curve2, curve2, curve, curve], None, fxf)
         assert abs(npv) < 1e-9
 
-        xcs = NonMtmXCS(dt(2022, 2, 1), "8M", "M", payment_lag=0, amortization=100e3,
-                        currency="eur", leg2_currency="usd",
-                        payment_lag_exchange=0)
+        xcs = NonMtmXCS(
+            dt(2022, 2, 1),
+            "8M",
+            "M",
+            payment_lag=0,
+            amortization=100e3,
+            currency="eur",
+            leg2_currency="usd",
+            payment_lag_exchange=0,
+        )
         npv2 = xcs._npv2(curve2, curve2, curve, curve, 1.10)
         npv = xcs.npv([curve2, curve2, curve, curve], None, fxf)
         assert abs(npv) < 1e-9
 
     def test_nonmtmxcs_fx_notional(self):
-        xcs = NonMtmXCS(dt(2022, 2, 1), "8M", "M",
-                        payment_lag=0, currency="eur", leg2_currency="usd",
-                        payment_lag_exchange=0, fx_fixing=2.0, notional=1e6)
+        xcs = NonMtmXCS(
+            dt(2022, 2, 1),
+            "8M",
+            "M",
+            payment_lag=0,
+            currency="eur",
+            leg2_currency="usd",
+            payment_lag_exchange=0,
+            fx_fixing=2.0,
+            notional=1e6,
+        )
         assert xcs.leg2_notional == -2e6
 
-    @pytest.mark.parametrize("float_spd, compound, expected",[
-        (10, "none_simple", 10.160794),
-        (100, "none_simple", 101.60794),
-        (100, "isda_compounding", 101.00),
-    ])
+    @pytest.mark.parametrize(
+        "float_spd, compound, expected",
+        [
+            (10, "none_simple", 10.160794),
+            (100, "none_simple", 101.60794),
+            (100, "isda_compounding", 101.023590),
+            (100, "isda_flat_compounding", 101.336040),
+        ],
+    )
     def test_nonmtmxcs_spread(self, curve, curve2, float_spd, compound, expected):
         fxf = FXForwards(
             FXRates({"usdnok": 10}, settlement=dt(2022, 1, 3)),
-            {"usdusd": curve, "nokusd": curve2, "noknok": curve2}
+            {"usdusd": curve, "nokusd": curve2, "noknok": curve2},
         )
 
-        xcs = NonMtmXCS(dt(2022, 2, 1), "8M", "M",
-                        payment_lag=0, currency="nok", leg2_currency="usd",
-                        payment_lag_exchange=0, notional=10e6,
-                        float_spread=float_spd, leg2_spread_compound_method=compound)
+        xcs = NonMtmXCS(
+            dt(2022, 2, 1),
+            "8M",
+            "M",
+            payment_lag=0,
+            currency="nok",
+            leg2_currency="usd",
+            payment_lag_exchange=0,
+            notional=10e6,
+            float_spread=float_spd,
+            leg2_spread_compound_method=compound,
+        )
 
         result = xcs.rate([curve, curve, curve2, curve2], None, fxf, 2)
         assert abs(result - expected) < 1e-4
         alias = xcs.spread([curve, curve, curve2, curve2], None, fxf, 2)
         assert alias == result
 
         xcs.leg2_float_spread = result
         validate = xcs.npv([curve, curve, curve2, curve2], None, fxf)
         assert abs(validate) < 1e-2
         result2 = xcs.rate([curve, curve, curve2, curve2], None, fxf, 2)
-        assert abs(result - result2) < 1e-9
+        assert abs(result - result2) < 1e-3
 
         # reverse legs
-        xcs_reverse = NonMtmXCS(dt(2022, 2, 1), "8M", "M",
-                                payment_lag=0, currency="usd", leg2_currency="nok",
-                                payment_lag_exchange=0, notional=1e6,
-                                leg2_float_spread=float_spd,
-                                spread_compound_method=compound)
+        xcs_reverse = NonMtmXCS(
+            dt(2022, 2, 1),
+            "8M",
+            "M",
+            payment_lag=0,
+            currency="usd",
+            leg2_currency="nok",
+            payment_lag_exchange=0,
+            notional=1e6,
+            leg2_float_spread=float_spd,
+            spread_compound_method=compound,
+        )
         result = xcs_reverse.rate([curve2, curve2, curve, curve], None, fxf, 1)
         assert abs(result - expected) < 1e-4
 
     def test_no_fx_raises(self, curve, curve2):
-        xcs = NonMtmXCS(dt(2022, 2, 1), "8M", "M",
-                        payment_lag=0, currency="nok", leg2_currency="usd",
-                        payment_lag_exchange=0, notional=10e6)
+        xcs = NonMtmXCS(
+            dt(2022, 2, 1),
+            "8M",
+            "M",
+            payment_lag=0,
+            currency="nok",
+            leg2_currency="usd",
+            payment_lag_exchange=0,
+            notional=10e6,
+        )
 
         with pytest.raises(ValueError, match="`fx` is required when `fx_fixing` is"):
             with default_context("no_fx_fixings_for_xcs", "raise"):
                 xcs.npv([curve, curve, curve2, curve2])
 
         with pytest.raises(ValueError, match="`fx` is required when `fx_fixing` is"):
             with default_context("no_fx_fixings_for_xcs", "raise"):
@@ -540,150 +1003,234 @@
         with pytest.warns():
             with default_context("no_fx_fixings_for_xcs", "warn"):
                 xcs.npv([curve, curve, curve2, curve2])
 
     def test_nonmtmxcs_cashflows(self, curve, curve2):
         fxf = FXForwards(
             FXRates({"usdnok": 10}, settlement=dt(2022, 1, 3)),
-            {"usdusd": curve, "nokusd": curve2, "noknok": curve2}
+            {"usdusd": curve, "nokusd": curve2, "noknok": curve2},
         )
 
-        xcs = NonMtmXCS(dt(2022, 2, 1), "8M", "M",
-                        payment_lag=0, currency="nok", leg2_currency="usd",
-                        payment_lag_exchange=0, notional=10e6)
+        xcs = NonMtmXCS(
+            dt(2022, 2, 1),
+            "8M",
+            "M",
+            payment_lag=0,
+            currency="nok",
+            leg2_currency="usd",
+            payment_lag_exchange=0,
+            notional=10e6,
+        )
 
         result = xcs.cashflows([curve, curve, curve2, curve2], None, fxf)
-        expected = DataFrame({
-            "Type": ["Cashflow", "FloatPeriod"],
-            "Period": ["Exchange", "Regular"],
-            "Ccy": ["NOK", "USD"],
-            "Notional": [-10000000, -996734.0252423884],
-            "FX Rate": [0.10002256337062124, 1.0],
-        }, index=MultiIndex.from_tuples([("leg1", 0), ("leg2", 8)]))
+        expected = DataFrame(
+            {
+                "Type": ["Cashflow", "FloatPeriod"],
+                "Period": ["Exchange", "Regular"],
+                "Ccy": ["NOK", "USD"],
+                "Notional": [-10000000, -996734.0252423884],
+                "FX Rate": [0.10002256337062124, 1.0],
+            },
+            index=MultiIndex.from_tuples([("leg1", 0), ("leg2", 8)]),
+        )
         assert_frame_equal(
-            result.loc[[("leg1", 0), ("leg2", 8)], ["Type", "Period", "Ccy", "Notional", "FX Rate"]],
+            result.loc[
+                [("leg1", 0), ("leg2", 8)],
+                ["Type", "Period", "Ccy", "Notional", "FX Rate"],
+            ],
             expected,
         )
 
     @pytest.mark.parametrize("fix", ["fxr", "fxf", "float", "dual", "dual2"])
     def test_nonmtm_fx_fixing(self, curve, curve2, fix):
         fxr = FXRates({"usdnok": 10}, settlement=dt(2022, 1, 1))
         fxf = FXForwards(fxr, {"usdusd": curve, "nokusd": curve2, "noknok": curve2})
         mapping = {
-            "fxr": fxr, "fxf": fxf, "float": 10.0,
-            "dual": Dual(10.0, "x"), "dual2": Dual2(10.0, "x")
+            "fxr": fxr,
+            "fxf": fxf,
+            "float": 10.0,
+            "dual": Dual(10.0, "x"),
+            "dual2": Dual2(10.0, "x"),
         }
-        xcs = NonMtmXCS(dt(2022, 2, 1), "8M", "M",
-                        payment_lag=0, currency="nok", leg2_currency="usd",
-                        payment_lag_exchange=0, notional=10e6, fx_fixing=mapping[fix])
+        xcs = NonMtmXCS(
+            dt(2022, 2, 1),
+            "8M",
+            "M",
+            payment_lag=0,
+            currency="nok",
+            leg2_currency="usd",
+            payment_lag_exchange=0,
+            notional=10e6,
+            fx_fixing=mapping[fix],
+        )
         assert abs(xcs.npv([curve, curve, curve2, curve2])) < 1e-7
 
 
 class TestNonMtmFixedFloatXCS:
-
-    @pytest.mark.parametrize("float_spd, compound, expected",[
-        (10, "none_simple", 6.70955968),
-        (100, "isda_compounding", 7.62137047),
-    ])
+    @pytest.mark.parametrize(
+        "float_spd, compound, expected",
+        [
+            (10, "none_simple", 6.70955968),
+            (100, "isda_compounding", 7.62137047),
+        ],
+    )
     def test_nonmtmfixxcs_rate_npv(self, curve, curve2, float_spd, compound, expected):
         fxf = FXForwards(
             FXRates({"usdnok": 10}, settlement=dt(2022, 1, 3)),
-            {"usdusd": curve, "nokusd": curve2, "noknok": curve2}
+            {"usdusd": curve, "nokusd": curve2, "noknok": curve2},
+        )
+        xcs = NonMtmFixedFloatXCS(
+            dt(2022, 2, 1),
+            "8M",
+            "M",
+            payment_lag=0,
+            currency="nok",
+            leg2_currency="usd",
+            payment_lag_exchange=0,
+            notional=10e6,
+            leg2_spread_compound_method=compound,
+            leg2_float_spread=float_spd,
         )
-        xcs = NonMtmFixedFloatXCS(dt(2022, 2, 1), "8M", "M",
-            payment_lag=0, currency="nok", leg2_currency="usd",
-            payment_lag_exchange=0, notional=10e6,
-            leg2_spread_compound_method=compound, leg2_float_spread=float_spd
-         )
 
         result = xcs.rate([curve2, curve2, curve, curve], None, fxf, 1)
         assert abs(result - expected) < 1e-4
         assert abs(xcs.npv([curve2, curve2, curve, curve], None, fxf)) < 1e-6
 
         xcs.fixed_rate = result  # set the fixed rate and check revalues to zero
         assert abs(xcs.npv([curve2, curve2, curve, curve], None, fxf)) < 1e-6
 
-        irs = IRS(dt(2022, 2, 1), "8M", "M",
-            payment_lag=0, currency="nok",
-            leg2_spread_compound_method=compound, leg2_float_spread=float_spd)
+        irs = IRS(
+            dt(2022, 2, 1),
+            "8M",
+            "M",
+            payment_lag=0,
+            currency="nok",
+            leg2_spread_compound_method=compound,
+            leg2_float_spread=float_spd,
+        )
         validate = irs.rate(curve2)
         assert abs(result - validate) < 1e-2
 
     def test_nonmtmfixxcs_fx_notional(self):
-        xcs = NonMtmFixedFloatXCS(dt(2022, 2, 1), "8M", "M",
-                        payment_lag=0, currency="eur", leg2_currency="usd",
-                        payment_lag_exchange=0, fx_fixing=2.0, notional=1e6)
+        xcs = NonMtmFixedFloatXCS(
+            dt(2022, 2, 1),
+            "8M",
+            "M",
+            payment_lag=0,
+            currency="eur",
+            leg2_currency="usd",
+            payment_lag_exchange=0,
+            fx_fixing=2.0,
+            notional=1e6,
+        )
         assert xcs.leg2_notional == -2e6
 
     def test_nonmtmfixxcs_no_fx_raises(self, curve, curve2):
-        xcs = NonMtmFixedFloatXCS(dt(2022, 2, 1), "8M", "M",
-                        payment_lag=0, currency="nok", leg2_currency="usd",
-                        payment_lag_exchange=0, notional=10e6)
+        xcs = NonMtmFixedFloatXCS(
+            dt(2022, 2, 1),
+            "8M",
+            "M",
+            payment_lag=0,
+            currency="nok",
+            leg2_currency="usd",
+            payment_lag_exchange=0,
+            notional=10e6,
+        )
 
         with pytest.raises(ValueError, match="`fx` is required when `fx_fixing` is"):
             with default_context("no_fx_fixings_for_xcs", "raise"):
                 xcs.npv([curve, curve, curve2, curve2])
 
         with pytest.raises(ValueError, match="`fx` is required when `fx_fixing` is"):
             with default_context("no_fx_fixings_for_xcs", "raise"):
                 xcs.cashflows([curve, curve, curve2, curve2])
 
     def test_nonmtmfixxcs_cashflows(self, curve, curve2):
         fxf = FXForwards(
             FXRates({"usdnok": 10}, settlement=dt(2022, 1, 3)),
-            {"usdusd": curve, "nokusd": curve2, "noknok": curve2}
+            {"usdusd": curve, "nokusd": curve2, "noknok": curve2},
         )
 
-        xcs = NonMtmFixedFloatXCS(dt(2022, 2, 1), "8M", "M",
-                        payment_lag=0, currency="nok", leg2_currency="usd",
-                        payment_lag_exchange=0, notional=10e6)
+        xcs = NonMtmFixedFloatXCS(
+            dt(2022, 2, 1),
+            "8M",
+            "M",
+            payment_lag=0,
+            currency="nok",
+            leg2_currency="usd",
+            payment_lag_exchange=0,
+            notional=10e6,
+        )
 
         result = xcs.cashflows([curve, curve, curve2, curve2], None, fxf)
-        expected = DataFrame({
-            "Type": ["Cashflow", "FloatPeriod"],
-            "Period": ["Exchange", "Regular"],
-            "Ccy": ["NOK", "USD"],
-            "Notional": [-10000000, -996734.0252423884],
-            "FX Rate": [0.10002256337062124, 1.0],
-        }, index=MultiIndex.from_tuples([("leg1", 0), ("leg2", 8)]))
+        expected = DataFrame(
+            {
+                "Type": ["Cashflow", "FloatPeriod"],
+                "Period": ["Exchange", "Regular"],
+                "Ccy": ["NOK", "USD"],
+                "Notional": [-10000000, -996734.0252423884],
+                "FX Rate": [0.10002256337062124, 1.0],
+            },
+            index=MultiIndex.from_tuples([("leg1", 0), ("leg2", 8)]),
+        )
         assert_frame_equal(
-            result.loc[[("leg1", 0), ("leg2", 8)], ["Type", "Period", "Ccy", "Notional", "FX Rate"]],
+            result.loc[
+                [("leg1", 0), ("leg2", 8)],
+                ["Type", "Period", "Ccy", "Notional", "FX Rate"],
+            ],
             expected,
         )
 
     @pytest.mark.parametrize("fix", ["fxr", "fxf", "float", "dual", "dual2"])
     def test_nonmtmfixxcs_fx_fixing(self, curve, curve2, fix):
         fxr = FXRates({"usdnok": 10}, settlement=dt(2022, 1, 1))
         fxf = FXForwards(fxr, {"usdusd": curve, "nokusd": curve2, "noknok": curve2})
         mapping = {
-            "fxr": fxr, "fxf": fxf, "float": 10.0,
-            "dual": Dual(10.0, "x"), "dual2": Dual2(10.0, "x")
+            "fxr": fxr,
+            "fxf": fxf,
+            "float": 10.0,
+            "dual": Dual(10.0, "x"),
+            "dual2": Dual2(10.0, "x"),
         }
-        xcs = NonMtmFixedFloatXCS(dt(2022, 2, 1), "8M", "M",
-                        payment_lag=0, currency="nok", leg2_currency="usd",
-                        payment_lag_exchange=0, notional=10e6, fx_fixing=mapping[fix],
-                        leg2_float_spread=10.0)
+        xcs = NonMtmFixedFloatXCS(
+            dt(2022, 2, 1),
+            "8M",
+            "M",
+            payment_lag=0,
+            currency="nok",
+            leg2_currency="usd",
+            payment_lag_exchange=0,
+            notional=10e6,
+            fx_fixing=mapping[fix],
+            leg2_float_spread=10.0,
+        )
         assert abs(xcs.npv([curve2, curve2, curve, curve])) < 1e-7
 
     def test_nonmtmfixxcs_raises(self, curve, curve2):
         fxf = FXForwards(
             FXRates({"usdnok": 10}, settlement=dt(2022, 1, 3)),
-            {"usdusd": curve, "nokusd": curve2, "noknok": curve2}
+            {"usdusd": curve, "nokusd": curve2, "noknok": curve2},
         )
 
-        xcs = NonMtmFixedFloatXCS(dt(2022, 2, 1), "8M", "M",
-                        payment_lag=0, currency="nok", leg2_currency="usd",
-                        payment_lag_exchange=0, notional=10e6)
+        xcs = NonMtmFixedFloatXCS(
+            dt(2022, 2, 1),
+            "8M",
+            "M",
+            payment_lag=0,
+            currency="nok",
+            leg2_currency="usd",
+            payment_lag_exchange=0,
+            notional=10e6,
+        )
 
         with pytest.raises(ValueError, match="Cannot solve for a"):
             xcs.rate([curve, curve, curve2, curve2], None, fxf, leg=2)
 
 
 class TestNonMtmFixedFixedXCS:
-
     # @pytest.mark.parametrize("float_spd, compound, expected",[
     #     (10, "none_simple", 6.70955968),
     #     (100, "isda_compounding", 7.62137047),
     # ])
     # def test_nonmtmfixxcs_rate_npv(self, curve, curve2, float_spd, compound, expected):
     #     fxf = FXForwards(
     #         FXRates({"usdnok": 10}, settlement=dt(2022, 1, 3)),
@@ -749,181 +1296,253 @@
     #     )
 
     @pytest.mark.parametrize("fix", ["fxr", "fxf", "float", "dual", "dual2"])
     def test_nonmtmfixxcs_fx_fixing(self, curve, curve2, fix):
         fxr = FXRates({"usdnok": 10}, settlement=dt(2022, 1, 1))
         fxf = FXForwards(fxr, {"usdusd": curve, "nokusd": curve2, "noknok": curve2})
         mapping = {
-            "fxr": fxr, "fxf": fxf, "float": 10.0,
-            "dual": Dual(10.0, "x"), "dual2": Dual2(10.0, "x")
+            "fxr": fxr,
+            "fxf": fxf,
+            "float": 10.0,
+            "dual": Dual(10.0, "x"),
+            "dual2": Dual2(10.0, "x"),
         }
-        xcs = NonMtmFixedFixedXCS(dt(2022, 2, 1), "8M", "M",
-                        payment_lag=0, currency="nok", leg2_currency="usd",
-                        payment_lag_exchange=0, notional=10e6, fx_fixing=mapping[fix],
-                        leg2_fixed_rate=2.0,
-                        )
+        xcs = NonMtmFixedFixedXCS(
+            dt(2022, 2, 1),
+            "8M",
+            "M",
+            payment_lag=0,
+            currency="nok",
+            leg2_currency="usd",
+            payment_lag_exchange=0,
+            notional=10e6,
+            fx_fixing=mapping[fix],
+            leg2_fixed_rate=2.0,
+        )
         assert abs(xcs.npv([curve2, curve2, curve, curve])) < 1e-7
 
-        xcs = NonMtmFixedFixedXCS(dt(2022, 2, 1), "8M", "M",
-                        payment_lag=0, currency="nok", leg2_currency="usd",
-                        payment_lag_exchange=0, notional=10e6, fx_fixing=mapping[fix],
-                        fixed_rate=2.0,
-                        )
+        xcs = NonMtmFixedFixedXCS(
+            dt(2022, 2, 1),
+            "8M",
+            "M",
+            payment_lag=0,
+            currency="nok",
+            leg2_currency="usd",
+            payment_lag_exchange=0,
+            notional=10e6,
+            fx_fixing=mapping[fix],
+            fixed_rate=2.0,
+        )
         assert abs(xcs.npv([curve2, curve2, curve, curve])) < 1e-7
 
     def test_nonmtmfixfixxcs_raises(self, curve, curve2):
         fxf = FXForwards(
             FXRates({"usdnok": 10}, settlement=dt(2022, 1, 3)),
-            {"usdusd": curve, "nokusd": curve2, "noknok": curve2}
+            {"usdusd": curve, "nokusd": curve2, "noknok": curve2},
         )
 
-        xcs = NonMtmFixedFixedXCS(dt(2022, 2, 1), "8M", "M",
-                        payment_lag=0, currency="nok", leg2_currency="usd",
-                        payment_lag_exchange=0, notional=10e6)
+        xcs = NonMtmFixedFixedXCS(
+            dt(2022, 2, 1),
+            "8M",
+            "M",
+            payment_lag=0,
+            currency="nok",
+            leg2_currency="usd",
+            payment_lag_exchange=0,
+            notional=10e6,
+        )
 
         with pytest.raises(ValueError, match="Cannot solve for a"):
             xcs.rate([curve, curve, curve2, curve2], None, fxf, leg=2)
 
         with pytest.raises(AttributeError, match="Cannot set `leg2_float_spread` for"):
             xcs.leg2_float_spread = 2.0
 
 
 class TestXCS:
-
     def test_mtmxcs_npv(self, curve, curve2):
         fxf = FXForwards(
             FXRates({"eurusd": 1.1}, settlement=dt(2022, 1, 3)),
-            {"usdusd": curve, "eurusd": curve2, "eureur": curve2}
+            {"usdusd": curve, "eurusd": curve2, "eureur": curve2},
         )
 
-        xcs = XCS(dt(2022, 2, 1), "8M", "M",
-                        payment_lag=0, currency="eur", leg2_currency="usd",
-                        payment_lag_exchange=0)
+        xcs = XCS(
+            dt(2022, 2, 1),
+            "8M",
+            "M",
+            payment_lag=0,
+            currency="eur",
+            leg2_currency="usd",
+            payment_lag_exchange=0,
+        )
 
         npv = xcs.npv([curve2, curve2, curve, curve], None, fxf)
         assert abs(npv) < 1e-9
 
     def test_mtmxcs_cashflows(self, curve, curve2):
         fxf = FXForwards(
             FXRates({"usdnok": 10}, settlement=dt(2022, 1, 3)),
-            {"usdusd": curve, "nokusd": curve2, "noknok": curve2}
+            {"usdusd": curve, "nokusd": curve2, "noknok": curve2},
         )
 
-        xcs = XCS(dt(2022, 2, 1), "8M", "M",
-                        payment_lag=0, currency="nok", leg2_currency="usd",
-                        payment_lag_exchange=0, notional=10e6)
+        xcs = XCS(
+            dt(2022, 2, 1),
+            "8M",
+            "M",
+            payment_lag=0,
+            currency="nok",
+            leg2_currency="usd",
+            payment_lag_exchange=0,
+            notional=10e6,
+        )
 
         result = xcs.cashflows([curve, curve, curve2, curve2], None, fxf)
-        expected = DataFrame({
-            "Type": ["Cashflow", "FloatPeriod", "Cashflow"],
-            "Period": ["Exchange", "Regular", "Mtm"],
-            "Ccy": ["NOK", "USD", "USD"],
-            "Notional": [-10000000, -990019.24969, -3509.80082],
-            "Rate": [np.nan,  8.181151773810475, 0.09829871161519926],
-            "FX Rate": [0.10002256337062124, 1.0, 1.0],
-        }, index=MultiIndex.from_tuples([("leg1", 0), ("leg2", 11), ("leg2", 14)]))
+        expected = DataFrame(
+            {
+                "Type": ["Cashflow", "FloatPeriod", "Cashflow"],
+                "Period": ["Exchange", "Regular", "Mtm"],
+                "Ccy": ["NOK", "USD", "USD"],
+                "Notional": [-10000000, -990019.24969, -3509.80082],
+                "Rate": [np.nan, 8.181151773810475, 0.09829871161519926],
+                "FX Rate": [0.10002256337062124, 1.0, 1.0],
+            },
+            index=MultiIndex.from_tuples([("leg1", 0), ("leg2", 11), ("leg2", 14)]),
+        )
         assert_frame_equal(
-            result.loc[[("leg1", 0), ("leg2", 11), ("leg2", 14)],
-                ["Type", "Period", "Ccy", "Notional", "Rate", "FX Rate"]],
+            result.loc[
+                [("leg1", 0), ("leg2", 11), ("leg2", 14)],
+                ["Type", "Period", "Ccy", "Notional", "Rate", "FX Rate"],
+            ],
             expected,
         )
 
     def test_mtmxcs_fx_fixings_raises(self):
         with pytest.raises(ValueError, match="`fx_fixings` for MTM XCS should"):
-           _ = XCS(dt(2022, 2, 1), "8M", "M", fx_fixings=None)
+            _ = XCS(dt(2022, 2, 1), "8M", "M", fx_fixings=None)
 
         with pytest.raises(ValueError, match="`fx_fixings` for MTM XCS should"):
-           _ = FixedFloatXCS(dt(2022, 2, 1), "8M", "M", fx_fixings=None)
+            _ = FixedFloatXCS(dt(2022, 2, 1), "8M", "M", fx_fixings=None)
 
         with pytest.raises(ValueError, match="`fx_fixings` for MTM XCS should"):
-           _ = FixedFixedXCS(dt(2022, 2, 1), "8M", "M", fx_fixings=None)
+            _ = FixedFixedXCS(dt(2022, 2, 1), "8M", "M", fx_fixings=None)
 
         with pytest.raises(ValueError, match="`fx_fixings` for MTM XCS should"):
-           _ = FloatFixedXCS(dt(2022, 2, 1), "8M", "M", fx_fixings=None)
+            _ = FloatFixedXCS(dt(2022, 2, 1), "8M", "M", fx_fixings=None)
 
-    @pytest.mark.parametrize("float_spd, compound, expected", [
-        (10, "none_simple", 9.97839804),
-        (100, "none_simple", 99.78398037),
-        (100, "isda_compounding", 101.00),
-    ])
+    @pytest.mark.parametrize(
+        "float_spd, compound, expected",
+        [
+            (10, "none_simple", 9.97839804),
+            (100, "none_simple", 99.78398037),
+            (100, "isda_compounding", 99.418428),
+            (100, "isda_flat_compounding", 99.621117),
+        ],
+    )
     def test_mtmxcs_rate(self, float_spd, compound, expected, curve, curve2):
         fxf = FXForwards(
             FXRates({"usdnok": 10}, settlement=dt(2022, 1, 3)),
-            {"usdusd": curve, "nokusd": curve2, "noknok": curve2}
+            {"usdusd": curve, "nokusd": curve2, "noknok": curve2},
         )
 
-        xcs = XCS(dt(2022, 2, 1), "8M", "M",
-                        payment_lag=0, currency="nok", leg2_currency="usd",
-                        payment_lag_exchange=0, notional=10e6,
-                        float_spread=float_spd, leg2_spread_compound_method=compound)
+        xcs = XCS(
+            dt(2022, 2, 1),
+            "8M",
+            "M",
+            payment_lag=0,
+            currency="nok",
+            leg2_currency="usd",
+            payment_lag_exchange=0,
+            notional=10e6,
+            float_spread=float_spd,
+            leg2_spread_compound_method=compound,
+        )
 
         result = xcs.rate([curve2, curve2, curve, curve], None, fxf, 2)
         assert abs(result - expected) < 1e-4
         alias = xcs.spread([curve2, curve2, curve, curve], None, fxf, 2)
         assert alias == result
 
         xcs.leg2_float_spread = result
         validate = xcs.npv([curve2, curve2, curve, curve], None, fxf)
         assert abs(validate) < 1e-2
         result2 = xcs.rate([curve2, curve2, curve, curve], None, fxf, 2)
-        assert abs(result - result2) < 1e-9
+        assert abs(result - result2) < 1e-3
 
 
 class TestFixedFloatXCS:
-
     def test_mtmfixxcs_rate(self, curve, curve2):
         fxf = FXForwards(
             FXRates({"usdnok": 10}, settlement=dt(2022, 1, 3)),
-            {"usdusd": curve, "nokusd": curve2, "noknok": curve2}
+            {"usdusd": curve, "nokusd": curve2, "noknok": curve2},
         )
 
-        xcs = FixedFloatXCS(dt(2022, 2, 1), "8M", "M",
-                        payment_lag=0, currency="nok", leg2_currency="usd",
-                        payment_lag_exchange=0, notional=10e6)
+        xcs = FixedFloatXCS(
+            dt(2022, 2, 1),
+            "8M",
+            "M",
+            payment_lag=0,
+            currency="nok",
+            leg2_currency="usd",
+            payment_lag_exchange=0,
+            notional=10e6,
+        )
 
         result = xcs.rate([curve2, curve2, curve, curve], None, fxf, 1)
 
         irs = IRS(dt(2022, 2, 1), "8M", "M", currency="nok", payment_lag=0)
         validate = irs.rate(curve2)
         assert abs(result - validate) < 1e-4
         # alias = xcs.spread([curve2, curve2, curve, curve], None, fxf, 2)
 
     def test_mtmfixxcs_rate_reversed(self, curve, curve2):
         fxf = FXForwards(
             FXRates({"usdnok": 10}, settlement=dt(2022, 1, 3)),
-            {"usdusd": curve, "nokusd": curve2, "noknok": curve2}
+            {"usdusd": curve, "nokusd": curve2, "noknok": curve2},
         )
 
-        xcs = FloatFixedXCS(dt(2022, 2, 1), "8M", "M",
-                        payment_lag=0, currency="usd", leg2_currency="nok",
-                        payment_lag_exchange=0, notional=10e6)
+        xcs = FloatFixedXCS(
+            dt(2022, 2, 1),
+            "8M",
+            "M",
+            payment_lag=0,
+            currency="usd",
+            leg2_currency="nok",
+            payment_lag_exchange=0,
+            notional=10e6,
+        )
 
         result = xcs.rate([curve, curve, curve2, curve2], None, fxf, 2)
 
         irs = IRS(dt(2022, 2, 1), "8M", "M", currency="nok", payment_lag=0)
         validate = irs.rate(curve2)
         assert abs(result - validate) < 1e-2
         alias = xcs.spread([curve, curve, curve2, curve2], None, fxf, 2)
         assert abs(result - alias) < 1e-4
 
 
 class TestFixedFixedXCS:
-
     def test_mtmfixfixxcs_rate(self, curve, curve2):
         fxf = FXForwards(
             FXRates({"usdnok": 10}, settlement=dt(2022, 1, 3)),
-            {"usdusd": curve, "nokusd": curve2, "noknok": curve2}
+            {"usdusd": curve, "nokusd": curve2, "noknok": curve2},
         )
 
         irs = IRS(dt(2022, 2, 1), "8M", "M", payment_lag=0)
         nok_rate = float(irs.rate(curve2))
-        xcs = FixedFixedXCS(dt(2022, 2, 1), "8M", "M",
-                        payment_lag=0, currency="nok", leg2_currency="usd",
-                        payment_lag_exchange=0, notional=10e6,
-                        fixed_rate=nok_rate)
+        xcs = FixedFixedXCS(
+            dt(2022, 2, 1),
+            "8M",
+            "M",
+            payment_lag=0,
+            currency="nok",
+            leg2_currency="usd",
+            payment_lag_exchange=0,
+            notional=10e6,
+            fixed_rate=nok_rate,
+        )
         result = xcs.rate([curve2, curve2, curve, curve], None, fxf, 2)
         validate = irs.rate(curve)
         assert abs(result - validate) < 1e-4
         alias = xcs.spread([curve2, curve2, curve, curve], None, fxf, 2)
         assert abs(result - alias) < 1e-8
 
         ## test reverse
@@ -934,44 +1553,85 @@
         validate = irs.rate(curve2)
         assert abs(result - validate) < 1e-4
         alias = xcs.spread([curve2, curve2, curve, curve], None, fxf, 1)
         assert abs(result - alias) < 1e-8
 
 
 class TestFXSwap:
-
     def test_fxswap_rate(self, curve, curve2):
         fxf = FXForwards(
             FXRates({"usdnok": 10}, settlement=dt(2022, 1, 3)),
-            {"usdusd": curve, "nokusd": curve2, "noknok": curve2}
+            {"usdusd": curve, "nokusd": curve2, "noknok": curve2},
+        )
+        fxs = FXSwap(
+            dt(2022, 2, 1),
+            "8M",
+            "M",
+            currency="usd",
+            leg2_currency="nok",
+            payment_lag_exchange=0,
+            notional=1e6,
         )
-        fxs = FXSwap(dt(2022, 2, 1), "8M", "M",
-                            currency="usd", leg2_currency="nok",
-                            payment_lag_exchange=0, notional=1e6,
-                            )
         expected = fxf.swap("usdnok", [dt(2022, 2, 1), dt(2022, 10, 1)])
         result = fxs.rate([None, curve, None, curve2], None, fxf)
         assert result == expected
 
     def test_fxswap_npv(self, curve, curve2):
         fxf = FXForwards(
             FXRates({"usdnok": 10}, settlement=dt(2022, 1, 3)),
-            {"usdusd": curve, "nokusd": curve2, "noknok": curve2}
+            {"usdusd": curve, "nokusd": curve2, "noknok": curve2},
+        )
+        fxs = FXSwap(
+            dt(2022, 2, 1),
+            "8M",
+            "M",
+            currency="usd",
+            leg2_currency="nok",
+            payment_lag_exchange=0,
+            notional=1e6,
         )
-        fxs = FXSwap(dt(2022, 2, 1), "8M", "M",
-                            currency="usd", leg2_currency="nok",
-                            payment_lag_exchange=0, notional=1e6,
-                            )
 
         assert abs(fxs.npv([None, curve, None, curve2], None, fxf)) < 1e-7
 
         result = fxs.rate([None, curve, None, curve2], None, fxf, fixed_rate=True)
         fxs.leg2_fixed_rate = result
         assert abs(fxs.npv([None, curve, None, curve2], None, fxf)) < 1e-7
 
+    def test_fxswap_points_raises(self):
+        with pytest.raises(ValueError, match="Cannot set `points` on FXSwap without"):
+            fxs = FXSwap(
+                dt(2022, 2, 1),
+                "8M",
+                "M",
+                points=1000.0,
+                currency="usd",
+                leg2_currency="nok",
+                payment_lag_exchange=0,
+                notional=1e6,
+            )
+
+    def test_fxswap_fixing_and_points(self, curve, curve2):
+        fxf = FXForwards(
+            FXRates({"usdnok": 10}, settlement=dt(2022, 1, 3)),
+            {"usdusd": curve, "nokusd": curve2, "noknok": curve2},
+        )
+        fxs = FXSwap(
+            dt(2022, 2, 1),
+            "8M",
+            "M",
+            fx_fixing=11.0,
+            points=1754.56233604,
+            currency="usd",
+            leg2_currency="nok",
+            payment_lag_exchange=0,
+            notional=1e6,
+        )
+        npv = fxs.npv([None, curve, None, curve2], None, fxf)
+        assert abs(npv + 4166.37288388) < 1e-4
+
     # def test_proxy_curve_from_fxf(self, curve, curve2):
     #     # TODO this needs a solver from which to test the proxy curve (line 92)
     #     fxf = FXForwards(
     #         FXRates({"usdnok": 10}, settlement=dt(2022, 1, 3)),
     #         {"usdusd": curve, "nokusd": curve2, "noknok": curve2}
     #     )
     #     fxs = FXSwap(dt(2022, 2, 1), "8M", "M",
@@ -982,112 +1642,166 @@
     #     npv_usd = fxs.npv([None, curve, None, fxf.curve("nok", "usd")], None, fxf)
     #     assert abs(npv_nok-npv_usd) < 1e-7  # npvs are equivalent becasue xcs basis =0
 
 
 class TestFixedRateBond:
     def test_fixed_rate_bond_price(self):
         # test pricing functions against Gilt Example prices from UK DMO
-        bond = FixedRateBond(dt(1995, 1, 1), dt(2015, 12, 7), "S", convention="ActActICMA",
-                             fixed_rate=8, ex_div=7, calendar="ldn")
+        bond = FixedRateBond(
+            dt(1995, 1, 1),
+            dt(2015, 12, 7),
+            "S",
+            convention="ActActICMA",
+            fixed_rate=8,
+            ex_div=7,
+            calendar="ldn",
+        )
         assert bond.price(4.445, dt(1999, 5, 24), True) - 145.012268 < 1e-6
         assert bond.price(4.445, dt(1999, 5, 26), True) - 145.047301 < 1e-6
         assert bond.price(4.445, dt(1999, 5, 27), True) - 141.070132 < 1e-6
         assert bond.price(4.445, dt(1999, 6, 7), True) - 141.257676 < 1e-6
 
-        bond = FixedRateBond(dt(1997, 1, 1), dt(2004, 11, 26), "S", convention="ActActICMA",
-                             fixed_rate=6.75, ex_div=7, calendar="ldn")
+        bond = FixedRateBond(
+            dt(1997, 1, 1),
+            dt(2004, 11, 26),
+            "S",
+            convention="ActActICMA",
+            fixed_rate=6.75,
+            ex_div=7,
+            calendar="ldn",
+        )
         assert bond.price(4.634, dt(1999, 5, 10), True) - 113.315543 < 1e-6
         assert bond.price(4.634, dt(1999, 5, 17), True) - 113.415969 < 1e-6
         assert bond.price(4.634, dt(1999, 5, 18), True) - 110.058738 < 1e-6
         assert bond.price(4.634, dt(1999, 5, 26), True) - 110.170218 < 1e-6
 
     def test_fixed_rate_bond_yield(self):
         # test pricing functions against Gilt Example prices from UK DMO
-        bond = FixedRateBond(dt(1995, 1, 1), dt(2015, 12, 7), "S", convention="ActActICMA",
-                             fixed_rate=8, ex_div=7, calendar="ldn")
-        assert bond.ytm(135., dt(1999, 5, 24), True) - 5.1620635 < 1e-6
-        assert bond.ytm(135., dt(1999, 5, 26), True) - 5.1649111 < 1e-6
-        assert bond.ytm(135., dt(1999, 5, 27), True) - 4.871425 < 1e-6
-        assert bond.ytm(135., dt(1999, 6, 7), True) - 4.8856785 < 1e-6
-
-        bond = FixedRateBond(dt(1997, 1, 1), dt(2004, 11, 26), "S", convention="ActActICMA",
-                             fixed_rate=6.75, ex_div=7, calendar="ldn")
-        assert bond.ytm(108., dt(1999, 5, 10), True) - 5.7009527 < 1e-6
-        assert bond.ytm(108., dt(1999, 5, 17), True) - 5.7253361 < 1e-6
-        assert bond.ytm(108., dt(1999, 5, 18), True) - 5.0413308 < 1e-6
-        assert bond.ytm(108., dt(1999, 5, 26), True) - 5.0652248 < 1e-6
+        bond = FixedRateBond(
+            dt(1995, 1, 1),
+            dt(2015, 12, 7),
+            "S",
+            convention="ActActICMA",
+            fixed_rate=8,
+            ex_div=7,
+            calendar="ldn",
+        )
+        assert bond.ytm(135.0, dt(1999, 5, 24), True) - 5.1620635 < 1e-6
+        assert bond.ytm(135.0, dt(1999, 5, 26), True) - 5.1649111 < 1e-6
+        assert bond.ytm(135.0, dt(1999, 5, 27), True) - 4.871425 < 1e-6
+        assert bond.ytm(135.0, dt(1999, 6, 7), True) - 4.8856785 < 1e-6
+
+        bond = FixedRateBond(
+            dt(1997, 1, 1),
+            dt(2004, 11, 26),
+            "S",
+            convention="ActActICMA",
+            fixed_rate=6.75,
+            ex_div=7,
+            calendar="ldn",
+        )
+        assert bond.ytm(108.0, dt(1999, 5, 10), True) - 5.7009527 < 1e-6
+        assert bond.ytm(108.0, dt(1999, 5, 17), True) - 5.7253361 < 1e-6
+        assert bond.ytm(108.0, dt(1999, 5, 18), True) - 5.0413308 < 1e-6
+        assert bond.ytm(108.0, dt(1999, 5, 26), True) - 5.0652248 < 1e-6
 
     def test_fixed_rate_bond_yield_domains(self):
-        bond = FixedRateBond(dt(1995, 1, 1), dt(2015, 12, 7), "S",
-                             convention="ActActICMA",
-                             fixed_rate=8, ex_div=7, calendar="ldn")
-        assert bond.ytm(500., dt(1999, 5, 24), True) + 5.86484231333 < 1e-8
+        bond = FixedRateBond(
+            dt(1995, 1, 1),
+            dt(2015, 12, 7),
+            "S",
+            convention="ActActICMA",
+            fixed_rate=8,
+            ex_div=7,
+            calendar="ldn",
+        )
+        assert bond.ytm(500.0, dt(1999, 5, 24), True) + 5.86484231333 < 1e-8
         assert bond.ytm(200, dt(1999, 5, 24), True) - 1.4366895440550 < 1e-8
         assert bond.ytm(100, dt(1999, 5, 24), True) - 8.416909601459 < 1e-8
         assert bond.ytm(50, dt(1999, 5, 24), True) - 18.486840866431 < 1e-6
         assert bond.ytm(1, dt(1999, 5, 24), True) - 13421775210.82037 < 1e-3
 
     def test_fixed_rate_bond_ytm_duals(self):
-        bond = FixedRateBond(dt(1995, 1, 1), dt(2015, 12, 7), "S", convention="ActActICMA",
-                             fixed_rate=8, ex_div=7, calendar="ldn")
+        bond = FixedRateBond(
+            dt(1995, 1, 1),
+            dt(2015, 12, 7),
+            "S",
+            convention="ActActICMA",
+            fixed_rate=8,
+            ex_div=7,
+            calendar="ldn",
+        )
 
         dPdy = bond.duration(4, dt(1995, 1, 1))
         P = bond.price(4, dt(1995, 1, 1))
         result = bond.ytm(Dual(P, ["a", "b"], [1, -0.5]), dt(1995, 1, 1))
         assert result == Dual(4.00, ["a", "b"], [-1 / dPdy, 0.5 / dPdy])
 
-        d2ydP2 = - bond.convexity(4, dt(1995, 1, 1)) * -dPdy ** -3
+        d2ydP2 = -bond.convexity(4, dt(1995, 1, 1)) * -(dPdy**-3)
         result = bond.ytm(Dual2(P, ["a", "b"], [1, -0.5]), dt(1995, 1, 1))
         expected = Dual2(
             4.00,
             ["a", "b"],
             [-1 / dPdy, 0.5 / dPdy],
-            0.5 * np.array([[d2ydP2, d2ydP2 * -0.5], [d2ydP2 * -0.5, d2ydP2 * 0.25]])
+            0.5 * np.array([[d2ydP2, d2ydP2 * -0.5], [d2ydP2 * -0.5, d2ydP2 * 0.25]]),
         )
         assert result == expected
 
     def test_fixed_rate_bond_accrual(self):
         # test pricing functions against Gilt Example prices from UK DMO, with stub
-        bond = FixedRateBond(dt(1999, 5, 7), dt(2002, 12, 7), "S",  convention="ActActICMA",
-                             front_stub=dt(1999, 12, 7),
-                             fixed_rate=6, ex_div=7, calendar="ldn")
+        bond = FixedRateBond(
+            dt(1999, 5, 7),
+            dt(2002, 12, 7),
+            "S",
+            convention="ActActICMA",
+            front_stub=dt(1999, 12, 7),
+            fixed_rate=6,
+            ex_div=7,
+            calendar="ldn",
+        )
         bond.accrued(dt(1999, 5, 8)) == 0.016484
         bond.accrued(dt(1999, 6, 8)) == 0.527382
         bond.accrued(dt(1999, 7, 8)) == 1.019186
         bond.accrued(dt(1999, 11, 8)) == 3.035579
         bond.accrued(dt(1999, 11, 26)) == 3.330661
         bond.accrued(dt(1999, 11, 27)) == -0.16393
         bond.accrued(dt(1999, 12, 6)) == -0.01639
         bond.accrued(dt(1999, 12, 7)) == 0.0
 
     def test_fixed_rate_bond_stub_ytm(self):
         # if a regular bond is set to stub similar output should be gotten
-        bond = FixedRateBond(dt(1999, 6, 7), dt(2002, 12, 7), "S",
-                             convention="ActActICMA",
-                             fixed_rate=6, ex_div=7, calendar="ldn")
+        bond = FixedRateBond(
+            dt(1999, 6, 7),
+            dt(2002, 12, 7),
+            "S",
+            convention="ActActICMA",
+            fixed_rate=6,
+            ex_div=7,
+            calendar="ldn",
+        )
         regular_ytm = bond.ytm(101, dt(1999, 11, 8), dirty=True)
         bond.leg1.periods[0].stub = True
         stubbed_ytm = bond.ytm(101, dt(1999, 11, 8), dirty=True)
         assert regular_ytm == stubbed_ytm
 
     def test_fixed_rate_bond_zero_frequency_raises(self):
         with pytest.raises(ValueError, match="FixedRateBond `frequency`"):
-            FixedRateBond(dt(1999, 5, 7), dt(2002, 12, 7), "Z",  convention="ActActICMA")
+            FixedRateBond(dt(1999, 5, 7), dt(2002, 12, 7), "Z", convention="ActActICMA")
 
     @pytest.mark.parametrize("metric", ["risk", "duration", "modified"])
     def test_fixed_rate_bond_duration(self, metric):
         gilt = FixedRateBond(
             effective=dt(1998, 12, 7),
             termination=dt(2015, 12, 7),
             frequency="S",
             calendar="ldn",
             currency="gbp",
             convention="ActActICMA",
             ex_div=7,
-            fixed_rate=8.0
+            fixed_rate=8.0,
         )
         price0 = gilt.price(4.445, dt(1999, 5, 27))
         price1 = gilt.price(4.446, dt(1999, 5, 27))
         if metric == "risk":
             numeric = price0 - price1
         elif metric == "modified":
             numeric = (price0 - price1) / price0 * 100
@@ -1102,18 +1816,19 @@
             effective=dt(1998, 12, 7),
             termination=dt(2015, 12, 7),
             frequency="S",
             calendar="ldn",
             currency="gbp",
             convention="ActActICMA",
             ex_div=7,
-            fixed_rate=8.0
+            fixed_rate=8.0,
+        )
+        numeric = gilt.duration(4.445, dt(1999, 5, 27)) - gilt.duration(
+            4.446, dt(1999, 5, 27)
         )
-        numeric = gilt.duration(4.445, dt(1999, 5, 27)) - \
-                  gilt.duration(4.446, dt(1999, 5, 27))
         result = gilt.convexity(4.445, dt(1999, 5, 27))
         assert (result - numeric * 1000) < 1e-3
 
     def test_fixed_rate_bond_rate(self):
         gilt = FixedRateBond(
             effective=dt(1998, 12, 7),
             termination=dt(2015, 12, 7),
@@ -1168,18 +1883,16 @@
         assert abs(result - expected) < 1e-6
 
         result = gilt.npv(curve, local=True)
         assert abs(result["gbp"] - expected) < 1e-6
 
     def test_fixed_rate_bond_npv_private(self):
         # this test shadows 'fixed_rate_bond_npv' but extends it for projection
-        curve = Curve({
-            dt(2004, 11, 25): 1.0,
-            dt(2010, 11, 25): 1.0,
-            dt(2015, 12, 7): 0.75}
+        curve = Curve(
+            {dt(2004, 11, 25): 1.0, dt(2010, 11, 25): 1.0, dt(2015, 12, 7): 0.75}
         )
         gilt = FixedRateBond(
             effective=dt(1998, 12, 7),
             termination=dt(2015, 12, 7),
             frequency="S",
             calendar="ldn",
             currency="gbp",
@@ -1271,21 +1984,24 @@
                 frequency="S",
                 calendar="ldn",
                 currency="gbp",
                 convention="ActActICMA",
                 ex_div=7,
                 fixed_rate=8.0,
                 notional=-100,
-                amortization=100
+                amortization=100,
             )
 
-    @pytest.mark.parametrize("f_s, exp", [
-        (dt(2001, 12, 31), 99.997513754),  # compounding of mid year coupon
-        (dt(2002, 1, 1), 99.9975001688)  # this is now ex div on last coupon
-    ])
+    @pytest.mark.parametrize(
+        "f_s, exp",
+        [
+            (dt(2001, 12, 31), 99.997513754),  # compounding of mid year coupon
+            (dt(2002, 1, 1), 99.9975001688),  # this is now ex div on last coupon
+        ],
+    )
     def test_fixed_rate_bond_forward_price_analogue(self, f_s, exp):
         gilt = FixedRateBond(
             effective=dt(2001, 1, 1),
             termination=dt(2002, 1, 1),
             frequency="S",
             calendar=None,
             currency="gbp",
@@ -1294,18 +2010,21 @@
             fixed_rate=1.0,
             notional=-100,
             settle=0,
         )
         result = gilt.fwd_from_repo(100.0, dt(2001, 1, 1), f_s, 1.0, "act365f")
         assert abs(result - exp) < 1e-6
 
-    @pytest.mark.parametrize("f_s, exp", [
-        (dt(2001, 12, 31), 100.49888361793),  # compounding of mid year coupon
-        (dt(2002, 1, 1), 99.9975001688)  # this is now ex div on last coupon
-    ])
+    @pytest.mark.parametrize(
+        "f_s, exp",
+        [
+            (dt(2001, 12, 31), 100.49888361793),  # compounding of mid year coupon
+            (dt(2002, 1, 1), 99.9975001688),  # this is now ex div on last coupon
+        ],
+    )
     def test_fixed_rate_bond_forward_price_analogue_dirty(self, f_s, exp):
         gilt = FixedRateBond(
             effective=dt(2001, 1, 1),
             termination=dt(2002, 1, 1),
             frequency="S",
             calendar=None,
             currency="gbp",
@@ -1316,20 +2035,23 @@
             settle=0,
         )
         result = gilt.fwd_from_repo(
             100.0, dt(2001, 1, 1), f_s, 1.0, "act365f", dirty=True
         )
         assert abs(result - exp) < 1e-6
 
-    @pytest.mark.parametrize("s, f_s, exp", [
-        (dt(2010, 11, 25), dt(2011, 11, 25), 99.9975000187),
-        (dt(2010, 11, 28), dt(2011, 11, 28), 99.9975000187),
-        (dt(2010, 11, 28), dt(2011, 11, 25), 99.997419419),
-        (dt(2010, 11, 25), dt(2011, 11, 28), 99.997579958),
-    ])
+    @pytest.mark.parametrize(
+        "s, f_s, exp",
+        [
+            (dt(2010, 11, 25), dt(2011, 11, 25), 99.9975000187),
+            (dt(2010, 11, 28), dt(2011, 11, 28), 99.9975000187),
+            (dt(2010, 11, 28), dt(2011, 11, 25), 99.997419419),
+            (dt(2010, 11, 25), dt(2011, 11, 28), 99.997579958),
+        ],
+    )
     def test_fixed_rate_bond_forward_price_analogue_ex_div(self, s, f_s, exp):
         gilt = FixedRateBond(
             effective=dt(1998, 12, 7),
             termination=dt(2015, 12, 7),
             frequency="S",
             calendar="ldn",
             currency="gbp",
@@ -1338,18 +2060,21 @@
             fixed_rate=1.0,
             notional=-100,
             settle=0,
         )
         result = gilt.fwd_from_repo(100.0, s, f_s, 1.0, "act365f")
         assert abs(result - exp) < 1e-6
 
-    @pytest.mark.parametrize("f_s, f_p", [
-        (dt(2001, 12, 31), 99.997513754),  # compounding of mid year coupon
-        (dt(2002, 1, 1), 99.9975001688)  # this is now ex div on last coupon
-    ])
+    @pytest.mark.parametrize(
+        "f_s, f_p",
+        [
+            (dt(2001, 12, 31), 99.997513754),  # compounding of mid year coupon
+            (dt(2002, 1, 1), 99.9975001688),  # this is now ex div on last coupon
+        ],
+    )
     def test_fixed_rate_bond_implied_repo(self, f_s, f_p):
         gilt = FixedRateBond(
             effective=dt(2001, 1, 1),
             termination=dt(2002, 1, 1),
             frequency="S",
             calendar=None,
             currency="gbp",
@@ -1358,18 +2083,21 @@
             fixed_rate=1.0,
             notional=-100,
             settle=0,
         )
         result = gilt.repo_from_fwd(100.0, dt(2001, 1, 1), f_s, f_p, "act365f")
         assert abs(result - 1.00) < 1e-8
 
-    @pytest.mark.parametrize("f_s, f_p", [
-        (dt(2001, 12, 31), 100.49888361793),  # compounding of mid year coupon
-        (dt(2002, 1, 1), 99.9975001688)  # this is now ex div on last coupon
-    ])
+    @pytest.mark.parametrize(
+        "f_s, f_p",
+        [
+            (dt(2001, 12, 31), 100.49888361793),  # compounding of mid year coupon
+            (dt(2002, 1, 1), 99.9975001688),  # this is now ex div on last coupon
+        ],
+    )
     def test_fixed_rate_bond_implied_repo_analogue_dirty(self, f_s, f_p):
         gilt = FixedRateBond(
             effective=dt(2001, 1, 1),
             termination=dt(2002, 1, 1),
             frequency="S",
             calendar=None,
             currency="gbp",
@@ -1381,16 +2109,263 @@
         )
         result = gilt.repo_from_fwd(
             100.0, dt(2001, 1, 1), f_s, f_p, "act365f", dirty=True
         )
         assert abs(result - 1.0) < 1e-8
 
 
-class TestBill:
+class TestIndexFixedRateBond:
+
+    def test_fixed_rate_bond_price(self):
+        # test pricing functions against Nominal Gilt Example prices from UK DMO
+        # these prices should be equivalent for the REAL component of Index Bonds
+        bond = IndexFixedRateBond(
+            dt(1995, 1, 1),
+            dt(2015, 12, 7),
+            "S",
+            convention="ActActICMA",
+            fixed_rate=8,
+            ex_div=7,
+            calendar="ldn",
+            index_base=100.0,
+        )
+        assert bond.price(4.445, dt(1999, 5, 24), True) - 145.012268 < 1e-6
+        assert bond.price(4.445, dt(1999, 5, 26), True) - 145.047301 < 1e-6
+        assert bond.price(4.445, dt(1999, 5, 27), True) - 141.070132 < 1e-6
+        assert bond.price(4.445, dt(1999, 6, 7), True) - 141.257676 < 1e-6
+
+        bond = IndexFixedRateBond(
+            dt(1997, 1, 1),
+            dt(2004, 11, 26),
+            "S",
+            convention="ActActICMA",
+            fixed_rate=6.75,
+            ex_div=7,
+            calendar="ldn",
+            index_base=100.0
+        )
+        assert bond.price(4.634, dt(1999, 5, 10), True) - 113.315543 < 1e-6
+        assert bond.price(4.634, dt(1999, 5, 17), True) - 113.415969 < 1e-6
+        assert bond.price(4.634, dt(1999, 5, 18), True) - 110.058738 < 1e-6
+        assert bond.price(4.634, dt(1999, 5, 26), True) - 110.170218 < 1e-6
+
+    def test_fixed_rate_bond_zero_frequency_raises(self):
+        with pytest.raises(ValueError, match="FixedRateBond `frequency`"):
+            IndexFixedRateBond(
+                dt(1999, 5, 7), dt(2002, 12, 7), "Z", convention="ActActICMA"
+            )
+
+    def test_fixed_rate_bond_no_amortization(self):
+        with pytest.raises(NotImplementedError, match="`amortization` for"):
+            gilt = IndexFixedRateBond(
+                effective=dt(1998, 12, 7),
+                termination=dt(2015, 12, 7),
+                frequency="S",
+                calendar="ldn",
+                currency="gbp",
+                convention="ActActICMA",
+                ex_div=7,
+                fixed_rate=8.0,
+                notional=-100,
+                amortization=100,
+                index_base=100.0
+            )
 
+    def test_fixed_rate_bond_rate_raises(self):
+        gilt = IndexFixedRateBond(
+            effective=dt(1998, 12, 7),
+            termination=dt(2015, 12, 7),
+            frequency="S",
+            calendar="ldn",
+            currency="gbp",
+            convention="ActActICMA",
+            ex_div=7,
+            fixed_rate=8.0,
+            notional=-100,
+            index_base=100.0,
+        )
+        curve = Curve({dt(1998, 12, 7): 1.0, dt(2015, 12, 7): 0.50})
+        with pytest.raises(ValueError, match="`metric` must be in"):
+            gilt.rate(curve, metric="bad_metric")
+
+        with pytest.raises(ValueError, match="`forward_settlement` needed to"):
+            gilt.rate(curve, metric="fwd_clean_price")
+
+    @pytest.mark.parametrize("i_fixings, expected", [
+        (None, 1.161227269),
+        (Series([90, 290], index=[dt(2022, 4, 1), dt(2022, 4, 29)]), 2.00)
+    ])
+    def test_index_ratio(self, i_fixings, expected):
+        i_curve = IndexCurve(
+            {dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99},
+            index_lag=3,
+            index_base=110.0,
+        )
+        bond = IndexFixedRateBond(
+            dt(2022, 1, 1),
+            "9m",
+            "Q",
+            convention="ActActICMA",
+            fixed_rate=4,
+            ex_div=0,
+            calendar="ldn",
+            index_base=95.0,
+            index_fixings=i_fixings,
+            index_method="daily",
+        )
+        result = bond.index_ratio(settlement=dt(2022, 4, 15), curve=i_curve)
+        assert abs(result-expected) < 1e-5
+
+    def test_index_ratio_raises_float_index_fixings(self):
+        i_curve = IndexCurve(
+            {dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99},
+            index_lag=3,
+            index_base=110.0,
+        )
+        bond = IndexFixedRateBond(
+            dt(2022, 1, 1),
+            "9m",
+            "Q",
+            convention="ActActICMA",
+            fixed_rate=4,
+            ex_div=0,
+            calendar="ldn",
+            index_base=95.0,
+            index_fixings=[100.0, 200.0],
+            index_method="daily",
+        )
+        with pytest.raises(ValueError, match="Must provide `index_fixings` as a Seri"):
+            bond.index_ratio(settlement=dt(2022, 4, 15), curve=i_curve)
+
+    def test_fixed_rate_bond_npv_private(self):
+        # this test shadows 'fixed_rate_bond_npv' but extends it for projection
+        curve = Curve(
+            {dt(2004, 11, 25): 1.0, dt(2010, 11, 25): 1.0, dt(2015, 12, 7): 0.75}
+        )
+        index_curve = IndexCurve(
+            {dt(2004, 11, 25): 1.0, dt(2034, 1, 1): 1.0}, index_base=100.0
+        )
+        gilt = IndexFixedRateBond(
+            effective=dt(1998, 12, 7),
+            termination=dt(2015, 12, 7),
+            frequency="S",
+            calendar="ldn",
+            currency="gbp",
+            convention="ActActICMA",
+            ex_div=7,
+            fixed_rate=8.0,
+            notional=-100,
+            settle=0,
+            index_base=50.0,
+            index_lag=3,
+            index_method="daily",
+        )
+        result = gilt._npv_local(
+            index_curve, curve, None, None, dt(2010, 11, 26), dt(2010, 11, 25)
+        )
+        expected = 109.229489312983 * 2.0 # npv should match associated test
+        assert abs(result - expected) < 1e-6
+
+    def test_index_base_forecast(self, curve):
+        i_curve = IndexCurve(
+            {dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99},
+            index_lag=3,
+            index_base=95.0,
+        )
+        bond = IndexFixedRateBond(
+            dt(2022, 1, 1),
+            "9m",
+            "Q",
+            convention="ActActICMA",
+            fixed_rate=4,
+            ex_div=0,
+            calendar=None,
+            index_method="daily",
+            settle=0,
+        )
+        cashflows = bond.cashflows([i_curve, curve])
+        for i in range(4):
+            assert cashflows.iloc[i]["Index Base"] == 95.0
+
+        result = bond.npv([i_curve, curve])
+        expected = -1006875.3812
+        assert abs(result - expected) < 1e-4
+
+        result = bond.rate([i_curve, curve], metric="index_dirty_price")
+        assert abs(result * -1e4 - expected) < 1e-4
+
+    def test_fixed_rate_bond_fwd_rate(self):
+        gilt = IndexFixedRateBond(
+            effective=dt(1998, 12, 7),
+            termination=dt(2015, 12, 7),
+            frequency="S",
+            calendar="ldn",
+            currency="gbp",
+            convention="ActActICMA",
+            ex_div=7,
+            fixed_rate=8.0,
+            settle=0,
+            index_base=50.0
+        )
+        curve = Curve({dt(1998, 12, 9): 1.0, dt(2015, 12, 7): 0.50})
+        i_curve = IndexCurve(
+            {dt(1998, 12, 9): 1.0, dt(2015, 12, 7): 1.0},
+            index_base=100.0
+        )
+        clean_price = gilt.rate([i_curve, curve], metric="clean_price")
+        index_clean_price = gilt.rate([i_curve, curve], metric="index_clean_price")
+        assert abs(index_clean_price * 0.5 - clean_price) < 1e-3
+
+        result = gilt.rate(
+            [i_curve, curve],
+            metric="fwd_clean_price",
+            forward_settlement=dt(1998, 12, 9)
+        )
+        assert abs(result - clean_price) < 1e-8
+        result = gilt.rate(
+            [i_curve, curve],
+            metric="fwd_index_clean_price",
+            forward_settlement=dt(1998, 12, 9)
+        )
+        assert abs(result * 0.5 - clean_price) < 1e-8
+
+        result = gilt.rate([i_curve, curve], metric="dirty_price")
+        expected = clean_price + gilt.accrued(dt(1998, 12, 9))
+        assert result == expected
+        result = gilt.rate(
+            [i_curve, curve],
+            metric="fwd_dirty_price",
+            forward_settlement=dt(1998, 12, 9)
+        )
+        assert abs(result - clean_price - gilt.accrued(dt(1998, 12, 9))) < 1e-8
+        result = gilt.rate(
+            [i_curve, curve],
+            metric="fwd_index_dirty_price",
+            forward_settlement=dt(1998, 12, 9)
+        )
+        assert abs(result * 0.5 - clean_price - gilt.accrued(dt(1998, 12, 9))) < 1e-8
+
+        result = gilt.rate([i_curve, curve], metric="ytm")
+        expected = gilt.ytm(clean_price, dt(1998, 12, 9), False)
+        assert abs(result - expected) < 1e-8
+
+    def test_fwd_from_repo(self):
+        assert False
+
+    def test_repo_from_fwd(self):
+        assert False
+
+    def test_duration(self):
+        assert False
+
+    def test_convexity(self):
+        assert False
+
+
+class TestBill:
     def test_bill_discount_rate(self):
         # test pricing functions against Treasury Bill Example from US Treasury
         bill = Bill(
             effective=dt(2004, 1, 22),
             termination=dt(2004, 2, 19),
             frequency="A",
             calendar="nyc",
@@ -1400,24 +2375,23 @@
 
         assert bill.discount_rate(99.93777, dt(2004, 1, 22)) == 0.8000999999999543
         assert bill.price(0.800, dt(2004, 1, 22)) == 99.93777777777778
         # this YTM is equivalent to the FixedRateBond ytm with coupon of 0.0
         assert abs(bill.ytm(99.937778, dt(2004, 1, 22)) - 0.8034566609543146) < 1e-9
 
         d = dcf(dt(2004, 1, 22), dt(2004, 2, 19), "Act360")
-        expected = 100 * (1 / (1-0.0080009999999*d) - 1) / d  # floating point truncation
+        expected = (
+            100 * (1 / (1 - 0.0080009999999 * d) - 1) / d
+        )  # floating point truncation
         expected = 100 * (100 / 99.93777777777778 - 1) / d
         result = bill.simple_rate(99.93777777777778, dt(2004, 1, 22))
         assert abs(result - expected) < 1e-6
 
     def test_bill_rate(self):
-        curve = Curve({
-            dt(2004, 1, 22): 1.00,
-            dt(2005, 1, 22): 0.992
-        })
+        curve = Curve({dt(2004, 1, 22): 1.00, dt(2005, 1, 22): 0.992})
 
         bill = Bill(
             effective=dt(2004, 1, 22),
             termination=dt(2004, 2, 19),
             frequency="A",
             calendar="nyc",
             currency="usd",
@@ -1456,18 +2430,15 @@
         assert abs(result - expected) < 1e-6
 
         result = bill.rate(curve, metric="ytm")
         expected = bill.ytm(99.94734388985547, dt(2004, 1, 26))
         assert abs(result - expected) < 1e-6
 
     def test_bill_rate_raises(self):
-        curve = Curve({
-            dt(2004, 1, 22): 1.00,
-            dt(2005, 1, 22): 0.992
-        })
+        curve = Curve({dt(2004, 1, 22): 1.00, dt(2005, 1, 22): 0.992})
 
         bill = Bill(
             effective=dt(2004, 1, 22),
             termination=dt(2004, 2, 19),
             frequency="A",
             calendar="nyc",
             currency="usd",
@@ -1475,31 +2446,33 @@
         )
 
         with pytest.raises(ValueError, match="`metric` must be in"):
             bill.rate(curve, metric="bad vibes")
 
 
 class TestFloatRateBond:
-
-    @pytest.mark.parametrize("curve_spd, method, float_spd, expected", [
-        (10, None, 0, 10.055032859883),
-        (500, None, 0, 508.93107035125325),
-        (-200, None, 0, -200.053341848676),
-        (10, "isda_compounding", 0, 10.00000120),
-        (500, "isda_compounding", 0, 500.050371345),
-        (-200, "isda_compounding", 0, -200.003309580533),
-        (10, None, 25, 10.055032859883),
-        (500, None, 250, 508.93107035125325),
-        (10, "isda_compounding", 25, 10.00000120),
-        (500, "isda_compounding", 250, 500.00635330533544),
-        (10, None, -25, 10.055032859883),
-        (500, None, -250, 508.93107035125325),
-        (10, "isda_compounding", -25, 10.00000120),
-        (500, "isda_compounding", -250, 500.16850637415),
-    ])
+    @pytest.mark.parametrize(
+        "curve_spd, method, float_spd, expected",
+        [
+            (10, None, 0, 10.055032859883),
+            (500, None, 0, 508.93107035125325),
+            (-200, None, 0, -200.053341848676),
+            (10, "isda_compounding", 0, 10.00000120),
+            (500, "isda_compounding", 0, 500.050371345),
+            (-200, "isda_compounding", 0, -200.003309580533),
+            (10, None, 25, 10.055032859883),
+            (500, None, 250, 508.93107035125325),
+            (10, "isda_compounding", 25, 10.00000120),
+            (500, "isda_compounding", 250, 500.00635330533544),
+            (10, None, -25, 10.055032859883),
+            (500, None, -250, 508.93107035125325),
+            (10, "isda_compounding", -25, 10.00000120),
+            (500, "isda_compounding", -250, 500.16850637415),
+        ],
+    )
     def test_float_rate_bond_rate_spread(self, curve_spd, method, float_spd, expected):
         """
         When a DF curve is shifted it bumps daily rates.
         But under the "none_simple" compounding method this does not compound daily
         therefore the `float_spread` should be slightly higher than the bumped curve.
         When the method is "isda_compounding" this closely matches the bumping method
         of the curve.
@@ -1511,49 +2484,43 @@
             frequency="S",
             convention="Act365f",
             ex_div=0,
             settle=0,
             float_spread=float_spd,
             spread_compound_method=method,
         )
-        curve = Curve({
-            dt(2007, 1, 1): 1.0,
-            dt(2017, 1, 1): 0.9
-        }, convention="Act365f"
-        )
+        curve = Curve({dt(2007, 1, 1): 1.0, dt(2017, 1, 1): 0.9}, convention="Act365f")
         disc_curve = curve.shift(curve_spd)
-        result = bond.rate(
-            [curve, disc_curve],
-            metric="spread"
-        )
+        result = bond.rate([curve, disc_curve], metric="spread")
         assert abs(result - expected) < 1e-4
 
         bond.float_spread = result
         validate = bond.npv([curve, disc_curve])
         assert abs(validate + bond.leg1.notional) < 0.30 * abs(curve_spd)
 
-    @pytest.mark.parametrize("curve_spd, method, float_spd, expected", [
-        (10, "isda_compounding", 0, 10.00000120),
-    ])
-    def test_float_rate_bond_rate_spread_fx(self, curve_spd, method, float_spd, expected):
+    @pytest.mark.parametrize(
+        "curve_spd, method, float_spd, expected",
+        [
+            (10, "isda_compounding", 0, 10.00000120),
+        ],
+    )
+    def test_float_rate_bond_rate_spread_fx(
+        self, curve_spd, method, float_spd, expected
+    ):
         bond = FloatRateBond(
             effective=dt(2007, 1, 1),
             termination=dt(2017, 1, 1),
             frequency="S",
             convention="Act365f",
             ex_div=0,
             settle=0,
             float_spread=float_spd,
             spread_compound_method=method,
         )
-        curve = Curve({
-            dt(2007, 1, 1): 1.0,
-            dt(2017, 1, 1): 0.9
-        }, convention="Act365f"
-        )
+        curve = Curve({dt(2007, 1, 1): 1.0, dt(2017, 1, 1): 0.9}, convention="Act365f")
         disc_curve = curve.shift(curve_spd)
         fxr = FXRates({"usdnok": 10.0}, settlement=dt(2007, 1, 1))
         result = bond.rate(
             [curve, disc_curve],
             metric="spread",
             fx=fxr,
         )
@@ -1577,45 +2544,48 @@
             method_param=5,
             spread_compound_method="none_simple",
         )
         result = bond.accrued(dt(2010, 3, 3))
         expected = 0.5019275497883  # approx 2 / 12 * 3%
         assert abs(result - expected) < 1e-8
 
-    @pytest.mark.parametrize("metric, spd, exp", [
-        ("clean_price", 0., 100.),
-        ("dirty_price", 0., 100.),
-        ("clean_price", 10., 99.99982764447981),  # compounding diff between shift
-        ("dirty_price", 10., 100.0165399732469),
-    ])
+    @pytest.mark.parametrize(
+        "metric, spd, exp",
+        [
+            ("clean_price", 0.0, 100.0),
+            ("dirty_price", 0.0, 100.0),
+            ("clean_price", 10.0, 99.99982764447981),  # compounding diff between shift
+            ("dirty_price", 10.0, 100.0165399732469),
+        ],
+    )
     def test_float_rate_bond_rate_metric(self, metric, spd, exp):
         fixings = Series(0.0, index=date_range(dt(2009, 12, 1), dt(2010, 3, 1)))
         bond = FloatRateBond(
             effective=dt(2007, 1, 1),
             termination=dt(2017, 1, 1),
             frequency="S",
             convention="Act365f",
             ex_div=3,
             float_spread=spd,
             fixing_method="rfr_observation_shift",
             fixings=fixings,
             method_param=5,
             spread_compound_method="none_simple",
-            settle=2
+            settle=2,
         )
         curve = Curve({dt(2010, 3, 1): 1.0, dt(2017, 1, 1): 1.0}, convention="act365f")
         disc_curve = curve.shift(spd)
 
         result = bond.rate(curves=[curve, disc_curve], metric=metric)
         assert abs(result - exp) < 1e-8
 
-    @pytest.mark.parametrize("settlement, expected", [
-        (dt(2010, 3, 3), 0.501369863013698),
-        (dt(2010, 12, 30), -0.005479452054)
-    ])
+    @pytest.mark.parametrize(
+        "settlement, expected",
+        [(dt(2010, 3, 3), 0.501369863013698), (dt(2010, 12, 30), -0.005479452054)],
+    )
     def test_float_rate_bond_accrued_ibor(self, settlement, expected):
         fixings = Series(2.0, index=date_range(dt(2009, 12, 1), dt(2010, 3, 1)))
         bond = FloatRateBond(
             effective=dt(2007, 1, 1),
             termination=dt(2017, 1, 1),
             frequency="S",
             convention="Act365f",
@@ -1640,18 +2610,21 @@
                 float_spread=100,
                 fixing_method="rfr_observation_shift",
                 fixings=None,
                 method_param=5,
                 spread_compound_method="none_simple",
             )
 
-    @pytest.mark.parametrize("fixings", [
-        Series(2.0, index=date_range(dt(2009, 12, 1), dt(2010, 3, 8))),
-        [2.0, [2.0, 2.0]],
-    ])
+    @pytest.mark.parametrize(
+        "fixings",
+        [
+            Series(2.0, index=date_range(dt(2009, 12, 1), dt(2010, 3, 8))),
+            [2.0, [2.0, 2.0]],
+        ],
+    )
     def test_negative_accrued_needs_forecasting(self, fixings):
         bond = FloatRateBond(
             effective=dt(2009, 9, 16),
             termination=dt(2017, 3, 16),
             frequency="Q",
             convention="Act365f",
             ex_div=5,
@@ -1661,20 +2634,23 @@
             method_param=5,
             spread_compound_method="none_simple",
             calendar=None,
         )
         result = bond.accrued(dt(2010, 3, 11))
 
         # approximate calculation 5 days of negative accrued at 2% = -0.027397
-        assert abs(result+0.027397) < 1e-3
+        assert abs(result + 0.027397) < 1e-3
 
-    @pytest.mark.parametrize("fixings", [
-        None,
-        [2.0, 2.0],
-    ])
+    @pytest.mark.parametrize(
+        "fixings",
+        [
+            None,
+            [2.0, 2.0],
+        ],
+    )
     def test_negative_accrued_raises(self, fixings):
         bond = FloatRateBond(
             effective=dt(2009, 9, 16),
             termination=dt(2017, 3, 16),
             frequency="Q",
             convention="Act365f",
             ex_div=5,
@@ -1709,149 +2685,167 @@
             fixing_method="rfr_observation_shift",
             fixings=None,
             method_param=0,
             spread_compound_method="none_simple",
             calendar=None,
         )
         result = bond.accrued(dt(2010, 3, 16))
-        assert result == 0.
+        assert result == 0.0
 
     def test_float_rate_bond_analytic_delta(self):
         frn = FloatRateBond(
             effective=dt(2010, 6, 7),
             termination=dt(2015, 12, 7),
             frequency="S",
             calendar="ldn",
             currency="gbp",
             convention="ActActICMA",
             ex_div=7,
             float_spread=100,
             notional=-1000000,
             settle=0,
             fixing_method="ibor",
-            fixings=2.0
+            fixings=2.0,
         )
         curve = Curve({dt(2010, 11, 25): 1.0, dt(2015, 12, 7): 1.0})
         result = frn.analytic_delta(curve)
         expected = -550.0
         assert abs(result - expected) < 1e-6
 
         frn.settle = 1
         result = frn.analytic_delta(curve)  # bond is ex div on settle 26th Nov 2010
         expected = -500.0  # bond has dropped a 6m coupon payment
         assert abs(result - expected) < 1e-6
 
-    @pytest.mark.parametrize("metric, spd, exp", [
-        ("fwd_clean_price", 0., 100),
-        ("fwd_dirty_price", 0., 100),
-        ("fwd_clean_price", 50., 99.99602155150806),
-        ("fwd_dirty_price", 50., 100.03848730493272),
-    ])
+    @pytest.mark.parametrize(
+        "metric, spd, exp",
+        [
+            ("fwd_clean_price", 0.0, 100),
+            ("fwd_dirty_price", 0.0, 100),
+            ("fwd_clean_price", 50.0, 99.99602155150806),
+            ("fwd_dirty_price", 50.0, 100.03848730493272),
+        ],
+    )
     def test_float_rate_bond_forward_prices(self, metric, spd, exp):
         bond = FloatRateBond(
             effective=dt(2007, 1, 1),
             termination=dt(2017, 1, 1),
             frequency="S",
             convention="Act365f",
             ex_div=3,
             float_spread=spd,
             fixing_method="rfr_observation_shift",
             method_param=5,
             spread_compound_method="none_simple",
-            settle=2
+            settle=2,
         )
         curve = Curve({dt(2010, 3, 1): 1.0, dt(2017, 1, 1): 1.0}, convention="act365f")
         disc_curve = curve.shift(spd)
 
         result = bond.rate(
-            curves=[curve, disc_curve],
-            metric=metric,
-            forward_settlement=dt(2010, 8, 1)
+            curves=[curve, disc_curve], metric=metric, forward_settlement=dt(2010, 8, 1)
         )
         assert abs(result - exp) < 1e-8
 
     def test_float_rate_bond_forward_accrued(self):
         bond = FloatRateBond(
             effective=dt(2007, 1, 1),
             termination=dt(2017, 1, 1),
             frequency="S",
             convention="Act365f",
             ex_div=3,
             float_spread=0,
             fixing_method="rfr_observation_shift",
             method_param=5,
             spread_compound_method="none_simple",
-            settle=2
+            settle=2,
         )
         curve = Curve({dt(2010, 3, 1): 1.0, dt(2017, 1, 1): 0.9}, convention="act365f")
         disc_curve = curve.shift(0)
         result = bond.accrued(dt(2010, 8, 1), forecast=True, curve=curve)
         expected = 0.13083715795372267
         assert abs(result - expected) < 1e-8
 
     def test_rate_raises(self):
         bond = FloatRateBond(
             effective=dt(2007, 1, 1),
             termination=dt(2017, 1, 1),
             frequency="S",
             convention="Act365f",
             ex_div=3,
-            float_spread=0.,
+            float_spread=0.0,
             fixing_method="rfr_observation_shift",
             method_param=5,
             spread_compound_method="none_simple",
-            settle=2
+            settle=2,
         )
         with pytest.raises(ValueError, match="`forward_settlement` needed to "):
             bond.rate(None, metric="fwd_clean_price", forward_settlement=None)
 
         with pytest.raises(ValueError, match="`metric` must be in"):
             bond.rate(None, metric="BAD")
 
+    def test_forecast_ibor(self, curve):
+        f_curve = LineCurve({
+            dt(2022, 1, 1): 3.0,
+            dt(2022, 2, 1): 4.0
+        })
+        frn = FloatRateBond(
+            effective=dt(2022, 2, 1),
+            termination="3m",
+            frequency="Q",
+            fixing_method="ibor",
+            method_param=0,
+        )
+        result = frn.accrued(dt(2022, 2, 5), forecast=True, curve=f_curve)
+        expected = 0.044444444
+        assert abs(result - expected) < 1e-4
 
-class TestBondFuture:
 
-    @pytest.mark.parametrize("delivery, mat, coupon, exp", [
-        (dt(2023, 6, 12), dt(2032, 2, 15), 0.0, 0.603058),
-        (dt(2023, 6, 12), dt(2032, 8, 15), 1.7, 0.703125),
-        (dt(2023, 6, 12), dt(2033, 2, 15), 2.3, 0.733943),
-        (dt(2023, 9, 11), dt(2032, 8, 15), 1.7, 0.709321),
-        (dt(2023, 9, 11), dt(2033, 2, 15), 2.3, 0.739087),
-        (dt(2023, 12, 11), dt(2032, 8, 15), 1.7, 0.715464),
-        (dt(2023, 12, 11), dt(2033, 2, 15), 2.3, 0.744390),
-    ])
+class TestBondFuture:
+    @pytest.mark.parametrize(
+        "delivery, mat, coupon, exp",
+        [
+            (dt(2023, 6, 12), dt(2032, 2, 15), 0.0, 0.603058),
+            (dt(2023, 6, 12), dt(2032, 8, 15), 1.7, 0.703125),
+            (dt(2023, 6, 12), dt(2033, 2, 15), 2.3, 0.733943),
+            (dt(2023, 9, 11), dt(2032, 8, 15), 1.7, 0.709321),
+            (dt(2023, 9, 11), dt(2033, 2, 15), 2.3, 0.739087),
+            (dt(2023, 12, 11), dt(2032, 8, 15), 1.7, 0.715464),
+            (dt(2023, 12, 11), dt(2033, 2, 15), 2.3, 0.744390),
+        ],
+    )
     def test_conversion_factors_eurex_bund(self, delivery, mat, coupon, exp):
         # The expected results are downloaded from the EUREX website
         # regarding precalculated conversion factors.
         # this test allows for an error in the cf < 1e-4.
         kwargs = dict(
             effective=dt(2020, 1, 1),
             stub="ShortFront",
             frequency="A",
             calendar="tgt",
             currency="eur",
-            convention="ActActICMA"
+            convention="ActActICMA",
         )
         bond1 = FixedRateBond(termination=mat, fixed_rate=coupon, **kwargs)
 
-        fut = BondFuture(
-            delivery=delivery,
-            coupon=6.0,
-            basket=[bond1]
-        )
+        fut = BondFuture(delivery=delivery, coupon=6.0, basket=[bond1])
         result = fut.cfs
-        assert abs(result[0]-exp) < 1e-4
+        assert abs(result[0] - exp) < 1e-4
 
-    @pytest.mark.parametrize("mat, coupon, exp", [
-        (dt(2032, 6, 7), 4.25, 1.0187757),
-        (dt(2033, 7, 31), 0.875, 0.7410593),
-        (dt(2034, 9, 7), 4.5, 1.0449380),
-        (dt(2035, 7, 31), 0.625, 0.6773884),
-        (dt(2036, 3, 7), 4.25, 1.0247516),
-    ])
+    @pytest.mark.parametrize(
+        "mat, coupon, exp",
+        [
+            (dt(2032, 6, 7), 4.25, 1.0187757),
+            (dt(2033, 7, 31), 0.875, 0.7410593),
+            (dt(2034, 9, 7), 4.5, 1.0449380),
+            (dt(2035, 7, 31), 0.625, 0.6773884),
+            (dt(2036, 3, 7), 4.25, 1.0247516),
+        ],
+    )
     def test_conversion_factors_ice_gilt(self, mat, coupon, exp):
         # The expected results are downloaded from the ICE LIFFE website
         # regarding precalculated conversion factors.
         # this test allows for an error in the cf < 1e-6.
         kwargs = dict(
             effective=dt(2020, 1, 1),
             stub="ShortFront",
@@ -1860,17 +2854,15 @@
             currency="gbp",
             convention="ActActICMA",
             ex_div=7,
         )
         bond1 = FixedRateBond(termination=mat, fixed_rate=coupon, **kwargs)
 
         fut = BondFuture(
-            delivery=(dt(2023, 6, 1), dt(2023, 6, 30)),
-            coupon=4.0,
-            basket=[bond1]
+            delivery=(dt(2023, 6, 1), dt(2023, 6, 30)), coupon=4.0, basket=[bond1]
         )
         result = fut.cfs
         assert abs(result[0] - exp) < 1e-6
 
     def test_dlv_screen_print(self):
         kws = dict(ex_div=7, frequency="S", convention="ActActICMA", calendar=None)
         bonds = [
@@ -1885,47 +2877,45 @@
         result = future.dlv(
             future_price=112.98,
             prices=[102.732, 131.461, 107.877, 134.455],
             repo_rate=6.24,
             settlement=dt(2000, 3, 16),
             convention="Act365f",
         )
-        expected = DataFrame({
-            "Bond": [
-                "5.750% 07-12-2009",
-                "9.000% 12-07-2011",
-                "6.250% 25-11-2010",
-                "9.000% 06-08-2012",
-            ],
-            "Price": [102.732, 131.461, 107.877, 134.455],
-            "YTM": [5.384243, 5.273217, 5.275481, 5.193851],
-            "C.Factor": [0.914225, 1.152571, 0.944931, 1.161956],
-            "Gross Basis": [-0.557192, 1.243582, 1.118677, 3.177230],
-            "Implied Repo": [7.381345, 3.564685, 2.199755, -1.414670],
-            "Actual Repo": [6.24, 6.24, 6.24, 6.24],
-            "Net Basis": [-0.343654, 1.033668, 1.275866, 3.010371],
-        })
+        expected = DataFrame(
+            {
+                "Bond": [
+                    "5.750% 07-12-2009",
+                    "9.000% 12-07-2011",
+                    "6.250% 25-11-2010",
+                    "9.000% 06-08-2012",
+                ],
+                "Price": [102.732, 131.461, 107.877, 134.455],
+                "YTM": [5.384243, 5.273217, 5.275481, 5.193851],
+                "C.Factor": [0.914225, 1.152571, 0.944931, 1.161956],
+                "Gross Basis": [-0.557192, 1.243582, 1.118677, 3.177230],
+                "Implied Repo": [7.381345, 3.564685, 2.199755, -1.414670],
+                "Actual Repo": [6.24, 6.24, 6.24, 6.24],
+                "Net Basis": [-0.343654, 1.033668, 1.275866, 3.010371],
+            }
+        )
         assert_frame_equal(result, expected)
 
         result2 = future.dlv(
             future_price=112.98,
             prices=[102.732, 131.461, 107.877, 134.455],
             repo_rate=[6.24, 6.24, 6.24, 6.24],  # test individual repo input
             settlement=dt(2000, 3, 16),
             convention="Act365f",
         )
         assert_frame_equal(result2, expected)
 
     def test_notional(self):
         future = BondFuture(
-            coupon=0,
-            delivery=dt(2000, 6, 1),
-            basket=[],
-            nominal=100000,
-            contracts=10
+            coupon=0, delivery=dt(2000, 6, 1), basket=[], nominal=100000, contracts=10
         )
         assert future.notional == -1e6
 
     def test_dirty_in_methods(self):
         kws = dict(ex_div=7, frequency="S", convention="ActActICMA", calendar=None)
         bonds = [
             FixedRateBond(dt(1999, 1, 1), dt(2009, 12, 7), fixed_rate=5.75, **kws),
@@ -1954,19 +2944,23 @@
             FixedRateBond(dt(1999, 1, 1), dt(2012, 8, 6), fixed_rate=9.00, **kws),
         ]
         future = BondFuture(
             delivery=(dt(2000, 6, 1), dt(2000, 6, 30)), coupon=7.0, basket=bonds
         )
         prices = [102.732, 131.461, 107.877, 134.455]
         expected = future.net_basis(112.98, prices, 6.24, dt(2000, 3, 16))
-        result = future.net_basis(112.98, prices, 6.24, dt(2000, 3, 16), delivery=dt(2000, 6, 30))
+        result = future.net_basis(
+            112.98, prices, 6.24, dt(2000, 3, 16), delivery=dt(2000, 6, 30)
+        )
         assert result == expected
 
         expected = future.implied_repo(112.98, prices, dt(2000, 3, 16))
-        result = future.implied_repo(112.98, prices, dt(2000, 3, 16), delivery=dt(2000, 6, 30))
+        result = future.implied_repo(
+            112.98, prices, dt(2000, 3, 16), delivery=dt(2000, 6, 30)
+        )
         assert result == expected
 
         expected = future.ytm(112.98)
         result = future.ytm(112.98, delivery=dt(2000, 6, 30))
         assert result == expected
 
         expected = future.duration(112.98)
@@ -1983,28 +2977,27 @@
         ]
         future = BondFuture(
             delivery=(dt(2000, 6, 1), dt(2000, 6, 30)), coupon=7.0, basket=bonds
         )
         prices = [102.732, 131.461, 107.877, 134.455]
         assert future.ctd_index(112.98, prices, dt(2000, 3, 16)) == 0
 
-    @pytest.mark.parametrize("metric, expected", [
-        ("future_price", 112.98),
-        ("ytm", 5.301975)
-    ])
+    @pytest.mark.parametrize(
+        "metric, expected", [("future_price", 112.98), ("ytm", 5.301975)]
+    )
     @pytest.mark.parametrize("delivery", [None, dt(2000, 6, 30)])
     def test_futures_rates(self, metric, expected, delivery):
         curve = Curve(
             nodes={
                 dt(2000, 3, 15): 1.0,
                 dt(2000, 6, 30): 1.0,
-                dt(2009,  12, 7): 1.0,
+                dt(2009, 12, 7): 1.0,
                 dt(2010, 11, 25): 1.0,
                 dt(2011, 7, 12): 1.0,
-                dt(2012, 8, 6): 1.0
+                dt(2012, 8, 6): 1.0,
             },
             id="gilt_curve",
             convention="act365f",
         )
         kws = dict(
             ex_div=7,
             frequency="S",
@@ -2018,16 +3011,23 @@
             FixedRateBond(dt(1999, 1, 1), dt(2011, 7, 12), fixed_rate=9.00, **kws),
             FixedRateBond(dt(1999, 1, 1), dt(2010, 11, 25), fixed_rate=6.25, **kws),
             FixedRateBond(dt(1999, 1, 1), dt(2012, 8, 6), fixed_rate=9.00, **kws),
         ]
         solver = Solver(
             curves=[curve],
             instruments=[
-                IRS(dt(2000, 3, 15), dt(2000, 6, 30), "A", convention="act365f", curves="gilt_curve")
-            ] + bonds,
+                IRS(
+                    dt(2000, 3, 15),
+                    dt(2000, 6, 30),
+                    "A",
+                    convention="act365f",
+                    curves="gilt_curve",
+                )
+            ]
+            + bonds,
             s=[7.381345, 102.732, 131.461, 107.877, 134.455],
         )  # note the repo rate as defined by 'gilt_curve' is set to analogue implied
         future = BondFuture(
             coupon=7.0,
             delivery=(dt(2000, 6, 1), dt(2000, 6, 30)),
             basket=bonds,
         )
@@ -2058,18 +3058,18 @@
             result = future.rate(metric="badstr")
 
     def test_futures_npv(self):
         curve = Curve(
             nodes={
                 dt(2000, 3, 15): 1.0,
                 dt(2000, 6, 30): 1.0,
-                dt(2009,  12, 7): 1.0,
+                dt(2009, 12, 7): 1.0,
                 dt(2010, 11, 25): 1.0,
                 dt(2011, 7, 12): 1.0,
-                dt(2012, 8, 6): 1.0
+                dt(2012, 8, 6): 1.0,
             },
             id="gilt_curve",
             convention="act365f",
         )
         kws = dict(
             ex_div=7,
             frequency="S",
@@ -2084,16 +3084,23 @@
             FixedRateBond(dt(1999, 1, 1), dt(2011, 7, 12), fixed_rate=9.00, **kws),
             FixedRateBond(dt(1999, 1, 1), dt(2010, 11, 25), fixed_rate=6.25, **kws),
             FixedRateBond(dt(1999, 1, 1), dt(2012, 8, 6), fixed_rate=9.00, **kws),
         ]
         solver = Solver(
             curves=[curve],
             instruments=[
-                IRS(dt(2000, 3, 15), dt(2000, 6, 30), "A", convention="act365f", curves="gilt_curve")
-            ] + bonds,
+                IRS(
+                    dt(2000, 3, 15),
+                    dt(2000, 6, 30),
+                    "A",
+                    convention="act365f",
+                    curves="gilt_curve",
+                )
+            ]
+            + bonds,
             s=[7.381345, 102.732, 131.461, 107.877, 134.455],
         )  # note the repo rate as defined by 'gilt_curve' is set to analogue implied
         future = BondFuture(
             coupon=7.0,
             delivery=(dt(2000, 6, 1), dt(2000, 6, 30)),
             basket=bonds,
             nominal=100000,
@@ -2130,112 +3137,185 @@
         )
         result = future.duration(112.98, delivery=delivery)[0]
         expected = 8.20178546111
         assert abs(result - expected) < 1e-3
 
         expected = (
             future.duration(112.98, delivery=delivery)[0]
-            - future.duration(112.98-result/100, delivery=delivery)[0]
+            - future.duration(112.98 - result / 100, delivery=delivery)[0]
         )
         result2 = future.convexity(112.98, delivery=delivery)[0]
-        assert abs(result2 - expected*100) < 1e-3
+        assert abs(result2 - expected * 100) < 1e-3
 
+        # Bond future duration which is not risk is not adjusted by CFs
+        result = future.duration(112.98, delivery=delivery, metric="modified")[0]
+        expected = 7.23419455163
+        assert abs(result - expected) < 1e-3
 
-class TestPricingMechanism:
 
+class TestPricingMechanism:
     def test_value(self, curve):
         ob = Value(dt(2022, 1, 28), curves=curve)
         ob.rate()
 
     def test_irs(self, curve):
         ob = IRS(dt(2022, 1, 28), "6m", "Q", curves=curve)
         ob.rate()
         ob.npv()
         ob.cashflows()
         ob.spread()
 
+    def test_iirs(self, curve):
+        i_curve = IndexCurve(
+            {dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99},
+            index_base=100.0,
+        )
+        ob = IIRS(dt(2022, 1, 28), "6m", "Q", curves=[i_curve, curve, curve, curve])
+        ob.rate()
+        ob.npv()
+        ob.cashflows()
+        ob.spread()
+
     def test_sbs(self, curve):
         ob = SBS(dt(2022, 1, 28), "6m", "Q", curves=curve)
         ob.rate()
         ob.npv()
         ob.cashflows()
         ob.spread()
 
     def test_fra(self, curve):
         ob = FRA(dt(2022, 1, 28), "6m", "S", curves=curve)
         ob.rate()
         ob.npv()
         ob.cashflows()
 
-    @pytest.mark.parametrize("klass, kwargs", [
-        (NonMtmXCS, {}),
-        (NonMtmFixedFloatXCS, {"fixed_rate": 2.0}),
-        (NonMtmFixedFixedXCS, {"fixed_rate": 2.0}),
-        (XCS, {}),
-        (FixedFloatXCS, {"fixed_rate": 2.0}),
-        (FloatFixedXCS, {}),
-        (FixedFixedXCS, {"fixed_rate": 2.0}),
-    ])
+    @pytest.mark.parametrize(
+        "klass, kwargs",
+        [
+            (NonMtmXCS, {}),
+            (NonMtmFixedFloatXCS, {"fixed_rate": 2.0}),
+            (NonMtmFixedFixedXCS, {"fixed_rate": 2.0}),
+            (XCS, {}),
+            (FixedFloatXCS, {"fixed_rate": 2.0}),
+            (FloatFixedXCS, {}),
+            (FixedFixedXCS, {"fixed_rate": 2.0}),
+        ],
+    )
     def test_allxcs(self, klass, kwargs, curve, curve2):
-        ob = klass(dt(2022, 1, 28), "6m", "S", currency="usd", leg2_currency="eur",
-                   curves=[curve, None, curve2, None], **kwargs)
+        ob = klass(
+            dt(2022, 1, 28),
+            "6m",
+            "S",
+            currency="usd",
+            leg2_currency="eur",
+            curves=[curve, None, curve2, None],
+            **kwargs,
+        )
         fxf = FXForwards(
             FXRates({"eurusd": 1.1}, settlement=dt(2022, 1, 3)),
-            {"usdusd": curve, "eurusd": curve2, "eureur": curve2}
+            {"usdusd": curve, "eurusd": curve2, "eureur": curve2},
         )
         ob.rate(leg=2, fx=fxf)
         ob.npv(fx=fxf)
         ob.cashflows(fx=fxf)
 
+    def test_zcs(self, curve):
+        ob = ZCS(dt(2022, 1, 28), "6m", "S", curves=curve)
+        ob.rate()
+        ob.npv()
+        ob.cashflows()
 
-class TestPortfolio:
+    def test_zcis(self, curve):
+        i_curve = IndexCurve(
+            {dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99},
+            index_base=100.0,
+        )
+        ob = ZCIS(dt(2022, 1, 28), "6m", "S", curves=[curve, curve, i_curve, curve])
+        ob.rate()
+        ob.npv()
+        ob.cashflows()
 
-    def test_portfolio_npv(self, curve):
 
+class TestPortfolio:
+    def test_portfolio_npv(self, curve):
         irs1 = IRS(dt(2022, 1, 1), "6m", "Q", fixed_rate=1.0, curves=curve)
         irs2 = IRS(dt(2022, 1, 1), "3m", "Q", fixed_rate=2.0, curves=curve)
         pf = Portfolio([irs1, irs2])
         assert pf.npv() == irs1.npv() + irs2.npv()
 
-        pf = Portfolio([irs1]*5)
+        pf = Portfolio([irs1] * 5)
         assert pf.npv() == irs1.npv() * 5
 
+        with default_context("pool", 2):  # also test parallel processing
+            result = pf.npv()
+            assert result == irs1.npv() * 5
+
+    def test_portfolio_npv_local(self, curve):
+        irs1 = IRS(dt(2022, 1, 1), "6m", "Q", fixed_rate=1.0, curves=curve, currency="usd")
+        irs2 = IRS(dt(2022, 1, 1), "3m", "Q", fixed_rate=2.0, curves=curve, currency="eur")
+        irs3 = IRS(dt(2022, 1, 1), "3m", "Q", fixed_rate=2.0, curves=curve, currency="usd")
+        pf = Portfolio([irs1, irs2, irs3])
+
+        result = pf.npv(local=True)
+        expected = {
+            "usd": 20093.295095887483,
+            "eur": 5048.87332403382,
+        }
+        assert result == expected
+
+        with default_context("pool", 2):  # also test parallel processing
+            result = pf.npv(local=True)
+            assert result == expected
 
-class TestFly:
 
+class TestFly:
     @pytest.mark.parametrize("mechanism", [False, True])
     def test_fly_npv(self, curve, mechanism):
         mechanism = curve if mechanism else None
         inverse = curve if mechanism is None else None
         irs1 = IRS(dt(2022, 1, 1), "3m", "Q", fixed_rate=1.0, curves=mechanism)
         irs2 = IRS(dt(2022, 1, 1), "4m", "Q", fixed_rate=2.0, curves=mechanism)
         irs3 = IRS(dt(2022, 1, 1), "5m", "Q", fixed_rate=1.0, curves=mechanism)
         fly = Fly(irs1, irs2, irs3)
-        assert fly.npv(inverse) == irs1.npv(inverse)+irs2.npv(inverse)+irs3.npv(inverse)
+        assert fly.npv(inverse) == irs1.npv(inverse) + irs2.npv(inverse) + irs3.npv(
+            inverse
+        )
 
     @pytest.mark.parametrize("mechanism", [False, True])
     def test_fly_rate(self, curve, mechanism):
         mechanism = curve if mechanism else None
         inv = curve if mechanism is None else None
         irs1 = IRS(dt(2022, 1, 1), "3m", "Q", fixed_rate=1.0, curves=mechanism)
         irs2 = IRS(dt(2022, 1, 1), "4m", "Q", fixed_rate=2.0, curves=mechanism)
         irs3 = IRS(dt(2022, 1, 1), "5m", "Q", fixed_rate=1.0, curves=mechanism)
         fly = Fly(irs1, irs2, irs3)
-        assert fly.rate(inv) == -irs1.rate(inv) + 2*irs2.rate(inv) - irs3.rate(inv)
+        assert fly.rate(inv) == -irs1.rate(inv) + 2 * irs2.rate(inv) - irs3.rate(inv)
 
     def test_fly_cashflows_executes(self, curve):
         irs1 = IRS(dt(2022, 1, 1), "3m", "Q", fixed_rate=1.0, curves=curve)
         irs2 = IRS(dt(2022, 1, 1), "4m", "Q", fixed_rate=2.0, curves=curve)
         irs3 = IRS(dt(2022, 1, 1), "5m", "Q", fixed_rate=1.0, curves=curve)
         fly = Fly(irs1, irs2, irs3)
         fly.cashflows()
 
+    def test_local_npv(self, curve):
+        irs1 = IRS(dt(2022, 1, 1), "3m", "Q", fixed_rate=1.0, curves=curve, currency="eur")
+        irs2 = IRS(dt(2022, 1, 1), "4m", "Q", fixed_rate=2.0, curves=curve, currency="usd")
+        irs3 = IRS(dt(2022, 1, 1), "3m", "Q", fixed_rate=1.0, curves=curve, currency="gbp")
+        fly = Fly(irs1, irs2, irs3)
+        result = fly.npv(local=True)
+        expected = {
+            "eur": 7523.321141258284,
+            "usd": 6711.514715925333,
+            "gbp": 7523.321141258284,
+        }
+        assert result == expected
 
-class TestSpread:
 
+class TestSpread:
     @pytest.mark.parametrize("mechanism", [False, True])
     def test_spread_npv(self, curve, mechanism):
         mechanism = curve if mechanism else None
         inverse = curve if mechanism is None else None
         irs1 = IRS(dt(2022, 1, 1), "3m", "Q", fixed_rate=1.0, curves=mechanism)
         irs2 = IRS(dt(2022, 1, 1), "4m", "Q", fixed_rate=2.0, curves=mechanism)
         spd = Spread(irs1, irs2)
@@ -2252,18 +3332,27 @@
 
     def test_spread_cashflows_executes(self, curve):
         irs1 = IRS(dt(2022, 1, 1), "3m", "Q", fixed_rate=1.0, curves=curve)
         irs2 = IRS(dt(2022, 1, 1), "4m", "Q", fixed_rate=2.0, curves=curve)
         spd = Spread(irs1, irs2)
         spd.cashflows()
 
+    def test_local_npv(self, curve):
+        irs1 = IRS(dt(2022, 1, 1), "3m", "Q", fixed_rate=1.0, curves=curve, currency="eur")
+        irs2 = IRS(dt(2022, 1, 1), "4m", "Q", fixed_rate=2.0, curves=curve, currency="usd")
+        spd = Spread(irs1, irs2)
+        result = spd.npv(local=True)
+        expected = {
+            "eur": 7523.321141258284,
+            "usd": 6711.514715925333,
+        }
+        assert result == expected
 
-class TestSensitivities:
 
+class TestSensitivities:
     def test_sensitivity_raises(self):
-
         irs = IRS(dt(2022, 1, 1), "6m", "Q")
         with pytest.raises(ValueError, match="`solver` is required"):
             irs.delta()
 
         with pytest.raises(ValueError, match="`solver` is required"):
-            irs.gamma()
+            irs.gamma()
```

### Comparing `rateslib-0.2.0/tests/test_legs.py` & `rateslib-0.3.0/tests/test_legs.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,19 +7,22 @@
 import context
 from rateslib import default_context
 from rateslib.legs import (
     FixedLeg,
     FloatLeg,
     FloatPeriod,
     ZeroFloatLeg,
+    ZeroFixedLeg,
+    ZeroIndexLeg,
     FixedPeriod,
     CustomLeg,
     FloatLegExchange,
     FixedLegExchange,
     IndexFixedLegExchange,
+    IndexFixedLeg,
     FloatLegExchangeMtm,
     FixedLegExchangeMtm,
     Cashflow,
 )
 from rateslib.fx import FXRates, FXForwards
 from rateslib.default import Defaults
 from rateslib.curves import Curve, IndexCurve
@@ -27,59 +30,67 @@
 
 @pytest.fixture()
 def curve():
     nodes = {
         dt(2022, 1, 1): 1.00,
         dt(2022, 4, 1): 0.99,
         dt(2022, 7, 1): 0.98,
-        dt(2022, 10, 1): 0.97
+        dt(2022, 10, 1): 0.97,
     }
     return Curve(nodes=nodes, interpolation="log_linear")
 
 
 class TestFloatLeg:
-
-    @pytest.mark.parametrize("obj", [
-        (FloatLeg(
-            effective=dt(2022, 1, 1),
-            termination=dt(2022, 6, 1),
-            payment_lag=0,
-            notional=1e9,
-            convention="Act360",
-            frequency="Q",
-            fixing_method="rfr_payment_delay",
-            spread_compound_method="none_simple",
-            currency="nok",
-        )),
-        (FloatLegExchange(
-            effective=dt(2022, 1, 1),
-            termination=dt(2022, 6, 1),
-            payment_lag=0,
-            payment_lag_exchange=0,
-            notional=1e9,
-            convention="Act360",
-            frequency="Q",
-            fixing_method="rfr_payment_delay",
-            spread_compound_method="none_simple",
-            currency="nok",
-        )),
-        (FloatLegExchangeMtm(
-            effective=dt(2022, 1, 1),
-            termination=dt(2022, 6, 1),
-            payment_lag=0,
-            payment_lag_exchange=0,
-            convention="Act360",
-            frequency="Q",
-            fixing_method="rfr_payment_delay",
-            spread_compound_method="none_simple",
-            currency="nok",
-            alt_currency="usd",
-            alt_notional=1e8,
-        ))
-    ])
+    @pytest.mark.parametrize(
+        "obj",
+        [
+            (
+                FloatLeg(
+                    effective=dt(2022, 1, 1),
+                    termination=dt(2022, 6, 1),
+                    payment_lag=0,
+                    notional=1e9,
+                    convention="Act360",
+                    frequency="Q",
+                    fixing_method="rfr_payment_delay",
+                    spread_compound_method="none_simple",
+                    currency="nok",
+                )
+            ),
+            (
+                FloatLegExchange(
+                    effective=dt(2022, 1, 1),
+                    termination=dt(2022, 6, 1),
+                    payment_lag=0,
+                    payment_lag_exchange=0,
+                    notional=1e9,
+                    convention="Act360",
+                    frequency="Q",
+                    fixing_method="rfr_payment_delay",
+                    spread_compound_method="none_simple",
+                    currency="nok",
+                )
+            ),
+            (
+                FloatLegExchangeMtm(
+                    effective=dt(2022, 1, 1),
+                    termination=dt(2022, 6, 1),
+                    payment_lag=0,
+                    payment_lag_exchange=0,
+                    convention="Act360",
+                    frequency="Q",
+                    fixing_method="rfr_payment_delay",
+                    spread_compound_method="none_simple",
+                    currency="nok",
+                    alt_currency="usd",
+                    alt_notional=1e8,
+                )
+            ),
+        ],
+    )
     def test_float_leg_analytic_delta_with_npv(self, curve, obj):
         result = 5 * obj.analytic_delta(curve, curve)
         before_npv = -obj.npv(curve, curve)
         obj.float_spread = 5
         after_npv = -obj.npv(curve, curve)
         expected = after_npv - before_npv
         assert abs(result - expected) < 1e-7
@@ -141,56 +152,65 @@
 
     def test_float_leg_fixings_scalar(self, curve):
         float_leg = FloatLeg(dt(2022, 2, 1), "9M", "Q", payment_lag=0, fixings=5.0)
         assert float_leg.periods[0].fixings == 5.0
         assert float_leg.periods[1].fixings is None
         assert float_leg.periods[2].fixings is None
 
-    @pytest.mark.parametrize("method, param", [
-        ("rfr_payment_delay", None),
-        ("rfr_lockout", 1),
-        ("rfr_observation_shift", 0),
-    ])
-    @pytest.mark.parametrize("fixings", [
-        [[1.19, 1.19, -8.81]],
-        Series([1.19, 1.19, -8.81], index=[
-            dt(2022, 12, 28), dt(2022, 12, 29), dt(2022, 12, 30)
-        ])
-    ])
+    @pytest.mark.parametrize(
+        "method, param",
+        [
+            ("rfr_payment_delay", None),
+            ("rfr_lockout", 1),
+            ("rfr_observation_shift", 0),
+        ],
+    )
+    @pytest.mark.parametrize(
+        "fixings",
+        [
+            [[1.19, 1.19, -8.81]],
+            Series(
+                [1.19, 1.19, -8.81],
+                index=[dt(2022, 12, 28), dt(2022, 12, 29), dt(2022, 12, 30)],
+            ),
+        ],
+    )
     def test_float_leg_rfr_fixings_table(self, method, param, fixings, curve):
         curve._set_ad_order(order=1)
         float_leg = FloatLeg(
             effective=dt(2022, 12, 28),
             termination="2M",
             frequency="M",
             fixings=fixings,
             currency="SEK",
             fixing_method=method,
             method_param=param,
         )
         float_leg.cashflows(curve)
-        result = float_leg.fixings_table(curve)[dt(2022, 12, 28):dt(2023, 1, 1)]
-        expected = DataFrame({
-            "obs_dates": [
-                dt(2022, 12, 28),
-                dt(2022, 12, 29),
-                dt(2022, 12, 30),
-                dt(2022, 12, 31),
-                dt(2023, 1, 1),
-            ],
-            "notional": [
-                -1002914.0840790921,
-                -1002914.0840790921,
-                -1003192.739517848,
-                -1002835.4299274746,
-                -1002835.4299274748,
-            ],
-            "dcf": [0.0027777777777777778] * 5,
-            "rates": [1.19, 1.19, -8.81, 4.01364, 4.01364]
-        }).set_index("obs_dates")
+        result = float_leg.fixings_table(curve)[dt(2022, 12, 28) : dt(2023, 1, 1)]
+        expected = DataFrame(
+            {
+                "obs_dates": [
+                    dt(2022, 12, 28),
+                    dt(2022, 12, 29),
+                    dt(2022, 12, 30),
+                    dt(2022, 12, 31),
+                    dt(2023, 1, 1),
+                ],
+                "notional": [
+                    -1002914.0840790921,
+                    -1002914.0840790921,
+                    -1003192.739517848,
+                    -1002835.4299274746,
+                    -1002835.4299274748,
+                ],
+                "dcf": [0.0027777777777777778] * 5,
+                "rates": [1.19, 1.19, -8.81, 4.01364, 4.01364],
+            }
+        ).set_index("obs_dates")
         assert_frame_equal(result, expected)
 
     def test_float_leg_set_float_spread(self, curve):
         float_leg = FloatLeg(
             effective=dt(2022, 1, 1),
             termination=dt(2022, 6, 1),
             payment_lag=2,
@@ -201,130 +221,192 @@
         assert float_leg.float_spread is None
         assert float_leg.periods[0].float_spread == 0
 
         float_leg.float_spread = 2.0
         assert float_leg.float_spread == 2.0
         assert float_leg.periods[0].float_spread == 2.0
 
-    @pytest.mark.parametrize("method, spread_method, expected", [
-        ("ibor", None, True),
-        ("rfr_payment_delay", "none_simple", True),
-        ("rfr_payment_delay", "isda_compounding", False),
-        ("rfr_payment_delay", "isda_flat_compounding", False),
-    ])
+    @pytest.mark.parametrize(
+        "method, spread_method, expected",
+        [
+            ("ibor", None, True),
+            ("rfr_payment_delay", "none_simple", True),
+            ("rfr_payment_delay", "isda_compounding", False),
+            ("rfr_payment_delay", "isda_flat_compounding", False),
+        ],
+    )
     def test_is_linear(self, method, spread_method, expected):
         float_leg = FloatLeg(
             effective=dt(2022, 1, 1),
             termination=dt(2022, 6, 1),
             payment_lag=2,
             notional=-1e9,
             convention="Act360",
             frequency="Q",
             fixing_method=method,
             spread_compound_method=spread_method,
         )
         assert float_leg._is_linear is expected
 
-    @pytest.mark.parametrize("method, expected", [
-        ("ISDA_compounding", 2.88250579),
-        ("NONE_Simple", 4.637779609),
-    ])
+    @pytest.mark.parametrize(
+        "method, expected",
+        [
+            ("ISDA_compounding", 357.7055853),
+            ("ISDA_flat_compounding", 360.658902),
+            ("NONE_Simple", 362.2342162),
+        ],
+    )
     def test_float_leg_spread_calculation(self, method, expected, curve):
         leg = FloatLeg(
             effective=dt(2022, 1, 1),
             termination=dt(2022, 6, 1),
             payment_lag=0,
             notional=1e9,
             convention="Act360",
             frequency="Q",
             fixing_method="rfr_payment_delay",
             spread_compound_method=method,
             currency="nok",
-            float_spread=-399,
+            float_spread=0,
         )
-        npv = leg.npv(curve, curve)
-        result = leg._spread(-npv, curve, curve)
-        assert abs(result + expected) < 1e-4
-        leg.float_spread = result - 399
-        assert abs(leg.npv(curve, curve)) < 1e-3
+        base_npv = leg.npv(curve, curve)
+        result = leg._spread(-15000000, curve, curve)
+        assert abs(result - expected) < 1e-3
+        leg.float_spread = result
+        assert abs(leg.npv(curve, curve) - base_npv + 15000000) < 2e2
 
     def test_fixing_method_raises(self):
         with pytest.raises(ValueError, match="`fixing_method`"):
             FloatLeg(dt(2022, 2, 1), "9M", "Q", fixing_method="bad")
 
-    @pytest.mark.parametrize("eff, term, freq, stub, expected", [
-        (dt(2022, 1, 1), dt(2022, 6, 15), "Q", "ShortFront",
-         [dt(2022, 1, 1), dt(2022, 3, 15), dt(2022, 6, 15)]),
-        (dt(2022, 1, 1), dt(2022, 6, 15), "Q", "ShortBack",
-         [dt(2022, 1, 1), dt(2022, 4, 1), dt(2022, 6, 15)]),
-        (dt(2022, 1, 1), dt(2022, 9, 15), "Q", "LongFront",
-         [dt(2022, 1, 1), dt(2022, 6, 15), dt(2022, 9, 15)]),
-        (dt(2022, 1, 1), dt(2022, 9, 15), "Q", "LongBack",
-         [dt(2022, 1, 1), dt(2022, 4, 1), dt(2022, 9, 15)]),
-    ])
+    @pytest.mark.parametrize(
+        "eff, term, freq, stub, expected",
+        [
+            (
+                dt(2022, 1, 1),
+                dt(2022, 6, 15),
+                "Q",
+                "ShortFront",
+                [dt(2022, 1, 1), dt(2022, 3, 15), dt(2022, 6, 15)],
+            ),
+            (
+                dt(2022, 1, 1),
+                dt(2022, 6, 15),
+                "Q",
+                "ShortBack",
+                [dt(2022, 1, 1), dt(2022, 4, 1), dt(2022, 6, 15)],
+            ),
+            (
+                dt(2022, 1, 1),
+                dt(2022, 9, 15),
+                "Q",
+                "LongFront",
+                [dt(2022, 1, 1), dt(2022, 6, 15), dt(2022, 9, 15)],
+            ),
+            (
+                dt(2022, 1, 1),
+                dt(2022, 9, 15),
+                "Q",
+                "LongBack",
+                [dt(2022, 1, 1), dt(2022, 4, 1), dt(2022, 9, 15)],
+            ),
+        ],
+    )
     def test_leg_periods_unadj_dates(self, eff, term, freq, stub, expected):
         leg = FloatLeg(effective=eff, termination=term, frequency=freq, stub=stub)
         assert leg.schedule.uschedule == expected
 
-    @pytest.mark.parametrize("eff, term, freq, stub, expected", [
-        (dt(2022, 1, 1), dt(2022, 6, 15), "Q", "ShortFront",
-         [dt(2022, 1, 3), dt(2022, 3, 15), dt(2022, 6, 15)]),
-        (dt(2022, 1, 1), dt(2022, 6, 15), "Q", "ShortBack",
-         [dt(2022, 1, 3), dt(2022, 4, 1), dt(2022, 6, 15)]),
-        (dt(2022, 1, 1), dt(2022, 9, 15), "Q", "LongFront",
-         [dt(2022, 1, 3), dt(2022, 6, 15), dt(2022, 9, 15)]),
-        (dt(2022, 1, 1), dt(2022, 9, 15), "Q", "LongBack",
-         [dt(2022, 1, 3), dt(2022, 4, 1), dt(2022, 9, 15)]),
-    ])
+    @pytest.mark.parametrize(
+        "eff, term, freq, stub, expected",
+        [
+            (
+                dt(2022, 1, 1),
+                dt(2022, 6, 15),
+                "Q",
+                "ShortFront",
+                [dt(2022, 1, 3), dt(2022, 3, 15), dt(2022, 6, 15)],
+            ),
+            (
+                dt(2022, 1, 1),
+                dt(2022, 6, 15),
+                "Q",
+                "ShortBack",
+                [dt(2022, 1, 3), dt(2022, 4, 1), dt(2022, 6, 15)],
+            ),
+            (
+                dt(2022, 1, 1),
+                dt(2022, 9, 15),
+                "Q",
+                "LongFront",
+                [dt(2022, 1, 3), dt(2022, 6, 15), dt(2022, 9, 15)],
+            ),
+            (
+                dt(2022, 1, 1),
+                dt(2022, 9, 15),
+                "Q",
+                "LongBack",
+                [dt(2022, 1, 3), dt(2022, 4, 1), dt(2022, 9, 15)],
+            ),
+        ],
+    )
     def test_leg_periods_adj_dates(self, eff, term, freq, stub, expected):
         leg = FloatLeg(
             effective=eff, termination=term, frequency=freq, stub=stub, calendar="bus"
         )
         assert leg.schedule.aschedule == expected
 
-    @pytest.mark.parametrize("eff, term, freq, stub, expected", [
-        (dt(2022, 1, 1), dt(2022, 6, 15), "Q", "ShortFront",
-         [FloatPeriod(
-             start=dt(2022, 1, 3),
-             end=dt(2022, 3, 15),
-             payment=dt(2022, 3, 17),
-             frequency="Q",
-             notional=Defaults.notional,
-             convention=Defaults.convention,
-             termination=dt(2022, 6, 15),
-         ),
-             FloatPeriod(
-                 start=dt(2022, 3, 15),
-                 end=dt(2022, 6, 15),
-                 payment=dt(2022, 6, 17),
-                 frequency="Q",
-                 notional=Defaults.notional,
-                 convention=Defaults.convention,
-                 termination=dt(2022, 6, 15),
-             )]),
-    ])
+    @pytest.mark.parametrize(
+        "eff, term, freq, stub, expected",
+        [
+            (
+                dt(2022, 1, 1),
+                dt(2022, 6, 15),
+                "Q",
+                "ShortFront",
+                [
+                    FloatPeriod(
+                        start=dt(2022, 1, 3),
+                        end=dt(2022, 3, 15),
+                        payment=dt(2022, 3, 17),
+                        frequency="Q",
+                        notional=Defaults.notional,
+                        convention=Defaults.convention,
+                        termination=dt(2022, 6, 15),
+                    ),
+                    FloatPeriod(
+                        start=dt(2022, 3, 15),
+                        end=dt(2022, 6, 15),
+                        payment=dt(2022, 6, 17),
+                        frequency="Q",
+                        notional=Defaults.notional,
+                        convention=Defaults.convention,
+                        termination=dt(2022, 6, 15),
+                    ),
+                ],
+            ),
+        ],
+    )
     def test_leg_periods_adj_dates2(self, eff, term, freq, stub, expected):
         leg = FloatLeg(
             effective=eff,
             termination=term,
             frequency=freq,
             stub=stub,
             payment_lag=2,
-            calendar="bus"
+            calendar="bus",
         )
         for i in range(2):
             assert leg.periods[i].__repr__() == expected[i].__repr__()
 
     def test_spread_compound_method_raises(self):
         with pytest.raises(ValueError, match="`spread_compound_method`"):
             FloatLeg(dt(2022, 2, 1), "9M", "Q", spread_compound_method="bad")
 
 
 class TestZeroFloatLeg:
-
     def test_zero_float_leg_set_float_spread(self, curve):
         float_leg = ZeroFloatLeg(
             effective=dt(2022, 1, 1),
             termination=dt(2022, 6, 1),
             payment_lag=2,
             notional=-1e9,
             convention="Act360",
@@ -369,16 +451,16 @@
             payment_lag=2,
             notional=-1e9,
             convention="Act360",
             frequency="Q",
             float_spread=500,
         )
         result = ftl.rate(curve)
-        expected = (1+ftl.periods[0].dcf * ftl.periods[0].rate(curve)/100)
-        expected *= (1+ftl.periods[1].dcf * ftl.periods[1].rate(curve)/100)
+        expected = 1 + ftl.periods[0].dcf * ftl.periods[0].rate(curve) / 100
+        expected *= 1 + ftl.periods[1].dcf * ftl.periods[1].rate(curve) / 100
         expected = (expected - 1) / ftl.dcf * 100
         assert result == expected
 
     def test_zero_float_leg_cashflows(self, curve):
         ftl = ZeroFloatLeg(
             effective=dt(2022, 1, 1),
             termination=dt(2022, 6, 1),
@@ -388,23 +470,22 @@
             frequency="Q",
             float_spread=500,
         )
         result = ftl.cashflows(curve)
         expected = DataFrame(
             {
                 "Type": ["ZeroFloatLeg"],
-                 "Acc Start": [dt(2022, 1, 1)],
-                 "Acc End": [dt(2022, 6, 1)],
-                 "DCF": [0.419444444444444],
-                 "Spread": [500.]
-             }
+                "Acc Start": [dt(2022, 1, 1)],
+                "Acc End": [dt(2022, 6, 1)],
+                "DCF": [0.419444444444444],
+                "Spread": [500.0],
+            }
         )
         assert_frame_equal(
-            result[["Type", "Acc Start", "Acc End", "DCF", "Spread"]],
-            expected
+            result[["Type", "Acc Start", "Acc End", "DCF", "Spread"]], expected
         )
 
     def test_zero_float_leg_npv(self, curve):
         ftl = ZeroFloatLeg(
             effective=dt(2022, 1, 1),
             termination=dt(2022, 6, 1),
             payment_lag=2,
@@ -427,17 +508,176 @@
             convention="Act360",
             frequency="Q",
         )
         result = ftl.cashflows()
         assert result.iloc[0].to_dict()[Defaults.headers["npv"]] is None
         assert result.iloc[0].to_dict()[Defaults.headers["npv_fx"]] is None
 
+    def test_zero_float_leg_analytic_delta(self, curve):
+        zfl = ZeroFloatLeg(
+            effective=dt(2022, 1, 1),
+            termination="5y",
+            payment_lag=0,
+            notional=-1e8,
+            convention="ActAct",
+            frequency="A",
+            float_spread=1.0,
+        )
+        result = zfl.analytic_delta(curve)
+        expected = -47914.3660
+
+        assert abs(result - expected) < 1e-3
+
+
+class TestZeroFixedLeg:
+    @pytest.mark.parametrize(
+        "freq, cash, rate",
+        [
+            ("A", 13140821.29, 2.50),
+            ("S", 13227083.80, 2.50),
+            ("A", None, None),
+        ],
+    )
+    def test_zero_fixed_leg_cashflows(self, freq, cash, rate, curve):
+        zfl = ZeroFixedLeg(
+            effective=dt(2022, 1, 1),
+            termination="5y",
+            payment_lag=0,
+            notional=-1e8,
+            convention="ActAct",
+            frequency=freq,
+            fixed_rate=rate,
+        )
+        result = zfl.cashflows(curve)
+        expected = DataFrame(
+            {
+                "Type": ["ZeroFixedLeg"],
+                "Acc Start": [dt(2022, 1, 1)],
+                "Acc End": [dt(2027, 1, 1)],
+                "DCF": [5.0],
+                "Rate": [rate],
+                "Cashflow": [cash],
+            }
+        )
+        assert_frame_equal(
+            result[["Type", "Acc Start", "Acc End", "DCF", "Rate", "Cashflow"]],
+            expected,
+            rtol=1e-3,
+        )
 
-class TestFloatLegExchange:
+    def test_zero_fixed_leg_npv(self, curve):
+        zfl = ZeroFixedLeg(
+            effective=dt(2022, 1, 1),
+            termination="5y",
+            payment_lag=0,
+            notional=-1e8,
+            convention="ActAct",
+            frequency="A",
+            fixed_rate=2.5,
+        )
+        result = zfl.npv(curve)
+        expected = 13140821.29 * curve[dt(2027, 1, 1)]
+        assert abs(result - expected) < 1e-2
+        result2 = zfl.npv(curve, local=True)
+        assert abs(result2["usd"] - expected) < 1e-2
+
+    def test_zero_fixed_leg_analytic_delta(self, curve):
+        zfl = ZeroFixedLeg(
+            effective=dt(2022, 1, 1),
+            termination="5y",
+            payment_lag=0,
+            notional=-1e8,
+            convention="ActAct",
+            frequency="A",
+            fixed_rate=2.5,
+        )
+        result1 = zfl._analytic_delta(curve)
+        result2 = zfl.analytic_delta(curve)
+        assert abs(result1 + 40789.7007) < 1e-3
+        assert abs(result2 + 45024.1974) < 1e-3
 
+    def test_zero_fixed_spread(self, curve):
+        zfl = ZeroFixedLeg(
+            effective=dt(2022, 1, 1),
+            termination="5y",
+            payment_lag=0,
+            notional=-1e8,
+            convention="ActAct",
+            frequency="A",
+            fixed_rate=None,
+        )
+        result = zfl._spread(13140821.29 * curve[dt(2027, 1, 1)], None, curve)
+        assert (result / 100 - 2.50) < 1e-3
+
+    def test_analytic_delta_no_fixed_rate(self, curve):
+        zfl = ZeroFixedLeg(
+            effective=dt(2022, 1, 1),
+            termination="5y",
+            payment_lag=0,
+            notional=-1e8,
+            convention="ActAct",
+            frequency="A",
+            fixed_rate=None,
+        )
+        result = zfl.analytic_delta(curve)
+        assert result is None
+
+
+class TestZeroIndexLeg:
+    @pytest.mark.parametrize(
+        "index_base, index_fixings, meth, exp",
+        [
+            (None, None, "monthly", -61855.670),
+            (None, None, "daily", -61782.379),
+            (100.0, None, "monthly", -61855.670),
+            (None, 110.0, "monthly", -100000.0),
+            (None, 110.0, "daily", -98696.645),
+            (100.0, 110.0, "monthly", -100000.0),
+            (100.0, 110.0, "daily", -100000.0),
+        ],
+    )
+    def test_zero_index_cashflow(self, index_base, index_fixings, meth, exp):
+        index_curve = IndexCurve(
+            {
+                dt(2022, 1, 1): 1.0,
+                dt(2023, 1, 1): 0.97,
+            },
+            index_base=100.0,
+        )
+        zil = ZeroIndexLeg(
+            effective=dt(2022, 1, 15),
+            termination="2Y",
+            frequency="A",
+            convention="1+",
+            index_base=index_base,
+            index_fixings=index_fixings,
+            index_method=meth,
+        )
+        result = zil.cashflow(index_curve)
+        assert abs(result - exp) < 1e-3
+
+    def test_set_index_leg_after_init(self):
+        leg = IndexFixedLeg(
+            effective=dt(2022, 3, 15),
+            termination="9M",
+            frequency="Q",
+            convention="ActActICMA",
+            payment_lag=0,
+            notional=40e6,
+            fixed_rate=5.0,
+            index_base=None,
+        )
+        for period in leg.periods:
+            assert period.index_base is None
+        leg.index_base = 205.0
+        for period in leg.periods:
+            assert period.index_base == 205.0
+
+
+class TestFloatLegExchange:
     def test_float_leg_exchange_notional_setter(self):
         float_leg_exc = FloatLegExchange(
             effective=dt(2022, 1, 1),
             termination=dt(2022, 6, 1),
             payment_lag=2,
             notional=-1e9,
             convention="Act360",
@@ -486,15 +726,15 @@
     def test_float_leg_exchange_amortization(self, curve):
         leg = FloatLegExchange(
             dt(2022, 1, 1),
             dt(2023, 1, 1),
             "Q",
             notional=5e6,
             amortization=1e6,
-            payment_lag=0
+            payment_lag=0,
         )
         assert len(leg.periods) == 9
         for i in [0, 2, 4, 6, 8]:
             assert type(leg.periods[i]) == Cashflow
         for i in [1, 3, 5, 7]:
             assert type(leg.periods[i]) == FloatPeriod
         assert leg.periods[1].notional == 5e6
@@ -506,24 +746,26 @@
         fle = FloatLegExchange(dt(2022, 2, 1), "6M", "Q", payment_lag=0)
         result = fle.npv(curve)
         assert abs(result) < 1e-9
 
     def test_float_leg_exchange_fixings_table(self, curve):
         fle = FloatLegExchange(dt(2022, 2, 1), "6M", "Q", payment_lag=0)
         result = fle.fixings_table(curve)
-        expected = DataFrame({
-            "notional": [-1009872.33778, -1010201.55052],
-            "dcf": [0.002777777777777778, 0.002777777777777778],
-            "rates": [4.01655, 4.01655]
-        }, index=Index([dt(2022, 4, 30), dt(2022, 5, 1)], name="obs_dates"))
-        assert_frame_equal(result[dt(2022, 4, 30): dt(2022, 5, 1)], expected)
+        expected = DataFrame(
+            {
+                "notional": [-1009872.33778, -1010201.55052],
+                "dcf": [0.002777777777777778, 0.002777777777777778],
+                "rates": [4.01655, 4.01655],
+            },
+            index=Index([dt(2022, 4, 30), dt(2022, 5, 1)], name="obs_dates"),
+        )
+        assert_frame_equal(result[dt(2022, 4, 30) : dt(2022, 5, 1)], expected)
 
 
 class TestFixedLeg:
-
     def test_fixed_leg_analytic_delta(self, curve):
         fixed_leg = FixedLeg(
             effective=dt(2022, 1, 1),
             termination=dt(2022, 6, 1),
             payment_lag=2,
             notional=1e9,
             convention="Act360",
@@ -536,15 +778,15 @@
         fixed_leg = FixedLeg(
             effective=dt(2022, 1, 1),
             termination=dt(2022, 6, 1),
             payment_lag=2,
             notional=1e9,
             convention="Act360",
             frequency="Q",
-            fixed_rate=4.00
+            fixed_rate=4.00,
         )
         result = fixed_leg.npv(curve)
         assert abs(result + 400 * fixed_leg.analytic_delta(curve)) < 1e-7
 
     def test_fixed_leg_cashflows(self, curve):
         fixed_leg = FixedLeg(
             fixed_rate=4.00,
@@ -575,24 +817,26 @@
 
         fixed_leg.fixed_rate = 2.0
         assert fixed_leg.fixed_rate == 2.0
         assert fixed_leg.periods[0].fixed_rate == 2.0
 
 
 class TestIndexFixedLegExchange:
-
-    @pytest.mark.parametrize("i_fixings", [
-        None,
-        [2.1, 2.2, 2.3],
-        2.1,
-        Series(
-            [2.1, 2.2, 2.3],
-            index=[dt(2022, 6, 15), dt(2022, 9, 15), dt(2022, 12, 15)]
-        )
-    ])
+    @pytest.mark.parametrize(
+        "i_fixings",
+        [
+            None,
+            [210, 220, 230],
+            210,
+            Series(
+                [210, 220, 230],
+                index=[dt(2022, 6, 15), dt(2022, 9, 15), dt(2022, 12, 15)],
+            ),
+        ],
+    )
     def test_idx_leg_cashflows(self, i_fixings):
         leg = IndexFixedLegExchange(
             effective=dt(2022, 3, 15),
             termination="9M",
             frequency="Q",
             convention="ActActICMA",
             payment_lag=0,
@@ -605,36 +849,36 @@
         index_curve = IndexCurve(
             nodes={
                 dt(2022, 3, 15): 1.0,
                 dt(2022, 6, 15): 1.0 / 1.05,
                 dt(2022, 9, 15): 1.0 / 1.10,
                 dt(2022, 12, 15): 1.0 / 1.15,
             },
-            index_base=200.0
+            index_base=200.0,
         )
         disc_curve = Curve({dt(2022, 3, 15): 1.0, dt(2022, 12, 15): 1.0})
         flows = leg.cashflows(curve=index_curve, disc_curve=disc_curve)
 
         def equals_with_tol(a, b):
             if isinstance(a, str):
                 return a == b
             else:
-                return abs(a-b) < 1e-7
+                return abs(a - b) < 1e-7
 
         expected = {
             "Type": "IndexFixedPeriod",
             "DCF": 0.250,
             "Notional": 40e6,
             "Rate": 5.0,
             "Real Cashflow": -500e3,
-            "Index Val": 230.0,
-            "Index Ratio": 1.15,
-            "Cashflow": -575000,
+            "Index Val": 210.0,
+            "Index Ratio": 1.05,
+            "Cashflow": -525000,
         }
-        flow = flows.iloc[2].to_dict()
+        flow = flows.iloc[0].to_dict()
         for key in set(expected.keys()) & set(flow.keys()):
             assert equals_with_tol(expected[key], flow[key])
 
         final_flow = flows.iloc[3].to_dict()
         expected = {
             "Type": "IndexCashflow",
             "Notional": 40e6,
@@ -649,100 +893,297 @@
     def test_args_raises(self):
         with pytest.raises(ValueError, match="`index_method` must be in"):
             leg = IndexFixedLegExchange(
                 effective=dt(2022, 3, 15),
                 termination="9M",
                 frequency="Q",
                 index_base=200.0,
-                index_method="BAD"
+                index_method="BAD",
             )
 
+    def test_set_index_leg_after_init(self):
+        leg = IndexFixedLegExchange(
+            effective=dt(2022, 3, 15),
+            termination="9M",
+            frequency="Q",
+            convention="ActActICMA",
+            payment_lag=0,
+            notional=40e6,
+            fixed_rate=5.0,
+            index_base=None,
+            initial_exchange=False,
+        )
+        for period in leg.periods:
+            assert period.index_base is None
+        leg.index_base = 205.0
+        for period in leg.periods:
+            assert period.index_base == 205.0
+
+
+class TestIndexFixedLeg:
+    @pytest.mark.parametrize(
+        "i_fixings, meth",
+        [
+            (None, "daily"),
+            ([210, 220, 230], "daily"),
+            (210, "daily"),
+            (
+                Series(
+                    [210, 220, 230],
+                    index=[dt(2022, 6, 15), dt(2022, 9, 15), dt(2022, 12, 15)],
+                ),
+                "daily",
+            ),
+            (
+                Series(
+                    [210, 220, 230],
+                    index=[dt(2022, 6, 1), dt(2022, 9, 1), dt(2022, 12, 1)],
+                ),
+                "monthly",
+            ),
+        ],
+    )
+    def test_idx_leg_cashflows(self, i_fixings, meth):
+        leg = IndexFixedLeg(
+            effective=dt(2022, 3, 15),
+            termination="9M",
+            frequency="Q",
+            convention="ActActICMA",
+            payment_lag=0,
+            notional=40e6,
+            fixed_rate=5.0,
+            index_base=200.0,
+            index_fixings=i_fixings,
+            index_method=meth,
+        )
+        index_curve = IndexCurve(
+            nodes={
+                dt(2022, 3, 15): 1.0,
+                dt(2022, 6, 15): 1.0 / 1.05,
+                dt(2022, 9, 15): 1.0 / 1.10,
+                dt(2022, 12, 15): 1.0 / 1.15,
+            },
+            index_base=200.0,
+        )
+        disc_curve = Curve({dt(2022, 3, 15): 1.0, dt(2022, 12, 15): 1.0})
+        flows = leg.cashflows(curve=index_curve, disc_curve=disc_curve)
 
-class TestFloatLegExchangeMtm:
+        def equals_with_tol(a, b):
+            if isinstance(a, str):
+                return a == b
+            else:
+                return abs(a - b) < 1e-7
 
-    @pytest.mark.parametrize("fx_fixings, exp", [
-        (None, [None, None, None]),
-        ([1.5], [1.5, None, None]),
-        (1.25, [1.25, None, None]),
+        expected = {
+            "Type": "IndexFixedPeriod",
+            "DCF": 0.250,
+            "Notional": 40e6,
+            "Rate": 5.0,
+            "Real Cashflow": -500e3,
+            "Index Val": 210.0,
+            "Index Ratio": 1.05,
+            "Cashflow": -525000,
+        }
+        flow = flows.iloc[0].to_dict()
+        for key in set(expected.keys()) & set(flow.keys()):
+            assert equals_with_tol(expected[key], flow[key])
+
+    @pytest.mark.parametrize(
+        "meth, exp",
+        [("daily", 230.0), ("monthly", 227.91208)]
+    )
+    def test_missing_fixings(self, meth, exp):
+        i_fixings = Series(
+            [210, 220],
+            index=[dt(2022, 6, 20), dt(2022, 9, 20)],
+        )
+        leg = IndexFixedLeg(
+            effective=dt(2022, 3, 20),
+            termination="9M",
+            frequency="Q",
+            convention="ActActICMA",
+            payment_lag=0,
+            notional=40e6,
+            fixed_rate=5.0,
+            index_base=200.0,
+            index_fixings=i_fixings,
+            index_method=meth,
+        )
+        index_curve = IndexCurve(
+            nodes={
+                dt(2022, 3, 20): 1.0,
+                dt(2022, 6, 20): 1.0 / 1.05,
+                dt(2022, 9, 20): 1.0 / 1.10,
+                dt(2022, 12, 20): 1.0 / 1.15,
+            },
+            index_base=200.0,
+        )
+        cashflows = leg.cashflows(index_curve)
+        result = cashflows.iloc[2]["Index Val"]
+        assert abs(result - exp) < 1e-3
+
+    def test_set_index_leg_after_init(self):
+        leg = IndexFixedLeg(
+            effective=dt(2022, 3, 15),
+            termination="9M",
+            frequency="Q",
+            convention="ActActICMA",
+            payment_lag=0,
+            notional=40e6,
+            fixed_rate=5.0,
+            index_base=None,
+        )
+        for period in leg.periods:
+            assert period.index_base is None
+        leg.index_base = 205.0
+        for period in leg.periods:
+            assert period.index_base == 205.0
+
+    @pytest.mark.parametrize("i_base", [
+        200.0,
+        Series([199.0, 201.0], index=[dt(2021, 12, 31), dt(2022, 1, 2)]),
     ])
+    def test_set_index_base(self, curve, i_base):
+        leg = IndexFixedLeg(
+            effective=dt(2022, 1, 1),
+            termination=dt(2022, 6, 1),
+            payment_lag=2,
+            notional=-1e9,
+            convention="Act360",
+            frequency="Q",
+            index_base=None,
+        )
+        assert leg.index_base is None
+        assert leg.periods[0].index_base is None
+
+        leg.index_base = i_base
+        assert leg.index_base == 200.0
+        assert leg.periods[0].index_base == 200.0
+
+    @pytest.mark.parametrize("i_base, exp", [
+        (Series([199.0, 201.0], index=[dt(2021, 12, 31), dt(2022, 1, 2)]), 200.0),
+        (Series([1.0, 2.0], index=[dt(2000, 1, 1), dt(2000, 12, 1)]), None),
+        (None, None),
+        (110.0, 110.0),
+    ])
+    def test_initialise_index_base(self, i_base, exp):
+        leg = IndexFixedLeg(
+            effective=dt(2022, 1, 1),
+            termination=dt(2022, 6, 1),
+            payment_lag=2,
+            notional=-1e9,
+            convention="Act360",
+            frequency="Q",
+            index_base=i_base,
+        )
+        assert leg.index_base == exp
+
+
+class TestFloatLegExchangeMtm:
+    @pytest.mark.parametrize(
+        "fx_fixings, exp",
+        [
+            (None, [None, None, None]),
+            ([1.5], [1.5, None, None]),
+            (1.25, [1.25, None, None]),
+        ],
+    )
     def test_float_leg_exchange_mtm(self, fx_fixings, exp):
         float_leg_exch = FloatLegExchangeMtm(
             effective=dt(2022, 1, 3),
             termination=dt(2022, 7, 3),
             frequency="Q",
             notional=265,
             float_spread=5.0,
             currency="usd",
             alt_currency="eur",
             alt_notional=10e6,
             payment_lag_exchange=3,
             fx_fixings=fx_fixings,
         )
         fxr = FXRates({"eurusd": 1.05}, settlement=dt(2022, 1, 3))
-        fxf = FXForwards(fxr, {
-            "usdusd": Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.965}),
-            "eureur": Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.985}),
-            "eurusd": Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.987}),
-        })
+        fxf = FXForwards(
+            fxr,
+            {
+                "usdusd": Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.965}),
+                "eureur": Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.985}),
+                "eurusd": Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.987}),
+            },
+        )
 
-        d = [dt(2022, 1, 6), dt(2022, 4, 6),
-             dt(2022, 7, 6)]  # payment_lag_exchange is 3 days.
-        rate = [_ if _ is not None else fxf.rate("eurusd", d[i]) for i, _ in
-                enumerate(exp)]
+        d = [
+            dt(2022, 1, 6),
+            dt(2022, 4, 6),
+            dt(2022, 7, 6),
+        ]  # payment_lag_exchange is 3 days.
+        rate = [
+            _ if _ is not None else fxf.rate("eurusd", d[i]) for i, _ in enumerate(exp)
+        ]
 
         float_leg_exch.cashflows(fxf.curve("usd", "usd"), fxf.curve("usd", "usd"), fxf)
         assert float(float_leg_exch.periods[0].cashflow - 10e6 * rate[0]) < 1e-6
-        assert float(
-            float_leg_exch.periods[2].cashflow - 10e6 * (rate[1] - rate[0])) < 1e-6
-        assert float(
-            float_leg_exch.periods[4].cashflow - 10e6 * (rate[2] - rate[1])) < 1e-6
+        assert (
+            float(float_leg_exch.periods[2].cashflow - 10e6 * (rate[1] - rate[0]))
+            < 1e-6
+        )
+        assert (
+            float(float_leg_exch.periods[4].cashflow - 10e6 * (rate[2] - rate[1]))
+            < 1e-6
+        )
         assert float_leg_exch.periods[4].payment == d[-1]
 
         assert float_leg_exch.periods[1].notional == 10e6 * rate[0]
         assert type(float_leg_exch.periods[1]) is FloatPeriod
         assert float_leg_exch.periods[3].notional == 10e6 * rate[1]
         assert type(float_leg_exch.periods[3]) is FloatPeriod
 
         assert float_leg_exch.periods[-1].notional == 10e6 * rate[1]
 
     def test_mtm_leg_exchange_spread(self):
-        expected = [522.324262, 522.324262]
         leg = FloatLegExchangeMtm(
             effective=dt(2022, 1, 3),
             termination=dt(2022, 7, 3),
             frequency="Q",
             notional=265,
             currency="usd",
             alt_currency="eur",
-            alt_notional=10e6,
+            alt_notional=1e9,
             fixing_method="rfr_payment_delay",
             spread_compound_method="isda_compounding",
             payment_lag_exchange=0,
             payment_lag=0,
             float_spread=0.0,
         )
         fxr = FXRates({"eurusd": 1.05}, settlement=dt(2022, 1, 3))
-        fxf = FXForwards(fxr, {
-            "usdusd": Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.965}),
-            "eureur": Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.985}),
-            "eurusd": Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.987}),
-        })
+        fxf = FXForwards(
+            fxr,
+            {
+                "usdusd": Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.965}),
+                "eureur": Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.985}),
+                "eurusd": Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.987}),
+            },
+        )
 
         npv = leg.npv(fxf.curve("usd", "usd"), fxf.curve("usd", "usd"), fxf)
-        a_delta = leg.analytic_delta(fxf.curve("usd", "usd"), fxf.curve("usd", "usd"), fxf)
+        a_delta = leg.analytic_delta(
+            fxf.curve("usd", "usd"), fxf.curve("usd", "usd"), fxf
+        )
         result = leg._spread(100, fxf.curve("usd", "usd"), fxf.curve("usd", "usd"), fxf)
         leg.float_spread = result
         npv2 = leg.npv(fxf.curve("usd", "usd"), fxf.curve("usd", "usd"), fxf)
-        assert abs(npv2 - npv - 100) < 1e-5
+        assert abs(npv2 - npv - 100) < 0.01
 
-    @pytest.mark.parametrize("fx_fixings, exp", [
-        (None, [None, None, None]),
-        ([1.5], [1.5, None, None]),
-        (1.25, [1.25, None, None]),
-    ])
+    @pytest.mark.parametrize(
+        "fx_fixings, exp",
+        [
+            (None, [None, None, None]),
+            ([1.5], [1.5, None, None]),
+            (1.25, [1.25, None, None]),
+        ],
+    )
     def test_mtm_leg_fx_fixings_warn_raise(self, curve, fx_fixings, exp):
         float_leg_exch = FloatLegExchangeMtm(
             effective=dt(2022, 1, 3),
             termination=dt(2022, 7, 3),
             frequency="Q",
             notional=265,
             float_spread=5.0,
@@ -759,24 +1200,63 @@
 
         with pytest.raises(ValueError, match="`fx` is required when `fx_fixings` are"):
             with default_context("no_fx_fixings_for_xcs", "raise"):
                 float_leg_exch.npv(curve)
 
 
 def test_leg_amortization():
-    fixed_leg = FixedLeg(dt(2022, 1, 1), dt(2022, 10, 1), frequency="Q",
-                         notional=1e6, amortization=250e3, fixed_rate=2.0)
+    fixed_leg = FixedLeg(
+        dt(2022, 1, 1),
+        dt(2022, 10, 1),
+        frequency="Q",
+        notional=1e6,
+        amortization=250e3,
+        fixed_rate=2.0,
+    )
     for i, period in enumerate(fixed_leg.periods):
-        assert period.notional == 1e6 - 250e3*i
+        assert period.notional == 1e6 - 250e3 * i
 
-    float_leg = FloatLeg(dt(2022, 1, 1), dt(2022, 10, 1), frequency="Q",
-                         notional=1e6, amortization=250e3, float_spread=2.0)
+    float_leg = FloatLeg(
+        dt(2022, 1, 1),
+        dt(2022, 10, 1),
+        frequency="Q",
+        notional=1e6,
+        amortization=250e3,
+        float_spread=2.0,
+    )
     for i, period in enumerate(float_leg.periods):
         assert period.notional == 1e6 - 250e3 * i
 
+    index_leg = IndexFixedLeg(
+        dt(2022, 1, 1),
+        dt(2022, 10, 1),
+        frequency="Q",
+        notional=1e6,
+        amortization=250e3,
+        fixed_rate=2.0,
+        index_base=100.0,
+    )
+    for i, period in enumerate(index_leg.periods):
+        assert period.notional == 1e6 - 250e3 * i
+
+    index_leg_exchange = IndexFixedLegExchange(
+        dt(2022, 1, 1),
+        dt(2022, 10, 1),
+        frequency="Q",
+        notional=1e6,
+        amortization=250e3,
+        fixed_rate=2.0,
+        index_base=100.0,
+        initial_exchange=False,
+    )
+    for i, period in enumerate(index_leg_exchange.periods[0::2]):
+        assert period.notional == 1e6 - 250e3 * i
+    for i, period in enumerate(index_leg_exchange.periods[1:4:2]):
+        assert period.notional == 250e3
+
 
 def test_custom_leg_raises():
     with pytest.raises(ValueError):
         _ = CustomLeg(periods=["bad_period"])
 
 
 def test_custom_leg():
@@ -784,46 +1264,56 @@
         effective=dt(2022, 1, 1), termination=dt(2023, 1, 1), frequency="S"
     )
     custom_leg = CustomLeg(periods=float_leg.periods)
     for i, period in enumerate(custom_leg.periods):
         assert period == float_leg.periods[i]
 
 
-@pytest.mark.parametrize("fx_fixings, exp", [
-    (None, [None, None, None]),
-    ([1.5], [1.5, None, None]),
-    (1.25, [1.25, None, None]),
-])
+@pytest.mark.parametrize(
+    "fx_fixings, exp",
+    [
+        (None, [None, None, None]),
+        ([1.5], [1.5, None, None]),
+        (1.25, [1.25, None, None]),
+    ],
+)
 def test_fixed_leg_exchange_mtm(fx_fixings, exp):
     fixed_leg_exch = FixedLegExchangeMtm(
         effective=dt(2022, 1, 3),
         termination=dt(2022, 7, 3),
         frequency="Q",
         notional=265,
         fixed_rate=5.0,
         currency="usd",
         alt_currency="eur",
         alt_notional=10e6,
         payment_lag_exchange=3,
-        fx_fixings=fx_fixings
+        fx_fixings=fx_fixings,
     )
     fxr = FXRates({"eurusd": 1.05}, settlement=dt(2022, 1, 3))
-    fxf = FXForwards(fxr, {
-        "usdusd": Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.965}),
-        "eureur": Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.985}),
-        "eurusd": Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.987}),
-    })
+    fxf = FXForwards(
+        fxr,
+        {
+            "usdusd": Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.965}),
+            "eureur": Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.985}),
+            "eurusd": Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.987}),
+        },
+    )
 
-    d = [dt(2022, 1, 6), dt(2022, 4, 6), dt(2022, 7, 6)]  # payment_lag_exchange is 3 days.
+    d = [
+        dt(2022, 1, 6),
+        dt(2022, 4, 6),
+        dt(2022, 7, 6),
+    ]  # payment_lag_exchange is 3 days.
     rate = [_ if _ is not None else fxf.rate("eurusd", d[i]) for i, _ in enumerate(exp)]
 
     fixed_leg_exch.cashflows(fxf.curve("usd", "usd"), fxf.curve("usd", "usd"), fxf)
     assert float(fixed_leg_exch.periods[0].cashflow - 10e6 * rate[0]) < 1e-6
-    assert float(fixed_leg_exch.periods[2].cashflow - 10e6 * (rate[1]-rate[0])) < 1e-6
-    assert float(fixed_leg_exch.periods[4].cashflow - 10e6 * (rate[2]-rate[1])) < 1e-6
+    assert float(fixed_leg_exch.periods[2].cashflow - 10e6 * (rate[1] - rate[0])) < 1e-6
+    assert float(fixed_leg_exch.periods[4].cashflow - 10e6 * (rate[2] - rate[1])) < 1e-6
     assert fixed_leg_exch.periods[4].payment == dt(2022, 7, 6)
 
     assert fixed_leg_exch.periods[1].notional == 10e6 * rate[0]
     assert type(fixed_leg_exch.periods[1]) is FixedPeriod
     assert fixed_leg_exch.periods[3].notional == 10e6 * rate[1]
     assert type(fixed_leg_exch.periods[3]) is FixedPeriod
 
@@ -851,43 +1341,121 @@
             termination=dt(2022, 7, 3),
             frequency="Q",
             notional=265,
             currency="usd",
             alt_currency="eur",
             alt_notional=10e6,
             payment_lag_exchange=3,
-            fx_fixings="bad_type"
+            fx_fixings="bad_type",
         )
 
 
-@pytest.mark.parametrize("type_, expected, kw", [
-    (FloatLegExchangeMtm, [522.324262, 522.324262], {"float_spread": 1.0}),
-    (FixedLegExchangeMtm, [522.324262, 53772.226595], {"fixed_rate": 2.5}),
-])
+@pytest.mark.parametrize(
+    "type_, expected, kw",
+    [
+        (FloatLegExchangeMtm, [522.324262, 522.324262], {"float_spread": 1.0}),
+        (FixedLegExchangeMtm, [522.324262, 53772.226595], {"fixed_rate": 2.5}),
+    ],
+)
 def test_mtm_leg_exchange_metrics(type_, expected, kw):
     leg = type_(
         effective=dt(2022, 1, 3),
         termination=dt(2022, 7, 3),
         frequency="Q",
         notional=265,
         currency="usd",
         alt_currency="eur",
         alt_notional=10e6,
         payment_lag_exchange=0,
         payment_lag=0,
-        **kw
+        **kw,
     )
     fxr = FXRates({"eurusd": 1.05}, settlement=dt(2022, 1, 3))
-    fxf = FXForwards(fxr, {
-        "usdusd": Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.965}),
-        "eureur": Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.985}),
-        "eurusd": Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.987}),
-    })
+    fxf = FXForwards(
+        fxr,
+        {
+            "usdusd": Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.965}),
+            "eureur": Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.985}),
+            "eurusd": Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.987}),
+        },
+    )
 
-    d = [dt(2022, 1, 6), dt(2022, 4, 6), dt(2022, 7, 6)]  # payment_lag_exchange is 3 days.
+    d = [
+        dt(2022, 1, 6),
+        dt(2022, 4, 6),
+        dt(2022, 7, 6),
+    ]  # payment_lag_exchange is 3 days.
     rate = [fxf.rate("eurusd", d[i]) for i in range(3)]
 
     result = leg.analytic_delta(fxf.curve("usd", "usd"), fxf.curve("usd", "usd"), fxf)
     assert float(result - expected[0]) < 1e-6
 
     result = leg.npv(fxf.curve("usd", "usd"), fxf.curve("usd", "usd"), fxf)
-    assert float(result - expected[1]) < 1e-6
+    assert float(result - expected[1]) < 1e-6
+
+
+@pytest.mark.parametrize("klass, kwargs, expected", [
+    (IndexFixedLeg, {}, [200.0, 300.0, 400.0]),
+    (IndexFixedLegExchange, {"initial_exchange": False}, [200.0, 300.0, 400.0, 400.0]),
+    (ZeroIndexLeg, {}, [400.0])
+])
+def test_set_index_fixings_series_leg_types(klass, kwargs, expected):
+    index_fixings = Series(
+        [100.0, 200.0, 300, 399.0, 401.0],
+        index=[dt(2022, 1, 1), dt(2022, 5, 1), dt(2022, 8, 1), dt(2022, 10, 31), dt(2022, 11, 2)]
+    )
+    obj = klass(
+        effective=dt(2022, 2, 5),
+        termination="9M",
+        frequency="Q",
+        index_fixings=index_fixings,
+        index_base=100.0,
+        index_lag=3,
+        index_method="monthly",
+        **kwargs,
+    )
+    for i, period in enumerate(obj.periods):
+        if type(period) is Cashflow:
+            continue
+        assert period.index_fixings == expected[i]
+
+
+@pytest.mark.parametrize("klass, kwargs, expected", [
+    (IndexFixedLeg, {"index_fixings": [200.0, 300.0, 400.0]}, [200.0, 300.0, 400.0]),
+    (IndexFixedLegExchange, {"initial_exchange": False, "index_fixings": [200.0, 300.0, 400.0, 400.0]}, [200.0, 300.0, 400.0, 400.0]),
+    (ZeroIndexLeg, {"index_fixings": [400.0]}, [400.0])
+])
+def test_set_index_fixings_list_leg_types(klass, kwargs, expected):
+    obj = klass(
+        effective=dt(2022, 2, 5),
+        termination="9M",
+        frequency="Q",
+        index_base=100.0,
+        index_lag=3,
+        index_method="monthly",
+        **kwargs,
+    )
+    for i, period in enumerate(obj.periods):
+        if type(period) is Cashflow:
+            continue
+        assert period.index_fixings == expected[i]
+
+
+@pytest.mark.parametrize("klass, kwargs, expected", [
+    (IndexFixedLeg, {"index_fixings": 200.0}, [200.0, None, None]),
+    (IndexFixedLegExchange, {"initial_exchange": False, "index_fixings": 200.0}, [200.0, None, None, None]),
+    (ZeroIndexLeg, {"index_fixings": 400.0}, [400.0])
+])
+def test_set_index_fixings_float_leg_types(klass, kwargs, expected):
+    obj = klass(
+        effective=dt(2022, 2, 5),
+        termination="9M",
+        frequency="Q",
+        index_base=100.0,
+        index_lag=3,
+        index_method="monthly",
+        **kwargs,
+    )
+    for i, period in enumerate(obj.periods):
+        if type(period) is Cashflow:
+            continue
+        assert period.index_fixings == expected[i]
```

### Comparing `rateslib-0.2.0/tests/test_periods.py` & `rateslib-0.3.0/tests/test_periods.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from datetime import timedelta
 from pandas.testing import assert_frame_equal
 from pandas import DataFrame, Series
 import numpy as np
 
 import context
 from rateslib.periods import (
-    Cashflow, FixedPeriod, FloatPeriod, IndexFixedPeriod, IndexCashflow
+    Cashflow, FixedPeriod, FloatPeriod, IndexFixedPeriod, IndexCashflow, IndexMixin
 )
 from rateslib.fx import FXRates
 from rateslib.default import Defaults
 from rateslib.curves import Curve, LineCurve, IndexCurve
 
 
 @pytest.fixture()
@@ -58,19 +58,31 @@
         dt(2022, 1, 5): 5.00,
     }
     return LineCurve(nodes=nodes, interpolation="linear", convention="act365f")
 
 
 class TestFloatPeriod:
 
+    def test_none_cashflow(self):
+        float_period = FloatPeriod(
+            start=dt(2022, 1, 1),
+            end=dt(2022, 4, 1),
+            payment=dt(2022, 4, 3),
+            notional=1e9,
+            convention="Act360",
+            termination=dt(2022, 4, 1),
+            frequency="Q",
+        )
+        assert float_period.cashflow(None) is None
+
     @pytest.mark.parametrize("spread_method, float_spread, expected", [
         ("none_simple", 100.0, 24744.478172244584),
         ("isda_compounding", 0.0, 24744.478172244584),
         ("isda_compounding", 100.0, 25053.484941157145),
-        ("isda_flat_compounding", 100.0, 24747.211149828523),
+        ("isda_flat_compounding", 100.0, 24867.852396116967),
     ])
     def test_float_period_analytic_delta(self, curve, spread_method, float_spread, expected):
         float_period = FloatPeriod(
             start=dt(2022, 1, 1),
             end=dt(2022, 4, 1),
             payment=dt(2022, 4, 3),
             notional=1e9,
@@ -207,15 +219,15 @@
         assert abs(result - expected) < 1e-12
 
     @pytest.mark.parametrize("curve_type", ["curve", "line_curve"])
     def test_rfr_lockout_method(self, curve_type, rfr_curve, line_curve):
         curve = rfr_curve if curve_type == "curve" else line_curve
         period = FloatPeriod(dt(2022, 1, 1), dt(2022, 1, 4), dt(2022, 1, 4), "Q",
                              fixing_method="rfr_lockout", method_param=2)
-        assert period._is_complex == True  # lockout requires all fixings.
+        assert period._is_inefficient == True  # lockout requires all fixings.
         result = period.rate(curve)
         expected = ((1 + 0.01 / 365) * (1 + 0.01 / 365) * (
                     1 + 0.01 / 365) - 1) * 36500 / 3
         assert abs(result - expected) < 1e-12
 
         period = FloatPeriod(dt(2022, 1, 2), dt(2022, 1, 5), dt(2022, 1, 5), "Q",
                              fixing_method="rfr_lockout", method_param=1)
@@ -369,15 +381,15 @@
         assert abs(result["notional"][0] - expected) < 1
 
     @pytest.mark.parametrize("method, expected", [
         ("none_simple", ((1 + 0.01 / 365) * (1 + 0.02 / 365) * (
                 1 + 0.03 / 365) - 1) * 36500 / 3 + 100 / 100),
         ("isda_compounding",
          ((1 + 0.02 / 365) * (1 + 0.03 / 365) * (1 + 0.04 / 365) - 1) * 36500 / 3),
-        ("isda_flat_compounding", 3.000118724464),
+        ("isda_flat_compounding", 3.000173518986841),
     ])
     def test_rfr_compounding_float_spreads(self, method, expected, rfr_curve):
         period = FloatPeriod(
             start=dt(2022, 1, 1),
             end=dt(2022, 1, 4),
             payment=dt(2022, 1, 4),
             frequency="M",
@@ -393,15 +405,15 @@
             start=dt(2022, 1, 5),
             end=dt(2022, 4, 5),
             payment=dt(2022, 4, 5),
             frequency="Q",
             fixing_method="ibor",
             method_param=2,
         )
-        assert period._is_complex == False
+        assert period._is_inefficient == False
         assert period.rate(line_curve) == 3.0
 
     def test_ibor_fixing_table(self, line_curve):
         float_period = FloatPeriod(
             start=dt(2022, 1, 4),
             end=dt(2022, 4, 4),
             payment=dt(2022, 4, 4),
@@ -414,14 +426,32 @@
             "obs_dates": [dt(2022, 1, 2)],
             "notional": [-1e6],
             "dcf": [None],
             "rates": [2.0]
         }).set_index("obs_dates")
         assert_frame_equal(expected, result)
 
+    def test_ibor_fixing_table_fast(self, line_curve):
+        float_period = FloatPeriod(
+            start=dt(2022, 1, 4),
+            end=dt(2022, 4, 4),
+            payment=dt(2022, 4, 4),
+            frequency="Q",
+            fixing_method="ibor",
+            method_param=2,
+        )
+        result = float_period.fixings_table(line_curve, approximate=True)
+        expected = DataFrame({
+            "obs_dates": [dt(2022, 1, 2)],
+            "notional": [-1e6],
+            "dcf": [None],
+            "rates": [2.0]
+        }).set_index("obs_dates")
+        assert_frame_equal(expected, result)
+
     def test_ibor_fixings(self):
         curve = Curve({dt(2022, 1, 1): 1.0, dt(2025, 1, 1): 0.90}, calendar="bus")
         fixings = Series([1.00, 2.801, 1.00, 1.00], index=[
             dt(2023, 3, 1), dt(2023, 3, 2), dt(2023, 3, 3), dt(2023, 3, 6)
         ])
         float_period = FloatPeriod(
             start=dt(2023, 3, 6),
@@ -572,23 +602,24 @@
             float_spread=100,
             fixings=1.0
         )
         with pytest.warns(UserWarning):
             result = float_period.rate(curve)
         assert result == 2.0
 
-    def test_float_period_rate_raises(self):
-        float_period = FloatPeriod(
-            start=dt(2022, 1, 4),
-            end=dt(2022, 4, 4),
-            payment=dt(2022, 4, 4),
-            frequency="Q",
-        )
-        with pytest.raises(TypeError, match="`curve` must be of type"):
-            float_period.rate("bad_curve")
+    # @pytest.mark.skip(reason="str is an erroneous input to function: test redundant.")
+    # def test_float_period_rate_raises(self):
+    #     float_period = FloatPeriod(
+    #         start=dt(2022, 1, 4),
+    #         end=dt(2022, 4, 4),
+    #         payment=dt(2022, 4, 4),
+    #         frequency="Q",
+    #     )
+    #     with pytest.raises(TypeError, match="Curve must be of type"):
+    #         float_period.rate("bad_curve")
 
     def test_float_period_fixings_list_raises_on_ibor(self):
         with pytest.raises(ValueError, match="`fixings` can only be a single"):
             float_period = FloatPeriod(
                 start=dt(2022, 1, 4),
                 end=dt(2022, 4, 4),
                 payment=dt(2022, 4, 4),
@@ -628,14 +659,49 @@
         assert_frame_equal(result, expected)
 
         curve._set_ad_order(order=1)
         # assert values are unchanged even if curve can calculate derivatives
         result = float_period.fixings_table(curve)
         assert_frame_equal(result, expected)
 
+    @pytest.mark.parametrize("method, param", [
+        ("rfr_payment_delay", None),
+        ("rfr_lookback", 4),
+        ("rfr_lockout", 1),
+        ("rfr_observation_shift", 2),
+    ])
+    @pytest.mark.parametrize("scm, spd", [
+        ("none_simple", 1000.0),
+        ("isda_compounding", 1000.0),
+        ("isda_flat_compounding", 1000.0),
+    ])
+    @pytest.mark.parametrize("crv", [
+        Curve({
+            dt(2022, 1, 1): 1.00,
+            dt(2022, 4, 1): 0.99,
+            dt(2022, 7, 1): 0.98,
+            dt(2022, 10, 1): 0.97,
+            dt(2023, 6, 1): 0.96,
+        }, interpolation="log_linear", calendar="bus"),
+    ])
+    def test_rfr_fixings_table_fast(self, method, param, scm, spd, crv):
+        float_period = FloatPeriod(
+            start=dt(2022, 12, 28),
+            end=dt(2023, 1, 3),
+            payment=dt(2023, 1, 3),
+            frequency="M",
+            fixing_method=method,
+            method_param=param,
+            spread_compound_method=scm,
+            float_spread=spd,
+        )
+        expected = float_period.fixings_table(crv)
+        result = float_period.fixings_table(crv, approximate=True)
+        assert_frame_equal(result, expected, rtol=1e-2)
+
     def test_rfr_rate_fixings_series_monotonic_error(self):
         nodes = {
             dt(2022, 1, 1): 1.00,
             dt(2022, 4, 1): 0.99,
             dt(2022, 7, 1): 0.98,
             dt(2022, 10, 1): 0.97
         }
@@ -908,41 +974,41 @@
 class TestIndexFixedPeriod:
 
     @pytest.mark.parametrize("method, expected", [
         ("daily", 201.00502512562812), ("monthly", 200.98317675333183)
     ])
     def test_period_rate(self, method, expected):
         index_period = IndexFixedPeriod(
-            start=dt(2022, 1, 1),
-            end=dt(2022, 4, 1),
+            start=dt(2022, 1, 3),
+            end=dt(2022, 4, 3),
             payment=dt(2022, 4, 3),
             notional=1e9,
             convention="Act360",
-            termination=dt(2022, 4, 1),
+            termination=dt(2022, 4, 3),
             frequency="Q",
             fixed_rate=4.00,
             currency="usd",
             index_base=100.,
             index_method=method,
         )
         index_curve = IndexCurve(
             nodes={dt(2022, 1, 1): 1.0, dt(2022, 4, 3): 0.995},
             index_base=200.,
         )
-        result = index_period.rate(index_curve)
+        _, result, _ = index_period.index_ratio(index_curve)
         assert abs(result - expected) < 1e-8
 
     def test_period_cashflow(self):
         index_period = IndexFixedPeriod(
-            start=dt(2022, 1, 1),
-            end=dt(2022, 4, 1),
+            start=dt(2022, 1, 3),
+            end=dt(2022, 4, 3),
             payment=dt(2022, 4, 3),
             notional=1e9,
             convention="Act360",
-            termination=dt(2022, 4, 1),
+            termination=dt(2022, 4, 3),
             frequency="Q",
             fixed_rate=4.00,
             currency="usd",
             index_base=100.,
         )
         index_curve = IndexCurve(
             nodes={dt(2022, 1, 1): 1.0, dt(2022, 4, 3): 0.995},
@@ -986,20 +1052,20 @@
             "daily",
         ),
         (Series([100., 500], index=[dt(2022, 4, 2), dt(2022, 4, 4)]), "daily"),
         (Series([300., 500], index=[dt(2022, 4, 1), dt(2022, 4, 5)]), "monthly"),
     ])
     def test_period_fixings_series(self, fixings, method, curve):
         fixed_period = IndexFixedPeriod(
-            start=dt(2022, 1, 1),
-            end=dt(2022, 4, 1),
+            start=dt(2022, 1, 3),
+            end=dt(2022, 4, 3),
             payment=dt(2022, 4, 3),
             notional=1e9,
             convention="Act360",
-            termination=dt(2022, 4, 1),
+            termination=dt(2022, 4, 3),
             frequency="Q",
             currency="usd",
             index_base=200.0,
             index_fixings=fixings,
             index_method=method,
         )
         result = fixed_period.analytic_delta(None, curve)
@@ -1018,20 +1084,20 @@
                 currency="usd",
                 index_base=200.0,
                 index_method="BAD",
             )
 
     def test_period_npv(self, curve):
         index_period = IndexFixedPeriod(
-            start=dt(2022, 1, 1),
-            end=dt(2022, 4, 1),
+            start=dt(2022, 1, 3),
+            end=dt(2022, 4, 3),
             payment=dt(2022, 4, 3),
             notional=1e9,
             convention="Act360",
-            termination=dt(2022, 4, 1),
+            termination=dt(2022, 4, 3),
             frequency="Q",
             fixed_rate=4.00,
             currency="usd",
             index_base=100.,
         )
         index_curve = IndexCurve(
             nodes={dt(2022, 1, 1): 1.0, dt(2022, 4, 3): 0.995},
@@ -1088,14 +1154,15 @@
             "DCF": 0.25,
             "DF": 0.9897791268897856 if curve_ else None,
             "Notional": 1e9,
             "Rate": 4.0,
             "Spread": None,
             "Cashflow": -20000000.0,
             "Real Cashflow": -10e6,
+            "Index Base": 100.0,
             "Index Val": 200.0,
             "Index Ratio": 2.0,
             "NPV": -19795582.53779571 if curve_ else None,
             "FX Rate": 1.0,
             "NPV Ccy": -19795582.53779571 if curve_ else None,
         }
         assert result == expected
@@ -1118,14 +1185,57 @@
             payment=dt(2022, 2, 1),
             frequency="M",
             index_base=100.0,
         )
         result = i_period.cashflows()
         assert result[Defaults.headers["index_ratio"]] is None
 
+    def test_bad_curve(self):
+        i_period = IndexFixedPeriod(
+            start=dt(2022, 1, 1),
+            end=dt(2022, 2, 1),
+            payment=dt(2022, 2, 1),
+            frequency="M",
+            index_base=100.0,
+        )
+        curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99})
+        with pytest.raises(TypeError, match="`index_value` must be forecast from"):
+            i_period.index_ratio(curve)
+
+    # TEST REDUNDANT: function was changed to fallback to forecast from curve
+    # def test_cannot_forecast_from_fixings(self):
+    #     i_fixings = Series([100], index=[dt(2021, 1, 1)])
+    #     i_period = IndexFixedPeriod(
+    #         start=dt(2022, 1, 1),
+    #         end=dt(2022, 2, 1),
+    #         payment=dt(2022, 2, 1),
+    #         frequency="M",
+    #         index_base=100.0,
+    #         index_fixings=i_fixings,
+    #     )
+    #     curve = IndexCurve(
+    #         {dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99},
+    #         index_lag=3,
+    #         index_base=100.0
+    #     )
+    #     with pytest.raises(ValueError, match="`index_fixings` cannot forecast the"):
+    #         i_period.index_ratio(curve)
+
+    def test_index_fixings_linear_interp(self):
+        i_fixings = Series([173.1, 174.2], index=[dt(2001, 7, 1), dt(2001, 8, 1)])
+        result = IndexMixin._index_value(
+            i_fixings=i_fixings,
+            i_curve=None,
+            i_date=dt(2001, 7, 20),
+            i_lag=3,
+            i_method="daily"
+        )
+        expected = 173.1 + 19/31 * (174.2 - 173.1)
+        assert abs(result - expected) < 1e-6
+
 
 class TestIndexCashflow:
 
     def test_cashflow_analytic_delta(self, curve):
         cashflow = IndexCashflow(
             notional=1e6, payment=dt(2022, 1, 1), index_base=100
         )
```

### Comparing `rateslib-0.2.0/tests/test_scheduling.py` & `rateslib-0.3.0/tests/test_scheduling.py`

 * *Files 7% similar despite different names*

```diff
@@ -560,8 +560,121 @@
 def test_schedule_n_periods():
     result = Schedule(
         effective=dt(2022, 1, 1),
         termination=dt(2023, 2, 1),
         frequency="S",
         stub="FRONT",
     )
-    assert result.n_periods == 3
+    assert result.n_periods == 3
+
+
+@pytest.mark.parametrize("ue, ut, exp", [
+    (dt(2023, 3, 17), dt(2023, 12, 20), dt(2023, 9, 20)),  # PR #9
+    (dt(2022, 12, 19), dt(2023, 12, 20), dt(2023, 3, 15))
+])
+def test_get_unadjusted_long_stub_imm(ue, ut, exp):
+    result = _get_unadjusted_stub_date(ue, ut, "Q", "LONGFRONT", False, "imm")
+    assert result == exp
+
+
+@pytest.mark.parametrize("ue, ut, exp", [
+    (dt(2023, 3, 17), dt(2023, 12, 20), dt(2023, 6, 21)),  # PR #9
+])
+def test_get_unadjusted_short_stub_imm(ue, ut, exp):
+    result = _get_unadjusted_short_stub_date(ue, ut, "Q", "FRONT", False, "imm")
+    assert result == exp
+
+
+def test_dead_stubs():
+    # this was a bug detected in performance testing which generated a 1d invalid stub.
+    # this failed originally because a 1D stub between Sun 2nd May 27 and Mon 3rd May 27
+    # was invalid since the adjusted accrual schedule modified the sunday to be
+    # equal to the Monday giving a 0 day period.
+    s = Schedule(
+        dt(2027, 5, 2),
+        dt(2046, 5, 3),
+        "A",
+        "SHORTFRONT",
+        None,
+        None,
+        None,
+        None,
+        False,
+        "bus",
+        None,
+    )
+    assert s.uschedule[0:2] == [dt(2027, 5, 3), dt(2028, 5, 3)]
+    assert s.aschedule[0:2] == [dt(2027, 5, 3), dt(2028, 5, 3)]
+
+    # manipulate this test to cover the case for dual sided stubs
+    s = Schedule(
+        dt(2027, 5, 2),
+        dt(2046, 6, 3),
+        "A",
+        "SHORTFRONTSHORTBACK",
+        None,
+        dt(2046, 5, 3),  # back stub means front stub is inferred
+        None,
+        None,
+        False,
+        "bus",
+        None,
+    )
+    assert s.uschedule[0:2] == [dt(2027, 5, 3), dt(2028, 5, 3)]
+    assert s.aschedule[0:2] == [dt(2027, 5, 3), dt(2028, 5, 3)]
+
+    # this was a bug detected in performance testing which generated a 1d invalid stub.
+    # this failed originally because the ueffective date of Sat 20-dec-25 and the
+    # inferred front stub of Sun 21-dec-25 both adjusted forwards to 22-dec-25
+    # giving a 0 day period.
+    s = Schedule(
+        dt(2025, 12, 20),
+        dt(2069, 12, 21),
+        "A",
+        "SHORTFRONT",
+        None,
+        None,
+        None,
+        None,
+        False,
+        "bus",
+        None,
+    )
+    assert s.uschedule[0:2] == [dt(2025, 12, 21), dt(2026, 12, 21)]
+    assert s.aschedule[0:2] == [dt(2025, 12, 22), dt(2026, 12, 21)]
+
+    # this was a bug detected in performance testing which generated a 1d invalid stub.
+    # this failed originally because the utermination date of Sat 20-dec-25 and the
+    # inferred front stub of Sun 21-dec-25 both adjusted forwards to 22-dec-25
+    # giving a 0 day period.
+    s = Schedule(
+        dt(2027, 10, 19),
+        dt(2047, 10, 20),
+        "A",
+        "SHORTBACK",
+        None,
+        None,
+        None,
+        None,
+        False,
+        "bus",
+        None,
+    )
+    assert s.uschedule[-2:] == [dt(2046, 10, 19), dt(2047, 10, 19)]
+    assert s.aschedule[-2:] == [dt(2046, 10, 19), dt(2047, 10, 21)]
+
+    # manipulate this test for dual sided stubs
+    s = Schedule(
+        dt(2027, 8, 19),
+        dt(2047, 10, 20),
+        "A",
+        "SHORTFRONTSHORTBACK",
+        dt(2027, 10, 19),
+        None,
+        None,
+        None,
+        False,
+        "bus",
+        None,
+    )
+    assert s.uschedule[-2:] == [dt(2046, 10, 19), dt(2047, 10, 19)]
+    assert s.aschedule[-2:] == [dt(2046, 10, 19), dt(2047, 10, 21)]
```

### Comparing `rateslib-0.2.0/tests/test_solver.py` & `rateslib-0.3.0/tests/test_solver.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,100 @@
 import pytest
 from datetime import datetime as dt
 from pandas import DataFrame, MultiIndex
-from pandas.testing import assert_frame_equal
+from pandas.testing import assert_frame_equal, assert_series_equal
 import numpy as np
 from numpy.testing import assert_allclose
 from math import log, exp
 
 import context
 from rateslib import default_context
-from rateslib.curves import Curve, index_left, LineCurve
-from rateslib.solver import Solver
-from rateslib.dual import Dual
+from rateslib.curves import Curve, index_left, LineCurve, CompositeCurve
+from rateslib.solver import Solver, Gradients
+from rateslib.dual import Dual, Dual2
 from rateslib.instruments import IRS, Value, FloatRateBond, Portfolio, XCS
 from rateslib.fx import FXRates, FXForwards
 
 
+class TestGradients:
+
+    @classmethod
+    def setup_class(cls):
+        class Inst:
+            def __init__(self, rate):
+                self._rate = rate
+
+            def rate(self, *args, **kwargs):
+                return self._rate
+
+        class SolverProxy(Gradients):
+            variables = ["v1", "v2", "v3"]
+            r = [
+                Dual(1.0, "v1"),
+                Dual(3.0, ["v1", "v2", "v3"], [2.0, 1.0, -2.0])
+            ]
+            _J = None
+            instruments = [
+                [Inst(Dual2(1.0, "v1", [1.], [[4.]])), tuple(), {}],
+                [Inst(Dual2(
+                    3.0,
+                    ["v1", "v2", "v3"],
+                    [2.0, 1.0, -2.0],
+                    [[-2.0, 1.0, 1.0],
+                     [1.0, -3.0, 2.0],
+                     [1.0, 2.0, -4.0]]
+                )), tuple(), {}]
+            ]
+            _J2 = None
+            _ad = 2
+            _grad_s_vT = np.array([
+                [1., 2.0, 3.0],
+                [2.0, 3.0, 4.0],
+            ])
+
+        setattr(cls, "solver", SolverProxy())
+
+    def test_J(self):
+        expected = np.array([
+            [1., 2.],
+            [0., 1.],
+            [0., -2.0],
+        ])
+        result = self.solver.J
+        assert_allclose(result, expected)
+
+    def test_grad_v_rT(self):
+        assert_allclose(self.solver.J, self.solver.grad_v_rT)
+
+    def test_J2(self):
+        expected = np.array([[
+            [8.0, 0.0, 0.0],
+            [0.0, 0.0, 0.0],
+            [0.0, 0.0, 0.0],
+        ], [
+            [-4.0, 2.0, 2.0],
+            [2.0, -6.0, 4.0],
+            [2.0, 4.0, -8.0],
+        ]])
+        expected = np.transpose(expected, (1, 2, 0))
+        result = self.solver.J2
+        assert_allclose(expected, result)
+
+    def test_grad_v_v_rT(self):
+        assert_allclose(self.solver.J2, self.solver.grad_v_v_rT)
+
+    def test_grad_s_vT(self):
+        expected = np.array([
+            [1.0, 2.0, 3.0],
+            [2.0, 3.0, 4.0],
+        ])
+        result = self.solver.grad_s_vT
+        assert_allclose(expected, result)
+
+
 @pytest.mark.parametrize("algo", [
     "gauss_newton",
     "levenberg_marquardt",
     "gradient_descent"
 ])
 def test_basic_solver(algo):
     curve = Curve({
@@ -104,15 +180,15 @@
         curves=[curve],
         instruments=instruments,
         s=s,
         algorithm=algo,
     )
     assert float(solver.g) < 1e-9
     for i, key in enumerate(curve.nodes.keys()):
-        assert abs(float(curve.nodes[key]) - s[i]) < 1e-6
+        assert abs(float(curve.nodes[key]) - s[i]) < 1e-5
 
 
 def test_basic_spline_solver():
     spline_curve = Curve(
         nodes={
             dt(2022, 1, 1): 1.0,
             dt(2023, 1, 1): 0.99,
@@ -246,14 +322,88 @@
     for i, instrument in enumerate(instruments):
         assert abs(
             float(instrument[0].rate(*instrument[1], **instrument[2]) - s[i])
         ) < 1e-7
     assert independent_curve == expected
 
 
+class TestSolverCompositeCurve:
+
+    def test_solver_composite_curve(self):
+        # this test creates a solver with a composite curve
+        # for the purpose of adding a turn
+        c_base = Curve({
+            dt(2022, 1, 1): 1.0,
+            dt(2023, 1, 1): 1.0,
+            dt(2024, 1, 1): 1.0,
+            dt(2025, 1, 1): 1.0
+        }, id="sek_base")
+        c_turns = Curve({
+            dt(2022, 1, 1): 1.0,
+            dt(2022, 12, 30): 1.0,
+            dt(2023, 1, 1): 1.0,
+            dt(2025, 1, 1): 1.0,
+        }, id="sek_turns")
+        composite_curve = CompositeCurve([c_base, c_turns], id="sek")
+
+        instruments_turns = [
+            IRS(dt(2022, 1, 1), "1d", "A", curves="sek_turns"),
+            IRS(dt(2022, 12, 30), "1d", "A", curves="sek_turns"),
+            IRS(dt(2023, 1, 1), "1d", "A", curves="sek_turns"),
+        ]
+        s_turns = [0.0, -0.50, 0.0]
+        labels_turns = ["NA1", "Turn1", "NA2"]
+
+        instruments_base = [
+            IRS(dt(2022, 1, 1), "1Y", "A", curves="sek"),
+            IRS(dt(2022, 1, 1), "2Y", "A", curves="sek"),
+            IRS(dt(2022, 1, 1), "3Y", "A", curves="sek"),
+        ]
+        s_base = [2.0, 2.3, 2.4]
+        labels_base = ["1Y", "2Y", "3Y"]
+
+        solver = Solver(
+            curves=[c_base, c_turns, composite_curve],
+            instruments=instruments_turns+instruments_base,
+            s=s_turns+s_base,
+            instrument_labels=labels_turns+labels_base,
+            id="solv"
+        )
+
+        test_irs = IRS(dt(2022, 6, 1), "15M", "A", notional=1e6, curves="sek")
+
+        expected = 2.31735564
+        result = test_irs.rate(solver=solver)
+        assert (result - expected) < 1e-8
+
+        delta = test_irs.delta(solver=solver)
+        expected = DataFrame(
+            data=[
+                -0.226074787,
+                0.2257131776,
+                0.0003616069,
+                -9.159037835,
+                131.75543312,
+                0.0033383280
+            ],
+            columns=MultiIndex.from_tuples(
+                [("usd", "usd")], names=["local_ccy", "display_ccy"]
+            ),
+            index=MultiIndex.from_tuples([
+                ("instruments", "solv", "NA1"),
+                ("instruments", "solv", "Turn1"),
+                ("instruments", "solv", "NA2"),
+                ("instruments", "solv", "1Y"),
+                ("instruments", "solv", "2Y"),
+                ("instruments", "solv", "3Y"),
+            ], names=["type", "solver", "label"]),
+        )
+        assert_frame_equal(delta, expected)
+
+
 def test_non_unique_curves():
     curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.98}, id="A")
     curve2 = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.98}, id="A")
     solver = Solver(
         curves=[curve],
         instruments=[(IRS(dt(2022, 1, 1), "1Y", "Q"), (curve,), {})],
         s=[1]
@@ -303,15 +453,15 @@
 def test_solver_pre_solver_dependency_generates_same_delta():
     """
     Build an ESTR curve with solver1.
     Build an IBOR curve with solver2 dependent upon solver1.
 
     Build an ESTR and IBOR curve simultaneously inside the same solver3.
 
-    :return:
+    Test the delta and the instrument calibration error
     """
     eur_disc_curve = Curve(
         nodes={
             dt(2022, 1, 1): 1.0,
             dt(2023, 1, 1): 1.0,
             dt(2024, 1, 1): 1.0
         },
@@ -374,14 +524,18 @@
     eur_swap = IRS(dt(2022, 3, 1), "16M", "M", fixed_rate=3.0, )
 
     delta_sim = eur_swap.delta([eur_ibor_curve2, eur_disc_curve2], eur_solver_sim)
     delta_pre = eur_swap.delta([eur_ibor_curve, eur_disc_curve], eur_solver2)
     delta_pre.index = delta_sim.index
     assert_frame_equal(delta_sim, delta_pre)
 
+    error_sim = eur_solver_sim.error
+    error_pre = eur_solver2.error
+    assert_series_equal(error_pre, error_sim, check_index=False, rtol=1e-5, atol=1e-3)
+
 
 def test_delta_gamma_calculation():
     estr_curve = Curve({dt(2022, 1, 1): 1.0, dt(2032, 1, 1): 1.0, dt(2042, 1, 1): 1.0},
                        id="estr_curve")
     estr_instruments = [
         (IRS(dt(2022, 1, 1), "10Y", "A"), (estr_curve,), {}),
         (IRS(dt(2022, 1, 1), "20Y", "A"), (estr_curve,), {}),
@@ -656,15 +810,15 @@
          ([f_c, d_c],), {"metric": "spread"}),
         (FloatRateBond(dt(2022, 1, 1), "18m", "Q", spread_compound_method="isda_compounding", settle=2),
          ([f_c, d_c],), {"metric": "spread"}),
     ]
     solver = Solver([d_c], instruments, [25, 25, 25])
     result = d_c.rate(dt(2022, 7, 1), "1D")
     expected = f_c.rate(dt(2022, 7, 1), "1D") + 0.25
-    assert abs(result - expected) < 1e-5
+    assert abs(result - expected) < 3e-4
 
 
 def test_solver_grad_s_s_vt_methods_equivalent():
     curve = Curve(
         nodes={
             dt(2022, 1, 1): 1.0,
             dt(2023, 1, 1): 1.0,
@@ -893,17 +1047,68 @@
     )
     pf = Portfolio([irs, irs2])
     pf.npv(solver=combined_solver)
     pf.delta(solver=combined_solver)
     fxr = FXRates({"eurusd": 1.10})
     fxr._set_ad_order(2)
     result = pf.gamma(solver=combined_solver, fx=fxr, base="eur")
-
-    # TODO define test result
-    raise NotImplementedError("this test needs to have a result comparison")
+    expected = DataFrame(
+        data=[
+            [0., 0., 0., 0., 0.],
+            [0., 0., 0., 0., 0.],
+            [0., 0., 0.13769, 0.28088, 0.],
+            [0., 0., 0.28088, 0.44493, 0.],
+            [0., 0., 0., 0., 0.],
+            [-0.28930, -0.45081, 0., 0., -0.68937],
+            [-0.45081, -0.47449, 0., 0., -1.37372],
+            [0., 0., 0., 0., 0.],
+            [0., 0., 0., 0., 0.],
+            [-0.68937, -1.37372, 0., 0., 0.00064],
+            [-0.31823, -0.49590, 0., 0., 0.],
+            [-0.49590, -0.52194, 0., 0., 0.],
+            [0., 0., 0., 0., 0.],
+            [0., 0., 0., 0., 0.],
+            [0., 0., 0., 0., 0.],
+            [-0.28930, -0.45081, 0., 0., -0.68937],
+            [-0.45081, -0.47449, 0., 0., -1.37372],
+            [0., 0., 0.13770, 0.28088, 0.],
+            [0., 0., 0.28088, 0.44493, 0.],
+            [-0.68937, -1.37372, 0., 0., 0.00064],
+        ],
+        index=MultiIndex.from_tuples([
+            ("eur", "eur", "instruments", "sofr", "4m"),
+            ("eur", "eur", "instruments", "sofr", "8m"),
+            ("eur", "eur", "instruments", "estr", "3m"),
+            ("eur", "eur", "instruments", "estr", "9m"),
+            ("eur", "eur", "fx", "fx", "eurusd"),
+            ("usd", "eur", "instruments", "sofr", "4m"),
+            ("usd", "eur", "instruments", "sofr", "8m"),
+            ("usd", "eur", "instruments", "estr", "3m"),
+            ("usd", "eur", "instruments", "estr", "9m"),
+            ("usd", "eur", "fx", "fx", "eurusd"),
+            ("usd", "usd", "instruments", "sofr", "4m"),
+            ("usd", "usd", "instruments", "sofr", "8m"),
+            ("usd", "usd", "instruments", "estr", "3m"),
+            ("usd", "usd", "instruments", "estr", "9m"),
+            ("usd", "usd", "fx", "fx", "eurusd"),
+            ("all", "eur", "instruments", "sofr", "4m"),
+            ("all", "eur", "instruments", "sofr", "8m"),
+            ("all", "eur", "instruments", "estr", "3m"),
+            ("all", "eur", "instruments", "estr", "9m"),
+            ("all", "eur", "fx", "fx", "eurusd"),
+        ], names=["local_ccy", "display_ccy", "type", "solver", "label"]),
+        columns=MultiIndex.from_tuples([
+            ("instruments", "sofr", "4m"),
+            ("instruments", "sofr", "8m"),
+            ("instruments", "estr", "3m"),
+            ("instruments", "estr", "9m"),
+            ("fx", "fx", "eurusd"),
+        ], names=["type", "solver", "label"])
+    )
+    assert_frame_equal(result, expected, atol=1e-2, rtol=1e-4)
 
 
 def test_solver_gamma_pnl_explain():
     instruments = [
         IRS(dt(2022, 1, 1), "10y", "A", currency="usd", curves="sofr"),
         IRS(dt(2032, 1, 1), "10y", "A", currency="usd", curves="sofr"),
         IRS(dt(2022, 1, 1), "10y", "A", currency="eur", curves="estr"),
@@ -926,15 +1131,15 @@
     )
     fxr = FXRates({"eurusd": 1.05}, settlement=dt(2022, 1, 3))
     fxf = FXForwards(fxr, {
         "eureur": estr,
         "eurusd": eurusd,
         "usdusd": sofr
     })
-    sofr_solver= Solver(
+    sofr_solver = Solver(
         curves=[sofr],
         instruments=instruments[:2],
         s=[3.45, 2.85],
         instrument_labels=["10y", "10y10y"],
         id="sofr",
         fx=fxf
     )
@@ -955,25 +1160,78 @@
         fx=fxf,
         pre_solvers=[sofr_solver, estr_solver]
     )
 
     pf = Portfolio([
         IRS(dt(2022, 1, 1), "20Y", "A", currency="eur", fixed_rate=2.0, notional=1e8, curves="estr"),
     ])
-    npv_base = pf.npv(solver=solver)
-    delta_base = pf.delta(solver=solver)
-    gamma_base = pf.gamma(solver=solver)
 
-    # s_new = np.array([3.65, 2.99, 2.10, 0.6, -25, -20])
-    # solver.s = s_new
-    # solver.iterate()
-    # npv_new = pf.npv(solver=solver)
+    npv_base = pf.npv(solver=solver, base="eur")
+    expected_npv = -6230451.035973
+    assert (npv_base - expected_npv) < 1e-5
+
+    delta_base = pf.delta(solver=solver, base="usd")
+    # this expectation is directly input from reviewed output.
+    expected_delta = DataFrame(
+        data=[
+            [3.51021, 0.0, 3.51021],
+            [-0.00005, 0.0, -0.00005],
+            [101841.37433, 97001.98184, 101841.37433],
+            [85750.45235, 81672.83139, 85750.45235],
+            [-3.55593, 0.0, -3.55593],
+            [0.00004, 0.0, 0.00004],
+            [-623.00136, 0.0, -623.00136],
+        ],
+        index=MultiIndex.from_tuples([
+            ("instruments", "sofr", "10y"),
+            ("instruments", "sofr", "10y10y"),
+            ("instruments", "estr", "10y"),
+            ("instruments", "estr", "10y10y"),
+            ("instruments", "xccy", "10y"),
+            ("instruments", "xccy", "10y10y"),
+            ("fx", "fx", "eurusd"),
+        ], names=["type", "solver", "label"]),
+        columns=MultiIndex.from_tuples(
+            [("all", "usd"), ("eur", "eur"), ("eur", "usd")],
+            names=["local_ccy", "display_ccy"]
+        )
+    )
+    assert_frame_equal(delta_base, expected_delta, atol=1e-2, rtol=1e-4)
 
-    # TODO comparison
-    raise NotImplementedError("this test needs a result to be defined")
+    gamma_base = pf.gamma(solver=solver)
+    expected_gamma = DataFrame(
+        data=[
+            [0., 0., 0., 0., 0., 0., 0.],
+            [0., 0., 0., 0., 0., 0., 0.],
+            [0., 0., -102.972447, -81.00807888, 0., 0., 0.],
+            [0., 0., -81.00807888, -87.84105303, 0., 0., 0.],
+            [0., 0., 0., 0., 0., 0., 0.],
+            [0., 0., 0., 0., 0., 0., 0.],
+            [0., 0., 0., 0., 0., 0., 0.]
+        ],
+        index=MultiIndex.from_tuples([
+            ("eur", "eur", "instruments", "sofr", "10y"),
+            ("eur", "eur", "instruments", "sofr", "10y10y"),
+            ("eur", "eur", "instruments", "estr", "10y"),
+            ("eur", "eur", "instruments", "estr", "10y10y"),
+            ("eur", "eur", "instruments", "xccy", "10y"),
+            ("eur", "eur", "instruments", "xccy", "10y10y"),
+            ("eur", "eur", "fx", "fx", "eurusd"),
+        ], names=["local_ccy", "display_ccy", "type", "solver", "label"]),
+        columns=MultiIndex.from_tuples([
+            ("instruments", "sofr", "10y"),
+            ("instruments", "sofr", "10y10y"),
+            ("instruments", "estr", "10y"),
+            ("instruments", "estr", "10y10y"),
+            ("instruments", "xccy", "10y"),
+            ("instruments", "xccy", "10y10y"),
+            ("fx", "fx", "eurusd"),
+        ], names=["type", "solver", "label"]),
+    )
+    assert_frame_equal(gamma_base, expected_gamma, atol=1e-2, rtol=1e-4)
 
 
 def test_gamma_with_fxrates_ad_order_1_raises():
     # when calculating gamma, AD order 2 is needed, the fx rates object passed
     # must also be converted. TODO
     pass
 
@@ -1014,7 +1272,72 @@
         solver2 = Solver(
             curves=[curve2],
             instruments=[(IRS(dt(2022, 1, 1), "1Y", "Q"), (curve2,), {})],
             s=[1],
             id="bad",
             pre_solvers=[solver]
         )
+
+
+def test_solving_indirect_parameters_from_proxy_composite():
+    eureur = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 1.0}, id="eureur")
+    eurspd = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.999}, id="eurspd")
+    eur3m = CompositeCurve([eureur, eurspd], id="eur3m")
+    usdusd = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 1.0}, id="usdusd")
+    eurusd = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 1.0}, id="eurusd")
+    fxr = FXRates({"eurusd": 1.1}, settlement=dt(2022, 1, 3))
+    fxf = FXForwards(
+        fx_rates=fxr,
+        fx_curves={
+            "eureur": eureur,
+            "usdusd": usdusd,
+            "eurusd": eurusd,
+        }
+    )
+    usdeur = fxf.curve("usd", "eur", id="usdeur")
+    instruments = [
+        IRS(dt(2022, 1, 1), "1Y", "A", currency="eur", curves=["eur3m", "eureur"]),
+        IRS(dt(2022, 1, 1), "1Y", "A", currency="usd", curves="usdusd"),
+        XCS(dt(2022, 1, 1), "1Y", "A", currency="eur", leg2_currency="usd",
+            curves=["eureur", "eureur", "usdusd", "usdeur"]),
+    ]
+    solver = Solver(curves=[eureur, eur3m, usdusd, eurusd, usdeur],
+                    instruments=instruments, s=[2.0, 2.7, -15], fx=fxf)
+
+
+def test_solver_dimensions_of_matmul():
+    swaps = [
+        IRS(dt(2023, 7, 21), "9m", "A", fixed_rate=2.0, curves="chf", currency="chf"),
+        IRS(dt(2023, 7, 21), "9m", "A", fixed_rate=2.0, curves="gbp", currency="gbp"),
+        IRS(dt(2023, 7, 21), "9m", "A", fixed_rate=2.0, curves="usd", currency="usd"),
+    ]
+    chf_inst = [
+        IRS(dt(2023, 7, 21), "6m", "A", curves="chf", currency="chf"),
+        IRS(dt(2023, 7, 21), "1y", "A", curves="chf", currency="chf"),
+    ]
+    gbp_inst = [
+        IRS(dt(2023, 7, 21), "6m", "A", curves="gbp", currency="gbp"),
+        IRS(dt(2023, 7, 21), "1y", "A", curves="gbp", currency="gbp"),
+    ]
+    usd_inst = [
+        IRS(dt(2023, 7, 21), "6m", "A", curves="usd", currency="usd"),
+        IRS(dt(2023, 7, 21), "1y", "A", curves="usd", currency="usd"),
+    ]
+    usd = Curve(
+        {dt(2023, 7, 21): 1.0, dt(2024, 1, 21): 1.0, dt(2024, 7, 21): 1.0},
+        id="usd",
+    )
+    gbp = Curve(
+        {dt(2023, 7, 21): 1.0, dt(2024, 1, 21): 1.0, dt(2024, 7, 21): 1.0},
+        id="gbp",
+    )
+    chf = Curve(
+        {dt(2023, 7, 21): 1.0, dt(2024, 1, 21): 1.0, dt(2024, 7, 21): 1.0},
+        id="chf",
+    )
+    fxr = FXRates({"gbpusd": 1.25, "chfgbp": 1.1})
+    solver1 = Solver(curves=[chf], instruments=chf_inst, s=[1.5, 1.8], id="CHF")
+    solver2 = Solver(curves=[gbp], instruments=gbp_inst, s=[1.6, 1.7], id="GBP", pre_solvers=[solver1])
+    solver3 = Solver(curves=[usd], instruments=usd_inst, s=[1.7, 1.9], id="USD", pre_solvers=[solver2])
+    pf = Portfolio(swaps)
+    result = pf.delta(solver=solver3, base="gbp", fx=fxr)
+    result2 = pf.gamma(solver=solver3, base="gbp", fx=fxr)
```

### Comparing `rateslib-0.2.0/tests/test_splines.py` & `rateslib-0.3.0/tests/test_splines.py`

 * *Files identical despite different names*

