# Comparing `tmp/UliEngineering-0.4.3.tar.gz` & `tmp/UliEngineering-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UliEngineering-0.4.3.tar", last modified: Tue Jul 18 16:03:19 2023, max compression
+gzip compressed data, was "UliEngineering-0.4.4.tar", last modified: Fri Jul 28 18:23:06 2023, max compression
```

## Comparing `UliEngineering-0.4.3.tar` & `UliEngineering-0.4.4.tar`

### file list

```diff
@@ -1,95 +1,98 @@
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-18 16:03:19.908412 UliEngineering-0.4.3/
--rw-rw-r--   0 uli       (1000) uli       (1000)    11342 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/LICENSE
--rw-rw-r--   0 uli       (1000) uli       (1000)     1048 2023-07-18 16:03:19.908412 UliEngineering-0.4.3/PKG-INFO
--rw-rw-r--   0 uli       (1000) uli       (1000)     6808 2023-07-18 15:59:30.000000 UliEngineering-0.4.3/README.md
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-18 16:03:19.888412 UliEngineering-0.4.3/UliEngineering/
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-18 16:03:19.888412 UliEngineering-0.4.3/UliEngineering/Economics/
--rw-rw-r--   0 uli       (1000) uli       (1000)     3661 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Economics/Interest.py
--rw-rw-r--   0 uli       (1000) uli       (1000)        0 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Economics/__init__.py
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-18 16:03:19.892412 UliEngineering-0.4.3/UliEngineering/Electronics/
--rwxrwxr-x   0 uli       (1000) uli       (1000)     1798 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Electronics/Capacitors.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     5427 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Electronics/Crystal.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     7882 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Electronics/Hysteresis.py
--rwxrwxr-x   0 uli       (1000) uli       (1000)      753 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Electronics/Inductors.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     2557 2023-05-20 01:18:20.000000 UliEngineering-0.4.3/UliEngineering/Electronics/LED.py
--rwxrwxr-x   0 uli       (1000) uli       (1000)     1960 2023-07-18 16:02:10.000000 UliEngineering-0.4.3/UliEngineering/Electronics/MOSFET.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     7077 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Electronics/Microstrip.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     1035 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Electronics/OpAmp.py
--rw-rw-r--   0 uli       (1000) uli       (1000)      873 2022-09-01 22:45:17.000000 UliEngineering-0.4.3/UliEngineering/Electronics/Power.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     1048 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Electronics/PowerFactor.py
--rwxrwxr-x   0 uli       (1000) uli       (1000)      786 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Electronics/Reactance.py
--rwxrwxr-x   0 uli       (1000) uli       (1000)     6324 2023-03-06 14:19:49.000000 UliEngineering-0.4.3/UliEngineering/Electronics/Resistors.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     6543 2022-09-01 22:45:17.000000 UliEngineering-0.4.3/UliEngineering/Electronics/TemperatureCoefficient.py
--rw-rw-r--   0 uli       (1000) uli       (1000)      884 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Electronics/Tolerance.py
--rwxrwxr-x   0 uli       (1000) uli       (1000)     5948 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Electronics/VoltageDivider.py
--rw-rw-r--   0 uli       (1000) uli       (1000)        0 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Electronics/__init__.py
--rwxrwxr-x   0 uli       (1000) uli       (1000)    21499 2022-09-01 22:45:17.000000 UliEngineering-0.4.3/UliEngineering/EngineerIO.py
--rw-rw-r--   0 uli       (1000) uli       (1000)      534 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Exceptions.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     2622 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Length.py
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-18 16:03:19.896412 UliEngineering-0.4.3/UliEngineering/Math/
--rw-rw-r--   0 uli       (1000) uli       (1000)     1890 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Math/Coordinates.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     2885 2023-05-20 01:18:20.000000 UliEngineering-0.4.3/UliEngineering/Math/Decibel.py
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-18 16:03:19.896412 UliEngineering-0.4.3/UliEngineering/Math/Geometry/
--rw-rw-r--   0 uli       (1000) uli       (1000)      591 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Math/Geometry/Circle.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     3668 2023-05-20 01:56:07.000000 UliEngineering-0.4.3/UliEngineering/Math/Geometry/Cylinder.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     1588 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Math/Geometry/Polygon.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     1113 2022-09-13 18:18:08.000000 UliEngineering-0.4.3/UliEngineering/Math/Geometry/Sphere.py
--rw-rw-r--   0 uli       (1000) uli       (1000)        0 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Math/Geometry/__init__.py
--rw-rw-r--   0 uli       (1000) uli       (1000)        0 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Math/__init__.py
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-18 16:03:19.896412 UliEngineering-0.4.3/UliEngineering/Mechanics/
--rw-rw-r--   0 uli       (1000) uli       (1000)     1493 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Mechanics/Threads.py
--rw-rw-r--   0 uli       (1000) uli       (1000)        0 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Mechanics/__init__.py
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-18 16:03:19.900412 UliEngineering-0.4.3/UliEngineering/Physics/
--rw-rw-r--   0 uli       (1000) uli       (1000)     1968 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Physics/Acceleration.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     3378 2023-05-20 01:51:18.000000 UliEngineering-0.4.3/UliEngineering/Physics/Density.py
--rw-rw-r--   0 uli       (1000) uli       (1000)      953 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Physics/Frequency.py
--rwxrwxr-x   0 uli       (1000) uli       (1000)     1835 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Physics/JohnsonNyquistNoise.py
--rwxrwxr-x   0 uli       (1000) uli       (1000)     1023 2022-09-01 22:45:17.000000 UliEngineering-0.4.3/UliEngineering/Physics/Light.py
--rw-rw-r--   0 uli       (1000) uli       (1000)      991 2023-03-06 14:19:49.000000 UliEngineering-0.4.3/UliEngineering/Physics/MagneticResonance.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     1451 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Physics/NTC.py
--rwxrwxr-x   0 uli       (1000) uli       (1000)     1012 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Physics/NoiseDensity.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     1355 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Physics/Pressure.py
--rwxrwxr-x   0 uli       (1000) uli       (1000)     2234 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Physics/RF.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     4945 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Physics/RTD.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     2175 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Physics/Rotation.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     2489 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Physics/Temperature.py
--rw-rw-r--   0 uli       (1000) uli       (1000)        0 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Physics/__init__.py
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-18 16:03:19.904412 UliEngineering-0.4.3/UliEngineering/SignalProcessing/
--rw-rw-r--   0 uli       (1000) uli       (1000)     8963 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/SignalProcessing/Chunks.py
--rw-rw-r--   0 uli       (1000) uli       (1000)      492 2022-09-01 22:45:17.000000 UliEngineering-0.4.3/UliEngineering/SignalProcessing/Correlation.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     1747 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/SignalProcessing/DateTime.py
--rwxrwxr-x   0 uli       (1000) uli       (1000)    12299 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/SignalProcessing/FFT.py
--rw-rw-r--   0 uli       (1000) uli       (1000)    11914 2022-09-01 22:45:17.000000 UliEngineering-0.4.3/UliEngineering/SignalProcessing/Filter.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     3030 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/SignalProcessing/Normalize.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     9022 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/SignalProcessing/Resampling.py
--rw-rw-r--   0 uli       (1000) uli       (1000)    19078 2022-09-01 22:45:17.000000 UliEngineering-0.4.3/UliEngineering/SignalProcessing/Selection.py
--rwxrwxr-x   0 uli       (1000) uli       (1000)     2446 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/SignalProcessing/Simulation.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     9831 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/SignalProcessing/Utils.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     1710 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/SignalProcessing/Weight.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     3332 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/SignalProcessing/Window.py
--rw-rw-r--   0 uli       (1000) uli       (1000)       22 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/SignalProcessing/__init__.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     2081 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Units.py
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-18 16:03:19.908412 UliEngineering-0.4.3/UliEngineering/Utils/
--rw-rw-r--   0 uli       (1000) uli       (1000)     1173 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Utils/Compression.py
--rw-rw-r--   0 uli       (1000) uli       (1000)      662 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Utils/Concurrency.py
--rw-rw-r--   0 uli       (1000) uli       (1000)    11944 2023-07-18 15:59:54.000000 UliEngineering-0.4.3/UliEngineering/Utils/Date.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     6193 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Utils/Files.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     3687 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Utils/Iterable.py
--rw-rw-r--   0 uli       (1000) uli       (1000)      606 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Utils/JSON.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     6972 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Utils/NumPy.py
--rw-rw-r--   0 uli       (1000) uli       (1000)      664 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Utils/Parser.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     1806 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Utils/Range.py
--rw-rw-r--   0 uli       (1000) uli       (1000)      286 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Utils/Slice.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     1348 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Utils/String.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     2372 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Utils/Temporary.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     2621 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Utils/ZIP.py
--rw-rw-r--   0 uli       (1000) uli       (1000)      104 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Utils/__init__.py
--rwxrwxr-x   0 uli       (1000) uli       (1000)       23 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/__init__.py
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-18 16:03:19.888412 UliEngineering-0.4.3/UliEngineering.egg-info/
--rw-rw-r--   0 uli       (1000) uli       (1000)     1048 2023-07-18 16:03:19.000000 UliEngineering-0.4.3/UliEngineering.egg-info/PKG-INFO
--rw-rw-r--   0 uli       (1000) uli       (1000)     2954 2023-07-18 16:03:19.000000 UliEngineering-0.4.3/UliEngineering.egg-info/SOURCES.txt
--rw-rw-r--   0 uli       (1000) uli       (1000)        1 2023-07-18 16:03:19.000000 UliEngineering-0.4.3/UliEngineering.egg-info/dependency_links.txt
--rw-rw-r--   0 uli       (1000) uli       (1000)       56 2023-07-18 16:03:19.000000 UliEngineering-0.4.3/UliEngineering.egg-info/requires.txt
--rw-rw-r--   0 uli       (1000) uli       (1000)       15 2023-07-18 16:03:19.000000 UliEngineering-0.4.3/UliEngineering.egg-info/top_level.txt
--rw-rw-r--   0 uli       (1000) uli       (1000)      100 2023-07-18 16:03:19.908412 UliEngineering-0.4.3/setup.cfg
--rwxrwxr-x   0 uli       (1000) uli       (1000)     1578 2023-07-18 16:00:52.000000 UliEngineering-0.4.3/setup.py
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-28 18:23:06.805311 UliEngineering-0.4.4/
+-rw-rw-r--   0 uli       (1000) uli       (1000)    11342 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/LICENSE
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1038 2023-07-28 18:23:06.805311 UliEngineering-0.4.4/PKG-INFO
+-rw-rw-r--   0 uli       (1000) uli       (1000)     6808 2023-07-28 16:51:33.000000 UliEngineering-0.4.4/README.md
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-28 18:23:06.785311 UliEngineering-0.4.4/UliEngineering/
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-28 18:23:06.789311 UliEngineering-0.4.4/UliEngineering/Economics/
+-rw-rw-r--   0 uli       (1000) uli       (1000)     3661 2022-02-21 16:48:03.000000 UliEngineering-0.4.4/UliEngineering/Economics/Interest.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)        0 2022-02-21 16:48:03.000000 UliEngineering-0.4.4/UliEngineering/Economics/__init__.py
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-28 18:23:06.793311 UliEngineering-0.4.4/UliEngineering/Electronics/
+-rwxr-xr-x   0 uli       (1000) uli       (1000)     1798 2021-09-18 02:45:54.000000 UliEngineering-0.4.4/UliEngineering/Electronics/Capacitors.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     5427 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Electronics/Crystal.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     7882 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Electronics/Hysteresis.py
+-rwxr-xr-x   0 uli       (1000) uli       (1000)      753 2021-09-18 02:45:54.000000 UliEngineering-0.4.4/UliEngineering/Electronics/Inductors.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     2557 2023-02-10 00:58:09.000000 UliEngineering-0.4.4/UliEngineering/Electronics/LED.py
+-rwxr-xr-x   0 uli       (1000) uli       (1000)     1960 2021-09-18 02:45:54.000000 UliEngineering-0.4.4/UliEngineering/Electronics/MOSFET.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     7077 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Electronics/Microstrip.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1035 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Electronics/OpAmp.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)      873 2022-06-19 16:15:14.000000 UliEngineering-0.4.4/UliEngineering/Electronics/Power.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1048 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Electronics/PowerFactor.py
+-rwxr-xr-x   0 uli       (1000) uli       (1000)      786 2021-09-18 02:45:55.000000 UliEngineering-0.4.4/UliEngineering/Electronics/Reactance.py
+-rwxrwxr-x   0 uli       (1000) uli       (1000)     6324 2023-02-04 03:37:45.000000 UliEngineering-0.4.4/UliEngineering/Electronics/Resistors.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     6543 2022-06-19 16:15:55.000000 UliEngineering-0.4.4/UliEngineering/Electronics/TemperatureCoefficient.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)      884 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Electronics/Tolerance.py
+-rwxrwxr-x   0 uli       (1000) uli       (1000)     5948 2022-02-21 16:48:03.000000 UliEngineering-0.4.4/UliEngineering/Electronics/VoltageDivider.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)        0 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Electronics/__init__.py
+-rwxrwxr-x   0 uli       (1000) uli       (1000)    21499 2022-06-19 16:45:11.000000 UliEngineering-0.4.4/UliEngineering/EngineerIO.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)      534 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Exceptions.py
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-28 18:23:06.793311 UliEngineering-0.4.4/UliEngineering/Filesystem/
+-rw-rw-r--   0 uli       (1000) uli       (1000)     4067 2023-07-28 18:09:29.000000 UliEngineering-0.4.4/UliEngineering/Filesystem/Hash.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)       22 2023-07-28 16:52:38.000000 UliEngineering-0.4.4/UliEngineering/Filesystem/__init__.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     2622 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Length.py
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-28 18:23:06.793311 UliEngineering-0.4.4/UliEngineering/Math/
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1890 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Math/Coordinates.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     2885 2023-03-13 04:42:02.000000 UliEngineering-0.4.4/UliEngineering/Math/Decibel.py
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-28 18:23:06.797311 UliEngineering-0.4.4/UliEngineering/Math/Geometry/
+-rw-rw-r--   0 uli       (1000) uli       (1000)      591 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Math/Geometry/Circle.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     3668 2023-07-28 16:51:33.000000 UliEngineering-0.4.4/UliEngineering/Math/Geometry/Cylinder.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1588 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Math/Geometry/Polygon.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1113 2022-09-15 15:07:11.000000 UliEngineering-0.4.4/UliEngineering/Math/Geometry/Sphere.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)        0 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Math/Geometry/__init__.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)        0 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Math/__init__.py
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-28 18:23:06.797311 UliEngineering-0.4.4/UliEngineering/Mechanics/
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1493 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Mechanics/Threads.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)        0 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Mechanics/__init__.py
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-28 18:23:06.801311 UliEngineering-0.4.4/UliEngineering/Physics/
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1968 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Physics/Acceleration.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     3378 2023-07-28 16:51:33.000000 UliEngineering-0.4.4/UliEngineering/Physics/Density.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)      953 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Physics/Frequency.py
+-rwxr-xr-x   0 uli       (1000) uli       (1000)     1835 2021-09-18 02:45:55.000000 UliEngineering-0.4.4/UliEngineering/Physics/JohnsonNyquistNoise.py
+-rwxr-xr-x   0 uli       (1000) uli       (1000)     1023 2022-06-19 16:44:08.000000 UliEngineering-0.4.4/UliEngineering/Physics/Light.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)      991 2023-02-04 03:03:35.000000 UliEngineering-0.4.4/UliEngineering/Physics/MagneticResonance.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1451 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Physics/NTC.py
+-rwxr-xr-x   0 uli       (1000) uli       (1000)     1012 2021-09-18 02:45:55.000000 UliEngineering-0.4.4/UliEngineering/Physics/NoiseDensity.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1355 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Physics/Pressure.py
+-rwxr-xr-x   0 uli       (1000) uli       (1000)     2234 2021-09-18 02:45:55.000000 UliEngineering-0.4.4/UliEngineering/Physics/RF.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     4945 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Physics/RTD.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     2175 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Physics/Rotation.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     2489 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Physics/Temperature.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)        0 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Physics/__init__.py
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-28 18:23:06.801311 UliEngineering-0.4.4/UliEngineering/SignalProcessing/
+-rw-rw-r--   0 uli       (1000) uli       (1000)     8963 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/SignalProcessing/Chunks.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)      492 2022-06-19 16:20:02.000000 UliEngineering-0.4.4/UliEngineering/SignalProcessing/Correlation.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1747 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/SignalProcessing/DateTime.py
+-rwxr-xr-x   0 uli       (1000) uli       (1000)    12299 2021-09-18 02:45:55.000000 UliEngineering-0.4.4/UliEngineering/SignalProcessing/FFT.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)    11914 2022-06-19 13:48:39.000000 UliEngineering-0.4.4/UliEngineering/SignalProcessing/Filter.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     3030 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/SignalProcessing/Normalize.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     9022 2022-02-21 16:48:04.000000 UliEngineering-0.4.4/UliEngineering/SignalProcessing/Resampling.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)    19078 2022-06-19 16:20:22.000000 UliEngineering-0.4.4/UliEngineering/SignalProcessing/Selection.py
+-rwxr-xr-x   0 uli       (1000) uli       (1000)     2446 2021-09-18 02:45:55.000000 UliEngineering-0.4.4/UliEngineering/SignalProcessing/Simulation.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     9831 2022-02-21 16:48:04.000000 UliEngineering-0.4.4/UliEngineering/SignalProcessing/Utils.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1710 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/SignalProcessing/Weight.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     3332 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/SignalProcessing/Window.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)       22 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/SignalProcessing/__init__.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     2081 2022-02-21 16:48:02.000000 UliEngineering-0.4.4/UliEngineering/Units.py
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-28 18:23:06.805311 UliEngineering-0.4.4/UliEngineering/Utils/
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1145 2023-07-28 17:30:02.000000 UliEngineering-0.4.4/UliEngineering/Utils/Compression.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)      662 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Utils/Concurrency.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)    11944 2023-07-28 16:51:33.000000 UliEngineering-0.4.4/UliEngineering/Utils/Date.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     6193 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Utils/Files.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     3687 2022-02-21 16:48:04.000000 UliEngineering-0.4.4/UliEngineering/Utils/Iterable.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)      606 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Utils/JSON.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     6972 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Utils/NumPy.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)      664 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Utils/Parser.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1806 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Utils/Range.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)      286 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Utils/Slice.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1348 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Utils/String.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     2372 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Utils/Temporary.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     2621 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Utils/ZIP.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)      104 2021-12-18 02:10:48.000000 UliEngineering-0.4.4/UliEngineering/Utils/__init__.py
+-rwxr-xr-x   0 uli       (1000) uli       (1000)       23 2021-09-18 02:45:55.000000 UliEngineering-0.4.4/UliEngineering/__init__.py
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-28 18:23:06.789311 UliEngineering-0.4.4/UliEngineering.egg-info/
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1038 2023-07-28 18:23:06.000000 UliEngineering-0.4.4/UliEngineering.egg-info/PKG-INFO
+-rw-rw-r--   0 uli       (1000) uli       (1000)     3026 2023-07-28 18:23:06.000000 UliEngineering-0.4.4/UliEngineering.egg-info/SOURCES.txt
+-rw-rw-r--   0 uli       (1000) uli       (1000)        1 2023-07-28 18:23:06.000000 UliEngineering-0.4.4/UliEngineering.egg-info/dependency_links.txt
+-rw-rw-r--   0 uli       (1000) uli       (1000)       56 2023-07-28 18:23:06.000000 UliEngineering-0.4.4/UliEngineering.egg-info/requires.txt
+-rw-rw-r--   0 uli       (1000) uli       (1000)       15 2023-07-28 18:23:06.000000 UliEngineering-0.4.4/UliEngineering.egg-info/top_level.txt
+-rw-rw-r--   0 uli       (1000) uli       (1000)      100 2023-07-28 18:23:06.805311 UliEngineering-0.4.4/setup.cfg
+-rwxrwxr-x   0 uli       (1000) uli       (1000)     1578 2023-07-28 18:16:26.000000 UliEngineering-0.4.4/setup.py
```

### Comparing `UliEngineering-0.4.3/LICENSE` & `UliEngineering-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/PKG-INFO` & `UliEngineering-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UliEngineering
-Version: 0.4.3
+Version: 0.4.4
 Summary: Computational tools for electronics engineering
 Home-page: https://techoverflow.net/
 Author: Uli Köhler
 Author-email: ukoehler@techoverflow.net
 License: Apache License v2.0
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -19,10 +19,7 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Provides-Extra: SciPy functionality
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `UliEngineering-0.4.3/README.md` & `UliEngineering-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Economics/Interest.py` & `UliEngineering-0.4.4/UliEngineering/Economics/Interest.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Electronics/Capacitors.py` & `UliEngineering-0.4.4/UliEngineering/Electronics/Capacitors.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Electronics/Crystal.py` & `UliEngineering-0.4.4/UliEngineering/Electronics/Crystal.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Electronics/Hysteresis.py` & `UliEngineering-0.4.4/UliEngineering/Electronics/Hysteresis.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Electronics/Inductors.py` & `UliEngineering-0.4.4/UliEngineering/Electronics/Inductors.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Electronics/LED.py` & `UliEngineering-0.4.4/UliEngineering/Electronics/LED.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Electronics/MOSFET.py` & `UliEngineering-0.4.4/UliEngineering/Electronics/MOSFET.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Electronics/Microstrip.py` & `UliEngineering-0.4.4/UliEngineering/Electronics/Microstrip.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Electronics/OpAmp.py` & `UliEngineering-0.4.4/UliEngineering/Electronics/OpAmp.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Electronics/Power.py` & `UliEngineering-0.4.4/UliEngineering/Electronics/Power.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Electronics/PowerFactor.py` & `UliEngineering-0.4.4/UliEngineering/Electronics/PowerFactor.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Electronics/Reactance.py` & `UliEngineering-0.4.4/UliEngineering/Electronics/Reactance.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Electronics/Resistors.py` & `UliEngineering-0.4.4/UliEngineering/Electronics/Resistors.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Electronics/TemperatureCoefficient.py` & `UliEngineering-0.4.4/UliEngineering/Electronics/TemperatureCoefficient.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Electronics/Tolerance.py` & `UliEngineering-0.4.4/UliEngineering/Electronics/Tolerance.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Electronics/VoltageDivider.py` & `UliEngineering-0.4.4/UliEngineering/Electronics/VoltageDivider.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/EngineerIO.py` & `UliEngineering-0.4.4/UliEngineering/EngineerIO.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Exceptions.py` & `UliEngineering-0.4.4/UliEngineering/Exceptions.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Length.py` & `UliEngineering-0.4.4/UliEngineering/Length.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Math/Coordinates.py` & `UliEngineering-0.4.4/UliEngineering/Math/Coordinates.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Math/Decibel.py` & `UliEngineering-0.4.4/UliEngineering/Math/Decibel.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Math/Geometry/Circle.py` & `UliEngineering-0.4.4/UliEngineering/Math/Geometry/Circle.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Math/Geometry/Cylinder.py` & `UliEngineering-0.4.4/UliEngineering/Math/Geometry/Cylinder.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Math/Geometry/Polygon.py` & `UliEngineering-0.4.4/UliEngineering/Math/Geometry/Polygon.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Math/Geometry/Sphere.py` & `UliEngineering-0.4.4/UliEngineering/Math/Geometry/Sphere.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Mechanics/Threads.py` & `UliEngineering-0.4.4/UliEngineering/Mechanics/Threads.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Physics/Acceleration.py` & `UliEngineering-0.4.4/UliEngineering/Physics/Acceleration.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Physics/Density.py` & `UliEngineering-0.4.4/UliEngineering/Physics/Density.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Physics/Frequency.py` & `UliEngineering-0.4.4/UliEngineering/Physics/Frequency.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Physics/JohnsonNyquistNoise.py` & `UliEngineering-0.4.4/UliEngineering/Physics/JohnsonNyquistNoise.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Physics/Light.py` & `UliEngineering-0.4.4/UliEngineering/Physics/Light.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Physics/MagneticResonance.py` & `UliEngineering-0.4.4/UliEngineering/Physics/MagneticResonance.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Physics/NTC.py` & `UliEngineering-0.4.4/UliEngineering/Physics/NTC.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Physics/NoiseDensity.py` & `UliEngineering-0.4.4/UliEngineering/Physics/NoiseDensity.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Physics/Pressure.py` & `UliEngineering-0.4.4/UliEngineering/Physics/Pressure.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Physics/RF.py` & `UliEngineering-0.4.4/UliEngineering/Physics/RF.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Physics/RTD.py` & `UliEngineering-0.4.4/UliEngineering/Physics/RTD.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Physics/Rotation.py` & `UliEngineering-0.4.4/UliEngineering/Physics/Rotation.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Physics/Temperature.py` & `UliEngineering-0.4.4/UliEngineering/Physics/Temperature.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/SignalProcessing/Chunks.py` & `UliEngineering-0.4.4/UliEngineering/SignalProcessing/Chunks.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/SignalProcessing/DateTime.py` & `UliEngineering-0.4.4/UliEngineering/SignalProcessing/DateTime.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/SignalProcessing/FFT.py` & `UliEngineering-0.4.4/UliEngineering/SignalProcessing/FFT.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/SignalProcessing/Filter.py` & `UliEngineering-0.4.4/UliEngineering/SignalProcessing/Filter.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/SignalProcessing/Normalize.py` & `UliEngineering-0.4.4/UliEngineering/SignalProcessing/Normalize.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/SignalProcessing/Resampling.py` & `UliEngineering-0.4.4/UliEngineering/SignalProcessing/Resampling.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/SignalProcessing/Selection.py` & `UliEngineering-0.4.4/UliEngineering/SignalProcessing/Selection.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/SignalProcessing/Simulation.py` & `UliEngineering-0.4.4/UliEngineering/SignalProcessing/Simulation.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/SignalProcessing/Utils.py` & `UliEngineering-0.4.4/UliEngineering/SignalProcessing/Utils.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/SignalProcessing/Weight.py` & `UliEngineering-0.4.4/UliEngineering/SignalProcessing/Weight.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/SignalProcessing/Window.py` & `UliEngineering-0.4.4/UliEngineering/SignalProcessing/Window.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Units.py` & `UliEngineering-0.4.4/UliEngineering/Units.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Utils/Compression.py` & `UliEngineering-0.4.4/UliEngineering/Utils/Compression.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,23 +22,23 @@
 """
 __mode_map = {
 	"r": "rt", "rb": "rb", "w": "wb", "wb": "wb",
 	"x": "xt", "xb": "xb", "a": "at", "ab": "ab",
 	"rt": "rt", "wt": "wt", "xt": "xt", "at": "at"
 }
 
-def auto_open(filename, mode="r", charset="utf8", **kwargs):
+def auto_open(filename, mode="r", **kwargs):
 	"""
 	Automatically open a potentially compressed file using the right
 	library variant of open().
 	The correct decompression algorithm is selected by filename extension.
 	This function can be used instead of open() and automatically selects
 	the right mode (text or binary).
 	"""
 	extension = os.path.splitext(filename)[1]
 	if extension not in __open_map:
 		raise ValueError(
-			"Unable to find correct decompression for extension '{0}' in filename {1}".format(extension, filename))
+			f"Unable to find correct decompression for extension '{extension}' in filename {filename}")
 	open_fn = __open_map[extension]
 	mode = __mode_map[mode] if extension else mode
 	return open_fn(filename, mode, **kwargs)
```

