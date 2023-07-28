# Comparing `tmp/pueda-0.1.6.tar.gz` & `tmp/pueda-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pueda-0.1.6.tar", last modified: Sun Jul 23 15:36:31 2023, max compression
+gzip compressed data, was "pueda-0.1.7.tar", last modified: Fri Jul 28 22:14:39 2023, max compression
```

## Comparing `pueda-0.1.6.tar` & `pueda-0.1.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-07-23 15:36:31.860701 pueda-0.1.6/
--rwxrwxrwx   0 marco     (1000) marco     (1000)    11357 2022-12-10 01:01:26.000000 pueda-0.1.6/LICENSE
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2267 2023-07-23 15:36:31.861025 pueda-0.1.6/PKG-INFO
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1923 2023-02-27 23:28:27.000000 pueda-0.1.6/README.md
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-07-23 15:36:31.804370 pueda-0.1.6/data/
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-07-23 15:36:31.806531 pueda-0.1.6/data/icarus/
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-07-23 15:36:31.816916 pueda-0.1.6/data/icarus/inc/
--rwxrwxrwx   0 marco     (1000) marco     (1000)       88 2023-02-26 23:04:23.000000 pueda-0.1.6/data/icarus/inc/dump.vh
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-07-23 15:36:31.818115 pueda-0.1.6/data/icarus/src/
--rwxrwxrwx   0 marco     (1000) marco     (1000)      296 2023-02-26 23:04:23.000000 pueda-0.1.6/data/icarus/src/dump.v
--rwxrwxrwx   0 marco     (1000) marco     (1000)      103 2023-07-23 15:36:31.862339 pueda-0.1.6/setup.cfg
--rwxrwxrwx   0 marco     (1000) marco     (1000)      963 2023-07-23 15:33:11.000000 pueda-0.1.6/setup.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-07-23 15:36:31.807834 pueda-0.1.6/src/
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-07-23 15:36:31.836585 pueda-0.1.6/src/pueda/
--rwxrwxrwx   0 marco     (1000) marco     (1000)      150 2023-03-15 01:01:16.000000 pueda-0.1.6/src/pueda/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     3092 2023-03-15 01:37:00.000000 pueda-0.1.6/src/pueda/common.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     7433 2023-03-26 15:13:03.000000 pueda-0.1.6/src/pueda/edalize.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      866 2023-02-27 22:13:51.000000 pueda-0.1.6/src/pueda/gtkw.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2924 2023-03-15 02:15:01.000000 pueda-0.1.6/src/pueda/icarus.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     4934 2023-03-15 01:37:22.000000 pueda-0.1.6/src/pueda/myhdl.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2159 2023-07-23 15:32:32.000000 pueda-0.1.6/src/pueda/pyverilator.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1688 2023-03-15 01:49:00.000000 pueda-0.1.6/src/pueda/vcd.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      325 2023-01-22 17:37:49.000000 pueda-0.1.6/src/pueda/veriloggen.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1376 2023-02-28 20:52:57.000000 pueda-0.1.6/src/pueda/yosys.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-07-23 15:36:31.850012 pueda-0.1.6/src/pueda.egg-info/
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2267 2023-07-23 15:36:31.000000 pueda-0.1.6/src/pueda.egg-info/PKG-INFO
--rwxrwxrwx   0 marco     (1000) marco     (1000)      558 2023-07-23 15:36:31.000000 pueda-0.1.6/src/pueda.egg-info/SOURCES.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)        1 2023-07-23 15:36:31.000000 pueda-0.1.6/src/pueda.egg-info/dependency_links.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)       69 2023-07-23 15:36:31.000000 pueda-0.1.6/src/pueda.egg-info/requires.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)        6 2023-07-23 15:36:31.000000 pueda-0.1.6/src/pueda.egg-info/top_level.txt
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-07-23 15:36:31.859371 pueda-0.1.6/test/
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1384 2023-06-14 20:13:34.000000 pueda-0.1.6/test/test.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1162 2023-02-27 20:41:20.000000 pueda-0.1.6/test/test_myhdl_counter.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      463 2023-02-27 20:41:20.000000 pueda-0.1.6/test/test_verilated_dpi_counter.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      454 2023-02-27 20:41:20.000000 pueda-0.1.6/test/test_verilator_counter.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-07-28 22:14:39.983189 pueda-0.1.7/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)    11357 2022-12-10 01:01:26.000000 pueda-0.1.7/LICENSE
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2267 2023-07-28 22:14:39.983608 pueda-0.1.7/PKG-INFO
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1923 2023-02-27 23:28:27.000000 pueda-0.1.7/README.md
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-07-28 22:14:39.925870 pueda-0.1.7/data/
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-07-28 22:14:39.926981 pueda-0.1.7/data/icarus/
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-07-28 22:14:39.938355 pueda-0.1.7/data/icarus/inc/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)       88 2023-02-26 23:04:23.000000 pueda-0.1.7/data/icarus/inc/dump.vh
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-07-28 22:14:39.940600 pueda-0.1.7/data/icarus/src/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      296 2023-02-26 23:04:23.000000 pueda-0.1.7/data/icarus/src/dump.v
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      103 2023-07-28 22:14:39.992885 pueda-0.1.7/setup.cfg
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      963 2023-07-28 21:44:08.000000 pueda-0.1.7/setup.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-07-28 22:14:39.928709 pueda-0.1.7/src/
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-07-28 22:14:39.962572 pueda-0.1.7/src/pueda/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      150 2023-03-15 01:01:16.000000 pueda-0.1.7/src/pueda/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3092 2023-03-15 01:37:00.000000 pueda-0.1.7/src/pueda/common.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     7433 2023-03-26 15:13:03.000000 pueda-0.1.7/src/pueda/edalize.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      866 2023-07-28 22:12:33.000000 pueda-0.1.7/src/pueda/gtkw.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2924 2023-03-15 02:15:01.000000 pueda-0.1.7/src/pueda/icarus.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     4961 2023-07-28 21:43:22.000000 pueda-0.1.7/src/pueda/myhdl.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2206 2023-07-28 21:30:20.000000 pueda-0.1.7/src/pueda/pyverilator.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2616 2023-07-28 21:38:50.000000 pueda-0.1.7/src/pueda/vcd.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      325 2023-01-22 17:37:49.000000 pueda-0.1.7/src/pueda/veriloggen.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1376 2023-02-28 20:52:57.000000 pueda-0.1.7/src/pueda/yosys.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-07-28 22:14:39.973205 pueda-0.1.7/src/pueda.egg-info/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2267 2023-07-28 22:14:39.000000 pueda-0.1.7/src/pueda.egg-info/PKG-INFO
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      558 2023-07-28 22:14:39.000000 pueda-0.1.7/src/pueda.egg-info/SOURCES.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        1 2023-07-28 22:14:39.000000 pueda-0.1.7/src/pueda.egg-info/dependency_links.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)       69 2023-07-28 22:14:39.000000 pueda-0.1.7/src/pueda.egg-info/requires.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        6 2023-07-28 22:14:39.000000 pueda-0.1.7/src/pueda.egg-info/top_level.txt
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-07-28 22:14:39.981450 pueda-0.1.7/test/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1374 2023-07-28 21:31:34.000000 pueda-0.1.7/test/test.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1162 2023-02-27 20:41:20.000000 pueda-0.1.7/test/test_myhdl_counter.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      463 2023-02-27 20:41:20.000000 pueda-0.1.7/test/test_verilated_dpi_counter.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      454 2023-02-27 20:41:20.000000 pueda-0.1.7/test/test_verilator_counter.py
```

### Comparing `pueda-0.1.6/LICENSE` & `pueda-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pueda-0.1.6/PKG-INFO` & `pueda-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pueda
-Version: 0.1.6
+Version: 0.1.7
 Summary: Collection of python for micro-Electronic Design Automation
 Home-page: https://github.com/bat52/pueda
 Author: Marco Merlin
 Author-email: marcomerli@gmail.com
 License: Apache 2.0
 Keywords: python EDA CAD
 Platform: UNKNOWN
