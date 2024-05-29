# Comparing `tmp/browsergym_experiments-0.3.3.tar.gz` & `tmp/browsergym_experiments-0.3.4.tar.gz`

## Comparing `browsergym_experiments-0.3.3.tar` & `browsergym_experiments-0.3.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.3/requirements.txt
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.3/src/browsergym/experiments/__init__.py
--rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.3/src/browsergym/experiments/agent.py
--rw-r--r--   0        0        0    21193 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.3/src/browsergym/experiments/loop.py
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.3/src/browsergym/experiments/utils.py
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.3/tests/test_exp_loop.py
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.3/.gitignore
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.3/README.md
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.4/requirements.txt
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.4/src/browsergym/experiments/__init__.py
+-rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.4/src/browsergym/experiments/agent.py
+-rw-r--r--   0        0        0    24192 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.4/src/browsergym/experiments/loop.py
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.4/src/browsergym/experiments/utils.py
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.4/tests/test_exp_loop.py
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.4/.gitignore
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.4/README.md
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.4/PKG-INFO
```

### Comparing `browsergym_experiments-0.3.3/src/browsergym/experiments/agent.py` & `browsergym_experiments-0.3.4/src/browsergym/experiments/agent.py`

 * *Files identical despite different names*

### Comparing `browsergym_experiments-0.3.3/src/browsergym/experiments/loop.py` & `browsergym_experiments-0.3.4/src/browsergym/experiments/loop.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import gzip
 import json
 import logging
+import os
 import pickle
 import sys
 import time
 import traceback
 import uuid
 from collections import defaultdict
 from dataclasses import dataclass, field, asdict, is_dataclass
@@ -19,14 +20,16 @@
 from tqdm import tqdm
 
 from browsergym.core.chat import Chat
 
 from .agent import Agent
 from .utils import count_messages_token, count_tokens
 
+logger = logging.getLogger(__name__)
+
 
 @dataclass
 class EnvArgs:
     task_name: str
     task_seed: int = None
     max_steps: int = None
     headless: bool = True
@@ -108,15 +111,16 @@
     agent_args: AbstractAgentArgs
     env_args: EnvArgs
     exp_dir: str = None
     exp_name: str = None
     enable_debug: bool = True
     err_msg: str = None
     stack_trace: str = None
-    order: int = None  # use to keep the original order the experiments were meant to be lancuhed.
+    order: int = None  # use to keep the original order the experiments were meant to be launched.
+    logging_level: int = logging.INFO
 
     def prepare(self, exp_root):
         """Prepare the experiment directory and save the experiment arguments.
 
         This enables inspecting experiments that are not run yet.
         """
         if self.env_args.task_seed is None:
@@ -144,57 +148,107 @@
             pickle.dump(self, f)
 
     # TODO distinguish between agent error and environment or system error. e.g.
     # the parsing error of an action should not be re-run.
     def run(self):
         """Run the experiment and save the results"""
 
+        # start writing logs to run logfile
+        self._set_logger()
+
         episode_info = []
         try:
-            logging.info(f"Running experiment {self.exp_name} in:\n  {self.exp_dir}")
+            logger.info(f"Running experiment {self.exp_name} in:\n  {self.exp_dir}")
             agent = self.agent_args.make_agent()
+            logger.debug(f"Agent created.")
             env = self.env_args.make_env(
                 action_mapping=agent.action_set.to_python_code, exp_dir=self.exp_dir
             )
+            logger.debug(f"Environment created.")
 
             err_msg, stack_trace = None, None
             step_info = StepInfo(step=0)
             episode_info = [step_info]
             step_info.from_reset(env, seed=self.env_args.task_seed)
+            logger.debug(f"Environment reset.")
 
             while not step_info.is_done:  # set a limit
+                logger.debug(f"Starting step {step_info.step}.")
                 action = step_info.from_action(agent)
+                logger.debug(f"Agent chose action:\n {action}")
+
                 step_info.save_step_info(self.exp_dir)
+                logger.debug(f"Step info saved.")
                 if action is None:
                     break
 
                 _send_chat_info(env.unwrapped.chat, action, step_info.agent_info)
