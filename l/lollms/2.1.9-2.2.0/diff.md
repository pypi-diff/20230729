# Comparing `tmp/lollms-2.1.9.tar.gz` & `tmp/lollms-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lollms-2.1.9.tar", last modified: Thu Jun 29 22:22:46 2023, max compression
+gzip compressed data, was "lollms-2.2.0.tar", last modified: Sat Jul 29 00:02:05 2023, max compression
```

## Comparing `lollms-2.1.9.tar` & `lollms-2.2.0.tar`

### file list

```diff
@@ -1,31 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 22:22:46.756621 lollms-2.1.9/
--rw-rw-rw-   0        0        0    11558 2023-06-03 19:43:42.000000 lollms-2.1.9/LICENSE
--rw-rw-rw-   0        0        0      225 2023-06-29 21:31:56.000000 lollms-2.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0    11076 2023-06-29 22:22:46.756621 lollms-2.1.9/PKG-INFO
--rw-rw-rw-   0        0        0    10600 2023-06-18 10:10:09.000000 lollms-2.1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 22:22:46.727621 lollms-2.1.9/lollms/
--rw-rw-rw-   0        0        0      146 2023-06-21 07:49:26.000000 lollms-2.1.9/lollms/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 22:22:46.751620 lollms-2.1.9/lollms/assets/
--rw-rw-rw-   0        0        0   470378 2023-06-12 16:11:49.000000 lollms-2.1.9/lollms/assets/logo.png
--rw-rw-rw-   0        0        0     9914 2023-06-25 17:30:21.000000 lollms-2.1.9/lollms/binding.py
--rw-rw-rw-   0        0        0    21424 2023-06-22 15:34:05.000000 lollms-2.1.9/lollms/config.py
-drwxrwxrwx   0        0        0        0 2023-06-29 22:22:46.754619 lollms-2.1.9/lollms/configs/
--rw-rw-rw-   0        0        0      651 2023-06-25 11:51:47.000000 lollms-2.1.9/lollms/configs/config.yaml
--rw-rw-rw-   0        0        0    30470 2023-06-29 22:04:08.000000 lollms-2.1.9/lollms/console.py
--rw-rw-rw-   0        0        0     2613 2023-06-20 17:34:25.000000 lollms-2.1.9/lollms/helpers.py
--rw-rw-rw-   0        0        0     9348 2023-06-12 16:11:49.000000 lollms-2.1.9/lollms/langchain_integration.py
--rw-rw-rw-   0        0        0     7239 2023-06-29 21:40:56.000000 lollms-2.1.9/lollms/main_config.py
--rw-rw-rw-   0        0        0    13221 2023-06-29 21:59:06.000000 lollms-2.1.9/lollms/paths.py
--rw-rw-rw-   0        0        0    38528 2023-06-28 21:28:43.000000 lollms-2.1.9/lollms/personality.py
--rw-rw-rw-   0        0        0    32664 2023-06-29 22:21:42.000000 lollms-2.1.9/lollms/server.py
--rw-rw-rw-   0        0        0    11120 2023-06-29 22:05:02.000000 lollms-2.1.9/lollms/settings.py
--rw-rw-rw-   0        0        0     1127 2023-06-28 21:31:20.000000 lollms-2.1.9/lollms/types.py
-drwxrwxrwx   0        0        0        0 2023-06-29 22:22:46.750618 lollms-2.1.9/lollms.egg-info/
--rw-rw-rw-   0        0        0    11076 2023-06-29 22:22:46.000000 lollms-2.1.9/lollms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-06-29 22:22:46.000000 lollms-2.1.9/lollms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 22:22:46.000000 lollms-2.1.9/lollms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      129 2023-06-29 22:22:46.000000 lollms-2.1.9/lollms.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      184 2023-06-29 22:22:46.000000 lollms-2.1.9/lollms.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-29 22:22:46.000000 lollms-2.1.9/lollms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 22:22:46.756621 lollms-2.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1792 2023-06-29 22:22:34.000000 lollms-2.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 00:02:05.087629 lollms-2.2.0/
+-rw-rw-rw-   0        0        0    11558 2023-06-03 19:43:42.000000 lollms-2.2.0/LICENSE
+-rw-rw-rw-   0        0        0      269 2023-07-19 17:46:44.000000 lollms-2.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    11076 2023-07-29 00:02:05.086628 lollms-2.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10600 2023-06-18 10:10:09.000000 lollms-2.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 00:02:04.994111 lollms-2.2.0/lollms/
+-rw-rw-rw-   0        0        0      146 2023-06-21 07:49:26.000000 lollms-2.2.0/lollms/__init__.py
+-rw-rw-rw-   0        0        0     9007 2023-07-23 16:01:43.000000 lollms-2.2.0/lollms/app.py
+drwxrwxrwx   0        0        0        0 2023-07-29 00:02:05.019631 lollms-2.2.0/lollms/apps/
+-rw-rw-rw-   0        0        0        0 2023-07-19 16:50:10.000000 lollms-2.2.0/lollms/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 00:02:05.020629 lollms-2.2.0/lollms/apps/console/
+-rw-rw-rw-   0        0        0    14754 2023-07-27 19:45:11.000000 lollms-2.2.0/lollms/apps/console/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 00:02:05.021630 lollms-2.2.0/lollms/apps/playground/
+-rw-rw-rw-   0        0        0      398 2023-07-19 16:42:16.000000 lollms-2.2.0/lollms/apps/playground/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 00:02:05.072629 lollms-2.2.0/lollms/apps/playground/static/
+-rw-rw-rw-   0        0        0    11558 2023-07-19 16:42:16.000000 lollms-2.2.0/lollms/apps/playground/static/LICENSE
+-rw-rw-rw-   0        0        0     3900 2023-07-19 16:42:16.000000 lollms-2.2.0/lollms/apps/playground/static/README.md
+-rw-rw-rw-   0        0        0      566 2023-07-19 16:42:16.000000 lollms-2.2.0/lollms/apps/playground/static/index.html
+-rw-rw-rw-   0        0        0   470378 2023-07-19 16:42:16.000000 lollms-2.2.0/lollms/apps/playground/static/logo.png
+-rw-rw-rw-   0        0        0    16548 2023-07-19 16:42:16.000000 lollms-2.2.0/lollms/apps/playground/static/lollms_playground.html
+-rw-rw-rw-   0        0        0       62 2023-07-19 16:42:16.000000 lollms-2.2.0/lollms/apps/playground/static/package.json
+drwxrwxrwx   0        0        0        0 2023-07-29 00:02:05.073630 lollms-2.2.0/lollms/apps/server/
+-rw-rw-rw-   0        0        0    34728 2023-07-27 19:45:11.000000 lollms-2.2.0/lollms/apps/server/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 00:02:05.075628 lollms-2.2.0/lollms/apps/settings/
+-rw-rw-rw-   0        0        0     7681 2023-07-27 19:45:11.000000 lollms-2.2.0/lollms/apps/settings/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 00:02:05.076630 lollms-2.2.0/lollms/assets/
+-rw-rw-rw-   0        0        0   470378 2023-06-12 16:11:49.000000 lollms-2.2.0/lollms/assets/logo.png
+-rw-rw-rw-   0        0        0    10963 2023-07-27 19:45:11.000000 lollms-2.2.0/lollms/binding.py
+-rw-rw-rw-   0        0        0    21426 2023-07-02 17:51:25.000000 lollms-2.2.0/lollms/config.py
+drwxrwxrwx   0        0        0        0 2023-07-29 00:02:05.084629 lollms-2.2.0/lollms/configs/
+-rw-rw-rw-   0        0        0      881 2023-07-19 16:42:16.000000 lollms-2.2.0/lollms/configs/config.yaml
+-rw-rw-rw-   0        0        0     4418 2023-07-02 12:47:59.000000 lollms-2.2.0/lollms/data.py
+-rw-rw-rw-   0        0        0     1357 2023-07-03 19:35:14.000000 lollms-2.2.0/lollms/extension.py
+-rw-rw-rw-   0        0        0     3027 2023-07-16 00:19:49.000000 lollms-2.2.0/lollms/helpers.py
+-rw-rw-rw-   0        0        0     9348 2023-06-12 16:11:49.000000 lollms-2.2.0/lollms/langchain_integration.py
+-rw-rw-rw-   0        0        0     7239 2023-07-03 22:53:18.000000 lollms-2.2.0/lollms/main_config.py
+-rw-rw-rw-   0        0        0    13693 2023-07-20 17:32:43.000000 lollms-2.2.0/lollms/paths.py
+-rw-rw-rw-   0        0        0    49264 2023-07-29 00:01:26.000000 lollms-2.2.0/lollms/personality.py
+-rw-rw-rw-   0        0        0    21967 2023-07-19 17:04:35.000000 lollms-2.2.0/lollms/terminal.py
+-rw-rw-rw-   0        0        0     2539 2023-07-29 00:00:49.000000 lollms-2.2.0/lollms/types.py
+-rw-rw-rw-   0        0        0    25307 2023-07-28 21:19:50.000000 lollms-2.2.0/lollms/utilities.py
+drwxrwxrwx   0        0        0        0 2023-07-29 00:02:05.017630 lollms-2.2.0/lollms.egg-info/
+-rw-rw-rw-   0        0        0    11076 2023-07-29 00:02:04.000000 lollms-2.2.0/lollms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      947 2023-07-29 00:02:04.000000 lollms-2.2.0/lollms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 00:02:04.000000 lollms-2.2.0/lollms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      192 2023-07-29 00:02:04.000000 lollms-2.2.0/lollms.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      245 2023-07-29 00:02:04.000000 lollms-2.2.0/lollms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-29 00:02:04.000000 lollms-2.2.0/lollms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 00:02:05.087629 lollms-2.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1870 2023-07-29 00:01:36.000000 lollms-2.2.0/setup.py
```

### Comparing `lollms-2.1.9/LICENSE` & `lollms-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lollms-2.1.9/PKG-INFO` & `lollms-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms
-Version: 2.1.9
+Version: 2.2.0
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/lollms
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms-2.1.9/README.md` & `lollms-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `lollms-2.1.9/lollms/assets/logo.png` & `lollms-2.2.0/lollms/apps/playground/static/logo.png`

 * *Files identical despite different names*

