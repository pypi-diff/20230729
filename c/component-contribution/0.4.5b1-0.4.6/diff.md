# Comparing `tmp/component-contribution-0.4.5b1.tar.gz` & `tmp/component-contribution-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "component-contribution-0.4.5b1.tar", last modified: Wed Oct  6 15:53:43 2021, max compression
+gzip compressed data, was "component-contribution-0.4.6.tar", last modified: Sat Jul 29 14:46:47 2023, max compression
```

## Comparing `component-contribution-0.4.5b1.tar` & `component-contribution-0.4.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 moritz    (1000) moritz    (1000)        0 2021-10-06 15:53:43.463339 component-contribution-0.4.5b1/
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     1282 2020-11-11 21:55:49.000000 component-contribution-0.4.5b1/LICENSE
--rw-rw-r--   0 moritz    (1000) moritz    (1000)      103 2020-11-11 21:55:49.000000 component-contribution-0.4.5b1/MANIFEST.in
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     3134 2021-10-06 15:53:43.463339 component-contribution-0.4.5b1/PKG-INFO
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     1707 2021-07-06 08:36:12.000000 component-contribution-0.4.5b1/README.md
--rw-rw-r--   0 moritz    (1000) moritz    (1000)      177 2020-11-11 21:55:49.000000 component-contribution-0.4.5b1/pyproject.toml
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     1955 2021-10-06 15:53:43.463339 component-contribution-0.4.5b1/setup.cfg
--rw-rw-r--   0 moritz    (1000) moritz    (1000)      195 2020-11-11 21:55:49.000000 component-contribution-0.4.5b1/setup.py
-drwxrwxr-x   0 moritz    (1000) moritz    (1000)        0 2021-10-06 15:53:43.463339 component-contribution-0.4.5b1/src/
-drwxrwxr-x   0 moritz    (1000) moritz    (1000)        0 2021-10-06 15:53:43.463339 component-contribution-0.4.5b1/src/component_contribution/
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     3004 2021-07-06 08:36:12.000000 component-contribution-0.4.5b1/src/component_contribution/__init__.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)      499 2021-10-06 15:53:43.463339 component-contribution-0.4.5b1/src/component_contribution/_version.py
-drwxrwxr-x   0 moritz    (1000) moritz    (1000)        0 2021-10-06 15:53:43.463339 component-contribution-0.4.5b1/src/component_contribution/data/
--rw-rw-r--   0 moritz    (1000) moritz    (1000)        0 2020-11-11 21:55:49.000000 component-contribution-0.4.5b1/src/component_contribution/data/__init__.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     3701 2020-11-11 21:55:49.000000 component-contribution-0.4.5b1/src/component_contribution/data/toy_training_data.csv
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     6476 2020-11-11 21:55:49.000000 component-contribution-0.4.5b1/src/component_contribution/linalg.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     4420 2021-09-29 20:35:07.000000 component-contribution-0.4.5b1/src/component_contribution/parameters.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)    19102 2021-07-06 08:36:12.000000 component-contribution-0.4.5b1/src/component_contribution/predict.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)    13507 2021-07-06 08:36:12.000000 component-contribution-0.4.5b1/src/component_contribution/preprocessor.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     8724 2020-11-11 21:55:49.000000 component-contribution-0.4.5b1/src/component_contribution/trainer.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)    26849 2021-10-06 15:04:52.000000 component-contribution-0.4.5b1/src/component_contribution/training_data.py
-drwxrwxr-x   0 moritz    (1000) moritz    (1000)        0 2021-10-06 15:53:43.463339 component-contribution-0.4.5b1/src/component_contribution.egg-info/
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     3134 2021-10-06 15:53:43.000000 component-contribution-0.4.5b1/src/component_contribution.egg-info/PKG-INFO
--rw-rw-r--   0 moritz    (1000) moritz    (1000)      788 2021-10-06 15:53:43.000000 component-contribution-0.4.5b1/src/component_contribution.egg-info/SOURCES.txt
--rw-rw-r--   0 moritz    (1000) moritz    (1000)        1 2021-10-06 15:53:43.000000 component-contribution-0.4.5b1/src/component_contribution.egg-info/dependency_links.txt
--rw-rw-r--   0 moritz    (1000) moritz    (1000)      246 2021-10-06 15:53:43.000000 component-contribution-0.4.5b1/src/component_contribution.egg-info/requires.txt
--rw-rw-r--   0 moritz    (1000) moritz    (1000)       23 2021-10-06 15:53:43.000000 component-contribution-0.4.5b1/src/component_contribution.egg-info/top_level.txt
--rw-rw-r--   0 moritz    (1000) moritz    (1000)        1 2021-08-06 12:12:45.000000 component-contribution-0.4.5b1/src/component_contribution.egg-info/zip-safe
--rw-rw-r--   0 moritz    (1000) moritz    (1000)    68611 2020-11-11 21:55:49.000000 component-contribution-0.4.5b1/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 14:46:47.155337 component-contribution-0.4.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2023-07-29 14:46:35.000000 component-contribution-0.4.6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-07-29 14:46:35.000000 component-contribution-0.4.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3064 2023-07-29 14:46:47.155337 component-contribution-0.4.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1707 2023-07-29 14:46:35.000000 component-contribution-0.4.6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-29 14:46:35.000000 component-contribution-0.4.6/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1955 2023-07-29 14:46:47.155337 component-contribution-0.4.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-07-29 14:46:35.000000 component-contribution-0.4.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 14:46:47.149336 component-contribution-0.4.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 14:46:47.155337 component-contribution-0.4.6/src/component_contribution/
+-rw-rw-rw-   0 root         (0) root         (0)     3004 2023-07-29 14:46:35.000000 component-contribution-0.4.6/src/component_contribution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-07-29 14:46:47.156337 component-contribution-0.4.6/src/component_contribution/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 14:46:47.154337 component-contribution-0.4.6/src/component_contribution/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 14:46:35.000000 component-contribution-0.4.6/src/component_contribution/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3701 2023-07-29 14:46:35.000000 component-contribution-0.4.6/src/component_contribution/data/toy_training_data.csv
+-rw-rw-rw-   0 root         (0) root         (0)     6476 2023-07-29 14:46:35.000000 component-contribution-0.4.6/src/component_contribution/linalg.py
+-rw-rw-rw-   0 root         (0) root         (0)     4420 2023-07-29 14:46:35.000000 component-contribution-0.4.6/src/component_contribution/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    21974 2023-07-29 14:46:35.000000 component-contribution-0.4.6/src/component_contribution/predict.py
+-rw-rw-rw-   0 root         (0) root         (0)    13507 2023-07-29 14:46:35.000000 component-contribution-0.4.6/src/component_contribution/preprocessor.py
+-rw-rw-rw-   0 root         (0) root         (0)     8724 2023-07-29 14:46:35.000000 component-contribution-0.4.6/src/component_contribution/trainer.py
+-rw-rw-rw-   0 root         (0) root         (0)    26829 2023-07-29 14:46:35.000000 component-contribution-0.4.6/src/component_contribution/training_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 14:46:47.154337 component-contribution-0.4.6/src/component_contribution.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3064 2023-07-29 14:46:47.000000 component-contribution-0.4.6/src/component_contribution.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      788 2023-07-29 14:46:47.000000 component-contribution-0.4.6/src/component_contribution.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 14:46:47.000000 component-contribution-0.4.6/src/component_contribution.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      283 2023-07-29 14:46:47.000000 component-contribution-0.4.6/src/component_contribution.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-29 14:46:47.000000 component-contribution-0.4.6/src/component_contribution.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 14:46:47.000000 component-contribution-0.4.6/src/component_contribution.egg-info/zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)    68611 2023-07-29 14:46:35.000000 component-contribution-0.4.6/versioneer.py
```

### Comparing `component-contribution-0.4.5b1/LICENSE` & `component-contribution-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `component-contribution-0.4.5b1/PKG-INFO` & `component-contribution-0.4.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: component-contribution
-Version: 0.4.5b1
+Version: 0.4.6
 Summary: Standard reaction Gibbs energy estimation for biochemical reactions.
 Home-page: https://gitlab.com/equilibrator/component-contribution
+Download-URL: https://pypi.org/project/component-contribution/
 Author: Elad Noor, Moritz E. Beber
 Author-email: eladn@weizmann.ac.il, midnighter@posteo.net
 License: MIT
-Download-URL: https://pypi.org/project/component-contribution/
 Project-URL: Source Code, https://gitlab.com/equilibrator/component-contribution
 Project-URL: Bug Tracker, https://gitlab.com/equilibrator/component-contribution/-/issues
 Keywords: component contribution,Gibbs energy,biochemical reaction,eQuilibrator,cache
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: development
 Provides-Extra: deployment
 License-File: LICENSE
 
 # Component Contribution
@@ -71,9 +69,7 @@
   - openbabel
   - equilibrator-assets
 
 ## Data sources
 
 * [Training data for the component contribution method](https://zenodo.org/record/3978440)
 * [Chemical group definitions for the component-contribution method](https://zenodo.org/record/4010930)
-
-
```

