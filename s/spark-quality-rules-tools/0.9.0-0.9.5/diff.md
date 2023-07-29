# Comparing `tmp/spark_quality_rules_tools-0.9.0.tar.gz` & `tmp/spark_quality_rules_tools-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_quality_rules_tools-0.9.0.tar", last modified: Sun Jul 16 03:49:17 2023, max compression
+gzip compressed data, was "spark_quality_rules_tools-0.9.5.tar", last modified: Sat Jul 29 17:25:06 2023, max compression
```

## Comparing `spark_quality_rules_tools-0.9.0.tar` & `spark_quality_rules_tools-0.9.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 03:49:17.105161 spark_quality_rules_tools-0.9.0/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.9.0/LICENSE
--rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.9.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4041 2023-07-16 03:49:17.105161 spark_quality_rules_tools-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.9.0/README.md
--rw-rw-rw-   0        0        0      685 2023-07-06 02:24:33.000000 spark_quality_rules_tools-0.9.0/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-07-16 03:49:17.106161 spark_quality_rules_tools-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0     1210 2023-07-16 03:48:50.000000 spark_quality_rules_tools-0.9.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 03:49:17.083156 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/
--rw-rw-rw-   0        0        0     3068 2023-07-16 01:29:29.000000 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 03:49:17.100160 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    62025 2023-07-16 03:48:50.000000 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-07-16 03:49:17.103160 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/utils/color.py
--rw-rw-rw-   0        0        0     2138 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/utils/resolve.py
-drwxrwxrwx   0        0        0        0 2023-07-16 03:49:17.104160 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/utils/resource/
--rw-rw-rw-   0        0        0      532 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/utils/resource/resolve_edge.conf
--rw-rw-rw-   0        0        0      742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf
--rw-rw-rw-   0        0        0    25810 2023-07-14 13:19:59.000000 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/utils/resource/rules.json
--rw-rw-rw-   0        0        0     3920 2023-07-14 13:01:54.000000 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/utils/rules.py
-drwxrwxrwx   0        0        0        0 2023-07-16 03:49:17.098159 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools.egg-info/
--rw-rw-rw-   0        0        0     4041 2023-07-16 03:49:17.000000 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      784 2023-07-16 03:49:17.000000 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 03:49:17.000000 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      205 2023-07-16 03:49:17.000000 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-07-16 03:49:17.000000 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 17:25:06.723728 spark_quality_rules_tools-0.9.5/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.9.5/LICENSE
+-rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.9.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     4041 2023-07-29 17:25:06.723728 spark_quality_rules_tools-0.9.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.9.5/README.md
+-rw-rw-rw-   0        0        0      685 2023-07-06 02:24:33.000000 spark_quality_rules_tools-0.9.5/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-07-29 17:25:06.724719 spark_quality_rules_tools-0.9.5/setup.cfg
+-rw-rw-rw-   0        0        0     1210 2023-07-29 17:25:05.000000 spark_quality_rules_tools-0.9.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 17:25:06.659570 spark_quality_rules_tools-0.9.5/spark_quality_rules_tools/
+-rw-rw-rw-   0        0        0     2792 2023-07-29 17:25:05.000000 spark_quality_rules_tools-0.9.5/spark_quality_rules_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 17:25:06.684577 spark_quality_rules_tools-0.9.5/spark_quality_rules_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.9.5/spark_quality_rules_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    56542 2023-07-29 17:25:05.000000 spark_quality_rules_tools-0.9.5/spark_quality_rules_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-07-29 17:25:06.711582 spark_quality_rules_tools-0.9.5/spark_quality_rules_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.9.5/spark_quality_rules_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.9.5/spark_quality_rules_tools/utils/color.py
+-rw-rw-rw-   0        0        0     2138 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.9.5/spark_quality_rules_tools/utils/resolve.py
+drwxrwxrwx   0        0        0        0 2023-07-29 17:25:06.722727 spark_quality_rules_tools-0.9.5/spark_quality_rules_tools/utils/resource/
+-rw-rw-rw-   0        0        0      532 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.9.5/spark_quality_rules_tools/utils/resource/resolve_edge.conf
+-rw-rw-rw-   0        0        0      742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.9.5/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf
+-rw-rw-rw-   0        0        0    26115 2023-07-29 17:17:22.000000 spark_quality_rules_tools-0.9.5/spark_quality_rules_tools/utils/resource/rules.json
+-rw-rw-rw-   0        0        0     3920 2023-07-14 13:01:54.000000 spark_quality_rules_tools-0.9.5/spark_quality_rules_tools/utils/rules.py
+drwxrwxrwx   0        0        0        0 2023-07-29 17:25:06.682576 spark_quality_rules_tools-0.9.5/spark_quality_rules_tools.egg-info/
+-rw-rw-rw-   0        0        0     4041 2023-07-29 17:25:06.000000 spark_quality_rules_tools-0.9.5/spark_quality_rules_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      784 2023-07-29 17:25:06.000000 spark_quality_rules_tools-0.9.5/spark_quality_rules_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 17:25:06.000000 spark_quality_rules_tools-0.9.5/spark_quality_rules_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      205 2023-07-29 17:25:06.000000 spark_quality_rules_tools-0.9.5/spark_quality_rules_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-07-29 17:25:06.000000 spark_quality_rules_tools-0.9.5/spark_quality_rules_tools.egg-info/top_level.txt
```

### Comparing `spark_quality_rules_tools-0.9.0/LICENSE` & `spark_quality_rules_tools-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.9.0/PKG-INFO` & `spark_quality_rules_tools-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_quality_rules_tools
-Version: 0.9.0
+Version: 0.9.5
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.9.0/README.md` & `spark_quality_rules_tools-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.9.0/pyproject.toml` & `spark_quality_rules_tools-0.9.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.9.0/setup.py` & `spark_quality_rules_tools-0.9.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_quality_rules_tools',
     packages=find_packages(),
