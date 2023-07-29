# Comparing `tmp/pandora_client-0.3.21.tar.gz` & `tmp/pandora_client-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandora_client-0.3.21.tar", last modified: Sat Jul 29 09:21:12 2023, max compression
+gzip compressed data, was "dist/pandora_client-0.3.6.tar", last modified: Sat Dec 21 17:34:56 2019, max compression
```

## Comparing `pandora_client-0.3.21.tar` & `pandora_client-0.3.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2023-07-29 09:21:12.190423 pandora_client-0.3.21/
--rw-r--r--   0 j         (1000) j         (1000)      603 2023-07-29 09:21:12.190423 pandora_client-0.3.21/PKG-INFO
--rw-r--r--   0 j         (1000) j         (1000)     2012 2019-12-21 18:34:41.000000 pandora_client-0.3.21/README.md
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2023-07-29 09:21:12.186423 pandora_client-0.3.21/bin/
--rwxr-xr-x   0 j         (1000) j         (1000)     2823 2023-07-28 16:29:12.000000 pandora_client-0.3.21/bin/pandora_client
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2023-07-29 09:21:12.190423 pandora_client-0.3.21/pandora_client/
--rwxr-xr-x   0 j         (1000) j         (1000)    45828 2023-07-29 08:15:06.000000 pandora_client-0.3.21/pandora_client/__init__.py
--rw-r--r--   0 j         (1000) j         (1000)     4346 2023-07-28 16:29:24.000000 pandora_client-0.3.21/pandora_client/client.py
--rw-r--r--   0 j         (1000) j         (1000)    10573 2023-07-29 09:04:59.000000 pandora_client-0.3.21/pandora_client/extract.py
--rw-r--r--   0 j         (1000) j         (1000)     3688 2017-07-01 14:49:54.000000 pandora_client-0.3.21/pandora_client/localnode.py
--rw-r--r--   0 j         (1000) j         (1000)     8399 2023-07-28 16:29:31.000000 pandora_client-0.3.21/pandora_client/server.py
--rw-r--r--   0 j         (1000) j         (1000)     3032 2023-07-28 16:29:35.000000 pandora_client-0.3.21/pandora_client/utils.py
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2023-07-29 09:21:12.190423 pandora_client-0.3.21/pandora_client.egg-info/
--rw-rw-r--   0 j         (1000) j         (1000)      603 2023-07-29 09:21:12.000000 pandora_client-0.3.21/pandora_client.egg-info/PKG-INFO
--rw-rw-r--   0 j         (1000) j         (1000)      414 2023-07-29 09:21:12.000000 pandora_client-0.3.21/pandora_client.egg-info/SOURCES.txt
--rw-rw-r--   0 j         (1000) j         (1000)        1 2023-07-29 09:21:12.000000 pandora_client-0.3.21/pandora_client.egg-info/dependency_links.txt
--rw-r--r--   0 j         (1000) j         (1000)       47 2015-09-29 13:38:05.000000 pandora_client-0.3.21/pandora_client.egg-info/pbr.json
--rw-rw-r--   0 j         (1000) j         (1000)       45 2023-07-29 09:21:12.000000 pandora_client-0.3.21/pandora_client.egg-info/requires.txt
--rw-rw-r--   0 j         (1000) j         (1000)       15 2023-07-29 09:21:12.000000 pandora_client-0.3.21/pandora_client.egg-info/top_level.txt
--rw-r--r--   0 j         (1000) j         (1000)       38 2023-07-29 09:21:12.190423 pandora_client-0.3.21/setup.cfg
--rw-r--r--   0 j         (1000) j         (1000)     1704 2023-07-29 09:21:11.000000 pandora_client-0.3.21/setup.py
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2019-12-21 17:34:56.000000 pandora_client-0.3.6/
+-rw-r--r--   0 j         (1000) j         (1000)      633 2019-12-21 17:34:56.000000 pandora_client-0.3.6/PKG-INFO
+-rw-r--r--   0 j         (1000) j         (1000)     1494 2018-04-03 08:27:32.000000 pandora_client-0.3.6/README.md
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2019-12-21 17:34:56.000000 pandora_client-0.3.6/bin/
+-rwxr-xr-x   0 j         (1000) j         (1000)     2854 2017-06-07 07:20:35.000000 pandora_client-0.3.6/bin/pandora_client
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2019-12-21 17:34:56.000000 pandora_client-0.3.6/pandora_client/
+-rwxr-xr-x   0 j         (1000) j         (1000)    45873 2019-12-19 11:15:56.000000 pandora_client-0.3.6/pandora_client/__init__.py
+-rw-r--r--   0 j         (1000) j         (1000)     4342 2018-06-06 07:58:05.000000 pandora_client-0.3.6/pandora_client/client.py
+-rw-r--r--   0 j         (1000) j         (1000)    10633 2019-11-01 20:50:01.000000 pandora_client-0.3.6/pandora_client/extract.py
+-rw-r--r--   0 j         (1000) j         (1000)     3688 2017-07-01 14:49:54.000000 pandora_client-0.3.6/pandora_client/localnode.py
+-rw-r--r--   0 j         (1000) j         (1000)     8480 2018-02-28 16:12:50.000000 pandora_client-0.3.6/pandora_client/server.py
+-rw-r--r--   0 j         (1000) j         (1000)     3096 2017-06-01 07:59:42.000000 pandora_client-0.3.6/pandora_client/utils.py
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2019-12-21 17:34:56.000000 pandora_client-0.3.6/pandora_client.egg-info/
+-rw-rw-r--   0 j         (1000) j         (1000)      633 2019-12-21 17:34:56.000000 pandora_client-0.3.6/pandora_client.egg-info/PKG-INFO
+-rw-rw-r--   0 j         (1000) j         (1000)      414 2019-12-21 17:34:56.000000 pandora_client-0.3.6/pandora_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 j         (1000) j         (1000)        1 2019-12-21 17:34:56.000000 pandora_client-0.3.6/pandora_client.egg-info/dependency_links.txt
+-rw-r--r--   0 j         (1000) j         (1000)       47 2015-09-29 13:38:05.000000 pandora_client-0.3.6/pandora_client.egg-info/pbr.json
+-rw-rw-r--   0 j         (1000) j         (1000)       54 2019-12-21 17:34:56.000000 pandora_client-0.3.6/pandora_client.egg-info/requires.txt
+-rw-rw-r--   0 j         (1000) j         (1000)       15 2019-12-21 17:34:56.000000 pandora_client-0.3.6/pandora_client.egg-info/top_level.txt
+-rw-r--r--   0 j         (1000) j         (1000)       38 2019-12-21 17:34:56.000000 pandora_client-0.3.6/setup.cfg
+-rw-r--r--   0 j         (1000) j         (1000)     1715 2019-12-21 17:34:56.000000 pandora_client-0.3.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pandora_client-0.3.21/README.md` & `pandora_client-0.3.6/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,9 @@
 # pandora_client - python client and libary to access a pan.do/ra instances
 
