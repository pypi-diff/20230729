# Comparing `tmp/meeko-0.4.0.tar.gz` & `tmp/meeko-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meeko-0.4.0.tar", last modified: Mon Nov 14 22:58:15 2022, max compression
+gzip compressed data, was "meeko-0.5.0.tar", last modified: Fri Jul 28 23:51:34 2023, max compression
```

## Comparing `meeko-0.4.0.tar` & `meeko-0.5.0.tar`

### file list

```diff
@@ -1,48 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 22:58:15.814569 meeko-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)    26526 2022-11-14 22:58:07.000000 meeko-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     9913 2022-11-14 22:58:15.814569 meeko-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8652 2022-11-14 22:58:07.000000 meeko-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 22:58:15.810569 meeko-0.4.0/meeko/
--rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-11-14 22:58:07.000000 meeko-0.4.0/meeko/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 22:58:15.814569 meeko-0.4.0/meeko/analysis/
--rw-r--r--   0 runner    (1001) docker     (121)      413 2022-11-14 22:58:07.000000 meeko-0.4.0/meeko/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4694 2022-11-14 22:58:07.000000 meeko-0.4.0/meeko/analysis/fingerprint_interactions.py
--rw-r--r--   0 runner    (1001) docker     (121)    11922 2022-11-14 22:58:07.000000 meeko-0.4.0/meeko/analysis/interactions.py
--rw-r--r--   0 runner    (1001) docker     (121)    12562 2022-11-14 22:58:07.000000 meeko-0.4.0/meeko/atomtyper.py
--rw-r--r--   0 runner    (1001) docker     (121)     3323 2022-11-14 22:58:07.000000 meeko-0.4.0/meeko/bondtyper.py
--rw-r--r--   0 runner    (1001) docker     (121)     9317 2022-11-14 22:58:07.000000 meeko-0.4.0/meeko/covalentbuilder.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 22:58:15.814569 meeko-0.4.0/meeko/data/
--rw-r--r--   0 runner    (1001) docker     (121)     2568 2022-11-14 22:58:07.000000 meeko-0.4.0/meeko/data/atomtypes.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2421 2022-11-14 22:58:07.000000 meeko-0.4.0/meeko/data/pi_non_aromatic.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5187 2022-11-14 22:58:07.000000 meeko-0.4.0/meeko/data/waterfield.txt
--rw-r--r--   0 runner    (1001) docker     (121)    12329 2022-11-14 22:58:07.000000 meeko-0.4.0/meeko/flexibility.py
--rw-r--r--   0 runner    (1001) docker     (121)     8597 2022-11-14 22:58:07.000000 meeko-0.4.0/meeko/hydrate.py
--rw-r--r--   0 runner    (1001) docker     (121)    10517 2022-11-14 22:58:07.000000 meeko-0.4.0/meeko/macrocycle.py
--rw-r--r--   0 runner    (1001) docker     (121)    30470 2022-11-14 22:58:07.000000 meeko-0.4.0/meeko/molecule_pdbqt.py
--rw-r--r--   0 runner    (1001) docker     (121)    28817 2022-11-14 22:58:07.000000 meeko-0.4.0/meeko/molsetup.py
--rw-r--r--   0 runner    (1001) docker     (121)    10418 2022-11-14 22:58:07.000000 meeko-0.4.0/meeko/preparation.py
--rw-r--r--   0 runner    (1001) docker     (121)    14592 2022-11-14 22:58:07.000000 meeko-0.4.0/meeko/rdkit_mol_create.py
--rw-r--r--   0 runner    (1001) docker     (121)     8086 2022-11-14 22:58:07.000000 meeko-0.4.0/meeko/receptor_pdbqt.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 22:58:15.814569 meeko-0.4.0/meeko/utils/
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-14 22:58:07.000000 meeko-0.4.0/meeko/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      775 2022-11-14 22:58:07.000000 meeko-0.4.0/meeko/utils/autodock4_atom_types_elements.py
--rw-r--r--   0 runner    (1001) docker     (121)     2187 2022-11-14 22:58:07.000000 meeko-0.4.0/meeko/utils/covalent_radius_table.py
--rw-r--r--   0 runner    (1001) docker     (121)    14086 2022-11-14 22:58:07.000000 meeko-0.4.0/meeko/utils/geomutils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4408 2022-11-14 22:58:07.000000 meeko-0.4.0/meeko/utils/obutils.py
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-11-14 22:58:07.000000 meeko-0.4.0/meeko/utils/pdbutils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2664 2022-11-14 22:58:07.000000 meeko-0.4.0/meeko/utils/rdkitutils.py
--rw-r--r--   0 runner    (1001) docker     (121)    13324 2022-11-14 22:58:07.000000 meeko-0.4.0/meeko/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2194 2022-11-14 22:58:07.000000 meeko-0.4.0/meeko/utils/van_der_waals_radius_table.py
--rw-r--r--   0 runner    (1001) docker     (121)     9320 2022-11-14 22:58:07.000000 meeko-0.4.0/meeko/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 22:58:15.810569 meeko-0.4.0/meeko.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9913 2022-11-14 22:58:15.000000 meeko-0.4.0/meeko.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      966 2022-11-14 22:58:15.000000 meeko-0.4.0/meeko.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 22:58:15.000000 meeko-0.4.0/meeko.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 22:58:15.000000 meeko-0.4.0/meeko.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-14 22:58:15.000000 meeko-0.4.0/meeko.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-14 22:58:15.000000 meeko-0.4.0/meeko.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 22:58:15.814569 meeko-0.4.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)     4668 2022-11-14 22:58:07.000000 meeko-0.4.0/scripts/mk_export.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    15197 2022-11-14 22:58:07.000000 meeko-0.4.0/scripts/mk_prepare_ligand.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-14 22:58:15.814569 meeko-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2348 2022-11-14 22:58:07.000000 meeko-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:51:34.266871 meeko-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-07-28 23:51:26.000000 meeko-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13459 2023-07-28 23:51:34.266871 meeko-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12200 2023-07-28 23:51:26.000000 meeko-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:51:34.262871 meeko-0.5.0/meeko/
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-28 23:51:26.000000 meeko-0.5.0/meeko/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:51:34.262871 meeko-0.5.0/meeko/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-28 23:51:26.000000 meeko-0.5.0/meeko/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-07-28 23:51:26.000000 meeko-0.5.0/meeko/analysis/fingerprint_interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-07-28 23:51:26.000000 meeko-0.5.0/meeko/analysis/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13020 2023-07-28 23:51:26.000000 meeko-0.5.0/meeko/atomtyper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-28 23:51:26.000000 meeko-0.5.0/meeko/bondtyper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-07-28 23:51:26.000000 meeko-0.5.0/meeko/covalentbuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:51:34.262871 meeko-0.5.0/meeko/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-07-28 23:51:26.000000 meeko-0.5.0/meeko/data/atomtypes.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-07-28 23:51:26.000000 meeko-0.5.0/meeko/data/flexres_templates.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-28 23:51:26.000000 meeko-0.5.0/meeko/data/pi_non_aromatic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   205550 2023-07-28 23:51:26.000000 meeko-0.5.0/meeko/data/residue_params.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-07-28 23:51:26.000000 meeko-0.5.0/meeko/data/waterfield.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12542 2023-07-28 23:51:26.000000 meeko-0.5.0/meeko/flexibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-07-28 23:51:26.000000 meeko-0.5.0/meeko/gridbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8597 2023-07-28 23:51:26.000000 meeko-0.5.0/meeko/hydrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-07-28 23:51:26.000000 meeko-0.5.0/meeko/macrocycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32118 2023-07-28 23:51:26.000000 meeko-0.5.0/meeko/molecule_pdbqt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30707 2023-07-28 23:51:26.000000 meeko-0.5.0/meeko/molsetup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10129 2023-07-28 23:51:26.000000 meeko-0.5.0/meeko/preparation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-07-28 23:51:26.000000 meeko-0.5.0/meeko/rdkit_mol_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-07-28 23:51:26.000000 meeko-0.5.0/meeko/reactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19881 2023-07-28 23:51:26.000000 meeko-0.5.0/meeko/receptor_pdbqt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:51:34.266871 meeko-0.5.0/meeko/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-28 23:51:26.000000 meeko-0.5.0/meeko/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-28 23:51:26.000000 meeko-0.5.0/meeko/utils/autodock4_atom_types_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-28 23:51:26.000000 meeko-0.5.0/meeko/utils/covalent_radius_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14086 2023-07-28 23:51:26.000000 meeko-0.5.0/meeko/utils/geomutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-07-28 23:51:26.000000 meeko-0.5.0/meeko/utils/obutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-28 23:51:26.000000 meeko-0.5.0/meeko/utils/pdbutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-28 23:51:26.000000 meeko-0.5.0/meeko/utils/rdkitutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13324 2023-07-28 23:51:26.000000 meeko-0.5.0/meeko/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-28 23:51:26.000000 meeko-0.5.0/meeko/utils/van_der_waals_radius_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11882 2023-07-28 23:51:26.000000 meeko-0.5.0/meeko/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:51:34.262871 meeko-0.5.0/meeko.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13459 2023-07-28 23:51:34.000000 meeko-0.5.0/meeko.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-28 23:51:34.000000 meeko-0.5.0/meeko.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 23:51:34.000000 meeko-0.5.0/meeko.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 23:51:34.000000 meeko-0.5.0/meeko.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 23:51:34.000000 meeko-0.5.0/meeko.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-28 23:51:34.000000 meeko-0.5.0/meeko.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:51:34.266871 meeko-0.5.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5377 2023-07-28 23:51:26.000000 meeko-0.5.0/scripts/mk_export.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18588 2023-07-28 23:51:26.000000 meeko-0.5.0/scripts/mk_prepare_ligand.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18906 2023-07-28 23:51:26.000000 meeko-0.5.0/scripts/mk_prepare_receptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 23:51:34.266871 meeko-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-07-28 23:51:26.000000 meeko-0.5.0/setup.py
```

### Comparing `meeko-0.4.0/LICENSE` & `meeko-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meeko-0.4.0/PKG-INFO` & `meeko-0.5.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,66 @@
-Metadata-Version: 2.1
-Name: meeko
-Version: 0.4.0
-Summary: Python package for preparing small molecule for docking
-Home-page: https://github.com/ccsb-scripps/meeko
-Author: Forli Lab
-Author-email: forli@scripps.edu
-License: LGPL-2.1
-Keywords: molecular modeling,drug design,docking,autodock
-Classifier: Environment :: Console
-Classifier: Environment :: Other Environment
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: OS Independent
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: C++
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Topic :: Scientific/Engineering :: Chemistry
-Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.5.*
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Meeko: preparation of small molecules for AutoDock
 
