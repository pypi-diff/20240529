# Comparing `tmp/toolforge_jobs_framework_cli-16.0.8.tar.gz` & `tmp/toolforge_jobs_framework_cli-16.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolforge_jobs_framework_cli-16.0.8.tar", last modified: Wed Apr 17 14:06:50 2024, max compression
+gzip compressed data, was "toolforge_jobs_framework_cli-16.0.9.tar", last modified: Wed May 29 02:50:36 2024, max compression
```

## Comparing `toolforge_jobs_framework_cli-16.0.8.tar` & `toolforge_jobs_framework_cli-16.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:06:50.177981 toolforge_jobs_framework_cli-16.0.8/
--rw-rw-rw-   0 root         (0) root         (0)    35120 2024-04-17 14:06:45.000000 toolforge_jobs_framework_cli-16.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      355 2024-04-17 14:06:50.177981 toolforge_jobs_framework_cli-16.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2318 2024-04-17 14:06:45.000000 toolforge_jobs_framework_cli-16.0.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-04-17 14:06:45.000000 toolforge_jobs_framework_cli-16.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 14:06:50.177981 toolforge_jobs_framework_cli-16.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      487 2024-04-17 14:06:45.000000 toolforge_jobs_framework_cli-16.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:06:50.173981 toolforge_jobs_framework_cli-16.0.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2651 2024-04-17 14:06:45.000000 toolforge_jobs_framework_cli-16.0.8/tests/test_api.py
--rw-rw-rw-   0 root         (0) root         (0)    11090 2024-04-17 14:06:45.000000 toolforge_jobs_framework_cli-16.0.8/tests/test_dump.py
--rw-rw-rw-   0 root         (0) root         (0)     6173 2024-04-17 14:06:45.000000 toolforge_jobs_framework_cli-16.0.8/tests/test_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:06:50.173981 toolforge_jobs_framework_cli-16.0.8/tjf_cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 14:06:45.000000 toolforge_jobs_framework_cli-16.0.8/tjf_cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1938 2024-04-17 14:06:45.000000 toolforge_jobs_framework_cli-16.0.8/tjf_cli/api.py
--rw-rw-rw-   0 root         (0) root         (0)    32304 2024-04-17 14:06:45.000000 toolforge_jobs_framework_cli-16.0.8/tjf_cli/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-04-17 14:06:45.000000 toolforge_jobs_framework_cli-16.0.8/tjf_cli/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     3799 2024-04-17 14:06:45.000000 toolforge_jobs_framework_cli-16.0.8/tjf_cli/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:06:50.177981 toolforge_jobs_framework_cli-16.0.8/toolforge_jobs_framework_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      355 2024-04-17 14:06:50.000000 toolforge_jobs_framework_cli-16.0.8/toolforge_jobs_framework_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      499 2024-04-17 14:06:50.000000 toolforge_jobs_framework_cli-16.0.8/toolforge_jobs_framework_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 14:06:50.000000 toolforge_jobs_framework_cli-16.0.8/toolforge_jobs_framework_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2024-04-17 14:06:50.000000 toolforge_jobs_framework_cli-16.0.8/toolforge_jobs_framework_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-04-17 14:06:50.000000 toolforge_jobs_framework_cli-16.0.8/toolforge_jobs_framework_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-17 14:06:50.000000 toolforge_jobs_framework_cli-16.0.8/toolforge_jobs_framework_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:50:36.547014 toolforge_jobs_framework_cli-16.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)    35120 2024-05-29 02:50:32.000000 toolforge_jobs_framework_cli-16.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      355 2024-05-29 02:50:36.547014 toolforge_jobs_framework_cli-16.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2318 2024-05-29 02:50:32.000000 toolforge_jobs_framework_cli-16.0.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-05-29 02:50:32.000000 toolforge_jobs_framework_cli-16.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 02:50:36.547014 toolforge_jobs_framework_cli-16.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      487 2024-05-29 02:50:32.000000 toolforge_jobs_framework_cli-16.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:50:36.547014 toolforge_jobs_framework_cli-16.0.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2651 2024-05-29 02:50:32.000000 toolforge_jobs_framework_cli-16.0.9/tests/test_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    12094 2024-05-29 02:50:32.000000 toolforge_jobs_framework_cli-16.0.9/tests/test_dump.py
+-rw-rw-rw-   0 root         (0) root         (0)     6727 2024-05-29 02:50:32.000000 toolforge_jobs_framework_cli-16.0.9/tests/test_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:50:36.547014 toolforge_jobs_framework_cli-16.0.9/tjf_cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 02:50:32.000000 toolforge_jobs_framework_cli-16.0.9/tjf_cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1938 2024-05-29 02:50:32.000000 toolforge_jobs_framework_cli-16.0.9/tjf_cli/api.py
+-rw-rw-rw-   0 root         (0) root         (0)    32939 2024-05-29 02:50:32.000000 toolforge_jobs_framework_cli-16.0.9/tjf_cli/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-05-29 02:50:32.000000 toolforge_jobs_framework_cli-16.0.9/tjf_cli/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     4119 2024-05-29 02:50:32.000000 toolforge_jobs_framework_cli-16.0.9/tjf_cli/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:50:36.547014 toolforge_jobs_framework_cli-16.0.9/toolforge_jobs_framework_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      355 2024-05-29 02:50:36.000000 toolforge_jobs_framework_cli-16.0.9/toolforge_jobs_framework_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      499 2024-05-29 02:50:36.000000 toolforge_jobs_framework_cli-16.0.9/toolforge_jobs_framework_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 02:50:36.000000 toolforge_jobs_framework_cli-16.0.9/toolforge_jobs_framework_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2024-05-29 02:50:36.000000 toolforge_jobs_framework_cli-16.0.9/toolforge_jobs_framework_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-29 02:50:36.000000 toolforge_jobs_framework_cli-16.0.9/toolforge_jobs_framework_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-29 02:50:36.000000 toolforge_jobs_framework_cli-16.0.9/toolforge_jobs_framework_cli.egg-info/top_level.txt
```

### Comparing `toolforge_jobs_framework_cli-16.0.8/LICENSE` & `toolforge_jobs_framework_cli-16.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `toolforge_jobs_framework_cli-16.0.8/README.md` & `toolforge_jobs_framework_cli-16.0.9/README.md`

 * *Files identical despite different names*