### Comparing `UliEngineering-0.4.3/UliEngineering/Utils/Concurrency.py` & `UliEngineering-0.4.4/UliEngineering/Utils/Concurrency.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Utils/Date.py` & `UliEngineering-0.4.4/UliEngineering/Utils/Date.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Utils/Files.py` & `UliEngineering-0.4.4/UliEngineering/Utils/Files.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Utils/Iterable.py` & `UliEngineering-0.4.4/UliEngineering/Utils/Iterable.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Utils/JSON.py` & `UliEngineering-0.4.4/UliEngineering/Utils/JSON.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Utils/NumPy.py` & `UliEngineering-0.4.4/UliEngineering/Utils/NumPy.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Utils/Parser.py` & `UliEngineering-0.4.4/UliEngineering/Utils/Parser.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Utils/Range.py` & `UliEngineering-0.4.4/UliEngineering/Utils/Range.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Utils/String.py` & `UliEngineering-0.4.4/UliEngineering/Utils/String.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Utils/Temporary.py` & `UliEngineering-0.4.4/UliEngineering/Utils/Temporary.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering/Utils/ZIP.py` & `UliEngineering-0.4.4/UliEngineering/Utils/ZIP.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.3/UliEngineering.egg-info/PKG-INFO` & `UliEngineering-0.4.4/UliEngineering.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UliEngineering
-Version: 0.4.3
+Version: 0.4.4
 Summary: Computational tools for electronics engineering
 Home-page: https://techoverflow.net/
 Author: Uli Köhler
 Author-email: ukoehler@techoverflow.net
 License: Apache License v2.0
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -19,10 +19,7 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Provides-Extra: SciPy functionality
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `UliEngineering-0.4.3/UliEngineering.egg-info/SOURCES.txt` & `UliEngineering-0.4.4/UliEngineering.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 UliEngineering/Electronics/PowerFactor.py
 UliEngineering/Electronics/Reactance.py
 UliEngineering/Electronics/Resistors.py
 UliEngineering/Electronics/TemperatureCoefficient.py
 UliEngineering/Electronics/Tolerance.py
 UliEngineering/Electronics/VoltageDivider.py
 UliEngineering/Electronics/__init__.py
+UliEngineering/Filesystem/Hash.py
+UliEngineering/Filesystem/__init__.py
 UliEngineering/Math/Coordinates.py
 UliEngineering/Math/Decibel.py
 UliEngineering/Math/__init__.py
 UliEngineering/Math/Geometry/Circle.py
 UliEngineering/Math/Geometry/Cylinder.py
 UliEngineering/Math/Geometry/Polygon.py
 UliEngineering/Math/Geometry/Sphere.py
```

### Comparing `UliEngineering-0.4.3/setup.py` & `UliEngineering-0.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup, find_packages
 
 if sys.version_info < (3, 0):
     print('ERROR: UliEngineering currently requires at least Python 3.0 to run.')
     sys.exit(1)
 
 setup(name='UliEngineering',
-      version='0.4.3',
+      version='0.4.4',
       description='Computational tools for electronics engineering',
       author='Uli Köhler',
       author_email='ukoehler@techoverflow.net',
       url='https://techoverflow.net/',
       license='Apache License v2.0',
       packages=find_packages(exclude=['tests*']),
       include_package_data=True,
```

