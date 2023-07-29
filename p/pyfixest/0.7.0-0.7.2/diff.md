# Comparing `tmp/pyfixest-0.7.0.tar.gz` & `tmp/pyfixest-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfixest-0.7.0.tar", max compression
+gzip compressed data, was "pyfixest-0.7.2.tar", max compression
```

## Comparing `pyfixest-0.7.0.tar` & `pyfixest-0.7.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1096 2022-11-19 12:53:04.921992 pyfixest-0.7.0/LICENSE.md
--rw-r--r--   0        0        0       26 2023-03-16 21:51:51.234748 pyfixest-0.7.0/pyfixest/__init__.py
--rw-r--r--   0        0        0     4450 2023-07-14 20:18:32.655093 pyfixest-0.7.0/pyfixest/demean.py
--rw-r--r--   0        0        0      669 2023-07-18 09:46:04.593817 pyfixest-0.7.0/pyfixest/exceptions.py
--rw-r--r--   0        0        0    23413 2023-07-18 10:38:25.626648 pyfixest-0.7.0/pyfixest/feols.py
--rw-r--r--   0        0        0    43168 2023-07-18 10:29:24.099434 pyfixest-0.7.0/pyfixest/fixest.py
--rw-r--r--   0        0        0    17641 2023-07-18 10:25:33.991093 pyfixest-0.7.0/pyfixest/FormulaParser.py
--rw-r--r--   0        0        0     3426 2023-04-27 19:03:35.062476 pyfixest-0.7.0/pyfixest/ssc_utils.py
--rw-r--r--   0        0        0     1312 2023-06-04 20:23:04.808444 pyfixest-0.7.0/pyfixest/utils.py
--rw-r--r--   0        0        0      939 2023-07-18 10:39:16.952418 pyfixest-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2617 2023-06-04 20:23:08.766777 pyfixest-0.7.0/readme.md
--rw-r--r--   0        0        0     3573 1970-01-01 00:00:00.000000 pyfixest-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1096 2022-11-19 12:53:04.921992 pyfixest-0.7.2/LICENSE.md
+-rw-r--r--   0        0        0       26 2023-03-16 21:51:51.234748 pyfixest-0.7.2/pyfixest/__init__.py
+-rw-r--r--   0        0        0     4450 2023-07-18 14:22:36.978128 pyfixest-0.7.2/pyfixest/demean.py
+-rw-r--r--   0        0        0      669 2023-07-29 18:02:45.424719 pyfixest-0.7.2/pyfixest/exceptions.py
+-rw-r--r--   0        0        0    23413 2023-07-29 18:02:45.425729 pyfixest-0.7.2/pyfixest/feols.py
+-rw-r--r--   0        0        0    43175 2023-07-29 18:03:32.047645 pyfixest-0.7.2/pyfixest/fixest.py
+-rw-r--r--   0        0        0    17641 2023-07-18 14:22:36.974477 pyfixest-0.7.2/pyfixest/FormulaParser.py
+-rw-r--r--   0        0        0     3426 2023-04-27 19:03:35.062476 pyfixest-0.7.2/pyfixest/ssc_utils.py
+-rw-r--r--   0        0        0     1312 2023-07-29 18:02:45.427468 pyfixest-0.7.2/pyfixest/utils.py
+-rw-r--r--   0        0        0      939 2023-07-29 18:05:57.186682 pyfixest-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     2320 2023-07-18 14:22:36.983620 pyfixest-0.7.2/readme.md
+-rw-r--r--   0        0        0     3317 1970-01-01 00:00:00.000000 pyfixest-0.7.2/PKG-INFO
```

### Comparing `pyfixest-0.7.0/LICENSE.md` & `pyfixest-0.7.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyfixest-0.7.0/pyfixest/demean.py` & `pyfixest-0.7.2/pyfixest/demean.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.7.0/pyfixest/exceptions.py` & `pyfixest-0.7.2/pyfixest/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.7.0/pyfixest/feols.py` & `pyfixest-0.7.2/pyfixest/feols.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.7.0/pyfixest/fixest.py` & `pyfixest-0.7.2/pyfixest/fixest.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         A class for fixed effects regression modeling.
         Args:
             data: The input pd.DataFrame for the object.
         Returns:
             None
         '''
 
-        self.data = data
+        self.data = data.copy()
         self.all_fitted_models = dict()
 
 
     def feols(self, fml: str, vcov: Union[None, str, Dict[str, str]] = None, ssc=ssc(), fixef_rm: str = "none") -> None:
         '''
         Method for fixed effects regression modeling using the PyHDFE package for projecting out fixed effects.
         Args:
```

### Comparing `pyfixest-0.7.0/pyfixest/FormulaParser.py` & `pyfixest-0.7.2/pyfixest/FormulaParser.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.7.0/pyfixest/ssc_utils.py` & `pyfixest-0.7.2/pyfixest/ssc_utils.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.7.0/pyfixest/utils.py` & `pyfixest-0.7.2/pyfixest/utils.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.7.0/pyproject.toml` & `pyfixest-0.7.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyfixest"
-version = "0.7.0"
+version = "0.7.2"
 
 description = "Experimental draft package for high dimensional fixed effect estimation. Supports OLS and IV estimation."
 authors = ["Alexander Fischer <alexander-fischer1801@t-online.de>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://s3alfisc.github.io/pyfixest/"
 repository = "https://github.com/s3alfisc/pyfixest"
```

