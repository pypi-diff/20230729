# Comparing `tmp/spark_generated_rules_tools-0.1.3.tar.gz` & `tmp/spark_generated_rules_tools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_generated_rules_tools-0.1.3.tar", last modified: Sat Jul 29 15:21:18 2023, max compression
+gzip compressed data, was "spark_generated_rules_tools-0.2.0.tar", last modified: Sat Jul 29 17:29:36 2023, max compression
```

## Comparing `spark_generated_rules_tools-0.1.3.tar` & `spark_generated_rules_tools-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 15:21:18.667905 spark_generated_rules_tools-0.1.3/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_generated_rules_tools-0.1.3/LICENSE
--rw-rw-rw-   0        0        0       52 2023-07-18 06:18:04.000000 spark_generated_rules_tools-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2411 2023-07-29 15:21:18.667905 spark_generated_rules_tools-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1604 2023-07-18 06:35:00.000000 spark_generated_rules_tools-0.1.3/README.md
--rw-rw-rw-   0        0        0      689 2023-07-18 06:18:04.000000 spark_generated_rules_tools-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-07-29 15:21:18.669906 spark_generated_rules_tools-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1218 2023-07-29 15:21:17.000000 spark_generated_rules_tools-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 15:21:18.618894 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools/
--rw-rw-rw-   0        0        0     1101 2023-07-29 05:44:29.000000 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 15:21:18.642899 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    25322 2023-07-29 15:21:17.000000 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-07-29 15:21:18.659903 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools/utils/color.py
-drwxrwxrwx   0        0        0        0 2023-07-29 15:21:18.667905 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools/utils/resource/
--rw-rw-rw-   0        0        0    26115 2023-07-29 02:06:11.000000 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools/utils/resource/rules.json
--rw-rw-rw-   0        0        0      501 2023-07-29 03:39:01.000000 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools/utils/utilitty.py
-drwxrwxrwx   0        0        0        0 2023-07-29 15:21:18.641899 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools.egg-info/
--rw-rw-rw-   0        0        0     2411 2023-07-29 15:21:18.000000 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      647 2023-07-29 15:21:18.000000 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 15:21:18.000000 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      205 2023-07-29 15:21:18.000000 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-07-29 15:21:18.000000 spark_generated_rules_tools-0.1.3/spark_generated_rules_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 17:29:36.256533 spark_generated_rules_tools-0.2.0/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_generated_rules_tools-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0       52 2023-07-18 06:18:04.000000 spark_generated_rules_tools-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2411 2023-07-29 17:29:36.256533 spark_generated_rules_tools-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1604 2023-07-18 06:35:00.000000 spark_generated_rules_tools-0.2.0/README.md
+-rw-rw-rw-   0        0        0      689 2023-07-18 06:18:04.000000 spark_generated_rules_tools-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-07-29 17:29:36.258511 spark_generated_rules_tools-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1218 2023-07-29 17:29:34.000000 spark_generated_rules_tools-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 17:29:36.237855 spark_generated_rules_tools-0.2.0/spark_generated_rules_tools/
+-rw-rw-rw-   0        0        0     1425 2023-07-29 17:29:34.000000 spark_generated_rules_tools-0.2.0/spark_generated_rules_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 17:29:36.253859 spark_generated_rules_tools-0.2.0/spark_generated_rules_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_generated_rules_tools-0.2.0/spark_generated_rules_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    30119 2023-07-29 17:29:34.000000 spark_generated_rules_tools-0.2.0/spark_generated_rules_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-07-29 17:29:36.255860 spark_generated_rules_tools-0.2.0/spark_generated_rules_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_generated_rules_tools-0.2.0/spark_generated_rules_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_generated_rules_tools-0.2.0/spark_generated_rules_tools/utils/color.py
+drwxrwxrwx   0        0        0        0 2023-07-29 17:29:36.256533 spark_generated_rules_tools-0.2.0/spark_generated_rules_tools/utils/resource/
+-rw-rw-rw-   0        0        0    26115 2023-07-29 02:06:11.000000 spark_generated_rules_tools-0.2.0/spark_generated_rules_tools/utils/resource/rules.json
+-rw-rw-rw-   0        0        0      501 2023-07-29 03:39:01.000000 spark_generated_rules_tools-0.2.0/spark_generated_rules_tools/utils/utilitty.py
+drwxrwxrwx   0        0        0        0 2023-07-29 17:29:36.252859 spark_generated_rules_tools-0.2.0/spark_generated_rules_tools.egg-info/
+-rw-rw-rw-   0        0        0     2411 2023-07-29 17:29:36.000000 spark_generated_rules_tools-0.2.0/spark_generated_rules_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      647 2023-07-29 17:29:36.000000 spark_generated_rules_tools-0.2.0/spark_generated_rules_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 17:29:36.000000 spark_generated_rules_tools-0.2.0/spark_generated_rules_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      205 2023-07-29 17:29:36.000000 spark_generated_rules_tools-0.2.0/spark_generated_rules_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-07-29 17:29:36.000000 spark_generated_rules_tools-0.2.0/spark_generated_rules_tools.egg-info/top_level.txt
```

### Comparing `spark_generated_rules_tools-0.1.3/LICENSE` & `spark_generated_rules_tools-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_generated_rules_tools-0.1.3/PKG-INFO` & `spark_generated_rules_tools-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_generated_rules_tools
-Version: 0.1.3
+Version: 0.2.0
 Summary: spark_generated_rules_tools
 Home-page: https://github.com/jonaqp/spark_generated_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_generated_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_generated_rules_tools-0.1.3/README.md` & `spark_generated_rules_tools-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `spark_generated_rules_tools-0.1.3/pyproject.toml` & `spark_generated_rules_tools-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spark_generated_rules_tools-0.1.3/setup.py` & `spark_generated_rules_tools-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_generated_rules_tools',
     packages=find_packages(),
