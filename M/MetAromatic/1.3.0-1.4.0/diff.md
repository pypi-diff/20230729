# Comparing `tmp/MetAromatic-1.3.0.tar.gz` & `tmp/MetAromatic-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MetAromatic-1.3.0.tar", last modified: Sat Jul 29 10:57:30 2023, max compression
+gzip compressed data, was "MetAromatic-1.4.0.tar", last modified: Sat Jul 29 12:51:25 2023, max compression
```

## Comparing `MetAromatic-1.3.0.tar` & `MetAromatic-1.4.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 dsw       (1000) dsw       (1000)        0 2023-07-29 10:57:30.292993 MetAromatic-1.3.0/
--rw-rw-rw-   0 dsw       (1000) dsw       (1000)    35149 2022-02-13 05:52:09.000000 MetAromatic-1.3.0/LICENSE
-drwxr-xr-x   0 dsw       (1000) dsw       (1000)        0 2023-07-29 10:57:30.249112 MetAromatic-1.3.0/MetAromatic/
--rw-r--r--   0 dsw       (1000) dsw       (1000)      191 2023-07-29 10:47:14.000000 MetAromatic-1.3.0/MetAromatic/__init__.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)     7565 2023-07-19 06:46:26.000000 MetAromatic-1.3.0/MetAromatic/batch.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)     2648 2023-07-19 06:46:26.000000 MetAromatic-1.3.0/MetAromatic/bridge.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)      987 2023-07-19 06:46:26.000000 MetAromatic-1.3.0/MetAromatic/complex_types.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)      117 2023-07-18 05:41:26.000000 MetAromatic-1.3.0/MetAromatic/consts.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)     2029 2023-07-19 06:46:26.000000 MetAromatic-1.3.0/MetAromatic/get_aromatic_midpoints.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)     3210 2023-07-19 06:46:26.000000 MetAromatic-1.3.0/MetAromatic/lone_pair_interpolators.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)    11907 2023-07-19 06:46:26.000000 MetAromatic-1.3.0/MetAromatic/pair.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)     4752 2023-07-19 06:46:26.000000 MetAromatic-1.3.0/MetAromatic/runner.py
-drwxr-xr-x   0 dsw       (1000) dsw       (1000)        0 2023-07-29 10:57:30.277036 MetAromatic-1.3.0/MetAromatic.egg-info/
--rw-r--r--   0 dsw       (1000) dsw       (1000)      931 2023-07-29 10:57:30.000000 MetAromatic-1.3.0/MetAromatic.egg-info/PKG-INFO
--rw-r--r--   0 dsw       (1000) dsw       (1000)      806 2023-07-29 10:57:30.000000 MetAromatic-1.3.0/MetAromatic.egg-info/SOURCES.txt
--rw-r--r--   0 dsw       (1000) dsw       (1000)        1 2023-07-29 10:57:30.000000 MetAromatic-1.3.0/MetAromatic.egg-info/dependency_links.txt
--rw-r--r--   0 dsw       (1000) dsw       (1000)       50 2023-07-29 10:57:30.000000 MetAromatic-1.3.0/MetAromatic.egg-info/entry_points.txt
--rw-r--r--   0 dsw       (1000) dsw       (1000)       47 2023-07-29 10:57:30.000000 MetAromatic-1.3.0/MetAromatic.egg-info/requires.txt
--rw-r--r--   0 dsw       (1000) dsw       (1000)       17 2023-07-29 10:57:30.000000 MetAromatic-1.3.0/MetAromatic.egg-info/top_level.txt
--rw-r--r--   0 dsw       (1000) dsw       (1000)      931 2023-07-29 10:57:30.292993 MetAromatic-1.3.0/PKG-INFO
--rw-r--r--   0 dsw       (1000) dsw       (1000)    19961 2023-07-29 10:56:09.000000 MetAromatic-1.3.0/README.md
--rw-r--r--   0 dsw       (1000) dsw       (1000)      567 2023-07-29 10:47:14.000000 MetAromatic-1.3.0/README_PYPI.md
--rw-r--r--   0 dsw       (1000) dsw       (1000)      651 2023-07-29 10:57:00.000000 MetAromatic-1.3.0/pyproject.toml
--rw-r--r--   0 dsw       (1000) dsw       (1000)       38 2023-07-29 10:57:30.293991 MetAromatic-1.3.0/setup.cfg
-drwxr-xr-x   0 dsw       (1000) dsw       (1000)        0 2023-07-29 10:57:30.290999 MetAromatic-1.3.0/tests/
--rw-r--r--   0 dsw       (1000) dsw       (1000)     1805 2023-07-29 10:47:14.000000 MetAromatic-1.3.0/tests/test_api_bridge.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)     1575 2023-07-29 10:47:14.000000 MetAromatic-1.3.0/tests/test_api_bridge_benchmark.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)     4344 2023-07-29 10:47:14.000000 MetAromatic-1.3.0/tests/test_api_pair.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)     2831 2023-07-29 10:47:14.000000 MetAromatic-1.3.0/tests/test_api_pair_benchmark.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)      308 2023-07-19 06:46:26.000000 MetAromatic-1.3.0/tests/test_get_hexagon_midpoints.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)     1152 2023-04-22 10:25:54.000000 MetAromatic-1.3.0/tests/test_lone_pair_interpolators.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)      304 2023-04-22 10:25:54.000000 MetAromatic-1.3.0/tests/test_resolve_runner_from_path.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)     4712 2023-04-24 08:25:14.000000 MetAromatic-1.3.0/tests/test_runner_batch.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)     1959 2023-04-23 12:19:11.000000 MetAromatic-1.3.0/tests/test_runner_bridge.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)     3906 2023-05-23 08:25:27.000000 MetAromatic-1.3.0/tests/test_runner_pair.py
+drwxr-xr-x   0 dsw       (1000) dsw       (1000)        0 2023-07-29 12:51:25.933780 MetAromatic-1.4.0/
+-rw-rw-rw-   0 dsw       (1000) dsw       (1000)    35149 2022-02-13 05:52:09.000000 MetAromatic-1.4.0/LICENSE
+drwxr-xr-x   0 dsw       (1000) dsw       (1000)        0 2023-07-29 12:51:25.876901 MetAromatic-1.4.0/MetAromatic/
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      191 2023-07-29 10:47:14.000000 MetAromatic-1.4.0/MetAromatic/__init__.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     7575 2023-07-29 12:50:24.000000 MetAromatic-1.4.0/MetAromatic/batch.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     2578 2023-07-29 12:50:24.000000 MetAromatic-1.4.0/MetAromatic/bridge.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     1867 2023-07-29 12:50:24.000000 MetAromatic-1.4.0/MetAromatic/complex_types.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      117 2023-07-18 05:41:26.000000 MetAromatic-1.4.0/MetAromatic/consts.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     2029 2023-07-19 06:46:26.000000 MetAromatic-1.4.0/MetAromatic/get_aromatic_midpoints.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     3210 2023-07-19 06:46:26.000000 MetAromatic-1.4.0/MetAromatic/lone_pair_interpolators.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)    11479 2023-07-29 12:50:24.000000 MetAromatic-1.4.0/MetAromatic/pair.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     4770 2023-07-29 12:50:24.000000 MetAromatic-1.4.0/MetAromatic/runner.py
+drwxr-xr-x   0 dsw       (1000) dsw       (1000)        0 2023-07-29 12:51:25.905824 MetAromatic-1.4.0/MetAromatic.egg-info/
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      931 2023-07-29 12:51:25.000000 MetAromatic-1.4.0/MetAromatic.egg-info/PKG-INFO
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      806 2023-07-29 12:51:25.000000 MetAromatic-1.4.0/MetAromatic.egg-info/SOURCES.txt
+-rw-r--r--   0 dsw       (1000) dsw       (1000)        1 2023-07-29 12:51:25.000000 MetAromatic-1.4.0/MetAromatic.egg-info/dependency_links.txt
+-rw-r--r--   0 dsw       (1000) dsw       (1000)       50 2023-07-29 12:51:25.000000 MetAromatic-1.4.0/MetAromatic.egg-info/entry_points.txt
+-rw-r--r--   0 dsw       (1000) dsw       (1000)       47 2023-07-29 12:51:25.000000 MetAromatic-1.4.0/MetAromatic.egg-info/requires.txt
+-rw-r--r--   0 dsw       (1000) dsw       (1000)       17 2023-07-29 12:51:25.000000 MetAromatic-1.4.0/MetAromatic.egg-info/top_level.txt
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      931 2023-07-29 12:51:25.932782 MetAromatic-1.4.0/PKG-INFO
+-rw-r--r--   0 dsw       (1000) dsw       (1000)    19963 2023-07-29 12:50:24.000000 MetAromatic-1.4.0/README.md
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      567 2023-07-29 10:47:14.000000 MetAromatic-1.4.0/README_PYPI.md
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      651 2023-07-29 12:50:50.000000 MetAromatic-1.4.0/pyproject.toml
+-rw-r--r--   0 dsw       (1000) dsw       (1000)       38 2023-07-29 12:51:25.933780 MetAromatic-1.4.0/setup.cfg
+drwxr-xr-x   0 dsw       (1000) dsw       (1000)        0 2023-07-29 12:51:25.927796 MetAromatic-1.4.0/tests/
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     1817 2023-07-29 11:54:54.000000 MetAromatic-1.4.0/tests/test_api_bridge.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     1578 2023-07-29 11:54:54.000000 MetAromatic-1.4.0/tests/test_api_bridge_benchmark.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     4368 2023-07-29 12:50:24.000000 MetAromatic-1.4.0/tests/test_api_pair.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     2840 2023-07-29 12:50:24.000000 MetAromatic-1.4.0/tests/test_api_pair_benchmark.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      308 2023-07-19 06:46:26.000000 MetAromatic-1.4.0/tests/test_get_hexagon_midpoints.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     1152 2023-04-22 10:25:54.000000 MetAromatic-1.4.0/tests/test_lone_pair_interpolators.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      304 2023-04-22 10:25:54.000000 MetAromatic-1.4.0/tests/test_resolve_runner_from_path.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     4712 2023-04-24 08:25:14.000000 MetAromatic-1.4.0/tests/test_runner_batch.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     1959 2023-04-23 12:19:11.000000 MetAromatic-1.4.0/tests/test_runner_bridge.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     3906 2023-05-23 08:25:27.000000 MetAromatic-1.4.0/tests/test_runner_pair.py
```

### Comparing `MetAromatic-1.3.0/LICENSE` & `MetAromatic-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `MetAromatic-1.3.0/MetAromatic/batch.py` & `MetAromatic-1.4.0/MetAromatic/batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,17 +136,17 @@
                 self.log.debug('Received interrupt signal - stopping worker thread...')
                 break
 
             try:
                 fs = handle_ma.get_met_aromatic_interactions(code)
                 results = {
                     '_id': code,
-                    'ok': fs.OK,
-                    'status': fs.status,
-                    'results': fs.interactions
+                    'ok': fs['OK'],
+                    'status': fs['status'],
+                    'results': fs['interactions'],
                 }
             except Exception:
                 self.count += 1
                 self.log.exception('Could not process code: %s. Count: %i', code, self.count)
             else:
                 self.count += 1
                 self.log.info('Processed %s. Count: %i', code, self.count)
```