### Comparing `toolforge_jobs_framework_cli-16.0.8/tests/test_api.py` & `toolforge_jobs_framework_cli-16.0.9/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `toolforge_jobs_framework_cli-16.0.8/tests/test_dump.py` & `toolforge_jobs_framework_cli-16.0.9/tests/test_dump.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         "filelog_stderr": "/data/project/tf-test/emails-test.err",
         "status_short": "Running for 1m24s",
         "status_long": "Last run at 2024-03-15T12:47:37Z. Pod in 'Failed' phase. [..]",
         "retry": 0,
         "mount": "all",
         "emails": "all",
         "health_check": None,
+        "port": None,
     },
     "dump_job": {
         "name": "emails-test",
         "command": "./mycommand.sh --argument1",
         "image": "bullseye",
         "emails": "all",
     },
@@ -70,14 +71,15 @@
         "filelog_stderr": "/data/project/tf-test/normal-job-with-custom-retry-policy.err",
         "status_short": "Running for 1m24s",
         "status_long": "Last run at 2024-03-15T12:47:37Z. Pod in 'Failed' phase. [..]",
         "emails": "none",
         "mount": "all",
         "retry": 2,
         "health_check": None,
+        "port": None,
     },
     "dump_job": {
         "name": "normal-job-with-custom-retry-policy",
         "command": "./mycommand.sh --argument1",
         "image": "bullseye",
         "retry": 2,
     },
@@ -94,14 +96,15 @@
         "filelog_stderr": None,
         "status_short": "Running for 1m24s",
         "status_long": "Last run at 2024-03-15T12:47:37Z. Pod in 'Failed' phase. [..]",
         "retry": 0,
         "mount": "all",
         "emails": "none",
         "health_check": None,