-Documentation at: https://code.0x2620.org/0x2620/pandora_client/wiki
-
-## Installation
-
-### Linux
-
-- install dependencies
-
-        sudo apt install python3 python3-pip ffmpeg
-
-- install pandora_client
-
-        sudo pip3 install pandora_client
-
-
-### macOS
-
-- install brew (https://brew.sh/)
-- install dependencies
-
-        brew install python3
-        brew install libvpx libvorbis
-        brew install ffmpeg --with-libvpx --with-libvorbis --with-libopus
-
-- install pandora_client
-
-        pip3 install pandora_client
-
 
 ## pandora client example:
 
   import pandora_client
   #example config.json
   '''
   {
```

### Comparing `pandora_client-0.3.21/bin/pandora_client` & `pandora_client-0.3.6/bin/pandora_client`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 # vi:si:et:sw=4:sts=4:ts=4
 # GPL 2012
+from __future__ import print_function
 
 import os
 import sys
 from argparse import ArgumentParser
 
 
 import json
@@ -45,15 +46,15 @@
     config = ('config', 'add_volume')
     server = ('server', 'client')
     if not args or args[0] not in actions + config + server:
         parser.error('''you must specify a valid action.
 \t\tknown actions are: %s
 \t\tconfiguration:     config, add_volume
 \t\tdistributed encoding: server, client
-for more information visit https://code.0x2620.org/0x2620/pandora_client/wiki''' % ', '.join(actions))
+for more information visit https://wiki.0x2620.org/wiki/pandora_client''' % ', '.join(actions))
 
     action = args[0]
 
     offline = action in config or action == 'client' or \
         (action == 'extract' and len(args) == 2 and args[1] in ('offline', 'all'))
     if action == 'client':
         opts.config = {'url': '', 'cache': '~/.ox/client.sqlite', 'media-cache': '~/.ox/media'}
```

### Comparing `pandora_client-0.3.21/pandora_client/__init__.py` & `pandora_client-0.3.6/pandora_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 # vi:si:et:sw=4:sts=4:ts=4
 # GPL 2012-2016
+from __future__ import division, with_statement, print_function, absolute_import
 
 import getpass
 from glob import glob
-import importlib.util
+import imp
 import json
 import math
-import mimetypes
 import os
 import socket
 import sqlite3
 import sys
 import tempfile
 import time
 import pkg_resources
 
-from urllib.parse import urlparse
+from six.moves.urllib.parse import urlparse
+from six.moves import input
+from six import string_types
 
 import ox
 
 from . import extract
 from . import utils
 
 
@@ -141,15 +143,15 @@
     sys.stdout.write("\033[?25h")
     sys.stdout.flush()
 
 class Client(object):
     _configfile = None
 
     def __init__(self, config, offline=False):
-        if isinstance(config, str):
+        if isinstance(config, string_types):
             self._configfile = os.path.expanduser(config)
             with open(config) as f:
                 try:
                     self._config = json.load(f)
                 except ValueError:
                     print("Failed to parse config at", config)
                     sys.exit(1)
@@ -220,36 +222,27 @@
                 c.execute(i)
             conn.commit()
         conn.close()
 
     def load_plugins(self, base=os.path.join(utils.basedir(), 'client.d')):
         global parse_path, example_path, ignore_file, sync_extensions, encode
         base = os.path.expanduser(base)
-        if not os.path.exists(base):
-            return
-        for name in sorted(os.listdir(base)):
-            if not name.endswith('.py'):
-                continue
-            path = os.path.join(base, name)
-
-            module_name = os.path.basename(path).split('.')[0]
-            spec = importlib.util.spec_from_file_location(module_name, path)
-            module = importlib.util.module_from_spec(spec)
-            spec.loader.exec_module(module)
-
-            if hasattr(module, 'parse_path'):
-                parse_path = module.parse_path
-            if hasattr(module, 'example_path'):
-                example_path = module.example_path
-            if hasattr(module, 'ignore_file'):
-                ignore_file = module.ignore_file
-            if hasattr(module, 'sync_extensions'):
-                sync_extensions = module.sync_extensions
-            if hasattr(module, 'encode'):
-                encode = module.encode
+        for path in sorted(glob('%s%s*.py' % (base, os.sep))):
+            with open(path) as fp:
+                module = imp.load_source(os.path.basename(path).split('.')[0], base, fp)
+                if hasattr(module, 'parse_path'):
+                    parse_path = module.parse_path
+                if hasattr(module, 'example_path'):
+                    example_path = module.example_path
+                if hasattr(module, 'ignore_file'):
+                    ignore_file = module.ignore_file
+                if hasattr(module, 'sync_extensions'):
+                    sync_extensions = module.sync_extensions
+                if hasattr(module, 'encode'):
+                    encode = module.encode
 
     def _conn(self):
         db_conn = self._config['cache']
         if isinstance(db_conn, bytes):
             db_conn = db_conn.decode('utf-8')
         db_conn = os.path.expanduser(db_conn)
         if not os.path.exists(os.path.dirname(db_conn)):
@@ -473,14 +466,35 @@
         if password:
             self._config['password'] = password
         url = input('Pan.do/ra URL (i.e. https://pandora.local/api/): ')
         if url:
             self._config['url'] = url
         self.save_config()
         print("\nconfiguration updated.")
+        self.install_programs()
+
+    def install_programs(self, args=[]):
+        update = 'update' in args
+        # install required programs
+        if sys.platform == 'darwin':
+            osext = 'macosx'
+        elif sys.platform.startswith('win'):
+            osext = 'exe'
+        else:
+            osext = 'linux'
+        bindir = os.path.join(utils.basedir(), 'bin')
+        ox.makedirs(bindir)
+        for p in ('ffmpeg', 'ffmpeg2theora'):
+            path = os.path.join(bindir, p)
+            if sys.platform.startswith('win'):
+                p += '.exe'
+            if not os.path.exists(path) or update:
+                print("installing %s in %s" % (p, bindir))
+                ox.net.save_url('http://firefogg.org/bin/%s.%s' % (p, osext), path, True)
+                os.chmod(path, 0o755)
 
     def add_volume(self, args):
         usage = "Usage: %s add_volume name path" % sys.argv[0]
         if len(args) != 2:
             print(usage)
             sys.exit(1)
         name = args[0]
@@ -931,20 +945,20 @@
                     print("No unused files found in cache, run \"%s clean all\" to remove the entire cache" % sys.argv[0])
                 else:
                     utils.cleanup_tree(self.api.media_cache)
 
     def import_srt(self, args):
         '''
             import srt as annotations, usage:
-                pandora_client import_srt ITEMID layername /path/to/transcript.srt
+                pandora_client ITEMID layername /path/to/transcript.srt
             i.e. 
-                pandora_client ipmort_srt ABC transcripts /path/to/transcript.srt
+                pandora_client ABC transcripts /path/to/transcript.srt
         '''
         if not args:
-            print('Usage: pandora_client import_srt ABC transcripts /path/to/transcript.srt')
+            print('Usage: pandora_client ABC transcripts /path/to/transcript.srt')
             sys.exit(1)
         item = args[0]
         layer = args[1]
         filename = args[2]
         layers = [l['id'] for l in self.api.site['layers']]
         if layer not in layers:
             print("invalid layer name, choices are: ", ', '.join(layers))
@@ -1042,29 +1056,24 @@
                     time.sleep(interval)
                     t = self.getTaskStatus(task_id=r['data']['taskId'])
         return t
 
     def uploadFrames(self, i, data):
         # upload frames
         if self.site['media'].get('importFrames') and i['frames']:
-            form = {
-                'action': 'upload',
-                'id': i['oshash']
-            }
-            files = []
+            form = ox.MultiPartForm()
+            form.add_field('action', 'upload')
+            form.add_field('id', i['oshash'])
             for key in data:
-                form[key] = data[key]
+                form.add_field(key, data[key])
             for frame in i['frames']:
                 fname = os.path.basename(frame)
                 if os.path.exists(frame):
-                    mimetype = mimetypes.guess_type(frame)[0] or 'application/octet-stream'
-                    files.append(
-                        ('frame', (fname, open(frame, 'rb'), mimetype))
-                    )
-            r = self._json_request(self.url, form, files)
+                    form.add_file('frame', fname, open(frame, 'rb'))
+            r = self._json_request(self.url, form)
             return r
 
     def uploadVideo(self, filename, data, profile, info=None):
         i = encode(filename, self.media_cache, profile, info,
                    self.site['media'].get('importFrames'))
         if not i:
             print("failed")
@@ -1087,52 +1096,42 @@
             print("Failed")
             return False
         return True
 
     def uploadData(self, filename, oshash):
         if DEBUG:
             print('upload', filename)
-        form = {
-            'action': 'upload',
-            'id': str(oshash)
-        }
+        form = ox.MultiPartForm()
+        form.add_field('action', 'upload')
+        form.add_field('id', str(oshash))
         fname = os.path.basename(filename)
         if not isinstance(fname, bytes):
             fname = fname.encode('utf-8')
-        mimetype = mimetypes.guess_type(filename)[0] or 'application/octet-stream'
-        files = [
-            ('file', (fname, open(filename, 'rb'), mimetype))
-        ]
-        r = self._json_request(self.url, form, files)
+        form.add_file('file', fname, open(filename, 'rb'))
+        r = self._json_request(self.url, form)
         return r
 
     def upload_chunks(self, url, filename, data=None):
+        form = ox.MultiPartForm()
         resume = None
         if self._resume_file and os.path.exists(self._resume_file):
             with open(self._resume_file) as f:
                 try:
                     resume = json.load(f)
                 except:
                     resume = {}
             if resume.get('chunkUploadUrl') != url:
                 resume = None
         if resume:
             data = resume
         else:
-            data = None
-            while not data:
-                try:
-                    data = self._json_request(url, data)
-                except KeyboardInterrupt:
-                    print("\ninterrupted by user.")
-                    sys.exit(1)
-                except:
-                    print("failed to start upload, will try again in 5 seconds\r", end='')
-                    sys.stdout.flush()
-                    time.sleep(5)
+            for key in data:
+                form.add_field(key, data[key])
+            data = self._json_request(url, form)
+
         print(filename)
         hide_cursor()
 
         def full_url(path):
             if path.startswith('/'):
                 u = urlparse(url)
                 path = '%s://%s%s' % (u.scheme, u.netloc, path)
@@ -1149,38 +1148,35 @@
                 done = data['offset']
                 f.seek(done)
                 resume_offset = done
             else:
                 resume_offset = 0
             chunk = f.read(CHUNK_SIZE)
             fname = os.path.basename(filename)
-            mimetype = mimetypes.guess_type(filename)[0] or 'application/octet-stream'
             if not isinstance(fname, bytes):
                 fname = fname.encode('utf-8')
             while chunk:
                 elapsed = time.mktime(time.localtime()) - start
                 remaining = ""
                 if done:
                     r = math.ceil((elapsed / (done/(fsize-resume_offset)) - elapsed)/60) * 60 * 1000 
                     r = ox.format_duration(r, milliseconds=False, verbosity=2)
                     if r:
                         remaining = ", %s remaining" % r
                 msg = '%0.2f%% %s of %s done%s' % (
                     100 * done/fsize, ox.format_bytes(done), ox.format_bytes(fsize), remaining)
                 print(''.join([msg, ' ' * (80-len(msg)), '\r']), end='')
                 sys.stdout.flush()
-                form = {}
+                form = ox.MultiPartForm()
+                form.add_file('chunk', fname, chunk)
                 if len(chunk) < CHUNK_SIZE or f.tell() == fsize:
-                    form['done'] = '1'
-                form['offset'] = str(done)
-                files = [
-                    ('chunk', (fname, chunk, mimetype))
-                ]
+                    form.add_field('done', '1')
+                form.add_field('offset', str(done))
                 try:
-                    data = self._json_request(uploadUrl, form, files)
+                    data = self._json_request(uploadUrl, form)
                 except KeyboardInterrupt:
                     print("\ninterrupted by user.")
                     sys.exit(1)
                 except:
                     print("uploading chunk failed, will try again in 5 seconds\r", end='')
                     sys.stdout.flush()
                     if DEBUG:
```

### Comparing `pandora_client-0.3.21/pandora_client/client.py` & `pandora_client-0.3.6/pandora_client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # encoding: utf-8
 # vi:si:et:sw=4:sts=4:ts=4
+from __future__ import division, with_statement, print_function, absolute_import
 
 import json
 import os
 import socket
 import subprocess
 import sys
 import threading
@@ -35,16 +36,14 @@
 
 class DistributedClient:
 
     interrupted = False
 
     def __init__(self, url, name, threads):
         self.url = url
-        while self.url and self.url[-1] == '/':
-            self.url = self.url[:-1]
         self.name = name
         self.threads = threads
         self.supported_formats = extract.supported_formats()
 
     def ping(self, oshash):
         try:
             url = '%s/ping/%s/%s' % (self.url, oshash, self.name)
```

### Comparing `pandora_client-0.3.21/pandora_client/extract.py` & `pandora_client-0.3.6/pandora_client/extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 # vi:si:et:sw=4:sts=4:ts=4
 # GPL 2017
+from __future__ import division, print_function, absolute_import
 
 from glob import glob
 import os
-import re
 import shutil
 import subprocess
 import sys
 
 import ox
 
 from .utils import AspectRatio, run_command, basedir
@@ -45,22 +45,21 @@
     ffmpeg = command('ffmpeg')
     if ffmpeg is None:
         return None
     p = subprocess.Popen([ffmpeg, '-codecs'],
                          stdout=subprocess.PIPE, stderr=subprocess.PIPE, close_fds=True)
     stdout, stderr = p.communicate()
     stdout = stdout.decode('utf-8')
-    mp4 = 'libx264' in stdout and bool(re.compile('DEA.L. aac').findall(stdout))
     return {
         'ogg': 'libtheora' in stdout and 'libvorbis' in stdout,
         'webm': 'libvpx' in stdout and 'libvorbis' in stdout,
         'vp8': 'libvpx' in stdout and 'libvorbis' in stdout,
         'vp9': 'libvpx-vp9' in stdout and 'libopus' in stdout,
-        'mp4': mp4,
-        'h264': mp4,
+        'mp4': 'libx264' in stdout and 'DEA.L. aac' in stdout,
+        'h264': 'libx264' in stdout and 'DEA.L. aac' in stdout,
     }
 
 def video_cmd(video, target, profile, info):
 
     if not os.path.exists(target):
         ox.makedirs(os.path.dirname(target))
 
@@ -281,17 +280,17 @@
         pass1_post[-1] = '/dev/null'
         if format == 'webm':
             pass1_post = ['-speed', '4'] + pass1_post
             post = ['-speed', '1'] + post
         cmds.append(base + ['-an', '-pass', '1', '-passlogfile', '%s.log' % target]
                          + video_settings + pass1_post)
         cmds.append(base + ['-pass', '2', '-passlogfile', '%s.log' % target]
-                         + video_settings + audio_settings + post)
+                         + audio_settings + video_settings + post)
     else:
-        cmds.append(base + video_settings + audio_settings + post)
+        cmds.append(base + audio_settings + video_settings + post)
 
     if not support.get(format):
         if format == 'webm':
             print("ffmpeg is compiled without WebM support")
         elif format == 'mp4':
             print("ffmpeg is compiled without H.264 support")
         else:
```

### Comparing `pandora_client-0.3.21/pandora_client/localnode.py` & `pandora_client-0.3.6/pandora_client/localnode.py`

 * *Files identical despite different names*

### Comparing `pandora_client-0.3.21/pandora_client/server.py` & `pandora_client-0.3.6/pandora_client/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # encoding: utf-8
 # vi:si:et:sw=4:sts=4:ts=4
+from __future__ import division, with_statement, print_function, absolute_import
 
 import os
 import json
 import shutil
 import time
 try:
     import _thread as thread
```

### Comparing `pandora_client-0.3.21/pandora_client/utils.py` & `pandora_client-0.3.6/pandora_client/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 # vi:si:et:sw=4:sts=4:ts=4
 # GPL 2010
+from __future__ import division, with_statement, print_function
 
 import fractions
 import os
 import sys
 import subprocess
 import time
```

### Comparing `pandora_client-0.3.21/pandora_client.egg-info/PKG-INFO` & `pandora_client-0.3.6/pandora_client.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: pandora-client
-Version: 0.3.21
+Version: 0.3.6
 Summary: pandora_client is a commandline client for pan.do/ra. You can use it to import videos into a pan.do/ra system. It is currently known to work on Linux and Mac OS X.