+                logger.debug(f"Chat info sent.")
 
                 step_info = StepInfo(step=step_info.step + 1)
                 episode_info.append(step_info)
+                logger.debug(f"Sending action to environment.")
                 step_info.from_step(env, action)
+                logger.debug(f"Environment stepped.")
 
         except Exception as e:
             err_msg = f"Exception uncaught by agent or environment in task {self.env_args.task_name}.\n{type(e).__name__}:\n{e}"
             stack_trace = traceback.format_exc()
 
             self.err_msg = err_msg
             self.stack_trace = stack_trace
 
-            logging.warning(err_msg + "\n" + stack_trace)
+            logger.warning(err_msg + "\n" + stack_trace)
             if _is_debugging() and self.enable_debug:
                 raise
 
         finally:
             try:
                 step_info.save_step_info(self.exp_dir)
+            except Exception as e:
+                logger.error(f"Error while saving step info in the finally block: {e}")
+            try:
+                if (
+                    not err_msg
+                    and len(episode_info) > 0
+                    and not (episode_info[-1].terminated or episode_info[-1].truncated)
+                ):
+                    e = KeyboardInterrupt("Early termination??")
+                    err_msg = f"Exception uncaught by agent or environment in task {self.env_args.task_name}.\n{type(e).__name__}:\n{e}"
                 _save_summary_info(episode_info, self.exp_dir, err_msg, stack_trace)
+            except Exception as e:
+                logger.error(f"Error while saving summary info in the finally block: {e}")
+            try:
                 env.close()
             except Exception as e:
-                logging.error(f"Error while finalizing the experiment loop: {e}")
+                logger.error(f"Error while closing the environment in the finally block: {e}")
+            try:
+                self._unset_logger()  # stop writing logs to run logfile
+            except Exception as e:
+                logger.error(f"Error while unsetting the logger in the finally block: {e}")
+
+    def _set_logger(self):
+        # output logging traces to a log file
+        file_handler = logging.FileHandler(self.exp_dir / "experiment.log")
+        file_handler.setLevel(self.logging_level)  # same level as console outputs
+        formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
+        file_handler.setFormatter(formatter)
+        # setup root logger
+        root_logger = logging.getLogger()
+        root_logger.setLevel(self.logging_level)
+        root_logger.addHandler(file_handler)
+        # setup openai logger (don't go below INFO verbosity)
+        openai_logger = logging.getLogger("openai._base_client")
+        openai_logger.setLevel(max(logging.INFO, self.logging_level))
+
+        self.logging_file_handler = file_handler
+
+    def _unset_logger(self):
+        root_logger = logging.getLogger()
+        root_logger.removeHandler(self.logging_file_handler)
 
 
 @dataclass
 class StepTimestamps:
     env_start: float = 0
     action_exec_start: float = 0  # to extract begining of visual action from video
     action_exec_stop: float = 0  # to extract end of visual action from video