### Comparing `lollms-2.1.9/lollms/binding.py` & `lollms-2.2.0/lollms/binding.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 import os
 import yaml
 from tqdm import tqdm
 import importlib
 import subprocess
 from lollms.config import TypedConfig, InstallOption
 from lollms.main_config import LOLLMSConfig
-
+import traceback
+import urllib
 
 __author__ = "parisneo"
 __github__ = "https://github.com/ParisNeo/lollms_bindings_zoo"
 __copyright__ = "Copyright 2023, "
 __license__ = "Apache 2.0"
 
 
@@ -59,15 +60,17 @@
             self.binding_config.config.save_config()
         else:
             self.load_binding_config()
 
         self.models_folder = config.lollms_paths.personal_models_path / self.binding_folder_name
         self.models_folder.mkdir(parents=True, exist_ok=True)
 
-
+    def __str__(self) -> str:
+        return self.config["binding_name"]+f"({self.config['model_name']})"
+    
     def download_and_install_wheel(self, url):
         # Create a temporary directory
         temp_dir = tempfile.mkdtemp()
 
         try:
             # Download the wheel file
             response = requests.get(url)
@@ -86,25 +89,43 @@
             else:
                 print('Failed to download the file.')
 
         except Exception as e:
             print('An error occurred during installation:', str(e))
             shutil.rmtree(temp_dir)
 
-
+    def get_file_size(self, url):
+        # Send a HEAD request to retrieve file metadata
+        response = urllib.request.urlopen(url)
+        
+        # Extract the Content-Length header value
+        file_size = response.headers.get('Content-Length')
+        
+        # Convert the file size to integer
+        if file_size:
+            file_size = int(file_size)
+        
+        return file_size
+    
     def build_model(self):
         """
         Build the model.
 
         This method is responsible for constructing the model for the LOLLMS class.
 
         Returns:
             the model
         """        
         return None
+    
+    def destroy_model(self):
+        """
+        destroys the current model
+        """
+        pass
 
     def install(self):
         """
         Installation procedure (to be implemented)
         """
         ASCIIColors.blue("*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*")
         ASCIIColors.red(f"Installing {self.binding_folder_name}")
@@ -121,19 +142,21 @@
         Returns:
             str: The path of the model.
         """
         if self.config.model_name is None:
             return None
         
         if self.config.model_name.endswith(".reference"):
+            ASCIIColors.yellow("Loading a reference model:")
             with open(str(self.lollms_paths.personal_models_path / f"{self.binding_folder_name}/{self.config.model_name}"), 'r') as f:
                 model_path = Path(f.read())
+            ASCIIColors.yellow(model_path)
         else:
             model_path = Path(self.lollms_paths.personal_models_path / f"{self.binding_folder_name}/{self.config.model_name}")
-        
+
         return model_path
 
     
     def get_current_seed(self):
         return self.seed
     
     def load_binding_config(self):
@@ -168,26 +191,26 @@
         """     
         self.binding_config.config.save_config(self.configuration_file_path)
 
     
 
 
     def generate(self, 
-                 prompt:str,                  
+                 prompt:str,
                  n_predict: int = 128,
-                 callback: Callable[[str], None] = None,
+                 callback: Callable[[str, int, dict], bool] = None,
                  verbose: bool = False,
                  **gpt_params ):
         """Generates text out of a prompt
         This should ber implemented by child class
 
         Args:
             prompt (str): The prompt to use for generation
             n_predict (int, optional): Number of tokens to prodict. Defaults to 128.
-            callback (Callable[[str], None], optional): A callback function that is called everytime a new text element is generated. Defaults to None.
+            callback (Callable[[str, int, dict], None], optional): A callback function that is called everytime a new text element is generated. Defaults to None.
             verbose (bool, optional): If true, the code will spit many informations about the generation process. Defaults to False.
         """
         pass
     def tokenize(self, prompt:str):
         """
         Tokenizes the given prompt using the model's tokenizer.
 
@@ -207,19 +230,30 @@
             tokens_list (list): A list of tokens to be detokenized.
 
         Returns:
             str: The detokenized text as a string.
         """
         return " ".join(tokens_list)
 
+
+    def embed(self, text):
+        """
+        Computes text embedding
+        Args:
+            text (str): The text to be embedded.
+        Returns:
+            List[float]
+        """
+        pass
+
     def list_models(self, config:dict):
         """Lists the models for this binding
         """
         models_dir = self.lollms_paths.personal_models_path/config["binding_name"]  # replace with the actual path to the models folder
-        return [f.name for f in models_dir.glob(self.file_extension)]
+        return [f.name for f in models_dir.iterdir() if f.suffix == self.file_extension.replace("*","") or f.suffix==".reference"]
 
     @staticmethod
     def reinstall_pytorch_with_cuda():
         result = subprocess.run(["pip", "install", "--upgrade", "torch", "torchvision", "torchaudio", "--no-cache-dir", "--index-url", "https://download.pytorch.org/whl/cu117"])
         if result.returncode != 0:
             ASCIIColors.warning("Couldn't find Cuda build tools on your PC. Reverting to CPU.")
             result = subprocess.run(["pip", "install", "--upgrade", "torch", "torchvision", "torchaudio", "--no-cache-dir"])
```

### Comparing `lollms-2.1.9/lollms/config.py` & `lollms-2.2.0/lollms/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,14 +239,15 @@
         self.file_path          = file_path
 
     @staticmethod
     def from_template(template:ConfigTemplate, exceptional_keys: list = [], file_path: Path | str = None):
         config = {}
         for entry in template.template:
             config[entry["name"]]=entry["value"]