### Comparing `MetAromatic-1.3.0/MetAromatic/bridge.py` & `MetAromatic-1.4.0/MetAromatic/bridge.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,88 +1,83 @@
-from dataclasses import dataclass, field
 from logging import getLogger
 from networkx import Graph, connected_components
 from MetAromatic.pair import MetAromatic
-from MetAromatic.complex_types import TYPE_MA_PARAMS
-
-
-@dataclass
-class BridgeSpace:
-
-    interactions: set[tuple[str, str]] = field(default_factory=set)
-    bridges: list[set[str]] = field(default_factory=list)
-
-    OK: bool = True
-    status: str = 'Success'
+from MetAromatic.complex_types import TYPE_MA_PARAMS, TYPE_BRIDGE_SPACE
 
 
 class GetBridgingInteractions:
 
     log = getLogger('met-aromatic')
 
     def __init__(self, ma_params: TYPE_MA_PARAMS) -> None:
 
         self.ma_params = ma_params
-        self.f: BridgeSpace
+        self.f: TYPE_BRIDGE_SPACE
 
     def get_interacting_pairs(self, code: str) -> bool:
 
         ma_results = MetAromatic(self.ma_params).get_met_aromatic_interactions(code)
 
-        if not ma_results.OK:
+        if not ma_results['OK']:
             self.log.error('Cannot get bridging interactions as Met-aromatic algorithm failed')
 
