# Comparing `tmp/py_build_cmake-0.1.9a3.tar.gz` & `tmp/py_build_cmake-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_build_cmake-0.1.9a3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "py_build_cmake-0.2.0a1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `py_build_cmake-0.1.9a3.tar` & `py_build_cmake-0.2.0a1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1086 2023-07-27 22:52:56.298855 py_build_cmake-0.1.9a3/LICENSE
--rw-r--r--   0        0        0     5273 2023-07-27 22:52:56.298855 py_build_cmake-0.1.9a3/README.md
--rw-r--r--   0        0        0     1446 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/pyproject.toml
--rw-r--r--   0        0        0      139 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/src/py_build_cmake/__init__.py
--rw-r--r--   0        0        0    33198 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/src/py_build_cmake/build.py
--rw-r--r--   0        0        0     9433 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/src/py_build_cmake/build_component.py
--rw-r--r--   0        0        0    10695 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/src/py_build_cmake/cli.py
--rw-r--r--   0        0        0     9339 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/src/py_build_cmake/cmake.py
--rw-r--r--   0        0        0     2490 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/src/py_build_cmake/cmd_runner.py
--rw-r--r--   0        0        0    10414 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/src/py_build_cmake/config.py
--rw-r--r--   0        0        0    34154 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/src/py_build_cmake/config_options.py
--rw-r--r--   0        0        0      306 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/src/py_build_cmake/datastructures.py
--rw-r--r--   0        0        0     4217 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/src/py_build_cmake/help/__init__.py
--rw-r--r--   0        0        0      180 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/src/py_build_cmake/help/__main__.py
--rw-r--r--   0        0        0        0 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/src/py_build_cmake/py.typed
--rw-r--r--   0        0        0    23844 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/src/py_build_cmake/pyproject_options.py
--rw-r--r--   0        0        0       89 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/src/py_build_cmake/quirks/__init__.py
--rw-r--r--   0        0        0     6530 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/src/py_build_cmake/quirks/config.py
--rw-r--r--   0        0        0     2612 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/src/py_build_cmake/tags.py
--rw-r--r--   0        0        0     6309 1970-01-01 00:00:00.000000 py_build_cmake-0.1.9a3/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-07-28 21:59:28.334363 py_build_cmake-0.2.0a1/LICENSE
+-rw-r--r--   0        0        0     6671 2023-07-28 21:59:28.334363 py_build_cmake-0.2.0a1/README.md
+-rw-r--r--   0        0        0     1446 2023-07-28 21:59:28.365551 py_build_cmake-0.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0      139 2023-07-28 21:59:28.365551 py_build_cmake-0.2.0a1/src/py_build_cmake/__init__.py
+-rw-r--r--   0        0        0    33266 2023-07-28 21:59:28.381224 py_build_cmake-0.2.0a1/src/py_build_cmake/build.py
+-rw-r--r--   0        0        0     9433 2023-07-28 21:59:28.381224 py_build_cmake-0.2.0a1/src/py_build_cmake/build_component.py
+-rw-r--r--   0        0        0    10695 2023-07-28 21:59:28.381224 py_build_cmake-0.2.0a1/src/py_build_cmake/cli.py
+-rw-r--r--   0        0        0     9339 2023-07-28 21:59:28.381224 py_build_cmake-0.2.0a1/src/py_build_cmake/cmake.py
+-rw-r--r--   0        0        0     2490 2023-07-28 21:59:28.381224 py_build_cmake-0.2.0a1/src/py_build_cmake/cmd_runner.py
+-rw-r--r--   0        0        0    10414 2023-07-28 21:59:28.381224 py_build_cmake-0.2.0a1/src/py_build_cmake/config.py
+-rw-r--r--   0        0        0    34154 2023-07-28 21:59:28.381224 py_build_cmake-0.2.0a1/src/py_build_cmake/config_options.py
+-rw-r--r--   0        0        0      306 2023-07-28 21:59:28.381224 py_build_cmake-0.2.0a1/src/py_build_cmake/datastructures.py
+-rw-r--r--   0        0        0     4217 2023-07-28 21:59:28.381224 py_build_cmake-0.2.0a1/src/py_build_cmake/help/__init__.py
+-rw-r--r--   0        0        0      180 2023-07-28 21:59:28.381224 py_build_cmake-0.2.0a1/src/py_build_cmake/help/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-28 21:59:28.381224 py_build_cmake-0.2.0a1/src/py_build_cmake/py.typed
+-rw-r--r--   0        0        0    25549 2023-07-28 21:59:28.381224 py_build_cmake-0.2.0a1/src/py_build_cmake/pyproject_options.py
+-rw-r--r--   0        0        0       89 2023-07-28 21:59:28.381224 py_build_cmake-0.2.0a1/src/py_build_cmake/quirks/__init__.py
+-rw-r--r--   0        0        0     6530 2023-07-28 21:59:28.381224 py_build_cmake-0.2.0a1/src/py_build_cmake/quirks/config.py
+-rw-r--r--   0        0        0     2612 2023-07-28 21:59:28.381224 py_build_cmake-0.2.0a1/src/py_build_cmake/tags.py
+-rw-r--r--   0        0        0     7693 1970-01-01 00:00:00.000000 py_build_cmake-0.2.0a1/PKG-INFO
```

### Comparing `py_build_cmake-0.1.9a3/LICENSE` & `py_build_cmake-0.2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.1.9a3/README.md` & `py_build_cmake-0.2.0a1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 
 Modern, [PEP 517](https://www.python.org/dev/peps/pep-0517/) compliant build
 backend for creating Python packages with extensions built using CMake.
 
 ## Features
 
  - Building and packaging C, C++ or Fortran extension modules for Python using CMake
- - Declarative configuration using `pyproject.toml` ([PEP 621](https://www.python.org/dev/peps/pep-0621/)), compatible with
-   [flit](https://github.com/pypa/flit)
+ - Declarative configuration using `pyproject.toml` ([PEP 621](https://www.python.org/dev/peps/pep-0621/))
  - Editable/development installations for Python modules ([PEP 660](https://www.python.org/dev/peps/pep-0660/))
- - Compatible with [pybind11](https://github.com/pybind/pybind11) and [nanobind](https://github.com/wjakob/nanobind)
+ - Easy integration with [pybind11](https://github.com/pybind/pybind11) and [nanobind](https://github.com/wjakob/nanobind), with stable ABI support
  - Stub generation for type checking and autocompletion
- - Customizable CMake configuration, build and installation options
- - Support for multiple installation configurations and components
- - Cross-compilation support
+ - Customizable CMake configuration, build, and installation options
+ - Support for multiple installation configurations and components, across different Wheel packages
+ - First-class cross-compilation support
+ - Reproducible source distributions
  - No dependency on [setuptools](https://github.com/pypa/setuptools)
  - Compatible with [cibuildwheel](https://github.com/pypa/cibuildwheel) for building Wheels
 
 ## Installation
 
 The py-build-cmake package is available on
 [PyPI](https://pypi.org/project/py-build-cmake/):
@@ -39,19 +39,23 @@
 
 Alternatively, use the [command-line interface](https://tttapa.github.io/py-build-cmake/CLI.html)
 to get the documentation for all supported options:
 ```sh
 py-build-cmake config format
 ```
 
+To get started quickly, have a look at the following section and the README in
+[`examples/minimal`](https://github.com/tttapa/py-build-cmake/tree/main/examples/minimal),
+which goes over the project structure and the configuration files you'll need.
+
 ## Usage
 
 If you don't have one already, add a `pyproject.toml` configuration file to your
-project's repository. Specify the metadata required by [PEP 621](https://www.python.org/dev/peps/pep-0621/),
-and tell py-build-cmake how to build your project. For example:
+project's repository. Specify the mandatory project metadata ([PyPA: Declaring project metadata](https://packaging.python.org/en/latest/specifications/declaring-project-metadata)),
+and tell py-build-cmake how to build your CMake project. For example:
 
 ```toml
 [project] # Project metadata
 name = "example-project"
 readme = "README.md"
 requires-python = ">=3.7"
 license = { "file" = "LICENSE" }
@@ -59,15 +63,15 @@
 keywords = ["some", "keywords"]
 classifiers = ["Topic :: Scientific/Engineering"]
 urls = { "Documentation" = "https://tttapa.github.io/py-build-cmake" }
 dependencies = ["numpy"]
 dynamic = ["version", "description"]
 
 [build-system] # How pip and other frontends should build this project
-requires = ["py-build-cmake~=0.1.9a3"]
+requires = ["py-build-cmake~=0.2.0a1"]
 build-backend = "py_build_cmake.build"
 
 [tool.py-build-cmake.module] # Where to find the Python module to package
 directory = "src-python"
 
 [tool.py-build-cmake.sdist] # What to include in source distributions
 include = ["CMakeLists.txt", "src/*"]
@@ -102,23 +106,33 @@
 
 As an introduction to py-build-cmake, see [`examples/minimal`](https://github.com/tttapa/py-build-cmake/tree/main/examples/minimal)
 for a detailed overview of the configuration files and the directory structure,
 using a very simple Python module as an example.  
 For a more advanced, real-world example, see [`examples/pybind11-project`](https://github.com/tttapa/py-build-cmake/tree/main/examples/pybind11-project)
 and [`examples/nanobind-project`](https://github.com/tttapa/py-build-cmake/tree/main/examples/nanobind-project).  
 If you are interested in packaging C/C++/Fortran programs using py-build-cmake,
-have a look at [`examples/minimal-program`](https://github.com/tttapa/py-build-cmake/tree/main/examples/minimal-program).
+have a look at [`examples/minimal-program`](https://github.com/tttapa/py-build-cmake/tree/main/examples/minimal-program).  
+See the [`examples`](https://github.com/tttapa/py-build-cmake/tree/main/examples) folder for a full list of examples.
 
 ## Projects using py-build-cmake
 
 If you need more examples, you can look at the following projects using
 py-build-cmake as their Python build backend:
 
 - [alpaqa](https://github.com/kul-optec/alpaqa/tree/develop)
 - [QPALM](https://github.com/kul-optec/QPALM)
 
+## Alternatives and related tools
+
+- [scikit-build-core](https://github.com/scikit-build/scikit-build-core): alternative CMake build backend, successor of [scikit-build](https://github.com/scikit-build/scikit-build)
+- [meson-python](https://github.com/mesonbuild/meson-python): Meson build backend
+- [flit](https://github.com/pypa/flit): pure-Python packaging tool and build backend
+- [hatchling](https://hatch.pypa.io/latest/config/build/#build-system): build backend of the [Hatch](https://hatch.pypa.io/latest/) project manager, supports build hooks
+- [poetry-core](https://python-poetry.org/docs/pyproject/#poetry-and-pep-517): pure-Python build backend for the [Poetry](https://python-poetry.org/) package manager
+- [crossenv](https://github.com/benfogle/crossenv): tool to trick `setuptools` into cross-compiling by monkey patching the `sysconfig` and `distutils` modules
+
 ## Planned features
 
  - [x] ~~macOS support~~
  - [x] ~~Entry point support~~
  - [ ] Namespace package support ([PEP 420](https://www.python.org/dev/peps/pep-0420/))
  - [ ] Doxygen and Sphinx support
```

### Comparing `py_build_cmake-0.1.9a3/pyproject.toml` & `py_build_cmake-0.2.0a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.1.9a3/src/py_build_cmake/build.py` & `py_build_cmake-0.2.0a1/src/py_build_cmake/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -636,26 +636,26 @@
 
     @staticmethod
     def convert_abi_tag(abi_tag: str, cmake_cfg: Optional[dict]):
         """Set the ABI tag to 'none' or 'abi3', depending on the config options
         specified by the user."""
         if not cmake_cfg:
             return 'none'
-        elif cmake_cfg['abi'] == 'auto':
+        elif cmake_cfg['python_extension_abi'] == 'auto':
             return abi_tag
-        elif cmake_cfg['abi'] == 'none':
+        elif cmake_cfg['python_extension_abi'] == 'none':
             return 'none'
-        elif cmake_cfg['abi'] == 'abi3':
+        elif cmake_cfg['python_extension_abi'] == 'abi3':
             # Only use abi3 if we're actually building for CPython
             m = re.match(r"^cp(\d+).*$", abi_tag)
             if m and int(m[1]) >= cmake_cfg['abi3_minimum_cpython_version']:
                 return 'abi3'
             return abi_tag
         else:
-            assert False, "Unsupported abi"
+            assert False, "Unsupported python_extension_abi"
 
     @staticmethod
     def convert_wheel_tags(tags, cfg):
         """Apply convert_abi_tag to each of the abi tags."""
         assert cfg.cmake
         tags = copy(tags)
         cmake_cfg, _ = _BuildBackend.get_cmake_configs(cfg)
```

### Comparing `py_build_cmake-0.1.9a3/src/py_build_cmake/build_component.py` & `py_build_cmake-0.2.0a1/src/py_build_cmake/build_component.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.1.9a3/src/py_build_cmake/cli.py` & `py_build_cmake-0.2.0a1/src/py_build_cmake/cli.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.1.9a3/src/py_build_cmake/cmake.py` & `py_build_cmake-0.2.0a1/src/py_build_cmake/cmake.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.1.9a3/src/py_build_cmake/cmd_runner.py` & `py_build_cmake-0.2.0a1/src/py_build_cmake/cmd_runner.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.1.9a3/src/py_build_cmake/config.py` & `py_build_cmake-0.2.0a1/src/py_build_cmake/config.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.1.9a3/src/py_build_cmake/config_options.py` & `py_build_cmake-0.2.0a1/src/py_build_cmake/config_options.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.1.9a3/src/py_build_cmake/help/__init__.py` & `py_build_cmake-0.2.0a1/src/py_build_cmake/help/__init__.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.1.9a3/src/py_build_cmake/pyproject_options.py` & `py_build_cmake-0.2.0a1/src/py_build_cmake/pyproject_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,33 +204,43 @@
         BoolConfigOption("pure_python",
                          "Indicate that this package contains no platform-"
                          "specific binaries, only Python scripts and other "
                          "platform-agnostic files. It causes the Wheel tags "
                          "to be set to `py3-none-any`.",
                          "pure_python = true",
                          default=DefaultValueValue(False)),
-        EnumConfigOption("abi",
+        EnumConfigOption("python_extension_abi",
                          "Override the default ABI tag for the Wheel package.\n"
+                         "For packages with a Python extension module that "
+                         "make use of the full Python C API, this option "
+                         "should be set to `auto`.\n"
                          "If your package does not contain Python extension "
                          "modules (e.g. because it only includes executables "
                          "to run as a subprocess, or only shared library files "
-                         "to be loaded using ctypes), you can set this to "
-                         "'none'.\n"
+                         "to be loaded using `ctypes`), you can set this to "
+                         "`none`.\n"
                          "If your package only includes Python extension "
                          "modules that use the CPython stable ABI, set this "
-                         "'abi3' (see also 'abi3_minimum_cpython_version' "
-                         "below).",
-                         "abi = 'none'",
+                         "`abi3` (see also `abi3_minimum_cpython_version` "
+                         "below).\n"
+                         "For details about platform compatibility tags, see "
+                         "the PyPA specification: https://packaging.python.org/"
+                         "en/latest/specifications/platform-compatibility-tags",
+                         "python_extension_abi = 'none'",
                          default=DefaultValueValue("auto"),
                          options=["auto", "none", "abi3"]),
         IntConfigOption("abi3_minimum_cpython_version",
-                        "If 'abi' is set to 'abi3', only use the stable "
-                        "CPython API for CPython version that are newer than "
-                        "'abi3_minimum_version'. Useful for nanobind, which "
-                        "supports the stable ABI for CPython 12 and later.",
+                        "If `python_extension_abi` is set to `abi3`, only use "
+                        "the stable CPython API for CPython version that are "
+                        "newer than `abi3_minimum_version`. Useful for "
+                        "nanobind, which supports the stable ABI for CPython "
+                        "12 and later.\n"
+                        "The Python version is encoded as a single integer, "
+                        "consisting of the major and minor version numbers, "
+                        "without a dot.",
                         "abi3_minimum_cpython_version = 312",
                         default=DefaultValueValue(32)),
     ])# yapf: disable
 
     # [tool.py-build-cmake.stubgen]
     stubgen = pbc.insert(
         ConfigOption(
@@ -288,28 +298,40 @@
         ))
     cross_pth = get_cross_path()
     cross.insert_multiple([
         EnumConfigOption('os',
                          "Operating system configuration to inherit from.",
                          options=["linux", "mac", "windows"]),
         StrConfigOption('implementation',
-                        "Identifier for the Python implementation.",
+                        "Identifier for the Python implementation.\n"
+                        "For details about platform compatibility tags, see "
+                        "the PyPA specification: https://packaging.python.org/"
+                        "en/latest/specifications/platform-compatibility-tags",
                         "implementation = 'cp' # CPython",
                         default=NoDefaultValue('same as current interpreter')),
         StrConfigOption('version',
-                        "Python version, major and minor, without dots.",
+                        "Python version, major and minor, without dots.\n"
+                        "For details about platform compatibility tags, see "
+                        "the PyPA specification: https://packaging.python.org/"
+                        "en/latest/specifications/platform-compatibility-tags",
                         "version = '310' # 3.10",
                         default=NoDefaultValue('same as current interpreter')),
         StrConfigOption('abi',
-                        "Python ABI.",
+                        "Python ABI.\n"
+                        "For details about platform compatibility tags, see "
+                        "the PyPA specification: https://packaging.python.org/"
+                        "en/latest/specifications/platform-compatibility-tags",
                         "abi = 'cp310'",
                         default=NoDefaultValue('same as current interpreter')),
         StrConfigOption('arch',
                         "Operating system and architecture (no dots or "
-                        "dashes, only underscores, all lowercase).",
+                        "dashes, only underscores, all lowercase).\n"
+                        "For details about platform compatibility tags, see "
+                        "the PyPA specification: https://packaging.python.org/"
+                        "en/latest/specifications/platform-compatibility-tags",
                         "arch = 'linux_x86_64'",
                         default=NoDefaultValue('same as current interpreter')),
         PathConfigOption('prefix',
                          "Root path of the Python installation. "
                          "Used to set the `Python3_ROOT_DIR` CMake hint, "
                          "see https://cmake.org/cmake/help/latest/module/"
                          "FindPython3.html#hints.",
```

### Comparing `py_build_cmake-0.1.9a3/src/py_build_cmake/quirks/config.py` & `py_build_cmake-0.2.0a1/src/py_build_cmake/quirks/config.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.1.9a3/src/py_build_cmake/tags.py` & `py_build_cmake-0.2.0a1/src/py_build_cmake/tags.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.1.9a3/PKG-INFO` & `py_build_cmake-0.2.0a1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-build-cmake
-Version: 0.1.9a3
+Version: 0.2.0a1
 Summary: Modern, PEP 517 compliant build backend for creating Python packages with
 Keywords: pep517,cmake
 Author-email: Pieter P <pieter.p.dev@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -33,22 +33,22 @@
 
 Modern, [PEP 517](https://www.python.org/dev/peps/pep-0517/) compliant build
 backend for creating Python packages with extensions built using CMake.
 
 ## Features
 
  - Building and packaging C, C++ or Fortran extension modules for Python using CMake
- - Declarative configuration using `pyproject.toml` ([PEP 621](https://www.python.org/dev/peps/pep-0621/)), compatible with
-   [flit](https://github.com/pypa/flit)
+ - Declarative configuration using `pyproject.toml` ([PEP 621](https://www.python.org/dev/peps/pep-0621/))
  - Editable/development installations for Python modules ([PEP 660](https://www.python.org/dev/peps/pep-0660/))
- - Compatible with [pybind11](https://github.com/pybind/pybind11) and [nanobind](https://github.com/wjakob/nanobind)
+ - Easy integration with [pybind11](https://github.com/pybind/pybind11) and [nanobind](https://github.com/wjakob/nanobind), with stable ABI support
  - Stub generation for type checking and autocompletion
- - Customizable CMake configuration, build and installation options
- - Support for multiple installation configurations and components
- - Cross-compilation support
+ - Customizable CMake configuration, build, and installation options
+ - Support for multiple installation configurations and components, across different Wheel packages
+ - First-class cross-compilation support
+ - Reproducible source distributions
  - No dependency on [setuptools](https://github.com/pypa/setuptools)
  - Compatible with [cibuildwheel](https://github.com/pypa/cibuildwheel) for building Wheels
 
 ## Installation
 
 The py-build-cmake package is available on
 [PyPI](https://pypi.org/project/py-build-cmake/):
@@ -66,19 +66,23 @@
 
 Alternatively, use the [command-line interface](https://tttapa.github.io/py-build-cmake/CLI.html)
 to get the documentation for all supported options:
 ```sh
 py-build-cmake config format
 ```
 
+To get started quickly, have a look at the following section and the README in
+[`examples/minimal`](https://github.com/tttapa/py-build-cmake/tree/main/examples/minimal),
+which goes over the project structure and the configuration files you'll need.
+
 ## Usage
 
 If you don't have one already, add a `pyproject.toml` configuration file to your
-project's repository. Specify the metadata required by [PEP 621](https://www.python.org/dev/peps/pep-0621/),
-and tell py-build-cmake how to build your project. For example:
+project's repository. Specify the mandatory project metadata ([PyPA: Declaring project metadata](https://packaging.python.org/en/latest/specifications/declaring-project-metadata)),
+and tell py-build-cmake how to build your CMake project. For example:
 
 ```toml
 [project] # Project metadata
 name = "example-project"
 readme = "README.md"
 requires-python = ">=3.7"
 license = { "file" = "LICENSE" }
@@ -86,15 +90,15 @@
 keywords = ["some", "keywords"]
 classifiers = ["Topic :: Scientific/Engineering"]
 urls = { "Documentation" = "https://tttapa.github.io/py-build-cmake" }
 dependencies = ["numpy"]
 dynamic = ["version", "description"]
 
 [build-system] # How pip and other frontends should build this project
-requires = ["py-build-cmake~=0.1.9a3"]
+requires = ["py-build-cmake~=0.2.0a1"]
 build-backend = "py_build_cmake.build"
 
 [tool.py-build-cmake.module] # Where to find the Python module to package
 directory = "src-python"
 
 [tool.py-build-cmake.sdist] # What to include in source distributions
 include = ["CMakeLists.txt", "src/*"]
@@ -129,24 +133,34 @@
 
 As an introduction to py-build-cmake, see [`examples/minimal`](https://github.com/tttapa/py-build-cmake/tree/main/examples/minimal)
 for a detailed overview of the configuration files and the directory structure,
 using a very simple Python module as an example.  
 For a more advanced, real-world example, see [`examples/pybind11-project`](https://github.com/tttapa/py-build-cmake/tree/main/examples/pybind11-project)
 and [`examples/nanobind-project`](https://github.com/tttapa/py-build-cmake/tree/main/examples/nanobind-project).  
 If you are interested in packaging C/C++/Fortran programs using py-build-cmake,
-have a look at [`examples/minimal-program`](https://github.com/tttapa/py-build-cmake/tree/main/examples/minimal-program).
+have a look at [`examples/minimal-program`](https://github.com/tttapa/py-build-cmake/tree/main/examples/minimal-program).  
+See the [`examples`](https://github.com/tttapa/py-build-cmake/tree/main/examples) folder for a full list of examples.
 
 ## Projects using py-build-cmake
 
 If you need more examples, you can look at the following projects using
 py-build-cmake as their Python build backend:
 
 - [alpaqa](https://github.com/kul-optec/alpaqa/tree/develop)
 - [QPALM](https://github.com/kul-optec/QPALM)
 
+## Alternatives and related tools
+
+- [scikit-build-core](https://github.com/scikit-build/scikit-build-core): alternative CMake build backend, successor of [scikit-build](https://github.com/scikit-build/scikit-build)
+- [meson-python](https://github.com/mesonbuild/meson-python): Meson build backend
+- [flit](https://github.com/pypa/flit): pure-Python packaging tool and build backend
+- [hatchling](https://hatch.pypa.io/latest/config/build/#build-system): build backend of the [Hatch](https://hatch.pypa.io/latest/) project manager, supports build hooks
+- [poetry-core](https://python-poetry.org/docs/pyproject/#poetry-and-pep-517): pure-Python build backend for the [Poetry](https://python-poetry.org/) package manager
+- [crossenv](https://github.com/benfogle/crossenv): tool to trick `setuptools` into cross-compiling by monkey patching the `sysconfig` and `distutils` modules
+
 ## Planned features
 
  - [x] ~~macOS support~~
  - [x] ~~Entry point support~~
  - [ ] Namespace package support ([PEP 420](https://www.python.org/dev/peps/pep-0420/))
  - [ ] Doxygen and Sphinx support
```

