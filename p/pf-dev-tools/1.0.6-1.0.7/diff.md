# Comparing `tmp/pf_dev_tools-1.0.6.tar.gz` & `tmp/pf_dev_tools-1.0.7.tar.gz`

## Comparing `pf_dev_tools-1.0.6.tar` & `pf_dev_tools-1.0.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/.flake8
--rw-r--r--   0        0        0    27037 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/.nova/Artwork
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/.nova/Configuration.json
--rw-r--r--   0        0        0     4260 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/CoreConfig.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/Exceptions.py
--rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/Git.py
--rw-r--r--   0        0        0     8585 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/OpenFPGACore.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/Paths.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/SCons.py
--rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/Utils.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/__about__.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/__init__.py
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/pfCommand/Clean.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/pfCommand/Clone.py
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/pfCommand/Convert.py
--rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/pfCommand/Delete.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/pfCommand/DryRun.py
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/pfCommand/Eject.py
--rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/pfCommand/Install.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/pfCommand/Make.py
--rw-r--r--   0        0        0     9925 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/pfCommand/Package.py
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/pfCommand/Qfs.py
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/pfCommand/Reverse.py
--rwxr-xr-x   0        0        0     1080 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/pfCommand/__main__.py
--rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pfDevTools/pfCommand/pfCommand.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/LICENSE
--rw-r--r--   0        0        0    10672 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/README.md
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/pyproject.toml
--rw-r--r--   0        0        0    11732 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.7/.flake8
+-rw-r--r--   0        0        0    27037 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.7/.nova/Artwork
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.7/.nova/Configuration.json
+-rw-r--r--   0        0        0     4260 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.7/pfDevTools/CoreConfig.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.7/pfDevTools/Exceptions.py
+-rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.7/pfDevTools/Git.py
+-rw-r--r--   0        0        0     9317 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.7/pfDevTools/OpenFPGACore.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.7/pfDevTools/Paths.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.7/pfDevTools/SCons.py
+-rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.7/pfDevTools/Utils.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.7/pfDevTools/__about__.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.7/pfDevTools/__init__.py
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.7/pfDevTools/pfCommand/Clean.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.7/pfDevTools/pfCommand/Clone.py
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.7/pfDevTools/pfCommand/Convert.py
+-rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.7/pfDevTools/pfCommand/Delete.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.7/pfDevTools/pfCommand/DryRun.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.7/pfDevTools/pfCommand/Eject.py
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.7/pfDevTools/pfCommand/Install.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.7/pfDevTools/pfCommand/Make.py
+-rw-r--r--   0        0        0     9925 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.7/pfDevTools/pfCommand/Package.py
+-rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.7/pfDevTools/pfCommand/Qfs.py
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.7/pfDevTools/pfCommand/Reverse.py
+-rwxr-xr-x   0        0        0     1080 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.7/pfDevTools/pfCommand/__main__.py
+-rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.7/pfDevTools/pfCommand/pfCommand.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.7/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.7/LICENSE
+-rw-r--r--   0        0        0    10621 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.7/README.md
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0    11681 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.7/PKG-INFO
```

### Comparing `pf_dev_tools-1.0.6/.nova/Artwork` & `pf_dev_tools-1.0.7/.nova/Artwork`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.6/pfDevTools/CoreConfig.py` & `pf_dev_tools-1.0.7/pfDevTools/CoreConfig.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.6/pfDevTools/Git.py` & `pf_dev_tools-1.0.7/pfDevTools/Git.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.6/pfDevTools/OpenFPGACore.py` & `pf_dev_tools-1.0.7/pfDevTools/OpenFPGACore.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,18 @@
         print(f'Copying core template repo from \'{src_folder}\'.')
 
         if os.path.exists(dest_folder):
             pfDevTools.Utils.deleteFolder(dest_folder, force_delete=True)
 
         copy_tree(src_folder, dest_folder)
 
+        git_folder = os.path.join(dest_folder, '.git')
+        if os.path.exists(git_folder):
+            pfDevTools.Utils.deleteFolder(git_folder, force_delete=True)
+
     @classmethod
     def _runDockerCommand(cls, image: str, command: str, build_folder: str = None, quiet: bool = True):
         try:
             pfDevTools.Utils.requireCommand('docker')
 
             if not OpenFPGACore._dockerIsRunning():
                 raise RuntimeError('Docker engine does not seem to be running.')
@@ -111,39 +115,53 @@
             if num_cpus_found != 0:
                 number_of_cpus = num_cpus_found
 
         return number_of_cpus
 
     @classmethod
     def _updateQsfFile(cls, target, source, env):
+        core_qsf_file = str(target)
+        if not os.path.exists(core_qsf_file):
+            if env.get('PF_CORE_TEMPLATE_REPO_FOLDER', None) is None:
+                OpenFPGACore._cloneRepo(core_qsf_file, core_qsf_file, env)
+            else:
+                OpenFPGACore._copyRepo(core_qsf_file, core_qsf_file, env)
+
         core_fpga_folder = env['PF_CORE_FPGA_FOLDER']
-        core_verilog_files = [str(Path(str(f)).relative_to(core_fpga_folder)) for f in source]
+
+        core_verilog_files = []
+        for f in source:
+            file_path = str(f)
+            if file_path.endswith('.v') or file_path.endswith('.sv'):
+                core_verilog_files.append(str(Path(str(f)).relative_to(core_fpga_folder)))
+
         number_of_cpus: int = OpenFPGACore._getNumberOfDockerCPUs(env['PF_DOCKER_IMAGE'])
-        pfDevTools.Qfs([str(source[0]), str(target[0]), f'cpus={number_of_cpus}'] + core_verilog_files[1:]).run()
+        pfDevTools.Qfs([core_qsf_file, f'cpus={number_of_cpus}'] + core_verilog_files).run()
 
     @classmethod
     def _installCore(cls, target, source, env):
         pfDevTools.Install([str(source[0])]).run()
         pfDevTools.Eject([]).run()
 
     @classmethod
     def _copyFile(cls, target, source, env):
         source_file = str(source[0])
         target_file = str(target[0])
+        print(f'Copying {source_file} to {target_file}.')
         parent_dest_dir = Path(target_file).parent
         os.makedirs(parent_dest_dir, exist_ok=True)
         shutil.copyfile(source_file, target_file)
 
     @classmethod
     def _searchSourceFiles(cls, env, path: str, dest_verilog_folder: str) -> List[str]:
         dest_verilog_files: List[str] = []
 
         for root, dirs, files in os.walk(path, topdown=False):
             for file in files:
-                if file.endswith('.sv') or file.endswith('.v'):
+                if file.endswith('.sv') or file.endswith('.v') or file.endswith('.svh') or file.endswith('.vh'):
                     src_path = os.path.join(root, file)
                     dest_path = os.path.join(dest_verilog_folder, Path(src_path).relative_to(path))
                     dest_verilog_files.append(dest_path)
 
                     env.Command(dest_path, src_path, OpenFPGACore._copyFile)
 
         return dest_verilog_files
@@ -159,14 +177,18 @@
             env.Command(dest_path, file, OpenFPGACore._copyFile)
 
         return extra_dest_files
 
     @classmethod
     def _compileBitStream(cls, target, source, env):
         print('Compiling core bitstream...')
+
+        core_qsf_file = env['PF_CORE_QSF_FILE']
+        OpenFPGACore._updateQsfFile(core_qsf_file, source, env)
+
         OpenFPGACore._runDockerCommand(env['PF_DOCKER_IMAGE'],
                                        'quartus_sh --flow compile pf_core',
                                        build_folder=os.path.realpath(env['PF_CORE_FPGA_FOLDER']),
                                        quiet=False)
 
     @classmethod
     def _packageCore(cls, target, source, env):
@@ -190,32 +212,31 @@
 
     core_template_folder: str = os.path.join(build_folder, '_core_template_repo')
     env.Replace(PF_CORE_TEMPLATE_FOLDER=core_template_folder)
 
     core_fpga_folder: str = os.path.join(core_template_folder, 'src', 'fpga')
     env.Replace(PF_CORE_FPGA_FOLDER=core_fpga_folder)
 
-    core_input_qsf_file = os.path.join(core_fpga_folder, 'ap_core.qsf')
-    core_output_qsf_file = os.path.join(core_fpga_folder, 'pf_core.qsf')
+    core_qsf_file = os.path.join(core_fpga_folder, 'pf_core.qsf')
+    env.Replace(PF_CORE_QSF_FILE=core_qsf_file)
 
     core_output_bitstream_file = os.path.join(core_fpga_folder, 'output_files', 'pf_core.rbf')
     env.Replace(PF_CORE_BITSTREAM_FILE=core_output_bitstream_file)
 
-    dest_verilog_folder: str = os.path.join(core_fpga_folder, 'core')
-
     if env.get('PF_CORE_TEMPLATE_REPO_FOLDER', None) is None:
-        env.Command(core_input_qsf_file, '', OpenFPGACore._cloneRepo)
+        env.Command(core_template_folder, '', OpenFPGACore._cloneRepo)
     else:
-        env.Command(core_input_qsf_file, '', OpenFPGACore._copyRepo)
+        env.Command(core_template_folder, '', OpenFPGACore._copyRepo)
 
+    dest_verilog_folder: str = os.path.join(core_fpga_folder, 'core')
     dest_verilog_files: List[str] = OpenFPGACore._searchSourceFiles(env, src_folder, dest_verilog_folder)
     extra_dest_files: List[str] = OpenFPGACore._addExtraFiles(env, src_folder, dest_verilog_folder, extra_files)
 
-    env.Command(core_output_qsf_file, [core_input_qsf_file] + dest_verilog_files, OpenFPGACore._updateQsfFile)
-    env.Command(core_output_bitstream_file, [core_output_qsf_file] + dest_verilog_files + extra_dest_files, OpenFPGACore._compileBitStream)
+    bitstream_target = env.Command(core_output_bitstream_file, dest_verilog_files + extra_dest_files, OpenFPGACore._compileBitStream)
+    env.Precious(bitstream_target)
 
     build_process: pfDevTools.Package = pfDevTools.Package([config_file, core_output_bitstream_file, build_folder])
     packaged_core = os.path.join(build_folder, build_process.packagedFilename())
     p = env.Command(packaged_core, build_process.dependencies(), OpenFPGACore._packageCore)
 
     env.Default(packaged_core)
     env.Clean(packaged_core, build_folder)
```