+        "port": None,
     },
     "dump_job": {
         "name": "mount-test",
         "command": "./mycommand.sh --argument1",
         "image": "tool-tf-test/tool-tf-test:latest",
         "mount": "all",
     },
@@ -118,14 +121,15 @@
         "filelog_stderr": None,
         "status_short": "Running for 1m24s",
         "status_long": "Last run at 2024-03-15T12:47:37Z. Pod in 'Failed' phase. [..]",
         "retry": 0,
         "mount": "none",
         "emails": "none",
         "health_check": None,
+        "port": None,
     },
     "dump_job": {
         "name": "mount-test",
         "command": "./mycommand.sh --argument1",
         "image": "tool-tf-test/tool-tf-test:latest",
     },
 }
@@ -141,14 +145,15 @@
         "filelog_stderr": None,
         "status_short": "Running for 1m24s",
         "status_long": "Last run at 2024-03-15T12:47:37Z. Pod in 'Failed' phase. [..]",
         "retry": 0,
         "mount": "none",
         "emails": "none",
         "health_check": None,
+        "port": None,
     },
     "dump_job": {
         "name": "filelog-test",
         "command": "./mycommand.sh --argument1",
         "image": "tool-tf-test/tool-tf-test:latest",
         "filelog": "yes",
         "filelog-stdout": "/something",
@@ -166,14 +171,15 @@
         "filelog_stderr": "/something",
         "status_short": "Running for 1m24s",
         "status_long": "Last run at 2024-03-15T12:47:37Z. Pod in 'Failed' phase. [..]",
         "retry": 0,
         "mount": "none",
         "emails": "none",
         "health_check": None,
+        "port": None,
     },
     "dump_job": {
         "name": "filelog-test",
         "command": "./mycommand.sh --argument1",
         "image": "tool-tf-test/tool-tf-test:latest",
         "filelog": "yes",
         "filelog-stderr": "/something",
@@ -191,14 +197,15 @@
         "filelog_stderr": None,
         "status_short": "Running for 1m24s",
         "status_long": "Last run at 2024-03-15T12:47:37Z. Pod in 'Failed' phase. [..]",
         "retry": 0,
         "mount": "none",
         "emails": "none",
         "health_check": None,
+        "port": None,
     },
     "dump_job": {
         "name": "filelog-test",
         "command": "./mycommand.sh --argument1",
         "image": "tool-tf-test/tool-tf-test:latest",
     },
 }
@@ -214,14 +221,15 @@
         "filelog_stderr": None,
         "status_short": "Running for 1m24s",
         "status_long": "Last run at 2024-03-15T12:47:37Z. Pod in 'Failed' phase. [..]",
         "retry": 0,
         "mount": "none",
         "emails": "none",
         "health_check": None,
+        "port": None,
     },
     "dump_job": {
         "name": "filelog-test",
         "command": "./mycommand.sh --argument1",
         "image": "tool-tf-test/tool-tf-test:latest",
         "filelog": "yes",
     },
@@ -238,14 +246,15 @@
         "filelog_stderr": None,
         "status_short": "Running for 1m24s",
         "status_long": "Last run at 2024-03-15T12:47:37Z. Pod in 'Failed' phase. [..]",
         "retry": 0,
         "mount": "all",
         "emails": "none",
         "health_check": None,
+        "port": None,
     },
     "dump_job": {
         "name": "filelog-test",
         "command": "./mycommand.sh --argument1",
         "image": "bookworm",
         "no-filelog": "true",
     },
@@ -263,14 +272,15 @@
         "status_short": "Running for 1m24s",
         "status_long": "Last run at 2024-03-15T12:47:37Z. Pod in 'Failed' phase. [..]",
         "retry": 0,
         "mount": "all",
         "emails": "none",
         "memory": "1G",
         "health_check": None,
+        "port": None,
     },
     "dump_job": {
         "name": "mem",
         "command": "./mycommand.sh --argument1",
         "image": "bookworm",
         "mem": "1G",
     },
@@ -287,14 +297,15 @@
         "filelog_stderr": "$TOOL_DATA_DIR/dir/something.err",
         "status_short": "Running for 1m24s",
         "status_long": "Last run at 2024-03-15T12:47:37Z. Pod in 'Failed' phase. [..]",
         "retry": 0,
         "mount": "all",
         "emails": "none",
         "health_check": None,
