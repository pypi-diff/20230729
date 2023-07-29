# Comparing `tmp/wwpdb.utils.emdb-1.4.3.tar.gz` & `tmp/wwpdb.utils.emdb-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.utils.emdb-1.4.3.tar", last modified: Mon Jul  3 15:25:41 2023, max compression
+gzip compressed data, was "wwpdb.utils.emdb-1.5.tar", last modified: Sat Jul 29 12:25:02 2023, max compression
```

## Comparing `wwpdb.utils.emdb-1.4.3.tar` & `wwpdb.utils.emdb-1.5.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-03 15:25:41.669876 wwpdb.utils.emdb-1.4.3/
--rw-r--r--   0 vsts      (1001) docker     (123)      106 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)      721 2023-07-03 15:25:41.669876 wwpdb.utils.emdb-1.4.3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)       46 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-07-03 15:25:41.669876 wwpdb.utils.emdb-1.4.3/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2278 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-03 15:25:41.661876 wwpdb.utils.emdb-1.4.3/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-03 15:25:41.665876 wwpdb.utils.emdb-1.4.3/wwpdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/wwpdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-03 15:25:41.665876 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/
--rw-r--r--   0 vsts      (1001) docker     (123)      322 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/EmdbSchema.py
--rw-r--r--   0 vsts      (1001) docker     (123)      145 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-03 15:25:41.665876 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/atomcheck/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/atomcheck/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7031 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/atomcheck/atomcheck.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-03 15:25:41.669876 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/cif_emdb_translator/
--rwxr-xr-x   0 vsts      (1001) docker     (123)      139 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/cif_emdb_translator/README.md
--rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/cif_emdb_translator/__init__.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)   667797 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     1866 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/cif_emdb_translator/em_emd_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (123)  2283184 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/cif_emdb_translator/emdb.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)      389 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/cif_emdb_translator/generatedsnamespaces.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     1196 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2490 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-03 15:25:41.669876 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/data/
--rw-r--r--   0 vsts      (1001) docker     (123)   217727 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/data/emdb-v3.xsd
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-03 15:25:41.665876 wwpdb.utils.emdb-1.4.3/wwpdb.utils.emdb.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      721 2023-07-03 15:25:41.000000 wwpdb.utils.emdb-1.4.3/wwpdb.utils.emdb.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      975 2023-07-03 15:25:41.000000 wwpdb.utils.emdb-1.4.3/wwpdb.utils.emdb.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-03 15:25:41.000000 wwpdb.utils.emdb-1.4.3/wwpdb.utils.emdb.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       87 2023-07-03 15:25:41.000000 wwpdb.utils.emdb-1.4.3/wwpdb.utils.emdb.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-03 15:25:21.000000 wwpdb.utils.emdb-1.4.3/wwpdb.utils.emdb.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)      101 2023-07-03 15:25:41.000000 wwpdb.utils.emdb-1.4.3/wwpdb.utils.emdb.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-07-03 15:25:41.000000 wwpdb.utils.emdb-1.4.3/wwpdb.utils.emdb.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:25:02.639000 wwpdb.utils.emdb-1.5/
+-rw-r--r--   0 vsts      (1001) docker     (123)      106 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)      719 2023-07-29 12:25:02.639000 wwpdb.utils.emdb-1.5/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)       46 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-07-29 12:25:02.639000 wwpdb.utils.emdb-1.5/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2278 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:25:02.631000 wwpdb.utils.emdb-1.5/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:25:02.635000 wwpdb.utils.emdb-1.5/wwpdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/wwpdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:25:02.635000 wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)      322 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/EmdbSchema.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      143 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:25:02.635000 wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/atomcheck/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/atomcheck/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7031 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/atomcheck/atomcheck.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:25:02.639000 wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/cif_emdb_translator/
+-rwxr-xr-x   0 vsts      (1001) docker     (123)      139 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/cif_emdb_translator/README.md
+-rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/cif_emdb_translator/__init__.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)   676573 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     1866 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/cif_emdb_translator/em_emd_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (123)  2305255 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/cif_emdb_translator/emdb.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     1196 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2490 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:25:02.639000 wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/data/
+-rw-r--r--   0 vsts      (1001) docker     (123)   219087 2023-07-29 12:24:00.000000 wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/data/emdb-v3.xsd
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-29 12:25:02.635000 wwpdb.utils.emdb-1.5/wwpdb.utils.emdb.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      719 2023-07-29 12:25:02.000000 wwpdb.utils.emdb-1.5/wwpdb.utils.emdb.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      914 2023-07-29 12:25:02.000000 wwpdb.utils.emdb-1.5/wwpdb.utils.emdb.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-29 12:25:02.000000 wwpdb.utils.emdb-1.5/wwpdb.utils.emdb.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       87 2023-07-29 12:25:02.000000 wwpdb.utils.emdb-1.5/wwpdb.utils.emdb.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-29 12:24:44.000000 wwpdb.utils.emdb-1.5/wwpdb.utils.emdb.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      101 2023-07-29 12:25:02.000000 wwpdb.utils.emdb-1.5/wwpdb.utils.emdb.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-07-29 12:25:02.000000 wwpdb.utils.emdb-1.5/wwpdb.utils.emdb.egg-info/top_level.txt
```

### Comparing `wwpdb.utils.emdb-1.4.3/PKG-INFO` & `wwpdb.utils.emdb-1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.emdb
-Version: 1.4.3
+Version: 1.5
 Summary: wwPDB EMDB to XML converter
 Home-page: https://github.com/rcsb/py-wwpdb_utils_config
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.emdb-1.4.3/setup.py` & `wwpdb.utils.emdb-1.5/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/atomcheck/atomcheck.py` & `wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/atomcheck/atomcheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py` & `wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,16 @@
 
     class Constants(object):
         """
         There are many constants in use for the translation.
         They have been collected here for ease of use.
         """
 
-        XML_OUT_VERSION = "3.0.4.0"
+        XML_OUT_VERSION = "3.0.7.2"
+        XML_VERSION = XML_OUT_VERSION.replace('.', '_')
 
         # Cif categories
         CITATION = "citation"
         CITATION_AUTHOR = "citation_author"
         DATABASE_2 = "database_2"
         EM_ADMIN = "em_admin"
         EM_DEPUI = "em_depui"
@@ -211,18 +212,18 @@
         SOFT_CTF_CORRECTION = "CTF CORRECTION"
         SOFT_FINAL_EULER_ASSIGNMENT = "FINAL EULER ASSIGNMENT"
         SOFT_IMAGE_ACQUISITION = "IMAGE ACQUISITION"
         SOFT_INITIAL_EULER_ASSIGNMENT = "INITIAL EULER ASSIGNMENT"
         SOFT_MODEL_FITTING = "MODEL FITTING"
         SOFT_PARTICLE_SELECTION = "PARTICLE SELECTION"
         SOFT_RECONSTRUCTION = "RECONSTRUCTION"
-        MOLECULAR_REPLACEMENT = "MOLECULAR REPLACEMENT"
-        LATTICE_DISTORTION_CORRECTION = "LATTICE DISTORTION CORRECTION"
-        SYMMETRY_DETERMINATION = "SYMMETRY DETERMINATION"
-        CRYSTALLOGRAPHY_MERGING = "CRYSTALLOGRAPHY MERGING"
+        SOFT_MOLECULAR_REPLACEMENT = "MOLECULAR REPLACEMENT"
+        SOFT_LATTICE_DISTORTION_CORRECTION = "LATTICE DISTORTION CORRECTION"
+        SOFT_SYMMETRY_DETERMINATION = "SYMMETRY DETERMINATION"
+        SOFT_CRYSTALLOGRAPHY_MERGING = "CRYSTALLOGRAPHY MERGING"
 
         # EM methods
         EMM_EC = "electronCrystallography"
         EMM_HEL = "helical"
         EMM_SP = "singleParticle"
         EMM_STOM = "subtomogramAveraging"
         EMM_TOM = "tomography"
@@ -529,14 +530,15 @@
             "_em_entity_assembly_naturalsource.tissue": '<xs:element name="tissue" type="xs:token" minOccurs="0">',
             "_em_entity_assembly_naturalsource.cell": '<xs:element name="cell" type="xs:token" minOccurs="0">',
             "_em_entity_assembly_naturalsource.organelle": '<xs:element name="organelle" type="xs:token" minOccurs="0">',
             "_em_entity_assembly_naturalsource.cellular_location": '<xs:element name="cellular_location" type="xs:token" minOccurs="0">',
             "_em_entity_assembly_naturalsource.strain": '<xs:element name="sci_species_strain" type="xs:string" minOccurs="0" maxOccurs="1"/>',
             "_em_entity_assembly_naturalsource.ncbi_tax_id": '<xs:attribute name="database">',
             "_em_entity_assembly_naturalsource.organism": '<xs:element name="organism" type="organism_type"/>',
+            "_em_entity_assembly_naturalsource.details": '<xs:element name="details" type="xs:string" minOccurs="0"/>',
             "_em_entity_assembly_synthetic.organ": '<xs:element name="organ" type="xs:token" minOccurs="0"/>',
             "_em_entity_assembly_synthetic.tissue": '<xs:element name="tissue" type="xs:token" minOccurs="0">',
             "_em_entity_assembly_synthetic.cell": '<xs:element name="cell" type="xs:token" minOccurs="0">',
             "_em_entity_assembly_synthetic.organelle": '<xs:element name="organelle" type="xs:token" minOccurs="0">',
             "_em_entity_assembly_synthetic.cellular_location": '<xs:element name="cellular_location" type="xs:token" minOccurs="0">',
             "_em_entity_assembly_synthetic.strain": '<xs:element name="sci_species_strain" type="xs:string" minOccurs="0" maxOccurs="1"/>',
             "_em_entity_assembly_synthetic.ncbi_tax_id": '<xs:attribute name="database">',
@@ -723,14 +725,15 @@
             "_citation.page_first": '<xs:element name="first_page" type="page_type" nillable="false" minOccurs="0"/>',
             "_citation.page_last": '<xs:element name="last_page" type="page_type" minOccurs="0"/>',
             "_citation.year": '<xs:element name="year" minOccurs="0">',
             "_citation.language": '<xs:element name="language" type="xs:language" minOccurs="0"/>',
             "_citation.details": '<xs:element name="details" type="xs:string" minOccurs="0"/>',
             "_citation.book_title": '<xs:element name="title" type="xs:token"/>',
             "_citation.book_publisher": '<xs:element name="publisher" type="xs:token" minOccurs="0"/>',
+            "_pdbx_database_related.db_name": '<xs:element name="db_name" type="token"/>',
             "_pdbx_database_related.db_id": '<xs:element name="emdb_id" type="emdb_id_type"/>',
             "_pdbx_database_related.content_type": '<xs:element name="relationship" minOccurs="0">',
             "_pdbx_database_related.details": '<xs:element name="details" type="xs:string" minOccurs="0"/>',
             "_em_entity_assembly_recombinan.strain": '<xs:element name="recombinant_strain" type="xs:token" minOccurs="0"/>',
             "_em_entity_assembly_recombinan.cell": '<xs:element name="recombinant_cell" type="xs:token" minOccurs="0"/>',
             "_em_entity_assembly_recombinan.plasmid": '<xs:element name="recombinant_plasmid" type="xs:token" minOccurs="0"/>',
             "_entity.id": '<xs:attribute name="macromolecule_id" type="xs:positiveInteger" use="required"/>',
@@ -969,14 +972,21 @@
         self.error_log_string = None
         self.logger = None
         self.parent_logger_level = None
         self.translation_log = self.TranslationLog()
         self.entry_in_translation_log = None
         # create_xml enables the XML out to be created - if False the creation of the output file and its validation shouldn't happen
         self.create_xml = True
