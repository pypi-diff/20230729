# Comparing `tmp/wordlistools-0.1.8.tar.gz` & `tmp/wordlistools-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordlistools-0.1.8.tar", last modified: Fri Mar 11 15:32:49 2022, max compression
+gzip compressed data, was "wordlistools-0.1.9.tar", last modified: Sat Jan 28 17:10:12 2023, max compression
```

## Comparing `wordlistools-0.1.8.tar` & `wordlistools-0.1.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2022-03-11 15:32:49.923080 wordlistools-0.1.8/
--rw-r--r--   0 nazime    (1000) nazime    (1000)     1063 2021-08-13 11:09:57.000000 wordlistools-0.1.8/LICENSE
--rw-r--r--   0 nazime    (1000) nazime    (1000)       18 2021-08-13 11:09:57.000000 wordlistools-0.1.8/MANIFEST.in
--rw-rw-r--   0 nazime    (1000) nazime    (1000)     4960 2022-03-11 15:32:49.923080 wordlistools-0.1.8/PKG-INFO
--rw-rw-r--   0 nazime    (1000) nazime    (1000)     3256 2022-03-03 14:17:09.000000 wordlistools-0.1.8/README.md
--rw-r--r--   0 nazime    (1000) nazime    (1000)      121 2021-08-13 11:09:57.000000 wordlistools-0.1.8/pyproject.toml
--rw-r--r--   0 nazime    (1000) nazime    (1000)       73 2022-03-11 15:32:49.923080 wordlistools-0.1.8/setup.cfg
--rw-r--r--   0 nazime    (1000) nazime    (1000)     3135 2022-02-06 20:59:54.000000 wordlistools-0.1.8/setup.py
-drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2022-03-11 15:32:49.919080 wordlistools-0.1.8/src/
-drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2022-03-11 15:32:49.923080 wordlistools-0.1.8/src/wordlistools/
--rw-r--r--   0 nazime    (1000) nazime    (1000)      309 2022-02-06 21:19:53.000000 wordlistools-0.1.8/src/wordlistools/__init__.py
--rw-r--r--   0 nazime    (1000) nazime    (1000)       91 2021-08-13 11:09:57.000000 wordlistools-0.1.8/src/wordlistools/__main__.py
--rw-r--r--   0 nazime    (1000) nazime    (1000)      560 2021-08-18 15:54:46.000000 wordlistools-0.1.8/src/wordlistools/api.py
--rw-rw-r--   0 nazime    (1000) nazime    (1000)     4763 2022-02-06 22:13:56.000000 wordlistools-0.1.8/src/wordlistools/base.py
--rw-r--r--   0 nazime    (1000) nazime    (1000)     8523 2022-02-06 21:03:38.000000 wordlistools-0.1.8/src/wordlistools/cmdline.py
--rw-rw-r--   0 nazime    (1000) nazime    (1000)      402 2022-03-11 15:32:20.000000 wordlistools-0.1.8/src/wordlistools/consts.py
--rw-r--r--   0 nazime    (1000) nazime    (1000)     8292 2021-08-18 15:53:06.000000 wordlistools-0.1.8/src/wordlistools/helpertest.py
--rw-r--r--   0 nazime    (1000) nazime    (1000)      237 2021-08-13 11:09:57.000000 wordlistools-0.1.8/src/wordlistools/parsers.py
-drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2022-03-11 15:32:49.923080 wordlistools-0.1.8/src/wordlistools/plugins/
--rw-rw-r--   0 nazime    (1000) nazime    (1000)       87 2022-02-06 21:19:30.000000 wordlistools-0.1.8/src/wordlistools/plugins/__init__.py
--rw-rw-r--   0 nazime    (1000) nazime    (1000)     9952 2022-03-11 15:32:20.000000 wordlistools-0.1.8/src/wordlistools/plugins/filters_tools.py
--rw-rw-r--   0 nazime    (1000) nazime    (1000)     4523 2022-03-11 15:32:20.000000 wordlistools-0.1.8/src/wordlistools/plugins/modifiers_tools.py
--rw-r--r--   0 nazime    (1000) nazime    (1000)     8493 2022-02-06 20:46:28.000000 wordlistools-0.1.8/src/wordlistools/plugins/plugins.py
--rw-rw-r--   0 nazime    (1000) nazime    (1000)     2760 2022-02-06 20:46:18.000000 wordlistools-0.1.8/src/wordlistools/plugins/statistics_tools.py
-drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2022-03-11 15:32:49.923080 wordlistools-0.1.8/src/wordlistools.egg-info/
--rw-rw-r--   0 nazime    (1000) nazime    (1000)     4960 2022-03-11 15:32:49.000000 wordlistools-0.1.8/src/wordlistools.egg-info/PKG-INFO
--rw-rw-r--   0 nazime    (1000) nazime    (1000)      769 2022-03-11 15:32:49.000000 wordlistools-0.1.8/src/wordlistools.egg-info/SOURCES.txt
--rw-rw-r--   0 nazime    (1000) nazime    (1000)        1 2022-03-11 15:32:49.000000 wordlistools-0.1.8/src/wordlistools.egg-info/dependency_links.txt
--rw-rw-r--   0 nazime    (1000) nazime    (1000)       61 2022-03-11 15:32:49.000000 wordlistools-0.1.8/src/wordlistools.egg-info/entry_points.txt
--rw-rw-r--   0 nazime    (1000) nazime    (1000)        1 2021-08-13 11:18:55.000000 wordlistools-0.1.8/src/wordlistools.egg-info/not-zip-safe
--rw-rw-r--   0 nazime    (1000) nazime    (1000)      227 2022-03-11 15:32:49.000000 wordlistools-0.1.8/src/wordlistools.egg-info/requires.txt
--rw-rw-r--   0 nazime    (1000) nazime    (1000)       13 2022-03-11 15:32:49.000000 wordlistools-0.1.8/src/wordlistools.egg-info/top_level.txt
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-01-28 17:10:12.564993 wordlistools-0.1.9/
+-rw-r--r--   0 nazime    (1000) nazime    (1000)     1063 2021-08-13 11:09:57.000000 wordlistools-0.1.9/LICENSE
+-rw-r--r--   0 nazime    (1000) nazime    (1000)       18 2021-08-13 11:09:57.000000 wordlistools-0.1.9/MANIFEST.in
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     4287 2023-01-28 17:10:12.564993 wordlistools-0.1.9/PKG-INFO
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     3256 2022-03-03 14:17:09.000000 wordlistools-0.1.9/README.md
+-rw-r--r--   0 nazime    (1000) nazime    (1000)      121 2021-08-13 11:09:57.000000 wordlistools-0.1.9/pyproject.toml
+-rw-r--r--   0 nazime    (1000) nazime    (1000)       73 2023-01-28 17:10:12.564993 wordlistools-0.1.9/setup.cfg
+-rw-r--r--   0 nazime    (1000) nazime    (1000)     3135 2023-01-28 17:04:28.000000 wordlistools-0.1.9/setup.py
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-01-28 17:10:12.560993 wordlistools-0.1.9/src/
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-01-28 17:10:12.560993 wordlistools-0.1.9/src/wordlistools/
+-rw-r--r--   0 nazime    (1000) nazime    (1000)      309 2022-02-06 21:19:53.000000 wordlistools-0.1.9/src/wordlistools/__init__.py
+-rw-r--r--   0 nazime    (1000) nazime    (1000)       91 2021-08-13 11:09:57.000000 wordlistools-0.1.9/src/wordlistools/__main__.py
+-rw-r--r--   0 nazime    (1000) nazime    (1000)      560 2021-08-18 15:54:46.000000 wordlistools-0.1.9/src/wordlistools/api.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     4764 2023-01-28 16:23:44.000000 wordlistools-0.1.9/src/wordlistools/base.py
+-rw-r--r--   0 nazime    (1000) nazime    (1000)     4739 2023-01-28 16:59:35.000000 wordlistools-0.1.9/src/wordlistools/cmdline.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)      410 2023-01-28 17:07:05.000000 wordlistools-0.1.9/src/wordlistools/consts.py
+-rw-r--r--   0 nazime    (1000) nazime    (1000)     8292 2021-08-18 15:53:06.000000 wordlistools-0.1.9/src/wordlistools/helpertest.py
+-rw-r--r--   0 nazime    (1000) nazime    (1000)      237 2021-08-13 11:09:57.000000 wordlistools-0.1.9/src/wordlistools/parsers.py
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-01-28 17:10:12.564993 wordlistools-0.1.9/src/wordlistools/plugins/
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)       87 2022-02-06 21:19:30.000000 wordlistools-0.1.9/src/wordlistools/plugins/__init__.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     9952 2022-03-11 15:32:20.000000 wordlistools-0.1.9/src/wordlistools/plugins/filters_tools.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     4523 2022-03-11 15:32:20.000000 wordlistools-0.1.9/src/wordlistools/plugins/modifiers_tools.py
+-rw-r--r--   0 nazime    (1000) nazime    (1000)     8495 2023-01-28 16:52:24.000000 wordlistools-0.1.9/src/wordlistools/plugins/plugins.py
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     2760 2022-02-06 20:46:18.000000 wordlistools-0.1.9/src/wordlistools/plugins/statistics_tools.py
+drwxrwxr-x   0 nazime    (1000) nazime    (1000)        0 2023-01-28 17:10:12.564993 wordlistools-0.1.9/src/wordlistools.egg-info/
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)     4287 2023-01-28 17:10:12.000000 wordlistools-0.1.9/src/wordlistools.egg-info/PKG-INFO
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)      769 2023-01-28 17:10:12.000000 wordlistools-0.1.9/src/wordlistools.egg-info/SOURCES.txt
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)        1 2023-01-28 17:10:12.000000 wordlistools-0.1.9/src/wordlistools.egg-info/dependency_links.txt
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)       60 2023-01-28 17:10:12.000000 wordlistools-0.1.9/src/wordlistools.egg-info/entry_points.txt
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)        1 2021-08-13 11:18:55.000000 wordlistools-0.1.9/src/wordlistools.egg-info/not-zip-safe
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)      227 2023-01-28 17:10:12.000000 wordlistools-0.1.9/src/wordlistools.egg-info/requires.txt
+-rw-rw-r--   0 nazime    (1000) nazime    (1000)       13 2023-01-28 17:10:12.000000 wordlistools-0.1.9/src/wordlistools.egg-info/top_level.txt
```

### Comparing `wordlistools-0.1.8/LICENSE` & `wordlistools-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wordlistools-0.1.8/PKG-INFO` & `wordlistools-0.1.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,112 +1,112 @@
 Metadata-Version: 2.1
 Name: wordlistools
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tools to play with wordlists
 Home-page: https://github.com/nazime/wordlistools
 Author: Nazime LAKEHAL
 Author-email: nazime.lkh@gmail.com
 Maintainer: Nazime LAKEHAL
 Maintainer-email: nazime.lkh@gmail.com
 License: MIT
 Project-URL: Documentation, https://wordlistools.readthedocs.org/
 Project-URL: Bug Tracker, https://github.com/nazime/wordlistools/issues
 Project-URL: Source Code, https://github.com/nazime/wordlistools
