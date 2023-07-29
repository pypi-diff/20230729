# Comparing `tmp/buckets-20230725.tar.gz` & `tmp/buckets-20230729.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buckets-20230725.tar", last modified: Tue Jul 25 09:38:38 2023, max compression
+gzip compressed data, was "buckets-20230729.tar", last modified: Sat Jul 29 16:44:21 2023, max compression
```

## Comparing `buckets-20230725.tar` & `buckets-20230729.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-25 09:38:38.414490 buckets-20230725/
--rw-rw-r--   0 pi        (1000) pi        (1000)     1211 2023-07-25 07:02:08.000000 buckets-20230725/LICENSE
--rw-rw-r--   0 pi        (1000) pi        (1000)      392 2023-07-25 09:38:38.410490 buckets-20230725/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)       90 2023-07-25 07:02:08.000000 buckets-20230725/README.md
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-25 09:38:38.402490 buckets-20230725/buckets/
--rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-07-25 07:03:12.000000 buckets-20230725/buckets/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      501 2023-07-25 07:03:12.000000 buckets-20230725/buckets/delete.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      532 2023-07-25 07:53:03.000000 buckets-20230725/buckets/get.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      517 2023-07-25 07:44:57.000000 buckets-20230725/buckets/put.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     8722 2023-07-25 07:52:41.000000 buckets-20230725/buckets/server.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-25 09:38:38.410490 buckets-20230725/buckets.egg-info/
--rw-rw-r--   0 pi        (1000) pi        (1000)      392 2023-07-25 09:38:37.000000 buckets-20230725/buckets.egg-info/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      236 2023-07-25 09:38:37.000000 buckets-20230725/buckets.egg-info/SOURCES.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-07-25 09:38:37.000000 buckets-20230725/buckets.egg-info/dependency_links.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        8 2023-07-25 09:38:37.000000 buckets-20230725/buckets.egg-info/top_level.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       38 2023-07-25 09:38:38.414490 buckets-20230725/setup.cfg
--rw-rw-r--   0 pi        (1000) pi        (1000)      533 2023-07-25 09:38:01.000000 buckets-20230725/setup.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-29 16:44:21.039913 buckets-20230729/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1211 2023-07-25 09:41:37.000000 buckets-20230729/LICENSE
+-rw-rw-r--   0 pi        (1000) pi        (1000)      392 2023-07-29 16:44:21.039913 buckets-20230729/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      167 2023-07-29 06:49:09.000000 buckets-20230729/README.md
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-29 16:44:21.035913 buckets-20230729/bin/
+-rwxrwxr-x   0 pi        (1000) pi        (1000)      413 2023-07-28 02:59:57.000000 buckets-20230729/bin/buckets-gen-cert
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-29 16:44:21.035913 buckets-20230729/buckets/
+-rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-07-25 09:41:37.000000 buckets-20230729/buckets/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1373 2023-07-29 03:59:44.000000 buckets-20230729/buckets/get.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1124 2023-07-29 15:16:13.000000 buckets-20230729/buckets/put.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    10716 2023-07-29 16:37:25.000000 buckets-20230729/buckets/server.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1033 2023-07-29 15:08:47.000000 buckets-20230729/buckets/token.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-29 16:44:21.039913 buckets-20230729/buckets.egg-info/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      392 2023-07-29 16:44:20.000000 buckets-20230729/buckets.egg-info/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      256 2023-07-29 16:44:20.000000 buckets-20230729/buckets.egg-info/SOURCES.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-07-29 16:44:20.000000 buckets-20230729/buckets.egg-info/dependency_links.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        8 2023-07-29 16:44:20.000000 buckets-20230729/buckets.egg-info/top_level.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       38 2023-07-29 16:44:21.039913 buckets-20230729/setup.cfg
+-rw-rw-r--   0 pi        (1000) pi        (1000)      571 2023-07-29 05:26:47.000000 buckets-20230729/setup.py
```

### Comparing `buckets-20230725/LICENSE` & `buckets-20230729/LICENSE`

 * *Files identical despite different names*

### Comparing `buckets-20230725/buckets/server.py` & `buckets-20230729/buckets/server.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 import os
+import sys
+import ssl
 import time
+import hmac
 import uuid
 import json
 import sanic
 import pickle
 import hashlib
 import sqlite3
 import asyncio
 import aiohttp
-import argparse
+import mimetypes
 
 APP = sanic.Sanic('kvlog')
 APP.config.KEEP_ALIVE_TIMEOUT = 300
 
+LEARNED_CACHE = dict()
+MAX_VERSION_CACHE = dict()
+
 
 class SQLite():
     def __init__(self, db):
         d = hashlib.sha256(db.encode()).hexdigest()
         self.path = os.path.join('db', d[0:3], d[3:6], d + '.sqlite3')
 
         if not os.path.isfile(self.path):