-Home-page: https://code.0x2620.org/0x2620/pandora_client/wiki
+Home-page: http://wiki.0x2620.org/wiki/pandora_client
 Author: j
 Author-email: j@mailb.org
 License: GPLv3
+Description: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `pandora_client-0.3.21/setup.py` & `pandora_client-0.3.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 from setuptools import setup
 
 
 def get_version():
-    return 21 #import os
+    return 6 #import os
     import re
     import subprocess
     dot_git = os.path.join(os.path.dirname(__file__), '.git')
     changelog = os.path.join(os.path.dirname(__file__), 'debian/changelog')
     if os.path.exists(dot_git):
         cmd = ['git', 'rev-list', 'HEAD', '--count']
         p = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
@@ -26,24 +26,25 @@
 
 setup(
     name="pandora_client",
     version="0.3.%s" % get_version(),
     description="pandora_client is a commandline client for pan.do/ra. You can use it to import videos into a pan.do/ra system. It is currently known to work on Linux and Mac OS X.",
     author="j",
     author_email="j@mailb.org",
-    url="https://code.0x2620.org/0x2620/pandora_client/wiki",
+    url="http://wiki.0x2620.org/wiki/pandora_client",
     license="GPLv3",
     scripts=[
         'bin/pandora_client',
     ],
     packages=[
         'pandora_client'
     ],
     install_requires=[
-        'ox >= 3.0.0',
+        'ox >= 2.3.804,<3',
+        'six',
         'requests >= 1.1.0',
         'zeroconf',
         'netifaces',
     ],
     keywords=[],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
```