+
         return BaseConfig(exceptional_keys, config, file_path)
 
     def to_dict(self):
         """
         Returns the configuration data as a dictionary.
 
         Returns:
```

### Comparing `lollms-2.1.9/lollms/langchain_integration.py` & `lollms-2.2.0/lollms/langchain_integration.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.9/lollms/main_config.py` & `lollms-2.2.0/lollms/main_config.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.9/lollms/paths.py` & `lollms-2.2.0/lollms/paths.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 from lollms.config import BaseConfig
 import subprocess
 
 lollms_path = Path(__file__).parent
 lollms_default_cfg_path = lollms_path / "configs/config.yaml"
 lollms_bindings_zoo_path = lollms_path / "bindings_zoo"
 lollms_personalities_zoo_path = lollms_path / "personalities_zoo"
+lollms_extensions_zoo_path = lollms_path / "extensions_zoo"
 
 
 personalities_zoo_repo = "https://github.com/ParisNeo/lollms_personalities_zoo.git"
 bindings_zoo_repo = "https://github.com/ParisNeo/lollms_bindings_zoo.git"
+extensions_zoo_repo = "https://github.com/ParisNeo/lollms_extensions_zoo.git"
 
 # Now we speify the personal folders
 class LollmsPaths:
     def __init__(self, global_paths_cfg_path=None, lollms_path=None, personal_path=None, custom_default_cfg_path=None, tool_prefix=""):
         self.global_paths_cfg_path  = global_paths_cfg_path
         self.tool_prefix            = tool_prefix
         if lollms_path is None:
@@ -33,68 +35,73 @@
             self.default_cfg_path   = lollms_path / "configs/config.yaml"
 
         self.personal_path                  = personal_path
         self.personal_configuration_path    = personal_path / "configs"
         self.personal_data_path             = personal_path / "data"
         self.personal_databases_path        = personal_path / "databases"
         self.personal_models_path           = personal_path / "models"
-        self.personal_uploads_path          = lollms_path / "uploads"
-        self.personal_log_path              = lollms_path / "logs"
+        self.personal_uploads_path          = personal_path / "uploads"
+        self.personal_log_path              = personal_path / "logs"
+        self.personal_outputs_path          = personal_path / "outputs"
+        self.personal_user_infos_path       = personal_path / "user_infos"
 
 
         self.bindings_zoo_path              = personal_path / "bindings_zoo"
         self.personalities_zoo_path         = personal_path / "personalities_zoo"
+        self.extensions_zoo_path            = personal_path / "extensions_zoo_path"
 
 
         self.create_directories()
         self.copy_default_config()
 
     def __str__(self) -> str:
         directories = {
             "Global paths configuration Path": self.global_paths_cfg_path,
             "Personal Configuration Path": self.personal_configuration_path,
             "Personal Data Path": self.personal_data_path,
             "Personal Databases Path": self.personal_databases_path,
             "Personal Models Path": self.personal_models_path,
             "Personal Uploads Path": self.personal_uploads_path,
             "Personal Log Path": self.personal_log_path,
+            "Personal outputs Path": self.personal_outputs_path,
             "Bindings Zoo Path": self.bindings_zoo_path,
-            "Personalities Zoo Path": self.personalities_zoo_path
+            "Personalities Zoo Path": self.personalities_zoo_path,
+            "Extensions zoo path": self.extensions_zoo_path,
+            "Personal user infos path": self.personal_user_infos_path
         }
         return "\n".join([f"{category}: {path}" for category, path in directories.items()])
 
     def change_personal_path(self, path):
         self.personal_path = path
 
     def create_directories(self):
         self.personal_path.mkdir(parents=True, exist_ok=True)
         self.personal_configuration_path.mkdir(parents=True, exist_ok=True)
         self.personal_models_path.mkdir(parents=True, exist_ok=True)
         self.personal_data_path.mkdir(parents=True, exist_ok=True)
         self.personal_databases_path.mkdir(parents=True, exist_ok=True)
         self.personal_log_path.mkdir(parents=True, exist_ok=True)
+        self.personal_outputs_path.mkdir(parents=True, exist_ok=True)
         self.personal_uploads_path.mkdir(parents=True, exist_ok=True)
+        self.personal_user_infos_path.mkdir(parents=True, exist_ok=True)
+        
+        if not self.bindings_zoo_path.exists():
+            # Clone the repository to the target path
+            ASCIIColors.info("No bindings found in your personal space.\nCloning the personalities zoo")
+            subprocess.run(["git", "clone", bindings_zoo_repo, self.bindings_zoo_path])
 
         if not self.personalities_zoo_path.exists():
             # Clone the repository to the target path
             ASCIIColors.info("No personalities found in your personal space.\nCloning the personalities zoo")
             subprocess.run(["git", "clone", personalities_zoo_repo, self.personalities_zoo_path])
-        else:
-            # Pull the repository if it already exists
-            ASCIIColors.info("Personalities zoo found in your personal space.\nPulling last personalities zoo")
-            subprocess.run(["git", "-C", self.personalities_zoo_path, "pull"])            
 
-        if not self.bindings_zoo_path.exists():
+        if not self.extensions_zoo_path.exists():
             # Clone the repository to the target path
-            ASCIIColors.info("No personalities found in your personal space.\nCloning the personalities zoo")
-            subprocess.run(["git", "clone", bindings_zoo_repo, self.bindings_zoo_path])
-        else:
-            # Pull the repository if it already exists
-            ASCIIColors.info("Personalities zoo found in your personal space.\nPulling last personalities zoo")
-            subprocess.run(["git", "-C", self.bindings_zoo_path, "pull"])            
+            ASCIIColors.info("No extensions found in your personal space.\nCloning the extensions zoo")
+            subprocess.run(["git", "clone", extensions_zoo_repo, self.extensions_zoo_path])
 
 
     def copy_default_config(self):
         local_config_path = self.personal_configuration_path / f"{self.tool_prefix}local_config.yaml"
         if not local_config_path.exists():
             shutil.copy(self.default_cfg_path, str(local_config_path))
 
@@ -148,15 +155,15 @@
                 cfg.load_config(global_paths_cfg_path)
                 lollms_path = cfg.lollms_path
                 lollms_personal_path = cfg.lollms_personal_path
                 return LollmsPaths(global_paths_cfg_path, lollms_path, lollms_personal_path, custom_default_cfg_path=custom_default_cfg_path, tool_prefix=tool_prefix)
             except Exception as ex:
                 print(f"{ASCIIColors.color_red}Global paths configuration file found but seems to be corrupted{ASCIIColors.color_reset}")
                 print("Couldn't find your personal data path!")
-                cfg.lollms_path = str(Path(__file__).parent)
+                cfg.lollms_path = lollms_path
                 cfg["lollms_personal_path"] = str(Path.home()/"Documents/lollms")
                 print("Please specify the folder where your configuration files, your models and your custom personalities need to be stored:")
                 lollms_personal_path = input(f"Folder path: ({cfg.lollms_personal_path}):")
                 if lollms_personal_path!="":
                     cfg.lollms_personal_path=lollms_personal_path
                 cfg.save_config(global_paths_cfg_path)
                 lollms_path = cfg.lollms_path
@@ -165,15 +172,15 @@
         else:
             # if the app is not forcing a specific path, then try to find out if the default installed library has specified a default path
             global_paths_cfg_path = Path.home()/f"{tool_prefix}global_paths_cfg.yaml"
             if global_paths_cfg_path.exists():
                 cfg = BaseConfig()
                 cfg.load_config(global_paths_cfg_path)
                 try:
-                    lollms_path = cfg.lollms_path
+                    # lollms_path = cfg.lollms_path
                     lollms_personal_path = cfg.lollms_personal_path
                     return LollmsPaths(global_paths_cfg_path, lollms_path, lollms_personal_path, custom_default_cfg_path=custom_default_cfg_path, tool_prefix=tool_prefix)
                 except Exception as ex:
                     print(f"{ASCIIColors.color_red}Global paths configuration file found but seems to be corrupted{ASCIIColors.color_reset}")
                     cfg.lollms_path = Path(__file__).parent
                     cfg.lollms_personal_path = input("Please specify the folder where your configuration files, your models and your custom personalities need to be stored:")
                     cfg.save_config(global_paths_cfg_path)
```

### Comparing `lollms-2.1.9/lollms/personality.py` & `lollms-2.2.0/lollms/personality.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 from datetime import datetime
 import importlib
 import shutil
 import subprocess
 import yaml
 from lollms.helpers import ASCIIColors
 from lollms.types import MSG_TYPE
-
+from typing import Callable
+import json
 
 
 def is_package_installed(package_name):
     try:
         dist = pkg_resources.get_distribution(package_name)
         return True
     except pkg_resources.DistributionNotFound:
@@ -40,42 +41,40 @@
         subprocess.check_call(["pip", "install", package_name])
         
         print(f"{package_name} has been successfully installed.")
 
 class AIPersonality:
 
     # Extra 
-    Conditionning_commands={
-        "date_time": datetime.now().strftime("%A, %B %d, %Y %I:%M:%S %p"), # Replaces {{date}} with actual date
-        "date": datetime.now().strftime("%A, %B %d, %Y"), # Replaces {{date}} with actual date
-        "time": datetime.now().strftime("%H:%M:%S"), # Replaces {{time}} with actual time
-    }
+
     
     def __init__(
                     self, 
                     personality_package_path: str|Path, 
                     lollms_paths:LollmsPaths, 
                     config:LOLLMSConfig,
                     model:LLMBinding=None, 
                     run_scripts=True, 
                     is_relative_path=True,
-                    installation_option:InstallOption=InstallOption.INSTALL_IF_NECESSARY
+                    installation_option:InstallOption=InstallOption.INSTALL_IF_NECESSARY,
+                    callback: Callable[[str, int, dict], bool]=None
                 ):
         """
         Initialize an AIPersonality instance.
 
         Parameters:
         personality_package_path (str or Path): The path to the folder containing the personality package.
 
         Raises:
         ValueError: If the provided path is not a folder or does not contain a config.yaml file.
         """
         self.lollms_paths = lollms_paths
         self.model = model
         self.config = config
+        self.callback = callback
 
         self.files = []
 
         self.installation_option = installation_option
 
         # First setup a default personality
         # Version
@@ -100,18 +99,18 @@
 It answers the questions with precise details
 Its performance depends on the underlying model size and training.
 Try to answer with as much details as you can
 Date: {{date}}
 """
         self._welcome_message: str = "Welcome! I am lollms (Lord of LLMs) A free and open assistant built by ParisNeo. What can I do for you today?"
         self._include_welcome_message_in_disucssion: bool = True
-        self._user_message_prefix: str = "## Human: "
+        self._user_message_prefix: str = "!@> Human: "
         self._link_text: str = "\n"
-        self._ai_message_prefix: str = "## lollms:"
-        self._anti_prompts:list = ["## Human","## lollms","##Human","##Assistant","##lollms"]
+        self._ai_message_prefix: str = "!@> lollms:"
+        self._anti_prompts:list = [self.config.discussion_prompt_separator]
 
         # Extra
         self._dependencies: List[str] = []
 
         # Disclaimer
         self._disclaimer: str = ""
         self._help: str = ""
@@ -176,20 +175,20 @@
             package_path = Path(package_path)
 
         # Verify that there is at least a configuration file
         config_file = package_path / "config.yaml"
         if not config_file.exists():
             raise ValueError(f"The provided folder {package_path} does not exist.")
 
-        with open(config_file, "r") as f:
+        with open(config_file, "r", encoding='utf-8') as f:
             config = yaml.safe_load(f)
 
         secret_file = package_path / "secret.yaml"
         if secret_file.exists():
-            with open(secret_file, "r") as f:
+            with open(secret_file, "r", encoding='utf-8') as f:
                 self._secret_cfg = yaml.safe_load(f)
         else:
             self._secret_cfg = None
 
 
         # Load parameters from the configuration file
         self._version = config.get("version", self._version)
@@ -202,15 +201,15 @@
         self._personality_conditioning = config.get("personality_conditioning", self._personality_conditioning)
         self._welcome_message = config.get("welcome_message", self._welcome_message)
         self._include_welcome_message_in_disucssion = config.get("include_welcome_message_in_disucssion", self._include_welcome_message_in_disucssion)
 
         self._user_message_prefix = config.get("user_message_prefix", self._user_message_prefix)
         self._link_text = config.get("link_text", self._link_text)
         self._ai_message_prefix = config.get("ai_message_prefix", self._ai_message_prefix)
-        self._anti_prompts = config.get("anti_prompts", self._anti_prompts)
+        self._anti_prompts = [self.config.discussion_prompt_separator]+config.get("anti_prompts", self._anti_prompts)
         self._dependencies = config.get("dependencies", self._dependencies)
         self._disclaimer = config.get("disclaimer", self._disclaimer)
         self._help = config.get("help", self._help)
         self._commands = config.get("commands", self._commands)
         self._model_temperature = config.get("model_temperature", self._model_temperature)
         self._model_n_predicts = config.get("model_n_predicts", self._model_n_predicts)
         self._model_top_k = config.get("model_top_k", self._model_top_k)
@@ -248,15 +247,15 @@
             self.processor_script_path = self.scripts_path / processor_file_name
             if self.processor_script_path.exists():
                 module_name = processor_file_name[:-3]  # Remove the ".py" extension
                 module_spec = importlib.util.spec_from_file_location(module_name, str(self.processor_script_path))
                 module = importlib.util.module_from_spec(module_spec)
                 module_spec.loader.exec_module(module)
                 if hasattr(module, "Processor"):
