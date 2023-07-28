# Comparing `tmp/xpiz-0.0.2.tar.gz` & `tmp/xpiz-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpiz-0.0.2.tar", last modified: Fri Jul 28 22:21:21 2023, max compression
+gzip compressed data, was "xpiz-0.0.3.tar", last modified: Fri Jul 28 23:09:38 2023, max compression
```

## Comparing `xpiz-0.0.2.tar` & `xpiz-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:21:21.976628 xpiz-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-28 22:21:09.000000 xpiz-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-28 22:21:21.976628 xpiz-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-28 22:21:09.000000 xpiz-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 22:21:21.976628 xpiz-0.0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3380 2023-07-28 22:21:09.000000 xpiz-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:21:21.976628 xpiz-0.0.2/xpiz/
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-07-28 22:21:09.000000 xpiz-0.0.2/xpiz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:21:21.976628 xpiz-0.0.2/xpiz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-28 22:21:21.000000 xpiz-0.0.2/xpiz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-28 22:21:21.000000 xpiz-0.0.2/xpiz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 22:21:21.000000 xpiz-0.0.2/xpiz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-28 22:21:21.000000 xpiz-0.0.2/xpiz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-28 22:21:21.000000 xpiz-0.0.2/xpiz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:09:38.058225 xpiz-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-28 23:09:27.000000 xpiz-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-28 23:09:38.058225 xpiz-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-28 23:09:27.000000 xpiz-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 23:09:38.058225 xpiz-0.0.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3380 2023-07-28 23:09:27.000000 xpiz-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:09:38.054225 xpiz-0.0.3/xpiz/
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-28 23:09:27.000000 xpiz-0.0.3/xpiz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:09:38.058225 xpiz-0.0.3/xpiz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-28 23:09:38.000000 xpiz-0.0.3/xpiz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-28 23:09:38.000000 xpiz-0.0.3/xpiz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 23:09:38.000000 xpiz-0.0.3/xpiz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-28 23:09:38.000000 xpiz-0.0.3/xpiz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-28 23:09:38.000000 xpiz-0.0.3/xpiz.egg-info/top_level.txt
```

### Comparing `xpiz-0.0.2/LICENSE` & `xpiz-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xpiz-0.0.2/setup.py` & `xpiz-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

### Comparing `xpiz-0.0.2/xpiz/__init__.py` & `xpiz-0.0.3/xpiz/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 			print(f"Exception :> {e}")
 			failure = True
 
 	if not failure:
 		os.remove(foil)
 	return foils_created
 
-def join(foil):
+def join(foil, quiet=True):
 	foil = foil.replace('.sums','')
 	mini_foils,current_binary = re(str(foil).replace('.zip','') + "_broken_up_*.zip"),None
 	mini_foils.sort()
 	for mini_foil in mini_foils:
 		raw_foil = mini_foil.replace('.zip','')
 		with zipfile.ZipFile(mini_foil,"r") as f:
 			raw_foil = f.extract(member=raw_foil, path=os.path.dirname(mini_foil))
@@ -99,19 +99,22 @@
 	hashFile = foil + ".sums"
 	if os.path.exists(hashFile):
 		try:
 			currentHash = hash(foil)
 			with open(hashFile, 'r') as reader:
 				oldHash = json.load(reader)['hash']
 			equal = "===" if currentHash == oldHash else "=!="
-			print("The old hash {0} the current hash".format(equal))
+			if not quiet:
+				print("The old hash {0} the current hash".format(equal))
 		except:
-			print("File {0} cannot be verified".format(foil))
+			if not quiet:
+				print("File {0} cannot be verified".format(foil))
 	else:
-		print("File {0} cannot be verified".format(foil))
+		if not quiet:
+			print("File {0} cannot be verified".format(foil))
 	return foil
 
 def arguments():
 	import argparse
 	parser = argparse.ArgumentParser(description=f"Enabling the capability to stretch a single large file into many smaller files")
 	parser.add_argument("-f","--file", help="The name of the file", nargs='*')
 	parser.add_argument("--split", help="Split the file up", action="store_true",default=False)
```

