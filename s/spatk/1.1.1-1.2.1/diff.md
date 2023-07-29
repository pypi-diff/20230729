# Comparing `tmp/spatk-1.1.1.tar.gz` & `tmp/spatk-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatk-1.1.1.tar", last modified: Mon Jun  5 14:01:21 2023, max compression
+gzip compressed data, was "spatk-1.2.1.tar", last modified: Sat Jul 29 09:36:09 2023, max compression
```

## Comparing `spatk-1.1.1.tar` & `spatk-1.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 christoph  (1000) christoph  (1000)        0 2023-06-05 14:01:21.309777 spatk-1.1.1/
--rw-r--r--   0 christoph  (1000) christoph  (1000)    35149 2017-09-30 07:16:26.000000 spatk-1.1.1/LICENSE
--rw-r--r--   0 christoph  (1000) christoph  (1000)    41629 2023-06-05 14:01:21.309777 spatk-1.1.1/PKG-INFO
--rw-r--r--   0 christoph  (1000) christoph  (1000)      564 2023-05-19 11:37:54.000000 spatk-1.1.1/README.md
--rw-r--r--   0 christoph  (1000) christoph  (1000)      713 2023-06-05 14:00:25.000000 spatk-1.1.1/pyproject.toml
--rw-r--r--   0 christoph  (1000) christoph  (1000)       38 2023-06-05 14:01:21.309777 spatk-1.1.1/setup.cfg
-drwxr-xr-x   0 christoph  (1000) christoph  (1000)        0 2023-06-05 14:01:21.305777 spatk-1.1.1/spatk/
--rw-r--r--   0 christoph  (1000) christoph  (1000)      840 2023-05-19 09:26:30.000000 spatk-1.1.1/spatk/__init__.py
--rw-r--r--   0 christoph  (1000) christoph  (1000)     9645 2023-06-05 13:59:05.000000 spatk-1.1.1/spatk/circuit.py
--rw-r--r--   0 christoph  (1000) christoph  (1000)     2663 2023-06-05 13:59:05.000000 spatk-1.1.1/spatk/elements.py
--rw-r--r--   0 christoph  (1000) christoph  (1000)     6019 2023-05-19 10:23:26.000000 spatk-1.1.1/spatk/genelems.py
--rw-r--r--   0 christoph  (1000) christoph  (1000)    13866 2023-05-19 08:47:55.000000 spatk-1.1.1/spatk/helems.py
--rw-r--r--   0 christoph  (1000) christoph  (1000)     9667 2023-04-12 18:59:09.000000 spatk-1.1.1/spatk/helpers.py
--rw-r--r--   0 christoph  (1000) christoph  (1000)    15389 2023-06-05 13:59:05.000000 spatk-1.1.1/spatk/ngelems.py
-drwxr-xr-x   0 christoph  (1000) christoph  (1000)        0 2023-06-05 14:01:21.309777 spatk-1.1.1/spatk.egg-info/
--rw-r--r--   0 christoph  (1000) christoph  (1000)    41629 2023-06-05 14:01:21.000000 spatk-1.1.1/spatk.egg-info/PKG-INFO
--rw-r--r--   0 christoph  (1000) christoph  (1000)      317 2023-06-05 14:01:21.000000 spatk-1.1.1/spatk.egg-info/SOURCES.txt
--rw-r--r--   0 christoph  (1000) christoph  (1000)        1 2023-06-05 14:01:21.000000 spatk-1.1.1/spatk.egg-info/dependency_links.txt
--rw-r--r--   0 christoph  (1000) christoph  (1000)       14 2023-06-05 14:01:21.000000 spatk-1.1.1/spatk.egg-info/requires.txt
--rw-r--r--   0 christoph  (1000) christoph  (1000)        6 2023-06-05 14:01:21.000000 spatk-1.1.1/spatk.egg-info/top_level.txt
-drwxr-xr-x   0 christoph  (1000) christoph  (1000)        0 2023-06-05 14:01:21.309777 spatk-1.1.1/tests/
--rw-r--r--   0 christoph  (1000) christoph  (1000)    24543 2023-06-05 13:59:05.000000 spatk-1.1.1/tests/test_spatk.py
+drwxr-xr-x   0 christoph  (1000) christoph  (1000)        0 2023-07-29 09:36:09.867458 spatk-1.2.1/
+-rw-r--r--   0 christoph  (1000) christoph  (1000)    35149 2023-02-15 18:58:01.000000 spatk-1.2.1/LICENSE
+-rw-r--r--   0 christoph  (1000) christoph  (1000)    41629 2023-07-29 09:36:09.867458 spatk-1.2.1/PKG-INFO
+-rw-r--r--   0 christoph  (1000) christoph  (1000)      564 2023-07-29 08:57:09.000000 spatk-1.2.1/README.md
+-rw-r--r--   0 christoph  (1000) christoph  (1000)      713 2023-07-29 09:31:55.000000 spatk-1.2.1/pyproject.toml
+-rw-r--r--   0 christoph  (1000) christoph  (1000)       38 2023-07-29 09:36:09.867458 spatk-1.2.1/setup.cfg
+drwxr-xr-x   0 christoph  (1000) christoph  (1000)        0 2023-07-29 09:36:09.863458 spatk-1.2.1/spatk/
+-rw-r--r--   0 christoph  (1000) christoph  (1000)      840 2023-07-29 08:57:09.000000 spatk-1.2.1/spatk/__init__.py
+-rw-r--r--   0 christoph  (1000) christoph  (1000)     9645 2023-07-29 08:57:09.000000 spatk-1.2.1/spatk/circuit.py
+-rw-r--r--   0 christoph  (1000) christoph  (1000)     2666 2023-07-29 09:21:10.000000 spatk-1.2.1/spatk/elements.py
+-rw-r--r--   0 christoph  (1000) christoph  (1000)     6862 2023-07-29 09:28:36.000000 spatk-1.2.1/spatk/genelems.py
+-rw-r--r--   0 christoph  (1000) christoph  (1000)    13910 2023-07-29 09:19:57.000000 spatk-1.2.1/spatk/helems.py
+-rw-r--r--   0 christoph  (1000) christoph  (1000)     9667 2023-07-29 08:57:09.000000 spatk-1.2.1/spatk/helpers.py
+-rw-r--r--   0 christoph  (1000) christoph  (1000)    15433 2023-07-29 09:23:01.000000 spatk-1.2.1/spatk/ngelems.py
+drwxr-xr-x   0 christoph  (1000) christoph  (1000)        0 2023-07-29 09:36:09.863458 spatk-1.2.1/spatk.egg-info/
+-rw-r--r--   0 christoph  (1000) christoph  (1000)    41629 2023-07-29 09:36:09.000000 spatk-1.2.1/spatk.egg-info/PKG-INFO
+-rw-r--r--   0 christoph  (1000) christoph  (1000)      317 2023-07-29 09:36:09.000000 spatk-1.2.1/spatk.egg-info/SOURCES.txt
+-rw-r--r--   0 christoph  (1000) christoph  (1000)        1 2023-07-29 09:36:09.000000 spatk-1.2.1/spatk.egg-info/dependency_links.txt
+-rw-r--r--   0 christoph  (1000) christoph  (1000)       14 2023-07-29 09:36:09.000000 spatk-1.2.1/spatk.egg-info/requires.txt
+-rw-r--r--   0 christoph  (1000) christoph  (1000)        6 2023-07-29 09:36:09.000000 spatk-1.2.1/spatk.egg-info/top_level.txt
+drwxr-xr-x   0 christoph  (1000) christoph  (1000)        0 2023-07-29 09:36:09.863458 spatk-1.2.1/tests/
+-rw-r--r--   0 christoph  (1000) christoph  (1000)    25641 2023-07-29 09:30:40.000000 spatk-1.2.1/tests/test_spatk.py
```

### Comparing `spatk-1.1.1/LICENSE` & `spatk-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spatk-1.1.1/PKG-INFO` & `spatk-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatk
-Version: 1.1.1
+Version: 1.2.1
 Summary: Module for handling and analyzing spice netlists
 Author: Christoph Weiser
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `spatk-1.1.1/README.md` & `spatk-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `spatk-1.1.1/pyproject.toml` & `spatk-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spatk"
-version = "1.1.1"
+version = "1.2.1"
 description = "Module for handling and analyzing spice netlists"
 readme = "README.md"
 authors = [{ name = "Christoph Weiser"}]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Programming Language :: Python",
