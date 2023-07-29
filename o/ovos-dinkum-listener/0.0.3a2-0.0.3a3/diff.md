# Comparing `tmp/ovos-dinkum-listener-0.0.3a2.tar.gz` & `tmp/ovos-dinkum-listener-0.0.3a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-dinkum-listener-0.0.3a2.tar", last modified: Thu Jul 27 22:46:13 2023, max compression
+gzip compressed data, was "ovos-dinkum-listener-0.0.3a3.tar", last modified: Sat Jul 29 17:07:04 2023, max compression
```

## Comparing `ovos-dinkum-listener-0.0.3a2.tar` & `ovos-dinkum-listener-0.0.3a3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:46:13.201897 ovos-dinkum-listener-0.0.3a2/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-27 22:46:08.000000 ovos-dinkum-listener-0.0.3a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-07-27 22:46:13.201897 ovos-dinkum-listener-0.0.3a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-07-27 22:46:08.000000 ovos-dinkum-listener-0.0.3a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:46:13.201897 ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-27 22:46:08.000000 ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-27 22:46:08.000000 ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-27 22:46:08.000000 ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:46:13.201897 ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener/res/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:46:13.201897 ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener/res/snd/
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-07-27 22:46:08.000000 ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener/res/snd/acknowledge.mp3
--rw-r--r--   0 runner    (1001) docker     (123)    13290 2023-07-27 22:46:08.000000 ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener/res/snd/error.mp3
--rw-r--r--   0 runner    (1001) docker     (123)    67090 2023-07-27 22:46:08.000000 ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener/res/snd/start_listening.wav
--rw-r--r--   0 runner    (1001) docker     (123)    36632 2023-07-27 22:46:08.000000 ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-07-27 22:46:08.000000 ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener/transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-27 22:46:08.000000 ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:46:13.201897 ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener/voice_loop/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-27 22:46:08.000000 ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener/voice_loop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12531 2023-07-27 22:46:08.000000 ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener/voice_loop/hotwords.py
--rw-r--r--   0 runner    (1001) docker     (123)    25955 2023-07-27 22:46:08.000000 ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener/voice_loop/voice_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:46:13.201897 ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-07-27 22:46:13.000000 ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-27 22:46:13.000000 ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 22:46:13.000000 ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-27 22:46:13.000000 ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-27 22:46:13.000000 ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 22:46:13.000000 ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 22:46:13.201897 ovos-dinkum-listener-0.0.3a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-07-27 22:46:08.000000 ovos-dinkum-listener-0.0.3a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:07:04.550918 ovos-dinkum-listener-0.0.3a3/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-29 17:06:59.000000 ovos-dinkum-listener-0.0.3a3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-07-29 17:07:04.550918 ovos-dinkum-listener-0.0.3a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-07-29 17:06:59.000000 ovos-dinkum-listener-0.0.3a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:07:04.546918 ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-29 17:06:59.000000 ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-29 17:06:59.000000 ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-29 17:06:59.000000 ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:07:04.546918 ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener/res/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:07:04.550918 ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener/res/snd/
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-07-29 17:06:59.000000 ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener/res/snd/acknowledge.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    13290 2023-07-29 17:06:59.000000 ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener/res/snd/error.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    67090 2023-07-29 17:06:59.000000 ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener/res/snd/start_listening.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    37170 2023-07-29 17:06:59.000000 ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-07-29 17:06:59.000000 ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-29 17:06:59.000000 ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:07:04.550918 ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener/voice_loop/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-29 17:06:59.000000 ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener/voice_loop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12531 2023-07-29 17:06:59.000000 ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener/voice_loop/hotwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26020 2023-07-29 17:06:59.000000 ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener/voice_loop/voice_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:07:04.546918 ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-07-29 17:07:04.000000 ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-29 17:07:04.000000 ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 17:07:04.000000 ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-29 17:07:04.000000 ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-29 17:07:04.000000 ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 17:07:04.000000 ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 17:07:04.550918 ovos-dinkum-listener-0.0.3a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-07-29 17:06:59.000000 ovos-dinkum-listener-0.0.3a3/setup.py
```

### Comparing `ovos-dinkum-listener-0.0.3a2/PKG-INFO` & `ovos-dinkum-listener-0.0.3a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-dinkum-listener
-Version: 0.0.3a2
+Version: 0.0.3a3
 Summary: ovos-core listener daemon client
 Home-page: https://github.com/OpenVoiceOS/ovos-dinkum-listener
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
```

### Comparing `ovos-dinkum-listener-0.0.3a2/README.md` & `ovos-dinkum-listener-0.0.3a3/README.md`

 * *Files identical despite different names*

### Comparing `ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener/__init__.py` & `ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener/__main__.py` & `ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener/__main__.py`

 * *Files identical despite different names*

### Comparing `ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener/plugins.py` & `ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener/plugins.py`

 * *Files identical despite different names*

### Comparing `ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener/res/snd/acknowledge.mp3` & `ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener/res/snd/acknowledge.mp3`

 * *Files identical despite different names*

### Comparing `ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener/res/snd/error.mp3` & `ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener/res/snd/error.mp3`

 * *Files identical despite different names*

### Comparing `ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener/res/snd/start_listening.wav` & `ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener/res/snd/start_listening.wav`

 * *Files identical despite different names*

### Comparing `ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener/service.py` & `ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-#
+
 import json
 import time
 import wave
 from enum import Enum
 from hashlib import md5
 from pathlib import Path
 from threading import Thread, RLock, Event
