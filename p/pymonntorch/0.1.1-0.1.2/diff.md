# Comparing `tmp/pymonntorch-0.1.1.tar.gz` & `tmp/pymonntorch-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymonntorch-0.1.1.tar", last modified: Sat May 27 06:20:10 2023, max compression
+gzip compressed data, was "pymonntorch-0.1.2.tar", last modified: Sat Jul 29 13:27:28 2023, max compression
```

## Comparing `pymonntorch-0.1.1.tar` & `pymonntorch-0.1.2.tar`

### file list

```diff
@@ -1,68 +1,79 @@
-drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-27 06:20:10.383475 pymonntorch-0.1.1/
--rw-r--r--   0 atenamohammadi   (501) staff       (20)      232 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/AUTHORS.rst
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     3592 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/CONTRIBUTING.rst
--rw-r--r--   0 atenamohammadi   (501) staff       (20)      261 2023-05-27 06:00:43.000000 pymonntorch-0.1.1/HISTORY.rst
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     1118 2023-05-27 06:00:43.000000 pymonntorch-0.1.1/LICENSE
--rw-r--r--   0 atenamohammadi   (501) staff       (20)      262 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/MANIFEST.in
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     4550 2023-05-27 06:20:10.383550 pymonntorch-0.1.1/PKG-INFO
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     3544 2023-05-27 06:18:55.000000 pymonntorch-0.1.1/README.rst
-drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-27 06:20:10.376985 pymonntorch-0.1.1/docs/
--rw-r--r--   0 atenamohammadi   (501) staff       (20)      612 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/docs/Makefile
-drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-27 06:20:10.377490 pymonntorch-0.1.1/docs/_images/
--rw-r--r--   0 atenamohammadi   (501) staff       (20)    42525 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/docs/_images/spike.png
--rw-r--r--   0 atenamohammadi   (501) staff       (20)   138598 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/docs/_images/voltage.png
--rw-r--r--   0 atenamohammadi   (501) staff       (20)       28 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/docs/authors.rst
--rwxr-xr-x   0 atenamohammadi   (501) staff       (20)     5024 2023-05-27 06:00:43.000000 pymonntorch-0.1.1/docs/conf.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)       33 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/docs/contributing.rst
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     1001 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/docs/documentation.rst
--rw-r--r--   0 atenamohammadi   (501) staff       (20)       28 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/docs/history.rst
--rw-r--r--   0 atenamohammadi   (501) staff       (20)      317 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/docs/index.rst
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     1130 2023-05-19 06:09:06.000000 pymonntorch-0.1.1/docs/installation.rst
--rw-r--r--   0 atenamohammadi   (501) staff       (20)      809 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/docs/make.bat
--rw-r--r--   0 atenamohammadi   (501) staff       (20)       27 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/docs/readme.rst
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     5803 2023-05-19 06:09:57.000000 pymonntorch-0.1.1/docs/tutorial.rst
-drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-27 06:20:10.378321 pymonntorch-0.1.1/pymonntorch/
-drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-27 06:20:10.379595 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/
-drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-27 06:20:10.380166 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/Basics/
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     5791 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/Basics/BasicHomeostasis.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)      964 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/Basics/Normalization.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)        0 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/Basics/__init__.py
-drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-27 06:20:10.381013 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/EulerEquationModules/
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     1426 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/EulerEquationModules/Equation.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)      865 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/EulerEquationModules/EulerClock.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     1082 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/EulerEquationModules/Helper.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     1695 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/EulerEquationModules/VariableInitializer.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)        0 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/EulerEquationModules/__init__.py
-drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-27 06:20:10.381339 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/Recorder/
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     7793 2023-05-27 06:00:43.000000 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/Recorder/Recorder.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)        0 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/Recorder/__init__.py
-drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-27 06:20:10.381654 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/Structure/
--rw-r--r--   0 atenamohammadi   (501) staff       (20)    11399 2023-05-27 06:00:43.000000 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/Structure/Structure.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)        0 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/Structure/__init__.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)        0 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/__init__.py
-drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-27 06:20:10.382955 pymonntorch-0.1.1/pymonntorch/NetworkCore/
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     8262 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/NetworkCore/AnalysisModule.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)    10859 2023-05-27 06:00:43.000000 pymonntorch-0.1.1/pymonntorch/NetworkCore/Base.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     7436 2023-05-27 06:00:43.000000 pymonntorch-0.1.1/pymonntorch/NetworkCore/Behavior.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)    14360 2023-05-27 06:00:43.000000 pymonntorch-0.1.1/pymonntorch/NetworkCore/Network.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)    14984 2023-05-27 06:00:43.000000 pymonntorch-0.1.1/pymonntorch/NetworkCore/NeuronGroup.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)    12458 2023-05-27 06:00:43.000000 pymonntorch-0.1.1/pymonntorch/NetworkCore/SynapseGroup.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     4194 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/NetworkCore/TaggableObject.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)        0 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/NetworkCore/__init__.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)      967 2023-05-27 06:00:43.000000 pymonntorch-0.1.1/pymonntorch/__init__.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)      411 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/cli.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)       19 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/pymonntorch.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)      459 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/utils.py
-drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-27 06:20:10.379446 pymonntorch-0.1.1/pymonntorch.egg-info/
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     4550 2023-05-27 06:20:10.000000 pymonntorch-0.1.1/pymonntorch.egg-info/PKG-INFO
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     1721 2023-05-27 06:20:10.000000 pymonntorch-0.1.1/pymonntorch.egg-info/SOURCES.txt
--rw-r--r--   0 atenamohammadi   (501) staff       (20)        1 2023-05-27 06:20:10.000000 pymonntorch-0.1.1/pymonntorch.egg-info/dependency_links.txt
--rw-r--r--   0 atenamohammadi   (501) staff       (20)       53 2023-05-27 06:20:10.000000 pymonntorch-0.1.1/pymonntorch.egg-info/entry_points.txt
--rw-r--r--   0 atenamohammadi   (501) staff       (20)        1 2023-05-09 14:25:31.000000 pymonntorch-0.1.1/pymonntorch.egg-info/not-zip-safe
--rw-r--r--   0 atenamohammadi   (501) staff       (20)       28 2023-05-27 06:20:10.000000 pymonntorch-0.1.1/pymonntorch.egg-info/requires.txt
--rw-r--r--   0 atenamohammadi   (501) staff       (20)       12 2023-05-27 06:20:10.000000 pymonntorch-0.1.1/pymonntorch.egg-info/top_level.txt
--rw-r--r--   0 atenamohammadi   (501) staff       (20)      428 2023-05-27 06:20:10.383815 pymonntorch-0.1.1/setup.cfg
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     1476 2023-05-27 06:00:43.000000 pymonntorch-0.1.1/setup.py
-drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-27 06:20:10.383245 pymonntorch-0.1.1/tests/
--rw-r--r--   0 atenamohammadi   (501) staff       (20)       41 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/tests/__init__.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     4169 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/tests/test_pymonntorch.py
+drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-07-29 13:27:28.908777 pymonntorch-0.1.2/
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)      356 2023-06-18 07:11:03.000000 pymonntorch-0.1.2/AUTHORS.rst
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     3592 2023-05-09 07:39:39.000000 pymonntorch-0.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)      261 2023-05-27 06:00:43.000000 pymonntorch-0.1.2/HISTORY.rst
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     1118 2023-05-27 06:00:43.000000 pymonntorch-0.1.2/LICENSE
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)      262 2023-05-09 07:39:39.000000 pymonntorch-0.1.2/MANIFEST.in
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     4705 2023-07-29 13:27:28.908848 pymonntorch-0.1.2/PKG-INFO
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     3699 2023-07-29 13:15:13.000000 pymonntorch-0.1.2/README.rst
+drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-07-29 13:27:28.903727 pymonntorch-0.1.2/docs/
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)      612 2023-05-09 07:39:39.000000 pymonntorch-0.1.2/docs/Makefile
+drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-07-29 13:27:28.900665 pymonntorch-0.1.2/docs/_build/
+drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-07-29 13:27:28.900789 pymonntorch-0.1.2/docs/_build/html/
+drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-07-29 13:27:28.904122 pymonntorch-0.1.2/docs/_build/html/_images/
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)    63873 2023-06-18 06:56:13.000000 pymonntorch-0.1.2/docs/_build/html/_images/pymoNNtorch-logo-t-256.png
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)    42525 2023-05-09 07:39:39.000000 pymonntorch-0.1.2/docs/_build/html/_images/spike.png
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)   138598 2023-05-09 07:39:39.000000 pymonntorch-0.1.2/docs/_build/html/_images/voltage.png
+drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-07-29 13:27:28.904524 pymonntorch-0.1.2/docs/_build/html/_static/
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)      286 2023-06-18 07:29:28.000000 pymonntorch-0.1.2/docs/_build/html/_static/file.png
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)       90 2023-06-18 07:29:28.000000 pymonntorch-0.1.2/docs/_build/html/_static/minus.png
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)       90 2023-06-18 07:29:28.000000 pymonntorch-0.1.2/docs/_build/html/_static/plus.png
+drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-07-29 13:27:28.904883 pymonntorch-0.1.2/docs/_images/
+-rw-------   0 atenamohammadi   (501) staff       (20)    63873 2023-06-18 06:56:13.000000 pymonntorch-0.1.2/docs/_images/pymoNNtorch-logo-t-256.png
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)    42525 2023-05-09 07:39:39.000000 pymonntorch-0.1.2/docs/_images/spike.png
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)   138598 2023-05-09 07:39:39.000000 pymonntorch-0.1.2/docs/_images/voltage.png
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)       28 2023-05-09 07:39:39.000000 pymonntorch-0.1.2/docs/authors.rst
+-rwxr-xr-x   0 atenamohammadi   (501) staff       (20)     5160 2023-07-29 13:15:13.000000 pymonntorch-0.1.2/docs/conf.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)       33 2023-05-09 07:39:39.000000 pymonntorch-0.1.2/docs/contributing.rst
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     1001 2023-05-09 07:39:39.000000 pymonntorch-0.1.2/docs/documentation.rst
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)       28 2023-05-09 07:39:39.000000 pymonntorch-0.1.2/docs/history.rst
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)      472 2023-07-29 13:15:13.000000 pymonntorch-0.1.2/docs/index.rst
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     1130 2023-05-19 06:09:06.000000 pymonntorch-0.1.2/docs/installation.rst
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)      809 2023-05-09 07:39:39.000000 pymonntorch-0.1.2/docs/make.bat
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)       27 2023-05-09 07:39:39.000000 pymonntorch-0.1.2/docs/readme.rst
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     5800 2023-06-18 06:38:34.000000 pymonntorch-0.1.2/docs/tutorial.rst
+drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-07-29 13:27:28.905376 pymonntorch-0.1.2/pymonntorch/
+drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-07-29 13:27:28.906247 pymonntorch-0.1.2/pymonntorch/NetworkBehavior/
+drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-07-29 13:27:28.906564 pymonntorch-0.1.2/pymonntorch/NetworkBehavior/Basics/
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     8022 2023-07-29 13:15:13.000000 pymonntorch-0.1.2/pymonntorch/NetworkBehavior/Basics/BasicHomeostasis.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     1165 2023-07-29 13:15:13.000000 pymonntorch-0.1.2/pymonntorch/NetworkBehavior/Basics/Normalization.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)        0 2023-05-09 07:39:39.000000 pymonntorch-0.1.2/pymonntorch/NetworkBehavior/Basics/__init__.py
+drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-07-29 13:27:28.907120 pymonntorch-0.1.2/pymonntorch/NetworkBehavior/EulerEquationModules/
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     1565 2023-07-29 13:15:13.000000 pymonntorch-0.1.2/pymonntorch/NetworkBehavior/EulerEquationModules/Equation.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)      973 2023-07-29 13:15:13.000000 pymonntorch-0.1.2/pymonntorch/NetworkBehavior/EulerEquationModules/EulerClock.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     1082 2023-05-09 07:39:39.000000 pymonntorch-0.1.2/pymonntorch/NetworkBehavior/EulerEquationModules/Helper.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     1895 2023-07-29 13:15:13.000000 pymonntorch-0.1.2/pymonntorch/NetworkBehavior/EulerEquationModules/VariableInitializer.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)        0 2023-05-09 07:39:39.000000 pymonntorch-0.1.2/pymonntorch/NetworkBehavior/EulerEquationModules/__init__.py
+drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-07-29 13:27:28.907315 pymonntorch-0.1.2/pymonntorch/NetworkBehavior/Recorder/
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     8222 2023-07-29 13:15:13.000000 pymonntorch-0.1.2/pymonntorch/NetworkBehavior/Recorder/Recorder.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)        0 2023-05-09 07:39:39.000000 pymonntorch-0.1.2/pymonntorch/NetworkBehavior/Recorder/__init__.py
+drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-07-29 13:27:28.907515 pymonntorch-0.1.2/pymonntorch/NetworkBehavior/Structure/
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)    11701 2023-07-29 13:15:13.000000 pymonntorch-0.1.2/pymonntorch/NetworkBehavior/Structure/Structure.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)        0 2023-05-09 07:39:39.000000 pymonntorch-0.1.2/pymonntorch/NetworkBehavior/Structure/__init__.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)        0 2023-05-09 07:39:39.000000 pymonntorch-0.1.2/pymonntorch/NetworkBehavior/__init__.py
+drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-07-29 13:27:28.908494 pymonntorch-0.1.2/pymonntorch/NetworkCore/
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     8262 2023-05-09 07:39:39.000000 pymonntorch-0.1.2/pymonntorch/NetworkCore/AnalysisModule.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)    12346 2023-06-18 06:38:34.000000 pymonntorch-0.1.2/pymonntorch/NetworkCore/Base.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     8040 2023-07-29 13:15:13.000000 pymonntorch-0.1.2/pymonntorch/NetworkCore/Behavior.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)    14360 2023-05-27 06:00:43.000000 pymonntorch-0.1.2/pymonntorch/NetworkCore/Network.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)    14985 2023-06-18 06:38:34.000000 pymonntorch-0.1.2/pymonntorch/NetworkCore/NeuronGroup.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)    12458 2023-05-27 06:00:43.000000 pymonntorch-0.1.2/pymonntorch/NetworkCore/SynapseGroup.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     4194 2023-05-09 07:39:39.000000 pymonntorch-0.1.2/pymonntorch/NetworkCore/TaggableObject.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)        0 2023-05-09 07:39:39.000000 pymonntorch-0.1.2/pymonntorch/NetworkCore/__init__.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)      967 2023-05-27 06:00:43.000000 pymonntorch-0.1.2/pymonntorch/__init__.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)      411 2023-05-09 07:39:39.000000 pymonntorch-0.1.2/pymonntorch/cli.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)       19 2023-05-09 07:39:39.000000 pymonntorch-0.1.2/pymonntorch/pymonntorch.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)      459 2023-05-09 07:39:39.000000 pymonntorch-0.1.2/pymonntorch/utils.py
+drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-07-29 13:27:28.906133 pymonntorch-0.1.2/pymonntorch.egg-info/
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     4705 2023-07-29 13:27:28.000000 pymonntorch-0.1.2/pymonntorch.egg-info/PKG-INFO
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     1988 2023-07-29 13:27:28.000000 pymonntorch-0.1.2/pymonntorch.egg-info/SOURCES.txt
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)        1 2023-07-29 13:27:28.000000 pymonntorch-0.1.2/pymonntorch.egg-info/dependency_links.txt
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)       53 2023-07-29 13:27:28.000000 pymonntorch-0.1.2/pymonntorch.egg-info/entry_points.txt
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)        1 2023-07-29 13:27:28.000000 pymonntorch-0.1.2/pymonntorch.egg-info/not-zip-safe
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)       28 2023-07-29 13:27:28.000000 pymonntorch-0.1.2/pymonntorch.egg-info/requires.txt
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)       12 2023-07-29 13:27:28.000000 pymonntorch-0.1.2/pymonntorch.egg-info/top_level.txt
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)      428 2023-07-29 13:27:28.909468 pymonntorch-0.1.2/setup.cfg
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     1476 2023-07-29 13:18:50.000000 pymonntorch-0.1.2/setup.py
+drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-07-29 13:27:28.908681 pymonntorch-0.1.2/tests/
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)       41 2023-05-09 07:39:39.000000 pymonntorch-0.1.2/tests/__init__.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     4169 2023-05-09 07:39:39.000000 pymonntorch-0.1.2/tests/test_pymonntorch.py
```

### Comparing `pymonntorch-0.1.1/CONTRIBUTING.rst` & `pymonntorch-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pymonntorch-0.1.1/LICENSE` & `pymonntorch-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymonntorch-0.1.1/PKG-INFO` & `pymonntorch-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonntorch
-Version: 0.1.1
+Version: 0.1.2
 Summary: PymoNNtorch is a Pytorch version of PymoNNto
 Home-page: https://github.com/cnrl/PymoNNtorch
 Author: Computational Neuroscience Research Laboratory
 Author-email: ashenatena@gmail.com
 License: MIT license
 Keywords: pymonntorch
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -19,14 +19,20 @@
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ===========
 PymoNNtorch
 ===========
 