```

### Comparing `spatk-1.1.1/spatk/__init__.py` & `spatk-1.2.1/spatk/__init__.py`

 * *Files identical despite different names*

### Comparing `spatk-1.1.1/spatk/circuit.py` & `spatk-1.2.1/spatk/circuit.py`

 * *Files identical despite different names*

### Comparing `spatk-1.1.1/spatk/elements.py` & `spatk-1.2.1/spatk/elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,42 +15,42 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from spatk import SYNTAX
 
 from spatk.genelems import (Args, Default, Component,
                             Component_2T, Component_3T,
                             Component_4T, Statement,
-                            Comment)
+                            Comment, Subckt, SubcktDef)
 
 if SYNTAX == "ngspice":
 
     from spatk.ngelems import elementmap
     from spatk.ngelems import process_statement, identify_linetype
     from spatk.ngelems import (Model, Include, Library,
                                Option, Function, Temp, Param,
                                Global, Xspice, Behavioral_source,
                                Capacitor, Diode, Vcvs, Cccs,
                                Vccs, Ccvs, Isource, Jfet,
                                Inductor, Mosfet, Numerical_device_gss,
                                Lossy_transmission_line, Bjt,
                                Resistor, Vcsw, Lossless_transmission_line,
                                Uniformely_distributed_rc_line,
-                               Vsource, Icsw, Subckt,
+                               Vsource, Icsw,
                                Single_lossy_transmission_line, Mesfet)
 
 elif SYNTAX == "hspice":
     from spatk.helems import elementmap
     from spatk.helems import process_statement, identify_linetype
     from spatk.helems import (Model, Include, Library,
                                Option, Function, Param,
                                Global, Xspice, Behavioral_source,
                                Capacitor, Diode, Vcvs, Cccs,
                                Vccs, Ccvs, Isource, Jfet,
                                Inductor, Mosfet, Numerical_device_gss,
                                Lossy_transmission_line, Bjt,
                                Resistor, Vcsw, Lossless_transmission_line,
                                Uniformely_distributed_rc_line,
-                               Vsource, Icsw, Subckt,
+                               Vsource, Icsw,
                                Single_lossy_transmission_line, Mesfet)
 
 else:
     raise Exception("The choosen syntax format is not supported!")
