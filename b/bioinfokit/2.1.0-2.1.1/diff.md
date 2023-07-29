# Comparing `tmp/bioinfokit-2.1.0.tar.gz` & `tmp/bioinfokit-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioinfokit-2.1.0.tar", last modified: Tue Sep 13 07:52:03 2022, max compression
+gzip compressed data, was "bioinfokit-2.1.1.tar", last modified: Sat Jul 29 19:31:56 2023, max compression
```

## Comparing `bioinfokit-2.1.0.tar` & `bioinfokit-2.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-09-13 07:52:03.428678 bioinfokit-2.1.0/
--rw-rw-rw-   0        0        0     1072 2022-09-04 05:33:18.000000 bioinfokit-2.1.0/LICENSE
--rw-rw-rw-   0        0        0    71224 2022-09-13 07:52:03.428678 bioinfokit-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    68857 2022-09-13 07:51:32.000000 bioinfokit-2.1.0/README.md
-drwxrwxrwx   0        0        0        0 2022-09-13 07:52:03.397427 bioinfokit-2.1.0/bioinfokit/
--rw-rw-rw-   0        0        0       72 2022-09-13 07:23:14.000000 bioinfokit-2.1.0/bioinfokit/__init__.py
--rw-rw-rw-   0        0        0   135342 2022-09-13 04:52:32.000000 bioinfokit-2.1.0/bioinfokit/analys.py
--rw-rw-rw-   0        0        0     3059 2022-09-04 05:33:18.000000 bioinfokit-2.1.0/bioinfokit/help.py
--rw-rw-rw-   0        0        0   118756 2022-09-04 05:33:18.000000 bioinfokit-2.1.0/bioinfokit/visuz.py
-drwxrwxrwx   0        0        0        0 2022-09-13 07:52:03.428678 bioinfokit-2.1.0/bioinfokit.egg-info/
--rw-rw-rw-   0        0        0    71224 2022-09-13 07:52:03.000000 bioinfokit-2.1.0/bioinfokit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2022-09-13 07:52:03.000000 bioinfokit-2.1.0/bioinfokit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-13 07:52:03.000000 bioinfokit-2.1.0/bioinfokit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-09-04 18:55:51.000000 bioinfokit-2.1.0/bioinfokit.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      109 2022-09-13 07:52:03.000000 bioinfokit-2.1.0/bioinfokit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-09-13 07:52:03.000000 bioinfokit-2.1.0/bioinfokit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-09-13 07:52:03.428678 bioinfokit-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1500 2022-09-04 05:33:18.000000 bioinfokit-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 19:31:56.447629 bioinfokit-2.1.1/
+-rw-rw-rw-   0        0        0     1072 2022-09-04 05:33:18.000000 bioinfokit-2.1.1/LICENSE
+-rw-rw-rw-   0        0        0    71224 2023-07-29 19:31:56.447629 bioinfokit-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    68857 2022-09-13 19:56:44.000000 bioinfokit-2.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 19:31:56.400750 bioinfokit-2.1.1/bioinfokit/
+-rw-rw-rw-   0        0        0       72 2023-07-29 19:27:15.000000 bioinfokit-2.1.1/bioinfokit/__init__.py
+-rw-rw-rw-   0        0        0   135500 2023-07-29 19:21:24.000000 bioinfokit-2.1.1/bioinfokit/analys.py
+-rw-rw-rw-   0        0        0     3059 2022-09-04 05:33:18.000000 bioinfokit-2.1.1/bioinfokit/help.py
+-rw-rw-rw-   0        0        0   118756 2022-09-04 05:33:18.000000 bioinfokit-2.1.1/bioinfokit/visuz.py
+drwxrwxrwx   0        0        0        0 2023-07-29 19:31:56.447629 bioinfokit-2.1.1/bioinfokit.egg-info/
+-rw-rw-rw-   0        0        0    71224 2023-07-29 19:31:56.000000 bioinfokit-2.1.1/bioinfokit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-07-29 19:31:56.000000 bioinfokit-2.1.1/bioinfokit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 19:31:56.000000 bioinfokit-2.1.1/bioinfokit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-09-04 18:55:51.000000 bioinfokit-2.1.1/bioinfokit.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      109 2023-07-29 19:31:56.000000 bioinfokit-2.1.1/bioinfokit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-29 19:31:56.000000 bioinfokit-2.1.1/bioinfokit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 19:31:56.447629 bioinfokit-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1500 2022-09-04 05:33:18.000000 bioinfokit-2.1.1/setup.py
```

### Comparing `bioinfokit-2.1.0/LICENSE` & `bioinfokit-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bioinfokit-2.1.0/PKG-INFO` & `bioinfokit-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2062 696f  : 2.1..Name: bio
 00000020: 696e 666f 6b69 740d 0a56 6572 7369 6f6e  infokit..Version