```

### Comparing `pueda-0.1.6/README.md` & `pueda-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pueda-0.1.6/setup.py` & `pueda-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     for d, folders, files in os.walk(datadir)]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='pueda',
-    version='0.1.6',
+    version='0.1.7',
     license='Apache 2.0',
     author="Marco Merlin",
     author_email='marcomerli@gmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     description="Collection of python for micro-Electronic Design Automation",
     long_description=long_description,
```

### Comparing `pueda-0.1.6/src/pueda/common.py` & `pueda-0.1.7/src/pueda/common.py`

 * *Files identical despite different names*

### Comparing `pueda-0.1.6/src/pueda/edalize.py` & `pueda-0.1.7/src/pueda/edalize.py`

 * *Files identical despite different names*

### Comparing `pueda-0.1.6/src/pueda/gtkw.py` & `pueda-0.1.7/src/pueda/gtkw.py`

 * *Files identical despite different names*

### Comparing `pueda-0.1.6/src/pueda/icarus.py` & `pueda-0.1.7/src/pueda/icarus.py`

 * *Files identical despite different names*

### Comparing `pueda-0.1.6/src/pueda/myhdl.py` & `pueda-0.1.7/src/pueda/myhdl.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,10 +151,10 @@
 
     def sim_cfg(self,tb):
         self.sim = Simulation( tb )
 
     def sim_run(self,duration=0):
         self.sim.run(duration)
 
