# Comparing `tmp/py40kie-0.1.3.tar.gz` & `tmp/py40kie-0.2.0.tar.gz`

## Comparing `py40kie-0.1.3.tar` & `py40kie-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 py40kie-0.1.3/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 py40kie-0.1.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py40kie-0.1.3/src/__init__.py
--rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 py40kie-0.1.3/src/py40kie.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 py40kie-0.1.3/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 py40kie-0.1.3/LICENSE
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 py40kie-0.1.3/README.md
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 py40kie-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 py40kie-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 py40kie-0.2.0/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 py40kie-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py40kie-0.2.0/src/__init__.py
+-rw-r--r--   0        0        0    11081 2020-02-02 00:00:00.000000 py40kie-0.2.0/src/py40kie.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 py40kie-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 py40kie-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3362 2020-02-02 00:00:00.000000 py40kie-0.2.0/README.md
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 py40kie-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 py40kie-0.2.0/PKG-INFO
```

### Comparing `py40kie-0.1.3/.github/workflows/publish-to-test-pypi.yml` & `py40kie-0.2.0/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `py40kie-0.1.3/.github/workflows/python-publish.yml` & `py40kie-0.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `py40kie-0.1.3/.gitignore` & `py40kie-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `py40kie-0.1.3/LICENSE` & `py40kie-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py40kie-0.1.3/README.md` & `py40kie-0.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,56 @@
 # Description
-Command line Python program to extract army rules and unit cards from 10th edition Warhammer 40k indexes to create army list specific pdfs with reduced file size. Requires Python and pypdf.
+Command line Python program to extract army rules and unit cards from 10th edition Warhammer 40k indexes to create army list specific pdfs with reduced file size. Requires Python.
 
 # Instructions
 - Download an army index https://www.warhammer-community.com/warhammer-40000-downloads/#indexes-faqs-and-errata  
 - Install [Python](https://wiki.python.org/moin/BeginnersGuide/Download)
 - Install py40kie using pip:  
   ```
-  pip install py40kie
+  pip install -U py40kie
   ```
 - Run py40kie using command line:  
   ```
-  py40kie [-h] [-o OUTPUT_PDF] [-e] [-nw] [-a ARMY_RULES_PAGES [ARMY_RULES_PAGES ...]] [-v] index_pdf pages [pages ...]
+  py40kie [-h] [-i EXTRA_INDEXES [EXTRA_INDEXES ...]] [-o OUTPUT_PDF] [-b] [-a] [-d] [-s] [-e] [-w] [-na] [-nd]
+               [-ns] [-ne] [-nw] [-r RULE_PAGES [RULE_PAGES ...]] [-v]
+               index_pdf pages [pages ...]
   ```
-  ###### Postional arguments
-    - The "index.pdf" file to extract cards from  
-    - Space separated list of cards to extract. Can be page numbers or **exact** unit titles. Army rules, strategems and unit wargear are included automatically  
-    ###### Optional arguments:  
-    - -o: The file to save the extracted pdf to. Folder path can be included
-    - -e: Optional flag to extract the enhancements page
-    - -nw: Optional flag to disable extracting wargear pages
-    - -a: Optional argument to specify army rules and strategem pages (space separated numbers). Use this if the army rules and strategems are not contained in the first 4 pages of the index  
-    - -v: Optional flag to override page extraction. Will extract only the page numbers specified  
   ### Examples  
   ```
-  py40kie "tyranids index.pdf" 9 21 25 27 -o "my army list"  
+  py40kie "Tyranids Index.pdf" 9 21 25 27 -o "my army list"  
+  ```
+  ```
+  py40kie "Tyranids Index.pdf" "hive tyrant" "tyranid warriors with ranged bio-weapons" 25 "hOrMaGaUnTs" -o "./my lists/my army list"
   ```
   ```