+.. image:: https://raw.githubusercontent.com/cnrl/PymoNNtorch/main/docs/_images/pymoNNtorch-logo-t-256.png
+    :width: 256
+    :alt: pymonntorch logo
+
+|
+
 
 .. image:: https://img.shields.io/pypi/v/pymonntorch.svg
         :target: https://pypi.python.org/pypi/pymonntorch
 
 .. .. image:: https://img.shields.io/travis/cnrl/pymonntorch.svg
 ..         :target: https://travis-ci.com/cnrl/pymonntorch
 
@@ -126,14 +132,15 @@
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 It changes the codebase of `PymoNNto <https://github.com/trieschlab/PymoNNto>`_ to use ``torch`` rather than ``numpy`` and ``tensorflow numpy``.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
+
 =======
 History
 =======
 
 0.1.1 (2023-05-26)
 ------------------
```

### Comparing `pymonntorch-0.1.1/README.rst` & `pymonntorch-0.1.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 ===========
 PymoNNtorch
 ===========
 
+.. image:: https://raw.githubusercontent.com/cnrl/PymoNNtorch/main/docs/_images/pymoNNtorch-logo-t-256.png
+    :width: 256
+    :alt: pymonntorch logo
+
+|
+
 
 .. image:: https://img.shields.io/pypi/v/pymonntorch.svg
         :target: https://pypi.python.org/pypi/pymonntorch
 
 .. .. image:: https://img.shields.io/travis/cnrl/pymonntorch.svg
 ..         :target: https://travis-ci.com/cnrl/pymonntorch
 
