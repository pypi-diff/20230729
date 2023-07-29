# Comparing `tmp/spark_generated_rules_tools-0.1.2.tar.gz` & `tmp/spark_generated_rules_tools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_generated_rules_tools-0.1.2.tar", last modified: Sat Jul 29 12:22:56 2023, max compression
+gzip compressed data, was "spark_generated_rules_tools-0.1.3.tar", last modified: Sat Jul 29 15:21:18 2023, max compression
```

## Comparing `spark_generated_rules_tools-0.1.2.tar` & `spark_generated_rules_tools-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 12:22:56.780182 spark_generated_rules_tools-0.1.2/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_generated_rules_tools-0.1.2/LICENSE
--rw-rw-rw-   0        0        0       52 2023-07-18 06:18:04.000000 spark_generated_rules_tools-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2411 2023-07-29 12:22:56.780182 spark_generated_rules_tools-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1604 2023-07-18 06:35:00.000000 spark_generated_rules_tools-0.1.2/README.md
--rw-rw-rw-   0        0        0      689 2023-07-18 06:18:04.000000 spark_generated_rules_tools-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-07-29 12:22:56.785185 spark_generated_rules_tools-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1218 2023-07-29 12:22:34.000000 spark_generated_rules_tools-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 12:22:56.758257 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools/
--rw-rw-rw-   0        0        0     1101 2023-07-29 05:44:29.000000 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 12:22:56.777334 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    24415 2023-07-29 12:21:38.000000 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-07-29 12:22:56.779334 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools/utils/color.py
-drwxrwxrwx   0        0        0        0 2023-07-29 12:22:56.779334 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools/utils/resource/
--rw-rw-rw-   0        0        0    26115 2023-07-29 02:06:11.000000 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools/utils/resource/rules.json
--rw-rw-rw-   0        0        0      501 2023-07-29 03:39:01.000000 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools/utils/utilitty.py
-drwxrwxrwx   0        0        0        0 2023-07-29 12:22:56.773356 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools.egg-info/
--rw-rw-rw-   0        0        0     2411 2023-07-29 12:22:56.000000 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      647 2023-07-29 12:22:56.000000 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 12:22:56.000000 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      205 2023-07-29 12:22:56.000000 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-07-29 12:22:56.000000 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 15:21:18.667905 spark_generated_rules_tools-0.1.3/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_generated_rules_tools-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0       52 2023-07-18 06:18:04.000000 spark_generated_rules_tools-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2411 2023-07-29 15:21:18.667905 spark_generated_rules_tools-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1604 2023-07-18 06:35:00.000000 spark_generated_rules_tools-0.1.3/README.md
+-rw-rw-rw-   0        0        0      689 2023-07-18 06:18:04.000000 spark_generated_rules_tools-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-07-29 15:21:18.669906 spark_generated_rules_tools-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1218 2023-07-29 15:21:17.000000 spark_generated_rules_tools-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 15:21:18.618894 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools/
+-rw-rw-rw-   0        0        0     1101 2023-07-29 05:44:29.000000 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 15:21:18.642899 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    25322 2023-07-29 15:21:17.000000 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-07-29 15:21:18.659903 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools/utils/color.py
+drwxrwxrwx   0        0        0        0 2023-07-29 15:21:18.667905 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools/utils/resource/
+-rw-rw-rw-   0        0        0    26115 2023-07-29 02:06:11.000000 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools/utils/resource/rules.json
+-rw-rw-rw-   0        0        0      501 2023-07-29 03:39:01.000000 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools/utils/utilitty.py
+drwxrwxrwx   0        0        0        0 2023-07-29 15:21:18.641899 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools.egg-info/
+-rw-rw-rw-   0        0        0     2411 2023-07-29 15:21:18.000000 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      647 2023-07-29 15:21:18.000000 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 15:21:18.000000 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      205 2023-07-29 15:21:18.000000 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-07-29 15:21:18.000000 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools.egg-info/top_level.txt
```

### Comparing `spark_generated_rules_tools-0.1.2/LICENSE` & `spark_generated_rules_tools-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_generated_rules_tools-0.1.2/PKG-INFO` & `spark_generated_rules_tools-0.1.3/spark_generated_rules_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: spark_generated_rules_tools
-Version: 0.1.2
+Name: spark-generated-rules-tools
+Version: 0.1.3
 Summary: spark_generated_rules_tools
 Home-page: https://github.com/jonaqp/spark_generated_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_generated_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_generated_rules_tools-0.1.2/README.md` & `spark_generated_rules_tools-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `spark_generated_rules_tools-0.1.2/pyproject.toml` & `spark_generated_rules_tools-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spark_generated_rules_tools-0.1.2/setup.py` & `spark_generated_rules_tools-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_generated_rules_tools',
     packages=find_packages(),