-            self.f.OK = False
-            self.f.status = ma_results.status
+            self.f['OK'] = False
+            self.f['status'] = ma_results['status']
             return False
 
-        if len(ma_results.interactions) < 1:
+        if len(ma_results['interactions']) < 1:
             self.log.info('No Met-aromatic interactions were found therefore cannot find bridges')
 
-            self.f.status = 'No Met-aromatic interactions were found'
+            self.f['status'] = 'No Met-aromatic interactions were found'
             return False
 
-        for interaction in ma_results.interactions:
+        for interaction in ma_results['interactions']:
             pair = (
                 f"{interaction['aromatic_residue']}{interaction['aromatic_position']}",
                 f"MET{interaction['methionine_position']}"
             )
-            self.f.interactions.add(pair)
+            self.f['interactions'].add(pair)
 
         return True
 
     def isolate_connected_components(self, vertices: int) -> None:
 
         graph = Graph()
-        graph.add_edges_from(self.f.interactions)
+        graph.add_edges_from(self.f['interactions'])
 
         for bridge in connected_components(graph):
             if len(bridge) == vertices:
-                self.f.bridges.append(bridge)
+                self.f['bridges'].append(bridge)
 
         # Note that inverse bridges (MET-ARO-MET) not removed!
 
-        num_bridges = len(self.f.bridges)
+        num_bridges = len(self.f['bridges'])
 
         if num_bridges > 0:
 
             if num_bridges == 1:
                 self.log.info('Found 1 bridge')
             else:
                 self.log.info('Found %i bridges', num_bridges)
 
             return
 
         self.log.info('Found no bridges')
-        self.f.status = 'No bridges'
+        self.f['status'] = 'No bridges'
 
-    def get_bridging_interactions(self, code: str, vertices: int) -> BridgeSpace:
+    def get_bridging_interactions(self, code: str, vertices: int) -> TYPE_BRIDGE_SPACE:
 
         self.log.info('Locating bridging interactions for entry "%s"', code)
 
-        self.f = BridgeSpace()
+        self.f = {
+            'interactions': set(),
+            'bridges': [],
+            'OK': True,
+            'status': 'Success'
+        }
 
         if not self.get_interacting_pairs(code):
             return self.f
 
         self.isolate_connected_components(vertices=vertices)
+
         return self.f
```

### Comparing `MetAromatic-1.3.0/MetAromatic/complex_types.py` & `MetAromatic-1.4.0/MetAromatic/complex_types.py`

 * *Files 26% similar despite different names*

```diff
@@ -44,7 +44,40 @@
         'aromatic_residue': str,
         'met_phi_angle': float,
         'met_theta_angle': float,
         'methionine_position': int,
         'norm': float
     }
 )
+
+TYPE_FEATURE_SPACE = TypedDict(
+    'TYPE_FEATURE_SPACE',
+    {
+        'cutoff_dist': float,
+        'cutoff_angle': float,
+        'chain': str,
+        'model': str,
+        'raw_data': list[str],
+        'first_model': list[str],
+        'coords_met': list[list[str]],
+        'coords_phe': list[list[str]],
+        'coords_tyr': list[list[str]],
+        'coords_trp': list[list[str]],
+        'lone_pairs_met': list[TYPE_LONE_PAIRS_MET],
+        'midpoints_phe': list[TYPE_MIDPOINTS],
+        'midpoints_tyr': list[TYPE_MIDPOINTS],
+        'midpoints_trp': list[TYPE_MIDPOINTS],
+        'interactions': list[TYPE_INTERACTIONS],
+        'OK': bool,
+        'status': str,
+    }
+)
+
+TYPE_BRIDGE_SPACE = TypedDict(
+    'TYPE_BRIDGE_SPACE',
+    {
+        'interactions': set[tuple[str, str]],
+        'bridges': list[set[str]],
+        'OK': bool,
+        'status': str,
+    }
+)
```

### Comparing `MetAromatic-1.3.0/MetAromatic/get_aromatic_midpoints.py` & `MetAromatic-1.4.0/MetAromatic/get_aromatic_midpoints.py`

 * *Files identical despite different names*

### Comparing `MetAromatic-1.3.0/MetAromatic/lone_pair_interpolators.py` & `MetAromatic-1.4.0/MetAromatic/lone_pair_interpolators.py`

 * *Files identical despite different names*

### Comparing `MetAromatic-1.3.0/MetAromatic/pair.py` & `MetAromatic-1.4.0/MetAromatic/pair.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from abc import ABC, abstractmethod
-from dataclasses import dataclass, field
 from gzip import open as gz_open
 from itertools import groupby
 from logging import getLogger
 from operator import itemgetter
 from os import path
 from re import match, compile
 from tempfile import gettempdir, NamedTemporaryFile
 from urllib.error import URLError
 from urllib.request import urlretrieve, urlcleanup
 
 from numpy import ndarray, array, dot, linalg, degrees, arccos