+        emdb.GenerateDSNamespaceDefs_ = {
+            "entry_type": 'xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" '
+                          'xsi:noNamespaceSchemaLocation="https://ftp.ebi.ac.uk/pub/databases/em_ebi/emdb_related/emdb-schemas/'
+                          'emdb_schemas/v3/v{0}/emdb.xsd" '
+                          'version="{1}"'.format(self.Constants.XML_VERSION, self.Constants.XML_OUT_VERSION)
+        }
+        emdb.GenerateDSNamespaceTypePrefixes_ = {}
 
     @property
     def is_translation_log_empty(self):
         logs = self.translation_log.logs
         if len(logs) == 0:
             return True
         else:
@@ -3209,15 +3219,15 @@
                     """
                     XSD: <xs:element name="pdb_list" type="pdb_cross_reference_list_type" minOccurs="0">
                     ..has only one element of
                     <xs:element name="pdb_reference" type="pdb_cross_reference_type" maxOccurs="unbounded">
                     ..is a sequence of 3 elements
                     """
 
-                    def set_el_emdb_id(pdb_ref, pdb_ref_in):
+                    def set_el_pdb_id(pdb_ref, pdb_ref_in):
                         """
                         XSD: <xs:element name="emdb_id" type="emdb_id_type"/>
                         CIF: _em_db_reference.access_code
                         """
                         set_cif_value(pdb_ref.set_pdb_id, "access_code", const.EM_DB_REFERENCE, cif_list=pdb_ref_in, fmt=str.lower, parent_el_req=False)
 
                     def set_el_relationship(pdb_ref, pdb_ref_in):
@@ -3252,26 +3262,86 @@
                     pdb_ref_list_in = x_ref_dict_in["PDB"]
                     for pdb_ref_in in pdb_ref_list_in:
                         el_emdb_id = get_cif_value("access_code", const.EM_DB_REFERENCE, cif_list=pdb_ref_in)
                         el_details = get_cif_value("details", const.EM_DB_REFERENCE)
                         if any(x is not None for x in [el_emdb_id, el_details]):
                             pdb_ref = emdb.pdb_cross_reference_type()
                             # element 1
-                            set_el_emdb_id(pdb_ref, pdb_ref_in)
+                            set_el_pdb_id(pdb_ref, pdb_ref_in)
                             # element 2
                             set_el_relationship(pdb_ref, pdb_ref_in)
                             # element 3
                             set_el_details(pdb_ref, pdb_ref_in)
 
                 if "PDB" in x_ref_dict_in:
                     pdb_ref_list = emdb.pdb_cross_reference_list_type()
                     set_pdb_cross_ref_list_type(pdb_ref_list, x_ref_dict_in)
                     if pdb_ref_list.has__content():
                         cross_references.set_pdb_list(pdb_ref_list)
 
+            def set_el_other_db_list(cross_references, other_db_ref_dict_in):
+                """
+                <xs:element name="other_db_list"
+                    type="other_cross_reference_list_type"
+                    minOccurs="0">
+                """
+
+                def set_other_db_cross_ref_list_type(other_db_ref_list, other_db_ref_dict_in):
+                    """
+                    XSD: <xs:element name="other_db_list" type="other_db_cross_reference_list_type" minOccurs="0">
+                    ..has only one element of
+                    <xs:element name="db_reference" type="db_cross_reference_type" maxOccurs="unbounded"/>
+                    ..is a sequence of 4 elements
+                    """
+
+                    def set_ref_el_db_name(other_db_ref, other_db_ref_in):
+                        """
+                        XSD: <xs:element name="db_name" type="token"/>
+                        CIF: _pdbx_database_related.db_name (MANDATORY)
+                        """
+                        set_cif_value(other_db_ref.set_db_name, "db_name", const.PDBX_DATABASE_RELATED, cif_list=other_db_ref_in)
+
+                    def set_ref_el_accession_id(other_db_ref, other_db_ref_in):
+                        """
+                        XSD: <xs:element name="accession_id" type="token"/>
+                        CIF: _pdbx_database_related.db_id (MANDATORY)
+                        """
+                        set_cif_value(other_db_ref.set_accession_id, "db_id", const.PDBX_DATABASE_RELATED, cif_list=other_db_ref_in)
+
+                    def set_ref_el_content_type(other_db_ref, other_db_ref_in):
+                        """
+                        XSD: <xs:element name="content_type" minOccurs="0" type="xs:string"/>
+                        CIF: _pdbx_database_related.details
+                        """
+                        set_cif_value(other_db_ref.set_content_type, "content_type", const.PDBX_DATABASE_RELATED, cif_list=other_db_ref_in)
+
+                    def set_ref_el_details(other_db_ref, other_db_ref_in):
+                        """
+                        XSD: <xs:element name="details" minOccurs="0" type="xs:string"/>
+                        CIF: _pdbx_database_related.details
+                        """
+                        set_cif_value(other_db_ref.set_details, "details", const.PDBX_DATABASE_RELATED, cif_list=other_db_ref_in)
+
+                    if "SASBDB" in other_db_ref_dict_in:
+                        other_db_ref_list_in = other_db_ref_dict_in["SASBDB"]
+                        for other_db_ref_in in other_db_ref_list_in:
+                            other_db_ref = emdb.other_db_cross_reference_type()
+                            set_ref_el_db_name(other_db_ref, other_db_ref_in)
+                            set_ref_el_accession_id(other_db_ref, other_db_ref_in)
+                            set_ref_el_content_type(other_db_ref, other_db_ref_in)
+                            set_ref_el_details(other_db_ref, other_db_ref_in)
+
+                            if other_db_ref.has__content():
+                                other_db_ref_list.add_db_reference(other_db_ref)
+
+                other_db_ref_list = emdb.other_db_cross_reference_list_type()
+                set_other_db_cross_ref_list_type(other_db_ref_list, other_db_ref_dict_in)
+                if other_db_ref_list.has__content():
+                    cross_references.set_other_db_list(other_db_ref_list)
+
             def set_el_auxiliary_link_list(cross_references):
                 """
                 <xs:element name="auxiliary_link_list" minOccurs="0">
                 ..a list of one and only one element
                 """
 
                 def set_aux_link_type(aux, aux_in):
@@ -3321,14 +3391,17 @@
             set_el_citation_list(cross_references)
             x_ref_dict_in = make_list_of_dicts(const.EM_DB_REFERENCE, "db_name")
             # element 2
             set_el_emdb_list(cross_references, x_ref_dict_in)
             # element 3
             set_el_pdb_list(cross_references, x_ref_dict_in)
             # element 4
+            other_db_ref_dict_in = make_list_of_dicts(const.PDBX_DATABASE_RELATED, "db_name")
+            set_el_other_db_list(cross_references, other_db_ref_dict_in)
+            # element 5
             set_el_auxiliary_link_list(cross_references)
 
         def set_sample_type(sample):
             """
             Sets <xs:element name="sample" type="sample_type"> as
             ..a sequence of 3 elements
             """
@@ -3344,15 +3417,15 @@
             def set_base_source_type(src, cif_category, src_in):
                 """
                 Parameters:
                 @param src: either an object for supramolecule or macromolecule
                 @param cif_category: _entity_src_nat, _entity_src_gen, _pdbx_entity_src_syn or _em_entity_assembly_naturalsource
                 @param src_in:
                 XSD: <xs:complexType name="base_source_type"> has
-                    .. 1 attribute and
+                    .. 2 attribute and
                     .. 3 elements
                 """
 
                 def set_attr_database(src, cif_category, src_in):
                     """
                     XSD: <xs:attribute name="database">; <xs:enumeration value="NCBI"/>
                     CIF: _entity_src_nat.pdbx_ncbi_taxonomy_id
@@ -3361,40 +3434,54 @@
                     CIF: _em_entity_assembly_naturalsource.ncbi_tax_id
                     """
                     tax_id_in = None
                     a_dict = {
                         const.ENTITY_SRC_NAT: "pdbx_ncbi_taxonomy_id",
                         const.ENTITY_SRC_GEN: "pdbx_gene_src_ncbi_taxonomy_id",
                         const.PDBX_ENTITY_SRC_SYN: "ncbi_taxonomy_id",
-                        const.EM_ENTITY_ASSEMBLY_NATURALSOURCE: "ncbi_tax_id",
+                        const.EM_ENTITY_ASSEMBLY_NATURALSOURCE: "ncbi_tax_id"
                     }
                     if cif_category is not None:
                         cif_key = a_dict.get(cif_category, None)
                         tax_id_in = get_cif_value(cif_key, cif_category, src_in)
                         if cif_key is None or cif_key.isspace():
                             txt = u"Cannot set the database attribute as the cif category (%s) is not one of: (%s)." % (cif_category, a_dict)
                             self.current_entry_log.error_logs.append(self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.error_title + txt))
                             self.log_formatted(self.error_log_string, const.REQUIRED_ALERT + txt)
                         else:
                             set_cif_value(src.set_database, cif_key, cif_category, cif_list=src_in, cif_value="NCBI")
 
                     return tax_id_in
 
+                def set_attr_synthetically_produced(src_in):
+                    """
+                    XSD: <xs:attribute name="synthetically_produced">/>
+                    CIF: _em_entity_assembly_source.source YES
+                    """
+                    source_dict = make_dict(const.EM_ENTITY_ASSEMBLY, "id")
+                    for i in source_dict.keys():
+                        assembly_type = get_cif_value("source", const.EM_ENTITY_ASSEMBLY, source_dict[i])
+                        assembly_id = get_cif_value("id", const.EM_ENTITY_ASSEMBLY, source_dict[i])
+                        if assembly_type == "SYNTHETIC":
+                            nat_src_id = get_cif_value("entity_assembly_id", const.EM_ENTITY_ASSEMBLY_NATURALSOURCE, src_in)
+                            if assembly_id == nat_src_id:
+                                set_cif_value(src.set_synthetically_produced, cif_value=True)
+
                 def set_el_organism(src, tax_id_in, cif_category, src_in):
                     """
                     XSD: <xs:element name="organism" type="organism_type">
                     CIF: _entity_src_nat.common_name
                     CIF: _entity_src_gen.pdbx_gene_src_scientific_name
                     CIF: _pdbx_entity_src_syn.organism_scientific
                     For some entries _entity_src_nat.common_name is not given but _entity_src_nat.pdbx_organism_scientific is
                     CIF: _entity_src_nat.pdbx_organism_scientific
                     CIF: _em_entity_assembly_naturalsource.organism
                     """
                     a_dict = {
-                        const.ENTITY_SRC_NAT: "common_name",
+                        const.ENTITY_SRC_NAT: "pdbx_organism_scientific",
                         const.ENTITY_SRC_GEN: "pdbx_gene_src_scientific_name",
                         const.PDBX_ENTITY_SRC_SYN: "organism_scientific",
                         const.EM_ENTITY_ASSEMBLY_NATURALSOURCE: "organism",
                     }
                     if cif_category is not None:
                         cif_key = a_dict.get(cif_category, None)
                         if cif_key is not None:
@@ -3477,21 +3564,36 @@
 
                 def set_el_synonym_organism():
                     """
                     XSD: <xs:element name="synonym_organism" type="xs:token" minOccurs="0">
                     Deprecated (2014-10-21)
                     """
 
+                def set_el_details(src, cif_category, src_in):
+                    """
+                    XSD: <xs:element name="details" type="xs:string" minOccurs="0"/>
+                    XPath: /element(*,base_source_type)/details
+                    CIF: _em_entity_assembly_naturalsource.details
+                    """
+                    det = get_cif_value("details", const.EM_ENTITY_ASSEMBLY_NATURALSOURCE, src_in)
+                    if det is not None:
+                        set_cif_value(src.set_details, "details", cif_category, cif_list=src_in)
+
+                # attribute 1
                 tax_id_in = set_attr_database(src, cif_category, src_in)