-  py40kie "tyranids index.pdf" "hive tyrant" "tyranid warriors with ranged bio-weapons" 25 "hOrMaGaUnTs" -o "./my lists/my army list"
+  py40kie "Space Wolves Index.pdf" 7 1-23 "Blood Claws" 1-53 "terminator squad" "2-culexus assassin" 2-7 3-1 -o "Best Army List Ever.pdf" -i "Space Marines Index.pdf" "Agents of Imperium Index.pdf" "Imperial Armour Astartes.pdf"
   ```
+  
+  # Arguments
+  #### Postional arguments
+    - The "index.pdf" file to extract cards from  
+    - Space separated list of cards to extract. Can be page numbers or **exact** unit titles. Army rules, detachment rules, stratagems, enhancements and unit wargear are included automatically  
+  #### Optional arguments:  
+    - -o: The file to save the extracted pdf to. Folder path can be included
+    - -i: Optional space separated list of additional pdfs to extract allied units from other Indexes/Imperial Armour/Legends ("1-10" to extract the card on page 10 from the first additional pdf). Also use this to extract the Adeptus Astartes army rule when using Space Marines
+    - -b: Optional flag for boarding actions (extracts the army rules page but not the detachment or stratagem pages)  
+    - -na: Optional flag to disable extracting the army rules page  
+    - -nd: Optional flag to disable extracting the detachment rules page  
+    - -ns: Optional flag to disable extracting the stratagem pages  
+    - -ne: Optional flag to disable extracting the enhancements page  
+    - -nw: Optional flag to disable extracting wargear pages  
+    - -r: Optional argument to specify army rules and stratagem pages (space separated numbers). Use this if the army rules and stratagems are not successfully extracted from the index  
+    - -v: Optional flag to override page extraction. Will extract only the page numbers specified from the main index  
 
 # Contributions  
 ## Future features  
-Any suggested features would be appreciated.  
+Any suggested features would be appreciated  
+ - [x] Allied units from other Indexes/Imperial Armour/Legends  
+ - [x] Extract Adeptus Astartes army rule page for Space Marine lists  
+ - [x] Convert Google Sheet army builder lists to runnable command https://www.reddit.com/r/WarhammerCompetitive/comments/14br6rw/10e_40k_list_builder_spreadsheets/  
+ - [ ] Extract extra rule pages. e.g. Deathwatch Armoury  
+ - [ ] Handle exceptions gracefully  
+ - [ ] Webapp version?...  
+
 
 ## Issues  
-py40kie was not tested on all indexes. If there is any problem extracting cards please submit an issue https://github.com/Dragons-Ire/40k-index-pdf-extractor/issues/new
+py40kie was not tested on all indexes. If there is any problem extracting cards please submit an issue https://github.com/Dragons-Ire/40k-index-pdf-extractor/issues/new
```

### Comparing `py40kie-0.1.3/pyproject.toml` & `py40kie-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "py40kie"
-version = "0.1.3"
+version = "0.2.0"
 authors = [
   { name="Chris Austin", email="dragons.ire.oce@gmail.com" },
 ]
 description = "Command line Python program to extract army rules and unit cards from 10th edition Warhammer 40k indexes to create army list specific pdfs with reduced file size."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `py40kie-0.1.3/PKG-INFO` & `py40kie-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py40kie
-Version: 0.1.3
+Version: 0.2.0
 Summary: Command line Python program to extract army rules and unit cards from 10th edition Warhammer 40k indexes to create army list specific pdfs with reduced file size.
 Project-URL: Homepage, https://github.com/Dragons-Ire/40k-index-pdf-extractor
 Project-URL: Bug Tracker, https://github.com/Dragons-Ire/40k-index-pdf-extractor/issues
 Author-email: Chris Austin <dragons.ire.oce@gmail.com>
 License-File: LICENSE
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
@@ -16,43 +16,62 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Requires-Dist: pypdf~=3.12.1
 Description-Content-Type: text/markdown
 
 # Description
-Command line Python program to extract army rules and unit cards from 10th edition Warhammer 40k indexes to create army list specific pdfs with reduced file size. Requires Python and pypdf.
+Command line Python program to extract army rules and unit cards from 10th edition Warhammer 40k indexes to create army list specific pdfs with reduced file size. Requires Python.
 
 # Instructions
 - Download an army index https://www.warhammer-community.com/warhammer-40000-downloads/#indexes-faqs-and-errata  
 - Install [Python](https://wiki.python.org/moin/BeginnersGuide/Download)
 - Install py40kie using pip:  
   ```
-  pip install py40kie
+  pip install -U py40kie
   ```
 - Run py40kie using command line:  
   ```