-from MetAromatic import complex_types
+from MetAromatic.complex_types import TYPE_MA_PARAMS, TYPE_FEATURE_SPACE
 from MetAromatic.get_aromatic_midpoints import get_phe_midpoints
 from MetAromatic.get_aromatic_midpoints import get_trp_midpoints
 from MetAromatic.get_aromatic_midpoints import get_tyr_midpoints
 from MetAromatic.lone_pair_interpolators import CrossProductMethod
 from MetAromatic.lone_pair_interpolators import RodriguesMethod
 
 TMPDIR = gettempdir()
@@ -24,92 +23,65 @@
 
     dot_prod = dot(u, v)
     prod_mag = linalg.norm(v) * linalg.norm(u)
 
     return degrees(arccos(dot_prod / prod_mag))
 
 
-@dataclass
-class FeatureSpace:
-
-    cutoff_dist: float = 4.9
-    cutoff_angle: float = 109.5
-    chain: str = 'A'
-    model: str = 'cp'
-
-    raw_data: list[str] = field(default_factory=list)
-    first_model: list[str] = field(default_factory=list)
-
-    coords_met: list[list[str]] = field(default_factory=list)
-    coords_phe: list[list[str]] = field(default_factory=list)
-    coords_tyr: list[list[str]] = field(default_factory=list)
-    coords_trp: list[list[str]] = field(default_factory=list)
-
-    lone_pairs_met: list[complex_types.TYPE_LONE_PAIRS_MET] = field(default_factory=list)
-    midpoints_phe: list[complex_types.TYPE_MIDPOINTS] = field(default_factory=list)
-    midpoints_tyr: list[complex_types.TYPE_MIDPOINTS] = field(default_factory=list)
-    midpoints_trp: list[complex_types.TYPE_MIDPOINTS] = field(default_factory=list)
-
-    interactions: list[complex_types.TYPE_INTERACTIONS] = field(default_factory=list)
-
-    OK: bool = True
-    status: str = 'Success'
-
-
 class MetAromaticBase(ABC):
 
     log = getLogger('met-aromatic')
 
-    def __init__(self, ma_params: complex_types.TYPE_MA_PARAMS) -> None:
+    def __init__(self, ma_params: TYPE_MA_PARAMS) -> None:
 
         self.cutoff_distance = ma_params['cutoff_distance']
         self.cutoff_angle = ma_params['cutoff_angle']
         self.chain = ma_params['chain']
         self.model = ma_params['model']
 
         self.was_input_validated = False
-        self.f: FeatureSpace
+        self.f: TYPE_FEATURE_SPACE
 
     def is_input_valid(self) -> bool:
 
         self.log.debug('Validating input parameters')
 
         if not isinstance(self.cutoff_distance, float):
-            self.f.OK = False
-            self.f.status = 'Cutoff distance must be a valid float'
+            self.f['OK'] = False
+            self.f['status'] = 'Cutoff distance must be a valid float'
             return False
 
         if not isinstance(self.cutoff_angle, float):
-            self.f.OK = False
-            self.f.status = 'Cutoff angle must be a valid float'
+            self.f['OK'] = False
+            self.f['status'] = 'Cutoff angle must be a valid float'
             return False
 
         if not isinstance(self.chain, str):
-            self.f.OK = False
-            self.f.status = 'Chain must be a valid string'
+            self.f['OK'] = False
+            self.f['status'] = 'Chain must be a valid string'
             return False
 
         if not isinstance(self.model, str):
-            self.f.OK = False
-            self.f.status = 'Model must be a valid string'
+            self.f['OK'] = False
+            self.f['status'] = 'Model must be a valid string'
             return False
 
         if self.cutoff_distance < 0:
-            self.f.OK = False
-            self.f.status = 'Invalid cutoff distance'
+            self.f['OK'] = False
+            self.f['status'] = 'Invalid cutoff distance'
             return False
 
         if (self.cutoff_angle < 0) or (self.cutoff_angle > 360):
-            self.f.OK = False
-            self.f.status = 'Invalid cutoff angle'
+            self.f['OK'] = False
+            self.f['status'] = 'Invalid cutoff angle'
             return False
 
         if self.model not in ('cp', 'rm'):
-            self.f.OK = False
-            self.f.status = 'Invalid model'
+            self.f['OK'] = False
+            self.f['status'] = 'Invalid model'
             return False
 
         return True
 
     @abstractmethod
     def load_pdb_file(self, source: str) -> bool:
         # Source can be either:
@@ -117,172 +89,185 @@
         # 2. Path to a local PDB file
         pass
 
     def get_first_model(self) -> None:
 
         self.log.debug('Stripping feature space down to only first model')
 
-        for line in self.f.raw_data:
+        for line in self.f['raw_data']:
             if 'ENDMDL' in line:
                 break
 
