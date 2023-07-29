# Comparing `tmp/mongo_queue_service-0.1.8.tar.gz` & `tmp/mongo_queue_service-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo_queue_service-0.1.8.tar", last modified: Mon Feb 20 10:04:13 2023, max compression
+gzip compressed data, was "mongo_queue_service-0.1.9.tar", last modified: Sat Jul 29 07:16:53 2023, max compression
```

## Comparing `mongo_queue_service-0.1.8.tar` & `mongo_queue_service-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 a          (501) staff       (20)        0 2023-02-20 10:04:13.380427 mongo_queue_service-0.1.8/
--rw-r--r--   0 a          (501) staff       (20)     1088 2019-12-26 07:56:09.000000 mongo_queue_service-0.1.8/LICENSE
--rw-r--r--   0 a          (501) staff       (20)     5363 2023-02-20 10:04:13.380530 mongo_queue_service-0.1.8/PKG-INFO
--rw-r--r--   0 a          (501) staff       (20)     4754 2023-02-20 10:02:51.000000 mongo_queue_service-0.1.8/README.md
-drwxr-xr-x   0 a          (501) staff       (20)        0 2023-02-20 10:04:13.379028 mongo_queue_service-0.1.8/mongo_queue/
--rw-r--r--   0 a          (501) staff       (20)      161 2019-12-26 06:32:52.000000 mongo_queue_service-0.1.8/mongo_queue/__init__.py
--rw-r--r--   0 a          (501) staff       (20)     3826 2023-02-03 11:49:01.000000 mongo_queue_service-0.1.8/mongo_queue/job.py
--rw-r--r--   0 a          (501) staff       (20)     2347 2019-12-26 07:52:23.000000 mongo_queue_service-0.1.8/mongo_queue/lock.py
--rw-r--r--   0 a          (501) staff       (20)     7518 2023-02-20 10:02:51.000000 mongo_queue_service-0.1.8/mongo_queue/queue.py
--rw-r--r--   0 a          (501) staff       (20)     2096 2023-02-07 06:24:22.000000 mongo_queue_service-0.1.8/mongo_queue/test-parallel.py
--rw-r--r--   0 a          (501) staff       (20)     9091 2023-02-20 10:02:51.000000 mongo_queue_service-0.1.8/mongo_queue/test.py
-drwxr-xr-x   0 a          (501) staff       (20)        0 2023-02-20 10:04:13.380224 mongo_queue_service-0.1.8/mongo_queue_service.egg-info/
--rw-r--r--   0 a          (501) staff       (20)     5363 2023-02-20 10:04:13.000000 mongo_queue_service-0.1.8/mongo_queue_service.egg-info/PKG-INFO
--rw-r--r--   0 a          (501) staff       (20)      383 2023-02-20 10:04:13.000000 mongo_queue_service-0.1.8/mongo_queue_service.egg-info/SOURCES.txt
--rw-r--r--   0 a          (501) staff       (20)        1 2023-02-20 10:04:13.000000 mongo_queue_service-0.1.8/mongo_queue_service.egg-info/dependency_links.txt
--rw-r--r--   0 a          (501) staff       (20)        8 2023-02-20 10:04:13.000000 mongo_queue_service-0.1.8/mongo_queue_service.egg-info/requires.txt
--rw-r--r--   0 a          (501) staff       (20)       12 2023-02-20 10:04:13.000000 mongo_queue_service-0.1.8/mongo_queue_service.egg-info/top_level.txt
--rw-r--r--   0 a          (501) staff       (20)       79 2023-02-20 10:04:13.380889 mongo_queue_service-0.1.8/setup.cfg
--rw-r--r--   0 a          (501) staff       (20)      858 2023-02-20 10:03:51.000000 mongo_queue_service-0.1.8/setup.py
+drwxr-xr-x   0 a          (501) staff       (20)        0 2023-07-29 07:16:53.300505 mongo_queue_service-0.1.9/
+-rw-r--r--   0 a          (501) staff       (20)     1088 2019-12-26 07:56:09.000000 mongo_queue_service-0.1.9/LICENSE
+-rw-r--r--   0 a          (501) staff       (20)     5422 2023-07-29 07:16:53.300562 mongo_queue_service-0.1.9/PKG-INFO
+-rw-r--r--   0 a          (501) staff       (20)     4813 2023-07-29 07:15:36.000000 mongo_queue_service-0.1.9/README.md
+drwxr-xr-x   0 a          (501) staff       (20)        0 2023-07-29 07:16:53.299555 mongo_queue_service-0.1.9/mongo_queue/
+-rw-r--r--   0 a          (501) staff       (20)      161 2019-12-26 06:32:52.000000 mongo_queue_service-0.1.9/mongo_queue/__init__.py
+-rw-r--r--   0 a          (501) staff       (20)     3826 2023-02-03 11:49:01.000000 mongo_queue_service-0.1.9/mongo_queue/job.py
+-rw-r--r--   0 a          (501) staff       (20)     2347 2019-12-26 07:52:23.000000 mongo_queue_service-0.1.9/mongo_queue/lock.py
+-rw-r--r--   0 a          (501) staff       (20)     8006 2023-07-29 07:04:28.000000 mongo_queue_service-0.1.9/mongo_queue/queue.py
+-rw-r--r--   0 a          (501) staff       (20)     2096 2023-02-07 06:24:22.000000 mongo_queue_service-0.1.9/mongo_queue/test-parallel.py
+-rw-r--r--   0 a          (501) staff       (20)     9695 2023-07-29 07:14:39.000000 mongo_queue_service-0.1.9/mongo_queue/test.py
+drwxr-xr-x   0 a          (501) staff       (20)        0 2023-07-29 07:16:53.300398 mongo_queue_service-0.1.9/mongo_queue_service.egg-info/
+-rw-r--r--   0 a          (501) staff       (20)     5422 2023-07-29 07:16:53.000000 mongo_queue_service-0.1.9/mongo_queue_service.egg-info/PKG-INFO
+-rw-r--r--   0 a          (501) staff       (20)      383 2023-07-29 07:16:53.000000 mongo_queue_service-0.1.9/mongo_queue_service.egg-info/SOURCES.txt
+-rw-r--r--   0 a          (501) staff       (20)        1 2023-07-29 07:16:53.000000 mongo_queue_service-0.1.9/mongo_queue_service.egg-info/dependency_links.txt
+-rw-r--r--   0 a          (501) staff       (20)        8 2023-07-29 07:16:53.000000 mongo_queue_service-0.1.9/mongo_queue_service.egg-info/requires.txt
+-rw-r--r--   0 a          (501) staff       (20)       12 2023-07-29 07:16:53.000000 mongo_queue_service-0.1.9/mongo_queue_service.egg-info/top_level.txt
+-rw-r--r--   0 a          (501) staff       (20)       79 2023-07-29 07:16:53.300774 mongo_queue_service-0.1.9/setup.cfg
+-rw-r--r--   0 a          (501) staff       (20)      858 2023-07-29 07:15:46.000000 mongo_queue_service-0.1.9/setup.py
```

### Comparing `mongo_queue_service-0.1.8/LICENSE` & `mongo_queue_service-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mongo_queue_service-0.1.8/PKG-INFO` & `mongo_queue_service-0.1.9/mongo_queue_service.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mongo_queue_service
-Version: 0.1.8
+Name: mongo-queue-service
+Version: 0.1.9
 Summary: Queue service built on top of mongo.
 Home-page: https://github.com/shunyeka/mongo_queue/
 Author: Amit Chotaliya
 Author-email: amit@shunyeka.com
 License: UNKNOWN
 Download-URL: https://github.com/shunyeka/mongo_queue/archive/v0.1.8.tar.gz
 Keywords: mongo,queue,priority queue,task queue