### Comparing `pf_dev_tools-1.0.6/pfDevTools/Utils.py` & `pf_dev_tools-1.0.7/pfDevTools/Utils.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.6/pfDevTools/__init__.py` & `pf_dev_tools-1.0.7/pfDevTools/__init__.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.6/pfDevTools/pfCommand/Clean.py` & `pf_dev_tools-1.0.7/pfDevTools/pfCommand/Clean.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.6/pfDevTools/pfCommand/Clone.py` & `pf_dev_tools-1.0.7/pfDevTools/pfCommand/Clone.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.6/pfDevTools/pfCommand/Convert.py` & `pf_dev_tools-1.0.7/pfDevTools/pfCommand/Convert.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.6/pfDevTools/pfCommand/Delete.py` & `pf_dev_tools-1.0.7/pfDevTools/pfCommand/Delete.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.6/pfDevTools/pfCommand/DryRun.py` & `pf_dev_tools-1.0.7/pfDevTools/pfCommand/DryRun.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.6/pfDevTools/pfCommand/Eject.py` & `pf_dev_tools-1.0.7/pfDevTools/pfCommand/Eject.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.6/pfDevTools/pfCommand/Install.py` & `pf_dev_tools-1.0.7/pfDevTools/pfCommand/Install.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         self._zip_filename = None
         self._volume_path = None
 
         nb_of_arguments = len(arguments)
         if nb_of_arguments != 0:
             if nb_of_arguments == 2:
                 self._volume_path = arguments[1]
