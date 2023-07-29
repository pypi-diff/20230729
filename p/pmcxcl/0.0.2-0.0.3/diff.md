# Comparing `tmp/pmcxcl-0.0.2-pp39-pypy39_pp73-win_amd64.whl.zip` & `tmp/pmcxcl-0.0.3-pp39-pypy39_pp73-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 135337 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat   318464 b- defN 23-Jul-28 04:28 _pmcxcl.pypy39-pp73-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1626 b- defN 23-Jul-28 04:24 pmcxcl/__init__.py
--rw-rw-rw-  2.0 fat     1737 b- defN 23-Jul-28 04:24 pmcxcl/bench.py
--rw-rw-rw-  2.0 fat    10072 b- defN 23-Jul-28 04:28 pmcxcl-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      107 b- defN 23-Jul-28 04:28 pmcxcl-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-Jul-28 04:28 pmcxcl-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      535 b- defN 23-Jul-28 04:28 pmcxcl-0.0.2.dist-info/RECORD
-7 files, 332556 bytes uncompressed, 134403 bytes compressed:  59.6%
+Zip file size: 540182 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat   888832 b- defN 23-Jul-29 20:17 _pmcxcl.pypy39-pp73-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     1626 b- defN 23-Jul-29 20:15 pmcxcl/__init__.py
+-rw-rw-rw-  2.0 fat     1737 b- defN 23-Jul-29 20:15 pmcxcl/bench.py
+-rw-rw-rw-  2.0 fat     9258 b- defN 23-Jul-29 20:17 pmcxcl-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      107 b- defN 23-Jul-29 20:17 pmcxcl-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-Jul-29 20:17 pmcxcl-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      534 b- defN 23-Jul-29 20:17 pmcxcl-0.0.3.dist-info/RECORD
+7 files, 902109 bytes uncompressed, 539248 bytes compressed:  40.2%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: pmcxcl/__init__.py
 Comment: 
 
 Filename: pmcxcl/bench.py
 Comment: 
 
-Filename: pmcxcl-0.0.2.dist-info/METADATA
+Filename: pmcxcl-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: pmcxcl-0.0.2.dist-info/WHEEL
+Filename: pmcxcl-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: pmcxcl-0.0.2.dist-info/top_level.txt
+Filename: pmcxcl-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pmcxcl-0.0.2.dist-info/RECORD
+Filename: pmcxcl-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pmcxcl/__init__.py

```diff
@@ -33,10 +33,10 @@
 except ImportError:  # pragma: no cover
     print("the pmcxcl binary extension (_pmcxcl) is not compiled! please compile first")
 
 # from .utils import detweight, cwdref
 # from .files import loadmc2, loadmch, load, save
 from .bench import bench
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 __all__ = ("gpuinfo", "run", "bench")
```

## Comparing `pmcxcl-0.0.2.dist-info/METADATA` & `pmcxcl-0.0.3.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmcxcl
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python bindings for Monte Carlo eXtreme photon transport simulator
 Home-page: https://github.com/fangq/mcxcl
 Author: Matin Raayai Ardakani, Qianqian Fang
 Author-email: raayaiardakani.m@northeastern.edu, q.fang@neu.edu
 Maintainer: Qianqian Fang
 License: GPLv3+
 Download-URL: http://mcx.space
