# Comparing `tmp/kohlrahbi-0.0.8.tar.gz` & `tmp/kohlrahbi-0.0.9.tar.gz`

## Comparing `kohlrahbi-0.0.8.tar` & `kohlrahbi-0.0.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0     6576 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/README.md
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/requirements.in
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/requirements.txt
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/tox.ini
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/.github/dependabot.yml
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/.github/workflows/black.yml
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/.github/workflows/packaging_test.yml
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/.github/workflows/pythonlint.yml
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/.github/workflows/unittests.yml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/_kohlrahbi_version.py
--rw-r--r--   0        0        0     9052 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/__init__.py
--rw-r--r--   0        0        0     8303 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/ahbfilefinder.py
--rw-r--r--   0        0        0     8770 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/all_known_pruefis.toml
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/collect_pruefis.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/logger.ini
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/logger.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/py.typed
--rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/read_functions.py
--rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/row_type_checker.py
--rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/seed.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/ahb/__init__.py
--rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/ahb/ahbsubtable.py
--rw-r--r--   0        0        0     7918 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/ahb/ahbtable.py
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/ahb/ahbtablerow.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/docxtablecells/__init__.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/docxtablecells/bedinungscell.py
--rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/docxtablecells/bodycell.py
--rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/docxtablecells/edifactstrukturcell.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/enums/__init__.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/enums/flat_ahb_row_type.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/enums/row_type.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/enums/row_type_color.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/unfoldedahb/__init__.py
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/unfoldedahb/unfoldedahbline.py
--rw-r--r--   0        0        0    18732 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/src/kohlrahbi/unfoldedahb/unfoldedahbtablemetadata.py
--rw-r--r--   0        0        0   861363 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/temp/test-fobar.docx
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/LICENSE
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     7738 2020-02-02 00:00:00.000000 kohlrahbi-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     6862 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/README.md
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/requirements.in
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/requirements.txt
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/tox.ini
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/.github/dependabot.yml
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/.github/workflows/black.yml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/.github/workflows/packaging_test.yml
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/.github/workflows/pythonlint.yml
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/src/_kohlrahbi_version.py
+-rw-r--r--   0        0        0     9080 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/src/kohlrahbi/__init__.py
+-rw-r--r--   0        0        0     8514 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/src/kohlrahbi/ahbfilefinder.py
+-rw-r--r--   0        0        0     8770 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/src/kohlrahbi/all_known_pruefis.toml
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/src/kohlrahbi/collect_pruefis.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/src/kohlrahbi/logger.ini
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/src/kohlrahbi/logger.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/src/kohlrahbi/py.typed
+-rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/src/kohlrahbi/read_functions.py
+-rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/src/kohlrahbi/row_type_checker.py
+-rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/src/kohlrahbi/seed.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/src/kohlrahbi/ahb/__init__.py
+-rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/src/kohlrahbi/ahb/ahbsubtable.py
+-rw-r--r--   0        0        0     7918 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/src/kohlrahbi/ahb/ahbtable.py
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/src/kohlrahbi/ahb/ahbtablerow.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/src/kohlrahbi/docxtablecells/__init__.py
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/src/kohlrahbi/docxtablecells/bedinungscell.py
+-rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/src/kohlrahbi/docxtablecells/bodycell.py
+-rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/src/kohlrahbi/docxtablecells/edifactstrukturcell.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/src/kohlrahbi/enums/__init__.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/src/kohlrahbi/enums/flat_ahb_row_type.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/src/kohlrahbi/enums/row_type.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/src/kohlrahbi/enums/row_type_color.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/src/kohlrahbi/unfoldedahb/__init__.py
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/src/kohlrahbi/unfoldedahb/unfoldedahbline.py
+-rw-r--r--   0        0        0    18853 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/src/kohlrahbi/unfoldedahb/unfoldedahbtablemetadata.py
+-rw-r--r--   0        0        0   861363 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/temp/test-fobar.docx
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 kohlrahbi-0.0.9/PKG-INFO
```

### Comparing `kohlrahbi-0.0.8/.pre-commit-config.yaml` & `kohlrahbi-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.8/README.md` & `kohlrahbi-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,16 @@
 ```
 
 You can also provide multiple prüfidentifikatoren.
 
 ```bash
 kohlrahbi --input_path ../edi_energy_mirror/edi_energy_de/current --output_path ./output/ --pruefis 11039 --pruefis 11040 --pruefi 11041 --file-type csv
 ```
+### Results
+There is a kohlrahbi based CI pipeline from the edi_energy_mirror mentioned above to the repository [machine-readable_anwendungshandbuecher](https://github.com/Hochfrequenz/machine-readable_anwendungshandbuecher) where you can find scraped AHBs as JSON, CSV or Excel files.
 
 ## Workflow
 
 ```mermaid
 flowchart TB
     S[Start] --> RD[Read docx]
     RD --> RPT[Read all paragraphs <br> and tables]