### Comparing `component-contribution-0.4.5b1/README.md` & `component-contribution-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `component-contribution-0.4.5b1/setup.cfg` & `component-contribution-0.4.6/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -10,18 +10,17 @@
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering :: Bio-Informatics
 	Topic :: Scientific/Engineering :: Chemistry
 license = MIT
 description = Standard reaction Gibbs energy estimation for biochemical reactions.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = 
@@ -30,47 +29,47 @@
 	biochemical reaction
 	eQuilibrator
 	cache
 
 [options]
 zip_safe = True
 install_requires = 
-	equilibrator-cache~=0.4.4b1
-	path~=15.0
-	periodictable~=1.5
+	equilibrator-cache~=0.4.6
+	path~=16.3
+	periodictable~=1.6
 	uncertainties~=3.1
-python_requires = >=3.6
+python_requires = >=3.9
 tests_require = 
 	tox
 packages = find:
 package_dir = 
 	= src
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 component_contribution.data = *.csv
 
 [options.extras_require]
 test = 
-	pytest
-	pytest-cov
-	pytest-raises
+	pytest~=7.0
+	pytest-cov~=3.0
+	pytest-raises~=0.11
+	pytest-mock~=3.7
 development = 
-	black
-	isort
-	tox
-	twine
+	black~=22.3
+	isort~=5.12
+	tox~=3.24
+	twine~=3.8
 deployment = 
 	click
 	click-log
 	python-dateutil
 	requests