-                    self._processor = module.Processor(self)
+                    self._processor = module.Processor(self, callback=self.callback)
                 else:
                     self._processor = None
             else:
                 self._processor = None
         # Get a list of all files in the assets folder
         contents = [str(file) for file in self.assets_path.iterdir() if file.is_file()]
 
@@ -350,14 +349,22 @@
             "model_repeat_penalty": self._model_repeat_penalty,
             "model_repeat_last_n": self._model_repeat_last_n,
             "assets_list":self._assets_list
         }
 
     # ========================================== Properties ===========================================
     @property
+    def conditionning_commands(self):
+        return {
+            "date_time": datetime.now().strftime("%A, %B %d, %Y %I:%M:%S %p"), # Replaces {{date}} with actual date
+            "date": datetime.now().strftime("%A, %B %d, %Y"), # Replaces {{date}} with actual date
+            "time": datetime.now().strftime("%H:%M:%S"), # Replaces {{time}} with actual time
+        }
+
+    @property
     def logo(self):
         """
         Get the personality logo.
 
         Returns:
         PIL.Image.Image: The personality logo as a Pillow Image object.
         """
@@ -449,15 +456,15 @@
     def personality_conditioning(self) -> str:
         """
         Getter for the personality conditioning.
 
         Returns:
             str: The personality conditioning of the AI assistant.
         """
-        return self.replace_keys(self._personality_conditioning, self.Conditionning_commands)
+        return self.replace_keys(self._personality_conditioning, self.conditionning_commands)
 
     @personality_conditioning.setter
     def personality_conditioning(self, conditioning: str):
         """
         Setter for the personality conditioning.
 
         Args:
@@ -469,15 +476,15 @@
     def welcome_message(self) -> str:
         """
         Getter for the welcome message.
 
         Returns:
             str: The welcome message of the AI assistant.
         """
-        return self.replace_keys(self._welcome_message, self.Conditionning_commands)
+        return self.replace_keys(self._welcome_message, self.conditionning_commands)
 
     @welcome_message.setter
     def welcome_message(self, message: str):
         """
         Setter for the welcome message.
 
         Args:
@@ -832,36 +839,108 @@
             return replacements.get(key, match.group(0))
 
         output_string = re.sub(pattern, replace, input_string)
         return output_string
 
 
 
+class StateMachine:
+    def __init__(self, states_dict):
+        """
+        states structure is the following
+        [
+            {
+                "name": the state name,
+                "commands": [ # list of commands
+                    "command": function
+                ],
+                "default": default function
+            }
+        ]
+        """
+        self.states_dict = states_dict
+        self.current_state_id = 0
+        self.callback = None
+    
+    def goto_state(self, state):
+        """
+        Transition to the state with the given name or index.
+
+        Args:
+            state (str or int): The name or index of the state to transition to.
+
+        Raises:
+            ValueError: If no state is found with the given name or index.
+        """
+        if isinstance(state, str):
+            for i, state_dict in enumerate(self.states_dict):
+                if state_dict["name"] == state:
+                    self.current_state_id = i
+                    return
+        elif isinstance(state, int):
+            if 0 <= state < len(self.states_dict):
+                self.current_state_id = state
+                return
+        raise ValueError(f"No state found with name or index: {state}")
+
+
+
+    def process_state(self, command, full_context, callback: Callable[[str, int, dict], bool]=None):
+        """
+        Process the given command based on the current state.
+
+        Args:
+            command: The command to process.
+
+        Raises:
+            ValueError: If the current state doesn't have the command and no default function is defined.
+        """
+        if callback:
+            self.callback=callback
+            
+        current_state = self.states_dict[self.current_state_id]
+        commands = current_state["commands"]
+        command = command.strip()
+        
+        for cmd, func in commands.items():
+            if cmd == command[0:len(cmd)]:
+                func(command, full_context)
+                return
+        
+        default_func = current_state.get("default")
+        if default_func is not None:
+            default_func(command, full_context)
+        else:
+            raise ValueError(f"Command '{command}' not found in current state and no default function defined.")
 
+        
 
-class APScript:
+class APScript(StateMachine):
     """
     Template class for implementing personality processor classes in the APScript framework.
 
     This class provides a basic structure and placeholder methods for processing model inputs and outputs.
     Personality-specific processor classes should inherit from this class and override the necessary methods.
     """
     def __init__(
                     self, 
                     personality         :AIPersonality,
-                    personality_config  :TypedConfig
+                    personality_config  :TypedConfig,
+                    states_dict         :dict   = {},
+                    callback            = None
                 ) -> None:
-        
+        super().__init__(states_dict)
         self.files=[]
         self.personality                        = personality
         self.personality_config                 = personality_config
         self.installation_option                = personality.installation_option
         self.configuration_file_path            = self.personality.lollms_paths.personal_configuration_path/f"personality_{self.personality.personality_folder_name}.yaml"
         self.personality_config.config.file_path    = self.configuration_file_path
 
+        self.callback = callback
         # Installation
         if (not self.configuration_file_path.exists() or self.installation_option==InstallOption.FORCE_INSTALL) and self.installation_option!=InstallOption.NEVER_INSTALL:
             self.install()
             self.personality_config.config.save_config()
         else:
             self.load_personality_config()
 
@@ -901,14 +980,25 @@
         Installation procedure (to be implemented)
         """
         ASCIIColors.blue("*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*")
         ASCIIColors.red(f"Uninstalling {self.personality.personality_folder_name}")
         ASCIIColors.blue("*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*")
 
 
+    @staticmethod
+    def reinstall_pytorch_with_cuda():
+        result = subprocess.run(["pip", "install", "--upgrade", "torch", "torchvision", "torchaudio", "--no-cache-dir", "--index-url", "https://download.pytorch.org/whl/cu117"])
+        if result.returncode != 0:
+            ASCIIColors.warning("Couldn't find Cuda build tools on your PC. Reverting to CPU.")
+            result = subprocess.run(["pip", "install", "--upgrade", "torch", "torchvision", "torchaudio", "--no-cache-dir"])
+            if result.returncode != 0:
+                ASCIIColors.error("Couldn't install pytorch !!")
+            else:
+                ASCIIColors.error("Pytorch installed successfully!!")
+
     def add_file(self, path):
         self.files.append(path)
         return True
 
     def remove_file(self, path):
         self.files.remove(path)
 
@@ -978,34 +1068,51 @@
         return string
     
     def process(self, text:str, message_type:MSG_TYPE):
         bot_says = self.bot_says + text
         antiprompt = self.personality.detect_antiprompt(bot_says)
         if antiprompt:
             self.bot_says = self.remove_text_from_string(bot_says,antiprompt)
-            ASCIIColors.warning("Detected hallucination")
+            ASCIIColors.warning(f"\nDetected hallucination with antiprompt: {antiprompt}")
             return False
         else:
             self.bot_says = bot_says
             return True
 
     def generate(self, prompt, max_size, temperature = None, top_k = None, top_p=None, repeat_penalty=None ):
         self.bot_says = ""
         ASCIIColors.info("Text generation started: Warming up")
-        return self.personality.model.generate(
+        self.personality.model.generate(
                                 prompt, 
                                 max_size, 
                                 self.process,
                                 temperature=self.personality.model_temperature if temperature is None else temperature,
                                 top_k=self.personality.model_top_k if top_k is None else top_k,
                                 top_p=self.personality.model_top_p if top_p is None else top_p,
                                 repeat_penalty=self.personality.model_repeat_penalty if repeat_penalty is None else repeat_penalty,
                                 ).strip()    
+        return self.bot_says
+
+
+    def execute_command(self, command:dict):
+        """Executes a command
+
+        Args:
+            command (dict): command information in form:
+            name: (command name)
+            value: (command value)
+            params: (command parameters)
+        """
+
+        if command["value"] in self.states_dict[self.current_state_id]["commands"]:
+            return self.states_dict[self.current_state_id]["commands"][command["value"]](command)
+        else:
+            return False
 
-    def run_workflow(self, prompt:str, previous_discussion_text:str="", callback=None):
+    def run_workflow(self, prompt:str, previous_discussion_text:str="", callback: Callable[[str, int, dict], bool]=None):
         """
         Runs the workflow for processing the model input and output.
 
         This method should be called to execute the processing workflow.
 
         Args:
             generate_fn (function): A function that generates model output based on the input prompt.
@@ -1014,48 +1121,192 @@
             previous_discussion_text (str, optional): The text of the previous discussion. Default is an empty string.
 
         Returns:
             None
         """
         return None
 
-    def process_model_input(self, text:str):
+    def step_start(self, step_text, callback: Callable[[str, int, dict], bool]=None):
+        """This triggers a step start
+
+        Args:
+            step_text (str): The step text
+            callback (callable, optional): A callable with this signature (str, MSG_TYPE) to send the step start to. Defaults to None.
         """
-        Process the model input.
+        if callback:
+            callback(step_text, MSG_TYPE.MSG_TYPE_STEP_START)
 
-        This method should be overridden in the personality-specific processor class to define
-        the desired behavior for processing the model input.
+    def step_end(self, step_text, status=True, callback: Callable[[str, int, dict], bool]=None):
+        """This triggers a step end
 
         Args:
-            text (str): The model input text.
+            step_text (str): The step text
+            callback (callable, optional): A callable with this signature (str, MSG_TYPE) to send the step end to. Defaults to None.
+        """
+        if callback:
+            callback(step_text, MSG_TYPE.MSG_TYPE_STEP_END, {'status':status})
 
-        Returns:
-            Any: The processed model input.
+    def step(self, step_text, callback: Callable[[str, int, dict], bool]=None):
+        """This triggers a step information
+
+        Args:
+            step_text (str): The step text
+            callback (callable, optional): A callable with this signature (str, MSG_TYPE) to send the step to. Defaults to None.
         """
-        return None
+        if callback:
+            callback(step_text, MSG_TYPE.MSG_TYPE_STEP)
 
-    def process_model_output(self, text:str):
+    def exception(self, ex, callback: Callable[[str, int, dict], bool]=None):
+        """This sends exception to the client
+
+        Args:
+            step_text (str): The step text
+            callback (callable, optional): A callable with this signature (str, MSG_TYPE) to send the step to. Defaults to None.
         """
-        Process the model output.
+        if callback:
+            callback(str(ex), MSG_TYPE.MSG_TYPE_EXCEPTION)
 
-        This method should be overridden in the personality-specific processor class to define
-        the desired behavior for processing the model output.
+    def warning(self, warning:str, callback: Callable[[str, int, dict], bool]=None):
+        """This sends exception to the client
 
         Args:
-            text (str): The model output text.
+            step_text (str): The step text
+            callback (callable, optional): A callable with this signature (str, MSG_TYPE) to send the step to. Defaults to None.
+        """
+        if callback:
+            callback(warning, MSG_TYPE.MSG_TYPE_EXCEPTION)
 
-        Returns:
-            Any: The processed model output.
+    def info(self, info:str, callback: Callable[[str, int, dict], bool]=None):
+        """This sends exception to the client
+
+        Args:
+            inf (str): The information to be sent
+            callback (callable, optional): A callable with this signature (str, MSG_TYPE) to send the step to. Defaults to None.
         """
-        return None
+        if callback:
+            callback(info, MSG_TYPE.MSG_TYPE_INFO)
+
+    def json(self, json_infos:dict, callback: Callable[[str, int, dict], bool]=None):
+        """This sends json data to front end
+
+        Args:
+            step_text (dict): The step text
+            callback (callable, optional): A callable with this signature (str, MSG_TYPE) to send the step to. Defaults to None.
+        """
+        if callback:
+            callback(json.dumps(json_infos), MSG_TYPE.MSG_TYPE_JSON_INFOS)
+
+    def ui(self, html_ui:str, callback: Callable[[str, int, dict], bool]=None):
+        """This sends ui elements to front end
+
+        Args:
+            step_text (dict): The step text
+            callback (callable, optional): A callable with this signature (str, MSG_TYPE) to send the step to. Defaults to None.
+        """
+        if callback:
+            callback(html_ui, MSG_TYPE.MSG_TYPE_UI)
+
+    def code(self, code:str, callback: Callable[[str, int, dict], bool]=None):
+        """This sends code to front end
+
+        Args:
+            step_text (dict): The step text
+            callback (callable, optional): A callable with this signature (str, MSG_TYPE) to send the step to. Defaults to None.
+        """
+        if callback:
+            callback(code, MSG_TYPE.MSG_TYPE_CODE)
+
+    def full(self, full_text:str, callback: Callable[[str, int, dict], bool]=None):
+        """This sends full text to front end
+
+        Args:
+            step_text (dict): The step text
+            callback (callable, optional): A callable with this signature (str, MSG_TYPE) to send the text to. Defaults to None.
+        """
+        if not callback and self.callback:
+            callback = self.callback
+
+        if callback:
+            callback(full_text, MSG_TYPE.MSG_TYPE_FULL)
 
+    def full_invisible_to_ai(self, full_text:str, callback: Callable[[str, int, dict], bool]=None):
+        """This sends full text to front end (INVISIBLE to AI)
 
+        Args:
+            step_text (dict): The step text
+            callback (callable, optional): A callable with this signature (str, MSG_TYPE) to send the text to. Defaults to None.
+        """
+        if not callback and self.callback:
+            callback = self.callback
+
+        if callback:
+            callback(full_text, MSG_TYPE.MSG_TYPE_FULL_INVISIBLE_TO_AI)
+
+    def full_invisible_to_user(self, full_text:str, callback: Callable[[str, int, dict], bool]=None):
+        """This sends full text to front end (INVISIBLE to user)
+
+        Args:
+            step_text (dict): The step text
+            callback (callable, optional): A callable with this signature (str, MSG_TYPE) to send the text to. Defaults to None.
+        """
+        if not callback and self.callback:
+            callback = self.callback
+
+        if callback:
+            callback(full_text, MSG_TYPE.MSG_TYPE_FULL_INVISIBLE_TO_USER)
+
+
+    def info(self, info_text:str, callback: Callable[[str, int, dict], bool]=None):
+        """This sends info text to front end
+
+        Args:
+            step_text (dict): The step text
+            callback (callable, optional): A callable with this signature (str, MSG_TYPE) to send the info to. Defaults to None.
+        """
+        if not callback and self.callback:
+            callback = self.callback
+
+        if callback:
+            callback(info_text, MSG_TYPE.MSG_TYPE_FULL)
+
+    def step_progress(self, step_text:str, progress:float, callback: Callable[[str, int, dict], bool]=None):
+        """This sends step rogress to front end
+
+        Args:
+            step_text (dict): The step progress in %
+            callback (callable, optional): A callable with this signature (str, MSG_TYPE) to send the progress to. Defaults to None.
+        """
+        if not callback and self.callback:
+            callback = self.callback
 
+        if callback:
+            callback(step_text, MSG_TYPE.MSG_TYPE_STEP_PROGRESS, {'progress':progress})
 
+    def new_message(self, step_text:str, message_type:MSG_TYPE, callback: Callable[[str, int, dict], bool]=None):
+        """This sends step rogress to front end
 