-                arguments = arguments[:0]
+                arguments = [arguments[0]]
                 nb_of_arguments -= 1
             else:
                 self._volume_path = pfDevTools.CoreConfig.coreInstallVolumePath()
 
             if nb_of_arguments != 1:
                 raise RuntimeError('Invalid arguments. Maybe start with `pf --help?')
```

### Comparing `pf_dev_tools-1.0.6/pfDevTools/pfCommand/Make.py` & `pf_dev_tools-1.0.7/pfDevTools/pfCommand/Make.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.6/pfDevTools/pfCommand/Package.py` & `pf_dev_tools-1.0.7/pfDevTools/pfCommand/Package.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.6/pfDevTools/pfCommand/Qfs.py` & `pf_dev_tools-1.0.7/pfDevTools/pfCommand/Qfs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # SPDX-FileCopyrightText: 2023-present Didier Malenfant
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import os
+import tempfile
+import shutil
+import filecmp
 
 from typing import List
 from enum import Enum
 
 from pfDevTools.Exceptions import ArgumentError
 
 
@@ -22,26 +25,22 @@
 
     def __init__(self, arguments):
         """Constructor based on command line arguments."""
 
         if len(arguments) < 3:
             raise RuntimeError('Invalid arguments. Maybe start with `pf --help?')
 
