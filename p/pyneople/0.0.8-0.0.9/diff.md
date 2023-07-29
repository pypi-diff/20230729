# Comparing `tmp/pyneople-0.0.8.tar.gz` & `tmp/pyneople-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyneople-0.0.8.tar", last modified: Wed Jul 26 12:40:19 2023, max compression
+gzip compressed data, was "pyneople-0.0.9.tar", last modified: Sat Jul 29 05:51:04 2023, max compression
```

## Comparing `pyneople-0.0.8.tar` & `pyneople-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 12:40:19.417376 pyneople-0.0.8/
--rw-rw-rw-   0        0        0     1088 2023-07-21 05:43:07.000000 pyneople-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      579 2023-07-26 12:40:19.416376 pyneople-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       54 2023-07-21 05:43:07.000000 pyneople-0.0.8/README.md
--rw-rw-rw-   0        0        0      108 2023-07-21 05:43:07.000000 pyneople-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-26 12:40:19.417376 pyneople-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      833 2023-07-26 12:34:44.000000 pyneople-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 12:40:19.378378 pyneople-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-07-26 12:40:19.401377 pyneople-0.0.8/src/pyneople/
--rw-rw-rw-   0        0        0     2889 2023-07-24 04:27:44.000000 pyneople-0.0.8/src/pyneople/METADATA.py
--rw-rw-rw-   0        0        0      223 2023-07-24 04:51:23.000000 pyneople-0.0.8/src/pyneople/__init__.py
--rw-rw-rw-   0        0        0     1722 2023-07-21 05:43:07.000000 pyneople-0.0.8/src/pyneople/avatars.py
--rw-rw-rw-   0        0        0     3453 2023-07-26 12:30:17.000000 pyneople-0.0.8/src/pyneople/buff.py
--rw-rw-rw-   0        0        0     1403 2023-07-21 05:43:07.000000 pyneople-0.0.8/src/pyneople/character_search.py
--rw-rw-rw-   0        0        0     4643 2023-07-21 05:59:42.000000 pyneople-0.0.8/src/pyneople/equipments.py
--rw-rw-rw-   0        0        0     7209 2023-07-21 05:43:07.000000 pyneople-0.0.8/src/pyneople/functions.py
--rw-rw-rw-   0        0        0     3048 2023-07-21 05:43:07.000000 pyneople-0.0.8/src/pyneople/others.py
--rw-rw-rw-   0        0        0     2178 2023-07-26 12:39:55.000000 pyneople-0.0.8/src/pyneople/status.py
--rw-rw-rw-   0        0        0     3999 2023-07-21 05:43:07.000000 pyneople-0.0.8/src/pyneople/timeline.py
-drwxrwxrwx   0        0        0        0 2023-07-26 12:40:19.415376 pyneople-0.0.8/src/pyneople.egg-info/
--rw-rw-rw-   0        0        0      579 2023-07-26 12:40:19.000000 pyneople-0.0.8/src/pyneople.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2023-07-26 12:40:19.000000 pyneople-0.0.8/src/pyneople.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 12:40:19.000000 pyneople-0.0.8/src/pyneople.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-26 12:40:19.000000 pyneople-0.0.8/src/pyneople.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 05:51:04.647388 pyneople-0.0.9/
+-rw-rw-rw-   0        0        0     1088 2023-07-21 05:43:07.000000 pyneople-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      579 2023-07-29 05:51:04.647388 pyneople-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       54 2023-07-21 05:43:07.000000 pyneople-0.0.9/README.md
+-rw-rw-rw-   0        0        0      108 2023-07-21 05:43:07.000000 pyneople-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-29 05:51:04.648386 pyneople-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      833 2023-07-29 05:50:37.000000 pyneople-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 05:51:04.610244 pyneople-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-07-29 05:51:04.630268 pyneople-0.0.9/src/pyneople/
+-rw-rw-rw-   0        0        0     2889 2023-07-24 04:27:44.000000 pyneople-0.0.9/src/pyneople/METADATA.py
+-rw-rw-rw-   0        0        0      223 2023-07-24 04:51:23.000000 pyneople-0.0.9/src/pyneople/__init__.py
+-rw-rw-rw-   0        0        0     1722 2023-07-21 05:43:07.000000 pyneople-0.0.9/src/pyneople/avatars.py
+-rw-rw-rw-   0        0        0     3534 2023-07-29 05:31:01.000000 pyneople-0.0.9/src/pyneople/buff.py
+-rw-rw-rw-   0        0        0     1403 2023-07-21 05:43:07.000000 pyneople-0.0.9/src/pyneople/character_search.py
+-rw-rw-rw-   0        0        0     4711 2023-07-29 05:48:41.000000 pyneople-0.0.9/src/pyneople/equipments.py
+-rw-rw-rw-   0        0        0     7209 2023-07-21 05:43:07.000000 pyneople-0.0.9/src/pyneople/functions.py
+-rw-rw-rw-   0        0        0     3048 2023-07-21 05:43:07.000000 pyneople-0.0.9/src/pyneople/others.py
+-rw-rw-rw-   0        0        0     2178 2023-07-26 12:39:55.000000 pyneople-0.0.9/src/pyneople/status.py
+-rw-rw-rw-   0        0        0     3999 2023-07-21 05:43:07.000000 pyneople-0.0.9/src/pyneople/timeline.py
+drwxrwxrwx   0        0        0        0 2023-07-29 05:51:04.645386 pyneople-0.0.9/src/pyneople.egg-info/
+-rw-rw-rw-   0        0        0      579 2023-07-29 05:51:04.000000 pyneople-0.0.9/src/pyneople.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2023-07-29 05:51:04.000000 pyneople-0.0.9/src/pyneople.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 05:51:04.000000 pyneople-0.0.9/src/pyneople.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-29 05:51:04.000000 pyneople-0.0.9/src/pyneople.egg-info/top_level.txt
```

### Comparing `pyneople-0.0.8/LICENSE` & `pyneople-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.8/PKG-INFO` & `pyneople-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneople
-Version: 0.0.8
+Version: 0.0.9
 Summary: Neople Open API wrapper for data analyst
 Home-page: https://github.com/ippo252525/PyNeople
 Author: ippo252525
 Author-email: ippo252525@gmail.com
 Project-URL: Bug Tracker, https://github.com/ippo252525/PyNeople/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyneople-0.0.8/setup.py` & `pyneople-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyneople",