+        Args:
+            step_text (dict): The step progress in %
+            callback (callable, optional): A callable with this signature (str, MSG_TYPE) to send the progress to. Defaults to None.
+        """
+        if not callback and self.callback:
+            callback = self.callback
+
+        if callback:
+            callback(step_text, MSG_TYPE.MSG_TYPE_NEW_MESSAGE, {'type':message_type})
+
+    #Helper method to convert outputs path to url
+    def path2url(file):
+        file = str(file).replace("\\","/")
+        pth = file.split('/')
+        idx = pth.index("outputs")
+        pth = "/".join(pth[idx:])
+        file_path = f"![](/{pth})\n"
+        return file_path
+            
 # ===========================================================
 class AIPersonalityInstaller:
     def __init__(self, personality:AIPersonality) -> None:
         self.personality = personality
 
 
 class PersonalityBuilder:
@@ -1068,29 +1319,35 @@
                 ):
         self.config = config
         self.lollms_paths = lollms_paths
         self.model = model
         self.installation_option = installation_option
 
 
-    def build_personality(self):
-        if self.config["active_personality_id"]>=len(self.config["personalities"]):
-            ASCIIColors.warning("Personality ID was out of range. Resetting to 0.")
-            self.config["active_personality_id"]=0
-        if len(self.config["personalities"][self.config["active_personality_id"]].split("/"))==3:
+    def build_personality(self, id:int=None):
+        if id is None:
+            id = self.config["active_personality_id"]
+            if self.config["active_personality_id"]>=len(self.config["personalities"]):
+                ASCIIColors.warning("Personality ID was out of range. Resetting to 0.")
+                self.config["active_personality_id"]=0
+                id = 0
+        else:
+            if id>len(self.config["personalities"]):
+                id = len(self.config["personalities"])-1
+        if len(self.config["personalities"][id].split("/"))==3:
             self.personality = AIPersonality(
-                                            self.lollms_paths.personalities_zoo_path / self.config["personalities"][self.config["active_personality_id"]],
+                                            self.lollms_paths.personalities_zoo_path / self.config["personalities"][id],
                                             self.lollms_paths,
                                             self.config,
                                             self.model, 
                                             installation_option=self.installation_option
                                         )
         else:
             self.personality = AIPersonality(
-                                            self.config["personalities"][self.config["active_personality_id"]],
+                                            self.config["personalities"][id],
                                             self.lollms_paths,
                                             self.config,
                                             self.model,
                                             is_relative_path=False,
                                             installation_option=self.installation_option
                                         )
         return self.personality
```

### Comparing `lollms-2.1.9/lollms/server.py` & `lollms-2.2.0/lollms/apps/server/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,133 +4,86 @@
 from flask_cors import CORS
 from lollms.types import MSG_TYPE
 from lollms.personality import AIPersonality
 from lollms.main_config import LOLLMSConfig
 from lollms.binding import LLMBinding, BindingBuilder, ModelBuilder
 from lollms.personality import PersonalityBuilder
 from lollms.helpers import ASCIIColors
-from lollms.console import MainMenu
+from lollms.apps.console import MainMenu
 from lollms.paths import LollmsPaths
-from lollms.console import MainMenu
+from lollms.apps.console import MainMenu
+from lollms.app import LollmsApplication
+from lollms.utilities import TextVectorizer
 from typing import List, Tuple
 import importlib
 from pathlib import Path
 import argparse
 import logging
 import yaml
 import copy
-
+import gc
+import json
 def reset_all_installs(lollms_paths:LollmsPaths):
     ASCIIColors.info("Removeing all configuration files to force reinstall")
     ASCIIColors.info(f"Searching files from {lollms_paths.personal_configuration_path}")
     for file_path in lollms_paths.personal_configuration_path.iterdir():
         if file_path.name!=f"{lollms_paths.tool_prefix}local_config.yaml" and file_path.suffix.lower()==".yaml":
             file_path.unlink()
             ASCIIColors.info(f"Deleted file: {file_path}")
 
 
-class LoLLMsServer:
+class LoLLMsServer(LollmsApplication):
     def __init__(self):
+        
+
         host = "localhost"
         port = "9601"
         self.clients = {}
         self.current_binding = None
-        self.active_model = None
+        self.model = None
         self.personalities = []
         self.answer = ['']
         self.is_ready = True
         
         
-        self.lollms_paths = LollmsPaths.find_paths(force_local=False, tool_prefix="lollms_server_")
-        self.menu = MainMenu(self)
         parser = argparse.ArgumentParser()
         parser.add_argument('--host', '-hst', default=host, help='Host name')
         parser.add_argument('--port', '-prt', default=port, help='Port number')
 
-        parser.add_argument('--config', '-cfg', default=None, help='Path to the configuration file')
-        parser.add_argument('--bindings_path', '-bp', default=str(self.lollms_paths.bindings_zoo_path),
-                            help='The path to the Bindings folder')
-        parser.add_argument('--personalities_path', '-pp',
-                            default=str(self.lollms_paths.personalities_zoo_path),
-                            help='The path to the personalities folder')
-        parser.add_argument('--models_path', '-mp', default=str(self.lollms_paths.personal_models_path),
-                            help='The path to the models folder')
-
-        parser.add_argument('--binding_name', '-b', default=None,
-                            help='Binding to be used by default')
-        parser.add_argument('--model_name', '-m', default=None,
-                            help='Model name')
-        parser.add_argument('--personality_full_name', '-p', default="personality",
-                            help='Personality path relative to the personalities folder (language/category/name)')
         
         parser.add_argument('--reset_personal_path', action='store_true', help='Reset the personal path')
         parser.add_argument('--reset_config', action='store_true', help='Reset the configurations')
         parser.add_argument('--reset_installs', action='store_true', help='Reset all installation status')
 
 
         args = parser.parse_args()
 
         if args.reset_installs:
-            reset_all_installs()
+            self.reset_all_installs()
 
         if args.reset_personal_path:
             LollmsPaths.reset_configs()
 
         if args.reset_config:
             lollms_paths = LollmsPaths.find_paths(tool_prefix="lollms_server_")
             cfg_path = lollms_paths.personal_configuration_path / f"{lollms_paths.tool_prefix}local_config.yaml"
             try:
                 cfg_path.unlink()
                 ASCIIColors.success("LOLLMS configuration reset successfully")
             except:
                 ASCIIColors.success("Couldn't reset LOLLMS configuration")
+        else:
+            lollms_paths = LollmsPaths.find_paths(force_local=False, tool_prefix="lollms_server_")
 
         # Configuration loading part
-        self.config = LOLLMSConfig.autoload(self.lollms_paths, args.config)
-
-
-        if args.binding_name:
-            self.config.binding_name = args.binding_name
+        config = LOLLMSConfig.autoload(lollms_paths, None)
 
-        if args.model_name:
-            self.config.model_name = args.model_name
-
-        # Recover bindings path
-        self.personalities_path = Path(args.personalities_path)
-        self.bindings_path = Path(args.bindings_path)
-        self.models_path = Path(args.models_path)
-        if self.config.binding_name is None:
-            self.menu.select_binding()
-        else:
-            self.binding = BindingBuilder().build_binding(self.config, self.lollms_paths)
-        if self.config.model_name is None:
-            self.menu.select_model()
-        else:
-            try:
-                self.active_model = self.binding.build_model()
-            except Exception as ex:
-                print(f"{ASCIIColors.color_red}Couldn't load model Please select a valid model{ASCIIColors.color_reset}")
-                print(f"{ASCIIColors.color_red}{ex}{ASCIIColors.color_reset}")
-                self.menu.select_model()
-
-        for p in self.config.personalities:
-            personality = AIPersonality(
-                                            self.config.lollms_paths.personalities_zoo_path/p,
-                                            self.lollms_paths,
-                                            self.config,
-                                            self.active_model
-                                        )
-            self.personalities.append(personality)
-
-        if self.config.active_personality_id>len(self.personalities):
-            self.config.active_personality_id = 0
-        self.active_personality = self.personalities[self.config.active_personality_id]
+        super().__init__("lollms-server", config, lollms_paths)
 
         self.menu.show_logo()        
-        
         self.app = Flask("LoLLMsServer")
         #self.app.config['SECRET_KEY'] = 'lollmssecret'
         CORS(self.app)  # Enable CORS for all routes
         
         self.socketio = SocketIO(self.app, cors_allowed_origins='*', ping_timeout=1200, ping_interval=4000)
 
         # Set log level to warning
@@ -140,53 +93,14 @@
         self.socketio_log.setLevel(logging.WARNING)
         self.socketio_log.addHandler(logging.StreamHandler())
 
         self.initialize_routes()
         self.run(args.host, args.port)
 
 
-    def load_binding(self):
-        if self.config.binding_name is None:
-            print(f"No bounding selected")
-            print("Please select a valid model or install a new one from a url")
-            self.menu.select_binding()
-            # cfg.download_model(url)
-        else:
-            try:
-                self.binding = BindingBuilder().build_binding(self.config, self.lollms_paths)
-            except Exception as ex:
-                print(ex)
-                print(f"Couldn't find binding. Please verify your configuration file at {self.config.file_path} or use the next menu to select a valid binding")
-                print(f"Trying to reinstall binding")
-                self.binding = BindingBuilder().build_binding(self.config, self.lollms_paths, InstallOption.FORCE_INSTALL)
-                self.menu.select_binding()
-
-    def load_model(self):
-        try:
-            self.active_model = ModelBuilder(self.binding).get_model()
-            ASCIIColors.success("Model loaded successfully")
-        except Exception as ex:
-            ASCIIColors.error(f"Couldn't load model.")
-            ASCIIColors.error(f"Binding returned this exception : {ex}")
-            ASCIIColors.error(f"{self.config.get_model_path_infos()}")
-            print("Please select a valid model or install a new one from a url")
-            self.menu.select_model()
-
-    def load_personality(self):
-        try:
-            self.personality = PersonalityBuilder(self.lollms_paths, self.config, self.model).build_personality()
-        except Exception as ex:
-            ASCIIColors.error(f"Couldn't load personality.")
-            ASCIIColors.error(f"Binding returned this exception : {ex}")
-            ASCIIColors.error(f"{self.config.get_personality_path_infos()}")
-            print("Please select a valid model or install a new one from a url")
-            self.menu.select_model()
-        self.cond_tk = self.personality.model.tokenize(self.personality.personality_conditioning)
-        self.n_cond_tk = len(self.cond_tk)
-
     def initialize_routes(self):
         @self.socketio.on('connect')
         def handle_connect():
             client_id = request.sid
             self.clients[client_id] = {
                     "namespace": request.namespace,
                     "full_discussion_blocks": [],
@@ -349,55 +263,161 @@
                 emit('list_available_personalities_names_list', {'success': False, 'error':str(ex)})
 
         @self.socketio.on('select_binding')
         def handle_select_binding(data):
             self.cp_config = copy.deepcopy(self.config)
             self.cp_config["binding_name"] = data['binding_name']
             try:
+                del self.model
+                del self.binding
+                self.model = None
+                self.binding = None
+                gc.collect()
+                for personality in self.mount_personalities:
+                    personality.model = None
                 self.binding = self.build_binding(self.bindings_path, self.cp_config)
                 self.config = self.cp_config
+                self.mount_personalities()
+                gc.collect()                
                 emit('select_binding', {'success':True, 'binding_name': self.cp_config["binding_name"]}, room=request.sid)
             except Exception as ex:
                 print(ex)
                 emit('select_binding', {'success':False, 'binding_name': self.cp_config["binding_name"], 'error':f"Couldn't load binding:\n{ex}"}, room=request.sid)
 
         @self.socketio.on('select_model')
         def handle_select_model(data):
             model_name = data['model_name']
             if self.binding is None:
                 emit('select_model', {'success':False, 'model_name':  model_name, 'error':f"Please select a binding first"}, room=request.sid)
                 return
             self.cp_config = copy.deepcopy(self.config)
             self.cp_config["model_name"] = data['model_name']
             try:
-                self.active_model = self.binding.build_model()
+                del self.model
+                self.model = None
+                gc.collect()
+                for personality in self.mount_personalities:
+                    personality.model = None
+                self.model = self.binding.build_model()
+                self.mount_personalities()
+                gc.collect()
                 emit('select_model', {'success':True, 'model_name':  model_name}, room=request.sid)
             except Exception as ex:
                 print(ex)
                 emit('select_model', {'success':False, 'model_name':  model_name, 'error':f"Please select a binding first"}, room=request.sid)
 
         @self.socketio.on('add_personality')
         def handle_add_personality(data):
             personality_path = data['path']
             try:
                 personality = AIPersonality(
                                                 personality_path, 
                                                 self.lollms_paths, 
                                                 self.config,
-                                                self.active_model
+                                                self.model
                                             )
                 self.personalities.append(personality)
                 self.config["personalities"].append(personality_path)
                 emit('personality_added', {'success':True, 'name': personality.name, 'id':len(self.personalities)-1}, room=request.sid)
                 self.config.save_config()
             except Exception as e:
                 error_message = str(e)
                 emit('personality_add_failed', {'success':False, 'error': error_message}, room=request.sid)
 
 
+        
+        @self.socketio.on('vectorize_text')
+        def vectorize_text(parameters:dict):
+            """Vectorizes text
+
+            Args:
+                parameters (dict): contains
+                'chunk_size': the maximum size of a text chunk (512 by default)
+                'vectorization_method': can be either "model_embedding" or "ftidf_vectorizer" (default is "ftidf_vectorizer")
+                'payloads': a list of dicts. each entry has the following format
+                {
+                    "path": the path to the document
+                    "text": the text of the document
+                },
+                'return_database': If true the vectorized database will be sent to the client (default is True)
+                'database_path': the path to store the database (default is none)
+                
+            returns a dict
+                status: True if success and false if not
+                if you asked for the database to be sent back you will ahve those fields too:
+                embeddings: a dictionary containing the text chunks with their ids and embeddings
+                "texts": a dictionary of text chunks for each embedding (use index for correspondance)
+                "infos": extra information
+                "vectorizer": The vectorize if this is using tfidf or none if it uses model
+                
+            """
+            vectorization_method = parameters.get('vectorization_method',"ftidf_vectorizer")
+            chunk_size = parameters.get("chunk_size",512)
+            payloads = parameters["payloads"]
+            database_path = parameters.get("database_path",None)
+            return_database = parameters.get("return_database",True)
+            if database_path is None and return_database is None:
+                ASCIIColors.warning("Vectorization should either ask to save the database or to recover it. You didn't ask for any one!")
+                emit('vectorized_db',{"status":False, "error":"Vectorization should either ask to save the database or to recover it. You didn't ask for any one!"}) 
+                return
+            tv = TextVectorizer(vectorization_method, self.model)
+            for payload in payloads:
+                tv.add_document(payload["path"],payload["text"],chunk_size=chunk_size)
+            json_db = tv.toJson()
+            if return_database:
+                emit('vectorized_db',{**{"status":True}, **json_db}) 
+            else:
+                emit('vectorized_db',{"status":True}) 
+                with open(database_path, "w") as file:
+                    json.dump(json_db, file, indent=4)
+                
+            
+        @self.socketio.on('query_database')
+        def query_database(parameters:dict):
+            """queries a database
+
+            Args:
+                parameters (dict): contains
+                'vectorization_method': can be either "model_embedding" or "ftidf_vectorizer"
+                'database': a list of dicts. each entry has the following format
+                {
+                    embeddings: a dictionary containing the text chunks with their ids and embeddings
+                    "texts": a dictionary of text chunks for each embedding (use index for correspondance)
+                    "infos": extra information
+                    "vectorizer": The vectorize if this is using tfidf or none if it uses model
+                }
+                'database_path': If supplied, the database is loaded from a path
+                'query': a query to search in the database
+            """
+            vectorization_method = parameters['vectorization_method']
+            database = parameters.get("database",None)
+            query = parameters.get("query",None)
+            if query is None:
+                ASCIIColors.error("No query given!")
+                emit('vector_db_query',{"status":False, "error":"Please supply a query"}) 
+                return
+            
+            if database is None:
+                database_path = parameters.get("database_path",None)
+                if database_path is None:
+                    ASCIIColors.error("No database given!")
+                    emit('vector_db_query',{"status":False, "error":"You did not supply a database file nor a database content"}) 
+                    return
+                else:
+                    with open(database_path, "r") as file:
+                        database = json.load(file)
+                        
+            tv = TextVectorizer(vectorization_method, self.model, database_dict=database)
+            docs, sorted_similarities = tv.recover_text(tv.embed_query(query))
+            emit('vectorized_db',{
+                "chunks":docs,
+                "refs":sorted_similarities
+            }) 
+            
+            
         @self.socketio.on('list_active_personalities')
         def handle_list_active_personalities():
             personality_names = [p.name for p in self.personalities]
             emit('active_personalities_list', {'success':True, 'personalities': personality_names}, room=request.sid)
 
         @self.socketio.on('activate_personality')
         def handle_activate_personality(data):
@@ -409,23 +429,29 @@
                 self.config.save_config()
             else:
                 emit('personality_add_failed', {'success':False, 'error': "Personality ID not valid"}, room=request.sid)
 
         @self.socketio.on('tokenize')
         def tokenize(data):
             prompt = data['prompt']
-            tk = self.active_model.tokenize(prompt)
+            tk = self.model.tokenize(prompt)
             emit("tokenized", {"tokens":tk})
 
         @self.socketio.on('detokenize')
         def detokenize(data):
             prompt = data['prompt']
-            txt = self.active_model.detokenize(prompt)
+            txt = self.model.detokenize(prompt)
             emit("detokenized", {"text":txt})
 
+        @self.socketio.on('embed')
+        def detokenize(data):
+            prompt = data['prompt']
+            txt = self.model.embed(prompt)
+            emit("embeded", {"text":txt})
+
         @self.socketio.on('cancel_generation')
         def cancel_generation(data):
             client_id = request.sid
             self.clients[client_id]["requested_stop"]=True
             print(f"Client {client_id} requested canceling generation")
             emit("generation_canceled", {"message":"Generation is canceled."})
             self.socketio.sleep(0)
@@ -438,15 +464,15 @@
             if not self.is_ready:
                 emit("buzzy", {"message":"I am buzzy. Come back later."}, room=client_id)
                 self.socketio.sleep(0)
                 ASCIIColors.warning(f"OOps request {client_id}  refused!! Server buzy")
                 return
             def generate_text():
                 self.is_ready = False
-                model = self.active_model
+                model = self.model
                 self.clients[client_id]["is_generating"]=True
                 self.clients[client_id]["requested_stop"]=False
                 prompt          = data['prompt']
                 personality_id  = data['personality']
                 n_predicts      = data["n_predicts"]
                 parameters      = data.get("parameters",{
                     "temperature":self.config["temperature"],
@@ -456,35 +482,37 @@
                     "repeat_last_n":self.config["repeat_last_n"],
                     "seed":self.config["seed"]
                 })
 
                 if personality_id==-1:
                     # Raw text generation
                     self.answer = {"full_text":""}
-                    def callback(text, message_type: MSG_TYPE):
+                    def callback(text, message_type: MSG_TYPE, metadata:dict={}):
                         if message_type == MSG_TYPE.MSG_TYPE_CHUNK:
-                            ASCIIColors.success(f"generated:{len(self.answer['full_text'])} words", end='\r')
+                            ASCIIColors.success(f"generated:{len(self.answer['full_text'].split())} words", end='\r')
                             self.answer["full_text"] = self.answer["full_text"] + text
                             self.socketio.emit('text_chunk', {'chunk': text, 'type':MSG_TYPE.MSG_TYPE_CHUNK.value}, room=client_id)
                             self.socketio.sleep(0)
                         if client_id in self.clients:# Client disconnected                      
                             if self.clients[client_id]["requested_stop"]:
                                 return False
                             else:
                                 return True
                         else:
                             return False                            
 
                     tk = model.tokenize(prompt)
                     n_tokens = len(tk)
-                    fd = model.detokenize(tk[-min(self.config.ctx_size,n_tokens):])
+                    fd = model.detokenize(tk[-min(self.config.ctx_size-n_predicts,n_tokens):])
 
                     try:
-                        ASCIIColors.print("warm up", ASCIIColors.color_bright_cyan)
-                        generated_text = model.generate(fd, n_predict=n_predicts, callback=callback,
+                        ASCIIColors.print("warming up", ASCIIColors.color_bright_cyan)
+                        generated_text = model.generate(fd, 
+                                                        n_predict=n_predicts, 
+                                                        callback=callback,
                                                         temperature = parameters["temperature"],
                                                         top_k = parameters["top_k"],
                                                         top_p = parameters["top_p"],
                                                         repeat_penalty = parameters["repeat_penalty"],
                                                         repeat_last_n = parameters["repeat_last_n"],
                                                         seed = parameters["seed"]                                                
                                                         )
@@ -497,14 +525,15 @@
                     except Exception as ex:
                         self.socketio.emit('generation_error', {'error': str(ex)}, room=client_id)
                         ASCIIColors.error(f"\ndone")
                     self.is_ready = True
                 else:
                     try:
                         personality: AIPersonality = self.personalities[personality_id]
+                        ump = self.config.discussion_prompt_separator +self.config.user_name+": " if self.config.use_user_name_in_discussions else self.personality.user_message_prefix
                         personality.model = model
                         cond_tk = personality.model.tokenize(personality.personality_conditioning)
                         n_cond_tk = len(cond_tk)
                         # Placeholder code for text generation
                         # Replace this with your actual text generation logic
                         print(f"Text generation requested by client: {client_id}")
 
@@ -514,58 +543,58 @@
                         if prompt != '':
                             if personality.processor is not None and personality.processor_cfg["process_model_input"]:
                                 preprocessed_prompt = personality.processor.process_model_input(prompt)
                             else:
                                 preprocessed_prompt = prompt
                             
                             if personality.processor is not None and personality.processor_cfg["custom_workflow"]:
-                                full_discussion_blocks.append(personality.user_message_prefix)
+                                full_discussion_blocks.append(ump)
                                 full_discussion_blocks.append(preprocessed_prompt)
                         
                             else:
 
-                                full_discussion_blocks.append(personality.user_message_prefix)
+                                full_discussion_blocks.append(ump)
                                 full_discussion_blocks.append(preprocessed_prompt)
                                 full_discussion_blocks.append(personality.link_text)
                                 full_discussion_blocks.append(personality.ai_message_prefix)
 
                         full_discussion = personality.personality_conditioning + ''.join(full_discussion_blocks)
 
-                        def callback(text, message_type: MSG_TYPE):
+                        def callback(text, message_type: MSG_TYPE, metadata:dict={}):
                             if message_type == MSG_TYPE.MSG_TYPE_CHUNK:
                                 self.answer["full_text"] = self.answer["full_text"] + text
                                 self.socketio.emit('text_chunk', {'chunk': text}, room=client_id)
                                 self.socketio.sleep(0)
                             try:
                                 if self.clients[client_id]["requested_stop"]:
                                     return False
                                 else:
                                     return True
                             except: # If the client is disconnected then we stop talking to it
                                 return False
 
                         tk = personality.model.tokenize(full_discussion)
                         n_tokens = len(tk)
-                        fd = personality.model.detokenize(tk[-min(self.config.ctx_size-n_cond_tk,n_tokens):])
+                        fd = personality.model.detokenize(tk[-min(self.config.ctx_size-n_cond_tk-personality.model_n_predicts,n_tokens):])
                         
                         if personality.processor is not None and personality.processor_cfg["custom_workflow"]:
-                            print("processing...", end="", flush=True)
+                            ASCIIColors.info("processing...")
                             generated_text = personality.processor.run_workflow(prompt, previous_discussion_text=personality.personality_conditioning+fd, callback=callback)
                         else:
-                            ASCIIColors.info("generating...", end="", flush=True)
+                            ASCIIColors.info("generating...")
                             generated_text = personality.model.generate(
                                                                         personality.personality_conditioning+fd, 
                                                                         n_predict=personality.model_n_predicts, 
                                                                         callback=callback)
 
                         if personality.processor is not None and personality.processor_cfg["process_model_output"]: 
                             generated_text = personality.processor.process_model_output(generated_text)
 
                         full_discussion_blocks.append(generated_text.strip())
-                        ASCIIColors.success("\ndone", end="", flush=True)
+                        ASCIIColors.success("\ndone")
 
                         # Emit the generated text to the client
                         self.socketio.emit('text_generated', {'text': generated_text}, room=client_id)
                         self.socketio.sleep(0)
                     except Exception as ex:
                         self.socketio.emit('generation_error', {'error': str(ex)}, room=client_id)
                         ASCIIColors.error(f"\ndone")
@@ -583,15 +612,28 @@
         loader = importlib.machinery.SourceFileLoader(module_name, str(absolute_path / "__init__.py"))
         binding_module = loader.load_module()
         binding = getattr(binding_module, binding_module.binding_name)
         return binding
 
 
     def run(self, host="localhost", port="9601"):
-        print(f"{ASCIIColors.color_red}Current personality : {ASCIIColors.color_reset}{self.active_personality}")
+        if self.binding is None:
+            ASCIIColors.warning("No binding selected. Please select one")
+            self.menu.select_binding()
+
+        print(f"{ASCIIColors.color_red}Current binding (model) : {ASCIIColors.color_reset}{self.binding}")
+        print(f"{ASCIIColors.color_red}Mounted personalities : {ASCIIColors.color_reset}{self.config.personalities}")
+        if len(self.config.personalities)==0:
+            ASCIIColors.warning("No personality selected. Selecting lollms. You can mount other personalities using lollms-settings application")
+            self.config.personalities = ["english/generic/lollms"]
+            self.config.save_config()
+
+        if self.config.active_personality_id>=len(self.config.personalities):
+            self.config.active_personality_id = 0
+        print(f"{ASCIIColors.color_red}Current personality : {ASCIIColors.color_reset}{self.config.personalities[self.config.active_personality_id]}")
         ASCIIColors.info(f"Serving on address: http://{host}:{port}")
 
         self.socketio.run(self.app, host=host, port=port)
 
 def main():
     LoLLMsServer()
```

### Comparing `lollms-2.1.9/lollms/settings.py` & `lollms-2.2.0/lollms/apps/settings/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,75 +4,39 @@
 from lollms.paths import LollmsPaths
 from lollms.binding import BindingBuilder, ModelBuilder
 import shutil
 from pathlib import Path
 import argparse
 from tqdm import tqdm
 from lollms.personality import PersonalityBuilder
-from lollms.console import MainMenu
+from lollms.apps.console import MainMenu
+from lollms.app import LollmsApplication
 
-def reset_all_installs(lollms_paths:LollmsPaths):
-    ASCIIColors.info("Removeing all configuration files to force reinstall")
-    ASCIIColors.info(f"Searching files from {lollms_paths.personal_configuration_path}")
-    for file_path in lollms_paths.personal_configuration_path.iterdir():
-        if file_path.name!=f"{lollms_paths.tool_prefix}local_config.yaml" and file_path.suffix.lower()==".yaml":
-            file_path.unlink()
-            ASCIIColors.info(f"Deleted file: {file_path}")
 
 
-class Settings:
+class Settings(LollmsApplication):
     def __init__(
                     self, 
                     configuration_path:str|Path=None, 
                     show_logo:bool=True, 
                     show_commands_list:bool=False, 
                     show_personality_infos:bool=True,
                     show_model_infos:bool=True,
                     show_welcome_message:bool=True
                 ):
-        
-        # Fore it to be a path
-        self.is_logging = False
-        self.log_file_path = ""
-        
-        self.bot_says = ""
+
         # get paths
-        self.lollms_paths = LollmsPaths.find_paths(force_local=False, tool_prefix="lollms_server_")
+        lollms_paths = LollmsPaths.find_paths(force_local=False, tool_prefix="lollms_server_")
         ASCIIColors.yellow("------ Lollms Paths ------")
-        ASCIIColors.info(self.lollms_paths)        
+        ASCIIColors.info(lollms_paths)        
         ASCIIColors.yellow("------ ------------ ------")
+        # Load maoin configuration
+        config = LOLLMSConfig.autoload(lollms_paths)
 
-        # Build menu
-        self.menu = MainMenu(self)
-        
-        # Change configuration
-        original = self.lollms_paths.default_cfg_path
-        if configuration_path is None:
-            local = self.lollms_paths.personal_configuration_path / f"{self.lollms_paths.tool_prefix}local_config.yaml"        
-        else:
-            local = Path(configuration_path)
-            
-        if not local.exists():
-            shutil.copy(original, local)
-        self.cfg_path = local
-
-        self.config = LOLLMSConfig(self.cfg_path, self.lollms_paths)
-        # load binding
-        if self.config.binding_name is not None:
-            self.load_binding()
-            # Load model
-            if self.config.model_name is not None:
-                self.load_model()
-
-        # Load personality
-        try:
-            self.load_personality()
-        except Exception as ex:
-            print(f"No personality selected. Please select one from the zoo. {ex}")
-            self.menu.select_personality()
+        super().__init__("lollms-settings", config, lollms_paths, load_model=False)
 
         if show_logo:
             self.menu.show_logo()
             
         if show_personality_infos:
             try:
                 print()
@@ -141,63 +105,26 @@
         except:
             return False            
 
     def stop_log(self):
         self.is_logging = False           
 
 
-
-    def load_binding(self):
-        if self.config.binding_name is None:
-            print(f"No bounding selected")
-            print("Please select a valid model or install a new one from a url")
-            self.menu.select_binding()
-            # cfg.download_model(url)
-        else:
-            try:
-                self.binding = BindingBuilder().build_binding(self.config, self.lollms_paths)
-            except Exception as ex:
-                print(ex)
-                print(f"Couldn't find binding. Please verify your configuration file at {self.cfg_path} or use the next menu to select a valid binding")
-                print(f"Trying to reinstall binding")
-                self.binding = BindingBuilder().build_binding(self.config, self.lollms_paths,installation_option=InstallOption.FORCE_INSTALL)
-                self.menu.select_binding()
-
-    def load_model(self):
-        try:
-            self.model = ModelBuilder(self.binding).get_model()
-        except Exception as ex:
-            ASCIIColors.error(f"Couldn't load model. Please verify your configuration file at {self.cfg_path} or use the next menu to select a valid model")
-            ASCIIColors.error(f"Binding returned this exception : {ex}")
-            ASCIIColors.error(f"{self.config.get_model_path_infos()}")
-            print("Please select a valid model or install a new one from a url")
-            self.menu.select_model()
-
-
-    def load_personality(self):
-        try:
-            self.personality = PersonalityBuilder(self.lollms_paths, self.config, self.model).build_personality()
-        except Exception as ex:
-            ASCIIColors.error(f"Couldn't load personality. Please verify your configuration file at {self.cfg_path} or use the next menu to select a valid personality")
-            ASCIIColors.error(f"Binding returned this exception : {ex}")
-            ASCIIColors.error(f"{self.config.get_personality_path_infos()}")
-            print("Please select a valid model or install a new one from a url")
-
     def reset_context(self):
         if self.personality.include_welcome_message_in_disucssion:
             full_discussion = (
                 self.personality.ai_message_prefix +
                 self.personality.welcome_message +
                 self.personality.link_text
             )
         else:
             full_discussion = ""
         return full_discussion
         
-    def safe_generate(self, full_discussion:str, n_predict=None, callback=None):
+    def safe_generate(self, full_discussion:str, n_predict=None, callback: Callable[[str, int, dict], bool]=None):
         """safe_generate
 
         Args:
             full_discussion (string): A prompt or a long discussion to use for generation
             callback (_type_, optional): A callback to call for each received token. Defaults to None.
 
         Returns:
@@ -244,15 +171,15 @@
 
 
 
     # Parse the command-line arguments
     args = parser.parse_args()
 
     if args.reset_installs:
-        reset_all_installs()
+        LollmsApplication.reset_all_installs()
 
     if args.reset_personal_path:
         LollmsPaths.reset_configs()
     
     if args.reset_config:
         lollms_paths = LollmsPaths.find_paths(tool_prefix="lollms_server_")
         cfg_path = lollms_paths.personal_configuration_path / f"{lollms_paths.tool_prefix}local_config.yaml"
```

### Comparing `lollms-2.1.9/lollms.egg-info/PKG-INFO` & `lollms-2.2.0/lollms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms
-Version: 2.1.9
+Version: 2.2.0
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/lollms
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms-2.1.9/setup.py` & `lollms-2.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,29 +22,30 @@
         if file_path.is_file():
             if file_path.name != "__pycache__" and file_path.suffix !=".pyc" and  file_path.name!="local_config.yaml" and file_path.name!=".installed" and file_path.name!=".git" and file_path.name!=".gitignore":
                 file_list.append("/".join(str(file_path).replace("\\","/").split("/")[1:]))
     return file_list
 
 setuptools.setup(
     name="lollms",
-    version="2.1.9",
+    version="2.2.0",
     author="Saifeddine ALOUI",
     author_email="aloui.saifeddine@gmail.com",
     description="A python library for AI personality definition",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/lollms",
     packages=setuptools.find_packages(),  
     include_package_data=True,
     install_requires=requirements,
     entry_points={
         'console_scripts': [
-            'lollms-server = lollms.server:main',
-            'lollms-console = lollms.console:main',
-            'lollms-settings = lollms.settings:main',
+            'lollms-server = lollms.apps.server:main',
+            'lollms-console = lollms.apps.console:main',
+            'lollms-settings = lollms.apps.settings:main',
+            'lollms-playground = lollms.apps.playground:main'
         ],
     },
     extras_require={"dev": requirements_dev},
     classifiers=[
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
```