@@ -23,46 +23,52 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires: numpy
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 ![](http://mcx.space/img/mcx18_banner.png)
 
-# PMCX-CL - Python bindings for Monte Carlo eXtreme photon transport simulator
+# PMCX-CL - Python bindings for Monte Carlo eXtreme (OpenCL) photon transport simulator
 
 - Copyright: (C) Matin Raayai Ardakani (2022-2023) <raayaiardakani.m at northeastern.edu> 
 and Qianqian Fang (2019-2023) <q.fang at neu.edu>
 - License: GNU Public License V3 or later
-- Version: 0.0.2
+- Version: 0.0.3
 - URL: https://pypi.org/project/pmcxcl/
 - Github: https://github.com/fangq/mcxcl
 
-[![Build Status](https://travis-ci.com/fangq/mcx.svg?branch=master)](https://travis-ci.com/fangq/mcxcl)
-
-This module provides a Python binding for Monte Carlo eXtreme (MCX).
-For other binaries, including the standalone executable and the MATLAB bindings, see [our website](http://mcx.space).
+![Linux Python Module](https://github.com/fangq/mcxcl/actions/workflows/build_linux_manywheel.yml/badge.svg)\
+![MacOS Python Module](https://github.com/fangq/mcxcl/actions/workflows/build_macos_wheel.yml/badge.svg)\
+![Windows Python Module](https://github.com/fangq/mcxcl/actions/workflows/build_windows_wheel.yml/badge.svg)\
+![Mex and Binaries](https://github.com/fangq/mcxcl/actions/workflows/build_all.yml/badge.svg)
+
+This module provides a Python binding for Monte Carlo eXtreme for OpenCL (MCXCL).
+For other binaries, including the standalone executable and the MATLAB bindings,
+see [our website](https://mcx.space).
 
 Monte Carlo eXtreme (MCX) is a fast photon transport simulation software for 3D 
 heterogeneous turbid media. By taking advantage of the massively parallel 
 threads and extremely low memory latency in a modern graphics processing unit 
 (GPU), MCX is capable of performing Monte Carlo (MC) photon simulations at a 
-blazing speed, typically hundreds to a thousand times faster than a fully 
-optimized CPU-based MC implementation.
+blazing speed, typically hundreds to a thousand times faster than a single-threaded
+CPU-based MC implementation.
 
 ## How to Install
 
-* PIP: ```pip install pmcxcl``` see https://pypi.org/project/pmcxcl/
+* PIP: ```pip install pmcxcl```
 
 ## Runtime Dependencies
-* **OpenCL runtime for CPU or GPU**: A OpenCL-capable GPU and driver is required to run MCX. An up-to-date driver is recommended.
-The binary wheel distributed over pip runs on drivers. For more details on driver versions and their CUDA support, see the 
-[CUDA Release Notes](https://docs.nvidia.com/cuda/cuda-toolkit-release-notes/index.html). 
-To download the latest driver for your system, see the 
-[NVIDIA Driver Download Page](https://www.nvidia.com/download/index.aspx).
-**You shouldn't need to have CUDA toolkit installed**. MCX is built with the static CUDA runtime library. 
+* **CPU or GPU**: An OpenCL-capable CPU or GPU; most modern CPUs or GPUs support OpenCL -
+an industrial-standard heterogeneous computing library and specification (https://www.khronos.org/opencl/)
+* **OpenCL CPU or GPU runtime/driver**: Both NVIDIA and AMD GPU graphics drivers should contain
+out-of-box OpenCL runtimes or drivers; for Intel GPUs, one should install additional OpenCL runtime
+support from https://github.com/intel/compute-runtime or install the `intel-opencl-icd` package
+if the OS provides (such as Ubuntu 22.04); one can also install an open-source OpenCL runtime
+[POCL](http://portablecl.org/), using package manager such as `sudo apt-get install pocl-opencl-icd`. However,
+POCL's support is largely limited to CPUs. You **do not need** to install CUDA SDK to use pmcxcl.
 * **Python**: Python 3.6 and newer is required. **Python 2 is not supported**.
 * **numpy**: Used to pass/receive volumetric information to/from pmcxcl. To install, use either conda or pip 
 package managers: `pip install numpy` or `conda install numpy`
 * (optional) **jdata**: Only needed to read/write JNIfTI output files. To install, use pip: `pip install jdata` 
 on all operating systems; For Debian-based Linux distributions, you can also install to the system interpreter 
 using apt-get: `sudo apt-get install python3-jdata`. See https://pypi.org/project/jdata/ for more details. 
 * (optional) **bjdata**: Only needed to read/write BJData/UBJSON files. To install, run `pip install bjdata` 
@@ -70,89 +76,72 @@
 using apt-get: `sudo apt-get install python3-bjdata`. See https://pypi.org/project/bjdata/ for more details. 
 * (optional) **matplotlib**: For plotting the results. To install, run either `pip install matplotlib` or
 `conda install matplotlib`
 
 ## Build Instructions
 
 ### Build Dependencies
-* **Operating System**: Windows and Linux are fully supported; For building MCX on macOS, OSX 10.13 (High Sierra) and 
-older are highly recommended since 10.13 was the last version of macOS with NVIDIA CUDA support, and matching the CUDA 
-compiler version with the C/C++ compiler shipped with Xcode is easier. Newer macOS versions can be used for building MCX, 
-but need to have System Integrity Protection disabled prior to installing the CUDA toolkit due to the NVIDIA installer copying
-its payload under the ```/Developer``` directory under root.
-* **NVIDIA CUDA Toolkit**: CUDA 7.5 or newer is required. On macOS, 10.2 is the last available CUDA version.
-For details on how to install CUDA, see the [CUDA Download Page](https://developer.nvidia.com/cuda-downloads). 
-The NVIDIA GPU driver of the target system must support the selected CUDA toolkit.
+* **Operating System**: pmcxcl and mcxcl can be compiled on most OSes, including Windows, Linux and MacOS.
+* **OpenCL library**: compiling mcxcl or pmcxcl requires to link with `libOpenCL.so` on Linux, or `libOpenCL.dylib`
+on MacOS or `OpenCL.dll` on Windows. These libraries should have been installed by either graphics driver or
+OpenCL runtimes.
 * **Python Interpreter**: Python 3.6 or above. The ```pip``` Python package manager and the ```wheel``` package (available
   via ```pip```) are not required but recommended.
-* **C/C++ Compiler**: CUDA Toolkit supports only the following compilers:
-  * GNU GCC for Linux-based distributions.
+* **C/C++ Compiler**: pmcxcl can be compiled using a wide variety of C compilers, including
+  * GNU GCC for Linux, MacOS (intalled via MacPorts or brew), and Windows (installed via msys2, mingw64 or cygwin64)
   * Microsoft Visual Studio C/C++ Compiler for Windows.
-  * Apple Clang for macOS, available via Xcode. The last Xcode version supported by CUDA 10.2 is 10.3. If using an OSX 
-  version higher than 10.15 it can be downloaded and installed from [Apple's Developer Website](https://developer.apple.com/download/) 
-  with an Apple ID. After installation, select the proper Xcode version from the commandline, and set the ```SDKROOT```
-  environment variable:
-    ```zsh
-    sudo xcode-select -s /Applications/Xcode_10.3.app/Contents/Developer/
-    export SDKROOT=/Applications/Xcode_10.3.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX.sdk
-    ```
-  
+  * Apple Clang for macOS, available via Xcode.
+
   Refer to each OS's online documentations for more in-depth information on how to install these compilers.
-  Note that the version of the C/C++ compiler used must be supported by the CUDA toolkit version. If not, compilation
-  will fail with an error notifying you of this problem. See the [CUDA Installation Guides](https://developer.nvidia.com/cuda-toolkit-archive)
-  for more details.
+  MacOS provides built-in OpenCL library support.
 * **OpenMP**: The installed C/C++ Compiler should have support for [OpenMP](https://www.openmp.org/). 
   GCC and Microsoft Visual Studio compiler support OpenMP out of the box. Apple Clang, however, requires manual 
   installation of OpenMP libraries for Apple Clang. The easiest way to do this is via the [Brew](https://brew.sh/) package
   manager, preferably after selecting the correct Xcode version:
   ```zsh
     brew install libomp
     brew link --force libomp
   ```
-
 * **CMake**: CMake version 3.15 and later is required. Refer to the [CMake website](https://cmake.org/download/) for more information on how to download.
   CMake is also widely available on package managers across all operating systems.
-  Additionally, on Windows, make sure **Visual Studio's C++ CMake tools for Windows** is also installed by selecting its option
-  during installation.
 * **Zlib Compression Development Headers**: On Linux, this is generally available via the built-in package manager. For 
   example, on Debian-based distributions like Ubuntu it is available via ```apt``` under the name ```zlib1g-dev```. On
   macOS, brew provides it under the name ```zlib```. No packaged versions of Zlib are available for windows, therefore it must be
   downloaded manually and added to the CMake environment variables in your working Powershell session:
   ```powershell
     curl.exe --retry 3 -kL https://cytranet.dl.sourceforge.net/project/gnuwin32/zlib/1.2.3/zlib-1.2.3-lib.zip --output zlib.zip
     Expand-Archive .\zlib.zip -DestinationPath zlib\
     $env:CMAKE_INCLUDE_PATH=$PWD\zlib\include
     $env:CMAKE_LIBRARY_PATH=$PWD\zlib\lib
   ```
 
 ### Build Steps
-1. Ensure that ```cmake```, ```nvcc``` (NVIDIA CUDA Compiler) and the C/C++ compiler are all located over your ```PATH```.
+1. Ensure that ```cmake```, ```python``` and the C/C++ compiler are all located over your ```PATH```.
 This can be queried via ```echo $env:PATH``` on Windows or ```echo $PATH``` on Linux. If not, locate them and add their folder to the ```PATH```.
 
 2. Clone the repository and switch to the ```pmcxcl/``` folder:
     ```bash
         git clone --recursive https://github.com/fangq/mcx.git
         cd mcx/pmcxcl
     ```
-
-3. Either run ```python setup.py install``` or ```pip install .``` to directly install, or run ```pip wheel .``` to only
-build the Python wheel without installing it.
+3. Run ```pip wheel .``` inside the `pmcxcl` folder to locally build the Python wheel without installing it
+4. One can also run ```python setup.py install``` or ```pip install .``` to build and directly install the compiled package
 
 
 ## How to use
 
 The PMCXCL module is easy to use. You can use the `pmcxcl.gpuinfo()` function to first verify
 if you have NVIDIA/CUDA compatible GPUs installed; if there are NVIDIA GPUs detected,
 you can then call the `run()` function to launch a photon simulation.
 
 A simulation can be defined conveniently in two approaches - a one-liner and a two-liner:
 
 * For the one-liner, one simply pass on each MCX simulation setting as positional
 argument. The supported setting names are compatible to nearly all the input fields
-for the MATLAB version of MCX - [MCXLAB](https://github.com/fangq/mcx/blob/master/mcxlab/mcxlab.m))
+for the MATLAB version of MCX/MCXCL - [MCXLAB](https://github.com/fangq/mcx/blob/master/mcxlab/mcxlab.m))
 
 ```python3
 import pmcxcl
 import numpy as np
 import matplotlib.pyplot as plt
 
 res = pmcxcl.run(nphoton=1000000, vol=np.ones([60, 60, 60], dtype='uint8'), tstart=0, tend=5e-9,
```