-00000030: 3a20 322e 312e 300d 0a53 756d 6d61 7279  : 2.1.0..Summary
+00000030: 3a20 322e 312e 310d 0a53 756d 6d61 7279  : 2.1.1..Summary
 00000040: 3a20 4269 6f69 6e66 6f72 6d61 7469 6373  : Bioinformatics
 00000050: 2064 6174 6120 616e 616c 7973 6973 2061   data analysis a
 00000060: 6e64 2076 6973 7561 6c69 7a61 7469 6f6e  nd visualization
 00000070: 2074 6f6f 6c6b 6974 0d0a 486f 6d65 2d70   toolkit..Home-p
 00000080: 6167 653a 2068 7474 7073 3a2f 2f67 6974  age: https://git
 00000090: 6875 622e 636f 6d2f 7265 6e65 7368 6265  hub.com/reneshbe
 000000a0: 6472 652f 6269 6f69 6e66 6f6b 6974 0d0a  dre/bioinfokit..
@@ -3188,15 +3188,15 @@
 0000c730: 6964 656e 6365 2069 6e74 6572 7661 6c20  idence interval 
 0000c740: 2843 4929 2e20 4966 2061 6c70 6861 3d30  (CI). If alpha=0
 0000c750: 2e30 352c 2074 6865 6e20 3935 2520 4349  .05, then 95% CI
 0000c760: 2077 696c 6c20 6265 2063 616c 6375 6c61   will be calcula
 0000c770: 7465 6420 205b 666c 6f61 745d 5b64 6566  ted  [float][def
 0000c780: 6175 6c74 3a20 302e 3035 5d0d 0a60 7465  ault: 0.05]..`te
 0000c790: 7374 5f74 7970 6560 207c 2054 7970 6520  st_type` | Type 
