# Comparing `tmp/mongo_queue_service-0.2.0.tar.gz` & `tmp/mongo_queue_service-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo_queue_service-0.2.0.tar", last modified: Wed Nov 22 11:13:15 2023, max compression
+gzip compressed data, was "mongo_queue_service-0.2.1.tar", last modified: Wed May 29 17:39:21 2024, max compression
```

## Comparing `mongo_queue_service-0.2.0.tar` & `mongo_queue_service-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 a          (501) staff       (20)        0 2023-11-22 11:13:15.312532 mongo_queue_service-0.2.0/
--rw-r--r--   0 a          (501) staff       (20)     1088 2019-12-26 07:56:09.000000 mongo_queue_service-0.2.0/LICENSE
--rw-r--r--   0 a          (501) staff       (20)     5558 2023-11-22 11:13:15.312686 mongo_queue_service-0.2.0/PKG-INFO
--rw-r--r--   0 a          (501) staff       (20)     4949 2023-11-22 11:12:50.000000 mongo_queue_service-0.2.0/README.md
-drwxr-xr-x   0 a          (501) staff       (20)        0 2023-11-22 11:13:15.311116 mongo_queue_service-0.2.0/mongo_queue/
--rw-r--r--   0 a          (501) staff       (20)      161 2019-12-26 06:32:52.000000 mongo_queue_service-0.2.0/mongo_queue/__init__.py
--rw-r--r--   0 a          (501) staff       (20)     3826 2023-02-03 11:49:01.000000 mongo_queue_service-0.2.0/mongo_queue/job.py
--rw-r--r--   0 a          (501) staff       (20)     2347 2019-12-26 07:52:23.000000 mongo_queue_service-0.2.0/mongo_queue/lock.py
--rw-r--r--   0 a          (501) staff       (20)     8023 2023-11-22 11:10:54.000000 mongo_queue_service-0.2.0/mongo_queue/queue.py
--rw-r--r--   0 a          (501) staff       (20)     2096 2023-02-07 06:24:22.000000 mongo_queue_service-0.2.0/mongo_queue/test-parallel.py
--rw-r--r--   0 a          (501) staff       (20)     9695 2023-07-29 07:14:39.000000 mongo_queue_service-0.2.0/mongo_queue/test.py
-drwxr-xr-x   0 a          (501) staff       (20)        0 2023-11-22 11:13:15.312390 mongo_queue_service-0.2.0/mongo_queue_service.egg-info/
--rw-r--r--   0 a          (501) staff       (20)     5558 2023-11-22 11:13:15.000000 mongo_queue_service-0.2.0/mongo_queue_service.egg-info/PKG-INFO
--rw-r--r--   0 a          (501) staff       (20)      383 2023-11-22 11:13:15.000000 mongo_queue_service-0.2.0/mongo_queue_service.egg-info/SOURCES.txt
--rw-r--r--   0 a          (501) staff       (20)        1 2023-11-22 11:13:15.000000 mongo_queue_service-0.2.0/mongo_queue_service.egg-info/dependency_links.txt
--rw-r--r--   0 a          (501) staff       (20)        8 2023-11-22 11:13:15.000000 mongo_queue_service-0.2.0/mongo_queue_service.egg-info/requires.txt
--rw-r--r--   0 a          (501) staff       (20)       12 2023-11-22 11:13:15.000000 mongo_queue_service-0.2.0/mongo_queue_service.egg-info/top_level.txt
--rw-r--r--   0 a          (501) staff       (20)       79 2023-11-22 11:13:15.312994 mongo_queue_service-0.2.0/setup.cfg
--rw-r--r--   0 a          (501) staff       (20)      858 2023-11-22 11:12:02.000000 mongo_queue_service-0.2.0/setup.py
+drwxr-xr-x   0 a          (501) staff       (20)        0 2024-05-29 17:39:21.430144 mongo_queue_service-0.2.1/
+-rw-r--r--   0 a          (501) staff       (20)     1088 2024-02-20 04:45:12.000000 mongo_queue_service-0.2.1/LICENSE
+-rw-r--r--   0 a          (501) staff       (20)     5587 2024-05-29 17:39:21.430042 mongo_queue_service-0.2.1/PKG-INFO
+-rw-r--r--   0 a          (501) staff       (20)     4991 2024-05-29 17:38:58.000000 mongo_queue_service-0.2.1/README.md
+drwxr-xr-x   0 a          (501) staff       (20)        0 2024-05-29 17:39:21.426643 mongo_queue_service-0.2.1/mongo_queue/
+-rw-r--r--   0 a          (501) staff       (20)      161 2024-02-20 04:45:12.000000 mongo_queue_service-0.2.1/mongo_queue/__init__.py
+-rw-r--r--   0 a          (501) staff       (20)     3826 2024-02-20 04:47:12.000000 mongo_queue_service-0.2.1/mongo_queue/job.py
+-rw-r--r--   0 a          (501) staff       (20)     2347 2024-02-20 04:45:12.000000 mongo_queue_service-0.2.1/mongo_queue/lock.py
+-rw-r--r--   0 a          (501) staff       (20)     8410 2024-05-29 17:25:25.000000 mongo_queue_service-0.2.1/mongo_queue/queue.py
+-rw-r--r--   0 a          (501) staff       (20)     2096 2024-02-20 04:45:12.000000 mongo_queue_service-0.2.1/mongo_queue/test-parallel.py
+-rw-r--r--   0 a          (501) staff       (20)    10115 2024-05-29 17:32:45.000000 mongo_queue_service-0.2.1/mongo_queue/test.py
+drwxr-xr-x   0 a          (501) staff       (20)        0 2024-05-29 17:39:21.429580 mongo_queue_service-0.2.1/mongo_queue_service.egg-info/
+-rw-r--r--   0 a          (501) staff       (20)     5587 2024-05-29 17:39:21.000000 mongo_queue_service-0.2.1/mongo_queue_service.egg-info/PKG-INFO
+-rw-r--r--   0 a          (501) staff       (20)      383 2024-05-29 17:39:21.000000 mongo_queue_service-0.2.1/mongo_queue_service.egg-info/SOURCES.txt
+-rw-r--r--   0 a          (501) staff       (20)        1 2024-05-29 17:39:21.000000 mongo_queue_service-0.2.1/mongo_queue_service.egg-info/dependency_links.txt
+-rw-r--r--   0 a          (501) staff       (20)        8 2024-05-29 17:39:21.000000 mongo_queue_service-0.2.1/mongo_queue_service.egg-info/requires.txt
+-rw-r--r--   0 a          (501) staff       (20)       12 2024-05-29 17:39:21.000000 mongo_queue_service-0.2.1/mongo_queue_service.egg-info/top_level.txt
+-rw-r--r--   0 a          (501) staff       (20)       79 2024-05-29 17:39:21.430569 mongo_queue_service-0.2.1/setup.cfg
+-rw-r--r--   0 a          (501) staff       (20)      858 2024-05-29 17:39:06.000000 mongo_queue_service-0.2.1/setup.py
```

### Comparing `mongo_queue_service-0.2.0/LICENSE` & `mongo_queue_service-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mongo_queue_service-0.2.0/PKG-INFO` & `mongo_queue_service-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: mongo_queue_service
-Version: 0.2.0
+Version: 0.2.1
 Summary: Queue service built on top of mongo.
 Home-page: https://github.com/shunyeka/mongo_queue/