-	openbabel>=3.0.0
 	equilibrator-assets
 
 [versioneer]
 VCS = git
 style = pep440
 versionfile_source = src/component_contribution/_version.py
 versionfile_build = component_contribution/_version.py
```

### Comparing `component-contribution-0.4.5b1/src/component_contribution/__init__.py` & `component-contribution-0.4.6/src/component_contribution/__init__.py`

 * *Files identical despite different names*

### Comparing `component-contribution-0.4.5b1/src/component_contribution/data/toy_training_data.csv` & `component-contribution-0.4.6/src/component_contribution/data/toy_training_data.csv`

 * *Files identical despite different names*

### Comparing `component-contribution-0.4.5b1/src/component_contribution/linalg.py` & `component-contribution-0.4.6/src/component_contribution/linalg.py`

 * *Files identical despite different names*

### Comparing `component-contribution-0.4.5b1/src/component_contribution/parameters.py` & `component-contribution-0.4.6/src/component_contribution/parameters.py`

 * *Files identical despite different names*

### Comparing `component-contribution-0.4.5b1/src/component_contribution/predict.py` & `component-contribution-0.4.6/src/component_contribution/predict.py`

 * *Files 22% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         return dg_uncertainty
 
     def standard_dgf(self, compound: Compound) -> ureg.Measurement:
         """Calculate the chemical formation energy of the major MS at pH 7.
 
         Parameters
         ----------
-        compound: Compound :
+        compound: Compound
             a compound object
 
 
         Returns
         -------
         Measurement
             a tuple of two arrays. the first is a 1D NumPy array
@@ -266,21 +266,22 @@
         """Calculate the biocheimcal formation energy of the compound.
 
         Parameters
         ----------
         compound : Compound
             a compound object
         p_h : Quantity
-            the pH
+            Set the -log10 of the proton concentration [H+].
         ionic_strength : Quantity
-            the ionic strength
+            Set the ionic strength.
         temperature : Quantity
-            temperature in Kalvin
-        p_mg : Quantity, optional
-            the pMg (Default value = default_pMg)
+            Set the temperature.
+        p_mg : Quantity
+            Set the -log10 of the magnesium ion concentration [Mg++].
+            (Default value = default_pMg)
 
 
         Returns
         -------
         type
             a tuple of two arrays. the first is a 1D NumPy array
             containing the CC estimates for the reactions' untransformed dG0
@@ -310,22 +311,23 @@
     ) -> ureg.Measurement:
         r"""Calculate the transformed reaction energies of a reaction.
 
         Parameters
         ----------
         reaction : Reaction
             the input Reaction object
-        p_h : Q_
-            pH
-        ionic_strength : Q_
-            ionic strength
-        temperature : Q_
-            temperature
-        p_mg: Q_ :
-             (Default value = default_pMg)
+        p_h : Quantity
+            Set the -log10 of the proton concentration [H+].
+        ionic_strength : Quantity
+            Set the ionic strength.
+        temperature : Quantity
+            Set the temperature.
+        p_mg : Quantity
+            Set the -log10 of the magnesium ion concentration [Mg++].
+            (Default value = default_pMg)
 
         Returns
         -------
         standard_dg : Measurement
             the :math:`\Delta G'` in kJ/mol and standard error. to
             calculate the 95% confidence interval, multiply the error by 1.96
 