-    version='0.1.2',
+    version='0.1.3',
     description='spark_generated_rules_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_generated_rules_tools/',
     download_url='https://github.com/jonaqp/spark_generated_rules_tools/archive/main.zip',
```

### Comparing `spark_generated_rules_tools-0.1.2/spark_generated_rules_tools/__init__.py` & `spark_generated_rules_tools-0.1.3/spark_generated_rules_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_generated_rules_tools-0.1.2/spark_generated_rules_tools/functions/generator.py` & `spark_generated_rules_tools-0.1.3/spark_generated_rules_tools/functions/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,66 +60,67 @@
                                 hamu_type=None):
     import sys
     import os
     import json
     from pyhocon import ConfigFactory
     from pyhocon import HOCONConverter
     from spark_generated_rules_tools import get_color, get_color_b
-
     is_windows = sys.platform.startswith('win')
     dir_hocons_mvp_name = os.getenv('pj_dq_dir_mvp_name')
     dir_hocons_mvp_filename = ""
-
     table_dict = dict()
     table_list = list()
     if table_name not in table_dict.keys():
         physical_target_name = str(str(target_path_name).split("/")[-1])
         uuaa_tag = "".join(table_name.split("_")[2:])
+        physical_target_name_extension = str(physical_target_name.split(".")[-1])
         table_dict[table_name] = dict(hammurabi=dict())
         table_dict[table_name]["hammurabi"]["dataFrameInfo"] = dict()
         table_dict[table_name]["hammurabi"]["dataFrameInfo"]["cutoffDate"] = "${?REPROCESS_DATE}"
         table_dict[table_name]["hammurabi"]["dataFrameInfo"]["frequencyRuleExecution"] = periodicity
         table_dict[table_name]["hammurabi"]["dataFrameInfo"]["physicalTargetName"] = f"{physical_target_name}"
         table_dict[table_name]["hammurabi"]["dataFrameInfo"]["targetPathName"] = f"{target_path_name}"
         table_dict[table_name]["hammurabi"]["dataFrameInfo"]["uuaa"] = namespace
 
         if hamu_type == "staging":
             dir_hocons_mvp_filename = os.path.join(dir_hocons_mvp_name, f"{table_name}", "staging.conf")
-
             table_dict[table_name]["hammurabi"]["dataFrameInfo"]["subset"] = "cutoff_date='${?DATE}'"
             table_dict[table_name]["hammurabi"]["Input"] = dict()
+
             table_dict[table_name]["hammurabi"]["Input"]["options"] = dict(delimiter="|", castMode="notPermissive", charset="UTF-8")
             table_dict[table_name]["hammurabi"]["Input"]["paths"] = [f"{target_path_name}"]
             table_dict[table_name]["hammurabi"]["Input"]["schema"] = dict(path="${ARTIFACTORY_UNIQUE_CACHE}/artifactory/${SCHEMAS_REPOSITORY}"
                                                                                f"/schemas/pe/{namespace}"
                                                                                f"/raw/{uuaa_tag}/latest/{uuaa_tag}.input.schema")
-            table_dict[table_name]["hammurabi"]["Input"]["type"] = "csv"
+            if physical_target_name_extension == "csv":
+                table_dict[table_name]["hammurabi"]["Input"]["type"] = "csv"
+            if physical_target_name_extension == "dat":
+                table_dict[table_name]["hammurabi"]["Input"]["type"] = "fixed"
 
         if hamu_type == "raw":
             dir_hocons_mvp_filename = os.path.join(dir_hocons_mvp_name, f"{table_name}", "raw.conf")