+Download-URL: https://github.com/shunyeka/mongo_queue/archive/v0.1.8.tar.gz
 Author: Amit Chotaliya
 Author-email: amit@shunyeka.com
-License: UNKNOWN
-Download-URL: https://github.com/shunyeka/mongo_queue/archive/v0.1.8.tar.gz
 Keywords: mongo,queue,priority queue,task queue
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pymongo
 
 # mongo_queue
 Task queue built on mongo with channels and unique job id.
 
 [Website](http://www.shunyeka.com) • [autobotAI Automation Platform](https://autobot.live/)
 
 Inspired by [kapilt/mongoqueue](https://github.com/kapilt/mongoqueue)
 
 ### Change Log:
 
-#### v0.2.0
+#### v0.2.1
 
-- Fixed the task queue cleanup method
+- Added optional locking when finding job by id, so it can be marked completed.
 
 #### v0.1.9
 
 - Added method to get pending jobs by channels
 
 #### v0.1.8
 
@@ -202,8 +201,7 @@
 export MONGO_URI=mongodb+srv://username:pwd@mongourl/test?retryWrites=true&w=majority
 cd mong_queue # Root directory of the package
 python3.9 -m venv venv
 source venv/bin/activate
 pip install -r requirements.txt
 python3 -m unittest mongo_queue.test
 ```
-
```

### Comparing `mongo_queue_service-0.2.0/README.md` & `mongo_queue_service-0.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 [Website](http://www.shunyeka.com) • [autobotAI Automation Platform](https://autobot.live/)
 
 Inspired by [kapilt/mongoqueue](https://github.com/kapilt/mongoqueue)
 
 ### Change Log:
 
-#### v0.2.0
+#### v0.2.1
 
-- Fixed the task queue cleanup method
+- Added optional locking when finding job by id, so it can be marked completed.
 
 #### v0.1.9
 
 - Added method to get pending jobs by channels
 
 #### v0.1.8
```

### Comparing `mongo_queue_service-0.2.0/mongo_queue/job.py` & `mongo_queue_service-0.2.1/mongo_queue/job.py`

 * *Files identical despite different names*

### Comparing `mongo_queue_service-0.2.0/mongo_queue/lock.py` & `mongo_queue_service-0.2.1/mongo_queue/lock.py`

 * *Files identical despite different names*

### Comparing `mongo_queue_service-0.2.0/mongo_queue/queue.py` & `mongo_queue_service-0.2.1/mongo_queue/queue.py`

 * *Files 9% similar despite different names*

```diff
@@ -155,28 +155,37 @@
             sort=[('priority', pymongo.DESCENDING), ("queued_at", pymongo.ASCENDING)],
             return_document=ReturnDocument.AFTER
         )
         if next_job:
             next_job = self._wrap_one(next_job)
         return next_job
 
-    def find_job_by_id(self, _id):
+    def find_job_by_id(self, _id, lock=False):
         if not _id:
             raise AttributeError("id required.")
         if not isinstance(_id, ObjectId):
             _id = ObjectId(_id)
-        return self._wrap_one(self.collection.find_one(filter={"_id": _id}))
+        if lock:
+            return self._wrap_one(self.collection.find_one_and_update(
+                filter={"_id": _id},
+                update={"$set": {"locked_by": self.consumer_id,
+                                 "locked_at": datetime.now()}},
+                return_document=ReturnDocument.AFTER
+            ))
+        else:
+            return self._wrap_one(self.collection.find_one(filter={"_id": _id}))
 
     def _jobs(self):
-        return self.collection.find(
+        jobs_cursor = self.collection.find(
             query={"locked_by": None,
                    "locked_at": None,
                    "attempts": {"$lt": self.max_attempts}},
             sort=[('priority', pymongo.DESCENDING)],
         )
+        jobs_cursor.hint("")
 
     def _wrap_one(self, data):
         return data and Job(self, data) or None
 
     @staticmethod
     def _depends_on_bson(depends_on):
         if not depends_on:
```

### Comparing `mongo_queue_service-0.2.0/mongo_queue/test-parallel.py` & `mongo_queue_service-0.2.1/mongo_queue/test-parallel.py`

 * *Files identical despite different names*

### Comparing `mongo_queue_service-0.2.0/mongo_queue/test.py` & `mongo_queue_service-0.2.1/mongo_queue/test.py`

 * *Files 5% similar despite different names*

```diff
@@ -149,14 +149,25 @@
 
         self.queue.put(data)
         self.assertEqual(self.queue.size(), 1)
         job = self.queue.next()
         find_copy_job = self.queue.find_job_by_id(job.job_id)
         self.assert_job_equal(find_copy_job, data)
 
+    def test_find_by_id(self):
+        data = {"context_id": "alpha",
+                "data": [1, 2, 3]}
+
+        job_id = self.queue.put(data)
+        self.assertEqual(self.queue.size(), 1)
+        non_locked_job = self.queue.find_job_by_id(job_id)
+        self.assertIsNone(non_locked_job.locked_by)
+        locked_job = self.queue.find_job_by_id(job_id, lock=True)
+        self.assertIsNotNone(locked_job.locked_by)
+
     def test_release(self):
         data = {"context_id": "alpha",
                 "data": [1, 2, 3],
                 "more-data": time.time()}
 
         self.queue.put(data)
         job = self.queue.next()
```

### Comparing `mongo_queue_service-0.2.0/mongo_queue_service.egg-info/PKG-INFO` & `mongo_queue_service-0.2.1/mongo_queue_service.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: mongo-queue-service
-Version: 0.2.0
+Version: 0.2.1
 Summary: Queue service built on top of mongo.
 Home-page: https://github.com/shunyeka/mongo_queue/
+Download-URL: https://github.com/shunyeka/mongo_queue/archive/v0.1.8.tar.gz
 Author: Amit Chotaliya
 Author-email: amit@shunyeka.com
-License: UNKNOWN
-Download-URL: https://github.com/shunyeka/mongo_queue/archive/v0.1.8.tar.gz
 Keywords: mongo,queue,priority queue,task queue
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pymongo
 
 # mongo_queue
 Task queue built on mongo with channels and unique job id.
 
 [Website](http://www.shunyeka.com) • [autobotAI Automation Platform](https://autobot.live/)
 
 Inspired by [kapilt/mongoqueue](https://github.com/kapilt/mongoqueue)
 
 ### Change Log:
 
-#### v0.2.0
+#### v0.2.1
 
-- Fixed the task queue cleanup method
+- Added optional locking when finding job by id, so it can be marked completed.
 
 #### v0.1.9
 
 - Added method to get pending jobs by channels
 
 #### v0.1.8
 
@@ -202,8 +201,7 @@
 export MONGO_URI=mongodb+srv://username:pwd@mongourl/test?retryWrites=true&w=majority
 cd mong_queue # Root directory of the package
 python3.9 -m venv venv
 source venv/bin/activate
 pip install -r requirements.txt
 python3 -m unittest mongo_queue.test
 ```
-
```

### Comparing `mongo_queue_service-0.2.0/setup.py` & `mongo_queue_service-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mongo_queue_service",
-    version="0.2.0",
+    version="0.2.1",
     author="Amit Chotaliya",
     author_email="amit@shunyeka.com",
     description="Queue service built on top of mongo.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/shunyeka/mongo_queue/",
     download_url='https://github.com/shunyeka/mongo_queue/archive/v0.1.8.tar.gz',
```

