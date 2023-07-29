# Comparing `tmp/speech_intelligibility_index-1.0.0.tar.gz` & `tmp/speech_intelligibility_index-1.0.1.tar.gz`

## Comparing `speech_intelligibility_index-1.0.0.tar` & `speech_intelligibility_index-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,11 @@
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.0/setup.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.0/speech_intelligibility_index/BUILD.bazel
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.0/speech_intelligibility_index/WORKSPACE
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.0/speech_intelligibility_index/__init__.py
--rw-r--r--   0        0        0    25522 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.0/speech_intelligibility_index/sii.py
--rw-r--r--   0        0        0    25659 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.0/speech_intelligibility_index/sii_jax.py
--rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.0/speech_intelligibility_index/sii_jax_test.py
--rw-r--r--   0        0        0    12939 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.0/speech_intelligibility_index/sii_test.py
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.0/LICENSE
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.0/README.md
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.1/speech_intelligibility_index/BUILD.bazel
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.1/speech_intelligibility_index/WORKSPACE
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.1/speech_intelligibility_index/__init__.py
+-rw-r--r--   0        0        0    25522 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.1/speech_intelligibility_index/sii.py
+-rw-r--r--   0        0        0    25659 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.1/speech_intelligibility_index/sii_jax.py
+-rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.1/speech_intelligibility_index/sii_jax_test.py
+-rw-r--r--   0        0        0    12939 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.1/speech_intelligibility_index/sii_test.py
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.1/README.md
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 speech_intelligibility_index-1.0.1/PKG-INFO
```

### Comparing `speech_intelligibility_index-1.0.0/setup.py` & `speech_intelligibility_index-1.0.1/speech_intelligibility_index/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -23,38 +23,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-"""Create the speech_intelligibility_index package files.
+"""Package init file for speech_intelligility_index
 """
+__version__ = "1.0.1"
 
-import setuptools
-
-with open('README.md', 'r') as fh:
-  long_description = fh.read()
-
-setuptools.setup(
-    name='speech_intelligibility_index',
-    version='1.0.0',
-    author='Malcolm Slaney',
-    author_email='speech-intelligibility-index-maintainers@googlegroups.com',
-    description='Speech Intelligibility Index',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    url='https://github.com/google/speech_intelligibility_index',
-    packages=['speech_intelligibility_index'],
-    classifiers=[
-        'Programming Language :: Python :: 3',
-        'License :: OSI Approved :: Apache Software License',
-        'Operating System :: OS Independent',
-    ],
-    python_requires='>=3.6',
-    install_requires=[
-        'absl-py',
-        'numpy',
-        # 'jax',  # Optional
-    ],
-    include_package_data=True,  # Using the files specified in MANIFEST.in
-)
+# No imports here, instead use
+#    from speech_intelligibility_index import XXX
+# where XXX is the individual file name (sii.py or sii_jax.py)
```

### Comparing `speech_intelligibility_index-1.0.0/speech_intelligibility_index/sii.py` & `speech_intelligibility_index-1.0.1/speech_intelligibility_index/sii.py`

 * *Files identical despite different names*

### Comparing `speech_intelligibility_index-1.0.0/speech_intelligibility_index/sii_jax.py` & `speech_intelligibility_index-1.0.1/speech_intelligibility_index/sii_jax.py`

 * *Files identical despite different names*

### Comparing `speech_intelligibility_index-1.0.0/speech_intelligibility_index/sii_jax_test.py` & `speech_intelligibility_index-1.0.1/speech_intelligibility_index/sii_jax_test.py`

 * *Files identical despite different names*

### Comparing `speech_intelligibility_index-1.0.0/speech_intelligibility_index/sii_test.py` & `speech_intelligibility_index-1.0.1/speech_intelligibility_index/sii_test.py`

 * *Files identical despite different names*

### Comparing `speech_intelligibility_index-1.0.0/LICENSE` & `speech_intelligibility_index-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `speech_intelligibility_index-1.0.0/README.md` & `speech_intelligibility_index-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `speech_intelligibility_index-1.0.0/pyproject.toml` & `speech_intelligibility_index-1.0.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,37 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
-name = "speech_intelligibility_index"
-version = "1.0.0"
-authors = [
-  { name="Malcolm Slaney", email="malcolmslaney@gmail.com" },
-]
-description = "Code that implements the ANSI standard Speech Intelligibility Index"
+name = "speech-intelligibility-index"
+dynamic = ["version"]
+description = "Speech Intelligibility Index"
 readme = "README.md"
-requires-python = ">=3.7"
+license = "Apache-2.0"
+requires-python = ">=3.6"
 classifiers = [
-    "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3",
+]
+dependencies = [
+    "absl-py",
+    "numpy",
+    "matplotlib",
+]
+
+[[project.authors]]
+name = "Malcolm Slaney"
+email = "speech-intelligibility-index-maintainers@googlegroups.com"
+
+[tool.hatch.version]
+path = "speech_intelligibility_index/__init__.py"
+
+[tool.hatch.build.targets.sdist]
+include = [
+    "/speech_intelligibility_index",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/google/speech_intelligibility_index"
 "Bug Tracker" = "https://github.com/google/speech_intelligibility_index/issues"
```

### Comparing `speech_intelligibility_index-1.0.0/PKG-INFO` & `speech_intelligibility_index-1.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
-Name: speech_intelligibility_index
-Version: 1.0.0
-Summary: Code that implements the ANSI standard Speech Intelligibility Index
+Name: speech-intelligibility-index
+Version: 1.0.1
+Summary: Speech Intelligibility Index
 Project-URL: Homepage, https://github.com/google/speech_intelligibility_index
 Project-URL: Bug Tracker, https://github.com/google/speech_intelligibility_index/issues
-Author-email: Malcolm Slaney <malcolmslaney@gmail.com>
+Author-email: Malcolm Slaney <speech-intelligibility-index-maintainers@googlegroups.com>
+License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.6
+Requires-Dist: absl-py
+Requires-Dist: matplotlib
+Requires-Dist: numpy
 Description-Content-Type: text/markdown
 
 A Python implementation of American National Standard ANSI S3.5-1997
 **"Methods for Calculation of the Speech Intelligibility Index"**
 This code is translated from Hannes Muesch's Matlab implementation.
 
 This package includes both Python/Numpy and Python/JAX implementations.
```