@@ -49,16 +55,16 @@
     def __exit__(self, exc_type, exc_value, exc_traceback):
         self.db.rollback()
         self.db.close()
 
 
 @APP.post('/<phase:str>/<db:str>/<key:str>/<version:int>/<proposal_seq:int>')
 async def paxos_server(request, phase, db, key, version, proposal_seq):
-    if ARGS.config['cluster_key'] != request.headers['x-cluster-key']:
-        raise sanic.exceptions.Unauthorized('INVALID_CLUSTER_KEY')
+    if request.transport.get_extra_info('peercert') is None:
+        raise sanic.exceptions.Unauthorized('INVALID_CERTIFICATE')
 
     with SQLite(db) as sql:
         sql('insert or ignore into paxos values(?,?,0,0,null)', key, version)
 
         _, _, promised_seq, accepted_seq, value = sql(
             'select * from paxos where key=? and version=?', key, version)[0]
 
@@ -81,182 +87,243 @@
                 proposal_seq, key, version)
             sql.commit()
 
             return response([accepted_seq, value])
 
         # Standard paxos protocol ACCEPT phase
         if 'accept' == phase and proposal_seq == promised_seq:
+            LEARNED_CACHE.pop((db, key), None)
+            MAX_VERSION_CACHE.pop((db, key), None)
+
             value = pickle.loads(request.body)
 
             sql('''update paxos
                    set accepted_seq=?, value=?
                    where key=? and version=?
                 ''', proposal_seq, value, key, version)
+            sql('delete from paxos where key=? and version < ?', key, version)
             sql.commit()
 
             return response('OK')
 
-        # Paxos protocol does not specify this phase.
-        # If a value for the key is accepted by a majority, it is learned.
+        # Paxos protocol does not include this phase.
         #
-        # Our paxos client, after a successful accept phase, runs another
-        # round to mark the row as final.
+        # If a value for the key is accepted by a majority, it is learned.
+        # Our paxos client, after a successful accept phase, asks participating
+        # nodes to mark the row as final.
         if 'learn' == phase and promised_seq == accepted_seq == proposal_seq:
             sql('''update paxos
                    set promised_seq=null, accepted_seq=null
                    where key=? and version=?
                 ''', key, version)
-            sql('delete from paxos where key=? and version < ?', key, version)
             sql.commit()
 
             return response('OK')
 
-    raise sanic.exceptions.BadRequest('INVALID_SEQ_OR_UNKNOWN')
+    raise sanic.exceptions.BadRequest('UNKNOWN')
 
 
-async def paxos_client(db, key, version, value):
+async def paxos_client(bucket, key, version, value):
     # paxos seq is an integer in the following format - YYYYmmddHHMMSS
     # This would increase monotonically. Even if same seq is generated by
     # more than one instances of paxos rounds, protocol handles it and rejects
     # the later round (as proposal_seq should be GREATER than the promised_seq)
     url = '{{}}/{}/{}/{}/{}'.format(
-        db, key, version, time.strftime('%Y%m%d%H%M%S'))
+        bucket, key, version, time.strftime('%Y%m%d%H%M%S'))
+
+    if version < 1:
+        return 'INVALID_VERSION'
 
     res = await rpc(url.format('promise'))
-    if ARGS.quorum > len(res):
+    if CONF.quorum > len(res):
         return 'NO_PROMISE_QUORUM'
 
     # Find out the accepted value with the highest accepted_seq
     proposal = (0, value)
     for accepted_seq, val in res.values():
         if accepted_seq > proposal[0]:
             proposal = (accepted_seq, val)
 
     if not proposal[1]:
         return 'CANT_SET_EMPTY_VALUE'
 
     res = await rpc(url.format('accept'), proposal[1])
-    if ARGS.quorum > len(res):
+    if CONF.quorum > len(res):
         return 'NO_ACCEPT_QUORUM'
 
     await rpc(url.format('learn'))
 
     return 'OK' if 0 == proposal[0] else 'CONFLICT'
 
 