-
             table_dict[table_name]["hammurabi"]["dataFrameInfo"]["subset"] = "cutoff_date='${?DATE}'"
             table_dict[table_name]["hammurabi"]["Input"] = dict()
             table_dict[table_name]["hammurabi"]["Input"]["applyConversions"] = False
             table_dict[table_name]["hammurabi"]["Input"]["paths"] = [f"{target_path_name}"]
             table_dict[table_name]["hammurabi"]["Input"]["schema"] = dict(path="${ARTIFACTORY_UNIQUE_CACHE}/artifactory/${SCHEMAS_REPOSITORY}"
                                                                                f"/schemas/pe/{namespace}"
                                                                                f"/raw/{uuaa_tag}/latest/{uuaa_tag}.output.schema")
             table_dict[table_name]["hammurabi"]["Input"]["type"] = "avro"
 
         if hamu_type == "master":
             dir_hocons_mvp_filename = os.path.join(dir_hocons_mvp_name, f"{table_name}", "master.conf")
-
             table_dict[table_name]["hammurabi"]["dataFrameInfo"]["subset"] = "cutoff_date='${?REPROCESS_DATE}'"
             table_dict[table_name]["hammurabi"]["Input"] = dict()
             table_dict[table_name]["hammurabi"]["Input"]["paths"] = [f"{target_path_name}"]
             table_dict[table_name]["hammurabi"]["Input"]["schema"] = dict(path="${ARTIFACTORY_UNIQUE_CACHE}/artifactory/${SCHEMAS_REPOSITORY}"
                                                                                f"/schemas/pe/{namespace}"
                                                                                f"/master/{uuaa_tag}/latest/{uuaa_tag}.output.schema")
 
+            table_dict[table_name]["hammurabi"]["Input"]["options"] = dict()
             table_dict[table_name]["hammurabi"]["Input"]["options"]["overrideSchema"] = True
             table_dict[table_name]["hammurabi"]["Input"]["options"]["includeMetadataAndDeleted"] = True
             table_dict[table_name]["hammurabi"]["Input"]["type"] = "parquet"
         table_dict[table_name]["hammurabi"]["rules"] = list()
     table_dict[table_name]["hammurabi"]["rules"] = hamu_list
     table_list.append(table_name)
 
@@ -132,14 +133,16 @@
     hocons_file2 = HOCONConverter.convert(conf2, "hocon")
     with open(dir_hocons_mvp_filename, "w") as f:
         f.write(hocons_file2)
     with open(dir_hocons_mvp_filename) as f:
         txt_conf = f.read()
     txt_conf = txt_conf.replace('"${?REPROCESS_DATE}"', "${?REPROCESS_DATE}")
     txt_conf = txt_conf.replace("${?DATE}", '"${?DATE}"')
+    txt_conf = txt_conf.replace("${?YEAR_MONTH}", '"${?YEAR_MONTH}"')
+    txt_conf = txt_conf.replace("${?PERIOD}", '"${?PERIOD}"')
     txt_conf = txt_conf.replace("/artifactory/", '"/artifactory/"')
     txt_conf = txt_conf.replace('"${ARTIFACTORY_UNIQUE_CACHE}', "${ARTIFACTORY_UNIQUE_CACHE}")
     txt_conf = txt_conf.replace('"${SCHEMAS_REPOSITORY}', '"${SCHEMAS_REPOSITORY}"')
     with open(dir_hocons_mvp_filename, "w") as f:
         f.write(txt_conf)
     print(f"{get_color('HOCON CREATE:')} {get_color_b(dir_hocons_mvp_filename)}")
 
@@ -282,27 +285,26 @@
         t.add_row([key_name, value_name])
     print(t)
 
 
 def dq_generated_mvp(table_name=None,
                      periodicity="Daily",
                      target_staging_path=None,
-                     apply_ctl=True,
                      is_uuaa_tag=True):
     import os
     import requests
     import json
     from spark_generated_rules_tools.utils.utilitty import extract_only_column_text
     from spark_generated_rules_tools.utils.utilitty import extract_only_parenthesis
 
     dir_schema_name = os.getenv('pj_dq_dir_schema_name')
     uuaa_name = str(table_name.split("_")[1]).lower()
     uuaa_tag = "".join(table_name.split("_")[2:])
     table_name_extract = "_".join(table_name.split("_")[2:])
