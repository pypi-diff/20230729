# Comparing `tmp/agentshell-0.0.4.tar.gz` & `tmp/agentshell-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentshell-0.0.4.tar", last modified: Fri Jul 28 02:19:15 2023, max compression
+gzip compressed data, was "agentshell-0.0.6.tar", last modified: Sat Jul 29 00:35:08 2023, max compression
```

## Comparing `agentshell-0.0.4.tar` & `agentshell-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:19:15.981243 agentshell-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-28 02:19:04.000000 agentshell-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-28 02:19:15.981243 agentshell-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-28 02:19:04.000000 agentshell-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:19:15.981243 agentshell-0.0.4/agentshell/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-28 02:19:04.000000 agentshell-0.0.4/agentshell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-28 02:19:04.000000 agentshell-0.0.4/agentshell/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     8497 2023-07-28 02:19:04.000000 agentshell-0.0.4/agentshell/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:19:15.981243 agentshell-0.0.4/agentshell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-28 02:19:15.000000 agentshell-0.0.4/agentshell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-28 02:19:15.000000 agentshell-0.0.4/agentshell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 02:19:15.000000 agentshell-0.0.4/agentshell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 02:19:15.000000 agentshell-0.0.4/agentshell.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 02:19:15.000000 agentshell-0.0.4/agentshell.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 02:19:15.981243 agentshell-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-28 02:19:04.000000 agentshell-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:35:08.257503 agentshell-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-29 00:34:55.000000 agentshell-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-07-29 00:35:08.257503 agentshell-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-07-29 00:34:55.000000 agentshell-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:35:08.253503 agentshell-0.0.6/agentshell/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-29 00:34:55.000000 agentshell-0.0.6/agentshell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-07-29 00:34:55.000000 agentshell-0.0.6/agentshell/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-07-29 00:34:55.000000 agentshell-0.0.6/agentshell/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:35:08.257503 agentshell-0.0.6/agentshell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-07-29 00:35:08.000000 agentshell-0.0.6/agentshell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-29 00:35:08.000000 agentshell-0.0.6/agentshell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 00:35:08.000000 agentshell-0.0.6/agentshell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-29 00:35:08.000000 agentshell-0.0.6/agentshell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-29 00:35:08.000000 agentshell-0.0.6/agentshell.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 00:35:08.257503 agentshell-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-29 00:34:55.000000 agentshell-0.0.6/setup.py
```

### Comparing `agentshell-0.0.4/LICENSE` & `agentshell-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `agentshell-0.0.4/PKG-INFO` & `agentshell-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentshell
-Version: 0.0.4
+Version: 0.0.6
 Summary: A shell for your agent.
 Home-page: https://github.com/AutonomousResearchGroup/agentshell
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
@@ -12,19 +12,21 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# agentshell
 
 A shell for your agent. Track state and history, multiple shells, and more.
 
 
+[![Lint and Test](https://github.com/AutonomousResearchGroup/agentshell/actions/workflows/test.yml/badge.svg)](https://github.com/AutonomousResearchGroup/agentshell/actions/workflows/test.yml)
+[![PyPI version](https://badge.fury.io/py/agentshell.svg)](https://badge.fury.io/py/agentshell)
+
 # Installation
 
 ```bash
 pip install agentshell
 ```
 
 # Documentation
```

### Comparing `agentshell-0.0.4/README.md` & `agentshell-0.0.6/agentshell.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,31 @@
-# agentshell
+Metadata-Version: 2.1
+Name: agentshell
+Version: 0.0.6
+Summary: A shell for your agent.
+Home-page: https://github.com/AutonomousResearchGroup/agentshell
+Author: Moon
+Author-email: shawmakesmagic@gmail.com
+License: MIT
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 
 A shell for your agent. Track state and history, multiple shells, and more.
 