-    version='0.1.3',
+    version='0.2.0',
     description='spark_generated_rules_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_generated_rules_tools/',
     download_url='https://github.com/jonaqp/spark_generated_rules_tools/archive/main.zip',
```

### Comparing `spark_generated_rules_tools-0.1.3/spark_generated_rules_tools/__init__.py` & `spark_generated_rules_tools-0.2.0/spark_generated_rules_tools/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 from spark_generated_rules_tools.functions.generator import dq_creating_directory_sandbox
 from spark_generated_rules_tools.functions.generator import dq_generated_rules
 from spark_generated_rules_tools.functions.generator import dq_get_rules_list
 from spark_generated_rules_tools.functions.generator import dq_path_workspace
 from spark_generated_rules_tools.functions.generator import dq_searching_rules
 from spark_generated_rules_tools.functions.generator import dq_generated_dataframe_info
 from spark_generated_rules_tools.functions.generator import dq_generated_mvp
+from spark_generated_rules_tools.functions.generator import dq_extract_parameters_file_malla
+from spark_generated_rules_tools.functions.generator import dq_extract_parameters_bitbucket_malla
 from spark_generated_rules_tools.utils import BASE_DIR
 from spark_generated_rules_tools.utils.color import get_color
 from spark_generated_rules_tools.utils.color import get_color_b
 
+generator_malla = [
+    "dq_extract_parameters_bitbucket_malla",
+    "dq_extract_parameters_file_malla"
+]
+
 generator_all = [
     "dq_generated_rules",
     "dq_get_rules_list",
     "dq_path_workspace",
     "dq_searching_rules",
     "dq_creating_directory_sandbox",
     "dq_generated_dataframe_info",
-    "dq_generated_mvp"
+    "dq_generated_mvp",
 ]
 
 utils_all = [
     "BASE_DIR",
     "get_color",
     "get_color_b"
 ]
 
-__all__ = generator_all + utils_all
+__all__ = generator_all + generator_malla + utils_all
```

### Comparing `spark_generated_rules_tools-0.1.3/spark_generated_rules_tools/functions/generator.py` & `spark_generated_rules_tools-0.2.0/spark_generated_rules_tools/functions/generator.py`

 * *Files 19% similar despite different names*

```diff
@@ -484,7 +484,115 @@
             target_path_name = f"/data/master/{namespace}/data/t_{namespace}_{table_name_extract}"
             dq_generated_dataframe_info(namespace=namespace,
                                         table_name=table_name,
                                         periodicity=periodicity,
                                         target_path_name=target_path_name,
                                         hamu_list=hamu_master_list,
                                         hamu_type=hamu_type)