@@ -103,8 +109,8 @@
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 It changes the codebase of `PymoNNto <https://github.com/trieschlab/PymoNNto>`_ to use ``torch`` rather than ``numpy`` and ``tensorflow numpy``.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
-.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
```

### Comparing `pymonntorch-0.1.1/docs/Makefile` & `pymonntorch-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pymonntorch-0.1.1/docs/_images/spike.png` & `pymonntorch-0.1.2/docs/_build/html/_images/spike.png`

 * *Files identical despite different names*

### Comparing `pymonntorch-0.1.1/docs/_images/voltage.png` & `pymonntorch-0.1.2/docs/_build/html/_images/voltage.png`

 * *Files identical despite different names*

### Comparing `pymonntorch-0.1.1/docs/conf.py` & `pymonntorch-0.1.2/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,16 +90,20 @@
 # theme further.  For a list of options available for each theme, see the
 # documentation.
 #
 html_theme_options = {
     "show_nav_level": 2,
     "show_toc_level": 2,
     "collapse_navigation": False,
+    "logo_only": False,
 }
 
+
+html_logo = "https://raw.githubusercontent.com/cnrl/PymoNNtorch/main/docs/_images/pymoNNtorch-logo-t-256.png"
+
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
 
 
 # -- Options for HTMLHelp output ---------------------------------------
