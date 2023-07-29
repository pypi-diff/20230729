# Comparing `tmp/cudagrad-0.0.30.tar.gz` & `tmp/cudagrad-0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cudagrad-0.0.30.tar", last modified: Thu Jul 27 03:57:53 2023, max compression
+gzip compressed data, was "cudagrad-0.0.31.tar", last modified: Sat Jul 29 19:25:39 2023, max compression
```

## Comparing `cudagrad-0.0.30.tar` & `cudagrad-0.0.31.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-27 03:57:53.407678 cudagrad-0.0.30/
--rw-r--r--   0 ryan       (501) staff       (20)       44 2023-07-18 06:47:23.000000 cudagrad-0.0.30/MANIFEST.in
--rw-r--r--   0 ryan       (501) staff       (20)     3672 2023-07-27 03:57:53.407543 cudagrad-0.0.30/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)     3170 2023-07-25 01:40:28.000000 cudagrad-0.0.30/README.md
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-27 03:57:53.405713 cudagrad-0.0.30/cudagrad/
--rw-r--r--   0 ryan       (501) staff       (20)      107 2023-07-27 03:25:50.000000 cudagrad-0.0.30/cudagrad/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     5925 2023-07-27 03:50:10.000000 cudagrad-0.0.30/cudagrad/mlp.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-27 03:57:53.406486 cudagrad-0.0.30/cudagrad.egg-info/
--rw-r--r--   0 ryan       (501) staff       (20)     3672 2023-07-27 03:57:53.000000 cudagrad-0.0.30/cudagrad.egg-info/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      331 2023-07-27 03:57:53.000000 cudagrad-0.0.30/cudagrad.egg-info/SOURCES.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-27 03:57:53.000000 cudagrad-0.0.30/cudagrad.egg-info/dependency_links.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-27 00:32:51.000000 cudagrad-0.0.30/cudagrad.egg-info/not-zip-safe
--rw-r--r--   0 ryan       (501) staff       (20)       25 2023-07-27 03:57:53.000000 cudagrad-0.0.30/cudagrad.egg-info/requires.txt
--rw-r--r--   0 ryan       (501) staff       (20)        9 2023-07-27 03:57:53.000000 cudagrad-0.0.30/cudagrad.egg-info/top_level.txt
--rw-r--r--   0 ryan       (501) staff       (20)      754 2023-07-27 03:38:51.000000 cudagrad-0.0.30/pyproject.toml
--rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-27 03:57:53.407723 cudagrad-0.0.30/setup.cfg
--rw-r--r--   0 ryan       (501) staff       (20)     1659 2023-07-27 00:49:51.000000 cudagrad-0.0.30/setup.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-27 03:57:53.406954 cudagrad-0.0.30/src/
--rw-r--r--   0 ryan       (501) staff       (20)     2944 2023-07-27 00:52:48.000000 cudagrad-0.0.30/src/bindings.cpp
--rw-r--r--   0 ryan       (501) staff       (20)    20533 2023-07-27 03:54:25.000000 cudagrad-0.0.30/src/cudagrad.hpp
--rw-r--r--   0 ryan       (501) staff       (20)      261 2023-07-27 03:56:09.000000 cudagrad-0.0.30/src/ops.cu
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-27 03:57:53.407188 cudagrad-0.0.30/tests/
--rw-r--r--   0 ryan       (501) staff       (20)     1082 2023-07-27 03:55:30.000000 cudagrad-0.0.30/tests/test.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-29 19:25:39.223912 cudagrad-0.0.31/
+-rw-r--r--   0 ryan       (501) staff       (20)       44 2023-07-18 06:47:23.000000 cudagrad-0.0.31/MANIFEST.in
+-rw-r--r--   0 ryan       (501) staff       (20)     3660 2023-07-29 19:25:39.223796 cudagrad-0.0.31/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)     3157 2023-07-28 03:27:33.000000 cudagrad-0.0.31/README.md
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-29 19:25:39.221685 cudagrad-0.0.31/cudagrad/
+-rw-r--r--   0 ryan       (501) staff       (20)      107 2023-07-27 03:25:50.000000 cudagrad-0.0.31/cudagrad/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     5925 2023-07-27 03:50:10.000000 cudagrad-0.0.31/cudagrad/mlp.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-29 19:25:39.222728 cudagrad-0.0.31/cudagrad.egg-info/
+-rw-r--r--   0 ryan       (501) staff       (20)     3660 2023-07-29 19:25:39.000000 cudagrad-0.0.31/cudagrad.egg-info/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)      331 2023-07-29 19:25:39.000000 cudagrad-0.0.31/cudagrad.egg-info/SOURCES.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-29 19:25:39.000000 cudagrad-0.0.31/cudagrad.egg-info/dependency_links.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-27 00:32:51.000000 cudagrad-0.0.31/cudagrad.egg-info/not-zip-safe
+-rw-r--r--   0 ryan       (501) staff       (20)       25 2023-07-29 19:25:39.000000 cudagrad-0.0.31/cudagrad.egg-info/requires.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        9 2023-07-29 19:25:39.000000 cudagrad-0.0.31/cudagrad.egg-info/top_level.txt
+-rw-r--r--   0 ryan       (501) staff       (20)      984 2023-07-29 19:17:46.000000 cudagrad-0.0.31/pyproject.toml
+-rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-29 19:25:39.223950 cudagrad-0.0.31/setup.cfg
+-rw-r--r--   0 ryan       (501) staff       (20)     1659 2023-07-27 00:49:51.000000 cudagrad-0.0.31/setup.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-29 19:25:39.223131 cudagrad-0.0.31/src/
+-rw-r--r--   0 ryan       (501) staff       (20)     2910 2023-07-29 19:18:45.000000 cudagrad-0.0.31/src/bindings.cpp
+-rw-r--r--   0 ryan       (501) staff       (20)    20457 2023-07-29 19:17:36.000000 cudagrad-0.0.31/src/cudagrad.hpp
+-rw-r--r--   0 ryan       (501) staff       (20)      254 2023-07-29 18:53:13.000000 cudagrad-0.0.31/src/ops.cu
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-29 19:25:39.223508 cudagrad-0.0.31/tests/
+-rw-r--r--   0 ryan       (501) staff       (20)     1083 2023-07-29 16:33:01.000000 cudagrad-0.0.31/tests/test.py
```

### Comparing `cudagrad-0.0.30/PKG-INFO` & `cudagrad-0.0.31/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: cudagrad
-Version: 0.0.30
+Version: 0.0.31
 Summary: A small autograd engine
 Home-page: https://github.com/yrom1/cudagrad
 Author: Ryan Moore