+                # attribute 2
+                set_attr_synthetically_produced(src_in)
                 # element 1
                 set_el_organism(src, tax_id_in, cif_category, src_in)
                 # element 2
                 set_el_strain(src, cif_category, src_in)
                 # element 3
                 set_el_synonym_organism()
+                # element 4
+                set_el_details(src, cif_category, src_in)
 
             def get_rec_exp_dict(ent_id_in, src_dicts, cif_cat_in, is_supramolecule):
                 """
                 Replace above
                 Helper function: It returns a dictionary needed for recombinant expression containing a cif category depending on several requirements.
 
                 SUPRAMOLECULE are all map entries. Cif category _em_entity_assembly:
@@ -9645,15 +9747,15 @@
                                 .. 1 attribute <xs:attribute fixed="A" name="units" type="xs:token" use="required"/>
                                 """
 
                             def set_el_software_list(mol_repl, cryst_dicts):
                                 """
                                 XSD: <xs:element name="software_list" type="software_list_type" minOccurs="0"/>
                                 """
-                                set_software_list(const.MOLECULAR_REPLACEMENT, cryst_dicts["cat_soft_dict_in"], mol_repl.set_software_list)
+                                set_software_list(const.SOFT_MOLECULAR_REPLACEMENT, cryst_dicts["cat_soft_dict_in"], mol_repl.set_software_list)
 
                             # element 1
                             set_el_starting_model()
                             # element 2
                             set_el_resolution_range()
                             # element 3
                             set_el_software_list(mol_repl, cryst_dicts)
@@ -9663,27 +9765,27 @@
                         if mol_repl.has__content():
                             im_proc.set_molecular_replacement(mol_repl)
 
                     def set_el_lat_dist_corr_soft_list(im_proc, cryst_dicts):
                         """
                         XSD: <xs:element name="lattice_distortion_correction_software_list" type="software_list_type" minOccurs="0"/>
                         """
-                        set_software_list(const.LATTICE_DISTORTION_CORRECTION, cryst_dicts["cat_soft_dict_in"], im_proc.set_lattice_distortion_correction_software_list)
+                        set_software_list(const.SOFT_LATTICE_DISTORTION_CORRECTION, cryst_dicts["cat_soft_dict_in"], im_proc.set_lattice_distortion_correction_software_list)
 
                     def set_el_sym_det_software_list(im_proc, cryst_dicts):
                         """
                         XSD: <xs:element name="symmetry_determination_software_list" type="software_list_type" minOccurs="0"/>
                         """
-                        set_software_list(const.SYMMETRY_DETERMINATION, cryst_dicts["cat_soft_dict_in"], im_proc.set_symmetry_determination_software_list)
+                        set_software_list(const.SOFT_SYMMETRY_DETERMINATION, cryst_dicts["cat_soft_dict_in"], im_proc.set_symmetry_determination_software_list)
 
                     def set_el_merging_software_list(im_proc, cryst_dicts):
                         """
                         XSD: <xs:element name="merging_software_list" type="software_list_type" minOccurs="0"/>
                         """
-                        set_software_list(const.CRYSTALLOGRAPHY_MERGING, cryst_dicts["cat_soft_dict_in"], im_proc.set_merging_software_list)
+                        set_software_list(const.SOFT_CRYSTALLOGRAPHY_MERGING, cryst_dicts["cat_soft_dict_in"], im_proc.set_merging_software_list)
 
                     def set_el_cryst_statistics(im_proc, cryst_dicts):
                         """
                         XSD: <xs:element name="crystallography_statistics" type="crystallography_statistics_type" minOccurs="0"/>
                         """
 
                         def set_cryst_statistics_type(cry_stats, cry_stats_in):
@@ -10008,15 +10110,15 @@
                         set_non_sub_tom_final_recon(ip_id_in, im_proc, non_st_dicts)
 
                     def set_el_alig_soft_list(im_proc, tomo_dicts):
                         """
                         XSD: <xs:element name="series_aligment_software_list" type="software_list_type" minOccurs="0"/>
                         """
                         cat_soft_dict_in = tomo_dicts["cat_soft_dict_in"]
-                        set_software_list(const.LATTICE_DISTORTION_CORRECTION, cat_soft_dict_in, im_proc.set_series_aligment_software_list)
+                        set_software_list(const.SOFT_LATTICE_DISTORTION_CORRECTION, cat_soft_dict_in, im_proc.set_series_aligment_software_list)
 
                     def set_el_ctf_correction(im_proc, ip_id_in, tomo_dicts):
                         """
                         XSD: <xs:element name="ctf_correction" type="ctf_correction_type" minOccurs="0"/>
                         """
                         ctf_corr_dict_in = tomo_dicts["ctf_corr_dict_in"]
                         if ip_id_in in ctf_corr_dict_in:
@@ -10674,14 +10776,30 @@
                                             self.log_formatted(self.error_log_string, const.REQUIRED_ALERT + txt)
                                     else:
                                         txt = u"Contour level is not set for TOMOGRAPHY primary map."
                                         self.current_entry_log.info_logs.append(
                                             self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.info_title + txt)
                                         )
                                         self.log_formatted(self.info_log_string, const.INFO_ALERT + txt)
+                            if map_type == "mask":
+                                cntr_level = get_cif_value("contour_level", const.EM_MAP, cif_list=map_in)
+                                if cntr_level is not None:
+                                    if not isinstance(cntr_level, str):
+                                        set_cif_value(cntr.set_level, "contour_level", const.EM_MAP, cif_list=map_in, fmt=float)
+                                    else:
+                                        # contour level is a string; check if the string can be converted
+                                        if is_number(cntr_level.lstrip("+-")):
+                                            cl_float = float(cntr_level.lstrip("+-"))
+                                            set_cif_value(cntr.set_level, "contour_level", const.EM_MAP, cif_list=map_in, cif_value=cl_float)
+                                        else:
+                                            txt = u"Contour level is given as a text value of %s. This is not correct. It should be a number." % cntr_level
+                                            self.current_entry_log.error_logs.append(
+                                                self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.error_title + txt)
+                                            )
+                                            self.log_formatted(self.error_log_string, const.REQUIRED_ALERT + txt)
 
                         def set_el_source(cntr, map_in):
                             """
                             XSD: <xs:element name="source" minOccurs="0">
                             CIF: _em_map.contour_level_source
                             """
                             set_cif_value(cntr.set_source, "contour_level_source", const.EM_MAP, cif_list=map_in, fmt=str.upper)
@@ -10952,22 +11070,24 @@
                                     def set_el_access_code(model, model_in):
                                         """
                                         XSD: <xs:element name="access_code">
                                         CIF: _em_3d_fitting_list.pdb_entry_id  1EHZ
                                         CIF: _em_3d_fitting_list.entry_id  1EHZ
                                         pattern "d[dA-Za-z]{3}"
                                         """
+                                        db_name = get_cif_value("source_name", const.EM_3D_FITTING_LIST, cif_list=model_in)
                                         accession_code = get_cif_value("accession_code", const.EM_3D_FITTING_LIST, cif_list=model_in)
                                         access_code = get_cif_value("pdb_entry_id", const.EM_3D_FITTING_LIST, cif_list=model_in)
                                         pdb_pattern = re.compile(r"\d[\dA-Za-z]{3}|pdb_\d{5}[\dA-Za-z]{3}")
-                                        if access_code is not None:
-                                            if not pdb_pattern.match(str(access_code)):
-                                                txt = u"(%s) PDB id is not in the correct format" % access_code
-                                                self.current_entry_log.error_logs.append(self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.error_title + txt))
-                                                self.log_formatted(self.error_log_string, const.REQUIRED_ALERT + txt)
+                                        if db_name == "PDB":
+                                            if access_code is not None:
+                                                if not pdb_pattern.match(str(access_code)):
+                                                    txt = u"(%s) PDB id is not in the correct format" % access_code
+                                                    self.current_entry_log.error_logs.append(self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.error_title + txt))
+                                                    self.log_formatted(self.error_log_string, const.REQUIRED_ALERT + txt)
                                         if accession_code is None and access_code is not None:
                                             set_cif_value(model.set_access_code, "pdb_entry_id", const.EM_3D_FITTING_LIST, cif_list=model_in)
                                         if accession_code is not None and access_code is None:
                                             set_cif_value(model.set_access_code, "accession_code", const.EM_3D_FITTING_LIST, cif_list=model_in)
                                         if accession_code is not None and access_code is not None:
                                             set_cif_value(model.set_access_code, "pdb_entry_id", const.EM_3D_FITTING_LIST, cif_list=model_in)
                                             if accession_code != access_code:
@@ -11254,26 +11374,44 @@
                         for hf_map_in in hf_map_list_in:
                             hf_map = make_map(hf_map_in, get_canonical_map_name(hf_map_in, "HALFMAP"))
                             if hf_map.has__content():
                                 hf_map_list.add_half_map(hf_map)
                         if hf_map_list.has__content():
                             intrp.set_half_map_list(hf_map_list)
 
+                    def set_el_mask_list(intrp, map_dict_in):
+                        """
+                        XSD: <xs:element name="mask_list" minOccurs="0">
+                        """
+
+                        msk_map_list_in = map_dict_in[const.MAP_MASK] if const.MAP_MASK in map_dict_in else []
+                        msk_map_list = emdb.mask_listType()
+                        for msk_map_in in msk_map_list_in:
+                            msk_map = make_map(msk_map_in, get_canonical_map_name(msk_map_in, "MASK"))
+                            msk_file = msk_map.get_file()
+                            set_cif_value(msk_map.set_file, cif_value=msk_file)
+                            if msk_map.has__content():
+                                msk_map_list.add_mask(msk_map)
+                        if msk_map_list.has__content():
+                            intrp.set_mask_list(msk_map_list)
+
                     # element 1
                     set_el_modelling_list(intrp)
                     # element 2
                     set_el_figure_list()
                     # element 3
                     set_el_segmentation_list(intrp)
                     # element 4
                     set_el_slices_list()
                     # element 5
                     set_el_additional_map_list(intrp, map_dict_in)
                     # element 6
                     set_el_half_map_list(intrp, map_dict_in)
+                    # element 7
+                    set_el_mask_list(intrp, map_dict_in)
 
                 map_dict_in = make_list_of_dicts(const.EM_MAP, "type")
                 intrp = emdb.interpretation_type()
                 set_interpretation_type(intrp, map_dict_in)
                 if intrp.has__content():
                     self.xml_out.set_interpretation(intrp)
```

### Comparing `wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/cif_emdb_translator/em_emd_conversion.py` & `wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/cif_emdb_translator/em_emd_conversion.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/cif_emdb_translator/emdb.py` & `wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/cif_emdb_translator/emdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #
-# Generated Tue May 23 14:21:39 2023 by generateDS.py version 2.41.5.
+# Generated Mon Jul 17 15:20:35 2023 by generateDS.py version 2.41.5.
 # Python 3.9.5 (default, May 18 2021, 12:31:01)  [Clang 10.0.0 ]
 #
 # Command line options:
 #   ('--root-element', 'emd')
 #   ('-f', '')
-#   ('-o', 'emdb-schemas/emdb_schemas/v3/v3_0_4_0/emdb.py')
+#   ('-o', 'emdb-schemas/emdb_schemas/v3/v3_0_7_2/emdb.py')
 #   ('--no-warnings', '')
 #   ('--external-encoding', 'utf-8')
 #
 # Command line arguments:
-#   emdb-schemas/emdb_schemas/v3/v3_0_4_0/emdb.xsd
+#   emdb-schemas/emdb_schemas/v3/v3_0_7_2/emdb.xsd
 #
 # Command line:
-#   /Users/amudha/project/generateDS-2.41.5/generateDS.py --root-element="emd" -f -o "emdb-schemas/emdb_schemas/v3/v3_0_4_0/emdb.py" --no-warnings --external-encoding="utf-8" emdb-schemas/emdb_schemas/v3/v3_0_4_0/emdb.xsd
+#   /Users/amudha/project/generateDS-2.41.5/generateDS.py --root-element="emd" -f -o "emdb-schemas/emdb_schemas/v3/v3_0_7_2/emdb.py" --no-warnings --external-encoding="utf-8" emdb-schemas/emdb_schemas/v3/v3_0_7_2/emdb.xsd
 #
 # Current working directory (os.getcwd()):
 #   IdeaProjects
 #
 
 import sys
 try:
@@ -1016,14 +1016,15 @@
     HELICAL_ARRAY='helicalArray'
     CELL='cell'
     TISSUE='tissue'
 
 
 class allowed_film_or_detector_model(str, Enum):
     AGFASCIENTAFILM='AGFA SCIENTA FILM'
+    DECTRISSINGLA_1_KX_1_K='DECTRIS SINGLA (1k x 1k)'
     DIRECTELECTRONAPOLLO_4_KX_4_K='DIRECT ELECTRON APOLLO (4k x 4k)'
     DIRECTELECTRONDE_10_5_KX_4_K='DIRECT ELECTRON DE-10 (5k x 4k)'
     DIRECTELECTRONDE_12_4_KX_3_K='DIRECT ELECTRON DE-12 (4k x 3k)'
     DIRECTELECTRONDE_16_4_KX_4_K='DIRECT ELECTRON DE-16 (4k x 4k)'
     DIRECTELECTRONDE_20_5_KX_3_K='DIRECT ELECTRON DE-20 (5k x 3k)'
     DIRECTELECTRONDE_64_8_KX_8_K='DIRECT ELECTRON DE-64 (8k x 8k)'
     FEICETA_4_KX_4_K='FEI CETA (4k x 4k)'
@@ -1407,14 +1408,15 @@
     JEOL_1000_EES='JEOL 1000EES'
     JEOL_1010='JEOL 1010'
     JEOL_1200='JEOL 1200'
     JEOL_1200_EX='JEOL 1200EX'
     JEOL_1200_EXII='JEOL 1200EXII'
     JEOL_1230='JEOL 1230'
     JEOL_1400='JEOL 1400'
+    JEOL_1400HRYPSFEG='JEOL 1400/HR + YPS FEG'
     JEOL_2000_EX='JEOL 2000EX'
     JEOL_2000_EXII='JEOL 2000EXII'
     JEOL_2010='JEOL 2010'
     JEOL_2010_F='JEOL 2010F'
     JEOL_2010_HC='JEOL 2010HC'
     JEOL_2010_HT='JEOL 2010HT'
     JEOL_2010_UHR='JEOL 2010UHR'
