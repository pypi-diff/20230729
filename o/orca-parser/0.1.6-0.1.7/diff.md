# Comparing `tmp/orca_parser-0.1.6-py2.py3-none-any.whl.zip` & `tmp/orca_parser-0.1.7-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7002 bytes, number of entries: 8
+Zip file size: 6998 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat     3325 b- defN 23-Jul-06 09:45 orca_parser/HessianTools.py
--rw-rw-rw-  2.0 fat    12227 b- defN 23-Jul-28 18:53 orca_parser/ORCAParse.py
+-rw-rw-rw-  2.0 fat    12207 b- defN 23-Jul-28 23:40 orca_parser/ORCAParse.py
 -rw-rw-rw-  2.0 fat      287 b- defN 23-Jul-06 09:50 orca_parser/__init__.py
--rw-rw-rw-  2.0 fat     1235 b- defN 23-Jul-28 23:37 orca_parser-0.1.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      482 b- defN 23-Jul-28 23:37 orca_parser-0.1.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-28 23:37 orca_parser-0.1.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Jul-28 23:37 orca_parser-0.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      651 b- defN 23-Jul-28 23:37 orca_parser-0.1.6.dist-info/RECORD
-8 files, 18329 bytes uncompressed, 5866 bytes compressed:  68.0%
+-rw-rw-rw-  2.0 fat     1235 b- defN 23-Jul-28 23:40 orca_parser-0.1.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      482 b- defN 23-Jul-28 23:40 orca_parser-0.1.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-28 23:40 orca_parser-0.1.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Jul-28 23:40 orca_parser-0.1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      651 b- defN 23-Jul-28 23:40 orca_parser-0.1.7.dist-info/RECORD
+8 files, 18309 bytes uncompressed, 5862 bytes compressed:  68.0%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: orca_parser/ORCAParse.py
 Comment: 
 
 Filename: orca_parser/__init__.py
 Comment: 
 
-Filename: orca_parser-0.1.6.dist-info/LICENSE
+Filename: orca_parser-0.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: orca_parser-0.1.6.dist-info/METADATA
+Filename: orca_parser-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: orca_parser-0.1.6.dist-info/WHEEL
+Filename: orca_parser-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: orca_parser-0.1.6.dist-info/top_level.txt
+Filename: orca_parser-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: orca_parser-0.1.6.dist-info/RECORD
+Filename: orca_parser-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## orca_parser/ORCAParse.py

```diff
@@ -192,15 +192,14 @@
     
     def parse_input(self):
         self.Z = int(round(float(self.raw.split("Sum of atomic charges:")[1].split("\n")[0])))
         self.Multiplicity = int(round(float(self.raw.split("* xyz")[1].replace("file","").split("\n")[0].split()[1])))
         self.orca_version = self.raw.split("Program Version ")[1].split()[0]
         inp = self.raw.split("|  1>")[1].split("\n")[0]
         inp = inp.upper()
-        print(inp)
         inp = inp.replace("!", "")
         inp = inp.split()
         inp_dict = {"Job": None, 
                     "Freq": False,
                     "Solvation": "Gas",
                     "Dispersion": None,
                     "Charge": self.Z,
```

## Comparing `orca_parser-0.1.6.dist-info/LICENSE` & `orca_parser-0.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `orca_parser-0.1.6.dist-info/RECORD` & `orca_parser-0.1.7.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 orca_parser/HessianTools.py,sha256=y936_LzZ3DGpnlElVQY96RtLPaKtRbEG5zPE4T-7VYY,3325
-orca_parser/ORCAParse.py,sha256=LwoWGmStsZ3aRHYiEw03fV5ZbKH5c2Q0yi5ASFzRDgo,12227
+orca_parser/ORCAParse.py,sha256=_koYtwiYKI9iytzuVciLT9qCSAeAwACfdMoIb6ojiCA,12207
 orca_parser/__init__.py,sha256=MlYoARmgG3uEVqcMY6rIRRYLHm0-4rh6WiSVGx-ngK4,287
-orca_parser-0.1.6.dist-info/LICENSE,sha256=Q2ptU2E48gOsMzhYz_kqVovmJ5d1KzrblLyqD2_-fvY,1235
-orca_parser-0.1.6.dist-info/METADATA,sha256=OlkxLpMgSufz1NN4IuLw37x1ocPmq23ohV3A_hzICY4,482
-orca_parser-0.1.6.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-orca_parser-0.1.6.dist-info/top_level.txt,sha256=8n8h8nQznt6NRgMjI0VijQ6cY5Nu7A0UUuc1M-GHe40,12
-orca_parser-0.1.6.dist-info/RECORD,,
+orca_parser-0.1.7.dist-info/LICENSE,sha256=Q2ptU2E48gOsMzhYz_kqVovmJ5d1KzrblLyqD2_-fvY,1235
+orca_parser-0.1.7.dist-info/METADATA,sha256=TO1dAipgsPqEZnQGVn_KKj4L0YQ03To6byTSzRISE2w,482
+orca_parser-0.1.7.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+orca_parser-0.1.7.dist-info/top_level.txt,sha256=8n8h8nQznt6NRgMjI0VijQ6cY5Nu7A0UUuc1M-GHe40,12
+orca_parser-0.1.7.dist-info/RECORD,,
```

