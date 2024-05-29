# Comparing `tmp/omdeventhandler-1.0.tar.gz` & `tmp/omdeventhandler-1.1.tar.gz`

## Comparing `omdeventhandler-1.0.tar` & `omdeventhandler-1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rwxr-xr-x   0        0        0     6740 2020-02-02 00:00:00.000000 omdeventhandler-1.0/bin/eventhandler
--rw-r--r--   0        0        0    12437 2020-02-02 00:00:00.000000 omdeventhandler-1.0/src/eventhandler/baseclass.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 omdeventhandler-1.0/src/eventhandler/bash/runner.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 omdeventhandler-1.0/src/eventhandler/default/decider.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 omdeventhandler-1.0/src/eventhandler/nsc_web/runner.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 omdeventhandler-1.0/src/eventhandler/omd_site_self_heal/decider.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 omdeventhandler-1.0/src/eventhandler/ssh/runner.py
--rw-r--r--   0        0        0     6017 2020-02-02 00:00:00.000000 omdeventhandler-1.0/tests/test_classes.py
--rw-r--r--   0        0        0     8552 2020-02-02 00:00:00.000000 omdeventhandler-1.0/tests/test_notify.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 omdeventhandler-1.0/tests/test_package.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 omdeventhandler-1.0/tests/pythonpath/local/lib/python/eventhandler/example/decider.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 omdeventhandler-1.0/tests/pythonpath/local/lib/python/eventhandler/example/runner.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 omdeventhandler-1.0/tests/pythonpath/local/lib/python/notificationforwarder/eventhandler_report/formatter.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 omdeventhandler-1.0/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omdeventhandler-1.0/README.md
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 omdeventhandler-1.0/pyproject.toml
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 omdeventhandler-1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     6741 2020-02-02 00:00:00.000000 omdeventhandler-1.1/bin/eventhandler
+-rw-r--r--   0        0        0    12756 2020-02-02 00:00:00.000000 omdeventhandler-1.1/src/eventhandler/baseclass.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 omdeventhandler-1.1/src/eventhandler/bash/runner.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 omdeventhandler-1.1/src/eventhandler/default/decider.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 omdeventhandler-1.1/src/eventhandler/nsc_web/runner.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 omdeventhandler-1.1/src/eventhandler/omd_site_self_heal/decider.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 omdeventhandler-1.1/src/eventhandler/ssh/runner.py
+-rw-r--r--   0        0        0     6039 2020-02-02 00:00:00.000000 omdeventhandler-1.1/tests/test_classes.py
+-rw-r--r--   0        0        0     8958 2020-02-02 00:00:00.000000 omdeventhandler-1.1/tests/test_notify.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 omdeventhandler-1.1/tests/test_package.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 omdeventhandler-1.1/tests/pythonpath/local/lib/python/eventhandler/example/decider.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 omdeventhandler-1.1/tests/pythonpath/local/lib/python/eventhandler/example/runner.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 omdeventhandler-1.1/tests/pythonpath/local/lib/python/notificationforwarder/eventhandler_report/formatter.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 omdeventhandler-1.1/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omdeventhandler-1.1/README.md
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 omdeventhandler-1.1/pyproject.toml
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 omdeventhandler-1.1/PKG-INFO
```

### Comparing `omdeventhandler-1.0/bin/eventhandler` & `omdeventhandler-1.1/bin/eventhandler`

 * *Files 2% similar despite different names*

```diff
@@ -96,29 +96,29 @@
 the type of backend. Example for VictorOps:
 --forwarderopt company_id=...
 --forwarderopt routing_key=...
 A forwarder is optional. If you use one, then the result of an event handler
 will be sent to the forwarder like an alarm notification.""")
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
-                      version=f'%(prog)%s 1.0')
+                      version=f'%(prog)%s 1.1')
 
     args = parser.parse_args()
     if not any(vars(args).values()):
         parser.print_help()
         parser.exit()
 
     if os.path.exists(os.environ["OMD_ROOT"]+"/var/log/eventhandler.debug"):
```

### Comparing `omdeventhandler-1.0/src/eventhandler/baseclass.py` & `omdeventhandler-1.1/src/eventhandler/baseclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,23 @@
     if debug:
         scrnloglevel = logging.DEBUG
         txtloglevel = logging.DEBUG
     else:
         txtloglevel = logging.INFO
     logger_name = "eventhandler_"+runner_name
 
-    setup_logging(logdir=os.environ["OMD_ROOT"]+"/var/log", logfile=logger_name+".log", scrnloglevel=scrnloglevel, txtloglevel=txtloglevel, format="%(asctime)s %(process)d - %(levelname)s - %(message)s")
+    if "logfile_backups" in runneropts:
+        backup_count = runneropts["logfile_backups"]
+        del runneropts["logfile_backups"]
+    elif "EVENTHANDLER_LOGFILE_BACKUPS" in os.environ:
+        backup_count = os.environ["EVENTHANDLER_LOGFILE_BACKUPS"]
+    else:
+        backup_count = 3
+
+    setup_logging(logdir=os.environ["OMD_ROOT"]+"/var/log", logfile=logger_name+".log", scrnloglevel=scrnloglevel, txtloglevel=txtloglevel, format="%(asctime)s %(process)d - %(levelname)s - %(message)s", backup_count=backup_count)
     logger = logging.getLogger(logger_name)
     try:
         if '.' in target_name:
             module_name, class_name = target_name.rsplit('.', 1)
         else:
             module_name = target_name
             class_name = "".join([x.title() for x in target_name.split("_")])+"Runner"
```

### Comparing `omdeventhandler-1.0/src/eventhandler/default/decider.py` & `omdeventhandler-1.1/src/eventhandler/default/decider.py`

 * *Files identical despite different names*

### Comparing `omdeventhandler-1.0/src/eventhandler/nsc_web/runner.py` & `omdeventhandler-1.1/src/eventhandler/nsc_web/runner.py`

 * *Files identical despite different names*

### Comparing `omdeventhandler-1.0/src/eventhandler/omd_site_self_heal/decider.py` & `omdeventhandler-1.1/src/eventhandler/omd_site_self_heal/decider.py`

 * *Files identical despite different names*

### Comparing `omdeventhandler-1.0/src/eventhandler/ssh/runner.py` & `omdeventhandler-1.1/src/eventhandler/ssh/runner.py`

 * *Files identical despite different names*

### Comparing `omdeventhandler-1.0/tests/test_classes.py` & `omdeventhandler-1.1/tests/test_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         "content": "halo i bims 1 alarm vong naemon her",
         "summary": "samari"+sig,
         "timestamp": time.time(),
     }
     event = eventhandler.baseclass.DecidedEvent(raw_event)
     assert event.eventopts["content"] == "halo i bims 1 alarm vong naemon her"
     dexample.decide_and_prepare(event)
-    assert event.summary == "samari"+sig
+    assert event.summary == "summary is samari"+sig
     assert event.payload["content"] == "halo i bims 1 alarm vong naemon her"
 
 
 def test_example_runner_run_nodiscard_nosummary(setup):
     sig = hashlib.sha256(secrets.token_bytes(32)).hexdigest()
     runneropts = { "path": "/tmp", }
     _setup() # delete logfile
@@ -104,15 +104,15 @@
         "summary": "i bim dem sammari",
         "content": "halo i bims 1 alarm vong naemon her"+sig,
     }
     example = eventhandler.baseclass.new("example", None, "example", True, True,  runneropts)
     example.handle(eventopts)
     log = open(get_logfile(example)).read()
     print("LOG="+log)
-    assert "INFO - i bim dem sammari" in log
+    assert "INFO - summary is i bim dem sammari" in log
     echo = open("/tmp/echo").read()
     assert "halo i bims 1 alarm vong naemon her" in echo
     assert sig in echo
 
 def test_example_runner_run_discard_loud(setup):
     runneropts = { "path": "/tmp", }
     _setup() # delete logfile
```

### Comparing `omdeventhandler-1.0/tests/test_notify.py` & `omdeventhandler-1.1/tests/test_notify.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 omd_root = os.path.dirname(__file__)
 os.environ["OMD_ROOT"] = omd_root
 if not [p for p in sys.path if "pythonpath" in p]:
     sys.path.append(omd_root+"/pythonpath/local/lib/python")
     sys.path.append(omd_root+"/pythonpath/lib/python")
     sys.path.append(omd_root+"/../../notificationforwarder/src")
     os.environ["PYTHONPATH"] = ":".join(sys.path)
+if not [p for p in sys.path if "notificationforwarder" in p]:
+    sys.path.append(omd_root+"/../../notificationforwarder/src")
+    os.environ["PYTHONPATH"] = ":".join(sys.path)
 
 import notificationforwarder.baseclass
 
 
 def _setup():
     omd_root = os.path.dirname(__file__)
     os.environ["OMD_ROOT"] = omd_root
@@ -144,15 +147,17 @@
         --forwarderopt password=i_bims_1_i_bims \\
         --forwardertag evtnot \\
         --formatter eventhandler_report \\
         --eventopt description=i_describe_an_eventhandler \\
         --eventopt signature=no_{} \\
         2>&1 > /tmp/eventhandler_errors.log
     """.format(omd_root, os.environ["OMD_ROOT"]+"/../bin/eventhandler", random_string, random_string)