-        self._input_qsf_file: str = arguments[0]
-        if not self._input_qsf_file.endswith('.qsf'):
+        self._qsf_filename: str = arguments[0]
+        if not self._qsf_filename.endswith('.qsf'):
             raise ArgumentError('Invalid input project file type for pf qsf.')
 
-        if not os.path.exists(self._input_qsf_file):
-            raise RuntimeError('File \'' + self._input_qsf_file + '\' does not exist.')
+        if not os.path.exists(self._qsf_filename):
+            raise RuntimeError('File \'' + self._qsf_filename + '\' does not exist.')
 
-        self._output_qsf_file: str = arguments[1]
-        if not self._output_qsf_file.endswith('.qsf'):
-            raise ArgumentError('Invalid output project file type for pf qsf.')
-
-        arguments = arguments[2:]
+        arguments = arguments[1:]
 
         self._number_of_cpus: int = 0
         if arguments[0].startswith('cpus='):
             value = arguments[0][5:]
             if value == 'max':
                 self._number_of_cpus = os.cpu_count()
             else:
@@ -69,55 +68,61 @@
                 raise ArgumentError('Unknown file type for \'' + file + '\'.')
 
             dest_file.write(file.replace('\\', '/') + '\n')
 
         dest_file.write('\n' + editing_wrappers[1])
 
     def run(self) -> None:
-        print('Updating QSF file...')
-
         editing_wrappers: List[str] = ['# Additions made by pf command\n',
                                        '# End of additions made by pf command\n']
 
-        src_file = open(self._input_qsf_file, 'r')
-        dest_file = open(self._output_qsf_file, 'w')
-
-        editing_state = EditingState.BEFORE_EDIT
-        last_line = None
+        src_file = open(self._qsf_filename, 'r')
 
-        for line in src_file.readlines():
-            last_line = line
+        # -- In a temporary folder.
+        with tempfile.TemporaryDirectory() as tmp_dir:
+            tmp_file: str = os.path.join(tmp_dir, 'temp.qsf')
+            dest_file = open(tmp_file, 'w')
+
+            editing_state = EditingState.BEFORE_EDIT
+            last_line = None
+
+            for line in src_file.readlines():
+                last_line = line
+
+                match editing_state:
+                    case EditingState.BEFORE_EDIT:
+                        if line == editing_wrappers[0]:
+                            self._writeAdditions(dest_file, editing_wrappers)
+
+                            editing_state = EditingState.DURING_EDIT
+                        else:
+                            dest_file.write(line)
+                    case EditingState.DURING_EDIT:
+                        if line == editing_wrappers[1]:
+                            editing_state = EditingState.AFTER_EDIT
+                    case EditingState.AFTER_EDIT:
+                        dest_file.write(line)
 
-            match editing_state:
-                case EditingState.BEFORE_EDIT:
-                    if line == editing_wrappers[0]:
-                        self._writeAdditions(dest_file, editing_wrappers)
+            if editing_state == EditingState.BEFORE_EDIT:
+                if not last_line.endswith('\n'):
+                    dest_file.write('\n')
 
-                        editing_state = EditingState.DURING_EDIT
-                    else:
-                        dest_file.write(line)
-                case EditingState.DURING_EDIT:
-                    if line == editing_wrappers[1]:
-                        editing_state = EditingState.AFTER_EDIT
-                case EditingState.AFTER_EDIT:
-                    dest_file.write(line)
-
-        if editing_state == EditingState.BEFORE_EDIT:
-            if not last_line.endswith('\n'):
-                dest_file.write('\n')
+                if last_line != '\n':
+                    dest_file.write('\n')
 
-            if last_line != '\n':
-                dest_file.write('\n')
+                self._writeAdditions(dest_file, editing_wrappers)
 
-            self._writeAdditions(dest_file, editing_wrappers)
+            src_file.close()
+            dest_file.close()
 