-            self.f.first_model.append(line)
+            self.f['first_model'].append(line)
 
     def get_met_coordinates(self) -> bool:
 
         self.log.debug('Isolating MET coordinates from feature space')
 
         pattern = compile(rf'(ATOM.*(CE|SD|CG)\s+MET\s+{self.chain}\s)')
 
-        for line in self.f.first_model:
+        for line in self.f['first_model']:
             if match(pattern, line):
-                self.f.coords_met.append(line.split()[:9])
+                self.f['coords_met'].append(line.split()[:9])
 
-        if len(self.f.coords_met) == 0:
+        if len(self.f['coords_met']) == 0:
             self.log.error('No methionine residues found for entry')
 
-            self.f.status = "No MET residues"
-            self.f.OK = False
+            self.f['status'] = "No MET residues"
+            self.f['OK'] = False
             return False
 
         return True
 
     def get_phe_coordinates(self) -> None:
 
         self.log.debug('Isolating PHE coordinates from feature space')
 
         pattern = compile(rf'(ATOM.*(CD1|CE1|CZ|CG|CD2|CE2)\s+PHE\s+{self.chain}\s)')
 
-        for line in self.f.first_model:
+        for line in self.f['first_model']:
             if match(pattern, line):
-                self.f.coords_phe.append(line.split()[:9])
+                self.f['coords_phe'].append(line.split()[:9])
 
     def get_tyr_coordinates(self) -> None:
 
         self.log.debug('Isolating TYR coordinates from feature space')
 
         pattern = compile(rf'(ATOM.*(CD1|CE1|CZ|CG|CD2|CE2)\s+TYR\s+{self.chain}\s)')
 
-        for line in self.f.first_model:
+        for line in self.f['first_model']:
             if match(pattern, line):
-                self.f.coords_tyr.append(line.split()[:9])
+                self.f['coords_tyr'].append(line.split()[:9])
 
     def get_trp_coordinates(self) -> None:
 
         self.log.debug('Isolating TRP coordinates from feature space')
 
         pattern = compile(rf'(ATOM.*(CD2|CE3|CZ2|CH2|CZ3|CE2)\s+TRP\s+{self.chain}\s)')
 
-        for line in self.f.first_model:
+        for line in self.f['first_model']:
             if match(pattern, line):
-                self.f.coords_trp.append(line.split()[:9])
+                self.f['coords_trp'].append(line.split()[:9])
 
     def check_if_not_coordinates(self) -> bool:
 
         self.log.debug('Ensuring that at least one aromatic residue exists in feature space')
 
-        if not any([self.f.coords_phe, self.f.coords_tyr, self.f.coords_trp]):
+        if not any([self.f['coords_phe'], self.f['coords_tyr'], self.f['coords_trp']]):
             self.log.error('No aromatic residues found for entry')
-            self.f.status = "No PHE/TYR/TRP residues"
-            self.f.OK = False
+            self.f['status'] = "No PHE/TYR/TRP residues"
+            self.f['OK'] = False
             return False
 
         return True
 
     def get_met_lone_pairs_cp(self) -> None:
 
-        for position, groups in groupby(self.f.coords_met, lambda entry: entry[5]):
+        for position, groups in groupby(self.f['coords_met'], lambda entry: entry[5]):
             ordered = sorted(list(groups), key=itemgetter(2))
 
             coords_ce = array(ordered[0][6:9]).astype(float)
             coords_cg = array(ordered[1][6:9]).astype(float)
             coords_sd = array(ordered[2][6:9]).astype(float)
 
             lp = CrossProductMethod(coords_cg, coords_sd, coords_ce)
 
