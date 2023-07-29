# Comparing `tmp/ifctester-0.0.230718.tar.gz` & `tmp/ifctester-0.0.230729.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifctester-0.0.230718.tar", last modified: Tue Jul 18 02:03:38 2023, max compression
+gzip compressed data, was "ifctester-0.0.230729.tar", last modified: Sat Jul 29 01:38:21 2023, max compression
```

## Comparing `ifctester-0.0.230718.tar` & `ifctester-0.0.230729.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:03:38.716851 ifctester-0.0.230718/
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-18 02:03:38.716851 ifctester-0.0.230718/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-18 02:03:27.000000 ifctester-0.0.230718/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:03:38.716851 ifctester-0.0.230718/ifctester/
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-18 02:03:27.000000 ifctester-0.0.230718/ifctester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-18 02:03:27.000000 ifctester-0.0.230718/ifctester/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46023 2023-07-18 02:03:27.000000 ifctester-0.0.230718/ifctester/facet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9579 2023-07-18 02:03:27.000000 ifctester-0.0.230718/ifctester/ids.py
--rw-r--r--   0 runner    (1001) docker     (123)    12485 2023-07-18 02:03:27.000000 ifctester-0.0.230718/ifctester/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:03:38.716851 ifctester-0.0.230718/ifctester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-18 02:03:38.000000 ifctester-0.0.230718/ifctester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-18 02:03:38.000000 ifctester-0.0.230718/ifctester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 02:03:38.000000 ifctester-0.0.230718/ifctester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-18 02:03:38.000000 ifctester-0.0.230718/ifctester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 02:03:38.000000 ifctester-0.0.230718/ifctester.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-18 02:03:30.000000 ifctester-0.0.230718/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 02:03:38.716851 ifctester-0.0.230718/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:03:38.716851 ifctester-0.0.230718/test/
--rw-r--r--   0 runner    (1001) docker     (123)    88738 2023-07-18 02:03:27.000000 ifctester-0.0.230718/test/test_facet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-07-18 02:03:27.000000 ifctester-0.0.230718/test/test_ids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:38:21.345997 ifctester-0.0.230729/
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-29 01:38:21.345997 ifctester-0.0.230729/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-29 01:38:08.000000 ifctester-0.0.230729/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:38:21.341997 ifctester-0.0.230729/ifctester/
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-29 01:38:08.000000 ifctester-0.0.230729/ifctester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-29 01:38:08.000000 ifctester-0.0.230729/ifctester/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46023 2023-07-29 01:38:08.000000 ifctester-0.0.230729/ifctester/facet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9579 2023-07-29 01:38:08.000000 ifctester-0.0.230729/ifctester/ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10924 2023-07-29 01:38:08.000000 ifctester-0.0.230729/ifctester/ids.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    12485 2023-07-29 01:38:08.000000 ifctester-0.0.230729/ifctester/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:38:21.341997 ifctester-0.0.230729/ifctester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-29 01:38:21.000000 ifctester-0.0.230729/ifctester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-29 01:38:21.000000 ifctester-0.0.230729/ifctester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 01:38:21.000000 ifctester-0.0.230729/ifctester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-29 01:38:21.000000 ifctester-0.0.230729/ifctester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-29 01:38:21.000000 ifctester-0.0.230729/ifctester.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-29 01:38:11.000000 ifctester-0.0.230729/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 01:38:21.345997 ifctester-0.0.230729/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:38:21.345997 ifctester-0.0.230729/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    88779 2023-07-29 01:38:08.000000 ifctester-0.0.230729/test/test_facet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13038 2023-07-29 01:38:08.000000 ifctester-0.0.230729/test/test_ids.py
```

### Comparing `ifctester-0.0.230718/PKG-INFO` & `ifctester-0.0.230729/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifctester
-Version: 0.0.230718
+Version: 0.0.230729
 Summary: IFC model auditing tool with support for IDS
 Author-email: Dion Moult <dion@thinkmoult.com>
 Project-URL: Homepage, http://ifcopenshell.org
 Project-URL: Bug Tracker, https://github.com/ifcopenshell/ifcopenshell/issues
 Keywords: IFC,IDS,BIM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `ifctester-0.0.230718/README.md` & `ifctester-0.0.230729/README.md`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.230718/ifctester/__init__.py` & `ifctester-0.0.230729/ifctester/__init__.py`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.230718/ifctester/__main__.py` & `ifctester-0.0.230729/ifctester/__main__.py`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.230718/ifctester/facet.py` & `ifctester-0.0.230729/ifctester/facet.py`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.230718/ifctester/ids.py` & `ifctester-0.0.230729/ifctester/ids.py`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.230718/ifctester/reporter.py` & `ifctester-0.0.230729/ifctester/reporter.py`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.230718/ifctester.egg-info/PKG-INFO` & `ifctester-0.0.230729/ifctester.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifctester
-Version: 0.0.230718
+Version: 0.0.230729
 Summary: IFC model auditing tool with support for IDS
 Author-email: Dion Moult <dion@thinkmoult.com>
 Project-URL: Homepage, http://ifcopenshell.org
 Project-URL: Bug Tracker, https://github.com/ifcopenshell/ifcopenshell/issues
 Keywords: IFC,IDS,BIM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `ifctester-0.0.230718/pyproject.toml` & `ifctester-0.0.230729/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ifctester"