+        "port": None,
     },
     "dump_job": {
         "name": "short",
         "command": "./mycommand.sh --argument1",
         "image": "bookworm",
         "filelog-stdout": "dir/something.out",
         "filelog-stderr": "dir/something.err",
@@ -315,24 +326,51 @@
         "retry": 0,
         "mount": "all",
         "emails": "none",
         "health_check": {
             "type": "script",
             "script": "./some-healthcheck-script.sh",
         },
+        "port": None,
     },
     "dump_job": {
         "name": "short",
         "command": "./mycommand.sh --argument1",
         "image": "bookworm",
         "no-filelog": "true",
         "health-check-script": "./some-healthcheck-script.sh",
     },
 }
 
+DumpTestCase_12_port = {
+    "api_job": {
+        "name": "short",
+        "cmd": "./mycommand.sh --argument1",
+        "image": "bookworm",
+        "image_state": "stable",
+        "filelog": None,
+        "filelog_stdout": None,
+        "filelog_stderr": None,
+        "status_short": "Running for 1m24s",
+        "status_long": "Last run at 2024-03-15T12:47:37Z. Pod in 'Failed' phase. [..]",
+        "retry": 0,
+        "mount": "all",
+        "emails": "none",
+        "health_check": None,
+        "port": 8080,
+    },
+    "dump_job": {
+        "name": "short",
+        "command": "./mycommand.sh --argument1",
+        "image": "bookworm",
+        "no-filelog": "true",
+        "port": 8080,
+    },
+}
+
 
 @pytest.mark.parametrize(
     ["testcase"],
     [
         [DumpTestCase_1_emails],
         [DumpTestCase_2_retry],
         [DumpTestCase_3_mount],
@@ -341,13 +379,14 @@
         [DumpTestCase_5_filelog_stderr],
         [DumpTestCase_6_filelog_buildservice],
         [DumpTestCase_7_filelog_buildservice],
         [DumpTestCase_8_filelog_non_buildservice],
         [DumpTestCase_9_memory],
         [DumpTestCase_10_filelog_path_shorten],
         [DumpTestCase_11_healthcheck],
+        [DumpTestCase_12_port],
     ],
 )
 def test_job_prepare_for_dump(mock_tool_account: None, testcase: dict[str, Any]) -> None:
     api_job = testcase["api_job"]
     job_prepare_for_dump(api_job)
     assert api_job == testcase["dump_job"]
```

### Comparing `toolforge_jobs_framework_cli-16.0.8/tests/test_loader.py` & `toolforge_jobs_framework_cli-16.0.9/tests/test_loader.py`

 * *Files 25% similar despite different names*

```diff
@@ -98,84 +98,89 @@
         [
             merge(SIMPLE_TEST_JOB, {"filelog-stderr": "xyz"}),
             merge(SIMPLE_TEST_JOB_API, {"filelog_stderr": "xyz"}),
             True,
         ],
         [merge(SIMPLE_TEST_JOB, {"filelog-stderr": "xyz"}), SIMPLE_TEST_JOB_API, False],
         [SIMPLE_TEST_JOB, merge(SIMPLE_TEST_JOB_API, {"filelog_stderr": "xyz"}), False],