-<img src="resources/image.jpg">
+
+[![Lint and Test](https://github.com/AutonomousResearchGroup/agentshell/actions/workflows/test.yml/badge.svg)](https://github.com/AutonomousResearchGroup/agentshell/actions/workflows/test.yml)
+[![PyPI version](https://badge.fury.io/py/agentshell.svg)](https://badge.fury.io/py/agentshell)
 
 # Installation
 
 ```bash
 pip install agentshell
 ```
```

### Comparing `agentshell-0.0.4/agentshell/__init__.py` & `agentshell-0.0.6/agentshell/__init__.py`

 * *Files identical despite different names*

### Comparing `agentshell-0.0.4/agentshell/action.py` & `agentshell-0.0.6/agentshell/action.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,17 @@
         "" + ("\n".join(get_files_in_cwd())) + "\n"
         "============================================\n"
     )
 
     return compose_prompt(use_shell_prompt, context)
 
 
-def use_shell(arguments):
+def use_shell_handler(arguments):
     command = arguments.get("command")
-    run_command(command)
+    return run_command(command)
 
 
 def get_actions():
     return [
         {
             "function": compose_function(
                 name="use_shell",
@@ -53,12 +53,12 @@
                         "description": "Describe the expected output of the command. Write it from the user's perspective, in the first person, e.g. 'I should see the current working directory.'",
                     },
                 },
                 required_properties=["command", "expected_output"],
             ),
             "prompt": use_shell_prompt,
             "builder": compose_use_shell_prompt,
-            "handler": use_shell,
+            "handler": use_shell_handler,
             "suggestion_after_actions": ["use_shell"],  # suggest self
             "never_after_actions": [],
         }
     ]
```

### Comparing `agentshell-0.0.4/agentshell/main.py` & `agentshell-0.0.6/agentshell/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,16 +281,16 @@
             set_cwd(cwd, shell_id)
             result_split = result_split[:-1]
             result_split = "\n".join(result_split)
         else:
             result_split = "\n".join(result_split)
 
         add_to_shell_history(shell_id, command, success="True", output=result)
-        return True
+        return { "success": True, "output": result_split, "error": None }
 
     else:  # If the process did not complete successfully
         output = process.stdout
         error = process.stderr
         add_to_shell_history(
             shell_id, command, success="False", output=output, error=error
         )
-        return False
+        return { "success": False, "output": output, "error": error }
```

### Comparing `agentshell-0.0.4/agentshell.egg-info/PKG-INFO` & `agentshell-0.0.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,268 +1,257 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 6167 656e  : 2.1.Name: agen
-00000020: 7473 6865 6c6c 0a56 6572 7369 6f6e 3a20  tshell.Version: 
-00000030: 302e 302e 340a 5375 6d6d 6172 793a 2041  0.0.4.Summary: A
-00000040: 2073 6865 6c6c 2066 6f72 2079 6f75 7220   shell for your 
-00000050: 6167 656e 742e 0a48 6f6d 652d 7061 6765  agent..Home-page
-00000060: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
-00000070: 2e63 6f6d 2f41 7574 6f6e 6f6d 6f75 7352  .com/AutonomousR
-00000080: 6573 6561 7263 6847 726f 7570 2f61 6765  esearchGroup/age
-00000090: 6e74 7368 656c 6c0a 4175 7468 6f72 3a20  ntshell.Author: 
-000000a0: 4d6f 6f6e 0a41 7574 686f 722d 656d 6169  Moon.Author-emai
-000000b0: 6c3a 2073 6861 776d 616b 6573 6d61 6769  l: shawmakesmagi
-000000c0: 6340 676d 6169 6c2e 636f 6d0a 4c69 6365  c@gmail.com.Lice
-000000d0: 6e73 653a 204d 4954 0a43 6c61 7373 6966  nse: MIT.Classif
-000000e0: 6965 723a 2044 6576 656c 6f70 6d65 6e74  ier: Development
-000000f0: 2053 7461 7475 7320 3a3a 2032 202d 2050   Status :: 2 - P
-00000100: 7265 2d41 6c70 6861 0a43 6c61 7373 6966  re-Alpha.Classif
-00000110: 6965 723a 2049 6e74 656e 6465 6420 4175  ier: Intended Au
-00000120: 6469 656e 6365 203a 3a20 5363 6965 6e63  dience :: Scienc
-00000130: 652f 5265 7365 6172 6368 0a43 6c61 7373  e/Research.Class
-00000140: 6966 6965 723a 204c 6963 656e 7365 203a  ifier: License :
-00000150: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-00000160: 3a20 4d49 5420 4c69 6365 6e73 650a 436c  : MIT License.Cl
-00000170: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-00000180: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000190: 3a20 5079 7468 6f6e 203a 3a20 330a 436c  : Python :: 3.Cl
-000001a0: 6173 7369 6669 6572 3a20 4f70 6572 6174  assifier: Operat
-000001b0: 696e 6720 5379 7374 656d 203a 3a20 504f  ing System :: PO
-000001c0: 5349 5820 3a3a 204c 696e 7578 0a43 6c61  SIX :: Linux.Cla
-000001d0: 7373 6966 6965 723a 204f 7065 7261 7469  ssifier: Operati
-000001e0: 6e67 2053 7973 7465 6d20 3a3a 204d 6163  ng System :: Mac
-000001f0: 4f53 203a 3a20 4d61 634f 5320 580a 436c  OS :: MacOS X.Cl
-00000200: 6173 7369 6669 6572 3a20 4f70 6572 6174  assifier: Operat
-00000210: 696e 6720 5379 7374 656d 203a 3a20 4d69  ing System :: Mi
-00000220: 6372 6f73 6f66 7420 3a3a 2057 696e 646f  crosoft :: Windo
-00000230: 7773 0a44 6573 6372 6970 7469 6f6e 2d43  ws.Description-C
-00000240: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
-00000250: 742f 6d61 726b 646f 776e 0a4c 6963 656e  t/markdown.Licen
-00000260: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
-00000270: 0a0a 2320 6167 656e 7473 6865 6c6c 0a0a  ..# agentshell..
-00000280: 4120 7368 656c 6c20 666f 7220 796f 7572  A shell for your
-00000290: 2061 6765 6e74 2e20 5472 6163 6b20 7374   agent. Track st
-000002a0: 6174 6520 616e 6420 6869 7374 6f72 792c  ate and history,
-000002b0: 206d 756c 7469 706c 6520 7368 656c 6c73   multiple shells
-000002c0: 2c20 616e 6420 6d6f 7265 2e0a 0a0a 2320  , and more....# 
-000002d0: 496e 7374 616c 6c61 7469 6f6e 0a0a 6060  Installation..``
-000002e0: 6062 6173 680a 7069 7020 696e 7374 616c  `bash.pip instal
-000002f0: 6c20 6167 656e 7473 6865 6c6c 0a60 6060  l agentshell.```
-00000300: 0a0a 2320 446f 6375 6d65 6e74 6174 696f  ..# Documentatio
-00000310: 6e0a 0a23 2320 6067 6574 5f66 696c 6573  n..## `get_files
-00000320: 5f69 6e5f 6377 6428 7368 656c 6c5f 6964  _in_cwd(shell_id
-00000330: 3d4e 6f6e 6529 600a 0a52 6574 7572 6e73  =None)`..Returns
-00000340: 2061 206c 6973 7420 6f66 2066 696c 6573   a list of files
-00000350: 2069 6e20 7468 6520 6375 7272 656e 7420   in the current 
-00000360: 6469 7265 6374 6f72 7920 6f66 2061 2073  directory of a s
-00000370: 7065 6369 6669 6320 7368 656c 6c2e 2049  pecific shell. I
-00000380: 6620 6073 6865 6c6c 5f69 6460 2069 7320  f `shell_id` is 
-00000390: 6e6f 7420 7370 6563 6966 6965 642c 2075  not specified, u
-000003a0: 7365 7320 7468 6520 6375 7272 656e 7420  ses the current 
-000003b0: 7368 656c 6c2e 0a0a 2a2a 5061 7261 6d65  shell...**Parame
-000003c0: 7465 7273 3a2a 2a0a 0a2d 2060 7368 656c  ters:**..- `shel
-000003d0: 6c5f 6964 603a 2054 6865 2075 6e69 7175  l_id`: The uniqu
-000003e0: 6520 6964 656e 7469 6669 6572 206f 6620  e identifier of 
-000003f0: 7468 6520 7368 656c 6c2e 0a0a 2a2a 5265  the shell...**Re
-00000400: 7475 726e 733a 2a2a 0a0a 2d20 4120 6c69  turns:**..- A li
-00000410: 7374 206f 6620 6669 6c65 6e61 6d65 7320  st of filenames 
-00000420: 696e 2074 6865 2063 7572 7265 6e74 2064  in the current d
-00000430: 6972 6563 746f 7279 2e0a 0a23 2320 6067  irectory...## `g
-00000440: 6574 5f63 7572 7265 6e74 5f73 6865 6c6c  et_current_shell
-00000450: 2829 600a 0a52 6574 7572 6e73 2074 6865  ()`..Returns the
-00000460: 2075 6e69 7175 6520 6964 656e 7469 6669   unique identifi
-00000470: 6572 206f 6620 7468 6520 6375 7272 656e  er of the curren
-00000480: 7420 7368 656c 6c2e 2049 6620 6e6f 2073  t shell. If no s
-00000490: 6865 6c6c 2069 7320 6375 7272 656e 746c  hell is currentl
-000004a0: 7920 6163 7469 7665 2c20 6372 6561 7465  y active, create
-000004b0: 7320 6120 6e65 7720 7368 656c 6c20 616e  s a new shell an
-000004c0: 6420 7265 7475 726e 7320 6974 7320 6964  d returns its id
-000004d0: 656e 7469 6669 6572 2e0a 0a2a 2a52 6574  entifier...**Ret
-000004e0: 7572 6e73 3a2a 2a0a 0a2d 2054 6865 2075  urns:**..- The u
-000004f0: 6e69 7175 6520 6964 656e 7469 6669 6572  nique identifier
-00000500: 206f 6620 7468 6520 6375 7272 656e 7420   of the current 
-00000510: 7368 656c 6c2e 0a0a 2323 2060 7365 745f  shell...## `set_
-00000520: 6377 6428 6377 642c 2073 6865 6c6c 5f69  cwd(cwd, shell_i
-00000530: 643d 4e6f 6e65 2960 0a0a 5365 7473 2074  d=None)`..Sets t
-00000540: 6865 2063 7572 7265 6e74 2077 6f72 6b69  he current worki
-00000550: 6e67 2064 6972 6563 746f 7279 206f 6620  ng directory of 
-00000560: 6120 7370 6563 6966 6963 2073 6865 6c6c  a specific shell
-00000570: 2e20 4966 2060 7368 656c 6c5f 6964 6020  . If `shell_id` 
-00000580: 6973 206e 6f74 2073 7065 6369 6669 6564  is not specified
-00000590: 2c20 7573 6573 2074 6865 2063 7572 7265  , uses the curre
-000005a0: 6e74 2073 6865 6c6c 2e0a 0a2a 2a50 6172  nt shell...**Par
-000005b0: 616d 6574 6572 733a 2a2a 0a0a 2d20 6063  ameters:**..- `c
-000005c0: 7764 603a 2054 6865 206e 6577 2063 7572  wd`: The new cur
-000005d0: 7265 6e74 2077 6f72 6b69 6e67 2064 6972  rent working dir
-000005e0: 6563 746f 7279 2e0a 2d20 6073 6865 6c6c  ectory..- `shell
-000005f0: 5f69 6460 3a20 5468 6520 756e 6971 7565  _id`: The unique
-00000600: 2069 6465 6e74 6966 6965 7220 6f66 2074   identifier of t
-00000610: 6865 2073 6865 6c6c 2e0a 0a23 2320 6073  he shell...## `s
-00000620: 6574 5f63 7572 7265 6e74 5f73 6865 6c6c  et_current_shell
-00000630: 2873 6865 6c6c 5f69 6429 600a 0a53 6574  (shell_id)`..Set
-00000640: 7320 7468 6520 6375 7272 656e 7420 7368  s the current sh
-00000650: 656c 6c20 746f 2074 6865 2073 6865 6c6c  ell to the shell
-00000660: 2077 6974 6820 7468 6520 7370 6563 6966   with the specif
-00000670: 6965 6420 6964 656e 7469 6669 6572 2e0a  ied identifier..
-00000680: 0a2a 2a50 6172 616d 6574 6572 733a 2a2a  .**Parameters:**
-00000690: 0a0a 2d20 6073 6865 6c6c 5f69 6460 3a20  ..- `shell_id`: 
-000006a0: 5468 6520 756e 6971 7565 2069 6465 6e74  The unique ident
-000006b0: 6966 6965 7220 6f66 2074 6865 2073 6865  ifier of the she
-000006c0: 6c6c 2074 6f20 6265 206d 6164 6520 6375  ll to be made cu
-000006d0: 7272 656e 742e 0a0a 2323 2060 6765 745f  rrent...## `get_
-000006e0: 6869 7374 6f72 7928 7368 656c 6c5f 6964  history(shell_id
-000006f0: 3d4e 6f6e 652c 206e 5f6c 696d 6974 3d32  =None, n_limit=2
-00000700: 3029 600a 0a52 6574 7572 6e73 2074 6865  0)`..Returns the
-00000710: 2063 6f6d 6d61 6e64 2068 6973 746f 7279   command history
-00000720: 206f 6620 6120 7370 6563 6966 6963 2073   of a specific s
-00000730: 6865 6c6c 2e20 4966 2060 7368 656c 6c5f  hell. If `shell_
-00000740: 6964 6020 6973 206e 6f74 2073 7065 6369  id` is not speci
-00000750: 6669 6564 2c20 7573 6573 2074 6865 2063  fied, uses the c
-00000760: 7572 7265 6e74 2073 6865 6c6c 2e0a 0a2a  urrent shell...*
-00000770: 2a50 6172 616d 6574 6572 733a 2a2a 0a0a  *Parameters:**..
-00000780: 2d20 6073 6865 6c6c 5f69 6460 3a20 5468  - `shell_id`: Th
-00000790: 6520 756e 6971 7565 2069 6465 6e74 6966  e unique identif
-000007a0: 6965 7220 6f66 2074 6865 2073 6865 6c6c  ier of the shell
-000007b0: 2e0a 2d20 606e 5f6c 696d 6974 603a 2054  ..- `n_limit`: T
-000007c0: 6865 206d 6178 696d 756d 206e 756d 6265  he maximum numbe
-000007d0: 7220 6f66 2068 6973 746f 7279 2065 6e74  r of history ent
-000007e0: 7269 6573 2074 6f20 7265 7475 726e 2e0a  ries to return..
-000007f0: 0a2a 2a52 6574 7572 6e73 3a2a 2a0a 0a2d  .**Returns:**..-
-00000800: 2041 206c 6973 7420 6f66 2064 6963 7469   A list of dicti
-00000810: 6f6e 6172 6965 732c 2065 6163 6820 7265  onaries, each re
-00000820: 7072 6573 656e 7469 6e67 2061 2063 6f6d  presenting a com
-00000830: 6d61 6e64 2061 6e64 2069 7473 2072 6573  mand and its res
-00000840: 756c 742e 0a0a 2323 2060 6765 745f 6869  ult...## `get_hi
-00000850: 7374 6f72 795f 666f 726d 6174 7465 6428  story_formatted(
-00000860: 7368 656c 6c5f 6964 3d4e 6f6e 6529 600a  shell_id=None)`.
-00000870: 0a52 6574 7572 6e73 2074 6865 2063 6f6d  .Returns the com
-00000880: 6d61 6e64 2068 6973 746f 7279 206f 6620  mand history of 
-00000890: 6120 7370 6563 6966 6963 2073 6865 6c6c  a specific shell
-000008a0: 2069 6e20 6120 6875 6d61 6e2d 7265 6164   in a human-read
-000008b0: 6162 6c65 2066 6f72 6d61 742e 2049 6620  able format. If 
-000008c0: 6073 6865 6c6c 5f69 6460 2069 7320 6e6f  `shell_id` is no
-000008d0: 7420 7370 6563 6966 6965 642c 2075 7365  t specified, use
-000008e0: 7320 7468 6520 6375 7272 656e 7420 7368  s the current sh
-000008f0: 656c 6c2e 0a0a 2a2a 5061 7261 6d65 7465  ell...**Paramete
-00000900: 7273 3a2a 2a0a 0a2d 2060 7368 656c 6c5f  rs:**..- `shell_
-00000910: 6964 603a 2054 6865 2075 6e69 7175 6520  id`: The unique 
-00000920: 6964 656e 7469 6669 6572 206f 6620 7468  identifier of th
-00000930: 6520 7368 656c 6c2e 0a0a 2a2a 5265 7475  e shell...**Retu
-00000940: 726e 733a 2a2a 0a0a 2d20 5468 6520 636f  rns:**..- The co
-00000950: 6d6d 616e 6420 6869 7374 6f72 7920 696e  mmand history in
-00000960: 2068 756d 616e 2d72 6561 6461 626c 6520   human-readable 
-00000970: 666f 726d 6174 2e0a 0a23 2320 6061 6464  format...## `add
-00000980: 5f74 6f5f 7368 656c 6c5f 6869 7374 6f72  _to_shell_histor
-00000990: 7928 7368 656c 6c5f 6964 2c20 636f 6d6d  y(shell_id, comm
-000009a0: 616e 642c 2073 7563 6365 7373 2c20 6f75  and, success, ou
-000009b0: 7470 7574 2c20 6572 726f 723d 4e6f 6e65  tput, error=None
-000009c0: 2960 0a0a 4164 6473 2061 2063 6f6d 6d61  )`..Adds a comma
-000009d0: 6e64 2061 6e64 2069 7473 2072 6573 756c  nd and its resul
-000009e0: 7420 746f 2074 6865 2068 6973 746f 7279  t to the history
-000009f0: 206f 6620 6120 7370 6563 6966 6963 2073   of a specific s
-00000a00: 6865 6c6c 2e0a 0a2a 2a50 6172 616d 6574  hell...**Paramet
-00000a10: 6572 733a 2a2a 0a0a 2d20 6073 6865 6c6c  ers:**..- `shell
-00000a20: 5f69 6460 3a20 5468 6520 756e 6971 7565  _id`: The unique
-00000a30: 2069 6465 6e74 6966 6965 7220 6f66 2074   identifier of t
-00000a40: 6865 2073 6865 6c6c 2e0a 2d20 6063 6f6d  he shell..- `com
-00000a50: 6d61 6e64 603a 2054 6865 2063 6f6d 6d61  mand`: The comma
-00000a60: 6e64 2074 6861 7420 7761 7320 6578 6563  nd that was exec
-00000a70: 7574 6564 2e0a 2d20 6073 7563 6365 7373  uted..- `success
-00000a80: 603a 2057 6865 7468 6572 2074 6865 2063  `: Whether the c
-00000a90: 6f6d 6d61 6e64 2077 6173 2073 7563 6365  ommand was succe
-00000aa0: 7373 6675 6c2e 0a2d 2060 6f75 7470 7574  ssful..- `output
-00000ab0: 603a 2054 6865 206f 7574 7075 7420 6f66  `: The output of
-00000ac0: 2074 6865 2063 6f6d 6d61 6e64 2e0a 2d20   the command..- 
-00000ad0: 6065 7272 6f72 603a 2041 6e79 2065 7272  `error`: Any err
-00000ae0: 6f72 206d 6573 7361 6765 7320 7072 6f64  or messages prod
-00000af0: 7563 6564 2062 7920 7468 6520 636f 6d6d  uced by the comm
-00000b00: 616e 642e 0a0a 2323 2060 636c 6561 725f  and...## `clear_
-00000b10: 6869 7374 6f72 7928 7368 656c 6c5f 6964  history(shell_id
-00000b20: 2960 0a0a 436c 6561 7273 2074 6865 2063  )`..Clears the c
-00000b30: 6f6d 6d61 6e64 2068 6973 746f 7279 206f  ommand history o
-00000b40: 6620 6120 7370 6563 6966 6963 2073 6865  f a specific she
-00000b50: 6c6c 2e0a 0a2a 2a50 6172 616d 6574 6572  ll...**Parameter
-00000b60: 733a 2a2a 0a0a 2d20 6073 6865 6c6c 5f69  s:**..- `shell_i
-00000b70: 6460 3a20 5468 6520 756e 6971 7565 2069  d`: The unique i
-00000b80: 6465 6e74 6966 6965 7220 6f66 2074 6865  dentifier of the
-00000b90: 2073 6865 6c6c 2e0a 0a23 2320 6077 6970   shell...## `wip
-00000ba0: 655f 616c 6c28 2960 0a0a 436c 6561 7273  e_all()`..Clears
-00000bb0: 2061 6c6c 2073 6865 6c6c 2061 6e64 2073   all shell and s
-00000bc0: 6865 6c6c 2068 6973 746f 7279 2064 6174  hell history dat
-00000bd0: 612e 0a0a 2323 2060 6c69 7374 5f61 6374  a...## `list_act
-00000be0: 6976 655f 7368 656c 6c73 2829 600a 0a52  ive_shells()`..R
-00000bf0: 6574 7572 6e73 2061 206c 6973 7420 6f66  eturns a list of
-00000c00: 2061 6374 6976 6520 7368 656c 6c73 2e0a   active shells..
-00000c10: 0a2a 2a52 6574 7572 6e73 3a2a 2a0a 0a2d  .**Returns:**..-
-00000c20: 2041 206c 6973 7420 6f66 2073 6865 6c6c   A list of shell
-00000c30: 2069 6465 6e74 6966 6965 7273 2e0a 0a23   identifiers...#
-00000c40: 2320 6063 6c6f 7365 5f73 6865 6c6c 2873  # `close_shell(s
-00000c50: 6865 6c6c 5f69 6429 600a 0a43 6c6f 7365  hell_id)`..Close
-00000c60: 7320 6120 7370 6563 6966 6963 2073 6865  s a specific she
-00000c70: 6c6c 2c20 636c 6561 7269 6e67 2069 7473  ll, clearing its
-00000c80: 2068 6973 746f 7279 2e0a 0a2a 2a50 6172   history...**Par
-00000c90: 616d 6574 6572 733a 2a2a 0a0a 2d20 6073  ameters:**..- `s
-00000ca0: 6865 6c6c 5f69 6460 3a20 5468 6520 756e  hell_id`: The un
-00000cb0: 6971 7565 2069 6465 6e74 6966 6965 7220  ique identifier 
-00000cc0: 6f66 2074 6865 2073 6865 6c6c 2e0a 0a23  of the shell...#
-00000cd0: 2320 606e 6577 5f73 6865 6c6c 2829 600a  # `new_shell()`.
-00000ce0: 0a43 7265 6174 6573 2061 206e 6577 2073  .Creates a new s
-00000cf0: 6865 6c6c 2061 6e64 2072 6574 7572 6e73  hell and returns
-00000d00: 2069 7473 2075 6e69 7175 6520 6964 656e   its unique iden
-00000d10: 7469 6669 6572 2e0a 0a2a 2a52 6574 7572  tifier...**Retur
-00000d20: 6e73 3a2a 2a0a 0a2d 2054 6865 2075 6e69  ns:**..- The uni
-00000d30: 7175 6520 6964 656e 7469 6669 6572 206f  que identifier o
-00000d40: 6620 7468 6520 6e65 7720 7368 656c 6c2e  f the new shell.
-00000d50: 0a0a 2323 2060 6765 745f 6377 6428 7368  ..## `get_cwd(sh
-00000d60: 656c 6c5f 6964 3d4e 6f6e 6529 600a 0a52  ell_id=None)`..R
-00000d70: 6574 7572 6e73 2074 6865 2063 7572 7265  eturns the curre
-00000d80: 6e74 2077 6f72 6b69 6e67 2064 6972 6563  nt working direc
-00000d90: 746f 7279 206f 6620 6120 7370 6563 6966  tory of a specif
-00000da0: 6963 2073 6865 6c6c 2e20 4966 2060 7368  ic shell. If `sh
-00000db0: 656c 6c5f 6964 6020 6973 206e 6f74 2073  ell_id` is not s
-00000dc0: 7065 6369 6669 6564 2c20 7573 6573 2074  pecified, uses t
-00000dd0: 6865 2063 7572 7265 6e74 2073 6865 6c6c  he current shell
-00000de0: 2e0a 0a2a 2a50 6172 616d 6574 6572 733a  ...**Parameters:
-00000df0: 2a2a 0a0a 2d20 6073 6865 6c6c 5f69 6460  **..- `shell_id`
-00000e00: 3a20 5468 6520 756e 6971 7565 2069 6465  : The unique ide
-00000e10: 6e74 6966 6965 7220 6f66 2074 6865 2073  ntifier of the s
-00000e20: 6865 6c6c 2e0a 0a2a 2a52 6574 7572 6e73  hell...**Returns
-00000e30: 3a2a 2a0a 0a2d 2054 6865 2063 7572 7265  :**..- The curre
-00000e40: 6e74 2077 6f72 6b69 6e67 2064 6972 6563  nt working direc
-00000e50: 746f 7279 206f 6620 7468 6520 7368 656c  tory of the shel
-00000e60: 6c2e 0a0a 2323 2060 7275 6e5f 636f 6d6d  l...## `run_comm
-00000e70: 616e 6428 636f 6d6d 616e 642c 2073 6865  and(command, she
-00000e80: 6c6c 5f69 643d 4e6f 6e65 2960 0a0a 5275  ll_id=None)`..Ru
-00000e90: 6e73 2061 2063 6f6d 6d61 6e64 2069 6e20  ns a command in 
-00000ea0: 6120 7370 6563 6966 6963 2073 6865 6c6c  a specific shell
-00000eb0: 2061 6e64 2061 6464 7320 6974 2074 6f20   and adds it to 
-00000ec0: 7468 6520 7368 656c 6c27 7320 6869 7374  the shell's hist
-00000ed0: 6f72 792e 2049 6620 6073 6865 6c6c 5f69  ory. If `shell_i
-00000ee0: 6460 2069 7320 6e6f 7420 7370 6563 6966  d` is not specif
-00000ef0: 6965 642c 2075 7365 7320 7468 6520 6375  ied, uses the cu
-00000f00: 7272 656e 7420 7368 656c 6c2e 0a0a 2a2a  rrent shell...**
-00000f10: 5061 7261 6d65 7465 7273 3a2a 2a0a 0a2d  Parameters:**..-
-00000f20: 2060 636f 6d6d 616e 6460 3a20 5468 6520   `command`: The 
-00000f30: 636f 6d6d 616e 6420 746f 2065 7865 6375  command to execu
-00000f40: 7465 2e0a 2d20 6073 6865 6c6c 5f69 6460  te..- `shell_id`
-00000f50: 3a20 5468 6520 756e 6971 7565 2069 6465  : The unique ide
-00000f60: 6e74 6966 6965 7220 6f66 2074 6865 2073  ntifier of the s
-00000f70: 6865 6c6c 2e0a 0a2a 2a52 6574 7572 6e73  hell...**Returns
-00000f80: 3a2a 2a0a 0a2d 2060 5472 7565 6020 6966  :**..- `True` if
-00000f90: 2074 6865 2063 6f6d 6d61 6e64 2077 6173   the command was
-00000fa0: 2073 7563 6365 7373 6675 6c2c 2060 4661   successful, `Fa
-00000fb0: 6c73 6560 206f 7468 6572 7769 7365 2e0a  lse` otherwise..
-00000fc0: 0a23 2043 6f6e 7472 6962 7574 696f 6e73  .# Contributions
-00000fd0: 2057 656c 636f 6d65 0a0a 4966 2079 6f75   Welcome..If you
-00000fe0: 206c 696b 6520 7468 6973 206c 6962 7261   like this libra
-00000ff0: 7279 2061 6e64 2077 616e 7420 746f 2063  ry and want to c
-00001000: 6f6e 7472 6962 7574 6520 696e 2061 6e79  ontribute in any
-00001010: 2077 6179 2c20 706c 6561 7365 2066 6565   way, please fee
-00001020: 6c20 6672 6565 2074 6f20 7375 626d 6974  l free to submit
-00001030: 2061 2050 5220 616e 6420 4920 7769 6c6c   a PR and I will
-00001040: 2072 6576 6965 7720 6974 2e20 506c 6561   review it. Plea
-00001050: 7365 206e 6f74 6520 7468 6174 2074 6865  se note that the
-00001060: 2067 6f61 6c20 6865 7265 2069 7320 7369   goal here is si
-00001070: 6d70 6c69 6369 7479 2061 6e64 2061 6363  mplicity and acc
-00001080: 6573 6962 696c 6974 792c 2075 7369 6e67  esibility, using
-00001090: 2063 6f6d 6d6f 6e20 6c61 6e67 7561 6765   common language
-000010a0: 2061 6e64 2066 6577 2064 6570 656e 6465   and few depende
-000010b0: 6e63 6965 732e 0a                        ncies..
+00000000: 2320 6167 656e 7473 6865 6c6c 203c 6120  # agentshell <a 
+00000010: 6872 6566 3d22 6874 7470 733a 2f2f 6469  href="https://di
+00000020: 7363 6f72 642e 6767 2f71 6574 5764 374a  scord.gg/qetWd7J
+00000030: 3944 6522 3e3c 696d 6720 7374 796c 653d  9De"><img style=
+00000040: 2266 6c6f 6174 3a20 7269 6768 7422 2073  "float: right" s
+00000050: 7263 3d22 6874 7470 733a 2f2f 6463 6261  rc="https://dcba
+00000060: 6467 652e 7665 7263 656c 2e61 7070 2f61  dge.vercel.app/a
+00000070: 7069 2f73 6572 7665 722f 7165 7457 6437  pi/server/qetWd7
+00000080: 4a39 4465 2220 616c 743d 2222 3e3c 2f61  J9De" alt=""></a
+00000090: 3e0a 0a41 2073 6865 6c6c 2066 6f72 2079  >..A shell for y
+000000a0: 6f75 7220 6167 656e 742e 2054 7261 636b  our agent. Track
+000000b0: 2073 7461 7465 2061 6e64 2068 6973 746f   state and histo
+000000c0: 7279 2c20 6d75 6c74 6970 6c65 2073 6865  ry, multiple she
+000000d0: 6c6c 732c 2061 6e64 206d 6f72 652e 0a0a  lls, and more...
+000000e0: 3c69 6d67 2073 7263 3d22 7265 736f 7572  <img src="resour
+000000f0: 6365 732f 696d 6167 652e 6a70 6722 3e0a  ces/image.jpg">.
+00000100: 0a5b 215b 4c69 6e74 2061 6e64 2054 6573  .[![Lint and Tes
+00000110: 745d 2868 7474 7073 3a2f 2f67 6974 6875  t](https://githu
+00000120: 622e 636f 6d2f 4175 746f 6e6f 6d6f 7573  b.com/Autonomous
+00000130: 5265 7365 6172 6368 4772 6f75 702f 6167  ResearchGroup/ag
+00000140: 656e 7473 6865 6c6c 2f61 6374 696f 6e73  entshell/actions
+00000150: 2f77 6f72 6b66 6c6f 7773 2f74 6573 742e  /workflows/test.
+00000160: 796d 6c2f 6261 6467 652e 7376 6729 5d28  yml/badge.svg)](
+00000170: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000180: 6f6d 2f41 7574 6f6e 6f6d 6f75 7352 6573  om/AutonomousRes
+00000190: 6561 7263 6847 726f 7570 2f61 6765 6e74  earchGroup/agent
+000001a0: 7368 656c 6c2f 6163 7469 6f6e 732f 776f  shell/actions/wo
+000001b0: 726b 666c 6f77 732f 7465 7374 2e79 6d6c  rkflows/test.yml
+000001c0: 290a 5b21 5b50 7950 4920 7665 7273 696f  ).[![PyPI versio
+000001d0: 6e5d 2868 7474 7073 3a2f 2f62 6164 6765  n](https://badge
+000001e0: 2e66 7572 792e 696f 2f70 792f 6167 656e  .fury.io/py/agen
+000001f0: 7473 6865 6c6c 2e73 7667 295d 2868 7474  tshell.svg)](htt
+00000200: 7073 3a2f 2f62 6164 6765 2e66 7572 792e  ps://badge.fury.
+00000210: 696f 2f70 792f 6167 656e 7473 6865 6c6c  io/py/agentshell
+00000220: 290a 0a23 2049 6e73 7461 6c6c 6174 696f  )..# Installatio
+00000230: 6e0a 0a60 6060 6261 7368 0a70 6970 2069  n..```bash.pip i
+00000240: 6e73 7461 6c6c 2061 6765 6e74 7368 656c  nstall agentshel
+00000250: 6c0a 6060 600a 0a23 2044 6f63 756d 656e  l.```..# Documen
+00000260: 7461 7469 6f6e 0a0a 2323 2060 6765 745f  tation..## `get_
+00000270: 6669 6c65 735f 696e 5f63 7764 2873 6865  files_in_cwd(she
+00000280: 6c6c 5f69 643d 4e6f 6e65 2960 0a0a 5265  ll_id=None)`..Re
+00000290: 7475 726e 7320 6120 6c69 7374 206f 6620  turns a list of 
+000002a0: 6669 6c65 7320 696e 2074 6865 2063 7572  files in the cur
+000002b0: 7265 6e74 2064 6972 6563 746f 7279 206f  rent directory o
+000002c0: 6620 6120 7370 6563 6966 6963 2073 6865  f a specific she
+000002d0: 6c6c 2e20 4966 2060 7368 656c 6c5f 6964  ll. If `shell_id
+000002e0: 6020 6973 206e 6f74 2073 7065 6369 6669  ` is not specifi
+000002f0: 6564 2c20 7573 6573 2074 6865 2063 7572  ed, uses the cur
+00000300: 7265 6e74 2073 6865 6c6c 2e0a 0a2a 2a50  rent shell...**P
+00000310: 6172 616d 6574 6572 733a 2a2a 0a0a 2d20  arameters:**..- 
+00000320: 6073 6865 6c6c 5f69 6460 3a20 5468 6520  `shell_id`: The 
+00000330: 756e 6971 7565 2069 6465 6e74 6966 6965  unique identifie
+00000340: 7220 6f66 2074 6865 2073 6865 6c6c 2e0a  r of the shell..
+00000350: 0a2a 2a52 6574 7572 6e73 3a2a 2a0a 0a2d  .**Returns:**..-
+00000360: 2041 206c 6973 7420 6f66 2066 696c 656e   A list of filen
+00000370: 616d 6573 2069 6e20 7468 6520 6375 7272  ames in the curr
+00000380: 656e 7420 6469 7265 6374 6f72 792e 0a0a  ent directory...
+00000390: 2323 2060 6765 745f 6375 7272 656e 745f  ## `get_current_
+000003a0: 7368 656c 6c28 2960 0a0a 5265 7475 726e  shell()`..Return
+000003b0: 7320 7468 6520 756e 6971 7565 2069 6465  s the unique ide
+000003c0: 6e74 6966 6965 7220 6f66 2074 6865 2063  ntifier of the c
+000003d0: 7572 7265 6e74 2073 6865 6c6c 2e20 4966  urrent shell. If
+000003e0: 206e 6f20 7368 656c 6c20 6973 2063 7572   no shell is cur
+000003f0: 7265 6e74 6c79 2061 6374 6976 652c 2063  rently active, c
+00000400: 7265 6174 6573 2061 206e 6577 2073 6865  reates a new she
+00000410: 6c6c 2061 6e64 2072 6574 7572 6e73 2069  ll and returns i
+00000420: 7473 2069 6465 6e74 6966 6965 722e 0a0a  ts identifier...
+00000430: 2a2a 5265 7475 726e 733a 2a2a 0a0a 2d20  **Returns:**..- 
+00000440: 5468 6520 756e 6971 7565 2069 6465 6e74  The unique ident
+00000450: 6966 6965 7220 6f66 2074 6865 2063 7572  ifier of the cur
+00000460: 7265 6e74 2073 6865 6c6c 2e0a 0a23 2320  rent shell...## 
+00000470: 6073 6574 5f63 7764 2863 7764 2c20 7368  `set_cwd(cwd, sh
+00000480: 656c 6c5f 6964 3d4e 6f6e 6529 600a 0a53  ell_id=None)`..S
+00000490: 6574 7320 7468 6520 6375 7272 656e 7420  ets the current 
+000004a0: 776f 726b 696e 6720 6469 7265 6374 6f72  working director
+000004b0: 7920 6f66 2061 2073 7065 6369 6669 6320  y of a specific 
+000004c0: 7368 656c 6c2e 2049 6620 6073 6865 6c6c  shell. If `shell
+000004d0: 5f69 6460 2069 7320 6e6f 7420 7370 6563  _id` is not spec
+000004e0: 6966 6965 642c 2075 7365 7320 7468 6520  ified, uses the 
+000004f0: 6375 7272 656e 7420 7368 656c 6c2e 0a0a  current shell...
+00000500: 2a2a 5061 7261 6d65 7465 7273 3a2a 2a0a  **Parameters:**.
+00000510: 0a2d 2060 6377 6460 3a20 5468 6520 6e65  .- `cwd`: The ne
+00000520: 7720 6375 7272 656e 7420 776f 726b 696e  w current workin
+00000530: 6720 6469 7265 6374 6f72 792e 0a2d 2060  g directory..- `
+00000540: 7368 656c 6c5f 6964 603a 2054 6865 2075  shell_id`: The u
+00000550: 6e69 7175 6520 6964 656e 7469 6669 6572  nique identifier
+00000560: 206f 6620 7468 6520 7368 656c 6c2e 0a0a   of the shell...
+00000570: 2323 2060 7365 745f 6375 7272 656e 745f  ## `set_current_
+00000580: 7368 656c 6c28 7368 656c 6c5f 6964 2960  shell(shell_id)`
+00000590: 0a0a 5365 7473 2074 6865 2063 7572 7265  ..Sets the curre
+000005a0: 6e74 2073 6865 6c6c 2074 6f20 7468 6520  nt shell to the 
+000005b0: 7368 656c 6c20 7769 7468 2074 6865 2073  shell with the s
+000005c0: 7065 6369 6669 6564 2069 6465 6e74 6966  pecified identif
+000005d0: 6965 722e 0a0a 2a2a 5061 7261 6d65 7465  ier...**Paramete
+000005e0: 7273 3a2a 2a0a 0a2d 2060 7368 656c 6c5f  rs:**..- `shell_
+000005f0: 6964 603a 2054 6865 2075 6e69 7175 6520  id`: The unique 
+00000600: 6964 656e 7469 6669 6572 206f 6620 7468  identifier of th
+00000610: 6520 7368 656c 6c20 746f 2062 6520 6d61  e shell to be ma
+00000620: 6465 2063 7572 7265 6e74 2e0a 0a23 2320  de current...## 
+00000630: 6067 6574 5f68 6973 746f 7279 2873 6865  `get_history(she
+00000640: 6c6c 5f69 643d 4e6f 6e65 2c20 6e5f 6c69  ll_id=None, n_li
+00000650: 6d69 743d 3230 2960 0a0a 5265 7475 726e  mit=20)`..Return
+00000660: 7320 7468 6520 636f 6d6d 616e 6420 6869  s the command hi
+00000670: 7374 6f72 7920 6f66 2061 2073 7065 6369  story of a speci
+00000680: 6669 6320 7368 656c 6c2e 2049 6620 6073  fic shell. If `s
+00000690: 6865 6c6c 5f69 6460 2069 7320 6e6f 7420  hell_id` is not 
+000006a0: 7370 6563 6966 6965 642c 2075 7365 7320  specified, uses 
+000006b0: 7468 6520 6375 7272 656e 7420 7368 656c  the current shel
+000006c0: 6c2e 0a0a 2a2a 5061 7261 6d65 7465 7273  l...**Parameters
+000006d0: 3a2a 2a0a 0a2d 2060 7368 656c 6c5f 6964  :**..- `shell_id
+000006e0: 603a 2054 6865 2075 6e69 7175 6520 6964  `: The unique id
+000006f0: 656e 7469 6669 6572 206f 6620 7468 6520  entifier of the 
+00000700: 7368 656c 6c2e 0a2d 2060 6e5f 6c69 6d69  shell..- `n_limi
+00000710: 7460 3a20 5468 6520 6d61 7869 6d75 6d20  t`: The maximum 
+00000720: 6e75 6d62 6572 206f 6620 6869 7374 6f72  number of histor
+00000730: 7920 656e 7472 6965 7320 746f 2072 6574  y entries to ret
+00000740: 7572 6e2e 0a0a 2a2a 5265 7475 726e 733a  urn...**Returns:
+00000750: 2a2a 0a0a 2d20 4120 6c69 7374 206f 6620  **..- A list of 
+00000760: 6469 6374 696f 6e61 7269 6573 2c20 6561  dictionaries, ea
+00000770: 6368 2072 6570 7265 7365 6e74 696e 6720  ch representing 
+00000780: 6120 636f 6d6d 616e 6420 616e 6420 6974  a command and it
+00000790: 7320 7265 7375 6c74 2e0a 0a23 2320 6067  s result...## `g
+000007a0: 6574 5f68 6973 746f 7279 5f66 6f72 6d61  et_history_forma
+000007b0: 7474 6564 2873 6865 6c6c 5f69 643d 4e6f  tted(shell_id=No
+000007c0: 6e65 2960 0a0a 5265 7475 726e 7320 7468  ne)`..Returns th
+000007d0: 6520 636f 6d6d 616e 6420 6869 7374 6f72  e command histor
+000007e0: 7920 6f66 2061 2073 7065 6369 6669 6320  y of a specific 
+000007f0: 7368 656c 6c20 696e 2061 2068 756d 616e  shell in a human
+00000800: 2d72 6561 6461 626c 6520 666f 726d 6174  -readable format
+00000810: 2e20 4966 2060 7368 656c 6c5f 6964 6020  . If `shell_id` 
+00000820: 6973 206e 6f74 2073 7065 6369 6669 6564  is not specified
+00000830: 2c20 7573 6573 2074 6865 2063 7572 7265  , uses the curre
+00000840: 6e74 2073 6865 6c6c 2e0a 0a2a 2a50 6172  nt shell...**Par
+00000850: 616d 6574 6572 733a 2a2a 0a0a 2d20 6073  ameters:**..- `s
+00000860: 6865 6c6c 5f69 6460 3a20 5468 6520 756e  hell_id`: The un
+00000870: 6971 7565 2069 6465 6e74 6966 6965 7220  ique identifier 
+00000880: 6f66 2074 6865 2073 6865 6c6c 2e0a 0a2a  of the shell...*
+00000890: 2a52 6574 7572 6e73 3a2a 2a0a 0a2d 2054  *Returns:**..- T
+000008a0: 6865 2063 6f6d 6d61 6e64 2068 6973 746f  he command histo
+000008b0: 7279 2069 6e20 6875 6d61 6e2d 7265 6164  ry in human-read
+000008c0: 6162 6c65 2066 6f72 6d61 742e 0a0a 2323  able format...##
+000008d0: 2060 6164 645f 746f 5f73 6865 6c6c 5f68   `add_to_shell_h
+000008e0: 6973 746f 7279 2873 6865 6c6c 5f69 642c  istory(shell_id,
+000008f0: 2063 6f6d 6d61 6e64 2c20 7375 6363 6573   command, succes
+00000900: 732c 206f 7574 7075 742c 2065 7272 6f72  s, output, error
+00000910: 3d4e 6f6e 6529 600a 0a41 6464 7320 6120  =None)`..Adds a 
+00000920: 636f 6d6d 616e 6420 616e 6420 6974 7320  command and its 
+00000930: 7265 7375 6c74 2074 6f20 7468 6520 6869  result to the hi
+00000940: 7374 6f72 7920 6f66 2061 2073 7065 6369  story of a speci
+00000950: 6669 6320 7368 656c 6c2e 0a0a 2a2a 5061  fic shell...**Pa
+00000960: 7261 6d65 7465 7273 3a2a 2a0a 0a2d 2060  rameters:**..- `
+00000970: 7368 656c 6c5f 6964 603a 2054 6865 2075  shell_id`: The u
+00000980: 6e69 7175 6520 6964 656e 7469 6669 6572  nique identifier
+00000990: 206f 6620 7468 6520 7368 656c 6c2e 0a2d   of the shell..-
+000009a0: 2060 636f 6d6d 616e 6460 3a20 5468 6520   `command`: The 
+000009b0: 636f 6d6d 616e 6420 7468 6174 2077 6173  command that was
+000009c0: 2065 7865 6375 7465 642e 0a2d 2060 7375   executed..- `su
+000009d0: 6363 6573 7360 3a20 5768 6574 6865 7220  ccess`: Whether 
+000009e0: 7468 6520 636f 6d6d 616e 6420 7761 7320  the command was 
+000009f0: 7375 6363 6573 7366 756c 2e0a 2d20 606f  successful..- `o
+00000a00: 7574 7075 7460 3a20 5468 6520 6f75 7470  utput`: The outp
+00000a10: 7574 206f 6620 7468 6520 636f 6d6d 616e  ut of the comman
+00000a20: 642e 0a2d 2060 6572 726f 7260 3a20 416e  d..- `error`: An
+00000a30: 7920 6572 726f 7220 6d65 7373 6167 6573  y error messages
+00000a40: 2070 726f 6475 6365 6420 6279 2074 6865   produced by the
+00000a50: 2063 6f6d 6d61 6e64 2e0a 0a23 2320 6063   command...## `c
+00000a60: 6c65 6172 5f68 6973 746f 7279 2873 6865  lear_history(she
+00000a70: 6c6c 5f69 6429 600a 0a43 6c65 6172 7320  ll_id)`..Clears 
+00000a80: 7468 6520 636f 6d6d 616e 6420 6869 7374  the command hist
+00000a90: 6f72 7920 6f66 2061 2073 7065 6369 6669  ory of a specifi
+00000aa0: 6320 7368 656c 6c2e 0a0a 2a2a 5061 7261  c shell...**Para
+00000ab0: 6d65 7465 7273 3a2a 2a0a 0a2d 2060 7368  meters:**..- `sh
+00000ac0: 656c 6c5f 6964 603a 2054 6865 2075 6e69  ell_id`: The uni
+00000ad0: 7175 6520 6964 656e 7469 6669 6572 206f  que identifier o
+00000ae0: 6620 7468 6520 7368 656c 6c2e 0a0a 2323  f the shell...##
+00000af0: 2060 7769 7065 5f61 6c6c 2829 600a 0a43   `wipe_all()`..C
+00000b00: 6c65 6172 7320 616c 6c20 7368 656c 6c20  lears all shell 
+00000b10: 616e 6420 7368 656c 6c20 6869 7374 6f72  and shell histor
+00000b20: 7920 6461 7461 2e0a 0a23 2320 606c 6973  y data...## `lis
+00000b30: 745f 6163 7469 7665 5f73 6865 6c6c 7328  t_active_shells(
+00000b40: 2960 0a0a 5265 7475 726e 7320 6120 6c69  )`..Returns a li
+00000b50: 7374 206f 6620 6163 7469 7665 2073 6865  st of active she
+00000b60: 6c6c 732e 0a0a 2a2a 5265 7475 726e 733a  lls...**Returns:
+00000b70: 2a2a 0a0a 2d20 4120 6c69 7374 206f 6620  **..- A list of 
+00000b80: 7368 656c 6c20 6964 656e 7469 6669 6572  shell identifier
+00000b90: 732e 0a0a 2323 2060 636c 6f73 655f 7368  s...## `close_sh
+00000ba0: 656c 6c28 7368 656c 6c5f 6964 2960 0a0a  ell(shell_id)`..
+00000bb0: 436c 6f73 6573 2061 2073 7065 6369 6669  Closes a specifi
+00000bc0: 6320 7368 656c 6c2c 2063 6c65 6172 696e  c shell, clearin
+00000bd0: 6720 6974 7320 6869 7374 6f72 792e 0a0a  g its history...
+00000be0: 2a2a 5061 7261 6d65 7465 7273 3a2a 2a0a  **Parameters:**.
+00000bf0: 0a2d 2060 7368 656c 6c5f 6964 603a 2054  .- `shell_id`: T
+00000c00: 6865 2075 6e69 7175 6520 6964 656e 7469  he unique identi
+00000c10: 6669 6572 206f 6620 7468 6520 7368 656c  fier of the shel
+00000c20: 6c2e 0a0a 2323 2060 6e65 775f 7368 656c  l...## `new_shel
+00000c30: 6c28 2960 0a0a 4372 6561 7465 7320 6120  l()`..Creates a 
+00000c40: 6e65 7720 7368 656c 6c20 616e 6420 7265  new shell and re
+00000c50: 7475 726e 7320 6974 7320 756e 6971 7565  turns its unique
+00000c60: 2069 6465 6e74 6966 6965 722e 0a0a 2a2a   identifier...**
+00000c70: 5265 7475 726e 733a 2a2a 0a0a 2d20 5468  Returns:**..- Th
+00000c80: 6520 756e 6971 7565 2069 6465 6e74 6966  e unique identif
+00000c90: 6965 7220 6f66 2074 6865 206e 6577 2073  ier of the new s
+00000ca0: 6865 6c6c 2e0a 0a23 2320 6067 6574 5f63  hell...## `get_c
+00000cb0: 7764 2873 6865 6c6c 5f69 643d 4e6f 6e65  wd(shell_id=None
+00000cc0: 2960 0a0a 5265 7475 726e 7320 7468 6520  )`..Returns the 
+00000cd0: 6375 7272 656e 7420 776f 726b 696e 6720  current working 
+00000ce0: 6469 7265 6374 6f72 7920 6f66 2061 2073  directory of a s
+00000cf0: 7065 6369 6669 6320 7368 656c 6c2e 2049  pecific shell. I
+00000d00: 6620 6073 6865 6c6c 5f69 6460 2069 7320  f `shell_id` is 
+00000d10: 6e6f 7420 7370 6563 6966 6965 642c 2075  not specified, u
+00000d20: 7365 7320 7468 6520 6375 7272 656e 7420  ses the current 
+00000d30: 7368 656c 6c2e 0a0a 2a2a 5061 7261 6d65  shell...**Parame
+00000d40: 7465 7273 3a2a 2a0a 0a2d 2060 7368 656c  ters:**..- `shel
+00000d50: 6c5f 6964 603a 2054 6865 2075 6e69 7175  l_id`: The uniqu
+00000d60: 6520 6964 656e 7469 6669 6572 206f 6620  e identifier of 
+00000d70: 7468 6520 7368 656c 6c2e 0a0a 2a2a 5265  the shell...**Re
+00000d80: 7475 726e 733a 2a2a 0a0a 2d20 5468 6520  turns:**..- The 
+00000d90: 6375 7272 656e 7420 776f 726b 696e 6720  current working 
+00000da0: 6469 7265 6374 6f72 7920 6f66 2074 6865  directory of the
+00000db0: 2073 6865 6c6c 2e0a 0a23 2320 6072 756e   shell...## `run
+00000dc0: 5f63 6f6d 6d61 6e64 2863 6f6d 6d61 6e64  _command(command
+00000dd0: 2c20 7368 656c 6c5f 6964 3d4e 6f6e 6529  , shell_id=None)
+00000de0: 600a 0a52 756e 7320 6120 636f 6d6d 616e  `..Runs a comman
+00000df0: 6420 696e 2061 2073 7065 6369 6669 6320  d in a specific 
+00000e00: 7368 656c 6c20 616e 6420 6164 6473 2069  shell and adds i
+00000e10: 7420 746f 2074 6865 2073 6865 6c6c 2773  t to the shell's
+00000e20: 2068 6973 746f 7279 2e20 4966 2060 7368   history. If `sh
+00000e30: 656c 6c5f 6964 6020 6973 206e 6f74 2073  ell_id` is not s
+00000e40: 7065 6369 6669 6564 2c20 7573 6573 2074  pecified, uses t
+00000e50: 6865 2063 7572 7265 6e74 2073 6865 6c6c  he current shell
+00000e60: 2e0a 0a2a 2a50 6172 616d 6574 6572 733a  ...**Parameters:
+00000e70: 2a2a 0a0a 2d20 6063 6f6d 6d61 6e64 603a  **..- `command`:
+00000e80: 2054 6865 2063 6f6d 6d61 6e64 2074 6f20   The command to 
+00000e90: 6578 6563 7574 652e 0a2d 2060 7368 656c  execute..- `shel
+00000ea0: 6c5f 6964 603a 2054 6865 2075 6e69 7175  l_id`: The uniqu
+00000eb0: 6520 6964 656e 7469 6669 6572 206f 6620  e identifier of 
+00000ec0: 7468 6520 7368 656c 6c2e 0a0a 2a2a 5265  the shell...**Re
+00000ed0: 7475 726e 733a 2a2a 0a0a 2d20 6054 7275  turns:**..- `Tru
+00000ee0: 6560 2069 6620 7468 6520 636f 6d6d 616e  e` if the comman
+00000ef0: 6420 7761 7320 7375 6363 6573 7366 756c  d was successful
+00000f00: 2c20 6046 616c 7365 6020 6f74 6865 7277  , `False` otherw
+00000f10: 6973 652e 0a0a 2320 436f 6e74 7269 6275  ise...# Contribu
+00000f20: 7469 6f6e 7320 5765 6c63 6f6d 650a 0a49  tions Welcome..I
+00000f30: 6620 796f 7520 6c69 6b65 2074 6869 7320  f you like this 
+00000f40: 6c69 6272 6172 7920 616e 6420 7761 6e74  library and want
+00000f50: 2074 6f20 636f 6e74 7269 6275 7465 2069   to contribute i
+00000f60: 6e20 616e 7920 7761 792c 2070 6c65 6173  n any way, pleas
+00000f70: 6520 6665 656c 2066 7265 6520 746f 2073  e feel free to s
+00000f80: 7562 6d69 7420 6120 5052 2061 6e64 2049  ubmit a PR and I
+00000f90: 2077 696c 6c20 7265 7669 6577 2069 742e   will review it.
+00000fa0: 2050 6c65 6173 6520 6e6f 7465 2074 6861   Please note tha
+00000fb0: 7420 7468 6520 676f 616c 2068 6572 6520  t the goal here 
+00000fc0: 6973 2073 696d 706c 6963 6974 7920 616e  is simplicity an
+00000fd0: 6420 6163 6365 7369 6269 6c69 7479 2c20  d accesibility, 
+00000fe0: 7573 696e 6720 636f 6d6d 6f6e 206c 616e  using common lan
+00000ff0: 6775 6167 6520 616e 6420 6665 7720 6465  guage and few de
+00001000: 7065 6e64 656e 6369 6573 2e0a            pendencies..
```

### Comparing `agentshell-0.0.4/setup.py` & `agentshell-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = [line for line in long_description if not "<img" in line]
     # now join all the lines back together
     long_description = "\n".join(long_description)
 
 
 setup(
     name="agentshell",
-    version="0.0.4",
+    version="0.0.6",
     description="A shell for your agent.",
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url="https://github.com/AutonomousResearchGroup/agentshell",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
```

