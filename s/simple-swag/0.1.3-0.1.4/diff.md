# Comparing `tmp/simple-swag-0.1.3.tar.gz` & `tmp/simple-swag-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-swag-0.1.3.tar", last modified: Mon Jul 17 09:56:08 2023, max compression
+gzip compressed data, was "simple-swag-0.1.4.tar", last modified: Sat Jul 29 15:09:35 2023, max compression
```

## Comparing `simple-swag-0.1.3.tar` & `simple-swag-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 peterprescott  (1000) peterprescott  (1000)        0 2023-07-17 09:56:08.322653 simple-swag-0.1.3/
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)      845 2023-07-17 09:56:08.322653 simple-swag-0.1.3/PKG-INFO
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)      489 2023-07-14 08:55:13.000000 simple-swag-0.1.3/README.md
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)      104 2023-07-11 17:11:37.000000 simple-swag-0.1.3/pyproject.toml
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)      679 2023-07-17 09:56:08.322653 simple-swag-0.1.3/setup.cfg
-drwxr-xr-x   0 peterprescott  (1000) peterprescott  (1000)        0 2023-07-17 09:56:08.318653 simple-swag-0.1.3/src/
-drwxr-xr-x   0 peterprescott  (1000) peterprescott  (1000)        0 2023-07-17 09:56:08.318653 simple-swag-0.1.3/src/simple_swag.egg-info/
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)      845 2023-07-17 09:56:08.000000 simple-swag-0.1.3/src/simple_swag.egg-info/PKG-INFO
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)      406 2023-07-17 09:56:08.000000 simple-swag-0.1.3/src/simple_swag.egg-info/SOURCES.txt
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)        1 2023-07-17 09:56:08.000000 simple-swag-0.1.3/src/simple_swag.egg-info/dependency_links.txt
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)       39 2023-07-17 09:56:08.000000 simple-swag-0.1.3/src/simple_swag.egg-info/entry_points.txt
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)       67 2023-07-17 09:56:08.000000 simple-swag-0.1.3/src/simple_swag.egg-info/requires.txt
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)        5 2023-07-17 09:56:08.000000 simple-swag-0.1.3/src/simple_swag.egg-info/top_level.txt
-drwxr-xr-x   0 peterprescott  (1000) peterprescott  (1000)        0 2023-07-17 09:56:08.322653 simple-swag-0.1.3/src/swag/
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)        0 2023-07-15 16:44:08.000000 simple-swag-0.1.3/src/swag/__init__.py
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)     2380 2023-07-15 18:50:02.000000 simple-swag-0.1.3/src/swag/autoblog.py
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)     5643 2023-07-17 09:12:33.000000 simple-swag-0.1.3/src/swag/builder.py
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)     2288 2023-07-17 09:12:47.000000 simple-swag-0.1.3/src/swag/cli.py
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)     1093 2023-07-15 17:02:53.000000 simple-swag-0.1.3/src/swag/lorem.py
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)     4689 2023-07-15 17:01:11.000000 simple-swag-0.1.3/src/swag/resources.py
-drwxr-xr-x   0 peterprescott  (1000) peterprescott  (1000)        0 2023-07-17 09:56:08.322653 simple-swag-0.1.3/tests/
--rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)      198 2023-07-14 09:25:30.000000 simple-swag-0.1.3/tests/test_cli.py
+drwxr-xr-x   0 peterprescott  (1000) peterprescott  (1000)        0 2023-07-29 15:09:35.940156 simple-swag-0.1.4/
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)      845 2023-07-29 15:09:35.940156 simple-swag-0.1.4/PKG-INFO
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)      489 2023-07-14 08:55:13.000000 simple-swag-0.1.4/README.md
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)      104 2023-07-11 17:11:37.000000 simple-swag-0.1.4/pyproject.toml
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)      700 2023-07-29 15:09:35.940156 simple-swag-0.1.4/setup.cfg
+drwxr-xr-x   0 peterprescott  (1000) peterprescott  (1000)        0 2023-07-29 15:09:35.940156 simple-swag-0.1.4/src/
+drwxr-xr-x   0 peterprescott  (1000) peterprescott  (1000)        0 2023-07-29 15:09:35.940156 simple-swag-0.1.4/src/simple_swag.egg-info/
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)      845 2023-07-29 15:09:35.000000 simple-swag-0.1.4/src/simple_swag.egg-info/PKG-INFO
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)      406 2023-07-29 15:09:35.000000 simple-swag-0.1.4/src/simple_swag.egg-info/SOURCES.txt
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)        1 2023-07-29 15:09:35.000000 simple-swag-0.1.4/src/simple_swag.egg-info/dependency_links.txt
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)       39 2023-07-29 15:09:35.000000 simple-swag-0.1.4/src/simple_swag.egg-info/entry_points.txt
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)       86 2023-07-29 15:09:35.000000 simple-swag-0.1.4/src/simple_swag.egg-info/requires.txt
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)        5 2023-07-29 15:09:35.000000 simple-swag-0.1.4/src/simple_swag.egg-info/top_level.txt
+drwxr-xr-x   0 peterprescott  (1000) peterprescott  (1000)        0 2023-07-29 15:09:35.940156 simple-swag-0.1.4/src/swag/
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)        0 2023-07-15 16:44:08.000000 simple-swag-0.1.4/src/swag/__init__.py
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)     2680 2023-07-17 23:37:02.000000 simple-swag-0.1.4/src/swag/autoblog.py
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)     5786 2023-07-29 14:26:18.000000 simple-swag-0.1.4/src/swag/builder.py
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)     2774 2023-07-27 11:56:40.000000 simple-swag-0.1.4/src/swag/cli.py
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)     1093 2023-07-15 17:02:53.000000 simple-swag-0.1.4/src/swag/lorem.py
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)     4689 2023-07-15 17:01:11.000000 simple-swag-0.1.4/src/swag/resources.py
+drwxr-xr-x   0 peterprescott  (1000) peterprescott  (1000)        0 2023-07-29 15:09:35.940156 simple-swag-0.1.4/tests/
+-rw-r--r--   0 peterprescott  (1000) peterprescott  (1000)      198 2023-07-14 09:25:30.000000 simple-swag-0.1.4/tests/test_cli.py
```

### Comparing `simple-swag-0.1.3/PKG-INFO` & `simple-swag-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-swag
-Version: 0.1.3
+Version: 0.1.4
 Summary: "Simple Website Auto Generator"
 Home-page: https://github.com/peterprescott/simple-swag
 Author: Peter Prescott
 Author-email: prescott.peter@gmail.com
 Project-URL: Bug Tracker, https://github.com/peterprescott/simple-swag/issues
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `simple-swag-0.1.3/setup.cfg` & `simple-swag-0.1.4/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = simple-swag
-version = 0.1.3
+version = 0.1.4
 author = Peter Prescott
 author_email = prescott.peter@gmail.com
 description = "Simple Website Auto Generator"
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/peterprescott/simple-swag
 project_urls = 
@@ -18,14 +18,16 @@
 install_requires = 
 	fire
 	lorem
 	markdown
 	markdown-full-yaml-metadata
 	multiavatar
 	pandas
+	Pygments
+	unidecode
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	swag = swag.cli:main
```

