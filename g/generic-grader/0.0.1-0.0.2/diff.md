# Comparing `tmp/generic_grader-0.0.1.tar.gz` & `tmp/generic_grader-0.0.2.tar.gz`

## Comparing `generic_grader-0.0.1.tar` & `generic_grader-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,12 @@
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 generic_grader-0.0.1/temp.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 generic_grader-0.0.1/src/__init__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 generic_grader-0.0.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 generic_grader-0.0.1/LICENSE
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 generic_grader-0.0.1/README.md
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 generic_grader-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 generic_grader-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 generic_grader-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 generic_grader-0.0.2/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 generic_grader-0.0.2/generic_grader/__init__.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 generic_grader-0.0.2/generic_grader/file/file_presence.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 generic_grader-0.0.2/generic_grader/utils/options.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 generic_grader-0.0.2/tests/test_file.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 generic_grader-0.0.2/tests/test_options.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 generic_grader-0.0.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 generic_grader-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 generic_grader-0.0.2/README.md
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 generic_grader-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 generic_grader-0.0.2/PKG-INFO
```

### Comparing `generic_grader-0.0.1/LICENSE` & `generic_grader-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `generic_grader-0.0.1/README.md` & `generic_grader-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -73,15 +73,15 @@
    pre-commit install
    ```
 
 7. Install the package.  Note that this installs the package as editable, so
    edits will be automatically reflected in the installed package.
 
    ``` bash
-   pip install -e .[code_style]
+   pip install -e .[dev]
    ```
 
 8. Run the tests.
 
    ``` bash
    pytest
    ```
```

### Comparing `generic_grader-0.0.1/PKG-INFO` & `generic_grader-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 Metadata-Version: 2.1
 Name: generic-grader
-Version: 0.0.1
+Version: 0.0.2
 Summary: A collection of parameterizable tests for automatic grading.
 Project-URL: Homepage, https://github.com/Purdue-EBEC/generic-grader
 Project-URL: Bug Tracker, https://github.com/Purdue-EBEC/generic-grader/issues
 Author-email: John Cole <jhcole@purdue.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
+Requires-Dist: gradescope-utils<1,>=0.5.0
+Requires-Dist: matplotlib<4,>=3.7.0
+Requires-Dist: parameterized<1,>=0.8.1
+Requires-Dist: pillow<10,>=9.4.0
+Requires-Dist: pytesseract<1,>=0.3.10
+Requires-Dist: python-dateutil<3,>=2.8.2
+Requires-Dist: pytz==2022.7.1
+Requires-Dist: rapidfuzz<4,>=3.1.1
+Requires-Dist: scipy<2,>=1.10.1
 Provides-Extra: dev
 Requires-Dist: build; extra == 'dev'
 Requires-Dist: pre-commit~=3.0; extra == 'dev'
 Requires-Dist: twine; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # Generic Grader
@@ -91,15 +100,15 @@
    pre-commit install
    ```
 
 7. Install the package.  Note that this installs the package as editable, so
    edits will be automatically reflected in the installed package.
 
    ``` bash
-   pip install -e .[code_style]
+   pip install -e .[dev]
    ```
 
 8. Run the tests.
 
    ``` bash
    pytest
    ```
```