```

### Comparing `pymonntorch-0.1.1/docs/documentation.rst` & `pymonntorch-0.1.2/docs/documentation.rst`

 * *Files identical despite different names*

### Comparing `pymonntorch-0.1.1/docs/installation.rst` & `pymonntorch-0.1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pymonntorch-0.1.1/docs/make.bat` & `pymonntorch-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pymonntorch-0.1.1/docs/tutorial.rst` & `pymonntorch-0.1.2/docs/tutorial.rst`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
     from pymonntorch import *
 
     net = Network()
     ng = NeuronGroup(net=net, size=1000, behavior={})
     syn = SynapseGroup(net=net, src=ng, dst=ng, tag='GLUTAMATE')
 
-So far, ``ng`` has been added to network ``net`` and synaptic connection has been defined to connect ``ng`` to itself, i.e. both afferent and efferent synapses of ``ng`` are ``syn``. By default, each network and its components are created on CPU and the data type of any tensor inside the objects is set to ``torch.float32``. Pass an argument ``settings`` to the ``Network`` to change these default setups. ``settings`` is a dictionary with keys ``device`` and ``def_dtype`` which indicate the device and data type of everything within the network, respectively.
+So far, ``ng`` has been added to network ``net`` and synaptic connection has been defined to connect ``ng`` to itself, i.e. both afferent and efferent synapses of ``ng`` are ``syn``. By default, each network and its components are created on CPU and the data type of any tensor inside the objects is set to ``torch.float32``. Pass an argument ``settings`` to the ``Network`` to change these default setups. ``settings`` is a dictionary with keys ``device`` and ``dtype`` which indicate the device and data type of everything within the network, respectively.
 
 To have a functioning network, we can write ``Behavior`` (s) for different network objects to define dynamics and attributes for them. To do so, we can proceed as follows: ::
 
     class BasicBehavior(Behavior):  # Any user-defined behavior should inherit pymonntorch.NetworkCore.Behavior
         # This behavior is defining dynamics for NeuronGroups
         def initialize(self, neurons):  # override this method to define and initialize attributes. This is called upon calling Network's initialize method.
 
@@ -103,8 +103,8 @@
     plt.title('Raster Plot')
     plt.show()
 
 .. image:: _images/voltage.png
     :width: 600
 
 .. image:: _images/spike.png
-    :width: 600
+    :width: 600
```

