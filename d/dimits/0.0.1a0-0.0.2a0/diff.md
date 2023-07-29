# Comparing `tmp/dimits-0.0.1a0.tar.gz` & `tmp/dimits-0.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dimits-0.0.1a0.tar", max compression
+gzip compressed data, was "dimits-0.0.2a0.tar", max compression
```

## Comparing `dimits-0.0.1a0.tar` & `dimits-0.0.2a0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      128 2023-07-06 12:15:58.182853 dimits-0.0.1a0/dimits/__init__.py
--rw-r--r--   0        0        0     9441 2023-07-06 07:11:25.156107 dimits-0.0.1a0/dimits/main.py
--rw-r--r--   0        0        0     4739 2023-07-06 14:35:07.238077 dimits-0.0.1a0/dimits/t.py
--rw-r--r--   0        0        0     2056 2023-07-06 10:19:58.221599 dimits-0.0.1a0/dimits/utils.py
--rw-r--r--   0        0        0     1079 2023-06-28 10:26:13.254270 dimits-0.0.1a0/LICENSE
--rw-r--r--   0        0        0      644 2023-07-08 15:17:19.856908 dimits-0.0.1a0/pyproject.toml
--rw-r--r--   0        0        0     2839 2023-07-06 12:25:10.583486 dimits-0.0.1a0/README.md
--rw-r--r--   0        0        0     3511 1970-01-01 00:00:00.000000 dimits-0.0.1a0/PKG-INFO
+-rw-r--r--   0        0        0      163 2023-07-29 15:53:03.793881 dimits-0.0.2a0/dimits/__init__.py
+-rw-r--r--   0        0        0     8114 2023-07-29 15:52:47.945568 dimits-0.0.2a0/dimits/main.py
+-rw-r--r--   0        0        0     6104 2023-07-29 15:49:49.628760 dimits-0.0.2a0/dimits/ttsmodel.py
+-rw-r--r--   0        0        0     2056 2023-07-06 10:19:58.221599 dimits-0.0.2a0/dimits/utils.py
+-rw-r--r--   0        0        0     1079 2023-06-28 10:26:13.254270 dimits-0.0.2a0/LICENSE
+-rw-r--r--   0        0        0      711 2023-07-29 15:56:45.375138 dimits-0.0.2a0/pyproject.toml
+-rw-r--r--   0        0        0     2843 2023-07-29 14:58:34.457187 dimits-0.0.2a0/README.md
+-rw-r--r--   0        0        0     3582 1970-01-01 00:00:00.000000 dimits-0.0.2a0/PKG-INFO
```

### Comparing `dimits-0.0.1a0/dimits/main.py` & `dimits-0.0.2a0/dimits/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import os
 
 from dimits.utils import download, untar, logger
-import requests
 
+from dimits.ttsmodel import TextToSpeechModel as ttsm
+import requests
+import shutil
 import platform
 
 import requests
-from tqdm import tqdm
 
 from pathlib import Path
 
 
 
 
 class Dimits():
@@ -29,92 +30,48 @@
 
         Example:
             >>> from Dimits import Dimits
             >>> dt = Dimits("voice-en-us-amy-low")
         """
         self.verbose = verbose
         # Define the URL for the latest release of piper
-        arch = str(self._get_arch())
-        if self._get_arch() == 'unsupported_machine': 
+        arch = str(self._get_os())
+        if self._get_os() == 'unsupported_machine': 
             logger(err= f'{arch} Detected', verbose=verbose)
-            
-        if self._get_arch() == 'unsupported_machine': return
-        logger(msg= f'{arch} Detected', verbose=verbose)
+            return 
 
         home = str(Path.home())
         
         self.voice = voice
         self.folder = 'piper'
-        self.piper_bin_zip = f'piper_{arch}.tar.gz'
+      
         
         self.parent_destn = os.path.join(home, self.folder)
         if not os.path.exists(self.parent_destn):
             os.mkdir(self.parent_destn)
 
-        # Set the full filepath for the downloaded file
-        self.filepath = os.path.join(self.parent_destn, self.piper_bin_zip)
-
-        #Download the binary if it does not exist
-        if not os.path.exists(self.filepath):
-            latest_releases_url = f"https://api.github.com/repos/rhasspy/piper/releases/latest"
-
-        # Fetch the latest release information from Github API
-            latest_releases_response = requests.get(latest_releases_url)
-    
-            # Parse the latest version number from the API response
-            if latest_releases_response.status_code == 200:
-                # Parse the api JSON to extract the release version
-                release_info = latest_releases_response.json()
-                latest_release = release_info["tag_name"]
-
-            # Set the URL for the binary download
-            binary_url = f"https://github.com/rhasspy/piper/releases/download/{latest_release}/{self.piper_bin_zip}"
-
-            # Download the binary file and check for errors
-            response = download(binary_url, self.filepath,
-                                self.piper_bin_zip, verbose=verbose)
-
-            # If the response is a tuple, extract the filepath and filename and untar the file
-            if type(response) is tuple:
-                fp, f = response
-                untar(fp, f, verbose=verbose)
-            # If the response is an integer, log an error message
-            elif type(response) is int:
-                logger(err=f"Can't Download {self.piper_bin_zip}", verbose=verbose)
-
-        # Set the path to the piper binary file
-        self.piper_binary = os.path.join(self.parent_destn, 'piper', 'piper')
-
-        # print(self.binary)
-
+       
         # Download the voice if it does not exist
         self._download_voice(voice)
 
         # Set the path to the ONNX voice file
 
         self.voice_onnx = voice
         self.voice_onnx = os.path.join(
         self.parent_destn, str(self.voice_onnx).replace('voice-', '') + '.onnx')
-        logger('Using' + str(self.voice_onnx), verbose=verbose)
+        logger('Using ' + str(self.voice_onnx), verbose=verbose)
 
     
     @staticmethod    
-    def _get_arch(_: str = '') -> str:
-
-        if platform.system() == 'Linux':
-            if platform.machine() == 'aarch64':
-                return 'arm64'
-            elif platform.machine() == 'amd64' or platform.machine() == 'x86_64':
-                return 'amd64'
-            elif platform.machine().startswith('armv7'):
-
-                return 'armv7'
-        else :
+    def _get_os() -> str:
+        if (platform.system() in ['Windows', 'Linux']):
+            return  platform.system();
+        else: 
+            return "unsupported_machine"
 
-            return ('unsupported_machine')
       
     @staticmethod
     def list_voice() -> list[str]:
         """
         Method `list_voice()` Lists the supported voice as per in from https://api.github.com/repos/rhasspy/piper/releases
         
         Args:
@@ -145,15 +102,15 @@
             if type(download(download_url, filepath, filename, verbose)) is tuple:
                 fp, f = tuple(download(download_url, filepath, filename, verbose))
                 untar(fp, f, verbose)
             
                 
            
 
-    def text_2_audio_file(self, text: str, filename: str, directory: str, format: str = 'wav', **kwargs: str) -> str:
+    def text_2_audio_file(self, text: str, filename: str, directory: str, format: str = 'wav') -> str:
         r"""
 
         Convert the provided text to a human-sounding audio file using a text-to-speech engine, and save it to disk.
 
         Args:
             text (str): The text to be converted to audio.
             filename (str): The name of the output audio file, without the file extension.
@@ -168,30 +125,23 @@
         Example:
             >>> from Dimits import Dimits
             >>> dt = ... #Initialize here
             >>> dt.text_to_audio("Hello World", "hello_world", "wav", "/path/to/output/directory/")
             >>> # Outputs an audio file named "hello_world.wav" in the directory "/path/to/output/directory/".
 
        """
-        if self._get_arch() == 'unsupported_machine': return
+        if self._get_os() == 'unsupported_machine': return
         if not os.path.exists(directory):
             os.mkdir(directory)
         filepath = os.path.join(directory, f'{filename}.{format}')
         
-        param = (' ').join(
-            list([f'--{_} {__}'for _, __ in tuple(kwargs.items())]))
-        
-
-        
-        if platform.system() == 'Linux':
-            command = f"""echo \"{text}\" |sudo {self.piper_binary} --model {self.voice_onnx} --output_file {filepath} {param}"""
-            os.system(command)
-        elif platform.system() == 'Windows':
-            # TODO 
-            pass
+     
+        out_bin = ttsm(self.voice_onnx).synthesize(text,length_scale=1.0, noise_scale=1.0, noise_w=1.0)
+        with open(filepath, 'wb') as f:
+            f.write(out_bin)
 
         return filepath
 
     def text_file_2_audio_file(self, text_file_path: str, audio_filename: str, directory: str, audio_format: str='wav', encoding='utf8', **kwargs) -> str:
         """
         Convert the provided text files to audio file
 
@@ -206,20 +156,20 @@
             str: audio file path
 
         Example:
             >>> from dimits import Dimits 
             >>> dd = ...
             >>> dd.text_file_2_audio_file(file_path,'hello', dir,)
         """
-        if self._get_arch() == 'unsupported_machine': return
+        if self._get_os() == 'unsupported_machine': return
         with open(text_file_path, encoding=encoding) as f:
            return self.text_2_audio_file(f.readline(), audio_filename, directory, audio_format, **kwargs)
 
 
-    def text_2_speech(self, text: str, engine: str = 'aplay', **kwargs: str) -> None:
+    def text_2_speech(self, text: str, engine: str = None , **kwargs: str) -> None:
         
         r"""
         Convert the provided text to human-sounding audio and play the audio file on-the-go.
 
         Args:
             text (str): The text to be converted to audio.
             engine (str): The text-to-speech engine to play the audio file .
@@ -232,35 +182,46 @@
         Example:
             >>> from dimits import Dimits
             >>> dt = ... #Initialize here
             >>> dt.text_2_speech("Hello World", "aplay"")
             >>> # plays the audio to the default audio output device using the 'alsa' engine.
         """
         