-Description: # wordlistools
-        Wordlistools is a collection of tools to play with wordlists. This tool was built with offensive security in mind,
-        to help bruteforcing, filtering wordlists to crack passwords, building
-        wordlists for fuzzing, etc.
-        This project is still under development.
-        
-        **Features**
-        
-        - Can be used as command lines or as a python library
-        - Can be used with stdin redirection ``|``
-        - Easily extensible, you can add your own plugins on your home directory ```~/.koalak/wordlistools/plugins```
-        
-        
-        ![wordlistools demo](https://raw.githubusercontent.com/nazime/wordlistools/master/images/help_v0.1.3.png)
-        
-        
-        ## Install
-        
-        ```bash
-        pip3 install wordlistools
-        ```
-        
-        ## Demonstration
-        Note: This demonstration is an old version of wordlistools,
-        but the principe remains the same.
-        [![wordlistools demo](https://raw.githubusercontent.com/nazime/wordlistools/master/images/wordlistools.gif)](https://asciinema.org/a/430731)
-        
-        
-        ## Using policy subcommand
-        You can filter your wordlist based on a policy, the policy follow the following format ``[base_policy][lenght_policy]``.
-        The base policy can have the following rules:
-        - a: word must contain at least one lower case letter
-        - A: word must contain at least one upper case letter
-        - 1: word must contain at least one digit
-        - @: word must contain at least one special character
-        
-        length rule have an operator (==, !=, <=, >=, <, >) followed by its length. Example if we want
-        to have passwords that have at least one lowercase, at least one upper case, at least one special
-        character and its length is at least 10 characters long ``policy 'aA@>=10'``. Do not forget
-        to quote your arguments.
-        
-        ![policy_cmd](https://raw.githubusercontent.com/nazime/wordlistools/master/images/policy_cmd.png)
-        
-        ## Add a tool
-        
-        You can easily add your own tools in wordlistools. Create a python file in ``~/koalak/wordlistools/plugins/`` and subclass ``BasePlugin``, wordlistools will automatically execute your script and register your plugin.
-        
-        You have to define the following attributes
-        
-        - name(str): the name of your plugin (must be unique)
-        - description(str): description of what your will plugin do, it will be displayed in the help CLI
-        
-        Implement the following abstract methods:
-        
-        - ``init_parser()``: to configure the CLI arguments by using the standard library argparse, use ``self.add_argument`` which is a wrapper for the original argparse method.
-        - run: implement here the logic of your plugin, take any things as parameters and must return an iterator of strings
-        - cmd(args): must call the ``self.run`` method based on the ``args`` arguments of argparse
-        
-        Plugin Template
-        
-        ```python
-        # path of this file: ~/koalak/wordlistools/plugins/myplugins.py
-        import itertools
-        from wordlistools import BaseTool
-        
-        
-        class MyTool(BaseTool):
-            name = "myplugin"
-            description = "Do nothing, return the same list"
-        
-            def init_parser(self):
-                self.add_argument("wordlists", help="wordlist to return", nargs="+", stdin=True)
-        
-            def cmd(cls, args):
-                return cls.run(*args.wordlists)
-        
-            def run(cls, *wordlists):
-                wordlists = cls.normalize_wordlists(wordlists)
-                for e in itertools.chain(*wordlists):
-                    yield e
-        ```
-        
-        If you want your plugins to handle stdin wordlists you have to add ``stdin=True`` in ``add_argument``.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: tests
+Provides-Extra: dev
 Provides-Extra: travis
+License-File: LICENSE
+
+# wordlistools
+Wordlistools is a collection of tools to play with wordlists. This tool was built with offensive security in mind,
+to help bruteforcing, filtering wordlists to crack passwords, building
+wordlists for fuzzing, etc.
+This project is still under development.
+
+**Features**
+
+- Can be used as command lines or as a python library
+- Can be used with stdin redirection ``|``
+- Easily extensible, you can add your own plugins on your home directory ```~/.koalak/wordlistools/plugins```
+
+
+![wordlistools demo](https://raw.githubusercontent.com/nazime/wordlistools/master/images/help_v0.1.3.png)
+
+
+## Install
+
+```bash
+pip3 install wordlistools
+```
+
+## Demonstration
+Note: This demonstration is an old version of wordlistools,
+but the principe remains the same.
+[![wordlistools demo](https://raw.githubusercontent.com/nazime/wordlistools/master/images/wordlistools.gif)](https://asciinema.org/a/430731)
+
+
+## Using policy subcommand
+You can filter your wordlist based on a policy, the policy follow the following format ``[base_policy][lenght_policy]``.
+The base policy can have the following rules:
+- a: word must contain at least one lower case letter
+- A: word must contain at least one upper case letter
+- 1: word must contain at least one digit
+- @: word must contain at least one special character
+
+length rule have an operator (==, !=, <=, >=, <, >) followed by its length. Example if we want
+to have passwords that have at least one lowercase, at least one upper case, at least one special
+character and its length is at least 10 characters long ``policy 'aA@>=10'``. Do not forget
+to quote your arguments.
+
+![policy_cmd](https://raw.githubusercontent.com/nazime/wordlistools/master/images/policy_cmd.png)
+
+## Add a tool
+
+You can easily add your own tools in wordlistools. Create a python file in ``~/koalak/wordlistools/plugins/`` and subclass ``BasePlugin``, wordlistools will automatically execute your script and register your plugin.
+
+You have to define the following attributes
+
+- name(str): the name of your plugin (must be unique)
+- description(str): description of what your will plugin do, it will be displayed in the help CLI
+
+Implement the following abstract methods:
+
+- ``init_parser()``: to configure the CLI arguments by using the standard library argparse, use ``self.add_argument`` which is a wrapper for the original argparse method.
+- run: implement here the logic of your plugin, take any things as parameters and must return an iterator of strings
+- cmd(args): must call the ``self.run`` method based on the ``args`` arguments of argparse
+
+Plugin Template
+
+```python
+# path of this file: ~/koalak/wordlistools/plugins/myplugins.py
+import itertools
+from wordlistools import BaseTool
+
+
+class MyTool(BaseTool):
+    name = "myplugin"
+    description = "Do nothing, return the same list"
+
+    def init_parser(self):
+        self.add_argument("wordlists", help="wordlist to return", nargs="+", stdin=True)
+
+    def cmd(cls, args):
+        return cls.run(*args.wordlists)
+
+    def run(cls, *wordlists):
+        wordlists = cls.normalize_wordlists(wordlists)
+        for e in itertools.chain(*wordlists):
+            yield e
+```
+
+If you want your plugins to handle stdin wordlists you have to add ``stdin=True`` in ``add_argument``.
```

### Comparing `wordlistools-0.1.8/README.md` & `wordlistools-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `wordlistools-0.1.8/setup.py` & `wordlistools-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
 ]
 
 # Packages information
 PACKAGES = find_packages(where="src")
 PACKAGE_DIR = {"": "src"}
-INSTALL_REQUIRES = ["argcomplete", "colorama", "koalak>=0.2.10"]
+INSTALL_REQUIRES = ["argcomplete", "colorama", "koalak>=0.2.15"]
 EXTRAS_REQUIRE = {
     "docs": ["sphinx"],
     "tests": [
         "coverage",
         "hypothesis",
         "pytest>=4.3.0",  # 4.3.0 dropped last use of `convert`
     ],
```

### Comparing `wordlistools-0.1.8/src/wordlistools/api.py` & `wordlistools-0.1.9/src/wordlistools/api.py`

 * *Files identical despite different names*

### Comparing `wordlistools-0.1.8/src/wordlistools/base.py` & `wordlistools-0.1.9/src/wordlistools/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 # Create the wordlistools framework with koalak
 wordlistools = koalak.mkframework("wordlistools")
 tools = wordlistools.mkpluginmanager("tools")
 
 
 @tools.mkbaseplugin
 class BaseTool:
-    description = tools.attr(type=str)
-    name = tools.attr(type=str)
-    group = "basic"
+    description: str = tools.field()
+    name: str = tools.field()
+    group: str = "basic"
     nb_outputs = 1
 
     def __init__(self):
         # Toos can have zero or one stdin argument
         # stdin argument are arguments (related to wordlists) that
         # can take their arguments from files or wordlist
         # => That means that, if stdin is not empty (when using pip "|" for example)
```

### Comparing `wordlistools-0.1.8/src/wordlistools/helpertest.py` & `wordlistools-0.1.9/src/wordlistools/helpertest.py`

 * *Files identical despite different names*

### Comparing `wordlistools-0.1.8/src/wordlistools/plugins/filters_tools.py` & `wordlistools-0.1.9/src/wordlistools/plugins/filters_tools.py`

 * *Files identical despite different names*

### Comparing `wordlistools-0.1.8/src/wordlistools/plugins/modifiers_tools.py` & `wordlistools-0.1.9/src/wordlistools/plugins/modifiers_tools.py`

 * *Files identical despite different names*

### Comparing `wordlistools-0.1.8/src/wordlistools/plugins/plugins.py` & `wordlistools-0.1.9/src/wordlistools/plugins/plugins.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     # TODO: each type tool will have it's own subparser
 
     def init_parser(self):
         # FIXME: in koalak   add function to get names of plugins!
         self.add_argument(
             "type",
             help="Type of output to parse",
-            choices=list(parsers._plugins.keys()),
+            # choices=list(parsers._plugins.keys()),
         )
         #
         self.add_argument("input", help="input to parse", stdin=True)
 
     def cmd(self, args):
         return self.run(args.type, args.input)
```

### Comparing `wordlistools-0.1.8/src/wordlistools/plugins/statistics_tools.py` & `wordlistools-0.1.9/src/wordlistools/plugins/statistics_tools.py`

 * *Files identical despite different names*

### Comparing `wordlistools-0.1.8/src/wordlistools.egg-info/PKG-INFO` & `wordlistools-0.1.9/src/wordlistools.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,112 +1,112 @@
 Metadata-Version: 2.1
 Name: wordlistools
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tools to play with wordlists
 Home-page: https://github.com/nazime/wordlistools
 Author: Nazime LAKEHAL
 Author-email: nazime.lkh@gmail.com
 Maintainer: Nazime LAKEHAL
 Maintainer-email: nazime.lkh@gmail.com
 License: MIT
 Project-URL: Documentation, https://wordlistools.readthedocs.org/
 Project-URL: Bug Tracker, https://github.com/nazime/wordlistools/issues
 Project-URL: Source Code, https://github.com/nazime/wordlistools
-Description: # wordlistools
-        Wordlistools is a collection of tools to play with wordlists. This tool was built with offensive security in mind,
-        to help bruteforcing, filtering wordlists to crack passwords, building
-        wordlists for fuzzing, etc.
-        This project is still under development.
-        
-        **Features**
-        
-        - Can be used as command lines or as a python library
-        - Can be used with stdin redirection ``|``
-        - Easily extensible, you can add your own plugins on your home directory ```~/.koalak/wordlistools/plugins```
-        
-        
-        ![wordlistools demo](https://raw.githubusercontent.com/nazime/wordlistools/master/images/help_v0.1.3.png)
-        
-        
-        ## Install
-        
-        ```bash
-        pip3 install wordlistools
-        ```
-        
-        ## Demonstration
-        Note: This demonstration is an old version of wordlistools,
-        but the principe remains the same.
-        [![wordlistools demo](https://raw.githubusercontent.com/nazime/wordlistools/master/images/wordlistools.gif)](https://asciinema.org/a/430731)
-        
-        
-        ## Using policy subcommand
-        You can filter your wordlist based on a policy, the policy follow the following format ``[base_policy][lenght_policy]``.
-        The base policy can have the following rules:
-        - a: word must contain at least one lower case letter
-        - A: word must contain at least one upper case letter
-        - 1: word must contain at least one digit
-        - @: word must contain at least one special character
-        
-        length rule have an operator (==, !=, <=, >=, <, >) followed by its length. Example if we want
-        to have passwords that have at least one lowercase, at least one upper case, at least one special
-        character and its length is at least 10 characters long ``policy 'aA@>=10'``. Do not forget
-        to quote your arguments.
-        
-        ![policy_cmd](https://raw.githubusercontent.com/nazime/wordlistools/master/images/policy_cmd.png)
-        
-        ## Add a tool
-        
-        You can easily add your own tools in wordlistools. Create a python file in ``~/koalak/wordlistools/plugins/`` and subclass ``BasePlugin``, wordlistools will automatically execute your script and register your plugin.
-        
-        You have to define the following attributes
-        
-        - name(str): the name of your plugin (must be unique)
-        - description(str): description of what your will plugin do, it will be displayed in the help CLI
-        
-        Implement the following abstract methods:
-        
-        - ``init_parser()``: to configure the CLI arguments by using the standard library argparse, use ``self.add_argument`` which is a wrapper for the original argparse method.
-        - run: implement here the logic of your plugin, take any things as parameters and must return an iterator of strings
-        - cmd(args): must call the ``self.run`` method based on the ``args`` arguments of argparse
-        
-        Plugin Template
-        
-        ```python
-        # path of this file: ~/koalak/wordlistools/plugins/myplugins.py
-        import itertools
-        from wordlistools import BaseTool
-        
-        
-        class MyTool(BaseTool):
-            name = "myplugin"
-            description = "Do nothing, return the same list"
-        
-            def init_parser(self):
-                self.add_argument("wordlists", help="wordlist to return", nargs="+", stdin=True)
-        
-            def cmd(cls, args):
-                return cls.run(*args.wordlists)
-        
-            def run(cls, *wordlists):
-                wordlists = cls.normalize_wordlists(wordlists)
-                for e in itertools.chain(*wordlists):
-                    yield e
-        ```
-        
-        If you want your plugins to handle stdin wordlists you have to add ``stdin=True`` in ``add_argument``.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: tests
+Provides-Extra: dev
 Provides-Extra: travis
+License-File: LICENSE
+
+# wordlistools
+Wordlistools is a collection of tools to play with wordlists. This tool was built with offensive security in mind,
+to help bruteforcing, filtering wordlists to crack passwords, building
+wordlists for fuzzing, etc.
+This project is still under development.
+
+**Features**
+
+- Can be used as command lines or as a python library
+- Can be used with stdin redirection ``|``
+- Easily extensible, you can add your own plugins on your home directory ```~/.koalak/wordlistools/plugins```
+
+
+![wordlistools demo](https://raw.githubusercontent.com/nazime/wordlistools/master/images/help_v0.1.3.png)
+
+
+## Install
+
+```bash
+pip3 install wordlistools
+```
+
+## Demonstration
+Note: This demonstration is an old version of wordlistools,
+but the principe remains the same.
+[![wordlistools demo](https://raw.githubusercontent.com/nazime/wordlistools/master/images/wordlistools.gif)](https://asciinema.org/a/430731)
+
+
+## Using policy subcommand
+You can filter your wordlist based on a policy, the policy follow the following format ``[base_policy][lenght_policy]``.
+The base policy can have the following rules:
+- a: word must contain at least one lower case letter
+- A: word must contain at least one upper case letter
+- 1: word must contain at least one digit
+- @: word must contain at least one special character
+
+length rule have an operator (==, !=, <=, >=, <, >) followed by its length. Example if we want
+to have passwords that have at least one lowercase, at least one upper case, at least one special
+character and its length is at least 10 characters long ``policy 'aA@>=10'``. Do not forget
+to quote your arguments.
+
+![policy_cmd](https://raw.githubusercontent.com/nazime/wordlistools/master/images/policy_cmd.png)
+
+## Add a tool
+
+You can easily add your own tools in wordlistools. Create a python file in ``~/koalak/wordlistools/plugins/`` and subclass ``BasePlugin``, wordlistools will automatically execute your script and register your plugin.
+
+You have to define the following attributes
+
+- name(str): the name of your plugin (must be unique)
+- description(str): description of what your will plugin do, it will be displayed in the help CLI
+
+Implement the following abstract methods:
+
+- ``init_parser()``: to configure the CLI arguments by using the standard library argparse, use ``self.add_argument`` which is a wrapper for the original argparse method.
+- run: implement here the logic of your plugin, take any things as parameters and must return an iterator of strings
+- cmd(args): must call the ``self.run`` method based on the ``args`` arguments of argparse
+
+Plugin Template
+
+```python
+# path of this file: ~/koalak/wordlistools/plugins/myplugins.py
+import itertools
+from wordlistools import BaseTool
+
+
+class MyTool(BaseTool):
+    name = "myplugin"
+    description = "Do nothing, return the same list"
+
+    def init_parser(self):
+        self.add_argument("wordlists", help="wordlist to return", nargs="+", stdin=True)
+
+    def cmd(cls, args):
+        return cls.run(*args.wordlists)
+
+    def run(cls, *wordlists):
+        wordlists = cls.normalize_wordlists(wordlists)
+        for e in itertools.chain(*wordlists):
+            yield e
+```
+
+If you want your plugins to handle stdin wordlists you have to add ``stdin=True`` in ``add_argument``.
```

### Comparing `wordlistools-0.1.8/src/wordlistools.egg-info/SOURCES.txt` & `wordlistools-0.1.9/src/wordlistools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