```

### Comparing `spatk-1.1.1/spatk/helems.py` & `spatk-1.2.1/spatk/helems.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 from spatk.genelems import (Args, 
                             Default, 
                             Component, 
                             Component_2T, 
                             Component_3T, 
                             Component_4T, 
                             Statement, 
-                            Comment)
+                            Comment,
+                            Subckt,
+                            SubcktDef)
 
 #----------------------------------------------------------------------
 # NGSpice element classes
 #----------------------------------------------------------------------
 
 class Model(Statement):
     """ .model Statement. """
@@ -410,20 +412,14 @@
 
 class Icsw(Component_2T):
     """ W - Current Controlled Switch. """
     def __init__(self, *args):
         super(Icsw, self).__init__(*args)
 
 
-class Subckt(Component):
-    """ X - Subcircuit. """
-    def __init__(self, *args):
-        super(Subckt, self).__init__(*args)
-
-
 class Single_lossy_transmission_line(Component_4T):
     """ Y - Single Lossy Transmission Line. """
     def __init__(self, *args):
         super(Single_lossy_transmission_line, self).__init__(*args)
 
 
 class Mesfet(Component_3T):
@@ -448,14 +444,15 @@
               "model":      Model,
               "include":    Include,
               "library":    Library,
               "option":     Option,
               "function":   Function,
               "param":      Param,
               "global":     Global,
+              "subckt":     SubcktDef,
               "A":          Xspice,
               "B":          Behavioral_source,
               "C":          Capacitor,
               "D":          Diode,
               "E":          Vcvs,
               "F":          Cccs,
               "G":          Vccs,
@@ -509,14 +506,16 @@
         return "option"
     elif identifier in [".func", ".function"]:
         return "function"
     elif identifier in [".global"]:
         return "global"
     elif identifier in [".par", ".param"]:
         return "param"