-0000c7a0: 6f66 2074 2d74 6573 7420 5b69 6e74 2028  of t-test [int (
+0000c7a0: 6f66 205a 2d74 6573 7420 5b69 6e74 2028  of Z-test [int (
 0000c7b0: 312c 3229 5d5b 6465 6661 756c 743a 204e  1,2)][default: N
 0000c7c0: 6f6e 655d 2e20 3c62 723e 203c 7374 726f  one]. <br> <stro
 0000c7d0: 6e67 3e3c 656d 3e31 3c2f 656d 3e3c 2f73  ng><em>1</em></s
 0000c7e0: 7472 6f6e 673e 3a20 4f6e 6520 7361 6d70  trong>: One samp
 0000c7f0: 6c65 205a 2d74 6573 7420 3c62 723e 203c  le Z-test <br> <
 0000c800: 7374 726f 6e67 3e3c 656d 3e32 3c2f 656d  strong><em>2</em
 0000c810: 3e3c 2f73 7472 6f6e 673e 3a20 5477 6f20  ></strong>: Two
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bioinfokit Version: 2.1.0 Summary: Bioinformatics
+Metadata-Version: 2.1 Name: bioinfokit Version: 2.1.1 Summary: Bioinformatics
 data analysis and visualization toolkit Home-page: https://github.com/
 reneshbedre/bioinfokit Author: Renesh Bedre Author-email: reneshbe@gmail.com
 Maintainer: Renesh Bedre License: MIT Platform: UNKNOWN Classifier: Development
 Status :: 4 - Beta Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: Unix
@@ -610,15 +610,15 @@
 Two sample independent: It should have atleast two variables `x` | column name
 for x group [string][default: None] `y` | column name for x group [string]
 [default: None] `mu` | Population or known mean for the one sample Z-test
 [float][default: None] `x_std` | Population standard deviation for x group
 [float][default: None] `y_std` | Population standard deviation for y group
 [float][default: None] `alpha` | Significance level for confidence interval
 (CI). If alpha=0.05, then 95% CI will be calculated [float][default: 0.05]
-`test_type` | Type of t-test [int (1,2)][default: None].
+`test_type` | Type of Z-test [int (1,2)][default: None].
 1: One sample Z-test
 2: Two sample Z-test Returns: Summary output as class attribute (summary and
 result) Description_and_Working_example ### One sample and two sample
 (independent and paired) t-tests `latest update v2.1.0`
 `bioinfokit.analys.stat.ttest(df, xfac, res, evar, alpha, test_type, mu)`
 Parameters | Description ------------ | ------------- `df` | Pandas dataframe
 for appropriate t-test.
```

### Comparing `bioinfokit-2.1.0/README.md` & `bioinfokit-2.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -935,15 +935,15 @@
 `df` | Pandas dataframe for appropriate Z-test. <br> <b>One sample</b>: It should have atleast one variable <br> <b>Two sample independent</b>: It should have atleast two variables 
 `x` | column name for x group [string][default: None]
 `y` | column name for x group [string][default: None]
 `mu` | Population or known mean for the one sample Z-test [float][default: None]
 `x_std` | Population standard deviation for x group [float][default: None]
 `y_std` | Population standard deviation for y group [float][default: None]
 `alpha` | Significance level for confidence interval (CI). If alpha=0.05, then 95% CI will be calculated  [float][default: 0.05]
-`test_type` | Type of t-test [int (1,2)][default: None]. <br> <strong><em>1</em></strong>: One sample Z-test <br> <strong><em>2</em></strong>: Two sample Z-test 
+`test_type` | Type of Z-test [int (1,2)][default: None]. <br> <strong><em>1</em></strong>: One sample Z-test <br> <strong><em>2</em></strong>: Two sample Z-test 
 
 Returns:
 
 Summary output as class attribute (summary and result) 
 
 <a href="https://reneshbedre.com/blog/ttest.html" target="_blank">Description and Working example</a>
```

#### html2text {}

```diff
@@ -597,15 +597,15 @@
 Two sample independent: It should have atleast two variables `x` | column name
 for x group [string][default: None] `y` | column name for x group [string]
 [default: None] `mu` | Population or known mean for the one sample Z-test
 [float][default: None] `x_std` | Population standard deviation for x group
 [float][default: None] `y_std` | Population standard deviation for y group
 [float][default: None] `alpha` | Significance level for confidence interval
 (CI). If alpha=0.05, then 95% CI will be calculated [float][default: 0.05]
-`test_type` | Type of t-test [int (1,2)][default: None].
+`test_type` | Type of Z-test [int (1,2)][default: None].
 1: One sample Z-test
 2: Two sample Z-test Returns: Summary output as class attribute (summary and
 result) Description_and_Working_example ### One sample and two sample
 (independent and paired) t-tests `latest update v2.1.0`
 `bioinfokit.analys.stat.ttest(df, xfac, res, evar, alpha, test_type, mu)`
 Parameters | Description ------------ | ------------- `df` | Pandas dataframe
 for appropriate t-test.
```

### Comparing `bioinfokit-2.1.0/bioinfokit/analys.py` & `bioinfokit-2.1.1/bioinfokit/analys.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,23 +61,23 @@
             seq = "".join(s.strip() for s in fasta_iter.__next__())
             yield fasta_header, seq
 
     @staticmethod
     def rev_com(seq=None, file=None):
         if seq is not None:
             rev_seq = seq[::-1]
-            rev_seq = rev_seq.translate(str.maketrans("ATGCUN", "TACGAN"))
+            rev_seq = rev_seq.translate(str.maketrans("ATGCUNatgcu", "TACGANtacga"))
             return rev_seq
         elif file is not None:
             out_file = open("output_revcom.fasta", 'w')
-            fasta_iter = fasta_reader(file)
+            fasta_iter = Fasta.fasta_reader(file)
             for record in fasta_iter:
                 fasta_header, seq = record
                 rev_seq = seq[::-1]
-                rev_seq = rev_seq.translate(str.maketrans("ATGCUN", "TACGAN"))
+                rev_seq = rev_seq.translate(str.maketrans("ATGCUNatgcu", "TACGANtacga"))
                 out_file.write(">" + fasta_header + "\n" + rev_seq + "\n")
             out_file.close()
 
     @staticmethod
     def ext_subseq(file="fasta_file", id="chr", st="start", end="end", strand="plus"):
         fasta_iter = Fasta.fasta_reader(file)
         for record in fasta_iter:
@@ -2592,14 +2592,16 @@
             self.data = pd.read_csv("https://reneshbedre.github.io/assets/posts/ttest/t_one_samp.csv")
         elif data=='z_one_samp':
             self.data = pd.read_csv("https://reneshbedre.github.io/assets/posts/ztest/z_one_samp.csv")
         elif data=='z_two_samp':
             self.data = pd.read_csv("https://reneshbedre.github.io/assets/posts/ztest/z_two_samp.csv")
         elif data=='t_pair':
             self.data = pd.read_csv("https://reneshbedre.github.io/assets/posts/ttest/t_pair.csv")
+        elif data == 'z_pair':
+            self.data = pd.read_csv("https://reneshbedre.github.io/assets/posts/ztest/paired_z.csv")
         elif data=='wdbc_train':
             self.data = pd.read_csv("https://reneshbedre.github.io/assets/posts/logit/wdbc_train.csv")
         elif data=='wdbc_test':
             self.data = pd.read_csv("https://reneshbedre.github.io/assets/posts/logit/wdbc_test.csv")
         elif data=='plant_richness':
             self.data = pd.read_csv('https://reneshbedre.github.io/assets/posts/reg/plant_richness_data_mlr.txt',
                                     sep='\t')
```

### Comparing `bioinfokit-2.1.0/bioinfokit/help.py` & `bioinfokit-2.1.1/bioinfokit/help.py`

 * *Files identical despite different names*

### Comparing `bioinfokit-2.1.0/bioinfokit/visuz.py` & `bioinfokit-2.1.1/bioinfokit/visuz.py`

 * *Files identical despite different names*

### Comparing `bioinfokit-2.1.0/bioinfokit.egg-info/PKG-INFO` & `bioinfokit-2.1.1/bioinfokit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2062 696f  : 2.1..Name: bio
 00000020: 696e 666f 6b69 740d 0a56 6572 7369 6f6e  infokit..Version
-00000030: 3a20 322e 312e 300d 0a53 756d 6d61 7279  : 2.1.0..Summary
+00000030: 3a20 322e 312e 310d 0a53 756d 6d61 7279  : 2.1.1..Summary
 00000040: 3a20 4269 6f69 6e66 6f72 6d61 7469 6373  : Bioinformatics
 00000050: 2064 6174 6120 616e 616c 7973 6973 2061   data analysis a
 00000060: 6e64 2076 6973 7561 6c69 7a61 7469 6f6e  nd visualization
 00000070: 2074 6f6f 6c6b 6974 0d0a 486f 6d65 2d70   toolkit..Home-p
 00000080: 6167 653a 2068 7474 7073 3a2f 2f67 6974  age: https://git
 00000090: 6875 622e 636f 6d2f 7265 6e65 7368 6265  hub.com/reneshbe
 000000a0: 6472 652f 6269 6f69 6e66 6f6b 6974 0d0a  dre/bioinfokit..
@@ -3188,15 +3188,15 @@
 0000c730: 6964 656e 6365 2069 6e74 6572 7661 6c20  idence interval 
 0000c740: 2843 4929 2e20 4966 2061 6c70 6861 3d30  (CI). If alpha=0
 0000c750: 2e30 352c 2074 6865 6e20 3935 2520 4349  .05, then 95% CI
 0000c760: 2077 696c 6c20 6265 2063 616c 6375 6c61   will be calcula
 0000c770: 7465 6420 205b 666c 6f61 745d 5b64 6566  ted  [float][def
 0000c780: 6175 6c74 3a20 302e 3035 5d0d 0a60 7465  ault: 0.05]..`te
 0000c790: 7374 5f74 7970 6560 207c 2054 7970 6520  st_type` | Type 
-0000c7a0: 6f66 2074 2d74 6573 7420 5b69 6e74 2028  of t-test [int (
+0000c7a0: 6f66 205a 2d74 6573 7420 5b69 6e74 2028  of Z-test [int (
 0000c7b0: 312c 3229 5d5b 6465 6661 756c 743a 204e  1,2)][default: N
 0000c7c0: 6f6e 655d 2e20 3c62 723e 203c 7374 726f  one]. <br> <stro
 0000c7d0: 6e67 3e3c 656d 3e31 3c2f 656d 3e3c 2f73  ng><em>1</em></s
 0000c7e0: 7472 6f6e 673e 3a20 4f6e 6520 7361 6d70  trong>: One samp
 0000c7f0: 6c65 205a 2d74 6573 7420 3c62 723e 203c  le Z-test <br> <
 0000c800: 7374 726f 6e67 3e3c 656d 3e32 3c2f 656d  strong><em>2</em
 0000c810: 3e3c 2f73 7472 6f6e 673e 3a20 5477 6f20  ></strong>: Two
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bioinfokit Version: 2.1.0 Summary: Bioinformatics
+Metadata-Version: 2.1 Name: bioinfokit Version: 2.1.1 Summary: Bioinformatics
 data analysis and visualization toolkit Home-page: https://github.com/
 reneshbedre/bioinfokit Author: Renesh Bedre Author-email: reneshbe@gmail.com
 Maintainer: Renesh Bedre License: MIT Platform: UNKNOWN Classifier: Development
 Status :: 4 - Beta Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: Unix
@@ -610,15 +610,15 @@
 Two sample independent: It should have atleast two variables `x` | column name
 for x group [string][default: None] `y` | column name for x group [string]
 [default: None] `mu` | Population or known mean for the one sample Z-test
 [float][default: None] `x_std` | Population standard deviation for x group
 [float][default: None] `y_std` | Population standard deviation for y group
 [float][default: None] `alpha` | Significance level for confidence interval
 (CI). If alpha=0.05, then 95% CI will be calculated [float][default: 0.05]
-`test_type` | Type of t-test [int (1,2)][default: None].
+`test_type` | Type of Z-test [int (1,2)][default: None].
 1: One sample Z-test
 2: Two sample Z-test Returns: Summary output as class attribute (summary and
 result) Description_and_Working_example ### One sample and two sample
 (independent and paired) t-tests `latest update v2.1.0`
 `bioinfokit.analys.stat.ttest(df, xfac, res, evar, alpha, test_type, mu)`
 Parameters | Description ------------ | ------------- `df` | Pandas dataframe
 for appropriate t-test.
```

### Comparing `bioinfokit-2.1.0/setup.py` & `bioinfokit-2.1.1/setup.py`

 * *Files identical despite different names*

