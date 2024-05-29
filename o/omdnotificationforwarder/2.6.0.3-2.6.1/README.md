# Comparing `tmp/omdnotificationforwarder-2.6.0.3.tar.gz` & `tmp/omdnotificationforwarder-2.6.1.tar.gz`

## Comparing `omdnotificationforwarder-2.6.0.3.tar` & `omdnotificationforwarder-2.6.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rwxr-xr-x   0        0        0     3617 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/bin/notificationforwarder
--rw-r--r--   0        0        0    15725 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/src/notificationforwarder/baseclass.py
--rw-r--r--   0        0        0     4786 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/src/notificationforwarder/email/formatter.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/src/notificationforwarder/email/forwarder.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/src/notificationforwarder/example/formatter.py
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/src/notificationforwarder/example/forwarder.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/src/notificationforwarder/rabbitmq/formatter.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/src/notificationforwarder/rabbitmq/forwarder.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/src/notificationforwarder/syslog/formatter.py
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/src/notificationforwarder/syslog/forwarder.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/src/notificationforwarder/telegram/forwarder.py
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/src/notificationforwarder/webhook/forwarder.py
--rw-r--r--   0        0        0     5796 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/test_alertmanager.py
--rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/test_classes.py
--rw-r--r--   0        0        0     6022 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/test_discard.py
--rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/test_formatter.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/test_package.py
--rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/test_paths.py
--rw-r--r--   0        0        0    12014 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/test_webhook.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/pythonpath/lib/python/notificationforwarder/split1/forwarder.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/pythonpath/lib/python/notificationforwarder/split2/formatter.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/pythonpath/lib/python/notificationforwarder/split2/forwarder.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/pythonpath/lib/python/notificationforwarder/split3/formatter.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/pythonpath/lib/python/notificationforwarder/split3/forwarder.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/pythonpath/local/lib/python/notificationforwarder/alertmanager_servicenow/formatter.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/pythonpath/local/lib/python/notificationforwarder/bayern/formatter.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/pythonpath/local/lib/python/notificationforwarder/discard/formatter.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/pythonpath/local/lib/python/notificationforwarder/split1/formatter.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/pythonpath/local/lib/python/notificationforwarder/split2/forwarder.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/pythonpath/local/lib/python/notificationforwarder/split3/formatter.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/pythonpath/local/lib/python/notificationforwarder/split3/forwarder.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/pythonpath/local/lib/python/notificationforwarder/split4/formatter.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/pythonpath/local/lib/python/notificationforwarder/split4/forwarder.py
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/pythonpath/local/lib/python/notificationforwarder/vong/formatter.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/.gitignore
--rw-r--r--   0        0        0    13728 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/README.md
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/pyproject.toml
--rw-r--r--   0        0        0    14517 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0     3616 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/bin/notificationforwarder
+-rw-r--r--   0        0        0    16475 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/src/notificationforwarder/baseclass.py
+-rw-r--r--   0        0        0     4786 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/src/notificationforwarder/email/formatter.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/src/notificationforwarder/email/forwarder.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/src/notificationforwarder/example/formatter.py
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/src/notificationforwarder/example/forwarder.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/src/notificationforwarder/rabbitmq/formatter.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/src/notificationforwarder/rabbitmq/forwarder.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/src/notificationforwarder/syslog/formatter.py
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/src/notificationforwarder/syslog/forwarder.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/src/notificationforwarder/telegram/forwarder.py
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/src/notificationforwarder/webhook/forwarder.py
+-rw-r--r--   0        0        0     5796 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/tests/test_alertmanager.py
+-rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/tests/test_classes.py
+-rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/tests/test_discard.py
+-rw-r--r--   0        0        0     6242 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/tests/test_formatter.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/tests/test_package.py
+-rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/tests/test_paths.py
+-rw-r--r--   0        0        0    12024 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/tests/test_webhook.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/tests/pythonpath/lib/python/notificationforwarder/split1/forwarder.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/tests/pythonpath/lib/python/notificationforwarder/split2/formatter.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/tests/pythonpath/lib/python/notificationforwarder/split2/forwarder.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/tests/pythonpath/lib/python/notificationforwarder/split3/formatter.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/tests/pythonpath/lib/python/notificationforwarder/split3/forwarder.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/tests/pythonpath/local/lib/python/notificationforwarder/alertmanager_servicenow/formatter.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/tests/pythonpath/local/lib/python/notificationforwarder/bayern/formatter.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/tests/pythonpath/local/lib/python/notificationforwarder/discard/formatter.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/tests/pythonpath/local/lib/python/notificationforwarder/split1/formatter.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/tests/pythonpath/local/lib/python/notificationforwarder/split2/forwarder.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/tests/pythonpath/local/lib/python/notificationforwarder/split3/formatter.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/tests/pythonpath/local/lib/python/notificationforwarder/split3/forwarder.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/tests/pythonpath/local/lib/python/notificationforwarder/split4/formatter.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/tests/pythonpath/local/lib/python/notificationforwarder/split4/forwarder.py
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/tests/pythonpath/local/lib/python/notificationforwarder/vong/formatter.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/.gitignore
+-rw-r--r--   0        0        0    14216 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/README.md
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/pyproject.toml
+-rw-r--r--   0        0        0    15003 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.1/PKG-INFO
```

### Comparing `omdnotificationforwarder-2.6.0.3/bin/notificationforwarder` & `omdnotificationforwarder-2.6.1/bin/notificationforwarder`

 * *Files 2% similar despite different names*

```diff
@@ -44,29 +44,29 @@
                       default = {},
                       help="""Receiver attributes. These are specific for
 the type of backend. Example for VictorOps:
 --forwarderopt company_id=...
 --forwarderopt routing_key=...""")
     parser.add_argument('--formatter', action='store', dest="formatter", nargs='?', const=None,
                       help='''The formatter to use for the event...
-                      default is the value of --receiver if not provided''',
+                      default is the value of --forwarder if not provided''',
                       default=argparse.SUPPRESS)
     parser.add_argument('--livestatus', action='store',
                       dest="livestatus",
                       help='The livestatus port')
     parser.add_argument('--verbose', action='store_true',
                       dest="verbose",
                       help='Show logs at stdout',
                       default=False)
     parser.add_argument('--debug', action='store_true',
                       dest="debug",
                       help='Increase the log level to DEBUG',
                       default=False)
     parser.add_argument('--version', action='version',
-                      version=f'%(prog)s 2.6.0.3')
+                      version=f'%(prog)s 2.6.1')
 
     args = parser.parse_args()
     if not hasattr(args, 'formatter'):
         args.formatter = args.forwarder
 
     try:
         forwarder = baseclass.new(args.forwarder, args.forwardertag, args.formatter, args.verbose, args.debug, args.forwarderopt)
```

### Comparing `omdnotificationforwarder-2.6.0.3/src/notificationforwarder/baseclass.py` & `omdnotificationforwarder-2.6.1/src/notificationforwarder/baseclass.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,51 +17,65 @@
 from importlib.util import find_spec, module_from_spec
 
 import sqlite3
 import logging
 from coshsh.util import setup_logging
 
 
-MAXAGE = 5
-
-
 logger = None
 
-def new(target_name, tag, formatter, verbose, debug, receiveropts):
+def new(target_name, tag, formatter, verbose, debug, forwarderopts):
 
     forwarder_name = target_name + ("_"+tag if tag else "")
     if verbose:
         scrnloglevel = logging.INFO
     else:
         scrnloglevel = 100
     if debug:
         scrnloglevel = logging.DEBUG
         txtloglevel = logging.DEBUG
     else:
         txtloglevel = logging.INFO
     logger_name = "notificationforwarder_"+forwarder_name
 
-    setup_logging(logdir=os.environ["OMD_ROOT"]+"/var/log", logfile=logger_name+".log", scrnloglevel=scrnloglevel, txtloglevel=txtloglevel, format="%(asctime)s %(process)d - %(levelname)s - %(message)s")
+    if "logfile_backups" in forwarderopts:
+        backup_count = forwarderopts["logfile_backups"]
+        del forwarderopts["logfile_backups"]
+    elif "NOTIFICATIONFORWARDER_LOGFILE_BACKUPS" in os.environ:
+        backup_count = os.environ["NOTIFICATIONFORWARDER_LOGFILE_BACKUPS"]
+    else:
+        backup_count = 3
+    if "max_spool_minutes" in forwarderopts:
+        max_spool_minutes = forwarderopts["max_spool_minutes"]
+        del forwarderopts["max_spool_minutes"]
+    elif "NOTIFICATIONFORWARDER_MAX_SPOOL_MINUTES" in os.environ:
+        max_spool_minutes = os.environ["NOTIFICATIONFORWARDER_MAX_SPOOL_MINUTES"]
+    else:
+        max_spool_minutes = 5
+
+
+    setup_logging(logdir=os.environ["OMD_ROOT"]+"/var/log", logfile=logger_name+".log", scrnloglevel=scrnloglevel, txtloglevel=txtloglevel, format="%(asctime)s %(process)d - %(levelname)s - %(message)s", backup_count=backup_count)
     logger = logging.getLogger(logger_name)
     try:
         if '.' in target_name:
             module_name, class_name = target_name.rsplit('.', 1)
         else:
             module_name = target_name
             class_name = "".join([x.title() for x in target_name.split("_")])+"Forwarder"
         forwarder_module = import_module('notificationforwarder.'+module_name+'.forwarder', package='notificationforwarder.'+module_name)
         forwarder_class = getattr(forwarder_module, class_name)
 
-        instance = forwarder_class(receiveropts)
+        instance = forwarder_class(forwarderopts)
         instance.__module_file__ = forwarder_module.__file__
         instance.name = target_name
         if tag:
             instance.tag = tag
         instance.forwarder_name = forwarder_name
         instance.formatter_name = formatter
+        instance.max_spool_minutes = max_spool_minutes
         instance.init_paths()
         instance.init_db()
 
         # so we can use logger.info(...) in the single modules
         forwarder_module.logger = logging.getLogger(logger_name)
         base_module = import_module('.baseclass', package='notificationforwarder')
         base_module.logger = logging.getLogger(logger_name)
@@ -265,15 +279,15 @@
                 logger.debug("flush lock set")
                 locked = True
             except IOError as e:
                 logger.debug("flush lock failed: "+str(e))
                 locked = False
             if locked:
                 try:
-                    outdated = int(time.time() - 60*MAXAGE)
+                    outdated = int(time.time() - 60*self.max_spool_minutes)
                     self.dbcurs.execute(sql_delete, (outdated,))
                     dropped = self.dbcurs.rowcount
                     if dropped:
                         logger.info("dropped {} outdated events".format(dropped))
                     last_events_to_flush = 0
                     while True:
                         events_to_flush = self.num_spooled_events()
```

### Comparing `omdnotificationforwarder-2.6.0.3/src/notificationforwarder/email/formatter.py` & `omdnotificationforwarder-2.6.1/src/notificationforwarder/email/formatter.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.3/src/notificationforwarder/email/forwarder.py` & `omdnotificationforwarder-2.6.1/src/notificationforwarder/email/forwarder.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.3/src/notificationforwarder/example/formatter.py` & `omdnotificationforwarder-2.6.1/src/notificationforwarder/example/formatter.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.3/src/notificationforwarder/example/forwarder.py` & `omdnotificationforwarder-2.6.1/src/notificationforwarder/example/forwarder.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.3/src/notificationforwarder/rabbitmq/formatter.py` & `omdnotificationforwarder-2.6.1/src/notificationforwarder/rabbitmq/formatter.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.3/src/notificationforwarder/rabbitmq/forwarder.py` & `omdnotificationforwarder-2.6.1/src/notificationforwarder/rabbitmq/forwarder.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.3/src/notificationforwarder/syslog/formatter.py` & `omdnotificationforwarder-2.6.1/src/notificationforwarder/syslog/formatter.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.3/src/notificationforwarder/syslog/forwarder.py` & `omdnotificationforwarder-2.6.1/src/notificationforwarder/syslog/forwarder.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.3/src/notificationforwarder/telegram/forwarder.py` & `omdnotificationforwarder-2.6.1/src/notificationforwarder/telegram/forwarder.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.3/src/notificationforwarder/webhook/forwarder.py` & `omdnotificationforwarder-2.6.1/src/notificationforwarder/webhook/forwarder.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.3/tests/test_alertmanager.py` & `omdnotificationforwarder-2.6.1/tests/test_alertmanager.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.3/tests/test_classes.py` & `omdnotificationforwarder-2.6.1/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.3/tests/test_discard.py` & `omdnotificationforwarder-2.6.1/tests/test_discard.py`

 * *Files 11% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         "username": "i_bims",
         "password": "dem_is_geheim"
     }
     split3 = notificationforwarder.baseclass.new("split3", None, "discard", True, True,  reveiveropts)
     pythonpath = os.environ["OMD_ROOT"]+"/../src:"+os.environ["OMD_ROOT"]+"/pythonpath/local/lib/python"+":"+os.environ["OMD_ROOT"]+"/pythonpath/lib/python"
     cmd = os.environ["OMD_ROOT"]+"/../bin/notificationforwarder"
     signature = hashlib.sha256(secrets.token_bytes(32)).hexdigest()
-    cmd = "OMD_SITE=my_devel_site OMD_ROOT={} PYTHONPATH={} {} --receiver split3 --receiveropt username=i_bims --receiveropt password=dem_is_geheim --formatter discard --eventopt description='halo i bims 1 alarm vong naemon her' --eventopt signature={} --eventopt was_i_machn_tu=nix".format(omd_root, pythonpath, cmd, signature)
+    cmd = "OMD_SITE=my_devel_site OMD_ROOT={} PYTHONPATH={} {} --forwarder split3 --forwarderopt username=i_bims --forwarderopt password=dem_is_geheim --formatter discard --eventopt description='halo i bims 1 alarm vong naemon her' --eventopt signature={} --eventopt was_i_machn_tu=nix".format(omd_root, pythonpath, cmd, signature)
     subprocess.call(cmd, shell=True)
     log = open(get_logfile(split3)).read()
     assert "forwarder" in log # written by split3 forwarder
     assert "forwarded" in log # written by the baseclass
     assert signature in log
 
 
@@ -64,15 +64,15 @@
         "username": "i_bims",
         "password": "dem_is_geheim"
     }
     split3 = notificationforwarder.baseclass.new("split3", None, "discard", True, True,  reveiveropts)
     pythonpath = os.environ["OMD_ROOT"]+"/../src:"+os.environ["OMD_ROOT"]+"/pythonpath/local/lib/python"+":"+os.environ["OMD_ROOT"]+"/pythonpath/lib/python"
     cmd = os.environ["OMD_ROOT"]+"/../bin/notificationforwarder"
     signature = hashlib.sha256(secrets.token_bytes(32)).hexdigest()
-    cmd = "OMD_SITE=my_devel_site OMD_ROOT={} PYTHONPATH={} {} --receiver split3 --receiveropt username=i_bims --receiveropt password=dem_is_geheim --formatter discard --eventopt description='halo i bims 1 alarm vong naemon her' --eventopt signature={} --eventopt 'was_i_machn_tu=dem maul haltn'".format(omd_root, pythonpath, cmd, signature)
+    cmd = "OMD_SITE=my_devel_site OMD_ROOT={} PYTHONPATH={} {} --forwarder split3 --forwarderopt username=i_bims --forwarderopt password=dem_is_geheim --formatter discard --eventopt description='halo i bims 1 alarm vong naemon her' --eventopt signature={} --eventopt 'was_i_machn_tu=dem maul haltn'".format(omd_root, pythonpath, cmd, signature)
     subprocess.call(cmd, shell=True)
     log = open(get_logfile(split3)).read()
     assert "forwarder" not in log # written by split3 forwarder
     assert "forwarded" not in log # written by the baseclass
     assert "discard" not in log # written by the baseclass
     assert signature not in log
 
@@ -82,15 +82,15 @@
         "username": "i_bims",
         "password": "dem_is_geheim"
     }
     split3 = notificationforwarder.baseclass.new("split3", None, "discard", True, True,  reveiveropts)
     pythonpath = os.environ["OMD_ROOT"]+"/../src:"+os.environ["OMD_ROOT"]+"/pythonpath/local/lib/python"+":"+os.environ["OMD_ROOT"]+"/pythonpath/lib/python"
     cmd = os.environ["OMD_ROOT"]+"/../bin/notificationforwarder"
     signature = hashlib.sha256(secrets.token_bytes(32)).hexdigest()
-    cmd = "OMD_SITE=my_devel_site OMD_ROOT={} PYTHONPATH={} {} --receiver split3 --receiveropt username=i_bims --receiveropt password=dem_is_geheim --formatter discard --eventopt description='halo i bims 1 alarm vong naemon her' --eventopt signature={} --eventopt 'was_i_machn_tu=dem semf dazugebn'".format(omd_root, pythonpath, cmd, signature)
+    cmd = "OMD_SITE=my_devel_site OMD_ROOT={} PYTHONPATH={} {} --forwarder split3 --forwarderopt username=i_bims --forwarderopt password=dem_is_geheim --formatter discard --eventopt description='halo i bims 1 alarm vong naemon her' --eventopt signature={} --eventopt 'was_i_machn_tu=dem semf dazugebn'".format(omd_root, pythonpath, cmd, signature)
     subprocess.call(cmd, shell=True)
     log = open(get_logfile(split3)).read()
     assert "forwarder" not in log # written by split3 forwarder
     assert "forwarded" not in log # written by the baseclass
     assert "discard" in log # written by the baseclass
     assert "dem semf" in log # written by the formatter
     assert signature not in log
@@ -101,15 +101,15 @@
         "username": "i_bims",
         "password": "dem_is_geheim"
     }
     split3 = notificationforwarder.baseclass.new("split3", None, "discard", True, True,  reveiveropts)
     pythonpath = os.environ["OMD_ROOT"]+"/../src:"+os.environ["OMD_ROOT"]+"/pythonpath/local/lib/python"+":"+os.environ["OMD_ROOT"]+"/pythonpath/lib/python"
     cmd = os.environ["OMD_ROOT"]+"/../bin/notificationforwarder"
     signature = hashlib.sha256(secrets.token_bytes(32)).hexdigest()
-    cmd = "OMD_SITE=my_devel_site OMD_ROOT={} PYTHONPATH={} {} --receiver split3 --receiveropt username=i_bims --receiveropt password=dem_is_geheim --formatter discard --eventopt description='halo i bims 1 alarm vong naemon her' --eventopt signature={} --eventopt 'was_i_machn_tu=dem automatischn semf dazugebn'".format(omd_root, pythonpath, cmd, signature)
+    cmd = "OMD_SITE=my_devel_site OMD_ROOT={} PYTHONPATH={} {} --forwarder split3 --forwarderopt username=i_bims --forwarderopt password=dem_is_geheim --formatter discard --eventopt description='halo i bims 1 alarm vong naemon her' --eventopt signature={} --eventopt 'was_i_machn_tu=dem automatischn semf dazugebn'".format(omd_root, pythonpath, cmd, signature)
     subprocess.call(cmd, shell=True)
     log = open(get_logfile(split3)).read()
     assert "forwarder" not in log # written by split3 forwarder
     assert "forwarded" not in log # written by the baseclass
     assert "discard" in log # written by the baseclass
     assert "dem semf" not in log # written by the formatter
     assert signature in log
```

### Comparing `omdnotificationforwarder-2.6.0.3/tests/test_formatter.py` & `omdnotificationforwarder-2.6.1/tests/test_formatter.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,16 +98,16 @@
         "password": "dem_is_geheim"
     }
     split3 = notificationforwarder.baseclass.new("split3", None, "split4", True, True,  reveiveropts)
     # split4 formatter writes "split4_<optional signature>_split4" in the summary
     pythonpath = os.environ["OMD_ROOT"]+"/../src:"+os.environ["OMD_ROOT"]+"/pythonpath/local/lib/python"+":"+os.environ["OMD_ROOT"]+"/pythonpath/lib/python"
     cmd = os.environ["OMD_ROOT"]+"/../bin/notificationforwarder"
     signature = hashlib.sha256(secrets.token_bytes(32)).hexdigest()
-    print("OMD_SITE=my_devel_site OMD_ROOT={} PYTHONPATH={} {} --receiver split3 --receiveropt username=i_bims --receiveropt password=dem_is_geheim --formatter split4 --eventopt description='halo i bims 1 alarm vong naemon her' --eventopt signature={}".format(omd_root, pythonpath, cmd, signature))
-    subprocess.call("OMD_SITE=my_devel_site OMD_ROOT={} PYTHONPATH={} {} --receiver split3 --receiveropt username=i_bims --receiveropt password=dem_is_geheim --formatter split4 --eventopt description='halo i bims 1 alarm vong naemon her' --eventopt signature={}".format(omd_root, pythonpath, cmd, signature), shell=True)
+    print("OMD_SITE=my_devel_site OMD_ROOT={} PYTHONPATH={} {} --forwarder split3 --forwarderopt username=i_bims --forwarderopt password=dem_is_geheim --formatter split4 --eventopt description='halo i bims 1 alarm vong naemon her' --eventopt signature={}".format(omd_root, pythonpath, cmd, signature))
+    subprocess.call("OMD_SITE=my_devel_site OMD_ROOT={} PYTHONPATH={} {} --forwarder split3 --forwarderopt username=i_bims --forwarderopt password=dem_is_geheim --formatter split4 --eventopt description='halo i bims 1 alarm vong naemon her' --eventopt signature={}".format(omd_root, pythonpath, cmd, signature), shell=True)
     log = open(get_logfile(split3)).read()
     assert "split4_"+signature+"_split4" in log
 
 def test_split3_forwarder_split4_formatter_bin(setup):
     # this is used to find out the logfile
     reveiveropts = {
         "username": "i_bims",
```

### Comparing `omdnotificationforwarder-2.6.0.3/tests/test_paths.py` & `omdnotificationforwarder-2.6.1/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.3/tests/test_webhook.py` & `omdnotificationforwarder-2.6.1/tests/test_webhook.py`

 * *Files 3% similar despite different names*

```diff
@@ -224,42 +224,42 @@
         "HOSTNAME": "vongsrv02",
         "HOSTSTATE": "DOWN",
         "NOTIFICATIONTYPE": "PROBLEM",
     }
     webhook = notificationforwarder.baseclass.new("webhook", None, "vong", True, True,  reveiveropts)
     pythonpath = os.environ["OMD_ROOT"]+"/../src:"+os.environ["OMD_ROOT"]+"/pythonpath/local/lib/python"+":"+os.environ["OMD_ROOT"]+"/pythonpath/lib/python"
     cmd = os.environ["OMD_ROOT"]+"/../bin/notificationforwarder"
-    reveiveroptsparams = " ".join(["--receiveropt {}='{}'".format(k, v) for k, v in reveiveropts.items()])
+    reveiveroptsparams = " ".join(["--forwarderopt {}='{}'".format(k, v) for k, v in reveiveropts.items()])
     eventoptsparams = " ".join(["--eventopt {}='{}'".format(k, v) for k, v in eventopts.items()])
-    print("OMD_SITE=my_devel_site OMD_ROOT={} PYTHONPATH={} {} --receiver webhook {} --formatter vong {}".format(omd_root, pythonpath, cmd, reveiveroptsparams, eventoptsparams))
-    subprocess.call("OMD_SITE=my_devel_site OMD_ROOT={} PYTHONPATH={} {} --receiver webhook {} --formatter vong {}".format(omd_root, pythonpath, cmd, reveiveroptsparams, eventoptsparams), shell=True)
+    print("OMD_SITE=my_devel_site OMD_ROOT={} PYTHONPATH={} {} --forwarder webhook {} --formatter vong {}".format(omd_root, pythonpath, cmd, reveiveroptsparams, eventoptsparams))
+    subprocess.call("OMD_SITE=my_devel_site OMD_ROOT={} PYTHONPATH={} {} --forwarder webhook {} --formatter vong {}".format(omd_root, pythonpath, cmd, reveiveroptsparams, eventoptsparams), shell=True)
     log = open(get_logfile(webhook)).read()
     with open("/tmp/received_payload.json") as f:
         payload = f.read()
     payload = json.loads(payload)
     assert payload["host_name"] == "vongsrv02"
 
 def test_forward_webhook_format_vong_bin_token_auth(server_fixture):
-    # auth with token, token is in receiveropts
+    # auth with token, token is in forwarderopts
     reveiveropts = {
         "url": "http://localhost:8080",
         "headers": '{"Authorization": "Bearer i_bims_1_token"}',
     }   
     eventopts = {
         "HOSTNAME": "vongsrv03",
         "HOSTSTATE": "DOWN",
         "NOTIFICATIONTYPE": "PROBLEM",
     }
     webhook = notificationforwarder.baseclass.new("webhook", None, "vong", True, True,  reveiveropts)
     pythonpath = os.environ["OMD_ROOT"]+"/../src:"+os.environ["OMD_ROOT"]+"/pythonpath/local/lib/python"+":"+os.environ["OMD_ROOT"]+"/pythonpath/lib/python"
     cmd = os.environ["OMD_ROOT"]+"/../bin/notificationforwarder"
-    reveiveroptsparams = " ".join(["--receiveropt {}='{}'".format(k, v) for k, v in reveiveropts.items()])
+    reveiveroptsparams = " ".join(["--forwarderopt {}='{}'".format(k, v) for k, v in reveiveropts.items()])
     eventoptsparams = " ".join(["--eventopt {}='{}'".format(k, v) for k, v in eventopts.items()])
-    print("OMD_SITE=my_devel_site OMD_ROOT={} PYTHONPATH={} {} --receiver webhook {} --formatter vong {}".format(omd_root, pythonpath, cmd, reveiveroptsparams, eventoptsparams))
-    subprocess.call("OMD_SITE=my_devel_site OMD_ROOT={} PYTHONPATH={} {} --receiver webhook {} --formatter vong {}".format(omd_root, pythonpath, cmd, reveiveroptsparams, eventoptsparams), shell=True)
+    print("OMD_SITE=my_devel_site OMD_ROOT={} PYTHONPATH={} {} --forwarder webhook {} --formatter vong {}".format(omd_root, pythonpath, cmd, reveiveroptsparams, eventoptsparams))
+    subprocess.call("OMD_SITE=my_devel_site OMD_ROOT={} PYTHONPATH={} {} --forwarder webhook {} --formatter vong {}".format(omd_root, pythonpath, cmd, reveiveroptsparams, eventoptsparams), shell=True)
     #raise
     log = open(get_logfile(webhook)).read()
     with open("/tmp/received_payload.json") as f:
         payload = f.read()
     payload = json.loads(payload)
     assert payload["host_name"] == "vongsrv03"
 
@@ -277,17 +277,17 @@
         # if this key exists, then the formatter fills the header
         # event.forwarderopts["headers"] = '{{"Authorization":
         "dem_is_geheim": "i_bims_1_token",
     }
     webhook = notificationforwarder.baseclass.new("webhook", None, "vong", True, True,  reveiveropts)
     pythonpath = os.environ["OMD_ROOT"]+"/../src:"+os.environ["OMD_ROOT"]+"/pythonpath/local/lib/python"+":"+os.environ["OMD_ROOT"]+"/pythonpath/lib/python"
     cmd = os.environ["OMD_ROOT"]+"/../bin/notificationforwarder"
-    reveiveroptsparams = " ".join(["--receiveropt {}='{}'".format(k, v) for k, v in reveiveropts.items()])
+    reveiveroptsparams = " ".join(["--forwarderopt {}='{}'".format(k, v) for k, v in reveiveropts.items()])
     eventoptsparams = " ".join(["--eventopt {}='{}'".format(k, v) for k, v in eventopts.items()])
-    print("OMD_SITE=my_devel_site OMD_ROOT={} PYTHONPATH={} {} --receiver webhook {} --formatter vong {}".format(omd_root, pythonpath, cmd, reveiveroptsparams, eventoptsparams))
-    subprocess.call("OMD_SITE=my_devel_site OMD_ROOT={} PYTHONPATH={} {} --receiver webhook {} --formatter vong {}".format(omd_root, pythonpath, cmd, reveiveroptsparams, eventoptsparams), shell=True)
+    print("OMD_SITE=my_devel_site OMD_ROOT={} PYTHONPATH={} {} --forwarder webhook {} --formatter vong {}".format(omd_root, pythonpath, cmd, reveiveroptsparams, eventoptsparams))
+    subprocess.call("OMD_SITE=my_devel_site OMD_ROOT={} PYTHONPATH={} {} --forwarder webhook {} --formatter vong {}".format(omd_root, pythonpath, cmd, reveiveroptsparams, eventoptsparams), shell=True)
     log = open(get_logfile(webhook)).read()
     with open("/tmp/received_payload.json") as f:
         payload = f.read()
     payload = json.loads(payload)
     assert payload["host_name"] == "vongsrv04"
```

### Comparing `omdnotificationforwarder-2.6.0.3/tests/pythonpath/local/lib/python/notificationforwarder/alertmanager_servicenow/formatter.py` & `omdnotificationforwarder-2.6.1/tests/pythonpath/local/lib/python/notificationforwarder/alertmanager_servicenow/formatter.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.3/tests/pythonpath/local/lib/python/notificationforwarder/discard/formatter.py` & `omdnotificationforwarder-2.6.1/tests/pythonpath/local/lib/python/notificationforwarder/discard/formatter.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.3/tests/pythonpath/local/lib/python/notificationforwarder/vong/formatter.py` & `omdnotificationforwarder-2.6.1/tests/pythonpath/local/lib/python/notificationforwarder/vong/formatter.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.3/README.md` & `omdnotificationforwarder-2.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,20 @@
         r = requests.head(self.url)
         return r.status_code == 200
 ```
 
 Again, the class name has to be the argument of the *\-\-forwarder* parameter with the first letter in upper case, but this time with "Forwarder" appended. This class must have a method *submit()*, which gets the event object which was supplied with payload and summary in the formatting step. If submit() returns a False value, the framework will spool the event in a database.
 The next time Naemon is executing the notificationforwarder script for this receiver, it will try to submit the events which have been spooled so far. If the Forwarder class has an optional method *probe()*, it will first check if the receiver is now up again before it flushes the spooled events with the *submit()* method.
 
+There are two special *forwarderopt* parameters.
+* \-\-forwarderopt logfile_backups=n  
+  Besides the default logfile *var/log/notificationforwarder_...* there will be n rotated archive files. (Rotation takes place after the logfile reaches 20MB, default is 3 archives)  
+* \-\-forwarderopt max_spool_minutes=n  
+  When submitting an event fails, it will be spooled for n minutes. Within this time re-submitting will be attempted on every call to notificationforwarder. (Default is 5)  
+
 ## Forwarders/Formatters which come with the module
 
 ### WebhookForwarder
 
 This is a generic class, which is used to upload random json payloads (that's why there is no WebhookFormatter as there are so many possibilities) with a POST request to an Api. The parameters it takes are *url*, *username* and *password* for basic auth, *headers* to add to the post request. The latter can be used for token based authentication.
 
 |parameter|description               |default|
```

### Comparing `omdnotificationforwarder-2.6.0.3/pyproject.toml` & `omdnotificationforwarder-2.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 packages = ["src/notificationforwarder"]
 
 [tool.hatch.build.targets.wheel.force-include]
 "./bin/notificationforwarder" = "notificationforwarder/bin_folder/notificationforwarder"
 
 [project]
 name = "omdnotificationforwarder"
-version = "2.6.0.3"
+version = "2.6.1"
 authors = [
   { name="Gerhard Lausser", email="lausser@yahoo.com" },
 ]
 description = "A framework for notification scripts for OMD"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `omdnotificationforwarder-2.6.0.3/PKG-INFO` & `omdnotificationforwarder-2.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: omdnotificationforwarder
-Version: 2.6.0.3
+Version: 2.6.1
 Summary: A framework for notification scripts for OMD
 Project-URL: Homepage, https://github.com/lausser/noteventificationforhandlerwarder
 Project-URL: Bug Tracker, https://github.com/lausser/noteventificationforhandlerwarder/issues
 Author-email: Gerhard Lausser <lausser@yahoo.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -118,14 +118,20 @@
         r = requests.head(self.url)
         return r.status_code == 200
 ```
 
 Again, the class name has to be the argument of the *\-\-forwarder* parameter with the first letter in upper case, but this time with "Forwarder" appended. This class must have a method *submit()*, which gets the event object which was supplied with payload and summary in the formatting step. If submit() returns a False value, the framework will spool the event in a database.
 The next time Naemon is executing the notificationforwarder script for this receiver, it will try to submit the events which have been spooled so far. If the Forwarder class has an optional method *probe()*, it will first check if the receiver is now up again before it flushes the spooled events with the *submit()* method.
 
+There are two special *forwarderopt* parameters.
+* \-\-forwarderopt logfile_backups=n  
+  Besides the default logfile *var/log/notificationforwarder_...* there will be n rotated archive files. (Rotation takes place after the logfile reaches 20MB, default is 3 archives)  
+* \-\-forwarderopt max_spool_minutes=n  
+  When submitting an event fails, it will be spooled for n minutes. Within this time re-submitting will be attempted on every call to notificationforwarder. (Default is 5)  
+
 ## Forwarders/Formatters which come with the module
 
 ### WebhookForwarder
 
 This is a generic class, which is used to upload random json payloads (that's why there is no WebhookFormatter as there are so many possibilities) with a POST request to an Api. The parameters it takes are *url*, *username* and *password* for basic auth, *headers* to add to the post request. The latter can be used for token based authentication.
 
 |parameter|description               |default|
```