@@ -1759,15 +1761,15 @@
     VIRUSLIKEPARTICLE='VIRUS-LIKE PARTICLE'
 
 
 class entry_type(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
-    def __init__(self, emdb_id=None, version='3.0.4.0', admin=None, crossreferences=None, sample=None, structure_determination_list=None, map=None, interpretation=None, validation=None, gds_collector_=None, **kwargs_):
+    def __init__(self, emdb_id=None, version='3.0.7.2', admin=None, crossreferences=None, sample=None, structure_determination_list=None, map=None, interpretation=None, validation=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         self.emdb_id = _cast(None, emdb_id)
         self.emdb_id_nsprefix_ = None
@@ -1885,15 +1887,15 @@
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='entry_type'):
         if self.emdb_id is not None and 'emdb_id' not in already_processed:
             already_processed.add('emdb_id')
             outfile.write(' emdb_id=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.emdb_id), input_name='emdb_id')), ))
-        if self.version != "3.0.4.0" and 'version' not in already_processed:
+        if self.version != "3.0.7.2" and 'version' not in already_processed:
             already_processed.add('version')
             outfile.write(' version=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.version), input_name='version')), ))
     def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='entry_type', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
@@ -3874,26 +3876,28 @@
 # end class author_order_type
 
 
 class crossreferences_type(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
-    def __init__(self, citation_list=None, emdb_list=None, pdb_list=None, auxiliary_link_list=None, gds_collector_=None, **kwargs_):
+    def __init__(self, citation_list=None, emdb_list=None, pdb_list=None, other_db_list=None, auxiliary_link_list=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         self.citation_list = citation_list
         self.citation_list_nsprefix_ = None
         self.emdb_list = emdb_list
         self.emdb_list_nsprefix_ = None
         self.pdb_list = pdb_list
         self.pdb_list_nsprefix_ = None
+        self.other_db_list = other_db_list
+        self.other_db_list_nsprefix_ = None
         self.auxiliary_link_list = auxiliary_link_list
         self.auxiliary_link_list_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
                 CurrentSubclassModule_, crossreferences_type)
             if subclass is not None:
@@ -3915,23 +3919,28 @@
         return self.emdb_list
     def set_emdb_list(self, emdb_list):
         self.emdb_list = emdb_list
     def get_pdb_list(self):
         return self.pdb_list
     def set_pdb_list(self, pdb_list):
         self.pdb_list = pdb_list
+    def get_other_db_list(self):
+        return self.other_db_list
+    def set_other_db_list(self, other_db_list):
+        self.other_db_list = other_db_list
     def get_auxiliary_link_list(self):
         return self.auxiliary_link_list
     def set_auxiliary_link_list(self, auxiliary_link_list):
         self.auxiliary_link_list = auxiliary_link_list
     def has__content(self):
         if (
             self.citation_list is not None or
             self.emdb_list is not None or
             self.pdb_list is not None or
+            self.other_db_list is not None or
             self.auxiliary_link_list is not None
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='crossreferences_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('crossreferences_type')
@@ -3968,14 +3977,17 @@
             self.citation_list.export(outfile, level, namespaceprefix_, namespacedef_='', name_='citation_list', pretty_print=pretty_print)
         if self.emdb_list is not None:
             namespaceprefix_ = self.emdb_list_nsprefix_ + ':' if (UseCapturedNS_ and self.emdb_list_nsprefix_) else ''
             self.emdb_list.export(outfile, level, namespaceprefix_, namespacedef_='', name_='emdb_list', pretty_print=pretty_print)
         if self.pdb_list is not None:
             namespaceprefix_ = self.pdb_list_nsprefix_ + ':' if (UseCapturedNS_ and self.pdb_list_nsprefix_) else ''
             self.pdb_list.export(outfile, level, namespaceprefix_, namespacedef_='', name_='pdb_list', pretty_print=pretty_print)
+        if self.other_db_list is not None:
+            namespaceprefix_ = self.other_db_list_nsprefix_ + ':' if (UseCapturedNS_ and self.other_db_list_nsprefix_) else ''
+            self.other_db_list.export(outfile, level, namespaceprefix_, namespacedef_='', name_='other_db_list', pretty_print=pretty_print)
         if self.auxiliary_link_list is not None:
             namespaceprefix_ = self.auxiliary_link_list_nsprefix_ + ':' if (UseCapturedNS_ and self.auxiliary_link_list_nsprefix_) else ''
             self.auxiliary_link_list.export(outfile, level, namespaceprefix_, namespacedef_='', name_='auxiliary_link_list', pretty_print=pretty_print)
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
@@ -4000,14 +4012,19 @@
             self.emdb_list = obj_
             obj_.original_tagname_ = 'emdb_list'
         elif nodeName_ == 'pdb_list':
             obj_ = pdb_cross_reference_list_type.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.pdb_list = obj_
             obj_.original_tagname_ = 'pdb_list'
+        elif nodeName_ == 'other_db_list':
+            obj_ = other_db_cross_reference_list_type.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            self.other_db_list = obj_
+            obj_.original_tagname_ = 'other_db_list'
         elif nodeName_ == 'auxiliary_link_list':
             obj_ = auxiliary_link_listType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.auxiliary_link_list = obj_
             obj_.original_tagname_ = 'auxiliary_link_list'
 # end class crossreferences_type
 
@@ -5360,14 +5377,274 @@
             value_ = self.gds_parse_string(value_, node, 'details')
             value_ = self.gds_validate_string(value_, node, 'details')
             self.details = value_
             self.details_nsprefix_ = child_.prefix
 # end class pdb_cross_reference_type
 
 
+class other_db_cross_reference_list_type(GeneratedsSuper):
+    __hash__ = GeneratedsSuper.__hash__
+    subclass = None
+    superclass = None
+    def __init__(self, db_reference=None, gds_collector_=None, **kwargs_):
+        self.gds_collector_ = gds_collector_
+        self.gds_elementtree_node_ = None
+        self.original_tagname_ = None
+        self.parent_object_ = kwargs_.get('parent_object_')
+        self.ns_prefix_ = None
+        if db_reference is None:
+            self.db_reference = []
+        else:
+            self.db_reference = db_reference
+        self.db_reference_nsprefix_ = None
+    def factory(*args_, **kwargs_):
+        if CurrentSubclassModule_ is not None:
+            subclass = getSubclassFromModule_(
+                CurrentSubclassModule_, other_db_cross_reference_list_type)
+            if subclass is not None:
+                return subclass(*args_, **kwargs_)
+        if other_db_cross_reference_list_type.subclass:
+            return other_db_cross_reference_list_type.subclass(*args_, **kwargs_)
+        else:
+            return other_db_cross_reference_list_type(*args_, **kwargs_)
+    factory = staticmethod(factory)
+    def get_ns_prefix_(self):
+        return self.ns_prefix_
+    def set_ns_prefix_(self, ns_prefix):
+        self.ns_prefix_ = ns_prefix
+    def get_db_reference(self):
+        return self.db_reference
+    def set_db_reference(self, db_reference):
+        self.db_reference = db_reference
+    def add_db_reference(self, value):
+        self.db_reference.append(value)
+    def insert_db_reference_at(self, index, value):
+        self.db_reference.insert(index, value)
+    def replace_db_reference_at(self, index, value):
+        self.db_reference[index] = value
+    def has__content(self):
+        if (
+            self.db_reference
+        ):
+            return True
+        else:
+            return False
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='other_db_cross_reference_list_type', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('other_db_cross_reference_list_type')
+        if imported_ns_def_ is not None:
+            namespacedef_ = imported_ns_def_
+        if pretty_print:
+            eol_ = '\n'
+        else:
+            eol_ = ''
+        if self.original_tagname_ is not None and name_ == 'other_db_cross_reference_list_type':
+            name_ = self.original_tagname_
+        if UseCapturedNS_ and self.ns_prefix_:
+            namespaceprefix_ = self.ns_prefix_ + ':'
+        showIndent(outfile, level, pretty_print)
+        outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
+        already_processed = set()
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='other_db_cross_reference_list_type')
+        if self.has__content():
+            outfile.write('>%s' % (eol_, ))
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='other_db_cross_reference_list_type', pretty_print=pretty_print)
+            showIndent(outfile, level, pretty_print)
+            outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
+        else:
+            outfile.write('/>%s' % (eol_, ))
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='other_db_cross_reference_list_type'):
+        pass
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='other_db_cross_reference_list_type', fromsubclass_=False, pretty_print=True):
+        if pretty_print:
+            eol_ = '\n'
+        else:
+            eol_ = ''
+        for db_reference_ in self.db_reference:
+            namespaceprefix_ = self.db_reference_nsprefix_ + ':' if (UseCapturedNS_ and self.db_reference_nsprefix_) else ''
+            db_reference_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='db_reference', pretty_print=pretty_print)
+    def build(self, node, gds_collector_=None):
+        self.gds_collector_ = gds_collector_
+        if SaveElementTreeNode:
+            self.gds_elementtree_node_ = node
+        already_processed = set()
+        self.ns_prefix_ = node.prefix
+        self._buildAttributes(node, node.attrib, already_processed)
+        for child in node:
+            nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
+            self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+        return self
+    def _buildAttributes(self, node, attrs, already_processed):
+        pass
+    def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
+        if nodeName_ == 'db_reference':
+            obj_ = other_db_cross_reference_type.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            self.db_reference.append(obj_)
+            obj_.original_tagname_ = 'db_reference'
+# end class other_db_cross_reference_list_type
+
+
+class other_db_cross_reference_type(GeneratedsSuper):
+    __hash__ = GeneratedsSuper.__hash__
+    subclass = None
+    superclass = None
+    def __init__(self, db_name=None, accession_id=None, content_type=None, details=None, gds_collector_=None, **kwargs_):
+        self.gds_collector_ = gds_collector_
+        self.gds_elementtree_node_ = None
+        self.original_tagname_ = None
+        self.parent_object_ = kwargs_.get('parent_object_')
+        self.ns_prefix_ = None
+        self.db_name = db_name
+        self.db_name_nsprefix_ = None
+        self.accession_id = accession_id
+        self.accession_id_nsprefix_ = None
+        self.content_type = content_type
+        self.content_type_nsprefix_ = None
+        self.details = details
+        self.details_nsprefix_ = None
+    def factory(*args_, **kwargs_):
+        if CurrentSubclassModule_ is not None:
+            subclass = getSubclassFromModule_(
+                CurrentSubclassModule_, other_db_cross_reference_type)
+            if subclass is not None:
+                return subclass(*args_, **kwargs_)
+        if other_db_cross_reference_type.subclass:
+            return other_db_cross_reference_type.subclass(*args_, **kwargs_)
+        else:
+            return other_db_cross_reference_type(*args_, **kwargs_)
+    factory = staticmethod(factory)
+    def get_ns_prefix_(self):
+        return self.ns_prefix_
+    def set_ns_prefix_(self, ns_prefix):
+        self.ns_prefix_ = ns_prefix
+    def get_db_name(self):
+        return self.db_name
+    def set_db_name(self, db_name):
+        self.db_name = db_name
+    def get_accession_id(self):
+        return self.accession_id
+    def set_accession_id(self, accession_id):
+        self.accession_id = accession_id
+    def get_content_type(self):
+        return self.content_type
+    def set_content_type(self, content_type):
+        self.content_type = content_type
+    def get_details(self):
+        return self.details
+    def set_details(self, details):
+        self.details = details
+    def has__content(self):
+        if (
+            self.db_name is not None or
+            self.accession_id is not None or
+            self.content_type is not None or
+            self.details is not None
+        ):
+            return True
+        else:
+            return False
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='other_db_cross_reference_type', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('other_db_cross_reference_type')
+        if imported_ns_def_ is not None:
+            namespacedef_ = imported_ns_def_
+        if pretty_print:
+            eol_ = '\n'
+        else:
+            eol_ = ''
+        if self.original_tagname_ is not None and name_ == 'other_db_cross_reference_type':
+            name_ = self.original_tagname_
+        if UseCapturedNS_ and self.ns_prefix_:
+            namespaceprefix_ = self.ns_prefix_ + ':'
+        showIndent(outfile, level, pretty_print)
+        outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
+        already_processed = set()
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='other_db_cross_reference_type')
+        if self.has__content():
+            outfile.write('>%s' % (eol_, ))
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='other_db_cross_reference_type', pretty_print=pretty_print)
+            showIndent(outfile, level, pretty_print)
+            outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
+        else:
+            outfile.write('/>%s' % (eol_, ))
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='other_db_cross_reference_type'):
+        pass
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='other_db_cross_reference_type', fromsubclass_=False, pretty_print=True):
+        if pretty_print:
+            eol_ = '\n'
+        else:
+            eol_ = ''
+        if self.db_name is not None:
+            namespaceprefix_ = self.db_name_nsprefix_ + ':' if (UseCapturedNS_ and self.db_name_nsprefix_) else ''
+            showIndent(outfile, level, pretty_print)
+            outfile.write('<%sdb_name>%s</%sdb_name>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.db_name), input_name='db_name')), namespaceprefix_ , eol_))
+        if self.accession_id is not None:
+            namespaceprefix_ = self.accession_id_nsprefix_ + ':' if (UseCapturedNS_ and self.accession_id_nsprefix_) else ''
+            showIndent(outfile, level, pretty_print)
+            outfile.write('<%saccession_id>%s</%saccession_id>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.accession_id), input_name='accession_id')), namespaceprefix_ , eol_))
+        if self.content_type is not None:
+            namespaceprefix_ = self.content_type_nsprefix_ + ':' if (UseCapturedNS_ and self.content_type_nsprefix_) else ''
+            showIndent(outfile, level, pretty_print)
+            outfile.write('<%scontent_type>%s</%scontent_type>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.content_type), input_name='content_type')), namespaceprefix_ , eol_))
+        if self.details is not None:
+            namespaceprefix_ = self.details_nsprefix_ + ':' if (UseCapturedNS_ and self.details_nsprefix_) else ''
+            showIndent(outfile, level, pretty_print)
+            outfile.write('<%sdetails>%s</%sdetails>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.details), input_name='details')), namespaceprefix_ , eol_))
+    def build(self, node, gds_collector_=None):
+        self.gds_collector_ = gds_collector_
+        if SaveElementTreeNode:
+            self.gds_elementtree_node_ = node
+        already_processed = set()
+        self.ns_prefix_ = node.prefix
+        self._buildAttributes(node, node.attrib, already_processed)
+        for child in node:
+            nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
+            self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+        return self
+    def _buildAttributes(self, node, attrs, already_processed):
+        pass
+    def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
+        if nodeName_ == 'db_name':
+            value_ = child_.text
+            if value_:
+                value_ = re_.sub(String_cleanup_pat_, " ", value_).strip()
+            else:
+                value_ = ""
+            value_ = self.gds_parse_string(value_, node, 'db_name')
+            value_ = self.gds_validate_string(value_, node, 'db_name')
+            self.db_name = value_
+            self.db_name_nsprefix_ = child_.prefix
+        elif nodeName_ == 'accession_id':
+            value_ = child_.text
+            if value_:
+                value_ = re_.sub(String_cleanup_pat_, " ", value_).strip()
+            else:
+                value_ = ""
+            value_ = self.gds_parse_string(value_, node, 'accession_id')
+            value_ = self.gds_validate_string(value_, node, 'accession_id')
+            self.accession_id = value_
+            self.accession_id_nsprefix_ = child_.prefix
+        elif nodeName_ == 'content_type':
+            value_ = child_.text
+            if value_:
+                value_ = re_.sub(String_cleanup_pat_, " ", value_).strip()
+            else:
+                value_ = ""
+            value_ = self.gds_parse_string(value_, node, 'content_type')
+            value_ = self.gds_validate_string(value_, node, 'content_type')
+            self.content_type = value_
+            self.content_type_nsprefix_ = child_.prefix
+        elif nodeName_ == 'details':
+            value_ = child_.text
+            value_ = self.gds_parse_string(value_, node, 'details')
+            value_ = self.gds_validate_string(value_, node, 'details')
+            self.details = value_
+            self.details_nsprefix_ = child_.prefix
+# end class other_db_cross_reference_type
+
+
 class auxiliary_link_type(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, type_=None, link=None, details=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
@@ -6148,28 +6425,32 @@
 # end class cell_supramolecule_type
 
 
 class base_source_type(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
-    def __init__(self, database=None, organism=None, strain=None, synonym_organism=None, extensiontype_=None, gds_collector_=None, **kwargs_):
+    def __init__(self, database=None, synthetically_produced=None, organism=None, strain=None, synonym_organism=None, details=None, extensiontype_=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         self.database = _cast(None, database)
         self.database_nsprefix_ = None
+        self.synthetically_produced = _cast(bool, synthetically_produced)
+        self.synthetically_produced_nsprefix_ = None
         self.organism = organism
         self.organism_nsprefix_ = None
         self.strain = strain
         self.strain_nsprefix_ = None
         self.synonym_organism = synonym_organism
         self.synonym_organism_nsprefix_ = None
+        self.details = details
+        self.details_nsprefix_ = None
         self.extensiontype_ = extensiontype_
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
                 CurrentSubclassModule_, base_source_type)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
@@ -6190,18 +6471,26 @@
         return self.strain
     def set_strain(self, strain):
         self.strain = strain
     def get_synonym_organism(self):
         return self.synonym_organism
     def set_synonym_organism(self, synonym_organism):
         self.synonym_organism = synonym_organism
+    def get_details(self):
+        return self.details
+    def set_details(self, details):
+        self.details = details
     def get_database(self):
         return self.database
     def set_database(self, database):
         self.database = database
+    def get_synthetically_produced(self):
+        return self.synthetically_produced
+    def set_synthetically_produced(self, synthetically_produced):
+        self.synthetically_produced = synthetically_produced
     def get_extensiontype_(self): return self.extensiontype_
     def set_extensiontype_(self, extensiontype_): self.extensiontype_ = extensiontype_
     def validate_databaseType(self, value):
         # Validate type databaseType, a restriction on xs:token.
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, str):
                 lineno = self.gds_get_node_lineno_()
@@ -6213,15 +6502,16 @@
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on databaseType' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
     def has__content(self):
         if (
             self.organism is not None or
             self.strain is not None or
-            self.synonym_organism is not None
+            self.synonym_organism is not None or
+            self.details is not None
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='base_source_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('base_source_type')
         if imported_ns_def_ is not None:
@@ -6245,14 +6535,17 @@
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='base_source_type'):
         if self.database is not None and 'database' not in already_processed:
             already_processed.add('database')
             outfile.write(' database=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.database), input_name='database')), ))
+        if self.synthetically_produced is not None and 'synthetically_produced' not in already_processed:
+            already_processed.add('synthetically_produced')
+            outfile.write(' synthetically_produced="%s"' % self.gds_format_boolean(self.synthetically_produced, input_name='synthetically_produced'))
         if self.extensiontype_ is not None and 'xsi:type' not in already_processed:
             already_processed.add('xsi:type')
             outfile.write(' xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"')
             if ":" not in self.extensiontype_:
                 imported_ns_type_prefix_ = GenerateDSNamespaceTypePrefixes_.get(self.extensiontype_, '')
                 outfile.write(' xsi:type="%s%s"' % (imported_ns_type_prefix_, self.extensiontype_))
             else:
@@ -6269,14 +6562,18 @@
             namespaceprefix_ = self.strain_nsprefix_ + ':' if (UseCapturedNS_ and self.strain_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sstrain>%s</%sstrain>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.strain), input_name='strain')), namespaceprefix_ , eol_))
         if self.synonym_organism is not None:
             namespaceprefix_ = self.synonym_organism_nsprefix_ + ':' if (UseCapturedNS_ and self.synonym_organism_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
             outfile.write('<%ssynonym_organism>%s</%ssynonym_organism>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.synonym_organism), input_name='synonym_organism')), namespaceprefix_ , eol_))
+        if self.details is not None:
+            namespaceprefix_ = self.details_nsprefix_ + ':' if (UseCapturedNS_ and self.details_nsprefix_) else ''
+            showIndent(outfile, level, pretty_print)
+            outfile.write('<%sdetails>%s</%sdetails>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.details), input_name='details')), namespaceprefix_ , eol_))
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
         self._buildAttributes(node, node.attrib, already_processed)
@@ -6287,14 +6584,23 @@
     def _buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('database', node)
         if value is not None and 'database' not in already_processed:
             already_processed.add('database')
             self.database = value
             self.database = ' '.join(self.database.split())
             self.validate_databaseType(self.database)    # validate type databaseType
+        value = find_attr_value_('synthetically_produced', node)
+        if value is not None and 'synthetically_produced' not in already_processed:
+            already_processed.add('synthetically_produced')
+            if value in ('true', '1'):
+                self.synthetically_produced = True
+            elif value in ('false', '0'):
+                self.synthetically_produced = False
+            else:
+                raise_parse_error(node, 'Bad boolean attribute')
         value = find_attr_value_('xsi:type', node)
         if value is not None and 'xsi:type' not in already_processed:
             already_processed.add('xsi:type')
             self.extensiontype_ = value
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'organism':
             obj_ = organism_type.factory(parent_object_=self)
@@ -6317,14 +6623,20 @@
                 value_ = re_.sub(String_cleanup_pat_, " ", value_).strip()
             else:
                 value_ = ""
             value_ = self.gds_parse_string(value_, node, 'synonym_organism')
             value_ = self.gds_validate_string(value_, node, 'synonym_organism')
             self.synonym_organism = value_
             self.synonym_organism_nsprefix_ = child_.prefix
+        elif nodeName_ == 'details':
+            value_ = child_.text
+            value_ = self.gds_parse_string(value_, node, 'details')
+            value_ = self.gds_validate_string(value_, node, 'details')
+            self.details = value_
+            self.details_nsprefix_ = child_.prefix
 # end class base_source_type
 
 
 class organism_type(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
@@ -6619,21 +6931,21 @@
 # end class complex_supramolecule_type
 
 
 class complex_source_type(base_source_type):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = base_source_type
-    def __init__(self, database=None, organism=None, strain=None, synonym_organism=None, organ=None, tissue=None, cell=None, organelle=None, cellular_location=None, gds_collector_=None, **kwargs_):
+    def __init__(self, database=None, synthetically_produced=None, organism=None, strain=None, synonym_organism=None, details=None, organ=None, tissue=None, cell=None, organelle=None, cellular_location=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
-        super(globals().get("complex_source_type"), self).__init__(database, organism, strain, synonym_organism,  **kwargs_)
+        super(globals().get("complex_source_type"), self).__init__(database, synthetically_produced, organism, strain, synonym_organism, details,  **kwargs_)
         self.organ = organ
         self.organ_nsprefix_ = None
         self.tissue = tissue
         self.tissue_nsprefix_ = None
         self.cell = cell
         self.cell_nsprefix_ = None
         self.organelle = organelle
@@ -7298,21 +7610,21 @@
 # end class organelle_or_cellular_component_supramolecule_type
 
 
 class organelle_source_type(base_source_type):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = base_source_type
-    def __init__(self, database=None, organism=None, strain=None, synonym_organism=None, organ=None, tissue=None, cell=None, organelle=None, cellular_location=None, gds_collector_=None, **kwargs_):
+    def __init__(self, database=None, synthetically_produced=None, organism=None, strain=None, synonym_organism=None, details=None, organ=None, tissue=None, cell=None, organelle=None, cellular_location=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
-        super(globals().get("organelle_source_type"), self).__init__(database, organism, strain, synonym_organism,  **kwargs_)
+        super(globals().get("organelle_source_type"), self).__init__(database, synthetically_produced, organism, strain, synonym_organism, details,  **kwargs_)
         self.organ = organ
         self.organ_nsprefix_ = None
         self.tissue = tissue
         self.tissue_nsprefix_ = None
         self.cell = cell
         self.cell_nsprefix_ = None
         self.organelle = organelle
@@ -7649,21 +7961,21 @@
 # end class sample_supramolecule_type
 
 
 class sample_source_type(base_source_type):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = base_source_type
-    def __init__(self, database=None, organism=None, strain=None, synonym_organism=None, organ=None, tissue=None, cell=None, gds_collector_=None, **kwargs_):
+    def __init__(self, database=None, synthetically_produced=None, organism=None, strain=None, synonym_organism=None, details=None, organ=None, tissue=None, cell=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
-        super(globals().get("sample_source_type"), self).__init__(database, organism, strain, synonym_organism,  **kwargs_)
+        super(globals().get("sample_source_type"), self).__init__(database, synthetically_produced, organism, strain, synonym_organism, details,  **kwargs_)
         self.organ = organ
         self.organ_nsprefix_ = None
         self.tissue = tissue
         self.tissue_nsprefix_ = None
         self.cell = cell
         self.cell_nsprefix_ = None
     def factory(*args_, **kwargs_):
@@ -7924,21 +8236,21 @@
 # end class tissue_supramolecule_type
 
 
 class tissue_source_type(base_source_type):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = base_source_type
-    def __init__(self, database=None, organism=None, strain=None, synonym_organism=None, organ=None, tissue=None, gds_collector_=None, **kwargs_):
+    def __init__(self, database=None, synthetically_produced=None, organism=None, strain=None, synonym_organism=None, details=None, organ=None, tissue=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
-        super(globals().get("tissue_source_type"), self).__init__(database, organism, strain, synonym_organism,  **kwargs_)
+        super(globals().get("tissue_source_type"), self).__init__(database, synthetically_produced, organism, strain, synonym_organism, details,  **kwargs_)
         self.organ = organ
         self.organ_nsprefix_ = None
         self.tissue = tissue
         self.tissue_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
@@ -8535,21 +8847,21 @@
 # end class virus_species_name_type
 
 
 class virus_host_type(base_source_type):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = base_source_type
-    def __init__(self, database=None, organism=None, strain=None, synonym_organism=None, gds_collector_=None, **kwargs_):
+    def __init__(self, database=None, synthetically_produced=None, organism=None, strain=None, synonym_organism=None, details=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
-        super(globals().get("virus_host_type"), self).__init__(database, organism, strain, synonym_organism,  **kwargs_)
+        super(globals().get("virus_host_type"), self).__init__(database, synthetically_produced, organism, strain, synonym_organism, details,  **kwargs_)
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
                 CurrentSubclassModule_, virus_host_type)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
         if virus_host_type.subclass:
@@ -9017,21 +9329,21 @@
 # end class base_macromolecule_type
 
 
 class macromolecule_source_type(base_source_type):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = base_source_type
-    def __init__(self, database=None, organism=None, strain=None, synonym_organism=None, organ=None, tissue=None, cell=None, organelle=None, cellular_location=None, gds_collector_=None, **kwargs_):
+    def __init__(self, database=None, synthetically_produced=None, organism=None, strain=None, synonym_organism=None, details=None, organ=None, tissue=None, cell=None, organelle=None, cellular_location=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
-        super(globals().get("macromolecule_source_type"), self).__init__(database, organism, strain, synonym_organism,  **kwargs_)
+        super(globals().get("macromolecule_source_type"), self).__init__(database, synthetically_produced, organism, strain, synonym_organism, details,  **kwargs_)
         self.organ = organ
         self.organ_nsprefix_ = None
         self.tissue = tissue
         self.tissue_nsprefix_ = None
         self.cell = cell
         self.cell_nsprefix_ = None
         self.organelle = organelle
@@ -14227,15 +14539,15 @@
         # Validate type microscopeType, a restriction on xs:token.
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, str):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             value = value
-            enumerations = ['FEI MORGAGNI', 'FEI POLARA 300', 'FEI TALOS ARCTICA', 'FEI TECNAI 10', 'FEI TECNAI 12', 'FEI TECNAI 20', 'FEI TECNAI ARCTICA', 'FEI TECNAI F20', 'FEI TECNAI F30', 'FEI TECNAI SPHERA', 'FEI TECNAI SPIRIT', 'FEI TITAN', 'FEI TITAN KRIOS', 'FEI/PHILIPS CM10', 'FEI/PHILIPS CM12', 'FEI/PHILIPS CM120T', 'FEI/PHILIPS CM200FEG', 'FEI/PHILIPS CM200FEG/SOPHIE', 'FEI/PHILIPS CM200FEG/ST', 'FEI/PHILIPS CM200FEG/UT', 'FEI/PHILIPS CM200T', 'FEI/PHILIPS CM300FEG/HE', 'FEI/PHILIPS CM300FEG/ST', 'FEI/PHILIPS CM300FEG/T', 'FEI/PHILIPS EM400', 'FEI/PHILIPS EM420', 'HITACHI EF2000', 'HITACHI H-9500SD', 'HITACHI H3000 UHVEM', 'HITACHI H7600', 'HITACHI HF2000', 'HITACHI HF3000', 'JEOL 100CX', 'JEOL 1000EES', 'JEOL 1010', 'JEOL 1200', 'JEOL 1200EX', 'JEOL 1200EXII', 'JEOL 1230', 'JEOL 1400', 'JEOL 2000EX', 'JEOL 2000EXII', 'JEOL 2010', 'JEOL 2010F', 'JEOL 2010HC', 'JEOL 2010HT', 'JEOL 2010UHR', 'JEOL 2011', 'JEOL 2100', 'JEOL 2100F', 'JEOL 2200FS', 'JEOL 2200FSC', 'JEOL 3000SFF', 'JEOL 3100FEF', 'JEOL 3100FFC', 'JEOL 3200FS', 'JEOL 3200FSC', 'JEOL 4000', 'JEOL 4000EX', 'JEOL CRYO ARM 200', 'JEOL CRYO ARM 300', 'JEOL KYOTO-3000SFF', 'TFS GLACIOS', 'TFS KRIOS', 'TFS TALOS', 'TFS TALOS L120C', 'TFS TALOS F200C', 'TFS TUNDRA', 'ZEISS LEO912', 'ZEISS LIBRA120PLUS']
+            enumerations = ['FEI MORGAGNI', 'FEI POLARA 300', 'FEI TALOS ARCTICA', 'FEI TECNAI 10', 'FEI TECNAI 12', 'FEI TECNAI 20', 'FEI TECNAI ARCTICA', 'FEI TECNAI F20', 'FEI TECNAI F30', 'FEI TECNAI SPHERA', 'FEI TECNAI SPIRIT', 'FEI TITAN', 'FEI TITAN KRIOS', 'FEI/PHILIPS CM10', 'FEI/PHILIPS CM12', 'FEI/PHILIPS CM120T', 'FEI/PHILIPS CM200FEG', 'FEI/PHILIPS CM200FEG/SOPHIE', 'FEI/PHILIPS CM200FEG/ST', 'FEI/PHILIPS CM200FEG/UT', 'FEI/PHILIPS CM200T', 'FEI/PHILIPS CM300FEG/HE', 'FEI/PHILIPS CM300FEG/ST', 'FEI/PHILIPS CM300FEG/T', 'FEI/PHILIPS EM400', 'FEI/PHILIPS EM420', 'HITACHI EF2000', 'HITACHI H-9500SD', 'HITACHI H3000 UHVEM', 'HITACHI H7600', 'HITACHI HF2000', 'HITACHI HF3000', 'JEOL 100CX', 'JEOL 1000EES', 'JEOL 1010', 'JEOL 1200', 'JEOL 1200EX', 'JEOL 1200EXII', 'JEOL 1230', 'JEOL 1400', 'JEOL 1400/HR + YPS FEG', 'JEOL 2000EX', 'JEOL 2000EXII', 'JEOL 2010', 'JEOL 2010F', 'JEOL 2010HC', 'JEOL 2010HT', 'JEOL 2010UHR', 'JEOL 2011', 'JEOL 2100', 'JEOL 2100F', 'JEOL 2200FS', 'JEOL 2200FSC', 'JEOL 3000SFF', 'JEOL 3100FEF', 'JEOL 3100FFC', 'JEOL 3200FS', 'JEOL 3200FSC', 'JEOL 4000', 'JEOL 4000EX', 'JEOL CRYO ARM 200', 'JEOL CRYO ARM 300', 'JEOL KYOTO-3000SFF', 'TFS GLACIOS', 'TFS KRIOS', 'TFS TALOS', 'TFS TALOS L120C', 'TFS TALOS F200C', 'TFS TUNDRA', 'ZEISS LEO912', 'ZEISS LIBRA120PLUS']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on microscopeType' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
     def validate_illumination_modeType(self, value):
         result = True
@@ -21370,15 +21682,15 @@
 # end class pixel_spacing_type
 
 
 class interpretation_type(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
-    def __init__(self, modelling_list=None, figure_list=None, segmentation_list=None, slices_list=None, additional_map_list=None, half_map_list=None, gds_collector_=None, **kwargs_):
+    def __init__(self, modelling_list=None, figure_list=None, segmentation_list=None, slices_list=None, additional_map_list=None, half_map_list=None, mask_list=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         self.modelling_list = modelling_list
         self.modelling_list_nsprefix_ = None
@@ -21388,14 +21700,16 @@
         self.segmentation_list_nsprefix_ = None
         self.slices_list = slices_list
         self.slices_list_nsprefix_ = None
         self.additional_map_list = additional_map_list
         self.additional_map_list_nsprefix_ = None
         self.half_map_list = half_map_list
         self.half_map_list_nsprefix_ = None
+        self.mask_list = mask_list
+        self.mask_list_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
                 CurrentSubclassModule_, interpretation_type)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
         if interpretation_type.subclass:
@@ -21427,22 +21741,27 @@
         return self.additional_map_list
     def set_additional_map_list(self, additional_map_list):
         self.additional_map_list = additional_map_list
     def get_half_map_list(self):
         return self.half_map_list
     def set_half_map_list(self, half_map_list):
         self.half_map_list = half_map_list
+    def get_mask_list(self):
+        return self.mask_list
+    def set_mask_list(self, mask_list):
+        self.mask_list = mask_list
     def has__content(self):
         if (
             self.modelling_list is not None or
             self.figure_list is not None or
             self.segmentation_list is not None or
             self.slices_list is not None or
             self.additional_map_list is not None or
-            self.half_map_list is not None
+            self.half_map_list is not None or
+            self.mask_list is not None
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='interpretation_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('interpretation_type')
         if imported_ns_def_ is not None:
@@ -21487,14 +21806,17 @@
             self.slices_list.export(outfile, level, namespaceprefix_, namespacedef_='', name_='slices_list', pretty_print=pretty_print)
         if self.additional_map_list is not None:
             namespaceprefix_ = self.additional_map_list_nsprefix_ + ':' if (UseCapturedNS_ and self.additional_map_list_nsprefix_) else ''
             self.additional_map_list.export(outfile, level, namespaceprefix_, namespacedef_='', name_='additional_map_list', pretty_print=pretty_print)
         if self.half_map_list is not None:
             namespaceprefix_ = self.half_map_list_nsprefix_ + ':' if (UseCapturedNS_ and self.half_map_list_nsprefix_) else ''
             self.half_map_list.export(outfile, level, namespaceprefix_, namespacedef_='', name_='half_map_list', pretty_print=pretty_print)
+        if self.mask_list is not None:
+            namespaceprefix_ = self.mask_list_nsprefix_ + ':' if (UseCapturedNS_ and self.mask_list_nsprefix_) else ''
+            self.mask_list.export(outfile, level, namespaceprefix_, namespacedef_='', name_='mask_list', pretty_print=pretty_print)
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
         self._buildAttributes(node, node.attrib, already_processed)
@@ -21531,14 +21853,19 @@
             self.additional_map_list = obj_
             obj_.original_tagname_ = 'additional_map_list'
         elif nodeName_ == 'half_map_list':
             obj_ = half_map_listType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.half_map_list = obj_
             obj_.original_tagname_ = 'half_map_list'
+        elif nodeName_ == 'mask_list':
+            obj_ = mask_listType.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            self.mask_list = obj_
+            obj_.original_tagname_ = 'mask_list'
 # end class interpretation_type
 
 
 class modelling_type(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
@@ -33356,15 +33683,15 @@
         # Validate type allowed_film_or_detector_model, a restriction on xs:token.
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, str):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             value = value
-            enumerations = ['AGFA SCIENTA FILM', 'DIRECT ELECTRON APOLLO (4k x 4k)', 'DIRECT ELECTRON DE-10 (5k x 4k)', 'DIRECT ELECTRON DE-12 (4k x 3k)', 'DIRECT ELECTRON DE-16 (4k x 4k)', 'DIRECT ELECTRON DE-20 (5k x 3k)', 'DIRECT ELECTRON DE-64 (8k x 8k)', 'FEI CETA (4k x 4k)', 'FEI EAGLE (2k x 2k)', 'FEI EAGLE (4k x 4k)', 'FEI FALCON I (4k x 4k)', 'FEI FALCON II (4k x 4k)', 'FEI FALCON III (4k x 4k)', 'FEI FALCON IV (4k x 4k)', 'GATAN K2 (4k x 4k)', 'GATAN K2 BASE (4k x 4k)', 'GATAN K2 IS (4k x 4k)', 'GATAN K2 QUANTUM (4k x 4k)', 'GATAN K2 SUMMIT (4k x 4k)', 'GATAN K3 (6k x 4k)', 'GATAN K3 BIOQUANTUM (6k x 4k)', 'GATAN MULTISCAN', 'GATAN ORIUS SC1000 (4k x 2.7k)', 'GATAN ORIUS SC200 (2k x 2k)', 'GATAN ORIUS SC600 (2.7k x 2.7k)', 'GATAN ULTRASCAN 1000 (2k x 2k)', 'GATAN ULTRASCAN 10000 (10k x 10k)', 'GATAN ULTRASCAN 4000 (4k x 4k)', 'GENERIC CCD', 'GENERIC CCD (2k x 2k)', 'GENERIC CCD (4k x 4k)', 'GENERIC FILM', 'GENERIC GATAN', 'GENERIC GATAN (2k x 2k)', 'GENERIC GATAN (4k x 4k)', 'GENERIC IMAGE PLATES', 'GENERIC TVIPS', 'GENERIC TVIPS (2k x 2k)', 'GENERIC TVIPS (4k x 4k)', 'KODAK 4489 FILM', 'KODAK SO-163 FILM', 'OTHER', 'PROSCAN TEM-PIV (2k x 2k)', 'SIA 15C (3k x 3k)', 'TFS FALCON 4i (4k x 4k)', 'TVIPS TEMCAM-F216 (2k x 2k)', 'TVIPS TEMCAM-F224 (2k x 2k)', 'TVIPS TEMCAM-F415 (4k x 4k)', 'TVIPS TEMCAM-F416 (4k x 4k)', 'TVIPS TEMCAM-F816 (8k x 8k)']
+            enumerations = ['AGFA SCIENTA FILM', 'DECTRIS SINGLA (1k x 1k)', 'DIRECT ELECTRON APOLLO (4k x 4k)', 'DIRECT ELECTRON DE-10 (5k x 4k)', 'DIRECT ELECTRON DE-12 (4k x 3k)', 'DIRECT ELECTRON DE-16 (4k x 4k)', 'DIRECT ELECTRON DE-20 (5k x 3k)', 'DIRECT ELECTRON DE-64 (8k x 8k)', 'FEI CETA (4k x 4k)', 'FEI EAGLE (2k x 2k)', 'FEI EAGLE (4k x 4k)', 'FEI FALCON I (4k x 4k)', 'FEI FALCON II (4k x 4k)', 'FEI FALCON III (4k x 4k)', 'FEI FALCON IV (4k x 4k)', 'GATAN K2 (4k x 4k)', 'GATAN K2 BASE (4k x 4k)', 'GATAN K2 IS (4k x 4k)', 'GATAN K2 QUANTUM (4k x 4k)', 'GATAN K2 SUMMIT (4k x 4k)', 'GATAN K3 (6k x 4k)', 'GATAN K3 BIOQUANTUM (6k x 4k)', 'GATAN MULTISCAN', 'GATAN ORIUS SC1000 (4k x 2.7k)', 'GATAN ORIUS SC200 (2k x 2k)', 'GATAN ORIUS SC600 (2.7k x 2.7k)', 'GATAN ULTRASCAN 1000 (2k x 2k)', 'GATAN ULTRASCAN 10000 (10k x 10k)', 'GATAN ULTRASCAN 4000 (4k x 4k)', 'GENERIC CCD', 'GENERIC CCD (2k x 2k)', 'GENERIC CCD (4k x 4k)', 'GENERIC FILM', 'GENERIC GATAN', 'GENERIC GATAN (2k x 2k)', 'GENERIC GATAN (4k x 4k)', 'GENERIC IMAGE PLATES', 'GENERIC TVIPS', 'GENERIC TVIPS (2k x 2k)', 'GENERIC TVIPS (4k x 4k)', 'KODAK 4489 FILM', 'KODAK SO-163 FILM', 'OTHER', 'PROSCAN TEM-PIV (2k x 2k)', 'SIA 15C (3k x 3k)', 'TFS FALCON 4i (4k x 4k)', 'TVIPS TEMCAM-F216 (2k x 2k)', 'TVIPS TEMCAM-F224 (2k x 2k)', 'TVIPS TEMCAM-F415 (4k x 4k)', 'TVIPS TEMCAM-F416 (4k x 4k)', 'TVIPS TEMCAM-F816 (8k x 8k)']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on allowed_film_or_detector_model' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
     def validate_categoryType43(self, value):
         # Validate type categoryType43, a restriction on xs:string.
@@ -43079,14 +43406,116 @@
             obj_ = map_type.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.half_map.append(obj_)
             obj_.original_tagname_ = 'half_map'
 # end class half_map_listType
 
 
+class mask_listType(GeneratedsSuper):
+    __hash__ = GeneratedsSuper.__hash__
+    subclass = None
+    superclass = None
+    def __init__(self, mask=None, gds_collector_=None, **kwargs_):
+        self.gds_collector_ = gds_collector_
+        self.gds_elementtree_node_ = None
+        self.original_tagname_ = None
+        self.parent_object_ = kwargs_.get('parent_object_')
+        self.ns_prefix_ = None
+        if mask is None:
+            self.mask = []
+        else:
+            self.mask = mask
+        self.mask_nsprefix_ = None
+    def factory(*args_, **kwargs_):
+        if CurrentSubclassModule_ is not None:
+            subclass = getSubclassFromModule_(
+                CurrentSubclassModule_, mask_listType)
+            if subclass is not None:
+                return subclass(*args_, **kwargs_)
+        if mask_listType.subclass:
+            return mask_listType.subclass(*args_, **kwargs_)
+        else:
+            return mask_listType(*args_, **kwargs_)
+    factory = staticmethod(factory)
+    def get_ns_prefix_(self):
+        return self.ns_prefix_
+    def set_ns_prefix_(self, ns_prefix):
+        self.ns_prefix_ = ns_prefix
+    def get_mask(self):
+        return self.mask
+    def set_mask(self, mask):
+        self.mask = mask
+    def add_mask(self, value):
+        self.mask.append(value)
+    def insert_mask_at(self, index, value):
+        self.mask.insert(index, value)
+    def replace_mask_at(self, index, value):
+        self.mask[index] = value
+    def has__content(self):
+        if (
+            self.mask
+        ):
+            return True
+        else:
+            return False
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='mask_listType', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('mask_listType')
+        if imported_ns_def_ is not None:
+            namespacedef_ = imported_ns_def_
+        if pretty_print:
+            eol_ = '\n'
+        else:
+            eol_ = ''
+        if self.original_tagname_ is not None and name_ == 'mask_listType':
+            name_ = self.original_tagname_
+        if UseCapturedNS_ and self.ns_prefix_:
+            namespaceprefix_ = self.ns_prefix_ + ':'
+        showIndent(outfile, level, pretty_print)
+        outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
+        already_processed = set()
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='mask_listType')
+        if self.has__content():
+            outfile.write('>%s' % (eol_, ))
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='mask_listType', pretty_print=pretty_print)
+            showIndent(outfile, level, pretty_print)
+            outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
+        else:
+            outfile.write('/>%s' % (eol_, ))
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='mask_listType'):
+        pass
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='mask_listType', fromsubclass_=False, pretty_print=True):
+        if pretty_print:
+            eol_ = '\n'
+        else:
+            eol_ = ''
+        for mask_ in self.mask:
+            namespaceprefix_ = self.mask_nsprefix_ + ':' if (UseCapturedNS_ and self.mask_nsprefix_) else ''
+            mask_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='mask', pretty_print=pretty_print)
+    def build(self, node, gds_collector_=None):
+        self.gds_collector_ = gds_collector_
+        if SaveElementTreeNode:
+            self.gds_elementtree_node_ = node
+        already_processed = set()
+        self.ns_prefix_ = node.prefix
+        self._buildAttributes(node, node.attrib, already_processed)
+        for child in node:
+            nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
+            self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+        return self
+    def _buildAttributes(self, node, attrs, already_processed):
+        pass
+    def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
+        if nodeName_ == 'mask':
+            obj_ = map_type.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            self.mask.append(obj_)
+            obj_.original_tagname_ = 'mask'
+# end class mask_listType
+
+
 class initial_modelType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, access_code=None, chain=None, details=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
@@ -43799,21 +44228,21 @@
 # end class non_subtom_final_reconstruction_type
 
 
 class cell_source_type(base_source_type):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = base_source_type
-    def __init__(self, database=None, organism=None, strain=None, synonym_organism=None, organ=None, tissue=None, cell=None, gds_collector_=None, **kwargs_):
+    def __init__(self, database=None, synthetically_produced=None, organism=None, strain=None, synonym_organism=None, details=None, organ=None, tissue=None, cell=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
-        super(globals().get("cell_source_type"), self).__init__(database, organism, strain, synonym_organism,  **kwargs_)
+        super(globals().get("cell_source_type"), self).__init__(database, synthetically_produced, organism, strain, synonym_organism, details,  **kwargs_)
         self.organ = organ
         self.organ_nsprefix_ = None
         self.tissue = tissue
         self.tissue_nsprefix_ = None
         self.cell = cell
         self.cell_nsprefix_ = None
     def factory(*args_, **kwargs_):
@@ -44349,14 +44778,15 @@
     "macromoleculeType",
     "macromolecule_listType",
     "macromolecule_list_type",
     "macromolecule_source_type",
     "macromolecules_and_complexes_type",
     "map_statistics_type",
     "map_type",
+    "mask_listType",
     "max",
     "max_angleType",
     "microscopy_centerType",
     "microscopy_listType",
     "min",
     "min_angleType",
     "modelling_listType",
@@ -44378,14 +44808,16 @@
     "organelle_source_type",
     "organism_type",
     "organizationType",
     "originType",
     "orthogonal_tiltType",
     "otherType",
     "otherType45",
+    "other_db_cross_reference_list_type",
+    "other_db_cross_reference_type",
     "other_macromolecule_type",
     "parallel_resolution",
     "particle_selection_type",
     "pdb_cross_reference_list_type",
     "pdb_cross_reference_type",
     "pdb_model_type",
     "perpendicular_resolution",
```

### Comparing `wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py` & `wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py` & `wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/data/emdb-v3.xsd` & `wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/data/emdb-v3.xsd`

 * *Files 1% similar despite different names*

#### Comparing `wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/data/emdb-v3.xsd` & `wwpdb.utils.emdb-1.5/wwpdb/utils/emdb/data/emdb-v3.xsd`

```diff
@@ -20,15 +20,15 @@
           <xs:sequence>
             <xs:element ref="validation_method" maxOccurs="unbounded"/>
           </xs:sequence>
         </xs:complexType>
       </xs:element>
     </xs:sequence>
     <xs:attribute name="emdb_id" type="emdb_id_type" use="required"/>
-    <xs:attribute name="version" type="xs:token" default="3.0.4.0"/>
+    <xs:attribute name="version" type="xs:token" default="3.0.7.2"/>
     <!-- <xs:attribute name="composite_structure" type="xs:boolean"/> -->
   </xs:complexType>
   <xs:complexType name="admin_type">
     <xs:sequence>
       <xs:element name="status_history_list" type="version_list_type" minOccurs="0"/>
       <xs:element name="current_status" type="version_type"/>
       <xs:element name="sites">
@@ -429,14 +429,15 @@
               </xs:complexType>
             </xs:element>
           </xs:sequence>
         </xs:complexType>
       </xs:element>
       <xs:element name="emdb_list" type="emdb_cross_reference_list_type" minOccurs="0"/>
       <xs:element name="pdb_list" type="pdb_cross_reference_list_type" minOccurs="0"/>
+      <xs:element name="other_db_list" type="other_db_cross_reference_list_type" minOccurs="0"/>
       <xs:element name="auxiliary_link_list" minOccurs="0">
         <xs:complexType>
           <xs:sequence minOccurs="1" maxOccurs="1">
             <xs:element name="auxiliary_link" type="auxiliary_link_type" maxOccurs="unbounded"/>
           </xs:sequence>
         </xs:complexType>
       </xs:element>
@@ -609,14 +610,27 @@
             <xs:element name="other" type="xs:string"/>
           </xs:choice>
         </xs:complexType>
       </xs:element>
       <xs:element name="details" type="xs:string" minOccurs="0"/>
     </xs:sequence>
   </xs:complexType>
+  <xs:complexType name="other_db_cross_reference_list_type">
+    <xs:sequence minOccurs="1" maxOccurs="1">
+      <xs:element name="db_reference" type="other_db_cross_reference_type" maxOccurs="unbounded"/>
+    </xs:sequence>
+  </xs:complexType>
+  <xs:complexType name="other_db_cross_reference_type">
+    <xs:sequence>
+      <xs:element name="db_name" type="xs:token"/>
+      <xs:element name="accession_id" type="xs:token"/>
+      <xs:element name="content_type" type="xs:token" minOccurs="0"/>
+      <xs:element name="details" type="xs:string" minOccurs="0"/>
+    </xs:sequence>
+  </xs:complexType>
   <xs:complexType name="auxiliary_link_type">
     <xs:sequence>
       <xs:element name="type">
         <xs:simpleType>
           <xs:restriction base="xs:token">
             <xs:enumeration value="2D EM DATA"/>
             <xs:enumeration value="CORRELATIVE LIGHT MICROSCOPY"/>
@@ -745,22 +759,24 @@
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="base_source_type">
     <xs:sequence>
       <xs:element name="organism" type="organism_type"/>
       <xs:element name="strain" type="xs:token" minOccurs="0"/>
       <xs:element name="synonym_organism" type="xs:token" minOccurs="0"/>
+      <xs:element name="details" type="xs:string" minOccurs="0"/>
     </xs:sequence>
     <xs:attribute name="database">
       <xs:simpleType>
         <xs:restriction base="xs:token">
           <xs:enumeration value="NCBI"/>
         </xs:restriction>
       </xs:simpleType>
     </xs:attribute>
+    <xs:attribute name="synthetically_produced" type="xs:boolean"/>
   </xs:complexType>
   <xs:complexType name="organism_type">
     <xs:simpleContent>
       <xs:extension base="xs:token">
         <xs:attribute name="ncbi" type="xs:positiveInteger"/>
       </xs:extension>
     </xs:simpleContent>
@@ -2048,14 +2064,15 @@
             <xs:enumeration value="JEOL 1000EES"/>
             <xs:enumeration value="JEOL 1010"/>
             <xs:enumeration value="JEOL 1200"/>
             <xs:enumeration value="JEOL 1200EX"/>
             <xs:enumeration value="JEOL 1200EXII"/>
             <xs:enumeration value="JEOL 1230"/>
             <xs:enumeration value="JEOL 1400"/>
+            <xs:enumeration value="JEOL 1400/HR + YPS FEG"/>
             <xs:enumeration value="JEOL 2000EX"/>
             <xs:enumeration value="JEOL 2000EXII"/>
             <xs:enumeration value="JEOL 2010"/>
             <xs:enumeration value="JEOL 2010F"/>
             <xs:enumeration value="JEOL 2010HC"/>
             <xs:enumeration value="JEOL 2010HT"/>
             <xs:enumeration value="JEOL 2010UHR"/>
@@ -2515,14 +2532,15 @@
       <xs:element name="version" type="xs:token" minOccurs="0"/>
       <xs:element name="processing_details" type="xs:string" minOccurs="0"/>
     </xs:sequence>
   </xs:complexType>
   <xs:simpleType name="allowed_film_or_detector_model">
     <xs:restriction base="xs:token">
       <xs:enumeration value="AGFA SCIENTA FILM"/>
+      <xs:enumeration value="DECTRIS SINGLA (1k x 1k)"/>
       <xs:enumeration value="DIRECT ELECTRON APOLLO (4k x 4k)"/>
       <xs:enumeration value="DIRECT ELECTRON DE-10 (5k x 4k)"/>
       <xs:enumeration value="DIRECT ELECTRON DE-12 (4k x 3k)"/>
       <xs:enumeration value="DIRECT ELECTRON DE-16 (4k x 4k)"/>
       <xs:enumeration value="DIRECT ELECTRON DE-20 (5k x 3k)"/>
       <xs:enumeration value="DIRECT ELECTRON DE-64 (8k x 8k)"/>
       <xs:enumeration value="FEI CETA (4k x 4k)"/>
@@ -3796,14 +3814,21 @@
                 <xs:complexType>
                     <xs:sequence>
                         <xs:element name="ref_map" minOccurs="0" type="map_type"/>
                     </xs:sequence>
                 </xs:complexType>
             </xs:element>
             -->
+      <xs:element minOccurs="0" name="mask_list">
+        <xs:complexType>
+          <xs:sequence>
+            <xs:element maxOccurs="unbounded" name="mask" type="map_type"/>
+          </xs:sequence>
+        </xs:complexType>
+      </xs:element>
     </xs:sequence>
   </xs:complexType>
   <xs:complexType name="modelling_type">
     <xs:sequence>
       <xs:element name="initial_model" minOccurs="0" maxOccurs="unbounded">
         <xs:complexType>
           <xs:sequence>
```

### Comparing `wwpdb.utils.emdb-1.4.3/wwpdb.utils.emdb.egg-info/PKG-INFO` & `wwpdb.utils.emdb-1.5/wwpdb.utils.emdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.emdb
-Version: 1.4.3
+Version: 1.5
 Summary: wwPDB EMDB to XML converter
 Home-page: https://github.com/rcsb/py-wwpdb_utils_config
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.emdb-1.4.3/wwpdb.utils.emdb.egg-info/SOURCES.txt` & `wwpdb.utils.emdb-1.5/wwpdb.utils.emdb.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -16,11 +16,10 @@
 wwpdb/utils/emdb/atomcheck/__init__.py
 wwpdb/utils/emdb/atomcheck/atomcheck.py
 wwpdb/utils/emdb/cif_emdb_translator/README.md
 wwpdb/utils/emdb/cif_emdb_translator/__init__.py
 wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py
 wwpdb/utils/emdb/cif_emdb_translator/em_emd_conversion.py
 wwpdb/utils/emdb/cif_emdb_translator/emdb.py
-wwpdb/utils/emdb/cif_emdb_translator/generatedsnamespaces.py
 wwpdb/utils/emdb/cif_emdb_translator/simple_test.py
 wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py
 wwpdb/utils/emdb/data/emdb-v3.xsd
```