@@ -349,20 +351,21 @@
         r"""Calculate the transformed reaction energies of a list of reactions.
 
         Parameters
         ----------
         reactions : List[Reaction]
             a list of Reaction objects
         p_h : Quantity
-            the pH
+            Set the -log10 of the proton concentration [H+].
         ionic_strength : Quantity
-            the ionic strength
+            Set the ionic strength.
         temperature : Quantity
-            the temperature
-        p_mg: Quantity, optional
+            Set the temperature.
+        p_mg : Quantity
+            Set the -log10 of the magnesium ion concentration [Mg++].
             (Default value = default_pMg)
 
         Returns
         -------
         standard_dg_prime : np.ndarray
             the array of Component Contribution estimates for the reactions'
             :math:`\Delta G'` in kJ/mol
@@ -535,7 +538,89 @@
         Returns
         -------
         bool
             True if the reaction require group contributions.
 
         """
         return self.preprocess.is_using_group_contribution(reaction)
+
+    @ureg.check(None, None, "", "[concentration]", "[temperature]", "")
+    def dgf_prime_sensitivity_to_p_h(
+        self,
+        compound: Compound,
+        p_h: Q_,
+        ionic_strength: Q_,
+        temperature: Q_,
+        p_mg: Q_ = default_pMg,
+    ) -> ureg.Measurement:
+        r"""Calculate the derivative of the reaction ΔG' w.r.t. pH.
+
+        By derivating the Legendre transform as a function of pH, we get
+        the slope which is a linear approximation of the pH response.
+
+        Parameters
+        ----------
+        compound : Compound
+            a compound object
+        p_h : Quantity
+            Set the -log10 of the proton concentration [H+].
+        ionic_strength : Quantity
+            Set the ionic strength.
+        temperature : Quantity
+            Set the temperature.
+        p_mg : Quantity
+            Set the -log10 of the magnesium ion concentration [Mg++].
+            (Default value = default_pMg)
+
+        Returns
+        -------
+        Quantity
+            The derivative of  :math:`\Delta G_r` with respect to pH.
+
+        """
+        return compound.sensitivity_to_p_h(
+            p_h=p_h,
+            ionic_strength=ionic_strength,
+            temperature=temperature,
+            p_mg=p_mg,
+        )
+
+    @ureg.check(None, None, "", "[concentration]", "[temperature]", "")
+    def dg_prime_sensitivity_to_p_h(
+        self,
+        reaction: Reaction,
+        p_h: Q_,
+        ionic_strength: Q_,
+        temperature: Q_,
+        p_mg: Q_ = default_pMg,
+    ) -> Q_:
+        r"""Calculate the derivative of the reaction ΔG' w.r.t. pH.
+
+        By derivating the Legendre transform as a function of pH, we get
+        the slope which is a linear approximation of the pH response.
+
+        Parameters
+        ----------
+        reaction : Reaction
+            the input Reaction object
+        p_h : Quantity
+            Set the -log10 of the proton concentration [H+].
+        ionic_strength : Quantity
+            Set the ionic strength.
+        temperature : Quantity
+            Set the temperature.
+        p_mg : Quantity
+            Set the -log10 of the magnesium ion concentration [Mg++].
+            (Default value = default_pMg)
+
+        Returns
+        -------
+        Quantity
+            The derivative of  :math:`\Delta G_r` with respect to pH.
+
+        """
+        return reaction.sensitivity_to_p_h(
+            p_h=p_h,
+            ionic_strength=ionic_strength,
+            temperature=temperature,
+            p_mg=p_mg,
+        )
```

### Comparing `component-contribution-0.4.5b1/src/component_contribution/preprocessor.py` & `component-contribution-0.4.6/src/component_contribution/preprocessor.py`

 * *Files identical despite different names*

### Comparing `component-contribution-0.4.5b1/src/component_contribution/trainer.py` & `component-contribution-0.4.6/src/component_contribution/trainer.py`

 * *Files identical despite different names*

### Comparing `component-contribution-0.4.5b1/src/component_contribution/training_data.py` & `component-contribution-0.4.6/src/component_contribution/training_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -406,15 +406,15 @@
         for col, unit in [
             ("standard_dg_prime", "kJ/mol"),
             ("ionic_strength", "M"),
             ("temperature", "K"),
             ("p_h", None),
             ("p_mg", None),
         ]:
-            reaction_df[col] = reaction_df[col].apply(lambda x: Q_(x, unit))
+            reaction_df[col] = reaction_df[col].apply(Q_, args=(unit,))
 
         non_decomposable_compounds = set()
 
         return TrainingData(
             self.ccache,
             groups,
             reaction_df,
@@ -522,15 +522,15 @@
         for col, unit in [
             ("K_prime", None),
             ("ionic_strength", "M"),
             ("temperature", "K"),
             ("p_h", None),
             ("p_mg", None),
         ]:
-            tecr_df[col] = tecr_df[col].apply(lambda x: Q_(x, unit))
+            tecr_df[col] = tecr_df[col].apply(Q_, args=(unit,))
 
         # calculate the dG'0 from the Keq and T
         standard_dg_primes = [
             (-R * row.temperature * np.log(row.K_prime)).to("kJ/mol")
             for row in tecr_df.itertuples()
         ]
         tecr_df = tecr_df.assign(
@@ -618,15 +618,15 @@
         for col, unit in [
             ("standard_dg_prime", "kJ/mol"),
             ("ionic_strength", "M"),
             ("temperature", "K"),
             ("p_h", None),
             ("p_mg", None),
         ]:
-            formation_df[col] = formation_df[col].apply(lambda x: Q_(x, unit))
+            formation_df[col] = formation_df[col].apply(Q_, args=(unit,))
 
         formation_df = formation_df.assign(
             **{
                 "reaction": compounds[mask_formation].apply(
                     lambda c: Reaction({c: 1})
                 ),
                 "balance": False,
@@ -659,15 +659,15 @@
         for col, unit in [
             ("standard_E_prime", "V"),
             ("ionic_strength", "M"),
             ("temperature", "K"),
             ("p_h", None),
             ("p_mg", None),
         ]:
-            redox_df[col] = redox_df[col].apply(lambda x: Q_(x, unit))
+            redox_df[col] = redox_df[col].apply(Q_, args=(unit,))
 
         compounds_ox = pd.Series(index=redox_df.index, dtype=object)
         mask = redox_df["inchi_key_ox"].notnull()
         logger.info(
             "Parsing %d/%d oxidized compounds with InChIKey.",
             mask.sum(),
             len(mask),
```

### Comparing `component-contribution-0.4.5b1/src/component_contribution.egg-info/PKG-INFO` & `component-contribution-0.4.6/src/component_contribution.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: component-contribution
-Version: 0.4.5b1
+Version: 0.4.6
 Summary: Standard reaction Gibbs energy estimation for biochemical reactions.
 Home-page: https://gitlab.com/equilibrator/component-contribution
+Download-URL: https://pypi.org/project/component-contribution/
 Author: Elad Noor, Moritz E. Beber
 Author-email: eladn@weizmann.ac.il, midnighter@posteo.net
 License: MIT
-Download-URL: https://pypi.org/project/component-contribution/
 Project-URL: Source Code, https://gitlab.com/equilibrator/component-contribution
 Project-URL: Bug Tracker, https://gitlab.com/equilibrator/component-contribution/-/issues
 Keywords: component contribution,Gibbs energy,biochemical reaction,eQuilibrator,cache
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: development
 Provides-Extra: deployment
 License-File: LICENSE
 
 # Component Contribution
@@ -71,9 +69,7 @@
   - openbabel
   - equilibrator-assets
 
 ## Data sources
 
 * [Training data for the component contribution method](https://zenodo.org/record/3978440)
 * [Chemical group definitions for the component-contribution method](https://zenodo.org/record/4010930)
-
-
```

### Comparing `component-contribution-0.4.5b1/src/component_contribution.egg-info/SOURCES.txt` & `component-contribution-0.4.6/src/component_contribution.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `component-contribution-0.4.5b1/versioneer.py` & `component-contribution-0.4.6/versioneer.py`

 * *Files identical despite different names*