### Comparing `simple-swag-0.1.3/src/simple_swag.egg-info/PKG-INFO` & `simple-swag-0.1.4/src/simple_swag.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-swag
-Version: 0.1.3
+Version: 0.1.4
 Summary: "Simple Website Auto Generator"
 Home-page: https://github.com/peterprescott/simple-swag
 Author: Peter Prescott
 Author-email: prescott.peter@gmail.com
 Project-URL: Bug Tracker, https://github.com/peterprescott/simple-swag/issues
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `simple-swag-0.1.3/src/swag/autoblog.py` & `simple-swag-0.1.4/src/swag/autoblog.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import os
 from pathlib import Path
 
 import openai
+from dotenv import dotenv_values
 
 import swag.builder
 
 print('hello world')
 
-with open(Path(os.getcwd()) / '../try-llm/secret.key', 'r') as f:
-    key = f.read().replace('\n', '')
-
-openai.api_key = key
 
 class ChatBot:
-    def __init__(self, engine="text-davinci-003", max_tokens=500):
+    def __init__(self, engine="text-davinci-003", max_tokens=500,
+                 config=None):
         self.engine = engine
         self.max_tokens = max_tokens
         self.prompts = []
         self._responses = []
         self.replies = []
+        if config is None:
+            self.config = dotenv_values(swag.builder.get_project_root()
+                                        / '.env')
+        else:
+            self.config = config
+        openai.api_key = self.config['OPENAIKEY']
+
 
     def say(self, something):
         self.prompts.append(something)
         self._responses.append(
                 response := openai.Completion.create(
                     engine=self.engine,
                     prompt=something,
@@ -61,32 +66,35 @@
                     self.write_post_about(idea))
         print(self.posts[idea])
 
     def save_posts(self, save_dir):
         pass
 
 def autoblog(subject='whatever'):
-    root = builder.get_project_root()
     blogger = AutoBlogger(subject=subject)
 
     blogger.get_ideas()
 
     [blogger.write_post(idea) for idea in blogger.ideas if idea]
 
     for i, (idea, post) in enumerate(blogger.posts.items()):
-        markdown = f"""
----
-title: {idea}
+        markdown = f"""---
+title: "{idea.replace('"','')}"
 date: 15/07/2023
 ---
 
 {post}
         """
-        with open(root / 'content' / 'auto' / f'{str(i).zfill(3)}.md',
+        auto_folder = swag.builder.get_project_root() / 'content' / 'auto'
+        if not os.path.exists(auto_folder):
+            os.mkdir(auto_folder)
+        with open(auto_folder / f'{str(i).zfill(3)}.md',
                   'w') as f:
             f.write(markdown)
 
 
     return blogger
 
 
-autoblog('Mastering the Linux Command Line')
+
+def main(subject):
+    autoblog(subject)
```