-    version='0.9.0',
+    version='0.9.5',
     description='spark_quality_rules_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_quality_rules_tools/',
     download_url='https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip',
```

### Comparing `spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/__init__.py` & `spark_quality_rules_tools-0.9.5/spark_quality_rules_tools/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,33 +13,29 @@
 from spark_quality_rules_tools.functions.generator import dq_validate_conf_artifactory
 from spark_quality_rules_tools.functions.generator import dq_validate_conf_file
 from spark_quality_rules_tools.functions.generator import dq_validate_file
 from spark_quality_rules_tools.functions.generator import dq_validate_file_with_rules
 from spark_quality_rules_tools.functions.generator import dq_get_rules_list
 from spark_quality_rules_tools.functions.generator import dq_generated_rules
 from spark_quality_rules_tools.functions.generator import dq_run_sandbox_archive_path_rules
-from spark_quality_rules_tools.functions.generator import dq_extract_parameters_file_malla
-from spark_quality_rules_tools.functions.generator import dq_extract_parameters_bitbucket_malla
 
 from spark_quality_rules_tools.utils import BASE_DIR
 from spark_quality_rules_tools.utils.color import get_color
 from spark_quality_rules_tools.utils.color import get_color_b
 from spark_quality_rules_tools.utils.resolve import get_replace_resolve_parameter
 from spark_quality_rules_tools.utils.rules import get_validate_rules
 
 generator_all = [
     "dq_creating_directory",
     "dq_spark_session",
     "dq_path_workspace",
     "dq_download_jar",
     "dq_get_rules_list",
     "dq_generated_rules",
-    "dq_searching_rules",
-    "dq_extract_parameters_file_malla",
-    "dq_extract_parameters_bitbucket_malla"
+    "dq_searching_rules"
 ]
 generator_artifactory = [
     "dq_validate_conf_artifactory",
     "dq_extract_parameters_artifactory",
     "dq_run_sandbox_artifactory",
     "dq_validate_rules_artifactory",
     "dq_validate_artifactory",
```

### Comparing `spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/functions/generator.py` & `spark_quality_rules_tools-0.9.5/spark_quality_rules_tools/functions/generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,46 +33,28 @@
                     elif rule_dtype[0] == "Double" and rule_dtype[2] == "100":
                         rules_value = ast.literal_eval(rule_dtype[2])
                     elif rule_dtype[0] == "String" and rule_dtype[2] in ("None", ""):
                         rules_value = ""
                     elif rule_dtype[0] == "Array[String]" and rule_dtype[2] in ("None", ""):
                         rules_value = ["default"]
                     elif rule_dtype[0] == "Dict" and rule_dtype[2] in ("None", ""):
-                        rules_value = dict(type="", paths="")
+                        rules_value = dict()
                     else:
                         rules_value = rule_dtype[2]
                     rs_dict[rule_name] = rules_value
                 if static_id:
                     rs_dict["id"] = static_id
                 else:
                     rule_id = str(rule_id).replace("-1", "").replace("-2", "").strip()
                     rs_dict["id"] = f"PE_{category_rule}_{table_name}_{rule_id}_{sequence}"
                 hamu_dict["class"] = rules_class
                 hamu_dict["config"] = rs_dict
     return hamu_dict, id_key_dict
 
 
-def dq_convert_url_bitbucket_artifactory(url_conf=None):
-    url = url_conf
-    url_conf_name = str(str(url).split("/")[-3])
-    url_conf_name = f"{url_conf_name}"
-    url_conf_zone = str(str(url).split("/")[-2])
-    uuaa_name = str(str(url).split("/")[-4])
-    url_conf = f"http://artifactory-gdt.central-02.nextgen.igrupobbva/" \
-               f"artifactory/gl-datio-generic-local/" \
-               f"kirby/" \
-               f"pe/" \
-               f"{uuaa_name.lower()}/" \
-               f"{url_conf_zone.lower()}/" \
-               f"{url_conf_name.lower()}/" \
-               f"0.1.0/" \
-               f"{url_conf_name.lower()}.conf"
-    return url_conf
-
-
 def dq_creating_directory_hdfs(spark=None, path=None):
     from spark_quality_rules_tools import get_color, get_color_b
 
     sc = spark.sparkContext
     fs = spark._jvm.org.apache.hadoop.fs.FileSystem.get(spark._jsc.hadoopConfiguration())
     if path in ("", None):
         raise Exception(f'required variable path')
@@ -885,15 +867,15 @@
         func.col("gf_cutoff_date"),
         func.col("gf_field_physical_name").alias("Field"),
         func.col("gf_qr_aux_attribute_desc").alias("Format"),
         func.col("g_qr_critical_type").alias("Is Critical"),
         func.col("gf_qr_min_acceptance_per").alias("% Acceptation"),
         func.col("g_quality_rule_status_type").alias("Status"),
         func.col("gf_quality_rule_compliance_per").alias("Por"))
