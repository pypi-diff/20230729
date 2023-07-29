# Comparing `tmp/pytorch_memlab-0.2.4.tar.gz` & `tmp/pytorch-memlab-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytorch_memlab-0.2.4.tar", last modified: Thu Oct 28 05:46:34 2021, max compression
+gzip compressed data, was "pytorch-memlab-0.3.0.tar", last modified: Sat Jul 29 13:26:26 2023, max compression
```

## Comparing `pytorch_memlab-0.2.4.tar` & `pytorch-memlab-0.3.0.tar`

### file list

```diff
@@ -1,39 +1,30 @@
-drwxr-xr-x   0 kys08    (949059) aispeech (20000)        0 2021-10-28 05:46:34.000000 pytorch_memlab-0.2.4/
-drwxr-xr-x   0 kys08    (949059) aispeech (20000)        0 2021-10-28 05:46:34.000000 pytorch_memlab-0.2.4/.github/
-drwxr-xr-x   0 kys08    (949059) aispeech (20000)        0 2021-10-28 05:46:34.000000 pytorch_memlab-0.2.4/.github/workflows/
--rw-r--r--   0 kys08    (949059) aispeech (20000)     1070 2021-10-28 05:09:13.000000 pytorch_memlab-0.2.4/.github/workflows/pypi-publish.yml
--rw-r--r--   0 kys08    (949059) aispeech (20000)     1078 2021-10-28 05:12:54.000000 pytorch_memlab-0.2.4/.github/workflows/test.yml
--rw-r--r--   0 kys08    (949059) aispeech (20000)     1789 2020-12-01 09:16:25.000000 pytorch_memlab-0.2.4/.gitignore
--rw-r--r--   0 kys08    (949059) aispeech (20000)     1066 2019-07-24 03:51:26.000000 pytorch_memlab-0.2.4/LICENSE
--rw-r--r--   0 kys08    (949059) aispeech (20000)     1616 2019-07-24 03:51:26.000000 pytorch_memlab-0.2.4/LICENSE_kernprof.txt
--rw-r--r--   0 kys08    (949059) aispeech (20000)    21699 2021-10-28 05:46:34.000000 pytorch_memlab-0.2.4/PKG-INFO
--rw-r--r--   0 kys08    (949059) aispeech (20000)    17288 2021-10-28 03:19:11.000000 pytorch_memlab-0.2.4/README.md
--rw-r--r--   0 kys08    (949059) aispeech (20000)    32948 2020-12-01 09:16:25.000000 pytorch_memlab-0.2.4/demo.ipynb
-drwxr-xr-x   0 kys08    (949059) aispeech (20000)        0 2021-10-28 05:46:34.000000 pytorch_memlab-0.2.4/pytorch_memlab/
--rw-r--r--   0 kys08    (949059) aispeech (20000)      275 2020-12-01 09:16:25.000000 pytorch_memlab-0.2.4/pytorch_memlab/__init__.py
--rw-r--r--   0 kys08    (949059) aispeech (20000)     1523 2020-12-01 09:16:25.000000 pytorch_memlab-0.2.4/pytorch_memlab/courtesy.py
-drwxr-xr-x   0 kys08    (949059) aispeech (20000)        0 2021-10-28 05:46:34.000000 pytorch_memlab-0.2.4/pytorch_memlab/line_profiler/
--rw-r--r--   0 kys08    (949059) aispeech (20000)      128 2020-12-01 09:16:25.000000 pytorch_memlab-0.2.4/pytorch_memlab/line_profiler/__init__.py
--rw-r--r--   0 kys08    (949059) aispeech (20000)     3466 2021-05-11 11:23:55.000000 pytorch_memlab-0.2.4/pytorch_memlab/line_profiler/extension.py
--rw-r--r--   0 kys08    (949059) aispeech (20000)     5707 2021-05-11 11:07:26.000000 pytorch_memlab-0.2.4/pytorch_memlab/line_profiler/line_profiler.py
--rw-r--r--   0 kys08    (949059) aispeech (20000)    10466 2021-03-03 13:36:52.000000 pytorch_memlab-0.2.4/pytorch_memlab/line_profiler/line_records.py
--rw-r--r--   0 kys08    (949059) aispeech (20000)     3451 2021-03-03 13:36:52.000000 pytorch_memlab-0.2.4/pytorch_memlab/line_profiler/profile.py
--rw-r--r--   0 kys08    (949059) aispeech (20000)     7576 2021-03-03 13:36:52.000000 pytorch_memlab-0.2.4/pytorch_memlab/mem_reporter.py
--rw-r--r--   0 kys08    (949059) aispeech (20000)      180 2021-03-03 13:36:52.000000 pytorch_memlab-0.2.4/pytorch_memlab/utils.py
-drwxr-xr-x   0 kys08    (949059) aispeech (20000)        0 2021-10-28 05:46:34.000000 pytorch_memlab-0.2.4/pytorch_memlab.egg-info/
--rw-r-----   0 kys08    (949059) aispeech (20000)    21699 2021-10-28 05:46:32.000000 pytorch_memlab-0.2.4/pytorch_memlab.egg-info/PKG-INFO
--rw-r-----   0 kys08    (949059) aispeech (20000)      816 2021-10-28 05:46:32.000000 pytorch_memlab-0.2.4/pytorch_memlab.egg-info/SOURCES.txt
--rw-r-----   0 kys08    (949059) aispeech (20000)        1 2021-10-28 05:46:32.000000 pytorch_memlab-0.2.4/pytorch_memlab.egg-info/dependency_links.txt
--rw-r-----   0 kys08    (949059) aispeech (20000)       84 2021-10-28 05:46:32.000000 pytorch_memlab-0.2.4/pytorch_memlab.egg-info/requires.txt
--rw-r-----   0 kys08    (949059) aispeech (20000)       20 2021-10-28 05:46:32.000000 pytorch_memlab-0.2.4/pytorch_memlab.egg-info/top_level.txt
--rw-r-----   0 kys08    (949059) aispeech (20000)        1 2019-08-06 12:27:58.000000 pytorch_memlab-0.2.4/pytorch_memlab.egg-info/zip-safe
--rw-r--r--   0 kys08    (949059) aispeech (20000)    73347 2020-12-01 09:16:26.000000 pytorch_memlab-0.2.4/readme-output.png
--rw-r--r--   0 kys08    (949059) aispeech (20000)       54 2020-12-01 09:16:26.000000 pytorch_memlab-0.2.4/requirements.txt
--rw-r--r--   0 kys08    (949059) aispeech (20000)       38 2021-10-28 05:46:34.000000 pytorch_memlab-0.2.4/setup.cfg
--rw-r--r--   0 kys08    (949059) aispeech (20000)     1010 2021-10-28 03:19:11.000000 pytorch_memlab-0.2.4/setup.py
-drwxr-xr-x   0 kys08    (949059) aispeech (20000)        0 2021-10-28 05:46:34.000000 pytorch_memlab-0.2.4/test/
--rw-r--r--   0 kys08    (949059) aispeech (20000)        0 2020-12-01 09:16:26.000000 pytorch_memlab-0.2.4/test/__init__.py
--rw-r--r--   0 kys08    (949059) aispeech (20000)      377 2021-03-04 16:30:12.000000 pytorch_memlab-0.2.4/test/demo.py
--rw-r--r--   0 kys08    (949059) aispeech (20000)      759 2019-07-24 03:51:26.000000 pytorch_memlab-0.2.4/test/test_courtesy.py
--rw-r--r--   0 kys08    (949059) aispeech (20000)     3523 2020-12-01 09:16:26.000000 pytorch_memlab-0.2.4/test/test_line_profiler.py
--rw-r--r--   0 kys08    (949059) aispeech (20000)     2185 2021-03-03 13:36:52.000000 pytorch_memlab-0.2.4/test/test_mem_reporter.py
+drwxr-xr-x   0 kaiyushi   (501) staff       (20)        0 2023-07-29 13:26:26.708739 pytorch-memlab-0.3.0/
+-rw-r--r--   0 kaiyushi   (501) staff       (20)     1066 2023-02-09 02:12:27.000000 pytorch-memlab-0.3.0/LICENSE
+-rw-r--r--   0 kaiyushi   (501) staff       (20)     1616 2023-02-09 02:12:27.000000 pytorch-memlab-0.3.0/LICENSE_kernprof.txt
+-rw-r--r--   0 kaiyushi   (501) staff       (20)    17842 2023-07-29 13:26:26.708581 pytorch-memlab-0.3.0/PKG-INFO
+-rw-r--r--   0 kaiyushi   (501) staff       (20)    17281 2023-07-29 10:38:12.000000 pytorch-memlab-0.3.0/README.md
+drwxr-xr-x   0 kaiyushi   (501) staff       (20)        0 2023-07-29 13:26:26.705628 pytorch-memlab-0.3.0/pytorch_memlab/
+-rw-r--r--   0 kaiyushi   (501) staff       (20)      275 2023-07-29 10:36:52.000000 pytorch-memlab-0.3.0/pytorch_memlab/__init__.py
+-rw-r--r--   0 kaiyushi   (501) staff       (20)     1523 2023-02-09 02:12:27.000000 pytorch-memlab-0.3.0/pytorch_memlab/courtesy.py
+drwxr-xr-x   0 kaiyushi   (501) staff       (20)        0 2023-07-29 13:26:26.707709 pytorch-memlab-0.3.0/pytorch_memlab/line_profiler/
+-rw-r--r--   0 kaiyushi   (501) staff       (20)      128 2023-07-29 10:36:52.000000 pytorch-memlab-0.3.0/pytorch_memlab/line_profiler/__init__.py
+-rw-r--r--   0 kaiyushi   (501) staff       (20)     3466 2023-07-29 10:36:52.000000 pytorch-memlab-0.3.0/pytorch_memlab/line_profiler/extension.py
+-rw-r--r--   0 kaiyushi   (501) staff       (20)     5707 2023-07-29 10:36:52.000000 pytorch-memlab-0.3.0/pytorch_memlab/line_profiler/line_profiler.py
+-rw-r--r--   0 kaiyushi   (501) staff       (20)    10476 2023-07-29 10:36:52.000000 pytorch-memlab-0.3.0/pytorch_memlab/line_profiler/line_records.py
+-rw-r--r--   0 kaiyushi   (501) staff       (20)     3451 2023-07-29 10:36:52.000000 pytorch-memlab-0.3.0/pytorch_memlab/line_profiler/profile.py
+-rw-r--r--   0 kaiyushi   (501) staff       (20)     7576 2023-07-29 10:36:52.000000 pytorch-memlab-0.3.0/pytorch_memlab/mem_reporter.py
+-rw-r--r--   0 kaiyushi   (501) staff       (20)      180 2023-07-29 10:36:52.000000 pytorch-memlab-0.3.0/pytorch_memlab/utils.py
+drwxr-xr-x   0 kaiyushi   (501) staff       (20)        0 2023-07-29 13:26:26.706742 pytorch-memlab-0.3.0/pytorch_memlab.egg-info/
+-rw-r--r--   0 kaiyushi   (501) staff       (20)    17842 2023-07-29 13:26:26.000000 pytorch-memlab-0.3.0/pytorch_memlab.egg-info/PKG-INFO
+-rw-r--r--   0 kaiyushi   (501) staff       (20)      684 2023-07-29 13:26:26.000000 pytorch-memlab-0.3.0/pytorch_memlab.egg-info/SOURCES.txt
+-rw-r--r--   0 kaiyushi   (501) staff       (20)        1 2023-07-29 13:26:26.000000 pytorch-memlab-0.3.0/pytorch_memlab.egg-info/dependency_links.txt
+-rw-r--r--   0 kaiyushi   (501) staff       (20)       84 2023-07-29 13:26:26.000000 pytorch-memlab-0.3.0/pytorch_memlab.egg-info/requires.txt
+-rw-r--r--   0 kaiyushi   (501) staff       (20)       20 2023-07-29 13:26:26.000000 pytorch-memlab-0.3.0/pytorch_memlab.egg-info/top_level.txt
+-rw-r--r--   0 kaiyushi   (501) staff       (20)        1 2023-07-29 13:26:26.000000 pytorch-memlab-0.3.0/pytorch_memlab.egg-info/zip-safe
+-rw-r--r--   0 kaiyushi   (501) staff       (20)       38 2023-07-29 13:26:26.708795 pytorch-memlab-0.3.0/setup.cfg
+-rw-r--r--   0 kaiyushi   (501) staff       (20)     1010 2023-07-29 13:17:35.000000 pytorch-memlab-0.3.0/setup.py
+drwxr-xr-x   0 kaiyushi   (501) staff       (20)        0 2023-07-29 13:26:26.708332 pytorch-memlab-0.3.0/test/
+-rw-r--r--   0 kaiyushi   (501) staff       (20)        0 2023-07-29 10:36:52.000000 pytorch-memlab-0.3.0/test/__init__.py
+-rw-r--r--   0 kaiyushi   (501) staff       (20)      759 2023-02-09 02:12:27.000000 pytorch-memlab-0.3.0/test/test_courtesy.py
+-rw-r--r--   0 kaiyushi   (501) staff       (20)     3523 2023-07-29 10:36:52.000000 pytorch-memlab-0.3.0/test/test_line_profiler.py
+-rw-r--r--   0 kaiyushi   (501) staff       (20)     2185 2023-07-29 10:36:52.000000 pytorch-memlab-0.3.0/test/test_mem_reporter.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pytorch_memlab-0.2.4/LICENSE` & `pytorch-memlab-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch_memlab-0.2.4/LICENSE_kernprof.txt` & `pytorch-memlab-0.3.0/LICENSE_kernprof.txt`

 * *Files identical despite different names*

### Comparing `pytorch_memlab-0.2.4/PKG-INFO` & `pytorch-memlab-0.3.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,503 +1,485 @@
-Metadata-Version: 2.1
-Name: pytorch_memlab
-Version: 0.2.4
-Summary: A lab to do simple and accurate memory experiments on pytorch
-Home-page: https://github.com/Stonesjtu/pytorch_memlab
-Author: Kaiyu Shi
-Author-email: skyisno.1@gmail.com
-License: MIT
-Description: pytorch_memlab
-        ======
-        [![Build Status](https://travis-ci.com/Stonesjtu/pytorch_memlab.svg?token=vyTdxHbi1PCRzV6disHp&branch=master)](https://travis-ci.com/Stonesjtu/pytorch_memlab)
-        ![PyPI](https://img.shields.io/pypi/v/pytorch_memlab.svg)
-        [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/Stonesjtu/pytorch_memlab.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Stonesjtu/pytorch_memlab/context:python)
-        ![PyPI - Downloads](https://img.shields.io/pypi/dm/pytorch_memlab.svg)
-        
-        A simple and accurate **CUDA** memory management laboratory for pytorch,
-        it consists of different parts about the memory:
-        
-        - Features:
-        
-          - Memory Profiler: A `line_profiler` style CUDA memory profiler with simple API.
-          - Memory Reporter: A reporter to inspect tensors occupying the CUDA memory.
-          - Courtesy: An interesting feature to temporarily move all the CUDA tensors into
-            CPU memory for courtesy, and of course the backward transferring.
-          - IPython support through `%mlrun`/`%%mlrun` line/cell magic
-            commands.
-        
-        
-        - Table of Contents
-          * [Installation](#installation)
-          * [User-Doc](#user-doc)
-            + [Memory Profiler](#memory-profiler)
-            + [IPython support](#ipython-support)
-            + [Memory Reporter](#memory-reporter)
-            + [Courtesy](#courtesy)
-            + [ACK](#ack)
-          * [CHANGES](#changes)
-        
-        Installation
-        -----
-        
-        - Released version:
-        ```bash
-        pip install pytorch_memlab
-        ```
-        
-        - Newest version:
-        ```bash
-        pip install git+https://github.com/stonesjtu/pytorch_memlab
-        ```
-        
-        What's for
-        -----
-        
-        Out-Of-Memory errors in pytorch happen frequently, for new-bees and
-        experienced programmers. A common reason is that most people don't really
-        learn the underlying memory management philosophy of pytorch and GPUs.
-        They wrote memory in-efficient codes and complained about pytorch eating too
-        much CUDA memory.
-        
-        In this repo, I'm going to share some useful tools to help debugging OOM, or
-        to inspect the underlying mechanism if anyone is interested in.
-        
-        
-        User-Doc
-        -----
-        
-        ### Memory Profiler
-        
-        The memory profiler is a modification of python's `line_profiler`, it gives
-        the memory usage info for each line of code in the specified function/method.
-        
-        #### Sample:
-        
-        ```python
-        import torch
-        from pytorch_memlab import LineProfiler
-        
-        def inner():
-            torch.nn.Linear(100, 100).cuda()
-        
-        def outer():
-            linear = torch.nn.Linear(100, 100).cuda()
-            linear2 = torch.nn.Linear(100, 100).cuda()
-            inner()
-        
-        with LineProfiler(outer, inner) as prof:
-            outer()
-        prof.display()
-        ```
-        
-        After the script finishes or interrupted by keyboard, it gives the following
-        profiling info if you're in a Jupyter notebook:
-        
-        <p align="center"><img src="readme-output.png" width="640"></p>
-        
-        or the following info if you're in a text-only terminal:
-        
-        ```
-        ## outer
-        
-        active_bytes reserved_bytes line  code
-                 all            all
-                peak           peak
-               0.00B          0.00B    7  def outer():
-              40.00K          2.00M    8      linear = torch.nn.Linear(100, 100).cuda()
-              80.00K          2.00M    9      linear2 = torch.nn.Linear(100, 100).cuda()
-             120.00K          2.00M   10      inner()
-        
-        
-        ## inner
-        
-        active_bytes reserved_bytes line  code
-                 all            all
-                peak           peak
-              80.00K          2.00M    4  def inner():
-             120.00K          2.00M    5      torch.nn.Linear(100, 100).cuda()
-        ```
-        
-        An explanation of what each column means can be found in the [Torch documentation](https://pytorch.org/docs/stable/cuda.html#torch.cuda.memory_stats). The name of any field from `memory_stats()`
-        can be passed to `display()` to view the corresponding statistic.
-        
-        If you use `profile` decorator, the memory statistics are collected during
-        multiple runs and only the maximum one is displayed at the end.
-        We also provide a more flexible API called `profile_every` which prints the
-        memory info every *N* times of function execution. You can simply replace
-        `@profile` with `@profile_every(1)` to print the memory usage for each
-        execution.
-        
-        The `@profile` and `@profile_every` can also be mixed to gain more control
-        of the debugging granularity.
-        
-        - You can also add the decorator in the module class:
-        
-        ```python
-        class Net(torch.nn.Module):
-            def __init__(self):
-                super().__init__()
-            @profile
-            def forward(self, inp):
-                #do_something
-        ```
-        
-        - The *Line Profiler* profiles the memory usage of CUDA device 0 by default,
-        you may want to switch the device to profile by `set_target_gpu`. The gpu
-        selection is globally,  which means you have to remember which gpu you are
-        profiling on during the whole process:
-        
-        ```python
-        import torch
-        from pytorch_memlab import profile, set_target_gpu
-        @profile
-        def func():
-            net1 = torch.nn.Linear(1024, 1024).cuda(0)
-            set_target_gpu(1)
-            net2 = torch.nn.Linear(1024, 1024).cuda(1)
-            set_target_gpu(0)
-            net3 = torch.nn.Linear(1024, 1024).cuda(0)
-        
-        func()
-        ```
-        
-        
-        More samples can be found in `test/test_line_profiler.py`
-        
-        ### IPython support
-        
-        Make sure you have `IPython` installed, or have installed `pytorch-memlab` with
-        `pip install pytorch-memlab[ipython]`.
-        
-        First, load the extension:
-        
-        ```python
-        %load_ext pytorch_memlab
-        ```
-        
-        This makes the `%mlrun` and `%%mlrun` line/cell magics available for use. For
-        example, in a new cell run the following to profile an entire cell
-        
-        ```python
-        %%mlrun -f func
-        import torch
-        from pytorch_memlab import profile, set_target_gpu
-        def func():
-            net1 = torch.nn.Linear(1024, 1024).cuda(0)
-            set_target_gpu(1)
-            net2 = torch.nn.Linear(1024, 1024).cuda(1)
-            set_target_gpu(0)
-            net3 = torch.nn.Linear(1024, 1024).cuda(0)
-        ```
-        
-        Or you can invoke the profiler for a single statement on via the `%mlrun` cell
-        magic.
-        
-        ```python
-        import torch
-        from pytorch_memlab import profile, set_target_gpu
-        def func(input_size):
-            net1 = torch.nn.Linear(input_size, 1024).cuda(0)
-        %mlrun -f func func(2048)
-        ```
-        
-        See `%mlrun?` for help on what arguments are supported. You can set the GPU
-        device to profile, dump profiling results to a file, and return the
-        `LineProfiler` object for post-profile inspection.
-        
-        Find out more by checking out the [demo Jupyter notebook](./demo.ipynb)
-        
-        
-        ### Memory Reporter
-        
-        As *Memory Profiler* only gives the overall memory usage information by lines,
-        a more low-level memory usage information can be obtained by *Memory Reporter*.
-        
-        *Memory reporter* iterates all the `Tensor` objects and gets the underlying
-        `Storage` object to get the actual memory usage instead of the surface
-        `Tensor.size`.
-        
-        #### Sample
-        
-        - A minimal one:
-        
-        ```python
-        import torch
-        from pytorch_memlab import MemReporter
-        linear = torch.nn.Linear(1024, 1024).cuda()
-        reporter = MemReporter()
-        reporter.report()
-        ```
-        outputs:
-        ```
-        Element type                                            Size  Used MEM
-        -------------------------------------------------------------------------------
-        Storage on cuda:0
-        Parameter0                                      (1024, 1024)     4.00M
-        Parameter1                                           (1024,)     4.00K
-        -------------------------------------------------------------------------------
-        Total Tensors: 1049600  Used Memory: 4.00M
-        The allocated memory on cuda:0: 4.00M
-        -------------------------------------------------------------------------------
-        ```
-        
-        - You can also pass in a model object for automatically name inference.
-        
-        ```python
-        import torch
-        from pytorch_memlab import MemReporter
-        
-        linear = torch.nn.Linear(1024, 1024).cuda()
-        inp = torch.Tensor(512, 1024).cuda()
-        # pass in a model to automatically infer the tensor names
-        reporter = MemReporter(linear)
-        out = linear(inp).mean()
-        print('========= before backward =========')
-        reporter.report()
-        out.backward()
-        print('========= after backward =========')
-        reporter.report()
-        ```
-        
-        outputs:
-        ```
-        ========= before backward =========
-        Element type                                            Size  Used MEM
-        -------------------------------------------------------------------------------
-        Storage on cuda:0
-        weight                                          (1024, 1024)     4.00M
-        bias                                                 (1024,)     4.00K
-        Tensor0                                          (512, 1024)     2.00M
-        Tensor1                                                 (1,)   512.00B
-        -------------------------------------------------------------------------------
-        Total Tensors: 1573889  Used Memory: 6.00M
-        The allocated memory on cuda:0: 6.00M
-        -------------------------------------------------------------------------------
-        ========= after backward =========
-        Element type                                            Size  Used MEM
-        -------------------------------------------------------------------------------
-        Storage on cuda:0
-        weight                                          (1024, 1024)     4.00M
-        weight.grad                                     (1024, 1024)     4.00M
-        bias                                                 (1024,)     4.00K
-        bias.grad                                            (1024,)     4.00K
-        Tensor0                                          (512, 1024)     2.00M
-        Tensor1                                                 (1,)   512.00B
-        -------------------------------------------------------------------------------
-        Total Tensors: 2623489  Used Memory: 10.01M
-        The allocated memory on cuda:0: 10.01M
-        -------------------------------------------------------------------------------
-        ```
-        
-        
-        - The reporter automatically deals with the sharing weights parameters:
-        
-        ```python
-        import torch
-        from pytorch_memlab import MemReporter
-        
-        linear = torch.nn.Linear(1024, 1024).cuda()
-        linear2 = torch.nn.Linear(1024, 1024).cuda()
-        linear2.weight = linear.weight
-        container = torch.nn.Sequential(
-            linear, linear2
-        )
-        inp = torch.Tensor(512, 1024).cuda()
-        # pass in a model to automatically infer the tensor names
-        
-        out = container(inp).mean()
-        out.backward()
-        
-        # verbose shows how storage is shared across multiple Tensors
-        reporter = MemReporter(container)
-        reporter.report(verbose=True)
-        ```
-        
-        outputs:
-        ```
-        Element type                                            Size  Used MEM
-        -------------------------------------------------------------------------------
-        Storage on cuda:0
-        0.weight                                        (1024, 1024)     4.00M
-        0.weight.grad                                   (1024, 1024)     4.00M
-        0.bias                                               (1024,)     4.00K
-        0.bias.grad                                          (1024,)     4.00K
-        1.bias                                               (1024,)     4.00K
-        1.bias.grad                                          (1024,)     4.00K
-        Tensor0                                          (512, 1024)     2.00M
-        Tensor1                                                 (1,)   512.00B
-        -------------------------------------------------------------------------------
-        Total Tensors: 2625537  Used Memory: 10.02M
-        The allocated memory on cuda:0: 10.02M
-        -------------------------------------------------------------------------------
-        ```
-        
-        - You can better understand the memory layout for more complicated module:
-        
-        ```python
-        import torch
-        from pytorch_memlab import MemReporter
-        
-        lstm = torch.nn.LSTM(1024, 1024).cuda()
-        reporter = MemReporter(lstm)
-        reporter.report(verbose=True)
-        inp = torch.Tensor(10, 10, 1024).cuda()
-        out, _ = lstm(inp)
-        out.mean().backward()
-        reporter.report(verbose=True)
-        ```
-        
-        As shown below, the `(->)` indicates the re-use of the same storage back-end
-        outputs:
-        ```
-        Element type                                            Size  Used MEM
-        -------------------------------------------------------------------------------
-        Storage on cuda:0
-        weight_ih_l0                                    (4096, 1024)    32.03M
-        weight_hh_l0(->weight_ih_l0)                    (4096, 1024)     0.00B
-        bias_ih_l0(->weight_ih_l0)                           (4096,)     0.00B
-        bias_hh_l0(->weight_ih_l0)                           (4096,)     0.00B
-        Tensor0                                       (10, 10, 1024)   400.00K
-        -------------------------------------------------------------------------------
-        Total Tensors: 8499200  Used Memory: 32.42M
-        The allocated memory on cuda:0: 32.52M
-        Memory differs due to the matrix alignment
-        -------------------------------------------------------------------------------
-        Element type                                            Size  Used MEM
-        -------------------------------------------------------------------------------
-        Storage on cuda:0
-        weight_ih_l0                                    (4096, 1024)    32.03M
-        weight_ih_l0.grad                               (4096, 1024)    32.03M
-        weight_hh_l0(->weight_ih_l0)                    (4096, 1024)     0.00B
-        weight_hh_l0.grad(->weight_ih_l0.grad)          (4096, 1024)     0.00B
-        bias_ih_l0(->weight_ih_l0)                           (4096,)     0.00B
-        bias_ih_l0.grad(->weight_ih_l0.grad)                 (4096,)     0.00B
-        bias_hh_l0(->weight_ih_l0)                           (4096,)     0.00B
-        bias_hh_l0.grad(->weight_ih_l0.grad)                 (4096,)     0.00B
-        Tensor0                                       (10, 10, 1024)   400.00K
-        Tensor1                                       (10, 10, 1024)   400.00K
-        Tensor2                                        (1, 10, 1024)    40.00K
-        Tensor3                                        (1, 10, 1024)    40.00K
-        -------------------------------------------------------------------------------
-        Total Tensors: 17018880         Used Memory: 64.92M
-        The allocated memory on cuda:0: 65.11M
-        Memory differs due to the matrix alignment
-        -------------------------------------------------------------------------------
-        ```
-        
-        NOTICE:
-        > When forwarding with `grad_mode=True`, pytorch maintains tensor buffers for
-        > future Back-Propagation, in C level. So these buffers are not going to be
-        > managed or collected by pytorch. But if you store these intermediate results
-        > as python variables, then they will be reported.
-        
-        - You can also filter the device to report on by passing extra arguments:
-        `report(device=torch.device(0))`
-        
-        - A failed example due to pytorch's C side tensor buffers
-        
-        In the following example, a temp buffer is created at `inp * (inp + 2)` to
-        store both `inp` and `inp + 2`, unfortunately python only knows the existence
-        of inp, so we have *2M* memory lost, which is the same size of Tensor `inp`.
-        
-        ```python
-        import torch
-        from pytorch_memlab import MemReporter
-        
-        linear = torch.nn.Linear(1024, 1024).cuda()
-        inp = torch.Tensor(512, 1024).cuda()
-        # pass in a model to automatically infer the tensor names
-        reporter = MemReporter(linear)
-        out = linear(inp * (inp + 2)).mean()
-        reporter.report()
-        ```
-        
-        outputs:
-        ```
-        Element type                                            Size  Used MEM
-        -------------------------------------------------------------------------------
-        Storage on cuda:0
-        weight                                          (1024, 1024)     4.00M
-        bias                                                 (1024,)     4.00K
-        Tensor0                                          (512, 1024)     2.00M
-        Tensor1                                                 (1,)   512.00B
-        -------------------------------------------------------------------------------
-        Total Tensors: 1573889  Used Memory: 6.00M
-        The allocated memory on cuda:0: 8.00M
-        Memory differs due to the matrix alignment or invisible gradient buffer tensors
-        -------------------------------------------------------------------------------
-        ```
-        
-        
-        ### Courtesy
-        
-        Sometimes people would like to preempt your running task, but you don't want
-        to save checkpoint and then load, actually all they need is GPU resources (
-        typically CPU resources and CPU memory is always spare in GPU clusters), so
-        you can move all your workspaces from GPU to CPU and then halt your task until
-        a restart signal is triggered, instead of saving&loading checkpoints and
-        bootstrapping from scratch.
-        
-        Still developing..... But you can have fun with:
-        ```python
-        from pytorch_memlab import Courtesy
-        
-        iamcourtesy = Courtesy()
-        for i in range(num_iteration):
-            if something_happens:
-                iamcourtesy.yield_memory()
-                wait_for_restart_signal()
-                iamcourtesy.restore()
-        ```
-        
-        #### Known Issues
-        
-        - As is stated above in `Memory_Reporter`, intermediate tensors are not covered
-        properly, so you may want to insert such courtesy logics after `backward` or
-        before `forward`.
-        - Currently the CUDA context of pytorch requires about 1 GB CUDA memory, which
-        means even all Tensors are on CPU, 1GB of CUDA memory is wasted, :-(. However
-        it's still under investigation if I can fully destroy the context and then
-        re-init.
-        
-        
-        ### ACK
-        
-        I suffered a lot debugging weird memory usage during my 3-years of developing
-        efficient Deep Learning models, and of course learned a lot from the great
-        open source community.
-        
-        ## CHANGES
-        
-        
-        ##### 0.2.4 (2021-10-28)
-          - Fix colab error (#35)
-          - Support python3.8 (#38)
-          - Support sparse tensor (#30)
-        ##### 0.2.3 (2020-12-01)
-          - Fix name mapping in `MemReporter` (#24)
-          - Fix reporter without model input (#22 #25)
-        ##### 0.2.2 (2020-10-23)
-          - Fix memory leak in `MemReporter`
-        ##### 0.2.1 (2020-06-18)
-          - Fix `line_profiler` not found
-        ##### 0.2.0 (2020-06-15)
-          - Add jupyter notebook figure and ipython support
-        ##### 0.1.0 (2020-04-17)
-          - Add ipython magic support (#8)
-        ##### 0.0.4 (2019-10-08)
-          - Add gpu switch for line-profiler(#2)
-          - Add device filter for reporter
-        ##### 0.0.3 (2019-06-15)
-          - Install dependency for pip installation
-        ##### 0.0.2 (2019-06-04)
-          - Fix statistics shift in loop
-        ##### 0.0.1 (2019-05-28)
-          - initial release
-        
-Keywords: pytorch memory profile
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-Provides-Extra: ipython
-Provides-Extra: test
+pytorch_memlab
+======
+[![Build Status](https://travis-ci.com/Stonesjtu/pytorch_memlab.svg?token=vyTdxHbi1PCRzV6disHp&branch=master)](https://travis-ci.com/Stonesjtu/pytorch_memlab)
+![PyPI](https://img.shields.io/pypi/v/pytorch_memlab.svg)
+[![CodeQL: Python](https://github.com/Stonesjtu/pytorch_memlab/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/Stonesjtu/pytorch_memlab/actions/workflows/github-code-scanning/codeql)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pytorch_memlab.svg)
+
+A simple and accurate **CUDA** memory management laboratory for pytorch,
+it consists of different parts about the memory:
+
+- Features:
+
+  - Memory Profiler: A `line_profiler` style CUDA memory profiler with simple API.
+  - Memory Reporter: A reporter to inspect tensors occupying the CUDA memory.
+  - Courtesy: An interesting feature to temporarily move all the CUDA tensors into
+    CPU memory for courtesy, and of course the backward transferring.
+  - IPython support through `%mlrun`/`%%mlrun` line/cell magic
+    commands.
+
+
+- Table of Contents
+  * [Installation](#installation)
+  * [User-Doc](#user-doc)
+    + [Memory Profiler](#memory-profiler)
+    + [IPython support](#ipython-support)
+    + [Memory Reporter](#memory-reporter)
+    + [Courtesy](#courtesy)
+    + [ACK](#ack)
+  * [CHANGES](#changes)
+
+Installation
+-----
+
+- Released version:
+```bash
+pip install pytorch_memlab
+```
+
+- Newest version:
+```bash
+pip install git+https://github.com/stonesjtu/pytorch_memlab
+```
+
+What's for
+-----
+
+Out-Of-Memory errors in pytorch happen frequently, for new-bees and
+experienced programmers. A common reason is that most people don't really
+learn the underlying memory management philosophy of pytorch and GPUs.
+They wrote memory in-efficient codes and complained about pytorch eating too
+much CUDA memory.
+
+In this repo, I'm going to share some useful tools to help debugging OOM, or
+to inspect the underlying mechanism if anyone is interested in.
+
+
+User-Doc
+-----
+
+### Memory Profiler
+
+The memory profiler is a modification of python's `line_profiler`, it gives
+the memory usage info for each line of code in the specified function/method.
+
+#### Sample:
+
+```python
+import torch
+from pytorch_memlab import LineProfiler
+
+def inner():
+    torch.nn.Linear(100, 100).cuda()
+
+def outer():
+    linear = torch.nn.Linear(100, 100).cuda()
+    linear2 = torch.nn.Linear(100, 100).cuda()
+    linear3 = torch.nn.Linear(100, 100).cuda()
+
+work()
+```
+
+After the script finishes or interrupted by keyboard, it gives the following
+profiling info if you're in a Jupyter notebook:
+
+<p align="center"><img src="readme-output.png" width="640"></p>
+
+or the following info if you're in a text-only terminal:
+
+```
+## outer
+
+active_bytes reserved_bytes line  code
+         all            all
+        peak           peak
+       0.00B          0.00B    7  def outer():
+      40.00K          2.00M    8      linear = torch.nn.Linear(100, 100).cuda()
+      80.00K          2.00M    9      linear2 = torch.nn.Linear(100, 100).cuda()
+     120.00K          2.00M   10      inner()
+
+
+## inner
+
+active_bytes reserved_bytes line  code
+         all            all
+        peak           peak
+      80.00K          2.00M    4  def inner():
+     120.00K          2.00M    5      torch.nn.Linear(100, 100).cuda()
+```
+
+An explanation of what each column means can be found in the [Torch documentation](https://pytorch.org/docs/stable/cuda.html#torch.cuda.memory_stats). The name of any field from `memory_stats()`
+can be passed to `display()` to view the corresponding statistic.
+
+If you use `profile` decorator, the memory statistics are collected during
+multiple runs and only the maximum one is displayed at the end.
+We also provide a more flexible API called `profile_every` which prints the
+memory info every *N* times of function execution. You can simply replace
+`@profile` with `@profile_every(1)` to print the memory usage for each
+execution.
+
+The `@profile` and `@profile_every` can also be mixed to gain more control
+of the debugging granularity.
+
+- You can also add the decorator in the module class:
+
+```python
+class Net(torch.nn.Module):
+    def __init__(self):
+        super().__init__()
+    @profile
+    def forward(self, inp):
+        #do_something
+```
+
+- The *Line Profiler* profiles the memory usage of CUDA device 0 by default,
+you may want to switch the device to profile by `set_target_gpu`. The gpu
+selection is globally,  which means you have to remember which gpu you are
+profiling on during the whole process:
+
+```python
+import torch
+from pytorch_memlab import profile, set_target_gpu
+@profile
+def func():
+    net1 = torch.nn.Linear(1024, 1024).cuda(0)
+    set_target_gpu(1)
+    net2 = torch.nn.Linear(1024, 1024).cuda(1)
+    set_target_gpu(0)
+    net3 = torch.nn.Linear(1024, 1024).cuda(0)
+
+func()
+```
+
+
+More samples can be found in `test/test_line_profiler.py`
+
+### IPython support
+
+Make sure you have `IPython` installed, or have installed `pytorch-memlab` with
+`pip install pytorch-memlab[ipython]`.
+
+First, load the extension:
+
+```python
+%load_ext pytorch_memlab
+```
+
+This makes the `%mlrun` and `%%mlrun` line/cell magics available for use. For
+example, in a new cell run the following to profile an entire cell
+
+```python
+%%mlrun -f func
+import torch
+from pytorch_memlab import profile, set_target_gpu
+def func():
+    net1 = torch.nn.Linear(1024, 1024).cuda(0)
+    set_target_gpu(1)
+    net2 = torch.nn.Linear(1024, 1024).cuda(1)
+    set_target_gpu(0)
+    net3 = torch.nn.Linear(1024, 1024).cuda(0)
+```
+
+Or you can invoke the profiler for a single statement on via the `%mlrun` cell
+magic.
+
+```python
+import torch
+from pytorch_memlab import profile, set_target_gpu
+def func(input_size):
+    net1 = torch.nn.Linear(input_size, 1024).cuda(0)
+%mlrun -f func func(2048)
+```
+
+See `%mlrun?` for help on what arguments are supported. You can set the GPU
+device to profile, dump profiling results to a file, and return the
+`LineProfiler` object for post-profile inspection.
+
+Find out more by checking out the [demo Jupyter notebook](./demo.ipynb)
+
+
+### Memory Reporter
+
+As *Memory Profiler* only gives the overall memory usage information by lines,
+a more low-level memory usage information can be obtained by *Memory Reporter*.
+
+*Memory reporter* iterates all the `Tensor` objects and gets the underlying
+`Storage` object to get the actual memory usage instead of the surface
+`Tensor.size`.
+
+#### Sample
+
+- A minimal one:
+
+```python
+import torch
+from pytorch_memlab import MemReporter
+linear = torch.nn.Linear(1024, 1024).cuda()
+reporter = MemReporter()
+reporter.report()
+```
+outputs:
+```
+Element type                                            Size  Used MEM
+-------------------------------------------------------------------------------
+Storage on cuda:0
+Parameter0                                      (1024, 1024)     4.00M
+Parameter1                                           (1024,)     4.00K
+-------------------------------------------------------------------------------
+Total Tensors: 1049600  Used Memory: 4.00M
+The allocated memory on cuda:0: 4.00M
+-------------------------------------------------------------------------------
+```
+
+- You can also pass in a model object for automatically name inference.
+
+```python
+import torch
+from pytorch_memlab import MemReporter
+
+linear = torch.nn.Linear(1024, 1024).cuda()
+inp = torch.Tensor(512, 1024).cuda()
+# pass in a model to automatically infer the tensor names
+reporter = MemReporter(linear)
+out = linear(inp).mean()
+print('========= before backward =========')
+reporter.report()
+out.backward()
+print('========= after backward =========')
+reporter.report()
+```
+
+outputs:
+```
+========= before backward =========
+Element type                                            Size  Used MEM
+-------------------------------------------------------------------------------
+Storage on cuda:0
+weight                                          (1024, 1024)     4.00M
+bias                                                 (1024,)     4.00K
+Tensor0                                          (512, 1024)     2.00M
+Tensor1                                                 (1,)   512.00B
+-------------------------------------------------------------------------------
+Total Tensors: 1573889  Used Memory: 6.00M
+The allocated memory on cuda:0: 6.00M
+-------------------------------------------------------------------------------
+========= after backward =========
+Element type                                            Size  Used MEM
+-------------------------------------------------------------------------------
+Storage on cuda:0
+weight                                          (1024, 1024)     4.00M
+weight.grad                                     (1024, 1024)     4.00M
+bias                                                 (1024,)     4.00K
+bias.grad                                            (1024,)     4.00K
+Tensor0                                          (512, 1024)     2.00M
+Tensor1                                                 (1,)   512.00B
+-------------------------------------------------------------------------------
+Total Tensors: 2623489  Used Memory: 10.01M
+The allocated memory on cuda:0: 10.01M
+-------------------------------------------------------------------------------
+```
+
+
+- The reporter automatically deals with the sharing weights parameters:
+
+```python
+import torch
+from pytorch_memlab import MemReporter
+
+linear = torch.nn.Linear(1024, 1024).cuda()
+linear2 = torch.nn.Linear(1024, 1024).cuda()
+linear2.weight = linear.weight
+container = torch.nn.Sequential(
+    linear, linear2
+)
+inp = torch.Tensor(512, 1024).cuda()
+# pass in a model to automatically infer the tensor names
+
+out = container(inp).mean()
+out.backward()
+
+# verbose shows how storage is shared across multiple Tensors
+reporter = MemReporter(container)
+reporter.report(verbose=True)
+```
+
+outputs:
+```
+Element type                                            Size  Used MEM
+-------------------------------------------------------------------------------
+Storage on cuda:0
+0.weight                                        (1024, 1024)     4.00M
+0.weight.grad                                   (1024, 1024)     4.00M
+0.bias                                               (1024,)     4.00K
+0.bias.grad                                          (1024,)     4.00K
+1.bias                                               (1024,)     4.00K
+1.bias.grad                                          (1024,)     4.00K
+Tensor0                                          (512, 1024)     2.00M
+Tensor1                                                 (1,)   512.00B
+-------------------------------------------------------------------------------
+Total Tensors: 2625537  Used Memory: 10.02M
+The allocated memory on cuda:0: 10.02M
+-------------------------------------------------------------------------------
+```
+
+- You can better understand the memory layout for more complicated module:
+
+```python
+import torch
+from pytorch_memlab import MemReporter
+
+lstm = torch.nn.LSTM(1024, 1024).cuda()
+reporter = MemReporter(lstm)
+reporter.report(verbose=True)
+inp = torch.Tensor(10, 10, 1024).cuda()
+out, _ = lstm(inp)
+out.mean().backward()
+reporter.report(verbose=True)
+```
+
+As shown below, the `(->)` indicates the re-use of the same storage back-end
+outputs:
+```
+Element type                                            Size  Used MEM
+-------------------------------------------------------------------------------
+Storage on cuda:0
+weight_ih_l0                                    (4096, 1024)    32.03M
+weight_hh_l0(->weight_ih_l0)                    (4096, 1024)     0.00B
+bias_ih_l0(->weight_ih_l0)                           (4096,)     0.00B
+bias_hh_l0(->weight_ih_l0)                           (4096,)     0.00B
+Tensor0                                       (10, 10, 1024)   400.00K
+-------------------------------------------------------------------------------
+Total Tensors: 8499200  Used Memory: 32.42M
+The allocated memory on cuda:0: 32.52M
+Memory differs due to the matrix alignment
+-------------------------------------------------------------------------------
+Element type                                            Size  Used MEM
+-------------------------------------------------------------------------------
+Storage on cuda:0
+weight_ih_l0                                    (4096, 1024)    32.03M
+weight_ih_l0.grad                               (4096, 1024)    32.03M
+weight_hh_l0(->weight_ih_l0)                    (4096, 1024)     0.00B
+weight_hh_l0.grad(->weight_ih_l0.grad)          (4096, 1024)     0.00B
+bias_ih_l0(->weight_ih_l0)                           (4096,)     0.00B
+bias_ih_l0.grad(->weight_ih_l0.grad)                 (4096,)     0.00B
+bias_hh_l0(->weight_ih_l0)                           (4096,)     0.00B
+bias_hh_l0.grad(->weight_ih_l0.grad)                 (4096,)     0.00B
+Tensor0                                       (10, 10, 1024)   400.00K
+Tensor1                                       (10, 10, 1024)   400.00K
+Tensor2                                        (1, 10, 1024)    40.00K
+Tensor3                                        (1, 10, 1024)    40.00K
+-------------------------------------------------------------------------------
+Total Tensors: 17018880         Used Memory: 64.92M
+The allocated memory on cuda:0: 65.11M
+Memory differs due to the matrix alignment
+-------------------------------------------------------------------------------
+```
+
+NOTICE:
+> When forwarding with `grad_mode=True`, pytorch maintains tensor buffers for
+> future Back-Propagation, in C level. So these buffers are not going to be
+> managed or collected by pytorch. But if you store these intermediate results
+> as python variables, then they will be reported.
+
+- You can also filter the device to report on by passing extra arguments:
+`report(device=torch.device(0))`
+
+- A failed example due to pytorch's C side tensor buffers
+
+In the following example, a temp buffer is created at `inp * (inp + 2)` to
+store both `inp` and `inp + 2`, unfortunately python only knows the existence
+of inp, so we have *2M* memory lost, which is the same size of Tensor `inp`.
+
+```python
+import torch
+from pytorch_memlab import MemReporter
+
+linear = torch.nn.Linear(1024, 1024).cuda()
+inp = torch.Tensor(512, 1024).cuda()
+# pass in a model to automatically infer the tensor names
+reporter = MemReporter(linear)
+out = linear(inp * (inp + 2)).mean()
+reporter.report()
+```
+
+outputs:
+```
+Element type                                            Size  Used MEM
+-------------------------------------------------------------------------------
+Storage on cuda:0
+weight                                          (1024, 1024)     4.00M
+bias                                                 (1024,)     4.00K
+Tensor0                                          (512, 1024)     2.00M
+Tensor1                                                 (1,)   512.00B
+-------------------------------------------------------------------------------
+Total Tensors: 1573889  Used Memory: 6.00M
+The allocated memory on cuda:0: 8.00M
+Memory differs due to the matrix alignment or invisible gradient buffer tensors
+-------------------------------------------------------------------------------
+```
+
+
+### Courtesy
+
+Sometimes people would like to preempt your running task, but you don't want
+to save checkpoint and then load, actually all they need is GPU resources (
+typically CPU resources and CPU memory is always spare in GPU clusters), so
+you can move all your workspaces from GPU to CPU and then halt your task until
+a restart signal is triggered, instead of saving&loading checkpoints and
+bootstrapping from scratch.
+
+Still developing..... But you can have fun with:
+```python
+from pytorch_memlab import Courtesy
+
+iamcourtesy = Courtesy()
+for i in range(num_iteration):
+    if something_happens:
+        iamcourtesy.yield_memory()
+        wait_for_restart_signal()
+        iamcourtesy.restore()
+```
+
+#### Known Issues
+
+- As is stated above in `Memory_Reporter`, intermediate tensors are not covered
+properly, so you may want to insert such courtesy logics after `backward` or
+before `forward`.
+- Currently the CUDA context of pytorch requires about 1 GB CUDA memory, which
+means even all Tensors are on CPU, 1GB of CUDA memory is wasted, :-(. However
+it's still under investigation if I can fully destroy the context and then
+re-init.
+
+
+### ACK
+
+I suffered a lot debugging weird memory usage during my 3-years of developing
+efficient Deep Learning models, and of course learned a lot from the great
+open source community.
+
+## CHANGES
+
+
+##### 0.2.4 (2021-10-28)
+  - Fix colab error (#35)
+  - Support python3.8 (#38)
+  - Support sparse tensor (#30)
+##### 0.2.3 (2020-12-01)
+  - Fix name mapping in `MemReporter` (#24)
+  - Fix reporter without model input (#22 #25)
+##### 0.2.2 (2020-10-23)
+  - Fix memory leak in `MemReporter`
+##### 0.2.1 (2020-06-18)
+  - Fix `line_profiler` not found
+##### 0.2.0 (2020-06-15)
+  - Add jupyter notebook figure and ipython support
+##### 0.1.0 (2020-04-17)
+  - Add ipython magic support (#8)
+##### 0.0.4 (2019-10-08)
+  - Add gpu switch for line-profiler(#2)
+  - Add device filter for reporter
+##### 0.0.3 (2019-06-15)
+  - Install dependency for pip installation
+##### 0.0.2 (2019-06-04)
+  - Fix statistics shift in loop
+##### 0.0.1 (2019-05-28)
+  - initial release
```

### Comparing `pytorch_memlab-0.2.4/README.md` & `pytorch-memlab-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,30 @@
+Metadata-Version: 2.1
+Name: pytorch-memlab
+Version: 0.3.0
+Summary: A lab to do simple and accurate memory experiments on pytorch
+Home-page: https://github.com/Stonesjtu/pytorch_memlab
+Author: Kaiyu Shi
+Author-email: skyisno.1@gmail.com
+License: MIT
+Keywords: pytorch memory profile
+Platform: UNKNOWN
+Classifier: Programming Language :: Python
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+Provides-Extra: ipython
+Provides-Extra: test
+License-File: LICENSE
+License-File: LICENSE_kernprof.txt
+
 pytorch_memlab
 ======
 [![Build Status](https://travis-ci.com/Stonesjtu/pytorch_memlab.svg?token=vyTdxHbi1PCRzV6disHp&branch=master)](https://travis-ci.com/Stonesjtu/pytorch_memlab)
 ![PyPI](https://img.shields.io/pypi/v/pytorch_memlab.svg)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/Stonesjtu/pytorch_memlab.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Stonesjtu/pytorch_memlab/context:python)
+[![CodeQL: Python](https://github.com/Stonesjtu/pytorch_memlab/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/Stonesjtu/pytorch_memlab/actions/workflows/github-code-scanning/codeql)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pytorch_memlab.svg)
 
 A simple and accurate **CUDA** memory management laboratory for pytorch,
 it consists of different parts about the memory:
 
 - Features:
 
@@ -70,19 +88,17 @@
 
 def inner():
     torch.nn.Linear(100, 100).cuda()
 
 def outer():
     linear = torch.nn.Linear(100, 100).cuda()
     linear2 = torch.nn.Linear(100, 100).cuda()
-    inner()
+    linear3 = torch.nn.Linear(100, 100).cuda()
 
-with LineProfiler(outer, inner) as prof:
-    outer()
-prof.display()
+work()
 ```
 
 After the script finishes or interrupted by keyboard, it gives the following
 profiling info if you're in a Jupyter notebook:
 
 <p align="center"><img src="readme-output.png" width="640"></p>
 
@@ -481,7 +497,9 @@
   - Add device filter for reporter
 ##### 0.0.3 (2019-06-15)
   - Install dependency for pip installation
 ##### 0.0.2 (2019-06-04)
   - Fix statistics shift in loop
 ##### 0.0.1 (2019-05-28)
   - initial release
+
+
```

### Comparing `pytorch_memlab-0.2.4/pytorch_memlab/courtesy.py` & `pytorch-memlab-0.3.0/pytorch_memlab/courtesy.py`

 * *Files identical despite different names*

### Comparing `pytorch_memlab-0.2.4/pytorch_memlab/line_profiler/extension.py` & `pytorch-memlab-0.3.0/pytorch_memlab/line_profiler/extension.py`

 * *Files identical despite different names*

### Comparing `pytorch_memlab-0.2.4/pytorch_memlab/line_profiler/line_profiler.py` & `pytorch-memlab-0.3.0/pytorch_memlab/line_profiler/line_profiler.py`

 * *Files identical despite different names*

### Comparing `pytorch_memlab-0.2.4/pytorch_memlab/line_profiler/line_records.py` & `pytorch-memlab-0.3.0/pytorch_memlab/line_profiler/line_records.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     `_accumulate_line_records` docstring for more detail."""
     # Column spec: https://pytorch.org/docs/stable/cuda.html#torch.cuda.memory_stats
     qual_names = {
         code_hash: info['func'].__qualname__ for code_hash, info in code_infos.items()}
     records = (_accumulate_line_records(raw_line_records)
                .assign(qual_name=lambda df: df.code_hash.map(qual_names))
                .set_index(['qual_name', 'line'])
-               .drop(['code_hash', 'num_alloc_retries', 'num_ooms', 'prev_record_idx'], 1))
+               .drop(['code_hash', 'num_alloc_retries', 'num_ooms', 'prev_record_idx'], axis=1))
     records.columns = pd.MultiIndex.from_tuples(
         [c.split('.') for c in records.columns])
 
     return records
 
 
 class LineRecords:
@@ -182,15 +182,15 @@
             maxlen = max(len(c) for c in merged.code)
             left_align = '{{:{maxlen}s}}'.format(maxlen=maxlen)
             merged[byte_cols] = merged[byte_cols].applymap(readable_size)
 
             # This is a mess, but I can't find any other way to left-align text strings.
             code_header = (left_align.format('code'), '', '')
             merged[code_header] = merged['code'].apply(lambda l: left_align.format(l.rstrip('\n\r')))
-            merged = merged.drop('code', 1, level=0)
+            merged = merged.drop('code', axis=1, level=0)
 
             string[qual_name] = merged.to_string(index=False)
 
         return '\n\n'.join(['## {q}\n\n{c}\n'.format(q=q, c=c) for q, c in string.items()])
 
     def _repr_html_(self):
         """Renders the stats as HTML"""
```

### Comparing `pytorch_memlab-0.2.4/pytorch_memlab/line_profiler/profile.py` & `pytorch-memlab-0.3.0/pytorch_memlab/line_profiler/profile.py`

 * *Files identical despite different names*

### Comparing `pytorch_memlab-0.2.4/pytorch_memlab/mem_reporter.py` & `pytorch-memlab-0.3.0/pytorch_memlab/mem_reporter.py`

 * *Files identical despite different names*

### Comparing `pytorch_memlab-0.2.4/pytorch_memlab.egg-info/SOURCES.txt` & `pytorch-memlab-0.3.0/pytorch_memlab.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,11 @@
-.gitignore
 LICENSE
 LICENSE_kernprof.txt
 README.md
-demo.ipynb
-readme-output.png
-requirements.txt
 setup.py
-.github/workflows/pypi-publish.yml
-.github/workflows/test.yml
 pytorch_memlab/__init__.py
 pytorch_memlab/courtesy.py
 pytorch_memlab/mem_reporter.py
 pytorch_memlab/utils.py
 pytorch_memlab.egg-info/PKG-INFO
 pytorch_memlab.egg-info/SOURCES.txt
 pytorch_memlab.egg-info/dependency_links.txt
@@ -20,11 +14,10 @@
 pytorch_memlab.egg-info/zip-safe
 pytorch_memlab/line_profiler/__init__.py
 pytorch_memlab/line_profiler/extension.py
 pytorch_memlab/line_profiler/line_profiler.py
 pytorch_memlab/line_profiler/line_records.py
 pytorch_memlab/line_profiler/profile.py
 test/__init__.py
-test/demo.py
 test/test_courtesy.py
 test/test_line_profiler.py
 test/test_mem_reporter.py
```

### Comparing `pytorch_memlab-0.2.4/setup.py` & `pytorch-memlab-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 try:
     long_description = open('README.md').read()
 except FileNotFoundError:
     long_description = ''
 
 setup(
-    name='pytorch_memlab',
-    version='0.2.4',
+    name='pytorch-memlab',
+    version='0.3.0',
     licence='MIT',
     description='A lab to do simple and accurate memory experiments on pytorch',
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         "Programming Language :: Python",
         "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `pytorch_memlab-0.2.4/test/test_courtesy.py` & `pytorch-memlab-0.3.0/test/test_courtesy.py`

 * *Files identical despite different names*

### Comparing `pytorch_memlab-0.2.4/test/test_line_profiler.py` & `pytorch-memlab-0.3.0/test/test_line_profiler.py`

 * *Files identical despite different names*

### Comparing `pytorch_memlab-0.2.4/test/test_mem_reporter.py` & `pytorch-memlab-0.3.0/test/test_mem_reporter.py`

 * *Files identical despite different names*