-@APP.put('/<db:str>/<key:str>/<version:int>')
-async def PUT(request, db, key, version):
-    status = await paxos_client(db, key, version, request.body)
+def get_hmac(token, salt, user):
+    salt = '{}:{}'.format(salt, user).encode()
+    return hmac.new(token.encode(), salt, hashlib.sha256).hexdigest()
+
+
+async def authenticate(request, bucket, user):
+    token = request.headers.get('x-token', None)
+
+    if token is None:
+        raise sanic.exceptions.Unauthorized('UNAUTHORIZED')
+
+    try:
+        await GET(request, bucket, user)
+    except Exception:
+        pass
+
+    version, value = LEARNED_CACHE.get((bucket, user), (0, None))
+
+    if version > 0:
+        profile = json.loads(value)
+
+        if profile['hmac'] != get_hmac(token, profile['salt'], user):
+            raise sanic.exceptions.Unauthorized('UNAUTHORIZED')
+
+    return version
+
+
+@APP.put('/<bucket:str>/<key:str>/<version:int>')
+async def PUT(request, bucket, key, version):
+    await authenticate(request, bucket, bucket)
+
+    status = await paxos_client(bucket, key, version, request.body)
+
+    if 'CONFLICT' == status:
+        raise sanic.exceptions.Forbidden(status)
 
     if 'OK' != status:
         raise sanic.exceptions.BadRequest(status)
 
-    return sanic.response.json(status, headers={
-        'x-db': db,
-        'x-key': key,
-        'x-version': version,
-        'x-length': len(request.body)})
+    return sanic.response.json(dict(bucket=bucket, key=key, version=version,
+                                    length=len(request.body)))
 
 
-@APP.post('/max_version/<db:str>/<key:str>')
-async def max_version(request, db, key):
-    if ARGS.config['cluster_key'] != request.headers['x-cluster-key']:
-        raise sanic.exceptions.Unauthorized('INVALID_CLUSTER_KEY')
+@APP.post('/<bucket:str>/<user:str>')
+async def TOKEN(request, bucket, user):
+    version = await authenticate(request, bucket, user)
 
-    with SQLite(db) as sql:
-        rows = sql('''select max(version) from paxos
-                      where key=? and (accepted_seq != 0 or
-                                       accepted_seq is null)
-                   ''', key)
-
-    return response(rows[0][0] if rows and rows[0][0] else 0)
+    salt, token = str(uuid.uuid4()), str(uuid.uuid4())
+
+    obj = dict(bucket=bucket, salt=salt, user=user,
+               hmac=get_hmac(token, salt, user),
+               cluster=['https://{}'.format(n) for n in CONF.nodes])
+
+    status = await paxos_client(bucket, user, version+1, json.dumps(obj))
+    if 'OK' != status:
+        raise sanic.exceptions.BadRequest(status)
+
+    return sanic.response.json(dict(bucket=obj['bucket'], user=obj['user'],
+                                    token=token, version=version+1,
+                                    cluster=obj['cluster']))
+
+
+@APP.post('/max_version/<bucket:str>/<key:str>')
+async def max_version(request, bucket, key):
+    if request.transport.get_extra_info('peercert') is None:
+        raise sanic.exceptions.Unauthorized('INVALID_CERTIFICATE')
 
+    if (bucket, key) not in MAX_VERSION_CACHE:
+        with SQLite(bucket) as sql:
+            rows = sql('''select max(version) from paxos
+                          where key=? and
+                                (accepted_seq > 0 or accepted_seq is null)
+                       ''', key)
 
-@APP.get('/<db:str>/<key:str>')
-async def GET(request, db, key):
-    res = await rpc('max_version/{}/{}'.format(db, key))
-    if ARGS.quorum > len(res):
+            if rows[0][0] is not None:
+                MAX_VERSION_CACHE[(bucket, key)] = rows[0][0]
+
+    return response(MAX_VERSION_CACHE.get((bucket, key), 0))
+
+
+@APP.get('/<bucket:str>/<key:str>')
+async def GET(request, bucket, key):
+    res = await rpc('max_version/{}/{}'.format(bucket, key))
+    if CONF.quorum > len(res):
         raise sanic.exceptions.BadRequest('NO_MAX_VERSION_QUORUM')
 
     version = max(res.values())
 
-    if 0 == max_version:
+    if 0 == version:
         raise sanic.exceptions.NotFound('KEY_NOT_FOUND')
 
-    for i in range(2):
-        with SQLite(db) as sql:
-            rows = sql('select * from paxos where key=? and version=?',
-                       key, version)
-
-        if rows and rows[0][2] is None and rows[0][3] is None:
-            return sanic.response.raw(rows[0][4], headers={
-                'x-db': db,
-                'x-key': rows[0][0],
-                'x-version': rows[0][1]})
-
-        await paxos_client(db, key, version, None)
-
-    raise sanic.exceptions.BadRequest('SYNC_FAILED')
+    cached_version, cached_value = LEARNED_CACHE.get((bucket, key), (0, None))
+    if version > cached_version:
+        for i in range(2):
+            with SQLite(bucket) as sql:
+                rows = sql('select * from paxos where key=? and version=?',
+                           key, version)
+
+            if rows and rows[0][2] is None and rows[0][3] is None:
+                LEARNED_CACHE[(bucket, key)] = (rows[0][1], rows[0][4])
+                break
+
+            await paxos_client(bucket, key, version, None)
+
+    cached_version, cached_value = LEARNED_CACHE.get((bucket, key), (0, None))
+
+    token = request.headers.get('x-token', None)
+    if token is not None:
+        profile = json.loads(cached_value)
+
+        if profile['hmac'] == get_hmac(token, profile['salt'], key):
+            return sanic.response.text('AUTHENTICATED')
+
+        raise sanic.exceptions.Unauthorized('AUTH_FAILED')
+
+    if cached_version >= version:
+        return sanic.response.raw(cached_value, headers={
+            'x-key': key,
+            'x-bucket': bucket,
+            'x-version': cached_version,
+            'content-type': mimetypes.guess_type(key)[0]})
 
 
 def response(obj):
     return sanic.response.raw(pickle.dumps(obj))
 
 
 async def rpc(url, obj=None):