-Author-email: Ryan Moore <moorethreads@hey.com>
+Author-email: Ryan Moore <ryanm.inbox@gmail.com>
 Project-URL: Homepage, https://github.com/yrom1/cudagrad
 Project-URL: Bug Tracker, https://github.com/yrom1/cudagrad/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 
 # cudagrad
 
 A small autograd engine
 
-Work In Progress! TODO: CUDA operation integration and release on PyPI 🙃
+Work In Progress! TODO: CUDA operation integration and release on PyPI
 
 ## Example
 
 ```cpp
 // c++ -std=c++11 -I./src examples/example.cpp && ./a.out
 #include "cudagrad.hpp"
 int main() {
@@ -51,18 +51,18 @@
 b = cg.tensor([2, 2], [6.0, 7.0, 8.0, 9.0])
 c = cg.tensor([2, 2], [10.0, 10.0, 10.0, 10.0])
 d = cg.tensor([2, 2], [11.0, 11.0, 11.0, 11.0])
 e = ((a @ b) + c) * d
 f = e.sum()
 f.backward()
 
-print(f.data) # [2794.0]
-print(f.size) # [1]
-print(a.grad) # [143.0, 187.0, 143.0, 187.0]
-print(b.grad) # [66.0, 66.0, 88.0, 88.0]
+print(f.data)  # [2794.0]
+print(f.size)  # [1]
+print(a.grad)  # [143.0, 187.0, 143.0, 187.0]
+print(b.grad)  # [66.0, 66.0, 88.0, 88.0]
 ```
 
 ## Design
 
 ~~The plan is to be similar to PyTorch's internals, particularily the [Variable/Tensor Merge Proposal](https://github.com/pytorch/pytorch/issues/13638) design.~~ The design is a mix of PyTorch and micrograd, with micrograd like members and PyTorch like backward classes with an `apply()` interface.
 
 For simplicity, many features PyTorch has cudagrad does not, like broadcasting and views. All operations are defined only on `std::shared_ptr<Tensor>`, for now at least.
