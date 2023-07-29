# Comparing `tmp/speech_intelligibility_index-1.0.1.tar.gz` & `tmp/speech_intelligibility_index-1.0.2.tar.gz`

## Comparing `speech_intelligibility_index-1.0.1.tar` & `speech_intelligibility_index-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.1/speech_intelligibility_index/BUILD.bazel
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.1/speech_intelligibility_index/WORKSPACE
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.1/speech_intelligibility_index/__init__.py
--rw-r--r--   0        0        0    25522 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.1/speech_intelligibility_index/sii.py
--rw-r--r--   0        0        0    25659 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.1/speech_intelligibility_index/sii_jax.py
--rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.1/speech_intelligibility_index/sii_jax_test.py
--rw-r--r--   0        0        0    12939 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.1/speech_intelligibility_index/sii_test.py
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.1/LICENSE
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.1/README.md
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.2/speech_intelligibility_index/BUILD.bazel
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.2/speech_intelligibility_index/WORKSPACE
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.2/speech_intelligibility_index/__init__.py
+-rw-r--r--   0        0        0    25522 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.2/speech_intelligibility_index/sii.py
+-rw-r--r--   0        0        0    25659 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.2/speech_intelligibility_index/sii_jax.py
+-rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.2/speech_intelligibility_index/sii_jax_test.py
+-rw-r--r--   0        0        0    12939 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.2/speech_intelligibility_index/sii_test.py
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.2/README.md
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.2/PKG-INFO
```

### Comparing `speech_intelligibility_index-1.0.1/speech_intelligibility_index/__init__.py` & `speech_intelligibility_index-1.0.2/speech_intelligibility_index/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,12 +25,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 """Package init file for speech_intelligility_index
 """
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 
 # No imports here, instead use
 #    from speech_intelligibility_index import XXX
 # where XXX is the individual file name (sii.py or sii_jax.py)
+
+__all__ = ['sii.py', 'sii_jax.py', 'sii_test.py', 'sii_jax_test.py']
```

### Comparing `speech_intelligibility_index-1.0.1/speech_intelligibility_index/sii.py` & `speech_intelligibility_index-1.0.2/speech_intelligibility_index/sii.py`

 * *Files identical despite different names*

### Comparing `speech_intelligibility_index-1.0.1/speech_intelligibility_index/sii_jax.py` & `speech_intelligibility_index-1.0.2/speech_intelligibility_index/sii_jax.py`

 * *Files identical despite different names*

### Comparing `speech_intelligibility_index-1.0.1/speech_intelligibility_index/sii_jax_test.py` & `speech_intelligibility_index-1.0.2/speech_intelligibility_index/sii_jax_test.py`

 * *Files identical despite different names*

### Comparing `speech_intelligibility_index-1.0.1/speech_intelligibility_index/sii_test.py` & `speech_intelligibility_index-1.0.2/speech_intelligibility_index/sii_test.py`

 * *Files identical despite different names*

### Comparing `speech_intelligibility_index-1.0.1/LICENSE` & `speech_intelligibility_index-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `speech_intelligibility_index-1.0.1/README.md` & `speech_intelligibility_index-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `speech_intelligibility_index-1.0.1/pyproject.toml` & `speech_intelligibility_index-1.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "absl-py",
+    "jax", 
+    "jaxlib", 
     "numpy",
     "matplotlib",
 ]
 
 [[project.authors]]
 name = "Malcolm Slaney"
 email = "speech-intelligibility-index-maintainers@googlegroups.com"
```

### Comparing `speech_intelligibility_index-1.0.1/PKG-INFO` & `speech_intelligibility_index-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: speech-intelligibility-index
-Version: 1.0.1
+Version: 1.0.2
 Summary: Speech Intelligibility Index
 Project-URL: Homepage, https://github.com/google/speech_intelligibility_index
 Project-URL: Bug Tracker, https://github.com/google/speech_intelligibility_index/issues
 Author-email: Malcolm Slaney <speech-intelligibility-index-maintainers@googlegroups.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Requires-Dist: absl-py
+Requires-Dist: jax
+Requires-Dist: jaxlib
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Description-Content-Type: text/markdown
 
 A Python implementation of American National Standard ANSI S3.5-1997
 **"Methods for Calculation of the Speech Intelligibility Index"**
 This code is translated from Hannes Muesch's Matlab implementation.
```