-    version="0.0.8",
+    version="0.0.9",
     author="ippo252525",
     author_email="ippo252525@gmail.com",
     description="Neople Open API wrapper for data analyst",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ippo252525/PyNeople",
     project_urls={
```

### Comparing `pyneople-0.0.8/src/pyneople/METADATA.py` & `pyneople-0.0.9/src/pyneople/METADATA.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.8/src/pyneople/avatars.py` & `pyneople-0.0.9/src/pyneople/avatars.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.8/src/pyneople/buff.py` & `pyneople-0.0.9/src/pyneople/buff.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,18 +45,21 @@
         self.buff_creature = None           
     
     def get_data(self, arg_server_id : str, arg_character_id : str):
         data = get_request(f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/skill/buff/equip/equipment?apikey={self.__api_key}")
         data = data['skill']['buff']
         
         if data:
-            for index, value in enumerate(data['skillInfo']['option']['values']):
-                data['skillInfo']['option']['desc'] = data['skillInfo']['option']['desc'].replace("{" + f"value{index + 1}" + "}", value)
-            self.buff_level = data['skillInfo']['option']['level']
-            self.buff_desc = data['skillInfo']['option']['desc']
+            try:
+                for index, value in enumerate(data['skillInfo']['option']['values']):
+                    data['skillInfo']['option']['desc'] = data['skillInfo']['option']['desc'].replace("{" + f"value{index + 1}" + "}", value)
+                self.buff_level = data['skillInfo']['option']['level']
+                self.buff_desc = data['skillInfo']['option']['desc']
+            except:
+                pass    
         if data:
             data = data['equipment']
         if data:
             for equipment in EQUIPMENT_LIST:
                 try:    
                     exec(f"self.buff_equipment_{equipment} = one_slot(data, '{equipment.upper()}')['itemName']")
                 except:
```

### Comparing `pyneople-0.0.8/src/pyneople/character_search.py` & `pyneople-0.0.9/src/pyneople/character_search.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.8/src/pyneople/equipments.py` & `pyneople-0.0.9/src/pyneople/equipments.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         self.exp_rate = None
         self.explain = None
     
     def get_option_info_data(self, arg_option_info_dict):
         try:
             self.level = arg_option_info_dict['level']
             self.exp_rate = arg_option_info_dict['expRate']
-            self.explain = arg_option_info_dict['explain']
+            self.explain = arg_option_info_dict['explain'].replace("'", "") # 얼음 땡 옵션 예외처리를 위한 replace
         except:
             pass    
 
 class GrowInfo():
     def __init__(self):
         self.total_level = None
         self.option_1 = OptionInfo()
```

### Comparing `pyneople-0.0.8/src/pyneople/functions.py` & `pyneople-0.0.9/src/pyneople/functions.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.8/src/pyneople/others.py` & `pyneople-0.0.9/src/pyneople/others.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.8/src/pyneople/status.py` & `pyneople-0.0.9/src/pyneople/status.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.8/src/pyneople/timeline.py` & `pyneople-0.0.9/src/pyneople/timeline.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.8/src/pyneople.egg-info/PKG-INFO` & `pyneople-0.0.9/src/pyneople.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneople
-Version: 0.0.8
+Version: 0.0.9
 Summary: Neople Open API wrapper for data analyst
 Home-page: https://github.com/ippo252525/PyNeople
 Author: ippo252525
 Author-email: ippo252525@gmail.com
 Project-URL: Bug Tracker, https://github.com/ippo252525/PyNeople/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