-        src_file.close()
-        dest_file.close()
+            if filecmp.cmp(tmp_file, self._qsf_filename) is False:
+                print('Updating QSF file...')
+                shutil.copyfile(tmp_file, self._qsf_filename)
 
     @classmethod
     def name(cls) -> str:
         return 'qfs'
 
     @classmethod
     def usage(cls) -> None:
-        print('   qfs qsf_in qsf_out <cpus=num> files   - Add files and set number of cpu for the project.')
+        print('   qfs qsf_file <cpus=num> files         - Add files and set number of cpu for the project.')
         print('                                           (if num is \'max\' then all CPU cores will be used).')
```

### Comparing `pf_dev_tools-1.0.6/pfDevTools/pfCommand/Reverse.py` & `pf_dev_tools-1.0.7/pfDevTools/pfCommand/Reverse.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.6/pfDevTools/pfCommand/__main__.py` & `pf_dev_tools-1.0.7/pfDevTools/pfCommand/__main__.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.6/pfDevTools/pfCommand/pfCommand.py` & `pf_dev_tools-1.0.7/pfDevTools/pfCommand/pfCommand.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.6/LICENSE` & `pf_dev_tools-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.6/README.md` & `pf_dev_tools-1.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -98,17 +98,17 @@
 ```console
  pf package config_file bistream_file dest_folder
 ```
 Packages a core into a zip file according to the content of `config_file`. The format for the configuration can be found [below](#core-config-file-format). `bistream_file` is the path to a reversed bitstream file for the core. Resulting package is written in `dest_folder`.
 
 #### qfs command
 ```console
-  pf qfs qsf_in qsf_out <cpus=num> files...
+  pf qfs qsf_file <cpus=num> files...
 ```
-Edits a **Quartus** `qfs` project file to add files and set number of cpu for the project. Reads the `qfs` file at `qsf_in` and writes the result to `qsf_out`. `files` is a list of **Verilog** `.v` or `.sv` files, separated by spaces.
+Edits a **Quartus** `qfs` project file to add files and set number of cpu for the project. Updates the `qfs_file` by adding a list of **Verilog** `.v` or `.sv` `files`, separated by spaces.
 
 Optionally `cpus` can set the number of cpu cores that the compilation process can use. If `num` is `max` then all available **CPU** cores will be used.
 
 #### reverse command
 ```console
   pf reverse src_filename dest_filename
 ```
```

### Comparing `pf_dev_tools-1.0.6/pyproject.toml` & `pf_dev_tools-1.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.6/PKG-INFO` & `pf_dev_tools-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pf-dev-tools
-Version: 1.0.6
+Version: 1.0.7
 Summary: A collection of tools for Project Freedom projects
 Project-URL: Homepage, https://didier.malenfant.net/ProjectFreedom/
 Project-URL: Documentation, https://github.com/DidierMalenfant/pfDevTools#readme
 Project-URL: Bug Tracker, https://github.com/DidierMalenfant/pfDevTools/issues
 Project-URL: Source Code, https://github.com/DidierMalenfant/pfDevTools
 Author-email: Didier Malenfant <coding@malenfant.net>
 License-Expression: GPL-3.0-or-later
@@ -122,17 +122,17 @@
 ```console
  pf package config_file bistream_file dest_folder
 ```
 Packages a core into a zip file according to the content of `config_file`. The format for the configuration can be found [below](#core-config-file-format). `bistream_file` is the path to a reversed bitstream file for the core. Resulting package is written in `dest_folder`.
 
 #### qfs command
 ```console
-  pf qfs qsf_in qsf_out <cpus=num> files...
+  pf qfs qsf_file <cpus=num> files...
 ```
-Edits a **Quartus** `qfs` project file to add files and set number of cpu for the project. Reads the `qfs` file at `qsf_in` and writes the result to `qsf_out`. `files` is a list of **Verilog** `.v` or `.sv` files, separated by spaces.
+Edits a **Quartus** `qfs` project file to add files and set number of cpu for the project. Updates the `qfs_file` by adding a list of **Verilog** `.v` or `.sv` `files`, separated by spaces.
 
 Optionally `cpus` can set the number of cpu cores that the compilation process can use. If `num` is `max` then all available **CPU** cores will be used.
 
 #### reverse command
 ```console
   pf reverse src_filename dest_filename
 ```
```