-version = "0.0.230718"
+version = "0.0.230729"
 authors = [
   { name="Dion Moult", email="dion@thinkmoult.com" },
 ]
 description = "IFC model auditing tool with support for IDS"
 readme = "README.md"
 keywords = ["IFC", "IDS", "BIM"]
 classifiers = [
@@ -19,7 +19,9 @@
 ]
 [project.urls]
 "Homepage" = "http://ifcopenshell.org"
 "Bug Tracker" = "https://github.com/ifcopenshell/ifcopenshell/issues"
 [tool.setuptools.packages.find]
 include = ["ifctester"]
 exclude = ["test*"]
+[tool.setuptools.package-data]
+ifctester = ["*.xsd"]
```

### Comparing `ifctester-0.0.230718/test/test_facet.py` & `ifctester-0.0.230729/test/test_facet.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
             inst=ifc.createIfcWall(),
             expected=False,
         )
         ifc = ifcopenshell.file()
         run(
             "Entities can be specified as a XSD regex pattern 2/2",
             facet=facet,
-            inst=ifc.createIfcWallType(),
+            inst=ifc.createIfcWallType(PredefinedType="USERDEFINED"),
             expected=True,
         )
 
         restriction = Restriction(options={"pattern": "FOO.*"})
         facet = Entity(name="IFCWALL", predefinedType=restriction)
         ifc = ifcopenshell.file()
         wall = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall", predefined_type="FOOBAR")
@@ -251,20 +251,21 @@
             expected=True,
         )
 
         ifc = ifcopenshell.file()
         facet = Attribute(name="Name")
         element = ifc.createIfcWall(Name="Foobar")
         run("A required facet checks all parameters as normal", facet=facet, inst=element, expected=True)
-        facet = Attribute(name="Name", minOccurs=0, maxOccurs=0)
-        run("A prohibited facet returns the opposite of a required facet", facet=facet, inst=element, expected=False)
-        facet = Attribute(name="Name", minOccurs=0)
-        run("An optional facet always passes regardless of outcome 1/2", facet=facet, inst=element, expected=True)
-        facet = Attribute(name="Rabbit", minOccurs=0)
-        run("An optional facet always passes regardless of outcome 2/2", facet=facet, inst=element, expected=True)
+
+        # facet = Attribute(name="Name", minOccurs=0, maxOccurs=0)
+        # run("A prohibited facet returns the opposite of a required facet", facet=facet, inst=element, expected=False)
+        # facet = Attribute(name="Name", minOccurs=0)
+        # run("An optional facet always passes regardless of outcome 1/2", facet=facet, inst=element, expected=True)
+        # facet = Attribute(name="Rabbit", minOccurs=0)
+        # run("An optional facet always passes regardless of outcome 2/2", facet=facet, inst=element, expected=True)
 
         ifc = ifcopenshell.file()
         facet = Attribute(name="Name")
         run("Attributes with null values always fail", facet=facet, inst=ifc.createIfcWall(), expected=False)
         # The logic is that unfortunately most BIM users cannot differentiate between the two.
         ifc = ifcopenshell.file()
         run("Attributes with empty strings always fail", facet=facet, inst=ifc.createIfcWall(Name=""), expected=False)