-  py40kie [-h] [-o OUTPUT_PDF] [-e] [-nw] [-a ARMY_RULES_PAGES [ARMY_RULES_PAGES ...]] [-v] index_pdf pages [pages ...]
+  py40kie [-h] [-i EXTRA_INDEXES [EXTRA_INDEXES ...]] [-o OUTPUT_PDF] [-b] [-a] [-d] [-s] [-e] [-w] [-na] [-nd]
+               [-ns] [-ne] [-nw] [-r RULE_PAGES [RULE_PAGES ...]] [-v]
+               index_pdf pages [pages ...]
   ```
-  ###### Postional arguments
-    - The "index.pdf" file to extract cards from  
-    - Space separated list of cards to extract. Can be page numbers or **exact** unit titles. Army rules, strategems and unit wargear are included automatically  
-    ###### Optional arguments:  
-    - -o: The file to save the extracted pdf to. Folder path can be included
-    - -e: Optional flag to extract the enhancements page
-    - -nw: Optional flag to disable extracting wargear pages
-    - -a: Optional argument to specify army rules and strategem pages (space separated numbers). Use this if the army rules and strategems are not contained in the first 4 pages of the index  
-    - -v: Optional flag to override page extraction. Will extract only the page numbers specified  
   ### Examples  
   ```
-  py40kie "tyranids index.pdf" 9 21 25 27 -o "my army list"  
+  py40kie "Tyranids Index.pdf" 9 21 25 27 -o "my army list"  
+  ```
+  ```
+  py40kie "Tyranids Index.pdf" "hive tyrant" "tyranid warriors with ranged bio-weapons" 25 "hOrMaGaUnTs" -o "./my lists/my army list"
   ```
   ```
-  py40kie "tyranids index.pdf" "hive tyrant" "tyranid warriors with ranged bio-weapons" 25 "hOrMaGaUnTs" -o "./my lists/my army list"
+  py40kie "Space Wolves Index.pdf" 7 1-23 "Blood Claws" 1-53 "terminator squad" "2-culexus assassin" 2-7 3-1 -o "Best Army List Ever.pdf" -i "Space Marines Index.pdf" "Agents of Imperium Index.pdf" "Imperial Armour Astartes.pdf"
   ```
+  
+  # Arguments
+  #### Postional arguments
+    - The "index.pdf" file to extract cards from  
+    - Space separated list of cards to extract. Can be page numbers or **exact** unit titles. Army rules, detachment rules, stratagems, enhancements and unit wargear are included automatically  
+  #### Optional arguments:  
+    - -o: The file to save the extracted pdf to. Folder path can be included
+    - -i: Optional space separated list of additional pdfs to extract allied units from other Indexes/Imperial Armour/Legends ("1-10" to extract the card on page 10 from the first additional pdf). Also use this to extract the Adeptus Astartes army rule when using Space Marines
+    - -b: Optional flag for boarding actions (extracts the army rules page but not the detachment or stratagem pages)  
+    - -na: Optional flag to disable extracting the army rules page  
+    - -nd: Optional flag to disable extracting the detachment rules page  
+    - -ns: Optional flag to disable extracting the stratagem pages  
+    - -ne: Optional flag to disable extracting the enhancements page  
+    - -nw: Optional flag to disable extracting wargear pages  
+    - -r: Optional argument to specify army rules and stratagem pages (space separated numbers). Use this if the army rules and stratagems are not successfully extracted from the index  
+    - -v: Optional flag to override page extraction. Will extract only the page numbers specified from the main index  
 
 # Contributions  
 ## Future features  
-Any suggested features would be appreciated.  
+Any suggested features would be appreciated  
+ - [x] Allied units from other Indexes/Imperial Armour/Legends  
+ - [x] Extract Adeptus Astartes army rule page for Space Marine lists  
+ - [x] Convert Google Sheet army builder lists to runnable command https://www.reddit.com/r/WarhammerCompetitive/comments/14br6rw/10e_40k_list_builder_spreadsheets/  
+ - [ ] Extract extra rule pages. e.g. Deathwatch Armoury  
+ - [ ] Handle exceptions gracefully  
+ - [ ] Webapp version?...  
+
 
 ## Issues  
-py40kie was not tested on all indexes. If there is any problem extracting cards please submit an issue https://github.com/Dragons-Ire/40k-index-pdf-extractor/issues/new
+py40kie was not tested on all indexes. If there is any problem extracting cards please submit an issue https://github.com/Dragons-Ire/40k-index-pdf-extractor/issues/new
```