+    elif identifier in [".subckt"]:
+        return "subckt"
     else:
         return "."
 
 
 def identify_linetype(line):
     """ Identify the type of line.
```

### Comparing `spatk-1.1.1/spatk/helpers.py` & `spatk-1.2.1/spatk/helpers.py`

 * *Files identical despite different names*

### Comparing `spatk-1.1.1/spatk/ngelems.py` & `spatk-1.2.1/spatk/ngelems.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,17 @@
                             Default, 
                             Component, 
                             Component_2T, 
                             Component_3T, 
                             Component_4T, 
                             Statement, 
                             Comment,
-                            Model)
+                            Model,
+                            Subckt,
+                            SubcktDef)
 
 #----------------------------------------------------------------------
 # NGSpice element classes
 #----------------------------------------------------------------------
 
 
 class Include(Statement):
@@ -453,20 +455,14 @@
 
 class Icsw(Component_2T):
     """ W - Current Controlled Switch. """
     def __init__(self, *args):
         super(Icsw, self).__init__(*args)
 
 
-class Subckt(Component):
-    """ X - Subcircuit. """
-    def __init__(self, *args):
-        super(Subckt, self).__init__(*args)
-
-
 class Single_lossy_transmission_line(Component_4T):
     """ Y - Single Lossy Transmission Line. """
     def __init__(self, *args):
         super(Single_lossy_transmission_line, self).__init__(*args)
 
 
 class Mesfet(Component_3T):
@@ -492,14 +488,15 @@
               "include":    Include,
               "library":    Library,
               "option":     Option,
               "function":   Function,
               "temp":       Temp,
               "param":      Param,
               "global":     Global,
+              "subckt":     SubcktDef,
               "A":          Xspice,
               "B":          Behavioral_source,
               "C":          Capacitor,
               "D":          Diode,
               "E":          Vcvs,
               "F":          Cccs,
               "G":          Vccs,
@@ -555,14 +552,16 @@
         return "function"
     elif identifier in [".global"]:
         return "global"
     elif identifier in [".temp"]:
         return "temp"
     elif identifier in [".par", ".param"]:
         return "param"
+    elif identifier in [".subckt"]:
+        return "subckt"
     else:
         return "."
 
 
 def identify_linetype(line):
     """ Identify the type of line.
```

### Comparing `spatk-1.1.1/spatk.egg-info/PKG-INFO` & `spatk-1.2.1/spatk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatk
-Version: 1.1.1
+Version: 1.2.1
 Summary: Module for handling and analyzing spice netlists
 Author: Christoph Weiser
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `spatk-1.1.1/tests/test_spatk.py` & `spatk-1.2.1/tests/test_spatk.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,14 +214,40 @@
     "uid"       : "testuid",
     "mod"       : spe.Global,
     "instance"  : None,
     "type"      : "global",
     "value"     : None,
     "ports"     : dict(),
 },
+"subckt":
+{
+    "line"        : "X1 neta netb netc mysubckt",
+    "loc"         : "root",
+    "lib"         : None,
+    "n"           : 1,
+    "uid"         : "testuid",
+    "mod"         : spe.Subckt,
+    "instance"    : "X1",
+    "type"        : "subckt",
+    "value"       : "mysubckt",
+    "ports"       : dict(),
+},
+"subcktdef":
+{
+    "line"        : ".subckt mysubckt neta netb ",
+    "loc"         : "root",
+    "lib"         : None,
+    "n"           : 1,
+    "uid"         : "testuid",
+    "mod"         : spe.SubcktDef,
+    "instance"    : None,
+    "type"        : "subcktdef",
+    "value"       : "mysubckt",
+    "ports"       : dict(),
+},
 "capacitor":
 {
     "line"        : "C1 neta netb 10e-12",
     "loc"         : "root",
     "lib"         : None,
     "n"           : 1,
     "uid"         : "testuid",
@@ -875,15 +901,31 @@
 
 
 def test_module_icsw():
     pass
 
 
 def test_module_subckt():
-    pass
+    """ Test subckt module specific properties """
+    case = CASES["subckt"]
+    mod = create_module(case)
+
+    assert(mod.name == "mysubckt")
+    mod.name = "testsubckt"
+    assert(mod.name == "testsubckt")
+
+
+def test_module_subcktdef():
+    """ Test subcktdef module specific properties """
+    case = CASES["subcktdef"]
+    mod = create_module(case)
+
+    assert(mod.name == "mysubckt")
+    mod.name = "testsubckt"
+    assert(mod.name == "testsubckt")
 
 
 def test_module_single_lossy_transmission_line():
     pass
```