-    run = subprocess.run(command, capture_output=True, shell=True)
+    # old github pythons cant capture
+    #run = subprocess.run(command, capture_output=True, shell=True)
+    run = subprocess.run(command, shell=True)
     tac = time.time()
     print(run.__dict__) 
     assert run.returncode == 0
     # assert the eventhandler 
     assert os.path.exists("/tmp/123")
     with open("/tmp/123") as f:
         rndstr = f.read().strip()
@@ -198,25 +203,27 @@
         --forwarderopt password=i_bims_1_i_bims \\
         --forwardertag evtnot \\
         --formatter eventhandler_report \\
         --eventopt description=i_describe_an_eventhandler \\
         --eventopt signature=no_{} \\
         2>&1 > /tmp/eventhandler_errors.log
     """.format(omd_root, os.environ["OMD_ROOT"]+"/../bin/eventhandler", random_string, random_string)
-    run = subprocess.run(command, capture_output=True, shell=True)
+    # old github pythons cant capture
+    #run = subprocess.run(command, capture_output=True, shell=True)
+    run = subprocess.run(command, shell=True)
     tac = time.time()
     print(run.__dict__) 
     assert run.returncode == 1
     # assert the eventhandler 
     assert not os.path.exists("/tmp/123")
     assert os.path.exists(omd_root+"/var/log/eventhandler_example_evthdl.log")
     with open(omd_root+"/var/log/eventhandler_example_evthdl.log") as f:
         evtlog = f.read().strip()
     assert "CRITICAL - run failed" in evtlog
-    assert "cannot create /tmp/123/123/123" in evtlog
+    assert "/tmp/123/123/123: No such file or directory" in evtlog or "cannot create /tmp/123/123/123" in evtlog
     # assert the notificationhandler
     assert os.path.exists("/tmp/received_payload.json")
     with open('/tmp/received_payload.json') as f:
         payload = json.load(f)
     assert payload["signature"] == "no_"+random_string
     assert payload["description"] == "i_describe_an_eventhandler"
     assert os.path.exists(omd_root+"/var/log/notificationforwarder_webhook_evtnot.log")
```

### Comparing `omdeventhandler-1.0/tests/pythonpath/local/lib/python/eventhandler/example/decider.py` & `omdeventhandler-1.1/tests/pythonpath/local/lib/python/eventhandler/example/decider.py`

 * *Files identical despite different names*

### Comparing `omdeventhandler-1.0/tests/pythonpath/local/lib/python/notificationforwarder/eventhandler_report/formatter.py` & `omdeventhandler-1.1/tests/pythonpath/local/lib/python/notificationforwarder/eventhandler_report/formatter.py`

 * *Files identical despite different names*

### Comparing `omdeventhandler-1.0/pyproject.toml` & `omdeventhandler-1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 packages = ["src/eventhandler"]
 
 [tool.hatch.build.targets.wheel.force-include]
 "./bin/eventhandler" = "eventhandler/bin_folder/eventhandler"
 
 [project]
 name = "omdeventhandler"
-version = "1.0"
+version = "1.1"
 authors = [
   { name="Gerhard Lausser", email="lausser@yahoo.com" },
 ]
 description = "A framework for event handlers for OMD"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `omdeventhandler-1.0/PKG-INFO` & `omdeventhandler-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: omdeventhandler
-Version: 1.0
+Version: 1.1
 Summary: A framework for event handlers for OMD
 Project-URL: Homepage, https://github.com/lausser/noteventificationforhandlerwarder
 Project-URL: Bug Tracker, https://github.com/lausser/noteventificationforhandlerwarder/issues
 Author-email: Gerhard Lausser <lausser@yahoo.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

