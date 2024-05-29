# Comparing `tmp/judoscale-1.7.0.tar.gz` & `tmp/judoscale-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "judoscale-1.7.0.tar", max compression
+gzip compressed data, was "judoscale-1.7.1.tar", max compression
```

## Comparing `judoscale-1.7.0.tar` & `judoscale-1.7.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1066 2024-03-18 11:58:40.377287 judoscale-1.7.0/LICENSE
--rw-r--r--   0        0        0    16929 2024-03-18 11:58:40.377287 judoscale-1.7.0/README.md
--rw-r--r--   0        0        0        0 2024-03-18 11:58:40.377287 judoscale-1.7.0/judoscale/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 11:58:40.377287 judoscale-1.7.0/judoscale/asgi/__init__.py
--rw-r--r--   0        0        0     2212 2024-03-18 11:58:40.377287 judoscale-1.7.0/judoscale/asgi/middleware.py
--rw-r--r--   0        0        0     1122 2024-03-18 11:58:40.377287 judoscale-1.7.0/judoscale/celery/__init__.py
--rw-r--r--   0        0        0     4717 2024-03-18 11:58:40.377287 judoscale-1.7.0/judoscale/celery/collector.py
--rw-r--r--   0        0        0        0 2024-03-18 11:58:40.377287 judoscale-1.7.0/judoscale/core/__init__.py
--rw-r--r--   0        0        0      642 2024-03-18 11:58:40.377287 judoscale-1.7.0/judoscale/core/adapter.py
--rw-r--r--   0        0        0     3456 2024-03-18 11:58:40.377287 judoscale-1.7.0/judoscale/core/config.py
--rw-r--r--   0        0        0       56 2024-03-18 11:58:40.377287 judoscale-1.7.0/judoscale/core/logger.py
--rw-r--r--   0        0        0     4271 2024-03-18 11:58:40.377287 judoscale-1.7.0/judoscale/core/metric.py
--rw-r--r--   0        0        0     2474 2024-03-18 11:58:40.377287 judoscale-1.7.0/judoscale/core/metrics_collectors.py
--rw-r--r--   0        0        0     1564 2024-03-18 11:58:40.377287 judoscale-1.7.0/judoscale/core/metrics_store.py
--rw-r--r--   0        0        0     4244 2024-03-18 11:58:40.377287 judoscale-1.7.0/judoscale/core/reporter.py
--rw-r--r--   0        0        0      275 2024-03-18 11:58:40.377287 judoscale-1.7.0/judoscale/django/__init__.py
--rw-r--r--   0        0        0     1320 2024-03-18 11:58:40.377287 judoscale-1.7.0/judoscale/django/apps.py
--rw-r--r--   0        0        0     1054 2024-03-18 11:58:40.377287 judoscale-1.7.0/judoscale/django/middleware.py
--rw-r--r--   0        0        0      829 2024-03-18 11:58:40.377287 judoscale-1.7.0/judoscale/django/redis.py
--rw-r--r--   0        0        0       73 2024-03-18 11:58:40.377287 judoscale-1.7.0/judoscale/flask/__init__.py
--rw-r--r--   0        0        0     1452 2024-03-18 11:58:40.377287 judoscale-1.7.0/judoscale/flask/judoscale.py
--rw-r--r--   0        0        0     1182 2024-03-18 11:58:40.377287 judoscale-1.7.0/judoscale/rq/__init__.py
--rw-r--r--   0        0        0      764 2024-03-18 11:58:40.377287 judoscale-1.7.0/judoscale/rq/apps.py
--rw-r--r--   0        0        0     3080 2024-03-18 11:58:40.377287 judoscale-1.7.0/judoscale/rq/collector.py
--rw-r--r--   0        0        0     1358 2024-03-18 11:58:40.377287 judoscale-1.7.0/pyproject.toml
--rw-r--r--   0        0        0    18460 1970-01-01 00:00:00.000000 judoscale-1.7.0/setup.py
--rw-r--r--   0        0        0    18110 1970-01-01 00:00:00.000000 judoscale-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-29 20:35:10.247209 judoscale-1.7.1/LICENSE
+-rw-r--r--   0        0        0    16929 2024-05-29 20:35:10.247209 judoscale-1.7.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-29 20:35:10.247209 judoscale-1.7.1/judoscale/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:35:10.247209 judoscale-1.7.1/judoscale/asgi/__init__.py
+-rw-r--r--   0        0        0     2212 2024-05-29 20:35:10.247209 judoscale-1.7.1/judoscale/asgi/middleware.py
+-rw-r--r--   0        0        0     1122 2024-05-29 20:35:10.247209 judoscale-1.7.1/judoscale/celery/__init__.py
+-rw-r--r--   0        0        0     4738 2024-05-29 20:35:10.247209 judoscale-1.7.1/judoscale/celery/collector.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:35:10.247209 judoscale-1.7.1/judoscale/core/__init__.py
+-rw-r--r--   0        0        0      642 2024-05-29 20:35:10.247209 judoscale-1.7.1/judoscale/core/adapter.py
+-rw-r--r--   0        0        0     3456 2024-05-29 20:35:10.247209 judoscale-1.7.1/judoscale/core/config.py
+-rw-r--r--   0        0        0       56 2024-05-29 20:35:10.247209 judoscale-1.7.1/judoscale/core/logger.py
+-rw-r--r--   0        0        0     4271 2024-05-29 20:35:10.247209 judoscale-1.7.1/judoscale/core/metric.py
+-rw-r--r--   0        0        0     2474 2024-05-29 20:35:10.247209 judoscale-1.7.1/judoscale/core/metrics_collectors.py
+-rw-r--r--   0        0        0     1564 2024-05-29 20:35:10.247209 judoscale-1.7.1/judoscale/core/metrics_store.py
+-rw-r--r--   0        0        0     4244 2024-05-29 20:35:10.247209 judoscale-1.7.1/judoscale/core/reporter.py
+-rw-r--r--   0        0        0      275 2024-05-29 20:35:10.247209 judoscale-1.7.1/judoscale/django/__init__.py
+-rw-r--r--   0        0        0     1320 2024-05-29 20:35:10.247209 judoscale-1.7.1/judoscale/django/apps.py
+-rw-r--r--   0        0        0     1054 2024-05-29 20:35:10.247209 judoscale-1.7.1/judoscale/django/middleware.py
+-rw-r--r--   0        0        0      829 2024-05-29 20:35:10.247209 judoscale-1.7.1/judoscale/django/redis.py
+-rw-r--r--   0        0        0       73 2024-05-29 20:35:10.247209 judoscale-1.7.1/judoscale/flask/__init__.py
+-rw-r--r--   0        0        0     1452 2024-05-29 20:35:10.247209 judoscale-1.7.1/judoscale/flask/judoscale.py
+-rw-r--r--   0        0        0     1182 2024-05-29 20:35:10.247209 judoscale-1.7.1/judoscale/rq/__init__.py
+-rw-r--r--   0        0        0      764 2024-05-29 20:35:10.247209 judoscale-1.7.1/judoscale/rq/apps.py
+-rw-r--r--   0        0        0     3080 2024-05-29 20:35:10.247209 judoscale-1.7.1/judoscale/rq/collector.py
+-rw-r--r--   0        0        0     1358 2024-05-29 20:35:10.247209 judoscale-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0    18460 1970-01-01 00:00:00.000000 judoscale-1.7.1/setup.py
+-rw-r--r--   0        0        0    18110 1970-01-01 00:00:00.000000 judoscale-1.7.1/PKG-INFO
```

### Comparing `judoscale-1.7.0/LICENSE` & `judoscale-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `judoscale-1.7.0/README.md` & `judoscale-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `judoscale-1.7.0/judoscale/asgi/middleware.py` & `judoscale-1.7.1/judoscale/asgi/middleware.py`

 * *Files identical despite different names*

### Comparing `judoscale-1.7.0/judoscale/celery/__init__.py` & `judoscale-1.7.1/judoscale/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `judoscale-1.7.0/judoscale/celery/collector.py` & `judoscale-1.7.1/judoscale/celery/collector.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
         self._celery_queues: Set[str] = set()
         self.task_sent_handler = TaskSentHandler(self, connection)
         logger.debug(f"Redis is at {self.redis.connection_pool}")
 
         system_queues = {"unacked", "unacked_index"}
         user_queues = {
-            q.decode("utf-8") if type(q) is bytes else q
+            q.decode("utf-8") if isinstance(q, bytes) else q
             for q in self.redis.scan_iter(match="[^_]*", _type="list")
         }
         logger.debug(f"Found initial queues: {list(user_queues)}")
         self._celery_queues = user_queues - system_queues
         self.task_sent_handler.start()
 
     @property
@@ -128,15 +128,15 @@
                     metrics.append(
                         Metric.for_queue(queue_name=queue, oldest_job_ts=published_at)
                     )
                 else:
                     task_id = task.get("id", None)
                     logger.warning(
                         "Unable to find `published_at` in task properties for "
-                        f"task ID {task_id}."
+                        f"task ID {task_id} in queue {queue}."
                     )
             else:
                 metrics.append(
                     Metric.for_queue(queue_name=queue, oldest_job_ts=time.time())
                 )
 
         return metrics
```