-    df3 = df2.distinct().sort("gf_qr_functional_definition_id")
+    df3 = metrics_filter.distinct().sort("gf_qr_functional_definition_id")
     df3 = df3.select(*[func.col(col).cast("string") for col in df3.columns])
     df3.show(500, False, True)
 
     metrics_filter_pandas = df3.toPandas()
     metrics_filter_pandas.to_csv(dir_reports_name_filename, index=False)
 
     print(f"{get_color(f'================================')} ")
@@ -1172,115 +1154,7 @@
         conf2 = ConfigFactory.parse_string(json_file2)
         hocons_file2 = HOCONConverter.convert(conf2, "hocon")
 
         with open(dir_hocons_filename, "w") as f:
             f.write(hocons_file2)
 
         print(f"{get_color('HOCON CREATE:')} {get_color_b(dir_hocons_filename)}")
-
-
-def dq_extract_parameters_file_malla(file_conf=None, uuaa=None):
-    import os
-    import sys
-    import re
-    import json
-    from spark_quality_rules_tools import get_color, get_color_b
-
-    is_windows = sys.platform.startswith('win')
-    dir_confs_name = os.getenv('pj_dq_dir_confs_name')
-    if file_conf in ("", None):
-        raise Exception(f'required variable url_conf')
-    if dir_confs_name is None:
-        raise Exception(f'required environment: pj_dq_dir_confs_name')
-
-    url_conf_name = str(str(file_conf).split(".")[0])
-    uuaa_name = str(uuaa).upper()
-    dir_confs_filename = os.path.join(dir_confs_name, uuaa_name, f"{url_conf_name}.txt")
-    dir_confs_env_parameters = os.path.join(dir_confs_name, uuaa_name, f"PARAMS_ENV.json")
-
-    if is_windows:
-        dir_confs_filename = dir_confs_filename.replace("\\", "/")
-        dir_confs_env_parameters = dir_confs_env_parameters.replace("\\", "/")
-    os.makedirs(os.path.dirname(dir_confs_filename), exist_ok=True)
-
-    with open(file_conf) as file:
-        hammurabi_conf = file.read()
-    with open(dir_confs_filename, 'w') as file:
-        file.write(hammurabi_conf)
-    with open(dir_confs_filename) as f:
-        hammurabi_conf = f.read()
-    variables_1 = sorted(list(set(re.findall(r'{([a-zA-Z_.-]+)}', hammurabi_conf))))
-    variables_2 = sorted(list(set(re.findall(r'{?([a-zA-Z_.-]+)}', hammurabi_conf))))
-    variables_list = list(set(variables_1 + variables_2))
-    variables_dict = {variables: "" for variables in variables_list if
-                      variables not in ("ARTIFACTORY_UNIQUE_CACHE", "SCHEMAS_REPOSITORY", "TEST_PATH")}
-    env_variables = {key: f"%%PARM{i + 1}" for i, key in enumerate(variables_dict)}
-    env_controlm = {"CONTROLM_JOB_ID": "%%JOBNAME", "CONTROLM_JOB_FLOW": "%%SCHEDTAB"}
-    env_dict = dict()
-    env_dict["env"] = dict()
-    env_dict["env"].update(env_variables)
-    env_dict["env"].update(env_controlm)
-    with open(f"{dir_confs_env_parameters}", "w") as f:
-        json.dump(env_dict, f)
-
-    with open(f"{dir_confs_env_parameters}") as f:
-        parameter_conf = f.read()
-
-    print(f"{get_color('ENV:')} {get_color_b(parameter_conf)}")
-
-
-def dq_extract_parameters_bitbucket_malla(url_conf=None):
-    import os
-    import sys
-    import re
-    import json
-    import requests
-    from spark_quality_rules_tools import get_color, get_color_b
-
-    is_windows = sys.platform.startswith('win')
-    dir_confs_name = os.getenv('pj_dq_dir_confs_name')
-    if url_conf in ("", None):
-        raise Exception(f'required variable url_conf')
-    if dir_confs_name is None:
-        raise Exception(f'required environment: pj_dq_dir_confs_name')
-
-    url = dq_convert_url_bitbucket_artifactory(url_conf=url_conf)
-    url_conf_extension = str(str(url).split("/")[-1]).replace("-", "_").upper().strip()
-    url_conf_name = str(str(url_conf_extension).split(".")[0])
-    uuaa_name = str(str(url).split("/")[-2]).upper()
-    if not len(uuaa_name) == 4:
-        uuaa_name = str(str(url).split("/")[-5]).upper()
-    dir_confs_filename = os.path.join(dir_confs_name, uuaa_name, f"{url_conf_name}.txt")
-    dir_confs_env_parameters = os.path.join(dir_confs_name, uuaa_name, f"PARAMS_ENV.json")
-
-    if is_windows:
-        dir_confs_filename = dir_confs_filename.replace("\\", "/")
-        dir_confs_env_parameters = dir_confs_env_parameters.replace("\\", "/")
-    os.makedirs(os.path.dirname(dir_confs_filename), exist_ok=True)
-
-    with requests.get(url, stream=True, verify=True) as r:
-        r.raise_for_status()
-        with open(dir_confs_filename, 'wb+') as f:
-            for chunk in r.iter_content(chunk_size=8192):
-                f.write(chunk)
-    with open(dir_confs_filename) as f:
-        hammurabi_conf = f.read()
-    variables_1 = sorted(list(set(re.findall(r'{([a-zA-Z_.-]+)}', hammurabi_conf))))
-    variables_2 = sorted(list(set(re.findall(r'{?([a-zA-Z_.-]+)}', hammurabi_conf))))
-    variables_list = list(set(variables_1 + variables_2))
-    variables_dict = {variables: "" for variables in variables_list if
-                      variables not in ("ARTIFACTORY_UNIQUE_CACHE", "SCHEMAS_REPOSITORY", "TEST_PATH")}
-
-    env_variables = {key: f"%%PARM{i + 1}" for i, key in enumerate(variables_dict)}
-    env_controlm = {"CONTROLM_JOB_ID": "%%JOBNAME", "CONTROLM_JOB_FLOW": "%%SCHEDTAB"}
-    env_dict = dict()
-    env_dict["env"] = dict()
-    env_dict["env"].update(env_variables)
-    env_dict["env"].update(env_controlm)
-
-    with open(f"{dir_confs_env_parameters}", "w") as f:
-        json.dump(env_dict, f)
-
-    with open(f"{dir_confs_env_parameters}") as f:
-        parameter_conf = f.read()
-
-    print(f"{get_color('ENV:')} {get_color_b(parameter_conf)}")
```

### Comparing `spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/utils/resolve.py` & `spark_quality_rules_tools-0.9.5/spark_quality_rules_tools/utils/resolve.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/utils/resource/resolve_edge.conf` & `spark_quality_rules_tools-0.9.5/spark_quality_rules_tools/utils/resource/resolve_edge.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf` & `spark_quality_rules_tools-0.9.5/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/utils/resource/rules.json` & `spark_quality_rules_tools-0.9.5/spark_quality_rules_tools/utils/resource/rules.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998640046296297%*

 * *Differences: {"'rules_config'": "{'completeness': {'CompletenessRule': {0: {'rules_columns': {0: "*

 * *                   "{'withRefusals': ['Boolean', 'False', 'False']}}}}, "*

 * *                   "'BasicPerimeterCompletenessRule': {0: {'rules_columns': {0: {'withRefusals': "*

 * *                   "['Boolean', 'False', 'False']}}}}, 'BasicPerimeterVariationCompletenessRule': "*

 * *                   "{0: {'rules_columns': {0: {'withRefusals': ['Boolean', 'False', 'False']}}}}, "*

 * *                   "'ConditionalPerimeterCompleteness […]*

```diff
@@ -626,14 +626,19 @@
                                 "False",
                                 "None"
                             ],
                             "targetThreshold": [
                                 "Double",
                                 "False",
                                 "100"
+                            ],
+                            "withRefusals": [
+                                "Boolean",
+                                "False",
+                                "False"
                             ]
                         }
                     ],
                     "rules_name": "Perimeter Completeness",
                     "rules_version": "2.2-1"
                 }
             ],
@@ -673,14 +678,19 @@
                                 "False",
                                 "None"
                             ],
                             "targetThreshold": [
                                 "Double",
                                 "False",
                                 "100"
+                            ],
+                            "withRefusals": [
+                                "Boolean",
+                                "False",
+                                "False"
                             ]
                         }
                     ],
                     "rules_name": "Perimeter Completeness",
                     "rules_version": "2.2-2"
                 }
             ],
@@ -710,14 +720,19 @@
                                 "False",
                                 "100"
                             ],
                             "targetThreshold": [
                                 "Double",
                                 "False",
                                 "100"
+                            ],
+                            "withRefusals": [
+                                "Boolean",
+                                "False",
+                                "False"
                             ]
                         }
                     ],
                     "rules_name": "Records Completeness",
                     "rules_version": "2.1"
                 }
             ],
@@ -762,14 +777,19 @@
                                 "False",
                                 "None"
                             ],
                             "targetThreshold": [
                                 "Double",
                                 "False",
                                 "100"
+                            ],
+                            "withRefusals": [
+                                "Boolean",
+                                "False",
+                                "False"
                             ]
                         }
                     ],
                     "rules_name": "Perimeter completeness with a filter",
                     "rules_version": "2.3-1"
                 }
             ],
@@ -809,14 +829,19 @@
                                 "False",
                                 "None"
                             ],
                             "targetThreshold": [
                                 "Double",
                                 "False",
                                 "100"
+                            ],
+                            "withRefusals": [
+                                "Boolean",
+                                "False",
+                                "False"
                             ]
                         }
                     ],
                     "rules_name": "Metadata completeness",
                     "rules_version": "2.4"
                 }
             ]
```

### Comparing `spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/utils/rules.py` & `spark_quality_rules_tools-0.9.5/spark_quality_rules_tools/utils/rules.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.9.0/spark_quality_rules_tools.egg-info/PKG-INFO` & `spark_quality_rules_tools-0.9.5/spark_quality_rules_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-quality-rules-tools
-Version: 0.9.0
+Version: 0.9.5
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.9.0/spark_quality_rules_tools.egg-info/SOURCES.txt` & `spark_quality_rules_tools-0.9.5/spark_quality_rules_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