-
+    physical_target_name_extension = str(target_staging_path.split(".")[-1])
     uuaa_tag_table = table_name
     if is_uuaa_tag:
         uuaa_tag_table = uuaa_tag
 
     url_raw = "http://artifactory-gdt.central-02.nextgen.igrupobbva/" \
               "artifactory/gl-datio-da-generic-local/" \
               f"schemas/pe/{uuaa_name}/raw/" \
@@ -330,15 +332,14 @@
 
     with open(dir_raw_schema_filename) as f:
         artifactory_json = json.load(f)
 
     table_name = artifactory_json.get("name")
     namespace = artifactory_json.get("namespace")
     table_name_path = artifactory_json.get("physicalPath")
-    zone = artifactory_json.get("database").lower()
 
     key_columns_list = list()
     for row in artifactory_json["fields"]:
         _naming = str(row['name']).lower().strip()
         _type = row['type']
         _logical_format = row['logicalFormat']
         _format_dtype = str(extract_only_column_text(_logical_format)).upper()
@@ -355,22 +356,22 @@
     category_rule = "MVP"
 
     hamu_staging_list = list()
     hamu_raw_list = list()
     hamu_master_list = list()
     sequence = 0
     index2 = 0
-    i = 0
     for i, field_name in enumerate(key_columns_list):
         field_name_str = str(list(field_name.keys())[0])
         field_value = int(list(field_name.values())[0][1])
         format_regex = f"^[0-9a-bA-Z]{{1,{field_value}}}$"
 
         for index, rule_id in enumerate(rule_ids_staging):
-            index2 = str(index + sequence + i).zfill(3)
+            sequence += 1
+            index2 = str(sequence).zfill(3)
             hamu_dict, id_key_dict = dq_searching_rules(category_rule=category_rule, table_name=table_name,
                                                         rule_id=rule_id, sequence=index2)
             if 'columns' in hamu_dict["config"].keys():
                 hamu_dict["config"]["columns"] = [field_name_str]
             if 'column' in hamu_dict["config"].keys():
                 hamu_dict["config"]["columns"] = field_name_str
             if 'format' in hamu_dict["config"].keys():
@@ -382,18 +383,19 @@
             if 'balanceIds' in hamu_dict["config"].keys():
                 del hamu_dict["config"]['balanceIds']
             if 'withRefusals' in hamu_dict["config"].keys():
                 hamu_dict["config"]['withRefusals'] = True
             hamu_staging_list.append(hamu_dict)
         sequence = int(index2)
 
-    if apply_ctl:
-        i = 0
+    if physical_target_name_extension == "dat":
+        sequence = 0
         for index, rule_id in enumerate(rule_ids_ctl):
-            index2 = str(sequence + i).zfill(3)
+            sequence += 1
+            index2 = str(sequence).zfill(3)
             hamu_dict, id_key_dict = dq_searching_rules(category_rule=category_rule, table_name=table_name,
                                                         rule_id=rule_id, sequence=index2)
             hamu_dict["config"]["dataValues"] = dict(metadataType="", position="", length="", path="")
             if 'drillDown' in hamu_dict["config"].keys():
                 del hamu_dict["config"]['drillDown']
             if 'subset' in hamu_dict["config"].keys():
                 del hamu_dict["config"]['subset']
@@ -402,41 +404,48 @@
 
             hamu_dict["config"]["dataValues"]["metadataType"] = "ctl"
             hamu_dict["config"]["dataValues"]["position"] = 59
             hamu_dict["config"]["dataValues"]["length"] = 9
             hamu_dict["config"]["dataValues"]["path"] = target_staging_path.replace(".dat", ".ctl")
             hamu_staging_list.append(hamu_dict)
 
-    i = 0
+    sequence = 0
     for index, rule_id in enumerate(rule_ids_raw):
-        index2 = str(sequence + i).zfill(3)
+        sequence += 1
+        index2 = str(sequence).zfill(3)
         hamu_dict, id_key_dict = dq_searching_rules(category_rule=category_rule, table_name=table_name,
                                                     rule_id=rule_id, sequence=index2)
         hamu_dict["config"]["dataValues"] = dict(options=dict(), paths="", schema=dict(), type="")
         if 'drillDown' in hamu_dict["config"].keys():
             del hamu_dict["config"]['drillDown']
         if 'subset' in hamu_dict["config"].keys():
             del hamu_dict["config"]['subset']
         if 'balanceIds' in hamu_dict["config"].keys():
             del hamu_dict["config"]['balanceIds']
         if 'withRefusals' in hamu_dict["config"].keys():