-        if self._get_arch() == 'unsupported_machine': return
+        if self._get_os() == 'unsupported_machine': return
         cache_dir  = os.path.join(self.parent_destn, 'cache')
-        os.system(f'rm -rf {cache_dir}/*')
-        
+        if os.path.isdir(cache_dir):
+            shutil.rmtree(cache_dir)
+            os.mkdir(cache_dir)
+
+        filepath = self.text_2_audio_file(
+                       text, 'main', directory=cache_dir, )
         if platform.system() == 'Linux':
         
            os.system(f'killall {engine}')
-           
-           
-           filepath = self.text_2_audio_file(
-               text, 'main', directory=cache_dir, **kwargs)
+           if engine == None: engine = 'aplay'
            
            if engine == 'aplay':
               os.system(f'{engine} {filepath}')
            else:
                pass
         elif platform.system() == 'Windows':
-            engine = ''
-            # TODO
-            pass
+            if engine == None:  engine = 'System.Media.SoundPlayer'
+
+
+           
+            if engine == 'System.Media.SoundPlayer':
+               cmd = f"""powershell (New-Object {engine} {filepath}).PlaySync()"""
+               os.system(cmd )
+           
     
  
 
+print(Dimits.list_voice())
+Dimits("voice-en-us-danny-low").text_2_speech(text="""
+Here is a randomly generated short story:
+
+It was a dark and stormy night. John was home alone, sitting in his living room reading a book. The wind howled outside as the rain pattered against the windows. Suddenly, there was a loud crash from the kitchen. John jumped up, his heart racing. What was that?
 
+As John slowly walked towards the kitchen, he could hear a strange skittering sound. He flipped on the light switch, but the power was out. Grabbing a flashlight from a drawer, he shined it around the room. In the beam of light, John saw the shattered remains of a flower vase on the floor.""", filename='test', directory='C:\\Users\\Ananiya\\PyProject\\PyPiperTTS\\dimits')
 
-Dimits("voice-en-us-amy-low")
```

### Comparing `dimits-0.0.1a0/dimits/utils.py` & `dimits-0.0.2a0/dimits/utils.py`

 * *Files identical despite different names*

### Comparing `dimits-0.0.1a0/LICENSE` & `dimits-0.0.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `dimits-0.0.1a0/pyproject.toml` & `dimits-0.0.2a0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [tool.poetry]
 name = "dimits"
-version = "0.0.1-alpha"
+version = "0.0.2-alpha"
 description = "Dimits is a Python library that provides an easy-to-use interface to the Piper text-to-speech (TTS) system. It utilizes the powerful Piper TTS engine, which is optimized for Raspberry Pi 4, to generate high-quality synthesized speech."
 authors = ["Reqeique <ananiyajemberu21@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "Dimits"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = { version = "^2.13.0", source = "private" }
+espeak-phonemizer-windows = { version = "*", platform = "win32" }
 tqdm = "4.64.0" 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dimits-0.0.1a0/README.md` & `dimits-0.0.2a0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 To change the voice used for synthesis, create a new instance of the `Dimits` class with the desired voice model:
 
 ```python
 # dt = Dimits("voice-en-us-amy-low")
 dt = Dimits("voice-en-us-danny-low")
 ```
 ## TODO 📝
-* Implement windows compatible executible to run the voice models
+* ~~Implement windows compatible executible to run the voice models~~
 * Support for multiple audio player engine
 * Benchmark
 * Documentation
 
 
 ## License 🪪
```

### Comparing `dimits-0.0.1a0/PKG-INFO` & `dimits-0.0.2a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: dimits
-Version: 0.0.1a0
+Version: 0.0.2a0
 Summary: Dimits is a Python library that provides an easy-to-use interface to the Piper text-to-speech (TTS) system. It utilizes the powerful Piper TTS engine, which is optimized for Raspberry Pi 4, to generate high-quality synthesized speech.
 License: MIT
 Author: Reqeique
 Author-email: ananiyajemberu21@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: espeak-phonemizer-windows ; sys_platform == "win32"
 Requires-Dist: requests (>=2.13.0,<3.0.0)
 Requires-Dist: tqdm (==4.64.0)
 Description-Content-Type: text/markdown
 
 
 # **Dimits - Python Bindings for Piper TTS**
 
@@ -88,15 +89,15 @@
 To change the voice used for synthesis, create a new instance of the `Dimits` class with the desired voice model:
 
 ```python
 # dt = Dimits("voice-en-us-amy-low")
 dt = Dimits("voice-en-us-danny-low")
 ```
 ## TODO 📝
-* Implement windows compatible executible to run the voice models
+* ~~Implement windows compatible executible to run the voice models~~
 * Support for multiple audio player engine
 * Benchmark
 * Documentation
 
 
 ## License 🪪
```