### Comparing `judoscale-1.7.0/judoscale/core/adapter.py` & `judoscale-1.7.1/judoscale/core/adapter.py`

 * *Files identical despite different names*

### Comparing `judoscale-1.7.0/judoscale/core/config.py` & `judoscale-1.7.1/judoscale/core/config.py`

 * *Files identical despite different names*

### Comparing `judoscale-1.7.0/judoscale/core/metric.py` & `judoscale-1.7.1/judoscale/core/metric.py`

 * *Files identical despite different names*

### Comparing `judoscale-1.7.0/judoscale/core/metrics_collectors.py` & `judoscale-1.7.1/judoscale/core/metrics_collectors.py`

 * *Files identical despite different names*

### Comparing `judoscale-1.7.0/judoscale/core/metrics_store.py` & `judoscale-1.7.1/judoscale/core/metrics_store.py`

 * *Files identical despite different names*

### Comparing `judoscale-1.7.0/judoscale/core/reporter.py` & `judoscale-1.7.1/judoscale/core/reporter.py`

 * *Files identical despite different names*

### Comparing `judoscale-1.7.0/judoscale/django/apps.py` & `judoscale-1.7.1/judoscale/django/apps.py`

 * *Files identical despite different names*

### Comparing `judoscale-1.7.0/judoscale/django/middleware.py` & `judoscale-1.7.1/judoscale/django/middleware.py`

 * *Files identical despite different names*