-[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![API stability](https://img.shields.io/badge/stable%20API-no-orange)](https://shields.io/)
-[![PyPI version fury.io](https://img.shields.io/badge/version-0.4.0-green.svg)](https://pypi.python.org/pypi/ansicolortags/)
+[![PyPI version fury.io](https://img.shields.io/badge/version-0.5.0-green.svg)](https://pypi.python.org/pypi/ansicolortags/)
 
 Meeko reads an RDKit molecule object and writes a PDBQT string (or file)
 for [AutoDock-Vina](https://github.com/ccsb-scripps/AutoDock-Vina)
 and [AutoDock-GPU](https://github.com/ccsb-scripps/AutoDock-GPU).
 It converts the docking output to RDKit molecules and
 SD files, without loss of bond orders.
 
 Meeko is developed by the [Forli lab](https://forlilab.org/) at the
 [Center for Computational Structural Biology (CCSB)](https://ccsb.scripps.edu)
 at [Scripps Research](https://www.scripps.edu/).
 
+
 ## Usage notes
+
 Meeko does not calculate 3D coordinates or assign protonation states.
 Input molecules must have explicit hydrogens.
 
 Sampling of macrocycle conformers ([paper](https://doi.org/10.1017/qrd.2022.18))
 is enabled by default.
 
-## Recent changes
+SDF format strongly preferred over Mol2.
+See
+[this discussion](https://github.com/rdkit/rdkit/discussions/3647)
+and RDKit issues
+[1755](https://github.com/rdkit/rdkit/issues/1755) and
+[917](https://github.com/rdkit/rdkit/issues/917).
 
-The Python API for creating RDKit molecules from docking results changed in `v0.4.0`.
-See [example below](#2.-rdkit-molecule-from-docking-results).
 
-The `--pH` option was removed since `v0.3.0`. See issue https://github.com/forlilab/Meeko/issues/11 for more info.
+## API changes in v0.5
+
+Class `MoleculePreparation` no longer has method `write_pdbqt_string()`.
+Instead, `MoleculePreparation.prepare()` returns a list of `MoleculeSetup` objects
+that must be passed, individually, to `PDBQTWriterLegacy.write_string()`.
+```python
+from meeko import MoleculePreparation
+from meeko import PDBQTWriterLegacy
+
+preparator = MoleculePreparation()
+mol_setups = preparator.prepare(rdkit_molecule_3D_with_Hs)
+for setup in mol_setups:
+    pdbqt_string, is_ok, error_msg = PDBQTWriterLegacy.write_string(setup)
+    if is_ok:
+        print(pdbqt_string, end="")
+```
+
+Argument `keep_nonpolar_hydrogens` is replaced by `merge_these_atom_types`, both in the Python
+interface and for script `mk_prepare_ligand.py`.
+The default is `merge_these_atom_types=("H",)`, which
+merges hydrogens typed `"H"`, keeping the current default behavior.
+To keep all hydrogens, set `merge_these_atom_types` to an empty
+list when initializing `MoleculePreparation`, or pass no atom types
+to `--merge_these_atom_types` from the command line:
+```sh
+mk_prepare_ligand.py -i molecule.sdf --merge_these_atom_types
+``` 
 
 ## Dependencies
 
 * Python (>=3.5)
 * Numpy
 * Scipy
 * RDKit
@@ -94,15 +93,15 @@
 ```
 
 
 ## Examples using the command line scripts
 
 #### 1. make PDBQT files
 AutoDock-GPU and Vina read molecules in the PDBQT format. These can be prepared
-by Meeko from SD files, or from Mol2 files, but SDF is preferred.
+by Meeko from SD files, or from Mol2 files, but SDF is strongly preferred.
 ```console
 mk_prepare_ligand.py -i molecule.sdf -o molecule.pdbqt
 mk_prepare_ligand.py -i multi_mol.sdf --multimol_outdir folder_for_pdbqt_files
 ```
 
 #### 2. convert docking results to SDF
 AutoDock-GPU and Vina write docking results in the PDBQT format. The DLG output
@@ -130,24 +129,26 @@
 
 ## Python tutorial
 
 #### 1. making PDBQT strings for Vina or for AutoDock-GPU
 
 ```python
 from meeko import MoleculePreparation
+from meeko import PDBQTWriterLegacy
 from rdkit import Chem
 
 input_molecule_file = "example/BACE_macrocycle/BACE_4.sdf"
 
 # there is one molecule in this SD file, this loop iterates just once
 for mol in Chem.SDMolSupplier(input_molecule_file, removeHs=False):
     preparator = MoleculePreparation()
-    preparator.prepare(mol)
-    preparator.show_setup() # optional
-    pdbqt_string = preparator.write_pdbqt_string()
+    mol_setups = preparator.prepare(mol)
+    for setup in mol_setups:
+        setup.show() # optional
+        pdbqt_string = PDBQTWriterLegacy.write_string(setup)
 ```
 At this point, `pdbqt_string` can be written to a file for
 docking with AutoDock-GPU or Vina, or passed directly to Vina within Python
 using `set_ligand_from_string(pdbqt_string)`. For context, see
 [the docs on using Vina from Python](https://autodock-vina.readthedocs.io/en/latest/docking_python.html).
 
 
@@ -259,7 +260,70 @@
     -i ligand_including_cys_sidechain.sdf\
     --receptor protein.pdb\
     --rec_residue ":CYS:6"\
     --tether_smarts "NC(=O)C(O)(C)SCC"\
     --tether_smarts_indices 9 8\
     -o prepared.pdbqt
 ```
+
+## Reactive Docking
+
+### 1. Prepare protein with waterkit
+Follow `wk_prepare_receptor.py` instructions and run with `--pdb`.
+The goal of this step is to perform essential fixes to the protein
+(such as missing atoms), to add hydrogens, and to follow the Amber
+naming scheme for atoms and residues, e.g., `HIE` or `HID`
+instead of `HIS`.
+
+### 2. Prepare protein pdbqt
+Here, `wk.pdb` was written by waterkit.
+Here, `wk.pdb` was written by waterkit. The example below will center a gridbox of specified size on the given reactive residue.
+
+```console
+   $ mk_prepare_receptor.py\
+    --pdb wk.pdb\
+    -o receptor.pdbqt\
+    --flexres " :ARG:348"\
+    --reactive_flexres " :SER:308"
+    --reactive_flexres " :SER:308"\
+    --box_center_on_reactive_res\
+    --box_size 40 40 40  # x y z (angstroms)
+```
+A manual box center can be specified with `--box_center`.
+Reactive parameters can also be modified:
+```sh
+  --r_eq_12 R_EQ_12     r_eq for reactive atoms (1-2 interaction)
+  --eps_12 EPS_12       epsilon for reactive atoms (1-2 interaction)
+  --r_eq_13_scaling R_EQ_13_SCALING
+                        r_eq scaling for 1-3 interaction across reactive atoms
+  --r_eq_14_scaling R_EQ_14_SCALING
+                        r_eq scaling for 1-4 interaction across reactive atoms
+```
+
+Receptor preparation can't handle heteroatoms for the moment.
+Also nucleic acids, ions, and post-translational modifications (e.g.
+phosphorilation) are not supported. Only the 20 standard amino acids
+can be parsed, and it is required to have Amber atom names and
+hydrogens. No atoms can be missing.
+
+### 3. Run autogrid
+
+Make affinity maps for the `_rigid.pdbqt` part of the receptor.
+Make affinity maps for the `_rigid.pdbqt` part of the receptor. `mk_prepare_receptor.py` will prepare the GPF for you.
+
+### 4. Write ligand PDBQT
+mk_prepare_ligand.py -i sufex1.sdf --reactive_smarts "S(=O)(=O)F" --reactive_smarts_idx 1 -o sufex1.pdbqt\
+
+### 5. Configure AD-GPU for reactive docking
+
+For reactive docking there are two options that need to be passed to AutoDock-GPU:
+For reactive docking there are an additional option that needs to be passed to AutoDock-GPU:
+    ```console
+    --import_dpf
+    ```
+
+The `--derivtype` option, if needed, was written by `mk_prepare_receptor.py` to a file suffixed with `.derivtype`.
+
+The filename to be passed to `--import_dpf` was written by `mk_prepare_receptor.py`
+and it is suffixed with `reactive_config`.
+```sh
+ADGPU -I *.reactive_config -L sufex1.pdbqt -N sufex1_docked_ -F *_flex.pdbqt -C 1
```

### Comparing `meeko-0.4.0/meeko/__init__.py` & `meeko-0.5.0/meeko/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
 # Meeko
 #
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 
 try:
     import openbabel
 except ImportError:
     _has_openbabel = False
 else:
     _has_openbabel = True
@@ -26,20 +26,28 @@
 from .utils import pdbutils
 from .utils import geomutils
 from .utils import utils
 from .atomtyper import AtomTyper
 from .receptor_pdbqt import PDBQTReceptor
 from .molecule_pdbqt import PDBQTMolecule
 from .rdkit_mol_create import RDKitMolCreate
+from .reactive import reactive_typer
+from .reactive import get_reactive_config
+from .writer import PDBQTWriterLegacy
 from . import analysis
 
 __all__ = ['MoleculePreparation', 'RDKitMoleculeSetup',
         'pdbutils', 'geomutils', 'rdkitutils', 'utils',
         'AtomTyper', 'PDBQTMolecule', 'PDBQTReceptor', 'analysis',
-        'RDKitMolCreate']
+        'RDKitMolCreate',
+        'PDBQTWriterLegacy',
+        'reactive_typer',
+        'get_reactive_config',
+        'gridbox',
+]
 
 if _has_openbabel:
     from .molsetup import OBMoleculeSetup
     from .utils import obutils
     __all__.append("OBMoleculeSetup")
     __all__.append("obutils")
```

### Comparing `meeko-0.4.0/meeko/analysis/fingerprint_interactions.py` & `meeko-0.5.0/meeko/analysis/fingerprint_interactions.py`

 * *Files identical despite different names*

### Comparing `meeko-0.4.0/meeko/analysis/interactions.py` & `meeko-0.5.0/meeko/analysis/interactions.py`

 * *Files identical despite different names*

### Comparing `meeko-0.4.0/meeko/atomtyper.py` & `meeko-0.5.0/meeko/atomtyper.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # -*- coding: utf-8 -*-
 #
 # Meeko atom typer
 #
 
 import os
 import json
-from collections import OrderedDict
 
 import numpy as np
 
 from .utils import utils
 from .utils import pdbutils
 
 
@@ -42,18 +41,27 @@
                 {"smarts": "[#7X3v3][#6X3v4]",  "atype": "N",  "comment": "amide"},
                 {"smarts": "[#7+1]",            "atype": "N",  "comment": "ammonium, pyridinium"},
                 {"smarts": "[SX2]",             "atype": "SA", "comment": "sulfur acceptor"}
             ]
         }
     }
     """
-    def __init__(self, parameters={}):
+    def __init__(self, parameters={}, add_parameters=[]):
         self.parameters = json.loads(self.defaults_json)
         for key in parameters:
             self.parameters[key] = json.loads(json.dumps(parameters[key])) # a safe copy
+        # add additional parameters
+        if len(add_parameters) > 0:
+            keys = list(self.parameters["ATOM_PARAMS"].keys())
+            if len(keys) != 1:
+                msg = "add_parameters is usable only when there is one group of parameters"
+                msg += ", but there are %d groups: %s" % (len(keys), str(keys))
+                raise RuntimeError(msg)
+            key = keys[0]
+            self.parameters['ATOM_PARAMS'][key].extend(add_parameters)
 
     def __call__(self, setup):
         self._type_atoms(setup)
         if 'OFFATOMS' in self.parameters:
             cached_offatoms = self._cache_offatoms(setup)
             coords = [x for x in setup.coord.values()]
             self._set_offatoms(setup, cached_offatoms, coords)
```

### Comparing `meeko-0.4.0/meeko/bondtyper.py` & `meeko-0.5.0/meeko/bondtyper.py`

 * *Files identical despite different names*

### Comparing `meeko-0.4.0/meeko/covalentbuilder.py` & `meeko-0.5.0/meeko/covalentbuilder.py`

 * *Files identical despite different names*

### Comparing `meeko-0.4.0/meeko/data/atomtypes.txt` & `meeko-0.5.0/meeko/data/atomtypes.txt`

 * *Files identical despite different names*

### Comparing `meeko-0.4.0/meeko/data/pi_non_aromatic.txt` & `meeko-0.5.0/meeko/data/pi_non_aromatic.txt`

 * *Files identical despite different names*

### Comparing `meeko-0.4.0/meeko/data/waterfield.txt` & `meeko-0.5.0/meeko/data/waterfield.txt`

 * *Files identical despite different names*

### Comparing `meeko-0.4.0/meeko/flexibility.py` & `meeko-0.5.0/meeko/flexibility.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from itertools import product
 from operator import itemgetter
 from .utils import pdbutils
 
 
 class FlexibilityBuilder:
 
-    def __call__(self, setup, freeze_bonds=None, root_atom_index=None, break_combo_data=None, bonds_in_rigid_rings=None):
+    def __call__(self, setup, freeze_bonds=None, root_atom_index=None, break_combo_data=None, bonds_in_rigid_rings=None, glue_pseudo_atoms=None):
         """ """
         self.setup = setup
         self.flexibility_models = {}
         self._frozen_bonds = []
         if not freeze_bonds is None:
             self._frozen_bonds = freeze_bonds[:]
         # build graph for standard molecule (no open macrocycle rings)
@@ -30,15 +30,15 @@
             bond_break_combos = break_combo_data['bond_break_combos']
             bond_break_scores = break_combo_data['bond_break_scores']
             broken_rings_list = break_combo_data['broken_rings']
             for index in range(len(bond_break_combos)):
                 bond_break_combo = bond_break_combos[index]
                 bond_break_score = bond_break_scores[index]
                 broken_rings =     broken_rings_list[index]
-                model = self.build_rigid_body_connectivity(bond_break_combo, broken_rings, bonds_in_rigid_rings)
+                model = self.build_rigid_body_connectivity(bond_break_combo, broken_rings, bonds_in_rigid_rings, glue_pseudo_atoms)
                 self.set_graph_root(model, root_atom_index) # finds root if root_atom_index==None
                 self.add_flex_model(model, score=True, initial_score=bond_break_score)
 
         self.select_best_model()
 
         # clean up
         del self._frozen_bonds
@@ -80,15 +80,15 @@
         if score == False:
             model['score'] = float('inf')
         else:
             penalty = self.score_flex_model(model)
             model['score'] = initial_score + penalty
         self.flexibility_models[model_id] = model
 
-    def build_rigid_body_connectivity(self, bonds_to_break=None, broken_rings=None, bonds_in_rigid_rings=None):
+    def build_rigid_body_connectivity(self, bonds_to_break=None, broken_rings=None, bonds_in_rigid_rings=None, glue_pseudo_atoms=None):
         """
         rigid_body_graph is the graph of rigid bodies
         ( rigid_body_id->[rigid_body_id,...] )
 
         rigid_body_members contains the atom indices in each rigid_body_id,
         ( rigid_body_id->[atom,...] )
 
@@ -98,15 +98,15 @@
         ( (rigid_body1, rigid_body2) -> (atom1,atom2)
         """
         # make a copy of the current mol graph, updated with the broken bond
         if bonds_to_break is None:
             self._current_setup = self.setup
         else:
             self._current_setup = self.copy_setup(bonds_to_break, broken_rings, bonds_in_rigid_rings)
-            self.update_closure_atoms(bonds_to_break)
+            self.update_closure_atoms(bonds_to_break, glue_pseudo_atoms)
 
         # walk the mol graph to build the rigid body maps
         self._visited = defaultdict(lambda:False)
         self._rigid_body_members = {}
         self._rigid_body_connectivity = {}
         self._rigid_body_graph = defaultdict(list)
         self._rigid_index_by_atom = {}
@@ -199,50 +199,53 @@
     def score_flex_model(self, model):
         """ score a flexibility model basing on the graph properties"""
         base = self.flexibility_models[0]['graph_depth']
         score = 10 * (base-model['graph_depth'])
         return score
 
 
-    def _generate_closure_pseudo(self, setup, bond_id):
+    def _generate_closure_pseudo(self, setup, bond_id, coords_dict={}):
         """ calculate position and parameters of the pseudoatoms for the closure"""
         closure_pseudo = []
         for idx in (0,1):
             target = bond_id[1 - idx]
             anchor = bond_id[0 - idx]
-            coord = setup.get_coord(target)
+            if coords_dict is None or len(coords_dict) == 0:
+                coord = setup.get_coord(target)
+            else:
+                coord = coords_dict[anchor]
             anchor_info = setup.pdbinfo[anchor]
             pdbinfo = pdbutils.PDBAtomInfo('G', anchor_info.resName, anchor_info.resNum, anchor_info.chain)
             closure_pseudo.append({
                 'coord': coord,
                 'anchor_list': [anchor],
                 'charge': 0.0,
                 'pdbinfo': pdbinfo,
                 'atom_type': 'G',
                 'bond_type': 0,
                 'rotatable': False})
         return closure_pseudo
 
 
-    def update_closure_atoms(self, bonds_to_break):
+    def update_closure_atoms(self, bonds_to_break, coords_dict):
         """ create pseudoatoms required by the flexible model with broken bonds"""
 
         setup = self._current_setup
         for i, bond in enumerate(bonds_to_break):
             setup.ring_closure_info["bonds_removed"].append(bond) # bond is pair of atom indices
-            pseudos = self._generate_closure_pseudo(setup, bond)
+            pseudos = self._generate_closure_pseudo(setup, bond, coords_dict)
             for pseudo in pseudos:
                 pseudo['atom_type'] = "%s%d" % (pseudo['atom_type'], i)
-                pseudo_index = self._current_setup.add_pseudo(**pseudo)
+                pseudo_index = setup.add_pseudo(**pseudo)
                 atom_index = pseudo['anchor_list'][0]
                 if atom_index in setup.ring_closure_info:
                     raise RuntimeError("did not expect more than one G per atom")
                 setup.ring_closure_info["pseudos_by_atom"][atom_index] = pseudo_index
-            self._current_setup.set_atom_type(bond[0], "CG%d" % i)
-            self._current_setup.set_atom_type(bond[1], "CG%d" % i)
+            setup.set_atom_type(bond[0], "CG%d" % i)
+            setup.set_atom_type(bond[1], "CG%d" % i)
 
 
     def walk_rigid_body_graph(self, start):
         """ recursive walk to build the graph of rigid bodies"""
         idx = 0
         rigid = [start]
         self._visited[start] = True
```

### Comparing `meeko-0.4.0/meeko/hydrate.py` & `meeko-0.5.0/meeko/hydrate.py`

 * *Files identical despite different names*

### Comparing `meeko-0.4.0/meeko/macrocycle.py` & `meeko-0.5.0/meeko/macrocycle.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,14 @@
         # accept also double bonds (if nothing better is found)
         self._double_bond_penalty = double_bond_penalty
         self.max_breaks = max_breaks
 
         self.setup = None
         self.breakable_rings = None
         self._conj_bond_list = None
-        self.breakable_bonds = None
 
     def collect_rings(self, setup):
         """ get non-aromatic rings of desired size and
             list bonds that are part of unbreakable rings
 
             Bonds belonging to rigid cycles can't be deleted or
             made rotatable even if they are part of a breakable ring
@@ -71,16 +70,16 @@
             bond = (f[1], f[2])
             bond = (min(bond), max(bond))
             conj_bond_list.append(bond)
         return conj_bond_list
 
     def _score_bond(self, bond):
         """ provide a score for the likeness of the bond to be broken"""
-        atom_idx1 = bond[0]
-        atom_idx2 = bond[1]
+        bond = self.setup.get_bond_id(bond[0], bond[1])
+        atom_idx1, atom_idx2 = bond
         score = 100
 
         bond_order = self.setup.bond[bond]['bond_order']
         if bond_order not in [1, 2, 3]: # aromatic, double, made rigid explicitly (order=1.1 from --rigidify)
             return -1
         if not self.setup.get_element(atom_idx1) == 6 or self.setup.is_aromatic(atom_idx1):
             return -1
@@ -115,27 +114,33 @@
         for ring_atom_indices in self.breakable_rings:
             for bond in self.setup.get_bonds_in_ring(ring_atom_indices):
                 score = self._score_bond(bond)
                 if score > 0 and bond not in bonds_in_rigid_rings:
                     breakable[bond] = {'score': score}
         return breakable
 
-    def search_macrocycle(self, setup):
+    def search_macrocycle(self, setup, delete_these_bonds=[]):
         """Search for macrocycle in the molecule
 
         Args:
             setup : MoleculeSetup object
 
         """
         self.setup = setup
 
         self.breakable_rings, bonds_in_rigid_rings = self.collect_rings(setup)
         self._conj_bond_list = self._detect_conj_bonds()
-        self.breakable_bonds = self.get_breakable_bonds(bonds_in_rigid_rings)
-        break_combo_data = self.combinatorial_break_search(self.breakable_bonds)
+        if len(delete_these_bonds) == 0:
+            breakable_bonds = self.get_breakable_bonds(bonds_in_rigid_rings)
+        else:
+            breakable_bonds = {}
+            for bond in delete_these_bonds:
+                bond = self.setup.get_bond_id(bond[0], bond[1])
+                breakable_bonds[bond] = {"score": self._score_bond(bond)}
+        break_combo_data = self.combinatorial_break_search(breakable_bonds)
         return break_combo_data, bonds_in_rigid_rings
 
     def combinatorial_break_search(self, breakable_bonds):
         """ enumerate all combinations of broken bonds
             once a bond is broken, it will break one or more rings
             subsequent bonds will be pulled from intact (unbroken) rings
```

### Comparing `meeko-0.4.0/meeko/molecule_pdbqt.py` & `meeko-0.5.0/meeko/molecule_pdbqt.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,28 +69,41 @@
         'intermolecular_energies': [],
         'internal_energies': [],
         'index_map': {},
         'pdbqt_string': [],
         'smiles': {},
         'smiles_index_map': {},
         'smiles_h_parent': {},
+        'cluster_id': [],
+        'rank_in_cluster': [],
+        'cluster_leads_sorted': [],
+        'cluster_size': [],
     }
 
+    tmp_cluster_data = {}
+
     buffer_index_map = {}
     buffer_smiles = None
     buffer_smiles_index_map = []
     buffer_smiles_h_parent = []
 
     lines = pdbqt_string.split('\n')
     if len(lines[-1]) == 0: lines = lines[:-1]
     lines = [line + '\n' for line in lines]
     for line in lines:
         if is_dlg:
             if line.startswith('DOCKED'):
                 line = line[8:]
+            # parse clustering
+            elif line.endswith('RANKING\n'):
+                fields = line.split()
+                cluster_id = int(fields[0])
+                subrank = int(fields[1])
+                run_id = int(fields[2])
+                tmp_cluster_data[run_id] = (cluster_id, subrank)
             else:
                 continue
 
         if not line.startswith(('MODEL', 'ENDMDL')):
             """This is very lazy I know...
             But would you rather spend time on rebuilding the whole torsion tree and stuff
             for writing PDBQT files or drinking margarita? Energy was already spend to build
@@ -137,22 +150,23 @@
                     i += 1
 
             # Once it is done, we can return to a normal life... and add existing atoms
             tmp_atoms.append((i, serial, name, resid, resname, chainid, xyz, partial_charges, atom_type))
             tmp_positions.append(xyz)
             tmp_actives.append(i)
 
-            # We store water idx separately from the rest since their number can be variable
-            if is_first_pose and atom_type != 'W':
-                atom_annotations[location].append(i)
-                atom_annotations['all'].append(i)
+            if is_first_pose:
                 atom_annotations["mol_index"].setdefault(mol_index, [])
                 atom_annotations["mol_index"][mol_index].append(i)
-                if not skip_typing:
-                    atom_annotations[atom_property_definitions[atom_type]].append(i)
+                # We store water idx separately from the rest since their number can be variable
+                if atom_type != 'W':
+                    atom_annotations[location].append(i)
+                    atom_annotations['all'].append(i)
+                    if not skip_typing:
+                        atom_annotations[atom_property_definitions[atom_type]].append(i)
 
             if atom_type == 'W':
                 water_indices.update([i])
 
             previous_serial = serial
             i += 1
         elif line.startswith("ROOT") and is_first_pose:
@@ -269,26 +283,46 @@
 
     pose_data['n_poses'] = n_poses
 
     # We add indices of all the water molecules we saw
     if water_indices:
         atom_annotations['water'] = list(water_indices)
 
+    # clustering        
+    if len(tmp_cluster_data) > 0:
+        if len(tmp_cluster_data) != n_poses:
+            raise RuntimeError("Nr of poses in cluster data (%d) differs from nr of poses (%d)" % (len(tmp_cluster_data, n_poses)))
+        pose_data["cluster_id"] = [None] * n_poses
+        pose_data["rank_in_cluster"] = [None] * n_poses
+        pose_data["cluster_size"] = [None] * n_poses
+        cluster_ids = [cluster_id for _, (cluster_id, _) in tmp_cluster_data.items()]
+        n_clusters = max(cluster_ids)
+        pose_data["cluster_leads_sorted"] = [None] * n_clusters
+        for pose_index, (cluster_id, rank_in_cluster) in tmp_cluster_data.items():
+            pose_data["cluster_id"][pose_index - 1] = cluster_id
+            pose_data["rank_in_cluster"][pose_index - 1] = rank_in_cluster
+            pose_data["cluster_size"][pose_index - 1] = cluster_ids.count(cluster_id)
+            if rank_in_cluster == 1: # is cluster lead
+                pose_data["cluster_leads_sorted"][cluster_id - 1] = pose_index - 1
     return atoms, positions, atom_annotations, pose_data
 
 
 def _identify_bonds(atom_idx, positions, atom_types):
     bonds = defaultdict(list)
     KDTree = spatial.cKDTree(positions)
     bond_allowance_factor = 1.1
     # If we ask more than the number of coordinates/element
     # in the BHTree, we will end up with some inf values
     k = 5 if len(atom_idx) > 5 else len(atom_idx)
     atom_idx = np.array(atom_idx)
 
+    # If there is only one atom, we know there won't be a single bond..
+    if len(atom_idx) == 1:
+        return bonds
+
     for atom_i, position, atom_type in zip(atom_idx, positions, atom_types):
         distances, indices = KDTree.query(position, k=k)
         r_cov = covalent_radius[autodock4_atom_types_elements[atom_type]]
 
         optimal_distances = [bond_allowance_factor * (r_cov + covalent_radius[autodock4_atom_types_elements[atom_types[i]]]) for i in indices[1:]]
         bonds[atom_i] = atom_idx[indices[1:][np.where(distances[1:] < optimal_distances)]].tolist()
 
@@ -456,15 +490,15 @@
                 atom_idx = np.array(atom_idx, dtype=np.int)
         else:
             atom_idx = np.arange(0, self._atoms.shape[0])
 
         # Get index of only the active atoms
         if only_active:
             active_atoms_idx = self._pose_data['active_atoms'][self._current_pose]
-            atom_idx = list(set(atom_idx).intersection(active_atoms_idx))
+            atom_idx = sorted(list(set(atom_idx).intersection(active_atoms_idx)))
 
         atoms = self._atoms[atom_idx].copy()
         atoms['xyz'] = self._positions[self._current_pose, atom_idx,:]
 
         return atoms
 
     def positions(self, atom_idx=None, only_active=True):
```

### Comparing `meeko-0.4.0/meeko/molsetup.py` & `meeko-0.5.0/meeko/molsetup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # Meeko
 #
 
 from copy import deepcopy
 from collections import defaultdict, OrderedDict
 import json
 import warnings
+import sys
 
 import numpy as np
 from rdkit import Chem
 from rdkit.Chem import rdPartialCharges
 
 from .utils import rdkitutils
 from .utils import utils
@@ -20,15 +21,14 @@
     from openbabel import openbabel as ob
     from .utils import obutils
 except ImportError:
     _has_openbabel = False
 else:
     _has_openbabel = True
 
-# based on the assumption we are using OpenBabel
 
 # TODO modify so that there are no more dictionaries and only list/arrays (fix me)
 # methods like add_x,del_x,get_x will deal with indexing (fix me)
 # the goal is to remove dictionaries (fix me)
 
 # (fix me)) provide infrastructure to calculate "differential" modifications,
 # like tautomers: the class calculating tautomers will copy and modify the setup
@@ -45,45 +45,17 @@
 class MoleculeSetup:
     """ mol: molecule structurally prepared with explicit hydrogens
 
         the setup provides:
             - data storage
             - SMARTS matcher for all atom typers
     """
-    # possibly useless here
-    attributes_to_copy = [
-        "atom_pseudo",
-        "atom_ignore",
-        "atom_type",
-        "atom_true_count",
-        "atom_pseudo",
-        "element",
-        "coord",
-        "charge",
-        "pdbinfo",
-        "chiral",
-        "graph",
-        "bond",
-        "interaction_vector",
-        "rings",
-        "rings_aromatic",
-        "atom_to_ring_id",
-        "flexibility_model",
-        "ring_closure_info",
-        'history',
-        'name',
-        ]
-
-    def __init__(self, mol, keep_chorded_rings=False, keep_equivalent_rings=False,
-                 assign_charges=True, template=None):
-        """initialize a molecule template, either from scratch (template is None)
-            or by using an existing setup (template is an instance of MoleculeSetup
-        """
 
-        self.mol = mol
+    def __init__(self):
+
         self.atom_pseudo = []
         self.coord = OrderedDict()  # FIXME all OrderedDict shuold be converted to lists?
         self.charge = OrderedDict()
         self.pdbinfo = OrderedDict()
         self.atom_type = OrderedDict()
         self.atom_ignore = OrderedDict()
         self.chiral = OrderedDict()
@@ -99,30 +71,19 @@
         }
         # ring information
         self.rings = {}
         self.rings_aromatic = []
         self.atom_to_ring_id = defaultdict(list)
         self.ring_corners = {}  # used to store corner flexibility
         self.name = None
-        # this could be used to keep track of transformations? (corner flipping)
-        self.history = []
-        if template is None:
-            self.process_mol(assign_charges, keep_chorded_rings, keep_equivalent_rings)
-        else:
-            if not isinstance(template, MoleculeSetup):
-                raise TypeError('FATAL: template must be an instance of MoleculeSetup')
-            self.copy_attributes_from(template)
-
-    def process_mol(self, assign_charges, keep_chorded_rings, keep_equivalent_rings):
-        self.atom_true_count = self.get_num_mol_atoms()
-        self.name = self.get_mol_name()
-        self.init_atom(assign_charges)
-        self.perceive_rings(keep_chorded_rings, keep_equivalent_rings)
-        self.init_bond()
-        return
+
+    def copy(self):
+        newsetup = MoleculeSetup()
+        newsetup.__dict__ = deepcopy(self.__dict__)
+        return newsetup
 
     def add_atom(self, idx=None, coord=np.array([0.0, 0.0,0.0], dtype='float'),
             element=None, charge=0.0, atom_type=None, pdbinfo=None, neighbors=None,
             ignore=False, chiral=False, overwrite=False):
         """ function to add all atom information at once;
             every property is optional
         """
@@ -436,43 +397,32 @@
         for attr in self.attributes_to_copy:
             attr_copy = deepcopy(getattr(template, attr))
             setattr(self, attr, attr_copy)
         # TODO possible BUG? the molecule is shared by the different setups
         #      if one of them alters the molecule, properties will not be the same
         self.mol = template.mol
 
-    def merge_hydrogen(self):
-        """ standard method to merge hydrogens bound to carbons"""
-        merged = 0
-
-        for a, neigh_list in list(self.graph.items()):
-            # look for hydrogens
-            if not self.get_element(a) == 1:
-                continue
-
-            hydrogen_charge = self.get_charge(a)
-
-            for n in neigh_list:
-                # look for carbons
-                if self.get_element(n) == 6:
-                    merged += 1
-                    carbon_charge = self.get_charge(n)
-                    # carbon adsorbs the final charge
-                    self.set_charge(n, carbon_charge + hydrogen_charge)
-                    # flag hydrogen to be ignored and set its charge to 0
-                    self.set_charge(a, 0)
-                    self.set_ignore(a, True)
-
+    def merge_terminal_atoms(self, indices):
+        """for merging hydrogens, but will merge any atom or pseudo atom
+            that is bonded to only one other atom"""
+
+        for index in indices:
+            if len(self.graph[index]) != 1:
+                msg = "Atempted to merge atom %d with %d neighbors. "
+                msg += "Only atoms with one neighbor can be merged."
+                msg = msg % (index + 1, len(self.graph[index]))
+                raise RuntimeError(msg)
+            neighbor_index = self.graph[index][0]
+            self.charge[neighbor_index] += self.get_charge(index)
+            self.charge[index] = 0.0
+            self.set_ignore(index, True)
+            
     def has_implicit_hydrogens(self):
         raise NotImplementedError("This method must be overloaded by inheriting class")
 
-    def copy(self):
-        """ return a copy of the current setup"""
-        raise NotImplementedError("This method must be overloaded by inheriting class")
-
     def init_atom(self):
         """ iterate through molecule atoms and build the atoms table """
         raise NotImplementedError("This method must be overloaded by inheriting class")
 
     def perceive_rings(self, keep_chorded_rings, keep_equivalent_rings):
         """ populate the rings and aromatic rings tableshe atoms table:
         self.rings_aromatics : list
@@ -532,78 +482,147 @@
 
     def find_pattern(self, smarts):
         raise NotImplementedError("This method must be overloaded by inheriting class")
 
     def get_smiles_and_order(self):
         raise NotImplementedError("This method must be overloaded by inheriting class")
 
+    def show(self):
+        tot_charge = 0
 
-class RDKitMoleculeSetup(MoleculeSetup):
+        print("Molecule setup\n")
+        print("==============[ ATOMS ]===================================================")
+        print("idx  |          coords            | charge |ign| atype    | connections")
+        print("-----+----------------------------+--------+---+----------+--------------- . . . ")
+        for k, v in list(self.coord.items()):
+            print("% 4d | % 8.3f % 8.3f % 8.3f | % 1.3f | %d" % (k, v[0], v[1], v[2],
+                  self.charge[k], self.atom_ignore[k]),
+                  "| % -8s |" % self.atom_type[k],
+                  self.graph[k])
+            tot_charge += self.charge[k]
+        print("-----+----------------------------+--------+---+----------+--------------- . . . ")
+        print("  TOT CHARGE: %3.3f" % tot_charge)
+
+        print("\n======[ DIRECTIONAL VECTORS ]==========")
+        for k, v in list(self.coord.items()):
+            if k in self.interaction_vector:
+                print("% 4d " % k, self.atom_type[k], end=' ')
+
+        print("\n==============[ BONDS ]================")
+        # For sanity users, we won't show those keys for now
+        keys_to_not_show = ['bond_order', 'type']
+        for k, v in list(self.bond.items()):
+            t = ', '.join('%s: %s' % (i, j) for i, j in v.items() if not i in keys_to_not_show)
+            print("% 8s - " % str(k), t)
 
-    warned_not3D = False
+        # _macrocycle_typer.show_macrocycle_scores(self)
 
-    def __init__(self, mol, keep_chorded_rings=False, keep_equivalent_rings=False,
-                 assign_charges=True, template=None):
-        nr_conformers = mol.GetNumConformers()
-        if nr_conformers == 0: 
+        print('')
+
+
+
+class RDKitMoleculeSetup(MoleculeSetup):
+
+    @classmethod
+    def from_mol(cls, mol, keep_chorded_rings=False, keep_equivalent_rings=False,
+                 assign_charges=True, conformer_id=-1):
+        if mol.GetNumConformers() == 0: 
             raise ValueError("RDKit molecule does not have a conformer. Need 3D coordinates.")
-        elif nr_conformers > 1:
+        rdkit_conformer = mol.GetConformer(conformer_id) 
+        if not rdkit_conformer.Is3D():
+            warnings.warn("RDKit molecule not labeled as 3D. This warning won't show again.")
+            RDKitMoleculeSetup.warned_not3D = True
+        if mol.GetNumConformers() > 1 and conformer_id == -1:
             msg = "RDKit molecule has multiple conformers. Considering only the first one." 
-            warnings.warn(msg) 
-        super().__init__(
-            mol,
-            keep_chorded_rings,
-            keep_equivalent_rings,
-            assign_charges,
-            template)
+            print(msg, file=sys.stderr)
+        molsetup = cls()
+        molsetup.mol = mol
+        molsetup.atom_true_count = molsetup.get_num_mol_atoms()
+        molsetup.name = molsetup.get_mol_name()
+        coords = rdkit_conformer.GetPositions()
+        molsetup.init_atom(assign_charges, coords)
+        molsetup.perceive_rings(keep_chorded_rings, keep_equivalent_rings)
+        molsetup.init_bond()
+        return molsetup
 
 
     def get_smiles_and_order(self):
+        """
+            return the SMILES after Chem.RemoveHs()
+            and the mapping between atom indices in smiles and self.mol
+        """
 
         # 3D SDF files written by other toolkits (OEChem, ChemAxon)
         # seem to not include the chiral flag in the bonds block, only in
         # the atoms block. RDKit ignores the atoms chiral flag as per the
         # spec. When reading SDF (e.g. from PubChem/PDB),
         # we may need to have RDKit assign stereo from coordinates, see:
         # https://sourceforge.net/p/rdkit/mailman/message/34399371/
         mol_noH = Chem.RemoveHs(self.mol) # imines (=NH) may become chiral
+        # stereo imines [H]/N=C keep [H] after RemoveHs()
+        # H isotopes also kept after RemoveHs()
         atomic_num_mol_noH = [atom.GetAtomicNum() for atom in mol_noH.GetAtoms()]
         noH_to_H = []
-        num_H_in_noH = 0 # e.g. stereo imines [H]/N=C keep [H] after RemoveHs()
+        parents_of_hs = {}
         for (index, atom) in enumerate(self.mol.GetAtoms()):
             if atom.GetAtomicNum() == 1: continue
             for i in range(len(noH_to_H), len(atomic_num_mol_noH)):
-                if atomic_num_mol_noH[i] > 1: break
+                if atomic_num_mol_noH[i] > 1:
+                    break
+                h_atom = mol_noH.GetAtomWithIdx(len(noH_to_H))
+                assert(h_atom.GetAtomicNum() == 1)
+                neighbors = h_atom.GetNeighbors()
+                assert(len(neighbors) == 1)
+                parents_of_hs[len(noH_to_H)] = neighbors[0].GetIdx()
                 noH_to_H.append('H')
             noH_to_H.append(index)
         extra_hydrogens = len(atomic_num_mol_noH) - len(noH_to_H)
         if extra_hydrogens > 0:
             assert(set(atomic_num_mol_noH[len(noH_to_H):]) == {1})
-            noH_to_H.extend(['H'] * extra_hydrogens)
-
-        # map indices of explicit hydrogens, e.g. stereo imine [H]/N=C
-        for index in range(len(noH_to_H)):
-            if noH_to_H[index] != 'H': continue
-            h_atom = mol_noH.GetAtomWithIdx(index)
+        for i in range(extra_hydrogens):
+            h_atom = mol_noH.GetAtomWithIdx(len(noH_to_H))
             assert(h_atom.GetAtomicNum() == 1)
-            parents = h_atom.GetNeighbors()
-            assert(len(parents) == 1)
-            num_h_in_parent = len([a for a in parents[0].GetNeighbors() if a.GetAtomicNum() == 1])
-            if num_h_in_parent != 1:
-                msg = "Can't handle %d explicit H for each heavy atomin noH mol.\n" % num_h_in_parent
-                msg += "Was expecting only imines [H]N=\n"
-                raise RuntimeError(msg)
-            parent_index_in_mol_with_H = noH_to_H[parents[0].GetIdx()]
-            parent_in_mol_with_H = self.mol.GetAtomWithIdx(parent_index_in_mol_with_H)
-            h_in_mol_with_H = [a for a in parent_in_mol_with_H.GetNeighbors() if a.GetAtomicNum() == 1]
-            if len(h_in_mol_with_H) != 1:
-                msg = "Can't handle %d explicit H for each heavy atomin noH mol.\n" % len(h_in_mol_with_H)
-                msg += "Was expecting only imines [H]N=\n"
-                raise RuntimeError(msg)
-            noH_to_H[index] = h_in_mol_with_H[0].GetIdx()
+            neighbors = h_atom.GetNeighbors()
+            assert(len(neighbors) == 1)
+            parents_of_hs[len(noH_to_H)] = neighbors[0].GetIdx()
+            noH_to_H.append('H')
+
+        # noH_to_H has the same length as the number of atoms in mol_noH
+        # and each value is:
+        #    - the index of the corresponding atom in mol, if value is integer
+        #    - an hydrogen, if value is "H"
+        # now, we need to replace those "H" with integers
+        # "H" occur with stereo imine (e.g. [H]/N=C) and heavy Hs (e.g. [2H])
+        hs_by_parent = {}
+        for hidx, pidx in parents_of_hs.items():
+            hs_by_parent.setdefault(pidx, [])
+            hs_by_parent[pidx].append(hidx)
+        for pidx, hidxs in hs_by_parent.items():
+            siblings_of_h = [atom for atom in self.mol.GetAtomWithIdx(noH_to_H[pidx]).GetNeighbors() if atom.GetAtomicNum() == 1]
+            sortidx = [i for i, j in sorted(list(enumerate(siblings_of_h)), key=lambda x: x[1].GetIdx())]
+            if len(hidxs) == len(siblings_of_h):  
+                # This is the easy case, just map H to each other in the order they appear
+                for i, hidx in enumerate(hidxs):
+                    noH_to_H[hidx] = siblings_of_h[sortidx[i]].GetIdx()
+            elif len(hidxs) < len(siblings_of_h):
+                # check hydrogen isotopes
+                sibling_isotopes = [siblings_of_h[sortidx[i]].GetIsotope() for i in range(len(siblings_of_h))]
+                molnoH_isotopes = [mol_noH.GetAtomWithIdx(hidx) for hidx in hidxs]
+                matches = []
+                for i, sibling_isotope in enumerate(sibling_isotopes):
+                    for hidx in hidxs[len(matches):]:
+                        if mol_noH.GetAtomWithIdx(hidx).GetIsotope() == sibling_isotope:
+                            matches.append(i)
+                            break
+                if len(matches) != len(hidxs):
+                    raise RuntimeError("Number of matched isotopes %d differs from query Hs: %d" % (len(matched), len(hidxs)))
+                for hidx, i in zip(hidxs, matches):
+                    noH_to_H[hidx] = siblings_of_h[sortidx[i]].GetIdx()
+            else:
+                raise RuntimeError("nr of Hs in mol_noH bonded to an atom exceeds nr of Hs in self.mol")
 
         smiles = Chem.MolToSmiles(mol_noH)
         order_string = mol_noH.GetProp("_smilesAtomOutputOrder")
         order_string = order_string.replace(',]', ']') # remove trailing comma
         order = json.loads(order_string) # mol_noH to smiles
         order = list(np.argsort(order))
         order = {noH_to_H[i]: order[i]+1 for i in range(len(order))} # 1-index
@@ -621,26 +640,24 @@
 
     def get_num_mol_atoms(self):
         return self.mol.GetNumAtoms()
 
     def get_equivalent_atoms(self):
        return list(Chem.CanonicalRankAtoms(self.mol, breakTies=False))
 
-    def init_atom(self, assign_charges):
+    def init_atom(self, assign_charges, coords):
         """ initialize the atom table information """
-        # extract the coordinates
-        c = self.mol.GetConformers()[0]
-        if not c.Is3D() and not RDKitMoleculeSetup.warned_not3D:
-            warnings.warn("RDKit molecule not labeled as 3D. This warning won't show again.")
-            RDKitMoleculeSetup.warned_not3D = True
-        coords = c.GetPositions()
         # extract/generate charges
         if assign_charges:
-            rdPartialCharges.ComputeGasteigerCharges(self.mol)
-            charges = [a.GetDoubleProp('_GasteigerCharge') for a in self.mol.GetAtoms()]
+            copy_mol = Chem.Mol(self.mol)
+            for atom in copy_mol.GetAtoms():
+                if atom.GetAtomicNum() == 34:
+                    atom.SetAtomicNum(16)
+            rdPartialCharges.ComputeGasteigerCharges(copy_mol)
+            charges = [a.GetDoubleProp('_GasteigerCharge') for a in copy_mol.GetAtoms()]
         else:
             charges = [0.0] * self.mol.GetNumAtoms()
         # perceive chirality
         # TODO check consistency for chiral model between OB and RDKit
         chiral_info = {}
         for data in Chem.FindMolChiralCenters(self.mol, includeUnassigned=True):
             chiral_info[data[0]] = data[1]
@@ -676,15 +693,20 @@
             idx1_rings = set(self.get_atom_rings(idx1))
             idx2_rings = set(self.get_atom_rings(idx2))
             in_rings = list(set.intersection(idx1_rings, idx2_rings))
             self.add_bond(idx1, idx2, order=bond_order, rotatable=rotatable, in_rings=in_rings)
 
     def copy(self):
         """ return a copy of the current setup"""
-        return RDKitMoleculeSetup(self.mol, template=self)
+        newsetup = RDKitMoleculeSetup()
+        for key, value in self.__dict__.items():
+            if key != "mol":
+                newsetup.__dict__[key] = deepcopy(value)
+        newsetup.mol = Chem.Mol(self.mol) # not sure how deep of a copy this is
+        return newsetup
 
     def has_implicit_hydrogens(self):
         # based on needsHs from RDKit's AddHs.cpp
         for atom in self.mol.GetAtoms():
             nr_H_neighbors = 0
             for neighbor in atom.GetNeighbors():
                 nr_H_neighbors += int(neighbor.GetAtomicNum() == 1)
```

### Comparing `meeko-0.4.0/meeko/rdkit_mol_create.py` & `meeko-0.5.0/meeko/rdkit_mol_create.py`

 * *Files 19% similar despite different names*

```diff
@@ -156,15 +156,17 @@
             "smiles": "CCc1ccc(cc1)O",
             "atom_names_in_smiles_order": ["CA", "CB", "CG", "CD1", "CE1", "CZ", "CE2", "CD2", "OH"],
             "h_to_parent_index": {"HH": 8},
         },
     }
 
     @classmethod
-    def from_pdbqt_mol(cls, pdbqt_mol): # TODO add pseudo-water (W atoms, variable nr each pose)
+    def from_pdbqt_mol(cls, pdbqt_mol, only_cluster_leads=False): # TODO add pseudo-water (W atoms, variable nr each pose)
+        if only_cluster_leads and len(pdbqt_mol._pose_data["cluster_leads_sorted"]) == 0:
+            raise RuntimeError("no cluster_leads in pdbqt_mol but only_cluster_leads=True")
         mol_list = []
         for mol_index in pdbqt_mol._atom_annotations["mol_index"]:
             smiles = pdbqt_mol._pose_data['smiles'][mol_index]
             index_map = pdbqt_mol._pose_data['smiles_index_map'][mol_index]
             h_parent = pdbqt_mol._pose_data['smiles_h_parent'][mol_index]
             atom_idx = pdbqt_mol._atom_annotations["mol_index"][mol_index]
 
@@ -177,21 +179,24 @@
                 if len(residue_names) == 1:
                     resname = residue_names.pop()
                     smiles, index_map, h_parent = cls.guess_flexres_smiles(resname, atom_names)
                     if smiles is None: # failed guessing smiles for possible flexres
                         mol_list.append(None)
                         continue
 
-            mol = Chem.MolFromSmiles(smiles)
+            if only_cluster_leads:
+                pose_ids = pdbqt_mol._pose_data["cluster_leads_sorted"]
+            else:
+                pose_ids = range(pdbqt_mol._pose_data["n_poses"])
 
+            mol = Chem.MolFromSmiles(smiles)
             coordinates_all_poses = []
-            i = 0
-            for pose in pdbqt_mol:
-                i += 1
-                coordinates = pose.positions(atom_idx)
+            for i in pose_ids:
+                pdbqt_mol._current_pose = i
+                coordinates = pdbqt_mol.positions(atom_idx)
                 mol = cls.add_pose_to_mol(mol, coordinates, index_map) 
                 coordinates_all_poses.append(coordinates) 
 
             # add Hs only after all poses are added as conformers
             # because Chem.AddHs() will affect all conformers at once 
             mol = cls.add_hydrogens(mol, coordinates_all_poses, h_parent) 
 
@@ -219,14 +224,16 @@
 
 
         if len(set(atom_names)) != len(atom_names):
             return None, None, None
         candidate_resnames = cls.ambiguous_flexres_choices.get(resname, [resname])
         for resname in candidate_resnames:
             is_match = False
+            if resname not in cls.flexres[resname]["atom_names_in_smiles_order"]:
+                continue
             atom_names_in_smiles_order = cls.flexres[resname]["atom_names_in_smiles_order"]
             h_to_parent_index = cls.flexres[resname]["h_to_parent_index"]
             expected_names = atom_names_in_smiles_order + list(h_to_parent_index.keys())
             if len(atom_names) != len(expected_names):
                 continue
             nr_matched_atom_names = sum([int(n in atom_names) for n in expected_names])
             if nr_matched_atom_names == len(expected_names):
@@ -260,26 +267,39 @@
 
         Raises:
             RuntimeError: Will raise error if number of coordinates provided does not
                 match the number of atoms there should be coordinates for.
         """
 
         n_atoms = mol.GetNumAtoms()
+        n_mappings = int(len(index_map) / 2)
         conf = Chem.Conformer(n_atoms)
-        if n_atoms != len(index_map) / 2:
+        if n_atoms < n_mappings:
             raise RuntimeError(
-                "ERROR! Given {n_coords} atom coordinates"
-                "but index_map is for {n_at} atoms.".format(
-                    n_coords=n_atoms, n_at=len(index_map) / 2))
-        for i in range(n_atoms):
+                "Given {n_coords} atom coordinates "
+                "but index_map is greater at {n_at} atoms.".format(
+                    n_coords=n_atoms, n_at=n_mappings))
+        coord_is_set = [False] * n_atoms
+        for i in range(n_mappings):
             pdbqt_index = int(index_map[i * 2 + 1]) - 1
+            mol_index = int(index_map[i * 2]) - 1
             x, y, z = [float(coord) for coord in ligand_coordinates[pdbqt_index]]
-            conf.SetAtomPosition(int(index_map[i * 2]) - 1, Point3D(x, y, z))
+            conf.SetAtomPosition(mol_index, Point3D(x, y, z))
+            coord_is_set[mol_index] = True
         mol.AddConformer(conf, assignId=True)
-
+        # some hydrogens (isotopes) may have no coordinate set yet
+        for i, is_set in enumerate(coord_is_set):
+            if not is_set:
+                atom = mol.GetAtomWithIdx(i)
+                if atom.GetAtomicNum() != 1:
+                    raise RuntimeError("Only H allowed to be in SMILES but not in PDBQT")
+                neigh = atom.GetNeighbors()
+                if len(neigh) != 1:
+                    raise RuntimeError("Expected H to have one neighbor")
+                AllChem.SetTerminalAtomCoords(mol, i, neigh[0].GetIdx())
         return mol
 
 
     @staticmethod
     def add_hydrogens(mol, coordinates_list, h_parent):
         """Add hydrogen atoms to ligand RDKit mol, adjust the positions of
             polar hydrogens to match pdbqt
@@ -330,33 +350,47 @@
             atom_names_in_smiles_order = cls.flexres[resname]["atom_names_in_smiles_order"]
             h_to_parent_index = cls.flexres[resname]["h_to_parent_index"]
             expected_names = atom_names_in_smiles_order + list(h_to_parent_index.keys())
             if len(expected_names) != len(set(expected_names)):
                 raise RuntimeError("repeated atom names in cls.flexres[%s]" % resname)
 
     @staticmethod
-    def write_sd_string(pdbqt_mol):
+    def write_sd_string(pdbqt_mol, only_cluster_leads=False):
         sio = StringIO()
         f = Chem.SDWriter(sio)
-        mol_list = RDKitMolCreate.from_pdbqt_mol(pdbqt_mol)
+        mol_list = RDKitMolCreate.from_pdbqt_mol(pdbqt_mol, only_cluster_leads)
         failures = [i for i, mol in enumerate(mol_list) if mol is None]
         combined_mol = RDKitMolCreate.combine_rdkit_mols(mol_list)
         if combined_mol is None:
             return "", failures
         nr_conformers = combined_mol.GetNumConformers()
         property_names = {
             "free_energy": "free_energies",
             "intermolecular_energy": "intermolecular_energies",
             "internal_energy": "internal_energies",
+            "cluster_size": "cluster_size",
+            "cluster_id": "cluster_id",
+            "rank_in_cluster": "rank_in_cluster",
         }
         props = {}
+        if only_cluster_leads:
+            nr_poses = len(pdbqt_mol._pose_data["cluster_leads_sorted"])
+            pose_idxs = pdbqt_mol._pose_data["cluster_leads_sorted"]
+        else:
+            nr_poses = pdbqt_mol._pose_data["n_poses"]
+            pose_idxs = list(range(nr_poses))
         for prop_sdf, prop_pdbqt in property_names.items():
-            if nr_conformers == len(pdbqt_mol._pose_data[prop_pdbqt]):
+            if nr_conformers == nr_poses:
                 props[prop_sdf] = prop_pdbqt
+        has_all_data = True
+        for _, key in props.items():
+            has_all_data &= len(pdbqt_mol._pose_data[key]) == nr_conformers
         for conformer in combined_mol.GetConformers():
             i = conformer.GetId()
-            data = {k: pdbqt_mol._pose_data[v][i] for k, v in props.items()}
-            if len(data): combined_mol.SetProp("meeko", json.dumps(data))
+            j = pose_idxs[i]
+            if has_all_data:
+                data = {k: pdbqt_mol._pose_data[v][j] for k, v in props.items()}
+                if len(data): combined_mol.SetProp("meeko", json.dumps(data))
             f.write(combined_mol, i)
         f.close()
         output_string = sio.getvalue()
         return output_string, failures
```

### Comparing `meeko-0.4.0/meeko/utils/autodock4_atom_types_elements.py` & `meeko-0.5.0/meeko/utils/autodock4_atom_types_elements.py`

 * *Files identical despite different names*

### Comparing `meeko-0.4.0/meeko/utils/covalent_radius_table.py` & `meeko-0.5.0/meeko/utils/covalent_radius_table.py`

 * *Files identical despite different names*

### Comparing `meeko-0.4.0/meeko/utils/geomutils.py` & `meeko-0.5.0/meeko/utils/geomutils.py`

 * *Files identical despite different names*

### Comparing `meeko-0.4.0/meeko/utils/obutils.py` & `meeko-0.5.0/meeko/utils/obutils.py`

 * *Files identical despite different names*

### Comparing `meeko-0.4.0/meeko/utils/rdkitutils.py` & `meeko-0.5.0/meeko/utils/rdkitutils.py`

 * *Files identical despite different names*

### Comparing `meeko-0.4.0/meeko/utils/utils.py` & `meeko-0.5.0/meeko/utils/utils.py`

 * *Files identical despite different names*

### Comparing `meeko-0.4.0/meeko/utils/van_der_waals_radius_table.py` & `meeko-0.5.0/meeko/utils/van_der_waals_radius_table.py`

 * *Files identical despite different names*

### Comparing `meeko-0.4.0/meeko.egg-info/PKG-INFO` & `meeko-0.5.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meeko
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python package for preparing small molecule for docking
 Home-page: https://github.com/ccsb-scripps/meeko
 Author: Forli Lab
 Author-email: forli@scripps.edu
 License: LGPL-2.1
 Keywords: molecular modeling,drug design,docking,autodock
 Classifier: Environment :: Console
@@ -21,47 +21,77 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.5.*
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Meeko: preparation of small molecules for AutoDock
 
-[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![API stability](https://img.shields.io/badge/stable%20API-no-orange)](https://shields.io/)
-[![PyPI version fury.io](https://img.shields.io/badge/version-0.4.0-green.svg)](https://pypi.python.org/pypi/ansicolortags/)
+[![PyPI version fury.io](https://img.shields.io/badge/version-0.5.0-green.svg)](https://pypi.python.org/pypi/ansicolortags/)
 
 Meeko reads an RDKit molecule object and writes a PDBQT string (or file)
 for [AutoDock-Vina](https://github.com/ccsb-scripps/AutoDock-Vina)
 and [AutoDock-GPU](https://github.com/ccsb-scripps/AutoDock-GPU).
 It converts the docking output to RDKit molecules and
 SD files, without loss of bond orders.
 
 Meeko is developed by the [Forli lab](https://forlilab.org/) at the
 [Center for Computational Structural Biology (CCSB)](https://ccsb.scripps.edu)
 at [Scripps Research](https://www.scripps.edu/).
 
+
 ## Usage notes
+
 Meeko does not calculate 3D coordinates or assign protonation states.
 Input molecules must have explicit hydrogens.
 
 Sampling of macrocycle conformers ([paper](https://doi.org/10.1017/qrd.2022.18))
 is enabled by default.
 
-## Recent changes
+SDF format strongly preferred over Mol2.
+See
+[this discussion](https://github.com/rdkit/rdkit/discussions/3647)
+and RDKit issues
+[1755](https://github.com/rdkit/rdkit/issues/1755) and
+[917](https://github.com/rdkit/rdkit/issues/917).
+
 
-The Python API for creating RDKit molecules from docking results changed in `v0.4.0`.
-See [example below](#2.-rdkit-molecule-from-docking-results).
+## API changes in v0.5
+
+Class `MoleculePreparation` no longer has method `write_pdbqt_string()`.
+Instead, `MoleculePreparation.prepare()` returns a list of `MoleculeSetup` objects
+that must be passed, individually, to `PDBQTWriterLegacy.write_string()`.
+```python
+from meeko import MoleculePreparation
+from meeko import PDBQTWriterLegacy
 
-The `--pH` option was removed since `v0.3.0`. See issue https://github.com/forlilab/Meeko/issues/11 for more info.
+preparator = MoleculePreparation()
+mol_setups = preparator.prepare(rdkit_molecule_3D_with_Hs)
+for setup in mol_setups:
+    pdbqt_string, is_ok, error_msg = PDBQTWriterLegacy.write_string(setup)
+    if is_ok:
+        print(pdbqt_string, end="")
+```
+
+Argument `keep_nonpolar_hydrogens` is replaced by `merge_these_atom_types`, both in the Python
+interface and for script `mk_prepare_ligand.py`.
+The default is `merge_these_atom_types=("H",)`, which
+merges hydrogens typed `"H"`, keeping the current default behavior.
+To keep all hydrogens, set `merge_these_atom_types` to an empty
+list when initializing `MoleculePreparation`, or pass no atom types
+to `--merge_these_atom_types` from the command line:
+```sh
+mk_prepare_ligand.py -i molecule.sdf --merge_these_atom_types
+``` 
 
 ## Dependencies
 
 * Python (>=3.5)
 * Numpy
 * Scipy
 * RDKit
@@ -94,15 +124,15 @@
 ```
 
 
 ## Examples using the command line scripts
 
 #### 1. make PDBQT files
 AutoDock-GPU and Vina read molecules in the PDBQT format. These can be prepared
-by Meeko from SD files, or from Mol2 files, but SDF is preferred.
+by Meeko from SD files, or from Mol2 files, but SDF is strongly preferred.
 ```console
 mk_prepare_ligand.py -i molecule.sdf -o molecule.pdbqt
 mk_prepare_ligand.py -i multi_mol.sdf --multimol_outdir folder_for_pdbqt_files
 ```
 
 #### 2. convert docking results to SDF
 AutoDock-GPU and Vina write docking results in the PDBQT format. The DLG output
@@ -130,24 +160,26 @@
 
 ## Python tutorial
 
 #### 1. making PDBQT strings for Vina or for AutoDock-GPU
 
 ```python
 from meeko import MoleculePreparation
+from meeko import PDBQTWriterLegacy
 from rdkit import Chem
 
 input_molecule_file = "example/BACE_macrocycle/BACE_4.sdf"
 
 # there is one molecule in this SD file, this loop iterates just once
 for mol in Chem.SDMolSupplier(input_molecule_file, removeHs=False):
     preparator = MoleculePreparation()
-    preparator.prepare(mol)
-    preparator.show_setup() # optional
-    pdbqt_string = preparator.write_pdbqt_string()
+    mol_setups = preparator.prepare(mol)
+    for setup in mol_setups:
+        setup.show() # optional
+        pdbqt_string = PDBQTWriterLegacy.write_string(setup)
 ```
 At this point, `pdbqt_string` can be written to a file for
 docking with AutoDock-GPU or Vina, or passed directly to Vina within Python
 using `set_ligand_from_string(pdbqt_string)`. For context, see
 [the docs on using Vina from Python](https://autodock-vina.readthedocs.io/en/latest/docking_python.html).
 
 
@@ -259,7 +291,70 @@
     -i ligand_including_cys_sidechain.sdf\
     --receptor protein.pdb\
     --rec_residue ":CYS:6"\
     --tether_smarts "NC(=O)C(O)(C)SCC"\
     --tether_smarts_indices 9 8\
     -o prepared.pdbqt
 ```
+
+## Reactive Docking
+
+### 1. Prepare protein with waterkit
+Follow `wk_prepare_receptor.py` instructions and run with `--pdb`.
+The goal of this step is to perform essential fixes to the protein
+(such as missing atoms), to add hydrogens, and to follow the Amber
+naming scheme for atoms and residues, e.g., `HIE` or `HID`
+instead of `HIS`.
+
+### 2. Prepare protein pdbqt
+Here, `wk.pdb` was written by waterkit.
+Here, `wk.pdb` was written by waterkit. The example below will center a gridbox of specified size on the given reactive residue.
+
+```console
+   $ mk_prepare_receptor.py\
+    --pdb wk.pdb\
+    -o receptor.pdbqt\
+    --flexres " :ARG:348"\
+    --reactive_flexres " :SER:308"
+    --reactive_flexres " :SER:308"\
+    --box_center_on_reactive_res\
+    --box_size 40 40 40  # x y z (angstroms)
+```
+A manual box center can be specified with `--box_center`.
+Reactive parameters can also be modified:
+```sh
+  --r_eq_12 R_EQ_12     r_eq for reactive atoms (1-2 interaction)
+  --eps_12 EPS_12       epsilon for reactive atoms (1-2 interaction)
+  --r_eq_13_scaling R_EQ_13_SCALING
+                        r_eq scaling for 1-3 interaction across reactive atoms
+  --r_eq_14_scaling R_EQ_14_SCALING
+                        r_eq scaling for 1-4 interaction across reactive atoms
+```
+
+Receptor preparation can't handle heteroatoms for the moment.
+Also nucleic acids, ions, and post-translational modifications (e.g.
+phosphorilation) are not supported. Only the 20 standard amino acids
+can be parsed, and it is required to have Amber atom names and
+hydrogens. No atoms can be missing.
+
+### 3. Run autogrid
+
+Make affinity maps for the `_rigid.pdbqt` part of the receptor.
+Make affinity maps for the `_rigid.pdbqt` part of the receptor. `mk_prepare_receptor.py` will prepare the GPF for you.
+
+### 4. Write ligand PDBQT
+mk_prepare_ligand.py -i sufex1.sdf --reactive_smarts "S(=O)(=O)F" --reactive_smarts_idx 1 -o sufex1.pdbqt\
+
+### 5. Configure AD-GPU for reactive docking
+
+For reactive docking there are two options that need to be passed to AutoDock-GPU:
+For reactive docking there are an additional option that needs to be passed to AutoDock-GPU:
+    ```console
+    --import_dpf
+    ```
+
+The `--derivtype` option, if needed, was written by `mk_prepare_receptor.py` to a file suffixed with `.derivtype`.
+
+The filename to be passed to `--import_dpf` was written by `mk_prepare_receptor.py`
+and it is suffixed with `reactive_config`.
+```sh
+ADGPU -I *.reactive_config -L sufex1.pdbqt -N sufex1_docked_ -F *_flex.pdbqt -C 1
```

### Comparing `meeko-0.4.0/meeko.egg-info/SOURCES.txt` & `meeko-0.5.0/meeko.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -2,38 +2,43 @@
 README.md
 setup.py
 meeko/__init__.py
 meeko/atomtyper.py
 meeko/bondtyper.py
 meeko/covalentbuilder.py
 meeko/flexibility.py
+meeko/gridbox.py
 meeko/hydrate.py
 meeko/macrocycle.py
 meeko/molecule_pdbqt.py
 meeko/molsetup.py
 meeko/preparation.py
 meeko/rdkit_mol_create.py
+meeko/reactive.py
 meeko/receptor_pdbqt.py
 meeko/writer.py
 meeko.egg-info/PKG-INFO
 meeko.egg-info/SOURCES.txt
 meeko.egg-info/dependency_links.txt
 meeko.egg-info/not-zip-safe
 meeko.egg-info/requires.txt
 meeko.egg-info/top_level.txt
 meeko/analysis/__init__.py
 meeko/analysis/fingerprint_interactions.py
 meeko/analysis/interactions.py
 meeko/data/atomtypes.txt
+meeko/data/flexres_templates.json
 meeko/data/pi_non_aromatic.txt
+meeko/data/residue_params.json
 meeko/data/waterfield.txt
 meeko/utils/__init__.py
 meeko/utils/autodock4_atom_types_elements.py
 meeko/utils/covalent_radius_table.py
 meeko/utils/geomutils.py
 meeko/utils/obutils.py
 meeko/utils/pdbutils.py
 meeko/utils/rdkitutils.py
 meeko/utils/utils.py
 meeko/utils/van_der_waals_radius_table.py
 scripts/mk_export.py
-scripts/mk_prepare_ligand.py
+scripts/mk_prepare_ligand.py
+scripts/mk_prepare_receptor.py
```

### Comparing `meeko-0.4.0/scripts/mk_export.py` & `meeko-0.5.0/scripts/mk_export.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
 #
 
 import argparse
+import gzip
 import os
 import sys
 import warnings
 
 from rdkit import Chem
 
 from meeko import PDBQTMolecule
@@ -20,15 +21,15 @@
     _has_openbabel = False
 else:
     _has_openbabel = True
 
 
 def cmd_lineparser():
     parser = argparse.ArgumentParser(description='Export docking results to SDF format')
-    parser.add_argument(dest='docking_results_filename',
+    parser.add_argument(dest='docking_results_filename', nargs = "+",
                         action='store', help='Docking output file, either a PDBQT \
                         file from Vina or a DLG file from AD-GPU.')
     parser.add_argument('-i', '--original_input', dest='template_filename',
                         action='store', help='[not recommended] Template molecule file, i.e. the original \
                         file that was used to prepare the PDBQT filename (hopefully SDF). \
                         This option requires OpenBabel, and is kept only for backwards compatibility with \
                         meeko v0.2.* and older, because it is only since v0.3.* that the SMILES string is \
@@ -37,30 +38,44 @@
                         action='store', help='Output molecule filename. If not specified, suffix _docked is \
                         added to the filename based on the input molecule file, and using the same \
                         molecule file format')
     parser.add_argument('-s', '--suffix', dest='suffix_name', default='_docked',
                         action='store', help='Add suffix to output filename if -o/--output_filename \
                         not specified. WARNING: If specified as empty string (\'\'), this will overwrite \
                         the original molecule input file (default: _docked).')
+    parser.add_argument('-c', '--only_cluster_leads', action='store_true',
+                        help='Keep top pose from each AutoDock-GPU cluster, sorted by \
+                        predicted free energy of cluster lead.')
     parser.add_argument('-', '--',  dest='redirect_stdout', action='store_true',
                         help='do not write file, redirect output to STDOUT. Arguments -o/--output_filename \
                         is ignored.')
     return parser.parse_args()
 
+args = cmd_lineparser()
 
-if __name__ == '__main__':
-    args = cmd_lineparser()
-    docking_results_filename = args.docking_results_filename
-    template_filename = args.template_filename
-    output_filename = args.output_filename
-    suffix_name = args.suffix_name
-    redirect_stdout = args.redirect_stdout
-
-    is_dlg = docking_results_filename.endswith('.dlg')
-    pdbqt_mol = PDBQTMolecule.from_file(docking_results_filename, is_dlg=is_dlg, skip_typing=True)
+docking_results_filenames = args.docking_results_filename
+template_filename = args.template_filename
+output_filename = args.output_filename
+suffix_name = args.suffix_name
+only_cluster_leads = args.only_cluster_leads
+redirect_stdout = args.redirect_stdout
+
+if output_filename is not None and len(docking_results_filenames) > 1:
+    print("Option -o/--output_filename incompatible with multiple input files", file=sys.stderr)
+    sys.exit()
+ 
+for filename in docking_results_filenames:
+    is_dlg = filename.endswith('.dlg') or filename.endswith(".dlg.gz")
+    if filename.endswith(".gz"):
+        with gzip.open(filename) as f:
+            string = f.read().decode()
+    else:
+        with open(filename) as f:
+            string = f.read()
+    pdbqt_mol = PDBQTMolecule(string, is_dlg=is_dlg, skip_typing=True)
 
     if template_filename is not None: # OBMol from template_filename
         if not _has_openbabel:
             raise ImportError('-i/--original_input requires openbabel which is not available')
         if output_filename is not None:
             output_format = os.path.splitext(output_filename)[1][1:]
         else:
@@ -71,24 +86,26 @@
             raise RuntimeError('Input molecule file format %s not recognized by OpenBabel.' % output_format)
         ori_obmol = obutils.load_molecule_from_file(template_filename)
         for pose in pdbqt_mol:
             copy_obmol = ob.OBMol(ori_obmol) # connectivity may be corrupted by removing and adding Hs multiple times
             pose.copy_coordinates_to_obmol(copy_obmol)
             output_string = conv.WriteString(copy_obmol)
     else: # RDKit mol from SMILES in docking output PDBQT remarks
-        output_string, failures = RDKitMolCreate.write_sd_string(pdbqt_mol)
+        output_string, failures = RDKitMolCreate.write_sd_string(
+                pdbqt_mol, only_cluster_leads=only_cluster_leads)
         output_format = 'sdf'
         for i in failures:
             warnings.warn("molecule %d not converted to RDKit/SD File" % i)
         if len(failures) == len(pdbqt_mol._atom_annotations["mol_index"]):
             msg = "\nCould not convert to RDKit. Maybe meeko was not used for preparing\n"
             msg += "the input PDBQT for docking, and the SMILES string is missing?\n"
             msg += "Except for standard protein sidechains, all ligands and flexible residues\n"
             msg += "require a REMARK SMILES line in the PDBQT, which is added automatically by meeko."
             raise RuntimeError(msg)
     if not redirect_stdout:
         if output_filename is None:
-            output_filename = '%s%s.%s' % (os.path.splitext(docking_results_filename)[0], suffix_name, output_format)
-
-        print(output_string, file=open(output_filename, 'w'))
+            fn = '%s%s.%s' % (os.path.splitext(filename)[0], suffix_name, output_format)
+        else:
+            fn = output_filename
+        print(output_string, file=open(fn, 'w'))
     else:
         print(output_string)
```

### Comparing `meeko-0.4.0/scripts/mk_prepare_ligand.py` & `meeko-0.5.0/scripts/mk_prepare_ligand.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import json
 import warnings
 
 from rdkit import Chem
 
 from meeko import MoleculePreparation
 from meeko import rdkitutils
+from meeko import PDBQTWriterLegacy
 
 try:
     import prody
     from meeko import CovalentBuilder
     _prody_parsers = {'pdb': prody.parsePDB, 'mmcif': prody.parseMMCIF}
     warnings.warn("Prody not available, covalent docking won't work", ImportWarning)
 except:
@@ -74,33 +75,41 @@
             help='configure MoleculePreparation from JSON file. Overriden by command line args.') # parsed above by conf_parser, here for help msg
     config_group.add_argument("--rigid_macrocycles",dest="rigid_macrocycles",
                         action="store_true", help="keep macrocycles rigid in input conformation")
     config_group.add_argument("--keep_chorded_rings",dest="keep_chorded_rings",
                         action="store_true", help="return all rings from exhaustive perception")
     config_group.add_argument("--keep_equivalent_rings",dest="keep_equivalent_rings",
                         action="store_true", help="equivalent rings have the same size and neighbors")
+    config_group.add_argument("--min_ring_size", dest="min_ring_size",
+                        type=int, help="min nr of atoms in ring for opening")
     config_group.add_argument("-w", "--hydrate", dest="hydrate",
                         action="store_true", help="add water molecules for hydrated docking")
-    config_group.add_argument("--keep_nonpolar_hydrogens", dest="keep_nonpolar_hydrogens",
-                        action="store_true", help="keep non-polar hydrogens (default: merge onto heavy atom)")
+    config_group.add_argument("--merge_these_atom_types", dest="merge_these_atom_types", nargs="*",
+                        help="list of atom types to merge, default is \"H\"", default=["H"])
     config_group.add_argument("-r", "--rigidify_bonds_smarts", dest="rigidify_bonds_smarts",
                         action="append", help="SMARTS patterns to rigidify bonds",
                         metavar='SMARTS')
     config_group.add_argument("-b", "--rigidify_bonds_indices", dest="rigidify_bonds_indices",
                         action="append", help="indices of two atoms (in the SMARTS) that define a bond (start at 1)",
                         nargs='+', type=int, metavar='i j')
     config_group.add_argument("-a", "--flexible_amides", dest="flexible_amides",
                         action="store_true", help="allow amide bonds to rotate and be non-planar, which is bad")
     config_group.add_argument("-p", "--atom_type_smarts", dest="atom_type_smarts_json",
                         action="store", help="SMARTS based atom typing (JSON format)")
+    config_group.add_argument("-aa", "--add_atom_types", dest="add_atom_types_json",
+                        action="append", help="Additional atom types to assign (JSON formated)", metavar="[{'smarts': '<smarts pattern>', 'atype': ',atomtype name>'}, {'smarts': '<smarts pattern>', 'atype': ',atomtype name>'}]")
     config_group.add_argument("--double_bond_penalty", help="penalty > 100 prevents breaking double bonds", type=int)
+    config_group.add_argument("--bad_charge_ok", help="NaN and Inf charges allowed in PDBQT", action="store_true")
     config_group.add_argument("--add_index_map", dest="add_index_map",
                         action="store_true", help="write map of atom indices from input to pdbqt")
     config_group.add_argument("--remove_smiles", dest="remove_smiles",
                         action="store_true", help="do not write smiles as remark to pdbqt")
+    reactive_group = parser.add_argument_group("Reactive docking")
+    reactive_group.add_argument('--reactive_smarts',  help="SMARTS pattern for reactive group")
+    reactive_group.add_argument('--reactive_smarts_idx', help='index (1-based) of the reactive atom in --reactive_smarts', type=int)
 
     need_prody_msg = ''
     if not _has_prody: need_prody_msg = ". Needs Prody which is unavailable"
     covalent_group = parser.add_argument_group("Covalent docking (tethered)%s" % (need_prody_msg))
     covalent_group.add_argument('--receptor', help='receptor filename. Supported formats: [%s]%s' % (
         '/'.join(list(_prody_parsers.keys())),
         need_prody_msg))
@@ -110,22 +119,42 @@
                                 help='SMARTS pattern to define ligand atoms for receptor attachment')
     covalent_group.add_argument('--tether_smarts_indices', type=int, nargs=2, required=False,
                                 metavar='IDX', default=[1, 2],
                                 help='indices (1-based) of the SMARTS atoms that will be attached (default: 1 2)')
 
     args = parser.parse_args(remaining_argv)
 
+    # check reactive arguments
+    if (args.reactive_smarts is None) != (args.reactive_smarts_idx is None):
+        print("Arguments --reactive_smarts and --reactive_smarts_idx require each other", file=sys.stderr)
+        sys.exit(2)
+    elif args.reactive_smarts_idx is not None:
+        if args.reactive_smarts_idx < 1:
+            print("--reactive_smarts_idx is 1-indexed, but got %d" % args.reactive_smarts_idx, file=sys.stderr)
+            sys.exit(2)
+        args.reactive_smarts_idx -= 1 # convert from 1- to 0-index
+
     # command line arguments override config
     for key in config:
         if key in args.__dict__:
             config[key] = args.__dict__[key]
 
     if args.atom_type_smarts_json is not None:
         with open(args.atom_type_smarts_json) as f:
             config['atom_type_smarts'] = json.load(f)
+    
+    if args.add_atom_types_json is not None:
+        additional_ats = []
+        for at in args.add_atom_types_json:
+            at = json.loads(at)
+            if type(at) == dict:
+                additional_ats.append(at)
+            elif type(at) == list:
+                additional_ats.extend(at)
+        config['add_atom_types'] = additional_ats
 
     if args.multimol_output_dir is not None or args.multimol_prefix is not None:
         if args.output_pdbqt_filename is not None:
             print("Warning: -o/--out ignored with --multimol_outdir or --multimol_prefix", file=sys.stderr)
         if args.redirect_stdout:
             print("Warning: -/-- ignored with --multimol_outdir or --multimol_prefix", file=sys.stderr)
 
@@ -136,14 +165,17 @@
     num_required_covalent_args += int(args.tether_smarts is not None)
     if num_required_covalent_args not in [0, 3]:
         print("Error: --receptor, --rec_residue, and --tether_smarts are all required for covalent docking.")
         sys.exit(2)
     is_covalent = num_required_covalent_args == 3
     if is_covalent and not _has_prody:
         raise ImportError("Covalent docking requires Prody which is not available")
+    if min(args.tether_smarts_indices) < 1:
+        print("--tether_smarts_indices is 1-indexed, all values must be greater than zero", file=sys.stderr) 
+        sys.exit(2)
     args.tether_smarts_indices = [i-1 for i in args.tether_smarts_indices] # convert to 0-index
 
     # verify sanity of SMARTS patterns to make bonds rigid and convert to 0-based indices
     rigidify_bonds_smarts = config['rigidify_bonds_smarts']
     rigidify_bonds_indices = config['rigidify_bonds_indices']
     if len(rigidify_bonds_indices) != len(rigidify_bonds_smarts):
         raise RuntimeError('length of --rigidify_bonds_indices differs from length of --rigidify_bonds_smarts')
@@ -166,29 +198,29 @@
         self.multimol_output_dir = multimol_output_dir
         self.multimol_prefix = multimol_prefix
         self.redirect_stdout = redirect_stdout
         self.output_filename = output_filename
         self.is_multimol = is_multimol
         self.visited_filenames = set()
         self.duplicate_filenames = set()
-        self.visited_molnames = set()
-        self.duplicate_molnames = set()
+        self.visited_names = set()
+        self.duplicate_names = set()
         self.num_files_written = 0
         self.counter = 0
 
-    def __call__(self, pdbqt_string, mol_name, sufix=None):
+    def __call__(self, pdbqt_string, name, suffixes=()):
         self.counter += 1
-        if mol_name in self.visited_molnames:
-            self.duplicate_molnames.add(mol_name)
-        self.visited_molnames.add(mol_name)
-        name = mol_name
+        if name in self.visited_names:
+            self.duplicate_names.add(name)
+        self.visited_names.add(name)
         if self.multimol_prefix is not None:
             name = '%s-%d' % (args.multimol_prefix, self.counter)
-        if sufix is not None:
-            name += '_%s' % sufix
+        for suffix in suffixes:
+            if suffix is not None and len(suffix) > 0:
+                name += "_" + suffix
         if self.is_multimol:
             if name in self.visited_filenames:
                 self.duplicate_filenames.add(name)
                 repeat_id = 1
                 newname = name + "-again%d" % repeat_id
                 while newname in self.visited_filenames:
                     repeat_id += 1
@@ -214,26 +246,33 @@
         if multimol_output_dir is not None:
             if not os.path.exists(multimol_output_dir):
                 os.mkdir(multimol_output_dir)
 
     def get_duplicates_info_string(self):
         if not self.is_multimol:
             return None
-        if len(self.duplicate_molnames):
+        if len(self.duplicate_names):
             # with multimol_prefix with can have duplicate molecule names,
             # but not duplicate filenames. This warning is for such cases.
-            string = "Warning: %d molecules have duplicated names" % len(self.duplicate_molnames)
+            string = "Warning: %d molecules have duplicated names" % len(self.duplicate_names)
         else:
             string = "No duplicate molecule molecule names were found"
         # if we have duplicate_filenames, we also have duplicate molecule names,
         # but it suffices to return the string below
         if len(self.duplicate_filenames):
             string = "Warning: %d molecules with repeated names were suffixed with -again<n>" % len(self.duplicate_filenames)
         return string
 
+    @staticmethod
+    def get_suffixes(molsetups):
+        if len(molsetups) == 1:
+            return ("",) # no suffix needed
+        else:
+            return tuple("mk%d" % (i + 1) for i in range(len(molsetups)))
+
 
 if __name__ == '__main__':
 
     args, config, backend, is_covalent = cmd_lineparser()
     input_molecule_filename = args.input_molecule_filename
 
     # read input
@@ -254,27 +293,30 @@
         output_filename = input_fname + '.pdbqt'
     else:
         output_filename = args.output_pdbqt_filename
     output = Output(
             args.multimol_output_dir,
             args.multimol_prefix,
             args.redirect_stdout,
-            output_filename)
+            output_filename,
+            )
 
     # initialize covalent object for receptor
     if is_covalent:
         rec_filename = args.receptor
         _, rec_extension = os.path.splitext(rec_filename)
         rec_extension = rec_extension[1:].lower()
-        parser = _prody_parsers[rec_extension]
-        rec_mol = parser(rec_filename) # rec_mol is a prody molecule
-        covalent_builder = CovalentBuilder(rec_mol, args.rec_residue)
+        prody_parser = _prody_parsers[rec_extension]
+        rec_prody_mol = prody_parser(rec_filename)
+        covalent_builder = CovalentBuilder(rec_prody_mol, args.rec_residue)
 
     input_mol_counter = 0
     input_mol_skipped = 0
+    input_mol_with_failure = 0 # if reactive or covalent, each mol can yield multiple PDBQT
+    nr_failures = 0
     is_after_first = False
     preparator = MoleculePreparation.from_config(config)
     for mol in mol_supplier:
         if is_after_first and output.is_multimol == False:
             print("Processed only the first molecule of multiple molecule input.")
             print("Use --multimol_prefix and/or --multimol_outdir to process all molecules in %s." % (
                 input_molecule_filename))
@@ -285,27 +327,49 @@
         if backend == 'rdkit':
             is_valid = mol is not None
         elif backend == 'ob':
             is_valid = mol.NumAtoms() > 0
         input_mol_skipped += int(is_valid==False)
         if not is_valid: continue
 
+        this_mol_had_failure = False
+
         if is_covalent:
             for cov_lig in covalent_builder.process(mol, args.tether_smarts, args.tether_smarts_indices):
                 root_atom_index = cov_lig.indices[0]
-                preparator.prepare(cov_lig.mol, root_atom_index=root_atom_index, not_terminal_atoms=[root_atom_index])
-                pdbqt_string = preparator.write_pdbqt_string()
+                molsetups = preparator.prepare(cov_lig.mol, root_atom_index=root_atom_index, not_terminal_atoms=[root_atom_index])
                 res, chain, num = cov_lig.res_id
-                pdbqt_string = preparator.adapt_pdbqt_for_autodock4_flexres(pdbqt_string, res, chain, num)
-                mol_name = preparator.setup.name
-                output(pdbqt_string, mol_name, sufix=cov_lig.label)
+                suffixes = output.get_suffixes(molsetups)
+                for molsetup, suffix in zip(molsetups, suffixes):
+                    pdbqt_string, success, error_msg = PDBQTWriterLegacy.write_string(molsetup, bad_charge_ok=args.bad_charge_ok)
+                    if success:
+                        pdbqt_string = PDBQTWriterLegacy.adapt_pdbqt_for_autodock4_flexres(pdbqt_string, res, chain, num)
+                        name = molsetup.name
+                        output(pdbqt_string, name, (cov_lig.label, suffix))
+                    else:
+                        nr_failures += 1
+                        this_mol_had_failure = True
+                        print(error_msg, file=sys.stderr)
+                        
         else:
-            preparator.prepare(mol)
-            pdbqt_string = preparator.write_pdbqt_string()
-            mol_name = preparator.setup.name # setup.name may be None
-            output(pdbqt_string, mol_name)
+            molsetups = preparator.prepare(mol)
+            suffixes = output.get_suffixes(molsetups) 
+            for molsetup, suffix in zip(molsetups, suffixes):
+                pdbqt_string, success, error_msg = PDBQTWriterLegacy.write_string(molsetup, bad_charge_ok=args.bad_charge_ok)
+                if success:
+                    name = molsetup.name
+                    output(pdbqt_string, name, (suffix,))
+                else:
+                    nr_failures += 1
+                    this_mol_had_failure = True
+                    print(error_msg, file=sys.stderr)
+                    
             if args.verbose: preparator.show_setup()
 
+        input_mol_with_failure += int(this_mol_had_failure)
+
     if output.is_multimol:
         print("Input molecules processed: %d, skipped: %d" % (output.counter, input_mol_skipped))
         print("PDBQT files written: %d" % (output.num_files_written))
+        print("PDBQT files not written due to error: %d" % (nr_failures))
+        print("Input molecules with errors: %d" % (input_mol_with_failure))
         print(output.get_duplicates_info_string())
```

### Comparing `meeko-0.4.0/setup.py` & `meeko-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,34 +17,36 @@
             matches.append(os.path.join(root, filename))
 
     return matches
 
 
 setup(
     name="meeko",
-    version='0.4.0',
+    version='0.5.0',
     author="Forli Lab",
     author_email="forli@scripps.edu",
     url="https://github.com/ccsb-scripps/meeko",
     description='Python package for preparing small molecule for docking',
     long_description=open(os.path.join(base_dir, 'README.md')).read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
     scripts=["scripts/mk_prepare_ligand.py",
-             "scripts/mk_export.py"],
+             "scripts/mk_prepare_receptor.py",
+             "scripts/mk_export.py",
            #"scripts/dry.py",
            #"scripts/mapwater.py",
            #"scripts/wet.py"],
+            ],
     package_data={"meeko" : ["data/*"]},
     data_files=[("", ["README.md", "LICENSE"]),
                 ("scripts", find_files("scripts"))],
     include_package_data=True,
     zip_safe=False,
     install_requires=['numpy>=1.18'],
-    python_requires='>=3.5.*',
+    python_requires='>=3.5',
     license="LGPL-2.1",
     keywords=["molecular modeling", "drug design",
             "docking", "autodock"],
     classifiers=[
         'Environment :: Console',
         'Environment :: Other Environment',
         'Intended Audience :: Education',
```