-            self.f.lone_pairs_met.append({
+            self.f['lone_pairs_met'].append({
                 'vector_a': lp.get_vector_a(),
                 'vector_g': lp.get_vector_g(),
                 'coords_sd': coords_sd,
                 'position': position
             })
 
     def get_met_lone_pairs_rm(self) -> None:
 
-        for position, groups in groupby(self.f.coords_met, lambda entry: entry[5]):
+        for position, groups in groupby(self.f['coords_met'], lambda entry: entry[5]):
             ordered = sorted(list(groups), key=itemgetter(2))
 
             coords_ce = array(ordered[0][6:9]).astype(float)
             coords_cg = array(ordered[1][6:9]).astype(float)
             coords_sd = array(ordered[2][6:9]).astype(float)
 
             lp = RodriguesMethod(coords_cg, coords_sd, coords_ce)
 
-            self.f.lone_pairs_met.append({
+            self.f['lone_pairs_met'].append({
                 'vector_a': lp.get_vector_a(),
                 'vector_g': lp.get_vector_g(),
                 'coords_sd': coords_sd,
                 'position': position
             })
 
     def get_midpoints(self) -> None:
 
         self.log.debug('Computing midpoints between PHE aromatic carbon atoms')
-        self.f.midpoints_phe = get_phe_midpoints(self.f.coords_phe)
+        self.f['midpoints_phe'] = get_phe_midpoints(self.f['coords_phe'])
 
         self.log.debug('Computing midpoints between TYR aromatic carbon atoms')
-        self.f.midpoints_tyr = get_tyr_midpoints(self.f.coords_tyr)
+        self.f['midpoints_tyr'] = get_tyr_midpoints(self.f['coords_tyr'])
 
         self.log.debug('Computing midpoints between TRP aromatic carbon atoms')
-        self.f.midpoints_trp = get_trp_midpoints(self.f.coords_trp)
+        self.f['midpoints_trp'] = get_trp_midpoints(self.f['coords_trp'])
 
     def apply_met_aromatic_criteria(self) -> None:
 
         self.log.debug('Finding pairs meeting Met-aromatic algorithm criteria in feature space')
 
-        midpoints = self.f.midpoints_phe + self.f.midpoints_tyr + self.f.midpoints_trp
+        midpoints = self.f['midpoints_phe'] + self.f['midpoints_tyr'] + self.f['midpoints_trp']
 
-        for lone_pair in self.f.lone_pairs_met:
+        for lone_pair in self.f['lone_pairs_met']:
             for midpoint in midpoints:
 
                 v = midpoint[2] - lone_pair['coords_sd']
                 norm_v = linalg.norm(v)
 
                 if norm_v > self.cutoff_distance:
                     continue
 
                 met_theta_angle = vector_angle(v, lone_pair['vector_a'])
                 met_phi_angle = vector_angle(v, lone_pair['vector_g'])
 
                 if (met_theta_angle > self.cutoff_angle) and (met_phi_angle > self.cutoff_angle):
                     continue
 
-                self.f.interactions.append({
+                self.f['interactions'].append({
                     'aromatic_position': int(midpoint[0]),
                     'aromatic_residue': midpoint[1],
                     'met_phi_angle': round(met_phi_angle, 3),
                     'met_theta_angle': round(met_theta_angle, 3),
                     'methionine_position': int(lone_pair['position']),
                     # Variable norm_v is of type numpy.float64 and so round() returns a numpy.float64
                     # which causes mypy to complain. So cast norm_v to float
                     'norm': round(float(norm_v), 3),
                 })
 
-        if len(self.f.interactions) == 0:
+        if len(self.f['interactions']) == 0:
             self.log.info('Found no Met-aromatic interactions for entry')
-            self.f.status = "No interactions"
-
-    def get_met_aromatic_interactions(self, source: str) -> FeatureSpace:
+            self.f['status'] = "No interactions"
 
-        self.f = FeatureSpace()
+    def get_met_aromatic_interactions(self, source: str) -> TYPE_FEATURE_SPACE:
 
-        self.f.cutoff_dist = self.cutoff_distance
-        self.f.cutoff_angle = self.cutoff_angle
-        self.f.chain = self.chain
-        self.f.model = self.model
+        self.f = {
+            'cutoff_dist': self.cutoff_distance,
+            'cutoff_angle': self.cutoff_angle,
+            'chain': self.chain,
+            'model': self.model,
+            'raw_data': [],
+            'first_model': [],
+            'coords_met': [],
+            'coords_phe': [],
+            'coords_tyr': [],
+            'coords_trp': [],
+            'lone_pairs_met': [],
+            'midpoints_phe': [],
+            'midpoints_tyr': [],
+            'midpoints_trp': [],
+            'interactions': [],
+            'OK': True,
+            'status': 'Success',
+        }
 
         if not self.was_input_validated:
             if not self.is_input_valid():
                 return self.f
 
             self.was_input_validated = True
 
@@ -330,37 +315,37 @@
 
             try:
                 urlcleanup()
                 urlretrieve(ftp_url, f.name)
             except URLError:
                 self.log.error('Invalid PDB entry "%s"', code)
 
-                self.f.status = "Invalid PDB entry"
-                self.f.OK = False
+                self.f['status'] = "Invalid PDB entry"
+                self.f['OK'] = False
                 return False
 
             with gz_open(f.name, 'rt') as gz:
                 for line in gz:
-                    self.f.raw_data.append(line)
+                    self.f['raw_data'].append(line)
 
         return True
 
 
 class MetAromaticLocal(MetAromaticBase):
 
     def load_pdb_file(self, source: str) -> bool:
 
         self.log.debug('Reading file "%s"', source)
 
         if not path.exists(source):
             errmsg = f'File "{source}" does not exist'
             self.log.error(errmsg)
 
-            self.f.status = errmsg
-            self.f.OK = False
+            self.f['status'] = errmsg
+            self.f['OK'] = False
 
             return False
 
         for line in open(source):
-            self.f.raw_data.append(line)
+            self.f['raw_data'].append(line)
 
         return True
```

### Comparing `MetAromatic-1.3.0/MetAromatic/runner.py` & `MetAromatic-1.4.0/MetAromatic/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,45 +61,45 @@
     if read_local:
         from MetAromatic.pair import MetAromaticLocal
         results = MetAromaticLocal(obj).get_met_aromatic_interactions(source)
     else:
         from MetAromatic.pair import MetAromatic
         results = MetAromatic(obj).get_met_aromatic_interactions(source)
 
-    if not results.OK:
-        sys.exit(results.status)
+    if not results['OK']:
+        sys.exit(results['status'])
 
     click.echo(SEPARATOR)
 
     header_success = ['ARO', 'POS', 'MET POS', 'NORM', 'MET-THETA', 'MET-PHI']
     click.echo("{:<10} {:<10} {:<10} {:<10} {:<10} {:<10}".format(*header_success))
 
     click.echo(SEPARATOR)
 
-    for line in results.interactions:
+    for line in results['interactions']:
         click.echo("{:<10} {:<10} {:<10} {:<10} {:<10} {:<10}".format(*line.values()))
 
     click.echo(SEPARATOR)
 
 @cli.command(help='Run a bridging interaction query on a single PDB entry.') # type: ignore
 @click.argument('code')
 @click.option('--vertices', default=3, type=click.IntRange(min=3), metavar='<vertices>')
 @click.pass_obj
 def bridge(obj: TYPE_MA_PARAMS, code: str, vertices: int) -> None:
 
     from MetAromatic.bridge import GetBridgingInteractions
 
     results = GetBridgingInteractions(obj).get_bridging_interactions(vertices=vertices, code=code)
 
-    if not results.OK:
-        sys.exit(results.status)
+    if not results['OK']:
+        sys.exit(results['status'])
 
     click.echo(SEPARATOR)
 
-    for line in results.bridges:
+    for line in results['bridges']:
         click.echo('{' + '}-{'.join(line) + '}')
 
     click.echo(SEPARATOR)
 
 @cli.command(help='Run a Met-aromatic query batch job.') # type: ignore
 @click.argument('path_batch_file')
 @click.option('--threads', default=5, type=int, metavar='<number-threads>', help='Specify number of workers to use.')
```

### Comparing `MetAromatic-1.3.0/MetAromatic.egg-info/PKG-INFO` & `MetAromatic-1.4.0/MetAromatic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MetAromatic
-Version: 1.3.0
+Version: 1.4.0
 Summary: MetAromatic algorithm
 Author: David Weber
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `MetAromatic-1.3.0/MetAromatic.egg-info/SOURCES.txt` & `MetAromatic-1.4.0/MetAromatic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MetAromatic-1.3.0/PKG-INFO` & `MetAromatic-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MetAromatic
-Version: 1.3.0
+Version: 1.4.0
 Summary: MetAromatic algorithm
 Author: David Weber
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `MetAromatic-1.3.0/README.md` & `MetAromatic-1.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 * Weber, D. S.; Warren, J. J. The Interaction between Methionine and Two Aromatic Amino Acids Is an Abundant
   and Multifunctional Motif in Proteins. _Arch. Biochem. Biophys._ **2019**, _672_, 108053.
 * Weber, D. S.; Warren, J. J. A Survey of Methionine-Aromatic Interaction Geometries in the Oxidoreductase
   Class of Enzymes: What Could Met-Aromatic Interactions be Doing Near Metal Sites? _J. Inorg. Biochem._
 **2018**, _186_, 34-41.
 ## Table of Contents
 - [Synopsis](#synopsis)
+- [Setup](#setup)
 - [How it works](#how-it-works)
   - [Step 1: Data preprocessing](#step-1-data-preprocessing)
   - [Step 2: The distance condition](#step-2-the-distance-condition)
   - [Step 3: The angular condition](#step-3-the-angular-condition)
   - [Summary](#summary)
-- [Setup](#setup)
 - [Basic usage](#basic-usage)
   - [Finding Met-aromatic pairs](#finding-met-aromatic-pairs)
   - [Finding "bridging interactions"](#finding-bridging-interactions)
 - [Batch jobs and MongoDB integration](#batch-jobs-and-mongodb-integration)
   - [A brief overview](#a-brief-overview)
   - [Designing a distributed mining strategy](#designing-a-distributed-mining-strategy)
 - [Using the MetAromatic API](#using-the-metaromatic-api)
@@ -24,14 +24,21 @@
   - [Example: programmatically obtaining bridging interactions](#example-programmatically-obtaining-bridging-interactions)
 - [Tests and automation](#tests-and-automation)
 
 ## Synopsis
 This program returns a list of closely spaced methionine-aromatic residue pairs for structures in the [Protein
 Data Bank](https://www.rcsb.org/) (PDB). The program supports running queries on single PDB entries or large
 scale multithreaded batch jobs consisting of hundreds of thousands of queries.
+
+## Setup
+Simply run:
+```
+pip install MetAromatic
+```
+
 ## How it works
 ### Step 1: Data preprocessing
 Files in the PDB are organized using the SMCRA hierarchy: _Structure_, _Model_, _Chain_, _Residue_ and _Atom_.
 For example, here is the fifth line for the entry 1RCY:
 ```
 1         2  3   4   5   6     7         8      9       10   11              12
 ATOM      5  CB  THR A   5     -13.081   2.366  23.788  1.00 37.95           C
@@ -106,19 +113,14 @@
 pairs are pointing into or near the region of highest electron density on the corresponding aromatic residues.
 A representative figure is shown below:
 
 <p align="center">
   <img width="336" height="300" src=./pngs/pair-met18-tyr122.png>
 </p>
 
-## Setup
-Simply run:
-```
-pip install MetAromatic
-```
 ## Basic usage
 ### Finding Met-aromatic pairs
 The easiest means of performing Met-aromatic calculations is to run jobs in a terminal session. The simplest
 query follows:
 ```
 runner pair 1rcy
 ```
```

### Comparing `MetAromatic-1.3.0/README_PYPI.md` & `MetAromatic-1.4.0/README_PYPI.md`

 * *Files identical despite different names*

### Comparing `MetAromatic-1.3.0/pyproject.toml` & `MetAromatic-1.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "MetAromatic"
-version = "1.3.0"
+version = "1.4.0"
 authors = [{name="David Weber"}]
 description = "MetAromatic algorithm"
 readme = "README_PYPI.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `MetAromatic-1.3.0/tests/test_api_bridge.py` & `MetAromatic-1.4.0/tests/test_api_bridge.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,16 +24,16 @@
         'cutoff_distance': cutoff_distance,
         'model': model,
         'chain': 'A'
     }
 
     results = GetBridgingInteractions(params).get_bridging_interactions(code=code, vertices=4)
 
-    assert not results.OK
-    assert results.status == status
+    assert not results['OK']
+    assert results['status'] == status
 
 @mark.parametrize(
     'code, message',
     [
         ('1a5r', 'No Met-aromatic interactions were found'),
         ('1rcy', 'No bridges')
     ]
@@ -45,9 +45,9 @@
         'cutoff_angle': 109.5,
         'chain': 'A',
         'model': 'cp'
     }
 
     results = GetBridgingInteractions(params).get_bridging_interactions(code=code, vertices=4)
 
-    assert results.OK
-    assert results.status == message
+    assert results['OK']
+    assert results['status'] == message
```

### Comparing `MetAromatic-1.3.0/tests/test_api_bridge_benchmark.py` & `MetAromatic-1.4.0/tests/test_api_bridge_benchmark.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,8 +52,8 @@
             TEST_PARAMETERS
         ).get_bridging_interactions(
             vertices=NETWORK_SIZE, code=bridges.get('pdb_code')
         )
     except IndexError:
         skip('Skipping list index out of range error. Occurs because of missing data.')
     else:
-        assert set(bridges.get('bridge')) in results.bridges
+        assert set(bridges.get('bridge')) in results['bridges']
```

### Comparing `MetAromatic-1.3.0/tests/test_api_pair.py` & `MetAromatic-1.4.0/tests/test_api_pair.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,42 +50,42 @@
 ]
 
 def test_pair_1rcy_valid_results():
     results = MetAromatic(TEST_PARAMETERS).get_met_aromatic_interactions('1rcy')
 
     tc = TestCase()
     tc.maxDiff = None
-    tc.assertCountEqual(results.interactions, VALID_RESULTS_1RCY)
+    tc.assertCountEqual(results['interactions'], VALID_RESULTS_1RCY)
 
 def test_pair_1rcy_valid_results_use_local():
 
     # File downloaded from RSCB PDB
     path_pdb_file = Path(__file__).resolve().parent / 'data_1rcy.pdb'
 
     if not path_pdb_file.exists():
         exit(f'File {path_pdb_file} is missing')
 
     results = MetAromaticLocal(TEST_PARAMETERS).get_met_aromatic_interactions(path_pdb_file)
 
     tc = TestCase()
     tc.maxDiff = None
-    tc.assertCountEqual(results.interactions, VALID_RESULTS_1RCY)
+    tc.assertCountEqual(results['interactions'], VALID_RESULTS_1RCY)
 
 def test_pair_1rcy_valid_results_use_local_invalid_file():
 
     # Simulating someone passing a non-PDB formatted file into program
     path_pdb_file = Path(__file__).resolve().parent / 'data_lorem_ipsum.pdb'
 
     if not path_pdb_file.exists():
         exit(f'File {path_pdb_file} is missing')
 
     results = MetAromaticLocal(TEST_PARAMETERS).get_met_aromatic_interactions(path_pdb_file)
 
-    assert results.status != 'Success'
-    assert not results.OK
+    assert results['status'] != 'Success'
+    assert not results['OK']
 
 @mark.parametrize(
     'code, cutoff_distance, cutoff_angle, model, status',
     [
         ('1rcy', -0.01,  109.5,  'cp', 'Invalid cutoff distance'),
         ('1rcy',  4.95,  -60.0,  'cp', 'Invalid cutoff angle'),
         ('1rcy',  4.95,  720.0,  'cp', 'Invalid cutoff angle'),
@@ -105,15 +105,15 @@
         'cutoff_angle': cutoff_angle,
         'cutoff_distance': cutoff_distance,
         'chain': 'A',
         'model': model
     }
 
     results = MetAromatic(params).get_met_aromatic_interactions(code)
-    assert not results.OK
-    assert results.status == status
+    assert not results['OK']
+    assert results['status'] == status
 
 def test_pair_no_results_error():
     results = MetAromatic(TEST_PARAMETERS).get_met_aromatic_interactions('1a5r')
 
-    assert results.status == 'No interactions'
-    assert results.OK
+    assert results['status'] == 'No interactions'
+    assert results['OK']
```

### Comparing `MetAromatic-1.3.0/tests/test_api_pair_benchmark.py` & `MetAromatic-1.4.0/tests/test_api_pair_benchmark.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,14 @@
 
     except IndexError:
         skip('Skipping list index out of range error. Occurs because of missing data.')
 
     sum_norms_control = sum(float(i[6]) for i in control)
     sum_theta_control = sum(float(i[5]) for i in control)
     sum_phi_control = sum(float(i[4]) for i in control)
-    sum_norms_test = sum(float(i['norm']) for i in test_data.interactions)
-    sum_theta_test = sum(float(i['met_theta_angle']) for i in test_data.interactions)
-    sum_phi_test = sum(float(i['met_phi_angle']) for i in test_data.interactions)
+    sum_norms_test = sum(float(i['norm']) for i in test_data['interactions'])
+    sum_theta_test = sum(float(i['met_theta_angle']) for i in test_data['interactions'])
+    sum_phi_test = sum(float(i['met_phi_angle']) for i in test_data['interactions'])
 
     assert abs(sum_norms_control - sum_norms_test) < 0.01
     assert abs(sum_theta_control - sum_theta_test) < 0.01
     assert abs(sum_phi_control - sum_phi_test) < 0.01
```

### Comparing `MetAromatic-1.3.0/tests/test_lone_pair_interpolators.py` & `MetAromatic-1.4.0/tests/test_lone_pair_interpolators.py`

 * *Files identical despite different names*

### Comparing `MetAromatic-1.3.0/tests/test_runner_batch.py` & `MetAromatic-1.4.0/tests/test_runner_batch.py`

 * *Files identical despite different names*

### Comparing `MetAromatic-1.3.0/tests/test_runner_bridge.py` & `MetAromatic-1.4.0/tests/test_runner_bridge.py`

 * *Files identical despite different names*

### Comparing `MetAromatic-1.3.0/tests/test_runner_pair.py` & `MetAromatic-1.4.0/tests/test_runner_pair.py`

 * *Files identical despite different names*