@@ -17,18 +17,22 @@
 License-File: LICENSE
 
 # mongo_queue
 Task queue built on mongo with channels and unique job id.
 
 [Website](http://www.shunyeka.com) • [autobotAI Automation Platform](https://autobot.live/)
 
-Inspired from [kapilt/mongoqueue](https://github.com/kapilt/mongoqueue)
+Inspired by [kapilt/mongoqueue](https://github.com/kapilt/mongoqueue)
 
 ### Change Log:
 
+#### v0.1.9
+
+- Added method to get pending jobs by channels
+
 #### v0.1.8
 
 - Added `delay` while queuing a new job. This allows user to delay the job execution by x seconds. It is similar to `sleep` but this allows the functionality for the fresh jobs.
 
 #### v0.1.7
 
 - Added index for repair operation.
```

### Comparing `mongo_queue_service-0.1.8/README.md` & `mongo_queue_service-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 # mongo_queue
 Task queue built on mongo with channels and unique job id.
 
 [Website](http://www.shunyeka.com) • [autobotAI Automation Platform](https://autobot.live/)
 
-Inspired from [kapilt/mongoqueue](https://github.com/kapilt/mongoqueue)
+Inspired by [kapilt/mongoqueue](https://github.com/kapilt/mongoqueue)
 
 ### Change Log:
 
+#### v0.1.9
+
+- Added method to get pending jobs by channels
+
 #### v0.1.8
 
 - Added `delay` while queuing a new job. This allows user to delay the job execution by x seconds. It is similar to `sleep` but this allows the functionality for the fresh jobs.
 
 #### v0.1.7
 
 - Added index for repair operation.
```

### Comparing `mongo_queue_service-0.1.8/mongo_queue/job.py` & `mongo_queue_service-0.1.9/mongo_queue/job.py`

 * *Files identical despite different names*

### Comparing `mongo_queue_service-0.1.8/mongo_queue/lock.py` & `mongo_queue_service-0.1.9/mongo_queue/lock.py`

 * *Files identical despite different names*

### Comparing `mongo_queue_service-0.1.8/mongo_queue/queue.py` & `mongo_queue_service-0.1.9/mongo_queue/queue.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,15 +89,15 @@
                                     update={"attempts": {"$gte": self.max_attempts}},
                                     remove=True)
 
     def put(self, payload, priority=0, channel="default", job_id=None, depends_on=[], delay: int = None):
         """Place a job into the queue
         """
         job = dict(DEFAULT_INSERT)
-        if delay:            
+        if delay:
             now_plus_seconds = datetime.now() + timedelta(seconds=delay)
             job['run_after'] = now_plus_seconds
         depends_on_bson = Queue._depends_on_bson(depends_on)
         job['priority'] = priority
         job['payload'] = payload
         job['channel'] = channel
         job['job_id'] = job_id or str(uuid4())
@@ -112,27 +112,44 @@
     def running_count(self, channel="default"):
         return self.collection.count_documents(filter={'locked_by': {"$ne": None}, 'locked_at': {"$ne": None},
                                                        "channel": channel,
                                                        "attempts": {"$lt": self.max_attempts}
                                                        })
 
     def _pending_filter(self, channel):
-        return {'locked_by': None,
-                'locked_at': None,
-                "channel": channel,
-                "attempts": {"$lt": self.max_attempts},
-                "$and": [
-                    {"$or": [{"depends_on": {"$exists": False}, "depends_on": {"$size": 0}}]},
-                    {"$or": [{"run_after": {"$exists": False}}, {"run_after": {"$lt": datetime.now()}}]}
-                ]
-                }
+        filters = {'locked_by': None,
+                   'locked_at': None,
+                   "attempts": {"$lt": self.max_attempts},
+                   "$and": [
+                       {"$or": [{"depends_on": {"$exists": False}, "depends_on": {"$size": 0}}]},
+                       {"$or": [{"run_after": {"$exists": False}}, {"run_after": {"$lt": datetime.now()}}]}
+                   ]
+                   }
+        if channel:
+            filters["channel"] = channel
+        return filters
 
     def pending_count(self, channel="default"):
         return self.collection.count_documents(filter=self._pending_filter(channel=channel))
 
+    def pending_count_by_channels(self):
+        pending_filter = self._pending_filter(channel=None)
+        return list(self.collection.aggregate([{
+            "$match": pending_filter
+        }, {
+            "$group": {"_id": "$channel", "count": {"$sum": 1}}
+        }, {
+            "$project": {
+                "channel": "$_id",
+                "count": 1,
+                "_id": 0
+            }
+        }
+        ]))
+
     def next(self, channel="default"):
         next_job = self.collection.find_one_and_update(
             filter=self._pending_filter(channel=channel),
             update={"$set": {"locked_by": self.consumer_id,
                              "locked_at": datetime.now()}},
             sort=[('priority', pymongo.DESCENDING), ("queued_at", pymongo.ASCENDING)],
             return_document=ReturnDocument.AFTER
```

### Comparing `mongo_queue_service-0.1.8/mongo_queue/test-parallel.py` & `mongo_queue_service-0.1.9/mongo_queue/test-parallel.py`

 * *Files identical despite different names*

### Comparing `mongo_queue_service-0.1.8/mongo_queue/test.py` & `mongo_queue_service-0.1.9/mongo_queue/test.py`

 * *Files 5% similar despite different names*

```diff
@@ -259,7 +259,20 @@
 
         self.queue.put(data, job_id=1)
         job2 = self.queue.put({"context_id": "beta",
                                "data": [1, 2, 3],
                                "more-data": time.time()}, job_id=1)
         self.assertEqual(job2, False)
         self.assert_job_equal(self.queue.next(), data)
+
+    def test_pending_count_by_channels(self):
+        data = {"context_id": "alpha",
+                "data": [1, 2, 3],
+                "more-data": time.time()}
+
+        self.queue.put(data, channel="one")
+        self.queue.put(data, channel="two")
+        self.queue.put(data, channel="two")
+        self.queue.put(data, channel="three")
+        self.queue.put(data, channel="three")
+        self.queue.put(data, channel="three")
+        self.assertCountEqual(self.queue.pending_count_by_channels(), [{"channel": "one", "count": 1}, {"channel": "two", "count": 2}, {"channel": "three", "count": 3}])
```

### Comparing `mongo_queue_service-0.1.8/mongo_queue_service.egg-info/PKG-INFO` & `mongo_queue_service-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mongo-queue-service
-Version: 0.1.8
+Name: mongo_queue_service
+Version: 0.1.9
 Summary: Queue service built on top of mongo.
 Home-page: https://github.com/shunyeka/mongo_queue/
 Author: Amit Chotaliya
 Author-email: amit@shunyeka.com
 License: UNKNOWN
 Download-URL: https://github.com/shunyeka/mongo_queue/archive/v0.1.8.tar.gz
 Keywords: mongo,queue,priority queue,task queue
@@ -17,18 +17,22 @@
 License-File: LICENSE
 
 # mongo_queue
 Task queue built on mongo with channels and unique job id.
 
 [Website](http://www.shunyeka.com) • [autobotAI Automation Platform](https://autobot.live/)
 
-Inspired from [kapilt/mongoqueue](https://github.com/kapilt/mongoqueue)
+Inspired by [kapilt/mongoqueue](https://github.com/kapilt/mongoqueue)
 
 ### Change Log:
 
+#### v0.1.9
+
+- Added method to get pending jobs by channels
+
 #### v0.1.8
 
 - Added `delay` while queuing a new job. This allows user to delay the job execution by x seconds. It is similar to `sleep` but this allows the functionality for the fresh jobs.
 
 #### v0.1.7
 
 - Added index for repair operation.
```

### Comparing `mongo_queue_service-0.1.8/setup.py` & `mongo_queue_service-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mongo_queue_service",
-    version="0.1.8",
+    version="0.1.9",
     author="Amit Chotaliya",
     author_email="amit@shunyeka.com",
     description="Queue service built on top of mongo.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/shunyeka/mongo_queue/",
     download_url='https://github.com/shunyeka/mongo_queue/archive/v0.1.8.tar.gz',
```