### Comparing `judoscale-1.7.0/judoscale/django/redis.py` & `judoscale-1.7.1/judoscale/django/redis.py`

 * *Files identical despite different names*

### Comparing `judoscale-1.7.0/judoscale/flask/judoscale.py` & `judoscale-1.7.1/judoscale/flask/judoscale.py`

 * *Files identical despite different names*

### Comparing `judoscale-1.7.0/judoscale/rq/__init__.py` & `judoscale-1.7.1/judoscale/rq/__init__.py`

 * *Files identical despite different names*

### Comparing `judoscale-1.7.0/judoscale/rq/apps.py` & `judoscale-1.7.1/judoscale/rq/apps.py`

 * *Files identical despite different names*

### Comparing `judoscale-1.7.0/judoscale/rq/collector.py` & `judoscale-1.7.1/judoscale/rq/collector.py`

 * *Files identical despite different names*

### Comparing `judoscale-1.7.0/pyproject.toml` & `judoscale-1.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "judoscale"
-version = "1.7.0"
+version = "1.7.1"
 description = "Official Python adapter for Judoscale — the advanced autoscaler for Heroku"
 authors = [
     "Adam McCrea <adam@adamlogic.com>",
     "Mara <mara@multiplace.org>",
     "Karl Sutt <karl@sutt.ee>"
 ]
 license = "MIT"