+        # health-check
+        # [
+        #     SIMPLE_TEST_JOB,
+        #     merge(SIMPLE_TEST_JOB_API, {"health_check": None}),
+        #     True,
+        # ],
+        # [merge(SIMPLE_TEST_JOB, {"health-check-script": "/healthcheck.sh"}), SIMPLE_TEST_JOB_API, False],
+        # [
+        #     SIMPLE_TEST_JOB,
+        #     merge(
+        #         SIMPLE_TEST_JOB_API,
+        #         {"health_check": {"type": "script", "script": "/healthcheck.sh"}},
+        #     ),
+        #     False,
+        # ],
+        # [
+        #     merge(SIMPLE_TEST_JOB, {"health-check-script": "/healthcheck.sh"}),
+        #     merge(
+        #         SIMPLE_TEST_JOB_API,
+        #         {"health_check": {"type": "script", "script": "/healthcheck.sh"}},
+        #     ),
+        #     True,
+        # ],
+        # port
+        [SIMPLE_TEST_JOB, merge(SIMPLE_TEST_JOB_API, {"port": None}), True],
+        [merge(SIMPLE_TEST_JOB, {"port": 8080}), SIMPLE_TEST_JOB_API, False],
+        [SIMPLE_TEST_JOB, merge(SIMPLE_TEST_JOB_API, {"port": 8080}), False],
+        [
+            merge(SIMPLE_TEST_JOB, {"port": 8080}),
+            merge(SIMPLE_TEST_JOB_API, {"port": 8080}),
+            True,
+        ],
     ],
 )
 def test_jobs_are_same(config: Dict, api: Dict, expected: bool):
     assert jobs_are_same(job_config=config, job_keys=RUN_ARGS.keys(), api_obj=api) == expected
 
 
 @pytest.mark.parametrize(
-    "jobs_data,filter,add,modify,delete,yaml_warning",
+    "jobs_data,filter,add,modify,yaml_warning",
     [
         # simple cases
-        [[], None, set(), set(), {"test-job"}, False],
-        [[SIMPLE_TEST_JOB], None, set(), set(), set(), False],
+        [[], None, set(), set(), False],
+        [[SIMPLE_TEST_JOB], None, set(), set(), False],
         # job data changes
-        [[merge(SIMPLE_TEST_JOB, {"mem": "2Gi"})], None, set(), {"test-job"}, set(), False],
-        # rename
-        [
-            [merge(SIMPLE_TEST_JOB, {"name": "foobar"})],
-            None,
-            {"foobar"},
-            set(),
-            {"test-job"},
-            False,
-        ],
+        [[merge(SIMPLE_TEST_JOB, {"mem": "2Gi"})], None, set(), {"test-job"}, False],
+        # new job
+        [[merge(SIMPLE_TEST_JOB, {"name": "new-test-job"})], None, {"new-test-job"}, set(), False],
         # configured jobs do not match filter
-        [[SIMPLE_TEST_JOB], lambda s: False, set(), set(), set(), False],
+        [[SIMPLE_TEST_JOB], lambda s: False, set(), set(), False],
         # filter set and matches
-        [[SIMPLE_TEST_JOB], lambda s: True, set(), set(), set(), False],
+        [[SIMPLE_TEST_JOB], lambda s: True, set(), set(), False],
         [
             [merge(SIMPLE_TEST_JOB, {"mem": "2Gi"})],
             lambda s: True,
             set(),
             {"test-job"},
-            set(),
-            False,
-        ],
-        # filter and rename
-        [
-            [merge(SIMPLE_TEST_JOB, {"name": "foobar"})],
-            lambda s: s == "foobar",
-            {"foobar"},
-            set(),
-            set(),
-            False,
-        ],
-        [
-            [merge(SIMPLE_TEST_JOB, {"name": "foobar"})],
-            lambda s: s == "test-job",
-            set(),
-            set(),
-            {"test-job"},
             False,
         ],
         # unknown yaml keys
-        [[merge(SIMPLE_TEST_JOB, {"xyz": "xyz"})], None, set(), set(), set(), True],
+        [[merge(SIMPLE_TEST_JOB, {"xyz": "xyz"})], None, set(), set(), True],
     ],
 )
 def test_calculate_changes(
     caplog,
     mock_api: ToolforgeClient,
     jobs_data: Dict,
     filter: Optional[Callable[[str], bool]],
     add: Set[str],
     modify: Set[str],
-    delete: Set[str],
     yaml_warning,
 ):
     result = calculate_changes(
         conf=mock_api,
         configured_job_data=jobs_data,
         job_keys=RUN_ARGS.keys(),
         filter=filter,
     )
 
     assert result.add == add
     assert result.modify == modify
-    assert result.delete == delete
     assert yaml_warning == ("Unknown key" in caplog.text)