@@ -232,29 +286,32 @@
         Extra statistics about the step.
     profiling: StepTimestamps
         Timestamps of the different events during the episode.
     """
 
     step: int = None
     obs: dict = None
-    reward: float = None
-    raw_reward: float = None
+    reward: float = 0
+    raw_reward: float = 0
     terminated: bool = None
     truncated: bool = None
     action: str = None
     agent_info: dict = field(default_factory=dict)
     stats: dict = None
     profiling: StepTimestamps = field(default_factory=StepTimestamps)
+    task_info: dict = None
 
     def from_step(self, env: gym.Env, action: str):
         t = self.profiling
         t.env_start = time.time()
         self.obs, self.reward, self.terminated, self.truncated, env_info = env.step(action)
         t.env_stop = time.time()
 
+        self.task_info = env_info.get("task_info", None)
+
         self.raw_reward = env_info.get("RAW_REWARD_GLOBAL", None)
 
         t.action_exec_start = env_info["action_exec_start"]  # start
         t.action_exect_after_timeout = env_info["action_exec_stop"]
         t.action_exec_stop = env_info["action_exec_stop"] - env_info["action_exec_timeout"]
 
     def from_action(self, agent: Agent):
@@ -424,17 +481,18 @@
     def __init__(self, exp_dir) -> None:
         self.exp_dir = Path(exp_dir)
         self._exp_args = None
         self._steps_info = {}
         self._summary_info = None
         self._screenshots = {}
         self._flat_exp_args = None
+        self._logs = None
 
     @property
-    def exp_args(self):
+    def exp_args(self) -> ExpArgs:
         if self._exp_args is None:
             with open(self.exp_dir / "exp_args.pkl", "rb") as f:
                 self._exp_args = pickle.load(f)
         return self._exp_args
 
     def get_step_info(self, step: int) -> StepInfo:
         """Load the step info from the file and return it."""
@@ -452,14 +510,17 @@
 
         return [self._steps_info[i] for i in range(len(self._steps_info))]
 
     @property
     def summary_info(self) -> dict:
         if self._summary_info is None:
             with open(self.exp_dir / "summary_info.json", "r") as f:
+                # if length is zero raise file not found error
+                if os.fstat(f.fileno()).st_size == 0:
+                    raise FileNotFoundError(f"summary_info.json is empty.")
                 self._summary_info = json.load(f)
         return self._summary_info
 
     def get_screenshot(self, step: int, som=False) -> Image:
         key = (step, som)
         if self._screenshots.get(key, None) is None:
             file_name = f"screenshot_{'som_' if som else ''}step_{step}.jpg"
@@ -514,19 +575,26 @@
         except StopIteration:
             raise FileNotFoundError(f"No task_video found in {self.exp_dir}")
 
     @property
     def combined_video_path(self) -> Path:
         return self.exp_dir / "combined_video.mp4"
 
+    @property
+    def logs(self):
+        if self._logs is None:
+            with open(self.exp_dir / "experiment.log", "r") as f:
+                self._logs = f.read()
+        return self._logs
+
 
 EXP_RESULT_CACHE = {}
 
 
-def get_exp_result(exp_dir):
+def get_exp_result(exp_dir) -> ExpResult:
     """Keep a cache of pre-loaded exp_results for faster loading"""
     exp_dir = str(exp_dir)  # make sure it's not a Path
     exp_result = EXP_RESULT_CACHE.get(exp_dir, None)
     if exp_result is None:
         exp_result = ExpResult(exp_dir)
         EXP_RESULT_CACHE[exp_dir] = exp_result
     return exp_result
@@ -604,15 +672,15 @@
 """
 
     msg += f"""\
 action:
 {action}
 """
 
-    logging.info(msg)
+    logger.info(msg)
     chat.add_message(role="info", msg=msg)
 
 
 def _flatten_dict(d, parent_key="", sep="."):
     """Recursively flatten a nested dictionary."""
     items = []
     for k, v in d.items():
```

### Comparing `browsergym_experiments-0.3.3/src/browsergym/experiments/utils.py` & `browsergym_experiments-0.3.4/src/browsergym/experiments/utils.py`

 * *Files identical despite different names*

### Comparing `browsergym_experiments-0.3.3/tests/test_exp_loop.py` & `browsergym_experiments-0.3.4/tests/test_exp_loop.py`

 * *Files identical despite different names*

### Comparing `browsergym_experiments-0.3.3/.gitignore` & `browsergym_experiments-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `browsergym_experiments-0.3.3/pyproject.toml` & `browsergym_experiments-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `browsergym_experiments-0.3.3/PKG-INFO` & `browsergym_experiments-0.3.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.3
 Name: browsergym-experiments
-Version: 0.3.3
+Version: 0.3.4
 Summary: Experimentation tools for BrowserGym
 Project-URL: homepage, https://github.com/ServiceNow/BrowserGym
 Author: Alex Lacoste, Massimo Caccia, Maxime Gasse, Thibault Le Sellier De Chezelles
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >3.7
-Requires-Dist: browsergym-core==0.3.3
+Requires-Dist: browsergym-core==0.3.4
 Requires-Dist: tiktoken>=0.4
 Description-Content-Type: text/markdown
 
 # BrowserGym experiments
 
 This package provides `browsergym.experiments`, a suite of experimentation tools for [BrowserGym](https://github.com/ServiceNow/BrowserGym).
```