-    def sim_view(self, vcd = 'dump.vcd', gtkw = ''):
+    def sim_view(self, vcd = 'dump.vcd', gtkw = '', mode='gtkwave'):
         if self.dump_en:
-            vcd_view(os.path.join(self.work, fname = vcd, savefname = gtkw), block_en = False)
+            vcd_view(os.path.join(self.work, fname = vcd, savefname = gtkw), block_en = False, mode=mode)
```

### Comparing `pueda-0.1.6/src/pueda/pyverilator.py` & `pueda-0.1.7/src/pueda/pyverilator.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,23 +40,24 @@
             else:
                 dump_ext = '.vcd'
             self.dump_filename = dump_filename + dump_ext
             # start gtkwave to view the waveforms as they are made
             self.sim.start_vcd_trace(self.dump_filename)
             # self.view_waves()
 
-    def view_waves(self,savefname='',options='', postcmd='', block_en = True):
+    def view_waves(self,savefname='',options='', postcmd='', block_en = True, mode='gtkwave'):
         ''' view vcd waves with gtkwave '''
 
         # if False:
         #    # start gtkwave to view the waveforms as they are made
         #    self.sim.start_gtkwave()
         #
         #    # add all the io and internal signals to gtkwave
         #    # self.sim.send_to_gtkwave(self.sim.io)
         #    # self.sim.send_to_gtkwave(self.sim.internals)
         # else:
         vcd_view(self.dump_filename,
                     savefname=savefname,
                     options=options,
                     postcmd=postcmd,
-                    block_en=block_en)
+                    block_en=block_en,
+                    mode=mode)
```

### Comparing `pueda-0.1.6/src/pueda/vcd.py` & `pueda-0.1.7/src/pueda/vcd.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,77 @@
 #!/usr/bin/env python3
 
 import os
 import numpy as np
+import shutil
 from ast import literal_eval
 
 # https://pypi.org/project/vcdvcd/
 from vcdvcd import VCDVCD
 
-def vcd_view(fname,savefname='',options='', postcmd='', block_en = True):
+def vcd_view(fname, mode='gtkwave', savefname='',options='', postcmd='', block_en = True):
+    if mode == 'gtkwave':
+        vcd_view_gtkwave(fname,savefname=savefname, options=options, postcmd=postcmd, block_en = block_en)
+    elif mode == 'vcdterm':
+        vcd_view_terminal(fname, block_en=block_en)
+    else:
+        assert False, f'Unsupported view mode {mode} !!!'
+
+def vcd_view_gtkwave(fname,savefname='',options='', postcmd='', block_en = True):
 
     # by default look for gtkw file named as vcd
     basefname = os.path.splitext(fname)[0]
     basegtkw = basefname + '.gtkw'
-        
+    
     if os.path.isfile(basegtkw):
         savefname = basegtkw
 
     if os.path.isfile(savefname):
         cmdstr = 'gtkwave %s -a %s %s %s' % (options, savefname,fname,postcmd)
     else:
         cmdstr = 'gtkwave %s %s %s' % (options,fname, postcmd)
 
     if not(block_en):
         cmdstr += ' &'
 
     # print(cmdstr)
     os.system(cmdstr)