### Comparing `simple-swag-0.1.3/src/swag/builder.py` & `simple-swag-0.1.4/src/swag/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import os
 from pathlib import Path
 import shutil
 from functools import cached_property
 
 import markdown
 import pandas as pd
+from unidecode import unidecode
 
-def get_project_root(max_depth=3):
+def get_project_root(max_depth=7):
     required = ('assets', 'content', 'templates', 'config.toml')
     found = False
     position = Path(os.getcwd())
     depth = 0
 
     while not found:
         if depth == max_depth:
@@ -41,30 +42,32 @@
             Relative filepath to {project_root} / 'content'
         ...
         """
         self._template = template
         self._content = content
         self._root = Path(get_project_root())
         self._md_interpreter = markdown.Markdown(
-                extensions=["full_yaml_metadata"])
+                extensions=["full_yaml_metadata", 'fenced_code',
+                'codehilite'])
         self.meta = {}
 
     def _load(self):
         self.load_raw_content()
         self.convert_raw_content()
 
 
     def load_template(self):
         with open(self._root / 'templates' / f'{self._template}.html') as f:
             self.template = f.read()
 
     def load_raw_content(self):
         if not self._content:
             return None
-        with open(self._root / 'content' / self._content) as f:
+        with open(self._root / 'content' / self._content,
+                    encoding='utf-8') as f:
             self.raw_content = f.read()
 
     def convert_raw_content(self):
         if '.md' in self._content.name:
             self.content = self._md_interpreter.convert(self.raw_content)
             self.meta = self._md_interpreter.Meta.copy()
             self._load_meta()
@@ -97,22 +100,22 @@
             name = self._content.name.replace('.md','.html') 
             filename = self._content.parent / name
         self.href = filename
         filepath = self._root / 'build' / filename
         
         while os.path.exists(filepath):
             filepath = filepath.parent / ('_' + filepath.name)
-        with open(filepath, 'w') as f:
-                  f.write(self.html)
+        with open(filepath, 'w', encoding='ascii') as f:
+                  f.write(unidecode(self.html))
 
     def get_summary(self):
         name = self._content.name.replace('.md',
                                                                  '.html')
         title = f'<h1><a href="{name}">{self.meta["title"]}</a></h1>'
-        date = f'<p>{self.meta["date"]}</p>' if hasattr(self, 'date') else ''
+        date = f'<p>{self.date.date()}</p>' if hasattr(self, 'date') else ''
         return f'{title}{date}'
 
 
 class Builder:
     def __init__(self):
         self.root = get_project_root()
         self._templates = {}
```

### Comparing `simple-swag-0.1.3/src/swag/cli.py` & `simple-swag-0.1.4/src/swag/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import fire
 from multiavatar.multiavatar import multiavatar
 
 import swag.lorem
 import swag.resources
 import swag.builder
+# import swag.autoblog
 
 
 
 def hello(name="World"):
     return f"Hello {name}!"
 
 
@@ -48,17 +49,27 @@
 
 def build():
     root = swag.builder.get_project_root()
     swag.builder.main()
 
 def serve(port = 8000, address="localhost", max_tries=3):
     root = swag.builder.get_project_root()
+    if '404.html' in os.listdir(root / 'build'):
+        path_404 = '404.html'
+    else:
+        path_404 = 'index.html'
+    with open(root / 'build' / path_404) as f:
+        page_404 = f.read()
     class Handler(SimpleHTTPRequestHandler):
         def __init__(self, *args, **kwargs):
-            super().__init__(directory=root / 'build', *args, **kwargs)
+            super().__init__(directory=str(root / 'build'), *args, **kwargs)
+        def send_error(self, code, message=None):
+            if code==404:
+                self.error_message_format = page_404 
+            SimpleHTTPRequestHandler.send_error(self, code, message)
 
     i = 0
     while i < max_tries:
         try:
             server = HTTPServer((address, port), Handler)
             print(f'\nSWAG is serving your site at https://{address}:{port}')
             server.serve_forever()
@@ -66,12 +77,15 @@
             print(f'\nPort {port} is busy...')
             port += 1
             i += 1
 
     if i == max_tries:
         print(f'Reached attempt limit of {max_tries}, try starting with a different port')
 
+# def autoblogger(subject):
+#     swag.autoblog.main(subject)
+
 
 
 
 def main():
     fire.Fire()
```

### Comparing `simple-swag-0.1.3/src/swag/lorem.py` & `simple-swag-0.1.4/src/swag/lorem.py`

 * *Files identical despite different names*

### Comparing `simple-swag-0.1.3/src/swag/resources.py` & `simple-swag-0.1.4/src/swag/resources.py`

 * *Files identical despite different names*