-            hamu_dict["config"]['withRefusals'] = True
+            hamu_dict["config"]['withRefusals'] = False
+        if 'isCritical' in hamu_dict["config"].keys():
+            hamu_dict["config"]['isCritical'] = True
         hamu_dict["config"]["dataValues"]["options"]["delimiter"] = "|"
         hamu_dict["config"]["dataValues"]["options"]["castMode"] = "notPermissive"
         hamu_dict["config"]["dataValues"]["options"]["charset"] = "UTF-8"
         hamu_dict["config"]["dataValues"]["paths"] = [target_staging_path]
         hamu_dict["config"]["dataValues"]["schema"]["path"] = "${ARTIFACTORY_UNIQUE_CACHE}/artifactory/${SCHEMAS_REPOSITORY}" \
                                                               f"/schemas/pe/{uuaa_name}" \
                                                               f"/raw/{uuaa_tag_table}/latest/{uuaa_tag_table}.input.schema"
-        hamu_dict["config"]["dataValues"]["type"] = "csv"
+        if physical_target_name_extension == "dat":
+            hamu_dict["config"]["dataValues"]["type"] = "fixed"
+        if physical_target_name_extension == "csv":
+            hamu_dict["config"]["dataValues"]["type"] = "csv"
         hamu_raw_list.append(hamu_dict)
 
-    i = 0
+    sequence = 0
     for index, rule_id in enumerate(rule_ids_master):
-        index2 = str(sequence + i).zfill(3)
+        sequence += 1
+        index2 = str(sequence).zfill(3)
         hamu_dict, id_key_dict = dq_searching_rules(category_rule=category_rule, table_name=table_name, rule_id=rule_id, sequence=index2)
         hamu_dict["config"]["dataValues"] = dict(applyConversions="", paths="", schema=dict(), type="")
         if 'drillDown' in hamu_dict["config"].keys():
             del hamu_dict["config"]['drillDown']
         if 'subset' in hamu_dict["config"].keys():
             del hamu_dict["config"]['subset']
         if 'balanceIds' in hamu_dict["config"].keys():
@@ -458,24 +467,24 @@
             dq_generated_dataframe_info(namespace=namespace,
                                         table_name=table_name,
                                         periodicity=periodicity,
                                         target_path_name=target_path_name,
                                         hamu_list=hamu_staging_list,
                                         hamu_type=hamu_type)
 
-        if zone == "raw":
+        if hamu_type == "raw":
             target_path_name = table_name_path
             dq_generated_dataframe_info(namespace=namespace,
                                         table_name=table_name,
                                         periodicity=periodicity,
                                         target_path_name=target_path_name,
-                                        hamu_list=hamu_staging_list,
+                                        hamu_list=hamu_raw_list,
                                         hamu_type=hamu_type)
 
-        if zone == "master":
-            target_path_name = f"t_{namespace}_{table_name_extract}"
+        if hamu_type == "master":
+            target_path_name = f"/data/master/{namespace}/data/t_{namespace}_{table_name_extract}"
             dq_generated_dataframe_info(namespace=namespace,
                                         table_name=table_name,
                                         periodicity=periodicity,
                                         target_path_name=target_path_name,
-                                        hamu_list=hamu_staging_list,
+                                        hamu_list=hamu_master_list,
                                         hamu_type=hamu_type)
```

### Comparing `spark_generated_rules_tools-0.1.2/spark_generated_rules_tools/utils/resource/rules.json` & `spark_generated_rules_tools-0.1.3/spark_generated_rules_tools/utils/resource/rules.json`

 * *Files identical despite different names*

### Comparing `spark_generated_rules_tools-0.1.2/spark_generated_rules_tools.egg-info/PKG-INFO` & `spark_generated_rules_tools-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: spark-generated-rules-tools
-Version: 0.1.2
+Name: spark_generated_rules_tools
+Version: 0.1.3
 Summary: spark_generated_rules_tools
 Home-page: https://github.com/jonaqp/spark_generated_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_generated_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_generated_rules_tools-0.1.2/spark_generated_rules_tools.egg-info/SOURCES.txt` & `spark_generated_rules_tools-0.1.3/spark_generated_rules_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