@@ -26,16 +26,16 @@
 from ovos_plugin_manager.microphone import OVOSMicrophoneFactory
 from ovos_plugin_manager.stt import get_stt_lang_configs, get_stt_supported_langs, get_stt_module_configs
 from ovos_plugin_manager.utils.tts_cache import hash_sentence
 from ovos_plugin_manager.vad import OVOSVADFactory
 from ovos_plugin_manager.vad import get_vad_configs
 from ovos_plugin_manager.wakewords import get_ww_lang_configs, get_ww_supported_langs, get_ww_module_configs
 from ovos_utils.file_utils import resolve_resource_file
-from ovos_utils.log import LOG
-from ovos_utils.process_utils import ProcessStatus, StatusCallbackMap
+from ovos_utils.log import LOG, log_deprecation
+from ovos_utils.process_utils import ProcessStatus, StatusCallbackMap, ProcessState
 from ovos_utils.sound import play_audio
 
 from ovos_dinkum_listener.plugins import load_stt_module, load_fallback_stt
 from ovos_dinkum_listener.transformers import AudioTransformersService
 from ovos_dinkum_listener.voice_loop import DinkumVoiceLoop, ListeningMode, ListeningState
 from ovos_dinkum_listener.voice_loop.hotwords import HotwordContainer
 
@@ -130,15 +130,14 @@
         self.service_id = "voice"
         self.status = ProcessStatus(self.service_id, self.bus,
                                     callback_map=callbacks)
         self._watchdog = watchdog
         self._shutdown_event = Event()
         self._stopping = False
         self.status.set_alive()
-        self._state: ServiceState = ServiceState.NOT_STARTED
         self.config = Configuration()
 
         self._before_start()  # connect to bus
 
         # Initialize with default (bundled) plugin
         microphone_config = self.config.get("listener",
                                             {}).get("microphone", {})
@@ -231,50 +230,63 @@
     def default_save_path(self):
         """ where recorded hotwords/utterances are saved """
         listener = Configuration().get("listener", {})
         return listener.get('save_path', f"{get_xdg_data_save_path()}/listener")
 
     @property
     def state(self):
-        return self._state
+        log_deprecation("This property is deprecated, reference `status.state`",
+                        "0.1.0")
+        if self.status.state in (ProcessState.NOT_STARTED, ProcessState.ALIVE):
+            return ServiceState.NOT_STARTED
+        if self.status.state == ProcessState.STARTED:
+            return ServiceState.STARTED
+        if self.status.state == ProcessState.READY:
+            return ServiceState.RUNNING
+        if self.status.state in (ProcessState.ERROR, ProcessState.STOPPING):
+            return ServiceState.STOPPING
+        return self.status.state
 
     def run(self):
         """
         Service entry point
         """
         try:
-            self._state = ServiceState.NOT_STARTED
+            self.status.set_alive()
             self._before_start()  # Ensure configuration and bus are initialized
             self._start()
