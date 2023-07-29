# Comparing `tmp/pyaogmaneo-2.1.0.tar.gz` & `tmp/pyaogmaneo-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaogmaneo-2.1.0.tar", last modified: Fri Jul 28 16:36:41 2023, max compression
+gzip compressed data, was "pyaogmaneo-2.1.1.tar", last modified: Sat Jul 29 15:23:29 2023, max compression
```

## Comparing `pyaogmaneo-2.1.0.tar` & `pyaogmaneo-2.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-28 16:36:41.515473 pyaogmaneo-2.1.0/
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-28 16:36:41.515473 pyaogmaneo-2.1.0/CMake/
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1250 2023-03-18 01:02:16.000000 pyaogmaneo-2.1.0/CMake/FindAOgmaNeo.cmake
--rw-r--r--   0 ericl     (1000) ericl     (1001)     2620 2023-07-28 16:35:00.000000 pyaogmaneo-2.1.0/CMakeLists.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)    17842 2022-12-03 02:07:03.000000 pyaogmaneo-2.1.0/LICENSE.md
--rw-r--r--   0 ericl     (1000) ericl     (1001)       64 2022-12-03 02:07:03.000000 pyaogmaneo-2.1.0/MANIFEST.in
--rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-07-28 16:36:41.515473 pyaogmaneo-2.1.0/PKG-INFO
--rw-r--r--   0 ericl     (1000) ericl     (1001)     2412 2023-06-22 14:37:40.000000 pyaogmaneo-2.1.0/README.md
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-28 16:36:41.515473 pyaogmaneo-2.1.0/pyaogmaneo.egg-info/
--rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-07-28 16:36:41.000000 pyaogmaneo-2.1.0/pyaogmaneo.egg-info/PKG-INFO
--rw-r--r--   0 ericl     (1000) ericl     (1001)      505 2023-07-28 16:36:41.000000 pyaogmaneo-2.1.0/pyaogmaneo.egg-info/SOURCES.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2023-07-28 16:36:41.000000 pyaogmaneo-2.1.0/pyaogmaneo.egg-info/dependency_links.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2023-06-29 17:53:40.000000 pyaogmaneo-2.1.0/pyaogmaneo.egg-info/not-zip-safe
--rw-r--r--   0 ericl     (1000) ericl     (1001)       11 2023-07-28 16:36:41.000000 pyaogmaneo-2.1.0/pyaogmaneo.egg-info/top_level.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)      101 2023-01-13 01:36:37.000000 pyaogmaneo-2.1.0/pyproject.toml
--rw-r--r--   0 ericl     (1000) ericl     (1001)       38 2023-07-28 16:36:41.515473 pyaogmaneo-2.1.0/setup.cfg
--rw-r--r--   0 ericl     (1000) ericl     (1001)     4204 2023-07-28 16:34:37.000000 pyaogmaneo-2.1.0/setup.py
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-28 16:36:41.515473 pyaogmaneo-2.1.0/source/
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-28 16:36:41.515473 pyaogmaneo-2.1.0/source/pyaogmaneo/
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1071 2023-06-22 14:37:40.000000 pyaogmaneo-2.1.0/source/pyaogmaneo/py_helpers.cpp
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1783 2023-06-22 14:37:40.000000 pyaogmaneo-2.1.0/source/pyaogmaneo/py_helpers.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)    15775 2023-07-28 16:35:40.000000 pyaogmaneo-2.1.0/source/pyaogmaneo/py_hierarchy.cpp
--rw-r--r--   0 ericl     (1000) ericl     (1001)     7014 2023-07-28 16:35:13.000000 pyaogmaneo-2.1.0/source/pyaogmaneo/py_hierarchy.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)     8140 2023-07-28 00:25:43.000000 pyaogmaneo-2.1.0/source/pyaogmaneo/py_image_encoder.cpp
--rw-r--r--   0 ericl     (1000) ericl     (1001)     3217 2023-07-26 01:03:23.000000 pyaogmaneo-2.1.0/source/pyaogmaneo/py_image_encoder.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)     9067 2023-07-28 00:25:43.000000 pyaogmaneo-2.1.0/source/pyaogmaneo/py_module.cpp
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-29 15:23:29.150615 pyaogmaneo-2.1.1/
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-29 15:23:29.147282 pyaogmaneo-2.1.1/CMake/
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     1250 2023-03-18 01:02:16.000000 pyaogmaneo-2.1.1/CMake/FindAOgmaNeo.cmake
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     2620 2023-07-29 15:21:13.000000 pyaogmaneo-2.1.1/CMakeLists.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)    17842 2022-12-03 02:07:03.000000 pyaogmaneo-2.1.1/LICENSE.md
+-rw-r--r--   0 ericl     (1000) ericl     (1001)       64 2022-12-03 02:07:03.000000 pyaogmaneo-2.1.1/MANIFEST.in
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-07-29 15:23:29.147282 pyaogmaneo-2.1.1/PKG-INFO
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     2412 2023-06-22 14:37:40.000000 pyaogmaneo-2.1.1/README.md
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-29 15:23:29.147282 pyaogmaneo-2.1.1/pyaogmaneo.egg-info/
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-07-29 15:23:29.000000 pyaogmaneo-2.1.1/pyaogmaneo.egg-info/PKG-INFO
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      505 2023-07-29 15:23:29.000000 pyaogmaneo-2.1.1/pyaogmaneo.egg-info/SOURCES.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2023-07-29 15:23:29.000000 pyaogmaneo-2.1.1/pyaogmaneo.egg-info/dependency_links.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2023-06-29 17:53:40.000000 pyaogmaneo-2.1.1/pyaogmaneo.egg-info/not-zip-safe
+-rw-r--r--   0 ericl     (1000) ericl     (1001)       11 2023-07-29 15:23:29.000000 pyaogmaneo-2.1.1/pyaogmaneo.egg-info/top_level.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      101 2023-01-13 01:36:37.000000 pyaogmaneo-2.1.1/pyproject.toml
+-rw-r--r--   0 ericl     (1000) ericl     (1001)       38 2023-07-29 15:23:29.150615 pyaogmaneo-2.1.1/setup.cfg
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     4204 2023-07-29 15:20:49.000000 pyaogmaneo-2.1.1/setup.py
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-29 15:23:29.147282 pyaogmaneo-2.1.1/source/
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-29 15:23:29.147282 pyaogmaneo-2.1.1/source/pyaogmaneo/
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     1071 2023-06-22 14:37:40.000000 pyaogmaneo-2.1.1/source/pyaogmaneo/py_helpers.cpp
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     1783 2023-06-22 14:37:40.000000 pyaogmaneo-2.1.1/source/pyaogmaneo/py_helpers.h
+-rw-r--r--   0 ericl     (1000) ericl     (1001)    15776 2023-07-29 00:23:47.000000 pyaogmaneo-2.1.1/source/pyaogmaneo/py_hierarchy.cpp
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     7013 2023-07-29 15:21:32.000000 pyaogmaneo-2.1.1/source/pyaogmaneo/py_hierarchy.h
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     8140 2023-07-28 23:07:46.000000 pyaogmaneo-2.1.1/source/pyaogmaneo/py_image_encoder.cpp
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     3217 2023-07-26 01:03:23.000000 pyaogmaneo-2.1.1/source/pyaogmaneo/py_image_encoder.h
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     9243 2023-07-29 15:11:58.000000 pyaogmaneo-2.1.1/source/pyaogmaneo/py_module.cpp
```

### Comparing `pyaogmaneo-2.1.0/CMake/FindAOgmaNeo.cmake` & `pyaogmaneo-2.1.1/CMake/FindAOgmaNeo.cmake`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.1.0/CMakeLists.txt` & `pyaogmaneo-2.1.1/CMakeLists.txt`

 * *Files 9% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     find_package(AOgmaNeo)
 else()
     message(STATUS "Not using system installation of AOgmaNeo, will download from repository")
 
     FetchContent_Declare(
         AOgmaNeo
         GIT_REPOSITORY https://github.com/ogmacorp/AOgmaNeo.git
-        GIT_TAG a9aacebf334da53f9234858b4fa9557262727b10
+        GIT_TAG 76314e0d90d723c8d655815d190bef46409e86d8
     )
 
     FetchContent_GetProperties(AOgmaNeo)
 
     if(NOT AOgmaNeo_POPULATED)
         FetchContent_Populate(AOgmaNeo)
         add_subdirectory(${aogmaneo_SOURCE_DIR} ${aogmaneo_BINARY_DIR})