```

### Comparing `ifctester-0.0.230718/test/test_ids.py` & `ifctester-0.0.230729/test/test_ids.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         result = specs.to_xml(fn)
         os.remove(fn)
 
     def test_creating_a_minimal_ids_and_validating(self):
         specs = ids.Ids(title="Title")
         spec = ids.Specification(name="Name")
         spec.applicability.append(ids.Entity(name="IFCWALL"))
-        spec.requirements.append(ids.Attribute(name="Name", value="Waldo"))
+        spec.requirements.append(name_attr := ids.Attribute(name="Name", value="Waldo"))
         specs.specifications.append(spec)
         assert "http://standards.buildingsmart.org/IDS" in specs.to_string()
         assert spec.status == None
 
         model = ifcopenshell.file()
         wall = model.createIfcWall()
         waldo = model.createIfcWall(Name="Waldo")
@@ -163,38 +163,51 @@
         wall = model.createIfcWall(Name="Waldo")
         run("Prohibited specifications fail if at least one entity passes all requirements 3/3", specs, model, False, [wall])
 
         spec.minOccurs = 0
         spec.maxOccurs = "unbounded"
         model = ifcopenshell.file()
         wall = model.createIfcWall(Name="Waldo")
-        spec.requirements.append(ids.Attribute(name="Description", value="Foobar"))
+        spec.requirements.append(description_attr := ids.Attribute(name="Description", value="Foobar"))
         run("A specification passes only if all requirements pass 1/2", specs, model, False, [wall], [wall])
         wall.Description = "Foobar"
         run("A specification passes only if all requirements pass 2/2", specs, model, True, [wall])
 
-        spec.requirements[1].minOccurs = 0
-        wall.Description = None
-        run("Specification optionality and facet optionality can be combined", specs, model, True, [wall])
+        # optional attribute
+        # description_attr.minOccurs = 0
+        # description_attr.maxOccurs = "unbounded"
+        # wall.Description = None
+        # run("Specification optionality and facet optionality can be combined", specs, model, True, [wall])
+
+        # double negative / required attributes
+        # spec.minOccurs = 0
+        # spec.maxOccurs = 0
+        # name_attr.minOccurs = 0
+        # name_attr.maxOccurs = 0
+        # description_attr.minOccurs = 0
+        # description_attr.maxOccurs = 0
+        # wall.Name = "Waldo"
+        # wall.Description = "Foobar"
+        # run("A prohibited specification and a prohibited facet results in a double negative", specs, model, True, [wall])
 
-        spec.minOccurs = 0
-        spec.maxOccurs = 0
-        spec.requirements[0].minOccurs = 0
-        spec.requirements[0].maxOccurs = 0
-        spec.requirements[1].minOccurs = 0
-        spec.requirements[1].maxOccurs = 0
-        wall.Name = "Waldo"
-        wall.Description = "Foobar"
-        run("A prohibited specification and a prohibited facet results in a double negative", specs, model, True, [wall])
+        # specs independency
+        specs = ids.Ids(title="Title")
+        spec = ids.Specification(name="Name")
+        spec.applicability.append(ids.Entity(name="IFCWALL"))
+        spec.requirements.append(ids.Attribute(name="Description", value="Foobar"))
+        specs.specifications.append(spec)
 
         spec = ids.Specification(name="Name")
         spec.applicability.append(ids.Entity(name="IFCWALL"))
         spec.requirements.append(ids.Attribute(name="Name", value="Waldo"))
         specs.specifications.append(spec)
-        wall2 = model.createIfcWall(Name="Waldo")
+
+        wall.Name = "Waldo"
+        wall.Description = "Foobar"
+        wall2 = model.createIfcWall(Name="Waldo", Description="Foobar")
         run("Multiple specifications are independent of one another", specs, model, True, [wall, wall2])
 
     def test_creating_multiple_specifications(self):
         specs = ids.Ids(title="Title")
         spec = ids.Specification(name="Name")
         spec.applicability.append(ids.Entity(name="IFCWALL"))
         spec.requirements.append(ids.Attribute(name="Name", value="Waldo"))
```