+
+
+def dq_extract_parameters_file_malla(file_conf=None, uuaa=None):
+    import os
+    import sys
+    import re
+    import json
+    from spark_generated_rules_tools import get_color, get_color_b
+
+    is_windows = sys.platform.startswith('win')
+    dir_confs_name = os.getenv('pj_dq_dir_confs_name')
+    if file_conf in ("", None):
+        raise Exception(f'required variable url_conf')
+    if dir_confs_name is None:
+        raise Exception(f'required environment: pj_dq_dir_confs_name')
+
+    url_conf_name = str(str(file_conf).split(".")[0])
+    uuaa_name = str(uuaa).upper()
+    dir_confs_filename = os.path.join(dir_confs_name, uuaa_name, f"{url_conf_name}.txt")
+    dir_confs_env_parameters = os.path.join(dir_confs_name, uuaa_name, f"PARAMS_ENV.json")
+
+    if is_windows:
+        dir_confs_filename = dir_confs_filename.replace("\\", "/")
+        dir_confs_env_parameters = dir_confs_env_parameters.replace("\\", "/")
+    os.makedirs(os.path.dirname(dir_confs_filename), exist_ok=True)
+
+    with open(file_conf) as file:
+        hammurabi_conf = file.read()
+    with open(dir_confs_filename, 'w') as file:
+        file.write(hammurabi_conf)
+    with open(dir_confs_filename) as f:
+        hammurabi_conf = f.read()
+    variables_1 = sorted(list(set(re.findall(r'{([a-zA-Z_.-]+)}', hammurabi_conf))))
+    variables_2 = sorted(list(set(re.findall(r'{?([a-zA-Z_.-]+)}', hammurabi_conf))))
+    variables_list = list(set(variables_1 + variables_2))
+    variables_dict = {variables: "" for variables in variables_list if
+                      variables not in ("ARTIFACTORY_UNIQUE_CACHE", "SCHEMAS_REPOSITORY", "TEST_PATH")}
+    env_variables = {key: f"%%PARM{i + 1}" for i, key in enumerate(variables_dict)}
+    env_controlm = {"CONTROLM_JOB_ID": "%%JOBNAME", "CONTROLM_JOB_FLOW": "%%SCHEDTAB"}
+    env_dict = dict()
+    env_dict["env"] = dict()
+    env_dict["env"].update(env_variables)
+    env_dict["env"].update(env_controlm)
+    with open(f"{dir_confs_env_parameters}", "w") as f:
+        json.dump(env_dict, f)
+
+    with open(f"{dir_confs_env_parameters}") as f:
+        parameter_conf = f.read()
+
+    print(f"{get_color('ENV:')} {get_color_b(parameter_conf)}")
+
+
+def dq_extract_parameters_bitbucket_malla(url_conf=None):
+    import os
+    import sys
+    import re
+    import json
+    import requests
+    from spark_generated_rules_tools import get_color, get_color_b
+
+    is_windows = sys.platform.startswith('win')
+    dir_confs_name = os.getenv('pj_dq_dir_confs_name')
+    if url_conf in ("", None):
+        raise Exception(f'required variable url_conf')
+    if dir_confs_name is None:
+        raise Exception(f'required environment: pj_dq_dir_confs_name')
+
+    url = dq_convert_url_bitbucket_artifactory(url_conf=url_conf)
+    url_conf_extension = str(str(url).split("/")[-1]).replace("-", "_").upper().strip()
+    url_conf_name = str(str(url_conf_extension).split(".")[0])
+    uuaa_name = str(str(url).split("/")[-2]).upper()
+    if not len(uuaa_name) == 4:
+        uuaa_name = str(str(url).split("/")[-5]).upper()
+    dir_confs_filename = os.path.join(dir_confs_name, uuaa_name, f"{url_conf_name}.txt")
+    dir_confs_env_parameters = os.path.join(dir_confs_name, uuaa_name, f"PARAMS_ENV.json")
+
+    if is_windows:
+        dir_confs_filename = dir_confs_filename.replace("\\", "/")
+        dir_confs_env_parameters = dir_confs_env_parameters.replace("\\", "/")
+    os.makedirs(os.path.dirname(dir_confs_filename), exist_ok=True)
+
+    with requests.get(url, stream=True, verify=True) as r:
+        r.raise_for_status()
+        with open(dir_confs_filename, 'wb+') as f:
+            for chunk in r.iter_content(chunk_size=8192):
+                f.write(chunk)
+    with open(dir_confs_filename) as f:
+        hammurabi_conf = f.read()
+    variables_1 = sorted(list(set(re.findall(r'{([a-zA-Z_.-]+)}', hammurabi_conf))))
+    variables_2 = sorted(list(set(re.findall(r'{?([a-zA-Z_.-]+)}', hammurabi_conf))))
+    variables_list = list(set(variables_1 + variables_2))
+    variables_dict = {variables: "" for variables in variables_list if
+                      variables not in ("ARTIFACTORY_UNIQUE_CACHE", "SCHEMAS_REPOSITORY", "TEST_PATH")}
+
+    env_variables = {key: f"%%PARM{i + 1}" for i, key in enumerate(variables_dict)}
+    env_controlm = {"CONTROLM_JOB_ID": "%%JOBNAME", "CONTROLM_JOB_FLOW": "%%SCHEDTAB"}
+    env_dict = dict()
+    env_dict["env"] = dict()
+    env_dict["env"].update(env_variables)
+    env_dict["env"].update(env_controlm)
+
+    with open(f"{dir_confs_env_parameters}", "w") as f:
+        json.dump(env_dict, f)
+
+    with open(f"{dir_confs_env_parameters}") as f:
+        parameter_conf = f.read()
+
+    print(f"{get_color('ENV:')} {get_color_b(parameter_conf)}")
```

### Comparing `spark_generated_rules_tools-0.1.3/spark_generated_rules_tools/utils/resource/rules.json` & `spark_generated_rules_tools-0.2.0/spark_generated_rules_tools/utils/resource/rules.json`

 * *Files identical despite different names*

### Comparing `spark_generated_rules_tools-0.1.3/spark_generated_rules_tools.egg-info/PKG-INFO` & `spark_generated_rules_tools-0.2.0/spark_generated_rules_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-generated-rules-tools
-Version: 0.1.3
+Version: 0.2.0
 Summary: spark_generated_rules_tools
 Home-page: https://github.com/jonaqp/spark_generated_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_generated_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_generated_rules_tools-0.1.3/spark_generated_rules_tools.egg-info/SOURCES.txt` & `spark_generated_rules_tools-0.2.0/spark_generated_rules_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