### Comparing `pymonntorch-0.1.1/pymonntorch/NetworkBehavior/EulerEquationModules/Equation.py` & `pymonntorch-0.1.2/pymonntorch/NetworkBehavior/EulerEquationModules/Equation.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,17 @@
     remove_units,
 )
 from sympy import symbols
 import torch
 
 
 class Equation(Behavior):
+    def __init__(self, *args, eq=None, step_size="1*ms", **kwargs):
+        super().__init__(*args, eq=eq, step_size=step_size, **kwargs)
+
     def initialize(self, neurons):
         super().initialize(neurons)
         n = neurons
         self.add_tag("EquationModule")
         self.step_size = self.parameter("step_size", "1*ms", neurons)
         eq_parts = eq_split(self.parameter("eq", None))
```

### Comparing `pymonntorch-0.1.1/pymonntorch/NetworkBehavior/EulerEquationModules/EulerClock.py` & `pymonntorch-0.1.2/pymonntorch/NetworkBehavior/EulerEquationModules/EulerClock.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from pymonntorch.NetworkCore.Behavior import Behavior
 
 from sympy.physics.units import convert_to, second, seconds
 
 
 class Clock(Behavior):
+    def __init__(self, *args, step="1*ms", **kwargs):
+        super().__init__(*args, step=step, **kwargs)
+
     def initialize(self, neuron_or_network):
         super().initialize(neuron_or_network)
 
         self.add_tag("Clock")
 
         neuron_or_network.clock_step_size = float(
             convert_to(eval(self.parameter("step", "1*ms")), seconds) / second
```

### Comparing `pymonntorch-0.1.1/pymonntorch/NetworkBehavior/EulerEquationModules/Helper.py` & `pymonntorch-0.1.2/pymonntorch/NetworkBehavior/EulerEquationModules/Helper.py`

 * *Files identical despite different names*

### Comparing `pymonntorch-0.1.1/pymonntorch/NetworkBehavior/EulerEquationModules/VariableInitializer.py` & `pymonntorch-0.1.2/pymonntorch/NetworkBehavior/EulerEquationModules/VariableInitializer.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 from pymonntorch.NetworkBehavior.EulerEquationModules.Helper import (
     eq_split,
     remove_units,
 )
 
 
 class Variable(Behavior):
+    def __init__(self, *args, eq=None, **kwargs):
+        super().__init__(*args, eq=eq, **kwargs)
+
     def initialize(self, neurons):
         super().initialize(neurons)
 
         n = neurons
 
         eq_parts = eq_split(self.parameter("eq", None))
 
@@ -31,14 +34,17 @@
     def forward(self, n):
         setattr(
             n, self.var_name, getattr(n, self.var_name + "_new")
         )  # apply the new value to variable
 
 
 class SynapseVariable(Behavior):
+    def __init__(self, *args, eq=None, **kwargs):
+        super().__init__(*args, eq=eq, **kwargs)
+
     def initialize(self, synapse):
         s = synapse
 
         eq_parts = eq_split(self.parameter("eq", None))
 
         if eq_parts[1] == "=" and len(eq_parts) >= 3:
             self.var_name = eq_parts[0]
```

### Comparing `pymonntorch-0.1.1/pymonntorch/NetworkBehavior/Recorder/Recorder.py` & `pymonntorch-0.1.2/pymonntorch/NetworkBehavior/Recorder/Recorder.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,34 @@
         auto_annotate (bool): This parameter specifies whether the variable names include the \
             network object prefix (neurons/synapse/n/s) or not. The default is True.
     """
 
     initialize_last = True
     visualization_module_outputs = []
 
+    def __init__(
+        self,
+        *args,
+        variables=None,
+        gap_width=0,
+        max_length=None,
+        auto_annotate=True,
+        tag=None,
+        **kwargs,
+    ):
+        super().__init__(
+            *args,
+            variables=variables,
+            gap_width=gap_width,
+            max_length=max_length,
+            auto_annotate=auto_annotate,
+            tag=tag,
+            **kwargs,
+        )
+
     def initialize(self, object):
         super().initialize(object)
 
         variables = self.parameter("variables", [])
         if variables == []:
             variables = self.parameter("arg_0", [])
         if isinstance(variables, str):
```

### Comparing `pymonntorch-0.1.1/pymonntorch/NetworkBehavior/Structure/Structure.py` & `pymonntorch-0.1.2/pymonntorch/NetworkBehavior/Structure/Structure.py`

 * *Files 8% similar despite different names*

```diff
@@ -104,14 +104,26 @@
         width (int): Width of the `NeuronGroup`. The default is 1.
         height (int): Height of the `NeuronGroup`. The default is 1.
         depth (int): Depth of the `NeuronGroup`. The default is 1.
     """
 
     initialize_on_init = True
 
+    def __init__(
+        self, *args, depth=1, height=1, width=1, input_patterns=None, **kwargs
+    ):
+        super().__init__(
+            *args,
+            depth=depth,
+            height=height,
+            width=width,
+            input_patterns=input_patterns,
+            **kwargs,
+        )
+
     def set_position(self, width, height, depth):
         """Set the coordinate of neurons by setting vectors `x`, `y`, and `z`.
 
         Args:
             width (int): Width of the neurons.
             height (int): Height of the neurons.
             depth (int): Depth of the neurons.
```

### Comparing `pymonntorch-0.1.1/pymonntorch/NetworkCore/AnalysisModule.py` & `pymonntorch-0.1.2/pymonntorch/NetworkCore/AnalysisModule.py`

 * *Files identical despite different names*

### Comparing `pymonntorch-0.1.1/pymonntorch/NetworkCore/Base.py` & `pymonntorch-0.1.2/pymonntorch/NetworkCore/Base.py`

 * *Files 10% similar despite different names*

```diff
@@ -207,15 +207,15 @@
         return mat
 
     def _get_mat(self, mode, dim, scale=None, density=None, plot=False, dtype=None):
         """Get a tensor with object's dimensionality.
 
         The tensor can be initialized in different modes. List of possible values for mode includes:
         - "random" or "rand" or "rnd" or "uniform": Uniformly distributed random numbers in range [0, 1).
-        - "normal": Normally distributed random numbers with zero mean and unit variance.
+        - "normal(mean=a, std=b)": Normally distributed random numbers with `a` as mean and `b` as standard derivation.
         - "ones": Tensor filled with ones.
         - "zeros": Tensor filled with zeros.
         - A single number: Tensor filled with that number.
         - You can also use any function from torch package for this purpose.
 
         Args:
             mode (str): Mode to be used to initialize tensor.
@@ -223,34 +223,43 @@
             scale (float): Scale of the tensor. The default is None (i.e. No scaling is applied).
             density (float): Density of the tensor. The default is None (i.e. dense tensor).
             plot (bool): If true, the histogram of the tensor will be plotted. The default is False.
             dtype (str or type): Data type of the tensor. If None, `def_dtype` will be used.
 
         Returns:
             torch.Tensor: The initialized tensor."""
-        if mode not in self._mat_eval_dict:
-            prefix = "torch."
 
-            if mode == "random" or mode == "rand" or mode == "rnd" or mode == "uniform":
-                mode = "rand"
+        dtype = self.def_dtype if dtype is None else dtype
 
-            if type(mode) == int or type(mode) == float:
-                mode = "ones()*" + str(mode)
+        if mode not in self._mat_eval_dict:
+            prefix = "torch."
+            ev_str = mode
 
-            mode = prefix + mode
-            if "(" not in mode and ")" not in mode:
-                mode += "()"
-
-            if dtype is not None:
-                mode = mode.replace(")", f",dtype={dtype})")
-            else:
-                mode = mode.replace(")", f",dtype={self.def_dtype})")
+            if (
+                ev_str == "random"
+                or ev_str == "rand"
+                or ev_str == "rnd"
+                or ev_str == "uniform"
+            ):
+                ev_str = "rand"
+
+            if type(ev_str) == int or type(ev_str) == float:
+                ev_str = "ones()*" + str(ev_str)
+
+            ev_str = prefix + ev_str
+            if "(" not in ev_str and ")" not in ev_str:
+                ev_str += "()"
+
+            a1 = "size=dim,device=self.device,dtype=dtype)"
+
+            # check for positional argument
+            if ev_str[ev_str.index("(") + 1 : ev_str.index(")")].strip():
+                a1 = "," + a1
 
-            a1 = "dim,device=" + f"'{self.device}'"
-            ev_str = mode.replace("(", "(" + a1)
+            ev_str = ev_str.replace(")", a1)
             self._mat_eval_dict[mode] = compile(ev_str, "<string>", "eval")
 
         result = eval(self._mat_eval_dict[mode])
 
         if density is not None:
             if type(density) == int or type(density) == float:
                 result = result * (torch.rand(dim, device=self.device) <= density)
@@ -266,14 +275,38 @@
             import matplotlib.pyplot as plt
 
             plt.hist(result.flatten().to("cpu"), bins=30)
             plt.show()
 
         return result
 
+    def tensor(self, mode, dim, scale=None, density=None, dtype=None):
+        """Get a tensor with desired dimensionality.
+
+        The tensor can be initialized in different modes. List of possible values for mode includes:
+        - "random" or "rand" or "rnd" or "uniform": Uniformly distributed random numbers in range [0, 1).
+        - "normal(mean=a, std=b)": Normally distributed random numbers with `a` as mean and `b` as standard derivation.
+        - "ones": Tensor filled with ones.
+        - "zeros": Tensor filled with zeros.
+        - A single number: Tensor filled with that number.
+        - You can also use any function from torch package for this purpose.
+
+        Args:
+            mode (str): Mode to be used to initialize tensor.
+            dim (int or tuple of int): Dimensionality of the tensor.
+            scale (float): Scale of the tensor. The default is None (i.e. No scaling is applied).
+            density (float): Density of the tensor. The default is None (i.e. dense tensor).
+            dtype (str or type): Data type of the tensor. If None, `def_dtype` will be used.
+
+        Returns:
+            torch.Tensor: The initialized tensor."""
+        return self._get_mat(
+            mode=mode, dim=dim, scale=scale, density=density, dtype=dtype
+        )
+
     def get_buffer_mat(self, dim, size, **kwargs):
         """Get a buffer of specific size with object's dimensionality.
 
         Args:
             dim (int or tuple of int): Dimensionality of the buffer.
             size (int): Size of the buffer.
             kwargs (dict): Keyword arguments to be passed to the initialization function.
```

### Comparing `pymonntorch-0.1.1/pymonntorch/NetworkCore/Behavior.py` & `pymonntorch-0.1.2/pymonntorch/NetworkCore/Behavior.py`

 * *Files 5% similar despite different names*

```diff
@@ -131,40 +131,43 @@
     def parameter(
         self,
         key,
         default,
         object=None,
         do_not_diversify=False,
         search_other_behaviors=False,
+        tensor=False,
         required=False,
     ):
         """Gets the value of an attribute.
 
         Args:
             key (str): Name of the attribute.
             default (any): Default value of the attribute.
             object (NetworkObject): The object possessing the behavior.
             do_not_diversify (bool): Whether to diversify the attribute. The default is False.
             search_other_behaviors (bool): Whether to search for the attribute in other behaviors of the object. The default is False.
+            tensor (bool): Whether to make a tensor out of value. Suitable for list and numbers.
             required (bool): Whether the attribute is required. The default is False.
 
         Returns:
             any: The value of the attribute.
         """
-        if required and key not in self.init_kwargs:
+        if required and self.init_kwargs.get(key, None) is None:
             print(
                 "Warning:",
                 key,
-                "has to be specified for the behavior to run properly.",
+                "has to be specified for the behavior with a non None value to run properly.",
                 self,
             )
 
         self.used_attr_keys.append(key)
 
         result = self.init_kwargs.get(key, default)
+        result = default if result is None else result
 
         if (
             key not in self.init_kwargs
             and object is not None
             and search_other_behaviors
         ):
             for b in object.behaviors:
@@ -176,14 +179,23 @@
 
         if type(result) is str and default is not None:
             if "%" in result and is_number(result.replace("%", "")):
                 result = str(float(result.replace("%", "")) / 100.0)
 
             result = type(default)(result)
 
+        if tensor and result is not None:
+            if object is None:
+                raise RuntimeError(
+                    f'To turn parameter value of key "{key}" to a tensor, object should not be None.'
+                )
+            result = torch.tensor(result, device=object.device)
+            if result.is_floating_point():
+                result = result.to(dtype=object.def_dtype)
+
         return result
 
     def is_empty_iteration_function(self):
         """Checks whether a function does anything or not.
 
         used to stop calling behaviors with empty forward method.
         """
```

### Comparing `pymonntorch-0.1.1/pymonntorch/NetworkCore/Network.py` & `pymonntorch-0.1.2/pymonntorch/NetworkCore/Network.py`

 * *Files identical despite different names*

### Comparing `pymonntorch-0.1.1/pymonntorch/NetworkCore/NeuronGroup.py` & `pymonntorch-0.1.2/pymonntorch/NetworkCore/NeuronGroup.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             plot (bool): If true, the histogram of the tensor will be plotted. The default is False.
             dtype (str or type): Data type of the tensor. If None, `def_dtype` will be used.
 
         Returns:
             torch.Tensor: The initialized tensor."""
         return self._get_mat(
             mode=mode,
-            dim=(self.size),
+            dim=(self.size,),
             scale=scale,
             density=density,
             plot=plot,
             dtype=dtype,
         )
 
     def vector_buffer(self, buffer_size, **kwargs):
```

### Comparing `pymonntorch-0.1.1/pymonntorch/NetworkCore/SynapseGroup.py` & `pymonntorch-0.1.2/pymonntorch/NetworkCore/SynapseGroup.py`

 * *Files identical despite different names*

### Comparing `pymonntorch-0.1.1/pymonntorch/NetworkCore/TaggableObject.py` & `pymonntorch-0.1.2/pymonntorch/NetworkCore/TaggableObject.py`

 * *Files identical despite different names*

### Comparing `pymonntorch-0.1.1/pymonntorch/__init__.py` & `pymonntorch-0.1.2/pymonntorch/__init__.py`

 * *Files identical despite different names*

### Comparing `pymonntorch-0.1.1/pymonntorch.egg-info/PKG-INFO` & `pymonntorch-0.1.2/pymonntorch.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonntorch
-Version: 0.1.1
+Version: 0.1.2
 Summary: PymoNNtorch is a Pytorch version of PymoNNto
 Home-page: https://github.com/cnrl/PymoNNtorch
 Author: Computational Neuroscience Research Laboratory
 Author-email: ashenatena@gmail.com
 License: MIT license
 Keywords: pymonntorch
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -19,14 +19,20 @@
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ===========
 PymoNNtorch
 ===========
 
+.. image:: https://raw.githubusercontent.com/cnrl/PymoNNtorch/main/docs/_images/pymoNNtorch-logo-t-256.png
+    :width: 256
+    :alt: pymonntorch logo
+
+|
+
 
 .. image:: https://img.shields.io/pypi/v/pymonntorch.svg
         :target: https://pypi.python.org/pypi/pymonntorch
 
 .. .. image:: https://img.shields.io/travis/cnrl/pymonntorch.svg
 ..         :target: https://travis-ci.com/cnrl/pymonntorch
 
@@ -126,14 +132,15 @@
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 It changes the codebase of `PymoNNto <https://github.com/trieschlab/PymoNNto>`_ to use ``torch`` rather than ``numpy`` and ``tensorflow numpy``.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
+
 =======
 History
 =======
 
 0.1.1 (2023-05-26)
 ------------------
```

### Comparing `pymonntorch-0.1.1/pymonntorch.egg-info/SOURCES.txt` & `pymonntorch-0.1.2/pymonntorch.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,21 @@
 docs/documentation.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/readme.rst
 docs/tutorial.rst
+docs/_build/html/_images/pymoNNtorch-logo-t-256.png
+docs/_build/html/_images/spike.png
+docs/_build/html/_images/voltage.png
+docs/_build/html/_static/file.png
+docs/_build/html/_static/minus.png
+docs/_build/html/_static/plus.png
+docs/_images/pymoNNtorch-logo-t-256.png
 docs/_images/spike.png
 docs/_images/voltage.png
 pymonntorch/__init__.py
 pymonntorch/cli.py
 pymonntorch/pymonntorch.py
 pymonntorch/utils.py
 pymonntorch.egg-info/PKG-INFO
```

### Comparing `pymonntorch-0.1.1/setup.py` & `pymonntorch-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,10 +45,10 @@
     include_package_data=True,
     keywords="pymonntorch",
     name="pymonntorch",
     packages=find_packages(include=["pymonntorch", "pymonntorch.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/cnrl/PymoNNtorch",
-    version="0.1.1",
+    version="0.1.2",
     zip_safe=False,
 )
```

### Comparing `pymonntorch-0.1.1/tests/test_pymonntorch.py` & `pymonntorch-0.1.2/tests/test_pymonntorch.py`

 * *Files identical despite different names*