-    servers = ARGS.config['cluster_nodes']
+    servers = CONF.nodes
 
     if not hasattr(rpc, 'session'):
+        SSL = ssl.create_default_context(
+            cafile='self_signed.pem',
+            purpose=ssl.Purpose.SERVER_AUTH)
+        SSL.load_cert_chain('self_signed.pem', 'self_signed.pem')
+        SSL.verify_mode = ssl.CERT_REQUIRED
+
         rpc.session = aiohttp.ClientSession(
-            headers={'x-cluster-key': ARGS.config['cluster_key']},
-            connector=aiohttp.TCPConnector(
-                limit=1000, limit_per_host=1000, ssl=False))
+            connector=aiohttp.TCPConnector(ssl=SSL))
 
     responses = await asyncio.gather(
         *[asyncio.ensure_future(rpc.session.post(
-            '{}/{}'.format(srv, url), data=pickle.dumps(obj)))
+            'https://{}/{}'.format(srv, url), data=pickle.dumps(obj)))
           for srv in servers],
         return_exceptions=True)
 
     result = dict()
     for s, r in zip(servers, responses):
         if type(r) is aiohttp.client_reqrep.ClientResponse:
             if 200 == r.status:
                 result[s] = pickle.loads(await r.read())
 
     return result
 
 
+class CONF:
+    nodes = None
+    quorum = None
+
+
 if '__main__' == __name__:
-    DEFAULT_CONF = dict(
-        cluster_key="supersecret",
-        cluster_nodes=[
-            "https://localhost:5001",
-            "https://localhost:5002",
-            "https://localhost:5003",
-            "https://localhost:5004",
-            "https://localhost:5005"],
-        ssl_cert="cert.pem",
-        ssl_key="key.pem")
-
-    PARSER = argparse.ArgumentParser(
-        formatter_class=argparse.RawTextHelpFormatter)
-
-    PARSER.add_argument('--bind', help='ip:port')
-    PARSER.add_argument('--config', default='kvlog.json',
-                        help='cluster config file in this format\n{}'.format(
-                             json.dumps(DEFAULT_CONF, indent=4, sort_keys=4)))
-
-    ARGS = PARSER.parse_args()
-
-    with open(ARGS.config) as fd:
-        ARGS.config = json.load(fd)
-        ARGS.quorum = int(len(ARGS.config['cluster_nodes']) / 2) + 1
-
-    HOST, PORT = ARGS.bind.split(':')
-    SSL = None
-    if 'ssl_cert' in ARGS.config:
-        SSL = dict(names=["*"],
-                   key=ARGS.config['ssl_key'],
-                   cert=ARGS.config['ssl_cert'])
+    HOST, PORT = sys.argv[1].split(':')
+    CONF.nodes = set(sys.argv[1:])
+    CONF.quorum = int((len(CONF.nodes)/2)+1)
+
+    SSL = ssl.create_default_context(
+        cafile='self_signed.pem',
+        purpose=ssl.Purpose.CLIENT_AUTH)
+    SSL.load_cert_chain('self_signed.pem', 'self_signed.pem')
+    SSL.verify_mode = ssl.CERT_OPTIONAL
 
     APP.run(HOST, int(PORT), single_process=True, access_log=True, ssl=SSL)
```

### Comparing `buckets-20230725/setup.py` & `buckets-20230729/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import time
 import glob
 from distutils.core import setup
 
 setup(
   name = 'buckets',
   packages = ['buckets'],
+  scripts = ['bin/buckets-gen-cert'],
   version = time.strftime('%Y%m%d'),
   description = 'Highly available key, value store - with GET/PUT operations over HTTPS.',
   long_description = 'Uses Paxos for replication and SQLite for storage. Leaderless and highly available.',
   author = 'Bhupendra Singh',
   author_email = 'bhsingh@gmail.com',
   url = 'https://github.com/magicray/buckets',
   keywords = ['paxos', 'kv', 'key', 'value', 'sqlite', 'consistent']
```