```

### Comparing `judoscale-1.7.0/setup.py` & `judoscale-1.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 {'celery-redis': ['celery[redis]>=4.4.0,<6.0.0'],
  'django': ['django>=2.1.0,<6.0.0'],
  'flask': ['flask>=1.1.0,<3.0.0'],
  'rq': ['rq>=1.0.0,<2.0.0']}
 
 setup_kwargs = {
     'name': 'judoscale',
-    'version': '1.7.0',
+    'version': '1.7.1',
     'description': 'Official Python adapter for Judoscale — the advanced autoscaler for Heroku',
     'long_description': '# Judoscale\n\nThis is the official Python adapter for [Judoscale](https://elements.heroku.com/addons/judoscale). You can use Judoscale without it, but this gives you request queue time metrics and job queue time (for supported job processors).\n\nIt is recommended to install the specific web framework and/or background job library support as "extras" to the `judoscale` PyPI package. This ensures that checking if the installed web framework and/or background task processing library is supported happens at dependency resolution time.\n\n## Supported web frameworks\n\n- [x] [Django](#using-judoscale-with-django)\n- [x] [Flask](#using-judoscale-with-flask)\n- [x] [FastAPI](#using-judoscale-with-fastapi)\n\n## Supported job processors\n\n- [x] [Celery](#using-judoscale-with-celery-and-redis) (with Redis 6.0+ as the broker)\n- [x] [RQ](#using-judoscale-with-rq)\n\n# Using Judoscale with Django\n\nInstall Judoscale for Django with:\n\n```sh\n$ pip install \'judoscale[django]\'\n```\n\nAdd Judoscale app to `settings.py`:\n\n```python\nINSTALLED_APPS = [\n    "judoscale.django",\n    # ... other apps\n]\n```\n\nThis sets up the Judoscale middleware to capture request queue times.\n\nOptionally, you can customize Judoscale in `settings.py`:\n\n```python\nJUDOSCALE = {\n    # Log level defaults to ENV["LOG_LEVEL"] or "INFO".\n    "LOG_LEVEL": "DEBUG",\n}\n```\n\nOnce deployed, you will see your request queue time metrics available in the Judoscale UI.\n\n# Using Judoscale with Flask\n\nInstall Judoscale for Flask with:\n\n```sh\n$ pip install \'judoscale[flask]\'\n```\n\nThe Flask support for Judoscale is packaged into a Flask extension. Import the extension class and use like you normally would in a Flask application:\n\n```py\n# app.py\n\nfrom judoscale.flask import Judoscale\n\n# If your app is a top-level global\n\napp = Flask("MyFlaskApp")\napp.config.from_object(\'...\')  # or however you configure your app\njudoscale = Judoscale(app)\n\n\n# If your app uses the application factory pattern\n\njudoscale = Judoscale()\n\ndef create_app():\n    app = Flask("MyFlaskApp")\n    app.config.from_object(\'...\')  # or however you configure your app\n    judoscale.init_app(app)\n    return app\n```\n\nThis sets up the Judoscale extension to capture request queue times.\n\nOptionally, you can override Judoscale\'s own configuration via your application\'s [configuration dictionary](https://flask.palletsprojects.com/en/2.2.x/api/#flask.Flask.config). The Judoscale Flask extension looks for a top-level `"JUDOSCALE"` key in `app.config`, which should be a dictionary, and which the extension uses to configure itself as soon as `judoscale.init_app()` is called.\n\n```python\nJUDOSCALE = {\n    # Log level defaults to ENV["LOG_LEVEL"] or "INFO".\n    "LOG_LEVEL": "DEBUG",\n}\n```\n\nNote the [official recommendations for configuring Flask](https://flask.palletsprojects.com/en/2.2.x/config/#configuration-best-practices).\n\n# Using Judoscale with FastAPI\n\nInstall Judoscale for FastAPI with:\n\n```sh\n$ pip install \'judoscale[asgi]\'\n```\n\nSince FastAPI uses [Starlette](https://www.starlette.io/), an ASGI framework, the integration is packaged into [ASGI middleware](https://asgi.readthedocs.io/en/latest/specs/main.html#middleware). Import the middleware class and register it with your FastAPI app:\n\n```py\n# app.py\n\nfrom judoscale.asgi.middleware import FastAPIRequestQueueTimeMiddleware\n\n# If your app is a top-level global\n\napp = FastAPI()\napp.add_middleware(FastAPIRequestQueueTimeMiddleware)\n\n\n# If your app uses the application factory pattern\n\ndef create_app():\n    app = FastAPI()\n    app.add_middleware(FastAPIRequestQueueTimeMiddleware)\n    return app\n```\n\nThis sets up the Judoscale extension to capture request queue times.\n\nOptionally, you can override Judoscale\'s configuration by passing in extra configuration to the `add_middleware` method:\n\n```py\napp.add_middleware(FastAPIRequestQueueTimeMiddleware, extra_config={"LOG_LEVEL": "DEBUG"})\n```\n\n## Other ASGI frameworks\n\nJudoscale also provides middleware classes for Starlette and Quart. You can use them with\n\n```py\n# For Starlette, if you\'re using Starlette directly, without FastAPI\nfrom judoscale.asgi.middleware import StarletteRequestQueueTimeMiddleware\n\n# For Quart\nfrom judoscale.asgi.middleware import QuartRequestQueueTimeMiddleware\n```\n\nIf your app uses a framework for which we have not provided a middleware class, but it implements the [ASGI spec](https://asgi.readthedocs.io/en/latest/specs/index.html), you can easily create your own version of the request queue time middleware.\n\n```py\nfrom judoscale.asgi.middleware import RequestQueueTimeMiddleware\n\nclass YourFrameworkRequestQueueTimeMiddleware(RequestQueueTimeMiddleware):\n    # NOTE: The `platform` class variable value should be the package name\n    # of the web framework you\'re using. It is used to look up package\n    # metadata for reporting back to the Judoscale API.\n    platform = "your_framework"\n```\n\nThen register `YourFrameworkRequestQueueTimeMiddleware` with your application like you normally would.\n\n# Using Judoscale with Celery and Redis\n\nInstall Judoscale for Celery with:\n\n```sh\n$ pip install \'judoscale[celery-redis]\'\n```\n\n> :warning: **NOTE 1:** The Judoscale Celery integration currently only works with the [Redis broker](https://docs.celeryq.dev/en/stable/getting-started/backends-and-brokers/index.html#redis). The minimum supported Redis server version is 6.0.\n\n> :warning: **NOTE 2:** Using [task priorities](https://docs.celeryq.dev/en/latest/userguide/calling.html#advanced-options) is currently not supported by `judoscale`. You can still use task priorities, but `judoscale` won\'t see and report metrics on any queues other than the default, unprioritised queue.\n\nJudoscale can automatically scale the number of Celery workers based on the queue latency (the age of the oldest pending task in the queue).\n\n## Setting up the integration\n\nTo use the Celery integration, import `judoscale_celery` and call it with the Celery app instance. `judoscale_celery` should be called after you have set up and configured the Celery instance.\n\n```py\nfrom celery import Celery\nfrom judoscale.celery import judoscale_celery\n\ncelery_app = Celery(broker="redis://localhost:6379/0")\n# Further setup\n# celery_app.conf.update(...)\n# ...\n\njudoscale_celery(celery_app)\n```\n\nThis sets up Judoscale to periodically calculate and report queue latency for each Celery queue.\n\nIf you need to change the Judoscale integration configuration, you can pass a dictionary of Judoscale configuration options to `judoscale_celery` to override the default Judoscale config variables:\n\n```py\njudoscale_celery(celery_app, extra_config={"LOG_LEVEL": "DEBUG"})\n```\n\nAn example configuration dictionary accepted by `extra_config`:\n\n```py\n{\n    "LOG_LEVEL": "INFO",\n\n    # In addition to global configuration options for the Judoscale\n    # integration above, you can also specify the following configuration\n    # options for the Celery integration.\n    "CELERY": {\n        # Enable (default) or disable the Celery integration\n        "ENABLED": True,\n\n        # Report metrics on up to MAX_QUEUES queues.\n        # The list of discovered queues are sorted by the length\n        # of the queue name (shortest first) and metrics are\n        # reported for the first MAX_QUEUES queues.\n        # Defaults to 20.\n        "MAX_QUEUES": 20,\n\n        # Specify a list of known queues to report metrics for.\n        # MAX_QUEUES is still honoured.\n        # Defaults to empty list (report metrics for discovered queues).\n        "QUEUES": [],\n\n        # Enable or disable (default) tracking how many jobs are currently being\n        # processed in each queue.\n        # This allows Judoscale to avoid downscaling workers that are executing jobs.\n        # See documentation: https://judoscale.com/docs/long-running-jobs-ruby#enable-long-running-job-support-in-the-dashboard\n        # NOTE: This option requires workers to have unique names. If you are running\n        # multiple Celery workers on the same machine, make sure to give each\n        # worker a distinct name.\n        # More information: https://docs.celeryq.dev/en/stable/userguide/workers.html#starting-the-worker\n        "TRACK_BUSY_JOBS": False,\n    }\n}\n```\n\n> :warning: **NOTE:** Calling `judoscale_celery` turns on sending [`task-sent`](https://docs.celeryq.dev/en/stable/userguide/configuration.html#task-send-sent-event) events. This is required for the Celery integration with Judoscale to work.\n\n### Judoscale with Celery and Flask\n\nDepending on how you\'ve structured your Flask app, you should call `judoscale_celery` after your application has finished configuring the Celery app instance. If you have followed the [Flask guide](https://flask.palletsprojects.com/en/2.2.x/patterns/celery/) in the Flask documentation, the easiest place to initialise the Judoscale integration is in the application factory:\n\n```py\ndef create_app():\n    app = Flask(__name__)\n    app.config.from_object(...) # or however you configure your app\n    celery_app = celery_init_app(app)\n    # Initialise the Judoscale integration\n    judoscale_celery(celery_app, extra_config=app.config["JUDOSCALE"])\n    return app\n```\n\n### Judoscale with Celery and Django\n\nIf you have followed the [Django guide](https://docs.celeryq.dev/en/stable/django/first-steps-with-django.html) in the Celery documentation, you should have a module where you initialise the Celery app instance, auto-discover tasks, etc. You should call `judoscale_celery` after you have configured the Celery app instance:\n\n```py\nfrom celery import Celery\nfrom django.conf import settings\nfrom judoscale.celery import judoscale_celery\n\napp = Celery()\napp.config_from_object("django.conf:settings", namespace="CELERY")\napp.autodiscover_tasks()\n# Initialise the Judoscale integration\njudoscale_celery(app, extra_config=settings.JUDOSCALE)\n```\n\n# Using Judoscale with RQ\n\nInstall Judoscale for RQ with:\n\n```sh\n$ pip install \'judoscale[rq]\'\n```\n\nJudoscale can automatically scale the number of RQ workers based on the queue latency (the age of the oldest pending task in the queue).\n\n## Setting up the integration\n\nTo use the RQ integration, import `judoscale_rq` and call it with an instance of `Redis` pointing to the same Redis database that RQ uses.\n\n```py\nfrom redis import Redis\nfrom judoscale.rq import judoscale_rq\n\nredis = Redis(...)\njudoscale_rq(redis)\n```\n\nThis sets up Judoscale to periodically calculate and report queue latency for each RQ queue.\n\nIf you need to change the Judoscale integration configuration, you can pass a dictionary of Judoscale configuration options to `judoscale_rq` to override the default Judoscale config variables:\n\n```py\njudoscale_rq(redis, extra_config={"LOG_LEVEL": "DEBUG"})\n```\n\nAn example configuration dictionary accepted by `extra_config`:\n\n```py\n {\n    "LOG_LEVEL": "INFO",\n\n    # In addition to global configuration options for the Judoscale\n    # integration above, you can also specify the following configuration\n    # options for the RQ integration.\n    "RQ": {\n        # Enable (default) or disable the RQ integration\n        "ENABLED": True,\n\n        # Report metrics on up to MAX_QUEUES queues.\n        # The list of discovered queues are sorted by the length\n        # of the queue name (shortest first) and metrics are\n        # reported for the first MAX_QUEUES queues.\n        # Defaults to 20.\n        "MAX_QUEUES": 20,\n\n        # Specify a list of known queues to report metrics for.\n        # MAX_QUEUES is still honoured.\n        # Defaults to empty list (report metrics for discovered queues).\n        "QUEUES": [],\n\n        # Enable or disable (default) tracking how many jobs are currently being\n        # processed in each queue.\n        # This allows Judoscale to avoid downscaling workers that are executing jobs.\n        # See documentation: https://judoscale.com/docs/long-running-jobs-ruby#enable-long-running-job-support-in-the-dashboard\n        "TRACK_BUSY_JOBS": False,\n}\n```\n\n### Judoscale with RQ and Flask\n\nThe recommended way to initialise Judoscale for RQ is in the application factory:\n\n```py\njudoscale = Judoscale()\n\ndef create_app():\n    app = Flask(__name__)\n    app.config.from_object("...") # or however you configure your application\n    app.redis = Redis()\n\n    # Initialise the Judoscale integration for Flask\n    judoscale.init_app(app)\n\n    # Initialise the Judoscale integration for RQ\n    judoscale_rq(app.redis)\n\n    return app\n```\n\nThen, in your worker script, make sure that you create an app, which will initialise the Judoscale integration with RQ. Although not required, it\'s useful to run the worker within the Flask app context. If you have followed the [RQ on Heroku pattern](https://python-rq.org/patterns/) for setting up your RQ workers on Heroku, your worker script should look something like this:\n\n```py\nfrom rq.worker import HerokuWorker as Worker\n\napp = create_app()\n\nworker = Worker(..., connection=app.redis)\nwith app.app_context():\n    worker.work()\n```\n\nSee the [run-worker.py script](./sample-apps/flask_rq_sample/run-worker.py) for reference.\n\n### Judoscale with RQ and Django\n\nThe Judoscale integration for RQ is packaged into a separate Django app.\n\nYou should already have `judoscale.django` in your `INSTALLED_APPS`. Next, add the RQ integration app `judoscale.rq`:\n\n```python\nINSTALLED_APPS = [\n    "judoscale.django",\n    "judoscale.rq",\n    # ... other apps\n]\n```\n\nBy default, `judoscale.rq` will connect to the Redis instance as specified by the `REDIS_URL` environment variable. If that is not suitable, you can supply Redis connection information in the `JUDOSCALE` configuration dictionary under the `"REDIS"` key.\n\nAccepted formats are:\n\n- a dictionary containing a single key `"URL"` pointing to a Redis server URL, or;\n- a dictionary of configuration options corresponding to the keyword arguments of the [`Redis` constructor](https://github.com/redis/redis-py/blob/6c708c2e0511364c2c3f21fa1259de05e590632d/redis/client.py#L905).\n\n```py\nJUDOSCALE = {\n    # Configuring with a Redis server URL\n    "REDIS": {\n        "URL": os.getenv("REDISTOGO_URL"),\n        "SSL_CERT_REQS": None  # If you are running on Heroku and using Heroku Data for Redis Premium\n    }\n\n    # Configuring as kwargs to Redis(...)\n    "REDIS": {\n        "HOST": "localhost",\n        "PORT": 6379,\n        "DB": 0\n        "SSL_CERT_REQS": None  # If you are running on Heroku and using Heroku Data for Redis Premium\n    }\n}\n```\n\n> :warning: **NOTE:** If you are running on Heroku and using any of the Premium plans for Heroku Data for Redis, you will have to turn off SSL certificate verification as per https://help.heroku.com/HC0F8CUS/redis-connection-issues.\n\nIf you are using [Django-RQ](https://github.com/rq/django-rq/tree/master), you can also pull configuration from `RQ_QUEUES` directly:\n\n```py\nRQ_QUEUES = {\n    "high_priority": {\n        "HOST": "...",\n        "PORT": 6379,\n        "DB": 0\n    },\n}\n\nJUDOSCALE = {\n    # ... other configuration options\n    "REDIS": RQ_QUEUES["high_priority"]\n}\n```\n\n> :warning: **NOTE:** Django-RQ enables configuring RQ such that different queues and workers use _different_ Redis instances. Judoscale currently only supports connecting to and monitoring queue latency on a single Redis instance.\n\n## Debugging & troubleshooting\n\nIf Judoscale is not recognizing your adapter installation or if you\'re not seeing expected metrics in Judoscale, you\'ll want to check the logging output. Here\'s how you\'d do that on Heroku.\n\nFirst, enable debug logging:\n\n```sh\nheroku config:set JUDOSCALE_LOG_LEVEL=debug\n```\n\nThen, tail your logs while your app initializes:\n\n```sh\nheroku logs --tail | grep Judoscale\n```\n\nYou should see Judoscale collecting and reporting metrics every 10 seconds from every running process. If the issue is not clear from the logs, email help@judoscale.com for support. Please include any logging you\'ve collected and any other behavior you\'ve observed.\n\n## Development\n\nThis repo includes a `sample-apps` directory containing apps you can run locally. These apps use the `judoscale` adapter, but they override `API_BASE_URL` so they\'re not connected to the real Judoscale API. Instead, they post API requests to https://requestinspector.com so you can observe the API behavior.\n\nSee the `README` in a sample app for details on how to set it up and run locally.\n\n### Contributing\n\n`judoscale` uses [Poetry](https://python-poetry.org/) for managing dependencies and packaging the project. Head over to the [installations instructions](https://python-poetry.org/docs/#installing-with-the-official-installer) and install Poetry, if needed.\n\nClone the repo with\n\n```sh\n$ git clone git@github.com:judoscale/judoscale-python.git\n$ cd judoscale-python\n```\n\nVerify that you are on a recent version of Poetry:\n\n```sh\n$ poetry --version\nPoetry (version 1.3.1)\n```\n\nInstall dependencies with Poetry and activate the virtualenv\n\n```sh\n$ poetry install --all-extras\n$ poetry shell\n```\n\nRun tests with\n\n```sh\n$ pytest\n```\n',
     'author': 'Adam McCrea',
     'author_email': 'adam@adamlogic.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/judoscale/judoscale-python',
```

### Comparing `judoscale-1.7.0/PKG-INFO` & `judoscale-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: judoscale
-Version: 1.7.0
+Version: 1.7.1
 Summary: Official Python adapter for Judoscale — the advanced autoscaler for Heroku
 Home-page: https://github.com/judoscale/judoscale-python
 License: MIT
 Author: Adam McCrea
 Author-email: adam@adamlogic.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