```

### Comparing `toolforge_jobs_framework_cli-16.0.8/tjf_cli/api.py` & `toolforge_jobs_framework_cli-16.0.9/tjf_cli/api.py`

 * *Files identical despite different names*

### Comparing `toolforge_jobs_framework_cli-16.0.8/tjf_cli/cli.py` & `toolforge_jobs_framework_cli-16.0.9/tjf_cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 }
 
 JOB_TABULATION_HEADERS_LONG = {
     "name": "Job name:",
     "cmd": "Command:",
     "type": "Job type:",
     "image": "Image:",
+    "port": "Port:",
     "filelog": "File log:",
     "filelog_stdout": "Output log:",
     "filelog_stderr": "Error log:",
     "emails": "Emails:",
     "resources": "Resources:",
     "mount": "Mounts:",
     "retry": "Retry:",
@@ -196,14 +197,22 @@
         "args": ["--health-check-script"],
         "kwargs": {
             "required": False,
             "default": None,
             "help": "specify a health check command to run on the job if any.",
         },
     },
+    "port": {
+        "args": ["-p", "--port"],
+        "kwargs": {
+            "required": False,
+            "type": int,
+            "help": "specify the port to expose for this job. only valid for continuous jobs",
+        },
+    },
 }
 
 
 @dataclass
 class JobsConfig(Section):
     _NAME_: str = field(default="jobs", init=False)
     jobs_endpoint: str = "/jobs/api/v1"
@@ -395,14 +404,15 @@
     if health_check is not None:
         script = health_check.get("script", None)
         if script:
             job["health_check"] = f"script: {script}"
     else:
         job["health_check"] = "none"
 
+    job["port"] = job.get("port") if job.get("port") else "none"
     mem = job.pop("memory", "default")
     cpu = job.pop("cpu", "default")
     if mem == "default" and cpu == "default":
         job["resources"] = "default"
     else:
         job["resources"] = f"mem: {mem}, cpu: {cpu}"
 
@@ -494,14 +504,15 @@
 
 def op_run(
     api: ToolforgeClient,
     name: str,
     command: str,
     schedule: Optional[str],
     continuous: bool,
+    port: Optional[int],
     image: str,
     wait: int | None,
     filelog: bool | None,
     filelog_stdout: Optional[str],
     filelog_stderr: Optional[str],
     mem: Optional[str],
     cpu: Optional[str],
@@ -520,19 +531,24 @@
         "emails": emails,
         "retry": retry,
         "mount": mount.value,
     }
 
     if continuous and schedule:
         raise TjfCliUserError("Only one of 'continuous' and 'schedule' can be set at the same time")
+    elif port and not continuous:
+        raise TjfCliUserError("--port is only valid for continuous jobs")
     elif continuous:
         payload["continuous"] = True
     elif schedule:
         payload["schedule"] = schedule
 
+    if port:
+        payload["port"] = port
+
     if filelog is not None:
         payload["filelog"] = filelog
     else:
         payload["filelog"] = not _image_is_buildservice(image)
 
     if mount == MountOption.NONE and payload["filelog"]:
         raise TjfCliUserError("Specifying --filelog on a build service image requires --mount=all")
@@ -670,14 +686,15 @@
         raise TjfCliUserError(
             f"Unable to load job number {n}: missing configuration parameter {str(e)}"
         ) from e
 
     # these are optional
     schedule = job.get("schedule", None)
     continuous = job.get("continuous", False)
+    port = job.get("port", None)
 
     filelog = job.get("filelog", None)
     if filelog is None and "no-filelog" in job:
         filelog = not job["no-filelog"]
 
     filelog_stdout = job.get("filelog-stdout", None)
     filelog_stderr = job.get("filelog-stderr", None)