```

### Comparing `pyaogmaneo-2.1.0/LICENSE.md` & `pyaogmaneo-2.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.1.0/PKG-INFO` & `pyaogmaneo-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.1.0/README.md` & `pyaogmaneo-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.1.0/pyaogmaneo.egg-info/PKG-INFO` & `pyaogmaneo-2.1.1/pyaogmaneo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.1.0/setup.py` & `pyaogmaneo-2.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             os.makedirs(self.build_temp)
 
         subprocess.check_call([ 'cmake', ext.sourcedir ] + cmake_args, cwd=self.build_temp, env=env)
         subprocess.check_call([ 'cmake', '--build', '.' ] + build_args, cwd=self.build_temp)
 
 setup(
     name="pyaogmaneo",
-    version="2.1.0",
+    version="2.1.1",
     description="Python bindings for the AOgmaNeo library",
     long_description='https://github.com/ogmacorp/PyAOgmaNeo',
     author='Ogma Intelligent Systems Corp',
     author_email='info@ogmacorp.com',
     url='https://ogmacorp.com/',
     license='Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License',
     classifiers=[
```

### Comparing `pyaogmaneo-2.1.0/source/pyaogmaneo/py_helpers.cpp` & `pyaogmaneo-2.1.1/source/pyaogmaneo/py_helpers.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.1.0/source/pyaogmaneo/py_helpers.h` & `pyaogmaneo-2.1.1/source/pyaogmaneo/py_helpers.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.1.0/source/pyaogmaneo/py_hierarchy.cpp` & `pyaogmaneo-2.1.1/source/pyaogmaneo/py_hierarchy.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -261,62 +261,62 @@
 
     for (int j = 0; j < predictions.size(); j++)
         predictions[j] = cis[j];
 
     return predictions;
 }
 
-std::vector<float> Hierarchy::get_prediction_probs(
+std::vector<float> Hierarchy::get_prediction_acts(
     int i
 ) const {
     if (i < 0 || i >= h.get_num_io())
         throw std::runtime_error("prediction index " + std::to_string(i) + " out of range [0, " + std::to_string(h.get_num_io() - 1) + "]!");
 
-    if (!h.io_layer_exists(i) || h.get_io_type(i) != aon::prediction)
-        throw std::runtime_error("no decoder exists at index " + std::to_string(i) + " - did you set it to the correct type?");
+    if (!h.io_layer_exists(i) || h.get_io_type(i) == aon::none)
+        throw std::runtime_error("no decoder or actor exists at index " + std::to_string(i) + " - did you set it to the correct type?");
 
-    std::vector<float> predictions(h.get_prediction_probs(i).size());
+    std::vector<float> predictions(h.get_prediction_acts(i).size());
 
     for (int j = 0; j < predictions.size(); j++)
-        predictions[j] = h.get_prediction_probs(i)[j];
+        predictions[j] = h.get_prediction_acts(i)[j];
 
     return predictions;
 }
 
 std::vector<int> Hierarchy::sample_prediction(
     int i,
     float temperature
 ) const {
     if (temperature == 0.0f)
         return get_prediction_cis(i);
 
     if (i < 0 || i >= h.get_num_io())
         throw std::runtime_error("prediction index " + std::to_string(i) + " out of range [0, " + std::to_string(h.get_num_io() - 1) + "]!");
 
-    if (!h.io_layer_exists(i) || h.get_io_type(i) != aon::prediction)
-        throw std::runtime_error("no decoder exists at index " + std::to_string(i) + " - did you set it to the correct type?");
+    if (!h.io_layer_exists(i) || h.get_io_type(i) == aon::none)
+        throw std::runtime_error("no decoder or actor exists at index " + std::to_string(i) + " - did you set it to the correct type?");
 
     std::vector<int> sample(h.get_prediction_cis(i).size());
 
     int size_z = h.get_io_size(i).z;
 
     float temperature_inv = 1.0f / temperature;
 
     for (int j = 0; j < sample.size(); j++) {
         float total = 0.0f;
 
         for (int k = 0; k < size_z; k++)
-            total += aon::powf(h.get_prediction_probs(i)[k + j * size_z], temperature_inv);
+            total += aon::powf(h.get_prediction_acts(i)[k + j * size_z], temperature_inv);
 
         float cusp = aon::randf(0.0f, total);
 
         float sum_so_far = 0.0f;
 
         for (int k = 0; k < size_z; k++) {
-            sum_so_far += aon::powf(h.get_prediction_probs(i)[k + j * size_z], temperature_inv);
+            sum_so_far += aon::powf(h.get_prediction_acts(i)[k + j * size_z], temperature_inv);
 
             if (sum_so_far >= cusp) {
                 sample[j] = k;
 
                 break;
             }
         }
```

### Comparing `pyaogmaneo-2.1.0/source/pyaogmaneo/py_hierarchy.h` & `pyaogmaneo-2.1.1/source/pyaogmaneo/py_hierarchy.h`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 #pragma once
 
 #include "py_helpers.h"
 #include <aogmaneo/hierarchy.h>
 
 namespace pyaon {
-const int hierarchy_magic = 3133285;
+const int hierarchy_magic = 2184245;
 
 enum IO_Type {
     none = 0,
     prediction = 1,
     action = 2
 };
 
@@ -139,15 +139,15 @@
         int i
     ) const;
 
     std::vector<int> get_layer_prediction_cis(
         int l
     ) const;
 
-    std::vector<float> get_prediction_probs(
+    std::vector<float> get_prediction_acts(
         int i
     ) const;
 
     std::vector<int> sample_prediction(
         int i,
         float temperature
     ) const;
```

### Comparing `pyaogmaneo-2.1.0/source/pyaogmaneo/py_image_encoder.cpp` & `pyaogmaneo-2.1.1/source/pyaogmaneo/py_image_encoder.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.1.0/source/pyaogmaneo/py_image_encoder.h` & `pyaogmaneo-2.1.1/source/pyaogmaneo/py_image_encoder.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.1.0/source/pyaogmaneo/py_module.cpp` & `pyaogmaneo-2.1.1/source/pyaogmaneo/py_module.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -66,20 +66,23 @@
         .def_readwrite("down_radius", &pyaon::Layer_Desc::down_radius)
         .def_readwrite("ticks_per_update", &pyaon::Layer_Desc::ticks_per_update)
         .def_readwrite("temporal_horizon", &pyaon::Layer_Desc::temporal_horizon);
 
     // bind params
     py::class_<aon::Encoder::Params>(m, "EncoderParams")
         .def(py::init<>())
-        .def_readwrite("lr", &aon::Encoder::Params::lr);
+        .def_readwrite("scale", &aon::Encoder::Params::scale)
+        .def_readwrite("lr", &aon::Encoder::Params::lr)
+        .def_readwrite("gcurve", &aon::Encoder::Params::gcurve);
 
     py::class_<aon::Decoder::Params>(m, "DecoderParams")
         .def(py::init<>())
-        .def_readwrite("temperature", &aon::Decoder::Params::temperature)
-        .def_readwrite("lr", &aon::Decoder::Params::lr);
+        .def_readwrite("scale", &aon::Decoder::Params::scale)
+        .def_readwrite("lr", &aon::Decoder::Params::lr)
+        .def_readwrite("gcurve", &aon::Decoder::Params::gcurve);
 
     py::class_<aon::Actor::Params>(m, "ActorParams")
         .def(py::init<>())
         .def_readwrite("vlr", &aon::Actor::Params::vlr)
         .def_readwrite("alr", &aon::Actor::Params::alr)
         .def_readwrite("bias", &aon::Actor::Params::bias)
         .def_readwrite("discount", &aon::Actor::Params::discount)
@@ -126,15 +129,15 @@
             py::arg("reward") = 0.0f,
             py::arg("mimic") = 0.0f
         )
         .def("clear_state", &pyaon::Hierarchy::clear_state)
         .def("get_num_layers", &pyaon::Hierarchy::get_num_layers)
         .def("get_prediction_cis", &pyaon::Hierarchy::get_prediction_cis)
         .def("get_layer_prediction_cis", &pyaon::Hierarchy::get_layer_prediction_cis)
-        .def("get_prediction_probs", &pyaon::Hierarchy::get_prediction_probs)
+        .def("get_prediction_acts", &pyaon::Hierarchy::get_prediction_acts)
         .def("sample_prediction", &pyaon::Hierarchy::sample_prediction)
         .def("get_hidden_cis", &pyaon::Hierarchy::get_hidden_cis)
         .def("get_hidden_size", &pyaon::Hierarchy::get_hidden_size)
         .def("get_num_encoder_visible_layers", &pyaon::Hierarchy::get_num_encoder_visible_layers)
         .def("get_ticks", &pyaon::Hierarchy::get_ticks)
         .def("get_ticks_per_update", &pyaon::Hierarchy::get_ticks_per_update)
         .def("get_num_io", &pyaon::Hierarchy::get_num_io)
```