-    pass
+
+def vcd_view_terminal(fname, block_en=True):
+    """ view vcd in terminal """
+    # check if vcd is installed
+    path = shutil.which("vcd")
+    assert not path is None, "vcd executable is not installed!!! \n\
+        install with the following: \n\
+        git clone https://github.com/yne/vcd.git \n\
+        cd vcd \n\
+        make \n\
+        sudo make install"
+
+    cmdstr = f'vcd < {fname}'
+    if block_en:
+        cmdstr += ' | less -S'
+
+    print(cmdstr)
+    os.system(cmdstr)
 
 def vcd_tv2list(tv,fmt='dec'):
+    """ converts .vcd file time-value lists, into a dictionary of time-value lists """
     time = []
     value = []
     for e in tv:
 
         if   fmt == 'dec':
             vstr = e[1]
         elif fmt == 'bin':
             vstr = '0b' + str.strip(e[1])
-        elif fmt == 'hex':    
+        elif fmt == 'hex':
             vstr = '0h' + str.strip(e[1])
         else:
-            print('unsupported format "%s" !!!' % fmt)
-            assert(False)
+            assert False, f'unsupported format {fmt} !!!'
 
         value.append(literal_eval(vstr))
         time.append(e[0])
     return {'value':value,'time':time}
 
 def vcd_resample(s, fs=1):
 
@@ -54,14 +80,14 @@
     tmax = max(s['time'])
     t = np.arange(tmin,tmax,fs)
     sout = np.interp(t, s['time'], s['value'])
     # sout = f(t)
 
     return {'value':sout, 'time': t}    
 
-def vcd_get_signal(vcdh,sname,fmt = 'dec', resample_en = False, fs=1e9):
+def vcd_get_signal(vcdh, sname,fmt = 'dec', resample_en = False, fs=1e9):
     signal = vcdh[sname]
     # tv is a list of Time/Value delta pairs for this signal.
     s = vcd_tv2list(signal.tv,fmt = fmt)
     if resample_en:
         s = vcd_resample(s)
-    return s 
+    return s
```

### Comparing `pueda-0.1.6/src/pueda/yosys.py` & `pueda-0.1.7/src/pueda/yosys.py`

 * *Files identical despite different names*

### Comparing `pueda-0.1.6/src/pueda.egg-info/PKG-INFO` & `pueda-0.1.7/src/pueda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pueda
-Version: 0.1.6
+Version: 0.1.7
 Summary: Collection of python for micro-Electronic Design Automation
 Home-page: https://github.com/bat52/pueda
 Author: Marco Merlin
 Author-email: marcomerli@gmail.com
 License: Apache 2.0
 Keywords: python EDA CAD
 Platform: UNKNOWN
```

### Comparing `pueda-0.1.6/src/pueda.egg-info/SOURCES.txt` & `pueda-0.1.7/src/pueda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pueda-0.1.6/test/test.py` & `pueda-0.1.7/test/test.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 import unittest
 
 class TestStringMethods(unittest.TestCase):
 
     def test_edalize_icarus_hello(self):
         from pueda.edalize import icarus        
         icarus(simname='hello', top='hello_tb', src_dirs = ['./hello'])
-   
+
     def test_edalize_icarus_counter(self):
        from pueda.edalize import icarus
        icarus(simname='counter', top='counter_tb', src_dirs = ['./counter/rtl','./counter/tb'], iverilog_options=['-g2005-sv'])
        # self.assertEqual('foo'.upper(), 'FOO')
 
     def test_pyverilator_counter(self):
         from pueda.pyverilator import pyverilator_wrapper
         pv = pyverilator_wrapper(fname='./counter/rtl/counter.v', src_dirs=['./counter/rtl'], command_args = [], dump_en = True, dump_level=1)
 
         for _ in range(16):
             pv.sim.clock.tick()
             print('count = %d' % pv.sim.io.count)
         assert pv.sim.io.count == 0
-        # pv.view_waves() this may hold the test, so skip it
+        pv.view_waves(mode='vcdterm', block_en=False)
 
     def test_verilator_counter(self):
         from test_verilator_counter import test_verilator_counter
         test_verilator_counter()
 
     def test_yosys_counter(self):
         from pueda.yosys import yosys
```

### Comparing `pueda-0.1.6/test/test_myhdl_counter.py` & `pueda-0.1.7/test/test_myhdl_counter.py`

 * *Files identical despite different names*