@@ -80,12 +80,11 @@
 ## Running tests
 
 Taking inspiration from [micrograd's tests](https://github.com/karpathy/micrograd/blob/master/test/test_engine.py), we will use [PyTorch's C++ frontend](https://pytorch.org/cppdocs/frontend.html) for high level sanity checks using GoogleTest.
 
 To run the tests use:
 
 ```sh
-chmod +x manage.sh
-./manage.sh test
+python makefile.py test
 ```
 
 Running the tests requires: `cmake`, `make`, `torch` installed (on the version of Python accessed by the `python` command), `git`, and a C++ compiler. Note that these requirements are only for when you need to run the tests, otherwise except the C++ compiler they are not needed.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cudagrad-0.0.30/README.md` & `cudagrad-0.0.31/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # cudagrad
 
 A small autograd engine
 
-Work In Progress! TODO: CUDA operation integration and release on PyPI 🙃
+Work In Progress! TODO: CUDA operation integration and release on PyPI
 
 ## Example
 
 ```cpp
 // c++ -std=c++11 -I./src examples/example.cpp && ./a.out
 #include "cudagrad.hpp"
 int main() {
@@ -36,18 +36,18 @@
 b = cg.tensor([2, 2], [6.0, 7.0, 8.0, 9.0])
 c = cg.tensor([2, 2], [10.0, 10.0, 10.0, 10.0])
 d = cg.tensor([2, 2], [11.0, 11.0, 11.0, 11.0])
 e = ((a @ b) + c) * d
 f = e.sum()
 f.backward()
 
-print(f.data) # [2794.0]
-print(f.size) # [1]
-print(a.grad) # [143.0, 187.0, 143.0, 187.0]
-print(b.grad) # [66.0, 66.0, 88.0, 88.0]
+print(f.data)  # [2794.0]
+print(f.size)  # [1]
+print(a.grad)  # [143.0, 187.0, 143.0, 187.0]
+print(b.grad)  # [66.0, 66.0, 88.0, 88.0]
 ```
 
 ## Design
 
 ~~The plan is to be similar to PyTorch's internals, particularily the [Variable/Tensor Merge Proposal](https://github.com/pytorch/pytorch/issues/13638) design.~~ The design is a mix of PyTorch and micrograd, with micrograd like members and PyTorch like backward classes with an `apply()` interface.
 
 For simplicity, many features PyTorch has cudagrad does not, like broadcasting and views. All operations are defined only on `std::shared_ptr<Tensor>`, for now at least.
@@ -65,12 +65,11 @@
 ## Running tests
 
 Taking inspiration from [micrograd's tests](https://github.com/karpathy/micrograd/blob/master/test/test_engine.py), we will use [PyTorch's C++ frontend](https://pytorch.org/cppdocs/frontend.html) for high level sanity checks using GoogleTest.
 
 To run the tests use:
 
 ```sh
-chmod +x manage.sh
-./manage.sh test
+python makefile.py test
 ```
 
 Running the tests requires: `cmake`, `make`, `torch` installed (on the version of Python accessed by the `python` command), `git`, and a C++ compiler. Note that these requirements are only for when you need to run the tests, otherwise except the C++ compiler they are not needed.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cudagrad-0.0.30/cudagrad/mlp.py` & `cudagrad-0.0.31/cudagrad/mlp.py`

 * *Files identical despite different names*

### Comparing `cudagrad-0.0.30/cudagrad.egg-info/PKG-INFO` & `cudagrad-0.0.31/cudagrad.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: cudagrad
-Version: 0.0.30
+Version: 0.0.31
 Summary: A small autograd engine
 Home-page: https://github.com/yrom1/cudagrad
 Author: Ryan Moore
-Author-email: Ryan Moore <moorethreads@hey.com>
+Author-email: Ryan Moore <ryanm.inbox@gmail.com>
 Project-URL: Homepage, https://github.com/yrom1/cudagrad
 Project-URL: Bug Tracker, https://github.com/yrom1/cudagrad/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 
 # cudagrad
 
 A small autograd engine
 
-Work In Progress! TODO: CUDA operation integration and release on PyPI 🙃
+Work In Progress! TODO: CUDA operation integration and release on PyPI
 
 ## Example
 
 ```cpp
 // c++ -std=c++11 -I./src examples/example.cpp && ./a.out
 #include "cudagrad.hpp"
 int main() {
@@ -51,18 +51,18 @@
 b = cg.tensor([2, 2], [6.0, 7.0, 8.0, 9.0])
 c = cg.tensor([2, 2], [10.0, 10.0, 10.0, 10.0])
 d = cg.tensor([2, 2], [11.0, 11.0, 11.0, 11.0])
 e = ((a @ b) + c) * d
 f = e.sum()
 f.backward()
 
-print(f.data) # [2794.0]
-print(f.size) # [1]
-print(a.grad) # [143.0, 187.0, 143.0, 187.0]
-print(b.grad) # [66.0, 66.0, 88.0, 88.0]
+print(f.data)  # [2794.0]
+print(f.size)  # [1]
+print(a.grad)  # [143.0, 187.0, 143.0, 187.0]
+print(b.grad)  # [66.0, 66.0, 88.0, 88.0]
 ```
 
 ## Design
 
 ~~The plan is to be similar to PyTorch's internals, particularily the [Variable/Tensor Merge Proposal](https://github.com/pytorch/pytorch/issues/13638) design.~~ The design is a mix of PyTorch and micrograd, with micrograd like members and PyTorch like backward classes with an `apply()` interface.
 
 For simplicity, many features PyTorch has cudagrad does not, like broadcasting and views. All operations are defined only on `std::shared_ptr<Tensor>`, for now at least.
@@ -80,12 +80,11 @@
 ## Running tests
 
 Taking inspiration from [micrograd's tests](https://github.com/karpathy/micrograd/blob/master/test/test_engine.py), we will use [PyTorch's C++ frontend](https://pytorch.org/cppdocs/frontend.html) for high level sanity checks using GoogleTest.
 
 To run the tests use:
 
 ```sh
-chmod +x manage.sh
-./manage.sh test
+python makefile.py test
 ```
 
 Running the tests requires: `cmake`, `make`, `torch` installed (on the version of Python accessed by the `python` command), `git`, and a C++ compiler. Note that these requirements are only for when you need to run the tests, otherwise except the C++ compiler they are not needed.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cudagrad-0.0.30/setup.py` & `cudagrad-0.0.31/setup.py`

 * *Files identical despite different names*

### Comparing `cudagrad-0.0.30/src/bindings.cpp` & `cudagrad-0.0.31/src/bindings.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -47,28 +47,27 @@
     //              override str when no str present?
     py::class_<cg::Tensor, std::shared_ptr<cg::Tensor>>(m, "Tensor")
         .def(py::init<std::vector<int>, std::vector<float>>())
         .def("get_shared", &cg::Tensor::get_shared)
         .def("backward", &cg::Tensor::backward)
         .def("zero_grad", &cg::Tensor::zero_grad)
         .def("sum", &cg::Tensor::sum)
-        .def("matmul", &cg::matmul)
         .def_property_readonly("size", &cg::Tensor::get_size)
         .def_property_readonly("data", &cg::Tensor::get_data)
         .def_property_readonly("grad", &cg::Tensor::get_grad)
         .def("graph", &cg::Tensor::graph)
         .def_static("ones", &cg::Tensor::ones)
         .def_static("zeros", &cg::Tensor::zeros)
         .def_static("explode", &cg::Tensor::explode)
         .def_static("rand", &cg::Tensor::rand)
         .def("__add__", [](std::shared_ptr<cg::Tensor> a, std::shared_ptr<cg::Tensor> b) { return a + b; })
         .def("__sub__", [](std::shared_ptr<cg::Tensor> a, std::shared_ptr<cg::Tensor> b) { return a - b; })
         .def("__mul__", [](std::shared_ptr<cg::Tensor> a, std::shared_ptr<cg::Tensor> b) { return a * b; })
         .def("__truediv__", [](std::shared_ptr<cg::Tensor> a, std::shared_ptr<cg::Tensor> b) { return a / b; })
-        .def("__matmul__", [](std::shared_ptr<cg::Tensor> a, std::shared_ptr<cg::Tensor> b) { return cg::matmul(a, b); })
+        .def("__matmul__", [](std::shared_ptr<cg::Tensor> a, std::shared_ptr<cg::Tensor> b) { return a.get()->matmul(b); })
         .def("__str__", [](std::shared_ptr<cg::Tensor> t) {
             std::ostringstream os;
             os << t;
             return os.str();
         })
         .def("__repr__", [](std::shared_ptr<cg::Tensor> t) {
             std::ostringstream os;
```

### Comparing `cudagrad-0.0.30/src/cudagrad.hpp` & `cudagrad-0.0.31/src/cudagrad.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -118,16 +118,15 @@
         strides_(std::move(other.strides_)) {}
 
   std::shared_ptr<Tensor> get_shared() { return this->shared_from_this(); }
 
   void backward();
   void zero_grad();
   std::shared_ptr<Tensor> sum();
-  std::shared_ptr<Tensor> matmul(std::shared_ptr<Tensor> lhs,
-                                 std::shared_ptr<Tensor> rhs);
+  std::shared_ptr<Tensor> matmul(std::shared_ptr<Tensor> other);
 
   void size() {
     for (auto x : size_) std::cout << x << std::endl;
   }
   void data() {
     for (auto x : data_) std::cout << x << std::endl;
   }
@@ -326,18 +325,17 @@
 template <typename T>
 std::shared_ptr<Tensor> binaryForwardOperator(std::shared_ptr<Tensor> lhs,
                                               std::shared_ptr<Tensor> rhs,
                                               T forward) {
   return (*forward)();  // forward.get()();
 }
 
-std::shared_ptr<Tensor> matmul(std::shared_ptr<Tensor> lhs,
-                               std::shared_ptr<Tensor> rhs) {
-  std::shared_ptr<MatMulForward> f = std::make_shared<MatMulForward>(lhs, rhs);
-  return binaryForwardOperator<std::shared_ptr<MatMulForward>>(lhs, rhs, f);
+std::shared_ptr<Tensor> Tensor::matmul(std::shared_ptr<Tensor> other) {
+  std::shared_ptr<MatMulForward> f = std::make_shared<MatMulForward>(this->get_shared(), other);
+  return binaryForwardOperator<std::shared_ptr<MatMulForward>>(this->get_shared(), other, f);
 }
 
 std::shared_ptr<Tensor> Tensor::sum() {
   std::vector<float> total(1, 0.0f);
   for (float x : data_) {
     total[0] += x;
   }
```

### Comparing `cudagrad-0.0.30/tests/test.py` & `cudagrad-0.0.31/tests/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # python tests/test.py
 
-import cudagrad as cg
 import torch
 
+import cudagrad as cg
+
 # assert cg.__version__ == '0.0.1'
 # assert cg.add(1, 2) == 3
 # assert cg.subtract(1, 2) == -1
 
 
 def flatten(l):
     out = []
```