@@ -137,16 +139,16 @@
 
 ### Run all tests and linters
 
 To run the tests, you can use tox.
 
 ```bash
 tox
-See our [Python Template Repository](https://github.com/Hochfrequenz/python_template_repository#how-to-use-this-repository-on-your-machine) for detailed explanations.
 ```
+See our [Python Template Repository](https://github.com/Hochfrequenz/python_template_repository#how-to-use-this-repository-on-your-machine) for detailed explanations.
 
 ## Contribute
 
 You are very welcome to contribute to this template repository by opening a pull request against the main branch.
 
 ## Related Tools and Context
```

### Comparing `kohlrahbi-0.0.8/requirements.txt` & `kohlrahbi-0.0.9/requirements.txt`

 * *Files 22% similar despite different names*

```diff
@@ -36,13 +36,13 @@
     # via pandas
 python-docx==0.8.11
     # via -r requirements.in
 pytz==2023.3
     # via pandas
 six==1.16.0
     # via python-dateutil
-tomlkit==0.11.8
+tomlkit==0.12.1
     # via -r requirements.in
 tzdata==2023.3
     # via pandas
 xlsxwriter==3.1.2
     # via -r requirements.in
```

### Comparing `kohlrahbi-0.0.8/tox.ini` & `kohlrahbi-0.0.9/tox.ini`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.8/.github/dependabot.yml` & `kohlrahbi-0.0.9/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.8/.github/workflows/black.yml` & `kohlrahbi-0.0.9/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.8/.github/workflows/coverage.yml` & `kohlrahbi-0.0.9/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.8/.github/workflows/packaging_test.yml` & `kohlrahbi-0.0.9/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.8/.github/workflows/python-publish.yml` & `kohlrahbi-0.0.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.8/.github/workflows/pythonlint.yml` & `kohlrahbi-0.0.9/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.8/.github/workflows/unittests.yml` & `kohlrahbi-0.0.9/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.8/src/kohlrahbi/__init__.py` & `kohlrahbi-0.0.9/src/kohlrahbi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,14 +222,15 @@
                 "There was an uncaught error while processing the pruefi '%s': %s",
                 pruefi,
                 str(general_error),
                 exc_info=True,
             )
             continue
         del ahb_table
+        del ahb_file_finder
         if "unfolded_ahb" in locals():
             del unfolded_ahb
         gc.collect()
 
 
 if __name__ == "__main__":
     # the parameter arguments gets provided over the CLI
```

### Comparing `kohlrahbi-0.0.8/src/kohlrahbi/ahbfilefinder.py` & `kohlrahbi-0.0.9/src/kohlrahbi/ahbfilefinder.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 
         return path_to_ahb_document.name.split("-")[0]
 
     def filter_for_latest_ahb_docx_files(self) -> None:
         """
         Filter the list of AHB docx paths for the latest AHB docx files.
         The latest files contain `LesefassungmitFehlerkorrekturen` in their file names.
+        This method is _not_ pure. It changes the state of the object.
         """
         result: list[Path] = []
 
         groups: dict[str, list[Path]] = {  # the key is the first part of the file name, the values are matching files
             group_key: list(group)
             for group_key, group in groupby(
                 sorted(self.paths_to_docx_files, key=AhbFileFinder.get_first_part_of_ahb_docx_file_name),
@@ -71,24 +72,26 @@
                     else:
                         logger.debug("Ignoring file %s", path.name)
         self.paths_to_docx_files = result
 
     def filter_docx_files_for_edifact_format(self, edifact_format: EdifactFormat) -> None:
         """
         Returns a list of docx files which contain the given edifact format.
+        This method is not pure. It changes the state of the object.
         """
 
         self.paths_to_docx_files = [path for path in self.paths_to_docx_files if str(edifact_format) in path.name]
 
     def get_docx_files_which_may_contain_searched_pruefi(self, searched_pruefi: str) -> list[Path]:
         """
         This functions takes a pruefidentifikator and returns a list of docx files which can contain the searched pruefi
         Unfortunately, it is not clear in which docx the pruefidentifikator you are looking for is located.
         A 11042 belongs to the UTILMD format. However, there are seven docx files that describe the UTILMD format.
         A further reduction of the number of files is not possible with the pruefidentifikator only.
+        This method is _not_ pure. It changes the state of the object.
         """
 
         edifact_format = get_format_of_pruefidentifikator(searched_pruefi)
         if edifact_format is None:
             logger.exception("❌ There is no known format for the prüfi '%s'.", searched_pruefi)
             raise ValueError(f"There is no known format for the prüfi '{searched_pruefi}'.")
```

### Comparing `kohlrahbi-0.0.8/src/kohlrahbi/all_known_pruefis.toml` & `kohlrahbi-0.0.9/src/kohlrahbi/all_known_pruefis.toml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.8/src/kohlrahbi/collect_pruefis.py` & `kohlrahbi-0.0.9/src/kohlrahbi/collect_pruefis.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.8/src/kohlrahbi/read_functions.py` & `kohlrahbi-0.0.9/src/kohlrahbi/read_functions.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.8/src/kohlrahbi/row_type_checker.py` & `kohlrahbi-0.0.9/src/kohlrahbi/row_type_checker.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.8/src/kohlrahbi/seed.py` & `kohlrahbi-0.0.9/src/kohlrahbi/seed.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.8/src/kohlrahbi/ahb/ahbsubtable.py` & `kohlrahbi-0.0.9/src/kohlrahbi/ahb/ahbsubtable.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.8/src/kohlrahbi/ahb/ahbtable.py` & `kohlrahbi-0.0.9/src/kohlrahbi/ahb/ahbtable.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.8/src/kohlrahbi/ahb/ahbtablerow.py` & `kohlrahbi-0.0.9/src/kohlrahbi/ahb/ahbtablerow.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.8/src/kohlrahbi/docxtablecells/bedinungscell.py` & `kohlrahbi-0.0.9/src/kohlrahbi/docxtablecells/bedinungscell.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.8/src/kohlrahbi/docxtablecells/bodycell.py` & `kohlrahbi-0.0.9/src/kohlrahbi/docxtablecells/bodycell.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.8/src/kohlrahbi/docxtablecells/edifactstrukturcell.py` & `kohlrahbi-0.0.9/src/kohlrahbi/docxtablecells/edifactstrukturcell.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.8/src/kohlrahbi/enums/row_type.py` & `kohlrahbi-0.0.9/src/kohlrahbi/enums/row_type.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.8/src/kohlrahbi/unfoldedahb/unfoldedahbline.py` & `kohlrahbi-0.0.9/src/kohlrahbi/unfoldedahb/unfoldedahbline.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.8/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py` & `kohlrahbi-0.0.9/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py`

 * *Files 2% similar despite different names*

```diff
@@ -356,14 +356,18 @@
         with open(file_path, "w", encoding="utf-8") as file:
             json.dump(dump_data, file, ensure_ascii=False, indent=2, sort_keys=True)
         logger.info(
             "The flatahb file for %s is saved at %s",
             self.meta_data.pruefidentifikator,
             flatahb_output_directory_path / f"{self.meta_data.pruefidentifikator}.json",
         )
+        del flat_ahb
+        del dump_data
+        if "existing_flat_ahb" in locals():
+            del existing_flat_ahb
 
     def convert_to_dataframe(self) -> pd.DataFrame:
         """
         Converts the unfolded AHB to a pandas dataframe.
         """
         unfolded_ahb_lines = [
             {
```

### Comparing `kohlrahbi-0.0.8/temp/test-fobar.docx` & `kohlrahbi-0.0.9/temp/test-fobar.docx`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.8/.gitignore` & `kohlrahbi-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.8/LICENSE` & `kohlrahbi-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.8/pyproject.toml` & `kohlrahbi-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.8/PKG-INFO` & `kohlrahbi-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kohlrahbi
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tool to generate machine readable files from AHB documents
 Project-URL: Changelog, https://github.com/Hochfrequenz/kohlrahbi/releases
 Project-URL: Homepage, https://github.com/Hochfrequenz/kohlrahbi
 Author-email: Kevin Krechan <kevin.krechan@hochfrequenz.de>
 License: GPL
 License-File: LICENSE
 Keywords: ahb,automation,bdew,edi@energy
@@ -131,14 +131,16 @@
 ```
 
 You can also provide multiple prüfidentifikatoren.
 
 ```bash
 kohlrahbi --input_path ../edi_energy_mirror/edi_energy_de/current --output_path ./output/ --pruefis 11039 --pruefis 11040 --pruefi 11041 --file-type csv
 ```
+### Results
+There is a kohlrahbi based CI pipeline from the edi_energy_mirror mentioned above to the repository [machine-readable_anwendungshandbuecher](https://github.com/Hochfrequenz/machine-readable_anwendungshandbuecher) where you can find scraped AHBs as JSON, CSV or Excel files.
 
 ## Workflow
 
 ```mermaid
 flowchart TB
     S[Start] --> RD[Read docx]
     RD --> RPT[Read all paragraphs <br> and tables]
@@ -168,16 +170,16 @@
 
 ### Run all tests and linters
 
 To run the tests, you can use tox.
 
 ```bash
 tox
-See our [Python Template Repository](https://github.com/Hochfrequenz/python_template_repository#how-to-use-this-repository-on-your-machine) for detailed explanations.
 ```
+See our [Python Template Repository](https://github.com/Hochfrequenz/python_template_repository#how-to-use-this-repository-on-your-machine) for detailed explanations.
 
 ## Contribute
 
 You are very welcome to contribute to this template repository by opening a pull request against the main branch.
 
 ## Related Tools and Context
```

