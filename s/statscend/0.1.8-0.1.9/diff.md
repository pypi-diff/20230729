# Comparing `tmp/statscend-0.1.8.tar.gz` & `tmp/statscend-0.1.9.tar.gz`

## Comparing `statscend-0.1.8.tar` & `statscend-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 statscend-0.1.8/.DS_Store
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 statscend-0.1.8/statscend/__init__.py
--rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 statscend-0.1.8/statscend/bn_logistic_regression.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 statscend-0.1.8/statscend/datasets.py
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 statscend-0.1.8/statscend/linear_regression.py
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 statscend-0.1.8/statscend/mn_logistic_regression.py
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 statscend-0.1.8/statscend/ordinal_regression.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 statscend-0.1.8/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 statscend-0.1.8/LICENSE
--rw-r--r--   0        0        0    13432 2020-02-02 00:00:00.000000 statscend-0.1.8/README.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 statscend-0.1.8/pyproject.toml
--rw-r--r--   0        0        0    15358 2020-02-02 00:00:00.000000 statscend-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 statscend-0.1.9/.DS_Store
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 statscend-0.1.9/.vscode/settings.json
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 statscend-0.1.9/statscend/__init__.py
+-rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 statscend-0.1.9/statscend/bn_logistic_regression.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 statscend-0.1.9/statscend/datasets.py
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 statscend-0.1.9/statscend/linear_regression.py
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 statscend-0.1.9/statscend/mn_logistic_regression.py
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 statscend-0.1.9/statscend/ordinal_regression.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 statscend-0.1.9/statscend/vif.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 statscend-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 statscend-0.1.9/LICENSE
+-rw-r--r--   0        0        0    13432 2020-02-02 00:00:00.000000 statscend-0.1.9/README.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 statscend-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    15358 2020-02-02 00:00:00.000000 statscend-0.1.9/PKG-INFO
```

### Comparing `statscend-0.1.8/.DS_Store` & `statscend-0.1.9/.DS_Store`

 * *Files 9% similar despite different names*

```diff
@@ -84,16 +84,16 @@
 00000530: 0203 0405 0607 0809 0909 090d 095d 5368  .............]Sh
 00000540: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
 00000550: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
 00000560: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
 00000570: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
 00000580: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
 00000590: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-000005a0: 0909 0909 5f10 187b 7b31 3537 2c20 3230  ...._..{{157, 20
-000005b0: 307d 2c20 7b37 3730 2c20 3530 357d 7d09  0}, {770, 505}}.
+000005a0: 0909 0909 5f10 187b 7b31 3534 2c20 3139  ...._..{{154, 19
+000005b0: 347d 2c20 7b37 3133 2c20 3530 357d 7d09  4}, {713, 505}}.
 000005c0: 0817 2531 3d49 606d 797a 7b7c 7d7e 9900  ..%1=I`myz{|}~..
 000005d0: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
 000005e0: 0000 0000 0000 0000 0000 0000 0000 9a00  ................
 000005f0: 0000 0900 7300 7400 6100 7400 7300 6300  ....s.t.a.t.s.c.
 00000600: 6500 6e00 646c 6731 5363 6f6d 7000 0000  e.n.dlg1Scomp...
 00000610: 0000 0000 0000 0000 0900 7300 7400 6100  ..........s.t.a.
 00000620: 7400 7300 6300 6500 6e00 646d 6f44 4462  t.s.c.e.n.dmoDDb
```

### Comparing `statscend-0.1.8/statscend/bn_logistic_regression.py` & `statscend-0.1.9/statscend/bn_logistic_regression.py`

 * *Files identical despite different names*

### Comparing `statscend-0.1.8/statscend/datasets.py` & `statscend-0.1.9/statscend/datasets.py`

 * *Files identical despite different names*

### Comparing `statscend-0.1.8/statscend/linear_regression.py` & `statscend-0.1.9/statscend/linear_regression.py`

 * *Files identical despite different names*

### Comparing `statscend-0.1.8/statscend/mn_logistic_regression.py` & `statscend-0.1.9/statscend/mn_logistic_regression.py`

 * *Files identical despite different names*

### Comparing `statscend-0.1.8/statscend/ordinal_regression.py` & `statscend-0.1.9/statscend/ordinal_regression.py`

 * *Files identical despite different names*

### Comparing `statscend-0.1.8/LICENSE` & `statscend-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `statscend-0.1.8/README.md` & `statscend-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `statscend-0.1.8/pyproject.toml` & `statscend-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "statscend"
-version = "0.1.8"
+version = "0.1.9"
 license = {file = "LICENSE"}
 authors = [
   { name="Hashim Puthiyakath", email="hashputhiyakath@gmail.com" },
 ]
 description = "A Python package for performing various statistical analyses"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `statscend-0.1.8/PKG-INFO` & `statscend-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statscend
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python package for performing various statistical analyses
 Project-URL: Homepage, https://github.com/hashimputhiyakath/statscend
 Project-URL: Bug Tracker, https://github.com/hashimputhiyakath/statscend/issues
 Author-email: Hashim Puthiyakath <hashputhiyakath@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Hashim Puthiyakath
```