@@ -705,14 +722,15 @@
 
     op_run(
         api=api,
         name=name,
         command=command,
         schedule=schedule,
         continuous=continuous,
+        port=port,
         image=image,
         wait=wait,
         filelog=filelog,
         filelog_stdout=filelog_stdout,
         filelog_stderr=filelog_stderr,
         retry=retry,
         mem=mem,
@@ -737,16 +755,16 @@
     changes = calculate_changes(
         conf=api,
         configured_job_data=jobslist,
         job_keys=RUN_ARGS.keys(),
         filter=filter,
     )
 
-    if len(changes.delete) > 0 or len(changes.modify) > 0:
-        _delete_and_wait(api, {*changes.delete, *changes.modify})
+    if len(changes.modify) > 0:
+        _delete_and_wait(api, {*changes.modify})
 
     for n, job in enumerate(jobslist, start=1):
         if "name" not in job:
             raise TjfCliUserError(
                 f"Unable to load job number {n}: missing configuration parameter name"
             )
 
@@ -888,14 +906,19 @@
         job.pop("retry")
 
     # hide default emails
     emails = job.get("emails")
     if emails == "none":
         job.pop("emails")
 
+    # hide default port
+    port = job.pop("port", None)
+    if port:
+        job["port"] = port
+
     mem = job.get("memory")
     if mem:
         job["mem"] = mem
 
     health_check = job.get("health_check")
     if health_check:
         # not using .get() on purpose to let it break in case of wrong entries
@@ -949,14 +972,15 @@
     elif args.operation == "run":
         op_run(
             api=api,
             name=args.name,
             command=args.command,
             schedule=args.schedule,
             continuous=args.continuous,
+            port=args.port,
             image=args.image,
             wait=args.wait,
             filelog=args.filelog,
             filelog_stdout=args.filelog_stdout,
             filelog_stderr=args.filelog_stderr,
             retry=args.retry,
             mem=args.mem,
```

### Comparing `toolforge_jobs_framework_cli-16.0.8/tjf_cli/errors.py` & `toolforge_jobs_framework_cli-16.0.9/tjf_cli/errors.py`

 * *Files identical despite different names*

### Comparing `toolforge_jobs_framework_cli-16.0.8/tjf_cli/loader.py` & `toolforge_jobs_framework_cli-16.0.9/tjf_cli/loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from toolforge_weld.api_client import ToolforgeClient
 
 LOGGER = getLogger(__name__)
 
 
 @dataclass
 class LoadChanges:
-    delete: Set[str]
     add: Set[str]
     modify: Set[str]
 
 
 def jobs_are_same(job_config: Dict, job_keys: List, api_obj: Dict) -> bool:
     """Determines if a job api object matches its configuration."""
 
@@ -27,14 +26,16 @@
     api_obj["command"] = api_obj["cmd"]
     api_obj["mem"] = api_obj.get("memory", None)
     api_obj["filelog-stdout"] = api_obj.get("filelog_stdout", None)
     api_obj["filelog-stderr"] = api_obj.get("filelog_stderr", None)
 
     # TODO: explicitely setting default CPU/memory should not count as a difference
     dont_evaluate_here = ["name", "emails", "filelog", "no-filelog", "wait", "retry"]
+    # TODO: Investigate and fix bug in health-check-script handling. For now just ignore
+    dont_evaluate_here += ["health-check-script"]
     keys = [k for k in job_keys if k not in dont_evaluate_here]
     for key in keys:
         if api_obj.get(key, None) != job_config.get(key, None):
             LOGGER.debug(
                 "currently existing job %s has different '%s' than the definition",
                 api_obj["name"],
                 key,
@@ -92,18 +93,22 @@
 
     current_job_data = conf.get("/list/")
 
     current_jobs = {
         job["name"]: job for job in current_job_data if not filter or filter(job["name"])
     }
 
-    to_delete = current_jobs.keys() - wanted_jobs.keys()
     to_add = wanted_jobs.keys() - current_jobs.keys()
 
+    # TODO: make it possible to rename a job that is already
+    # running by simply changing the name in the loads.yaml file.
+    # note that this will require each job having some other
+    # immutable unique identifier so we might need to wait on T359650
+
     to_modify = set()
     for job_name, job_data in wanted_jobs.items():
         if job_name in current_jobs and not jobs_are_same(
             job_config=job_data, job_keys=job_keys, api_obj=current_jobs[job_name]
         ):
             to_modify.add(job_name)
 
-    return LoadChanges(to_delete, to_add, to_modify)
+    return LoadChanges(add=to_add, modify=to_modify)
```