-            self._state = ServiceState.STARTED
+            self.status.set_started()
             self._after_start()
             LOG.debug("Service started")
-
-            try:
-                self.status.set_ready()
-                LOG.info("Service ready")
-                while not self._stopping:
-                    if not self._reload_event.wait(30):
-                        raise TimeoutError("Timed out waiting for reload")
-                    self._state = ServiceState.RUNNING
-                    self.voice_loop.run()
-            except KeyboardInterrupt:
-                pass
-            except Exception as e:
-                LOG.exception("voice_loop failed")
-                self.status.set_error(str(e))
-            finally:
-                LOG.info("Service stopping")
-                self._state = ServiceState.STOPPING
-                self._shutdown()
-                self._after_stop()
-                self._state = ServiceState.NOT_STARTED
         except Exception as e:
             LOG.exception("Service failed to start")
             self.status.set_error(str(e))
+            return
+
+        try:
+            self.status.set_ready()
+            LOG.info("Service ready")
+            while not self._stopping:
+                if not self._reload_event.wait(30):
+                    raise TimeoutError("Timed out waiting for reload")
+                self.voice_loop.run()
+            self.status.set_stopping()
+        except KeyboardInterrupt:
+            self.status.set_stopping()
+        except Exception as e:
+            LOG.exception("voice_loop failed")
+            self.status.set_error(str(e))
+        finally:
+            LOG.info("Service stopping")
+            self._shutdown()
+            LOG.debug("shutdown done")
+            self._after_stop()
+            LOG.debug("stopped")
+            if self.status.state != ProcessState.ERROR:
+                self.status.state = ProcessState.NOT_STARTED
 
     def _before_start(self):
         """
         Initialization logic called on module init
         """
         self.config = self.config or Configuration()
         LOG.info("Starting service...")
@@ -358,15 +370,15 @@
         except Exception as e:
             LOG.exception(f"Shutdown failed with: {e}")
         self._shutdown_event.set()
         self._load_lock.release()
 
     def _after_stop(self):
         """Shut down code called after stop()"""
-        self.status.set_stopping()
+        # self.status.set_stopping()
         self.bus.close()
 
     def _connect_to_bus(self):
         """Connects to the websocket message bus"""
         self.bus = self.bus or MessageBusClient()
         if not self.bus.started_running:
             LOG.debug("Starting bus connection")
```

### Comparing `ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener/transformers.py` & `ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener/transformers.py`

 * *Files identical despite different names*

### Comparing `ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener/voice_loop/__init__.py` & `ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener/voice_loop/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener/voice_loop/hotwords.py` & `ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener/voice_loop/hotwords.py`

 * *Files identical despite different names*

### Comparing `ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener/voice_loop/voice_loop.py` & `ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener/voice_loop/voice_loop.py`

 * *Files 0% similar despite different names*

```diff
@@ -511,15 +511,16 @@
 
             # Wait for enough speech before looking for the end of the
             # command (silence).
             try:
                 self._chunk_info.is_speech = not self.vad.is_silence(stt_chunk)
             except Exception as e:
                 LOG.exception(f"Error processing chunk of "
-                              f"size={len(stt_chunk)}: {e}")
+                              f"size={len(stt_chunk)} with "
+                              f"SR={self.vad.sample_rate}: {e}")
 
             if self._chunk_info.is_speech:
                 self.speech_seconds_left -= self.mic.seconds_per_chunk
                 if self.speech_seconds_left <= 0:
                     # Voice command has started, so start looking for the
                     # end.
                     self.state = ListeningState.IN_COMMAND
```

### Comparing `ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener.egg-info/PKG-INFO` & `ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-dinkum-listener
-Version: 0.0.3a2
+Version: 0.0.3a3
 Summary: ovos-core listener daemon client
 Home-page: https://github.com/OpenVoiceOS/ovos-dinkum-listener
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
```

### Comparing `ovos-dinkum-listener-0.0.3a2/ovos_dinkum_listener.egg-info/SOURCES.txt` & `ovos-dinkum-listener-0.0.3a3/ovos_dinkum_listener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-dinkum-listener-0.0.3a2/setup.py` & `ovos-dinkum-listener-0.0.3a3/setup.py`

 * *Files identical despite different names*

