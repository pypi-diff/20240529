# Comparing `tmp/notochord-0.5.3.tar.gz` & `tmp/notochord-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notochord-0.5.3.tar", max compression
+gzip compressed data, was "notochord-0.5.4.tar", max compression
```

## Comparing `notochord-0.5.3.tar` & `notochord-0.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1084 2023-11-28 17:22:02.563723 notochord-0.5.3/LICENSE
--rw-r--r--   0        0        0     5193 2024-05-24 01:09:33.499776 notochord-0.5.3/README.md
--rw-r--r--   0        0        0      854 2024-05-24 01:10:39.153789 notochord-0.5.3/pyproject.toml
--rw-r--r--   0        0        0       87 2023-11-28 17:22:02.566423 notochord-0.5.3/src/notochord/__init__.py
--rw-r--r--   0        0        0     1197 2024-05-24 01:09:33.500220 notochord-0.5.3/src/notochord/__main__.py
--rw-r--r--   0        0        0      163 2023-11-28 17:22:02.566552 notochord-0.5.3/src/notochord/app/__init__.py
--rw-r--r--   0        0        0      316 2023-11-28 17:22:02.566610 notochord-0.5.3/src/notochord/app/harmonizer.css
--rw-r--r--   0        0        0    10522 2023-11-28 17:22:02.566797 notochord-0.5.3/src/notochord/app/harmonizer.py
--rw-r--r--   0        0        0     1870 2024-05-24 01:09:33.500441 notochord-0.5.3/src/notochord/app/homunculus.css
--rw-r--r--   0        0        0    52480 2024-05-24 01:09:33.500982 notochord-0.5.3/src/notochord/app/homunculus.py
--rw-r--r--   0        0        0     3325 2024-05-24 01:09:33.501229 notochord-0.5.3/src/notochord/app/homunculus.toml
--rw-r--r--   0        0        0    18983 2023-11-28 17:22:02.567055 notochord-0.5.3/src/notochord/app/improviser-txala.py
--rw-r--r--   0        0        0      385 2023-11-28 17:22:02.567122 notochord-0.5.3/src/notochord/app/improviser.css
--rw-r--r--   0        0        0    19710 2024-04-24 13:59:31.571434 notochord-0.5.3/src/notochord/app/improviser.py
--rw-r--r--   0        0        0      606 2024-05-24 01:02:59.965896 notochord-0.5.3/src/notochord/app/preset-zeno.toml
--rw-r--r--   0        0        0     4413 2024-05-15 20:23:17.998802 notochord-0.5.3/src/notochord/app/server.py
--rw-r--r--   0        0        0     3073 2023-11-28 17:22:02.567375 notochord-0.5.3/src/notochord/app/simple_harmonizer.py
--rw-r--r--   0        0        0    10631 2024-04-24 13:59:31.572536 notochord-0.5.3/src/notochord/data.py
--rw-r--r--   0        0        0    12790 2023-11-28 17:22:02.567536 notochord-0.5.3/src/notochord/distributions.py
--rw-r--r--   0        0        0    47819 2024-05-24 01:09:33.501721 notochord-0.5.3/src/notochord/model.py
--rw-r--r--   0        0        0    12706 2024-04-24 13:59:31.573908 notochord-0.5.3/src/notochord/perform.py
--rw-r--r--   0        0        0     2528 2023-11-28 17:22:02.567874 notochord-0.5.3/src/notochord/rnn.py
--rw-r--r--   0        0        0    13940 2024-04-24 13:59:31.574327 notochord-0.5.3/src/notochord/train.py
--rw-r--r--   0        0        0     2488 2023-11-28 17:22:02.568040 notochord-0.5.3/src/notochord/util.py
--rw-r--r--   0        0        0     6028 1970-01-01 00:00:00.000000 notochord-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-11-28 17:22:02.563723 notochord-0.5.4/LICENSE
+-rw-r--r--   0        0        0     5193 2024-05-24 01:16:06.116207 notochord-0.5.4/README.md
+-rw-r--r--   0        0        0      854 2024-05-29 15:50:40.830338 notochord-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0       87 2023-11-28 17:22:02.566423 notochord-0.5.4/src/notochord/__init__.py
+-rw-r--r--   0        0        0     1344 2024-05-24 17:06:16.862665 notochord-0.5.4/src/notochord/__main__.py
+-rw-r--r--   0        0        0      206 2024-05-24 17:04:02.068480 notochord-0.5.4/src/notochord/app/__init__.py
+-rw-r--r--   0        0        0      316 2023-11-28 17:22:02.566610 notochord-0.5.4/src/notochord/app/harmonizer.css
+-rw-r--r--   0        0        0    10522 2023-11-28 17:22:02.566797 notochord-0.5.4/src/notochord/app/harmonizer.py
+-rw-r--r--   0        0        0     1870 2024-05-24 01:16:06.116872 notochord-0.5.4/src/notochord/app/homunculus.css
+-rw-r--r--   0        0        0    52480 2024-05-24 01:22:08.455655 notochord-0.5.4/src/notochord/app/homunculus.py
+-rw-r--r--   0        0        0     3325 2024-05-24 01:16:06.117645 notochord-0.5.4/src/notochord/app/homunculus.toml
+-rw-r--r--   0        0        0      385 2023-11-28 17:22:02.567122 notochord-0.5.4/src/notochord/app/improviser.css
+-rw-r--r--   0        0        0    19710 2024-04-24 13:59:31.571434 notochord-0.5.4/src/notochord/app/improviser.py
+-rw-r--r--   0        0        0      606 2024-05-24 01:02:59.965896 notochord-0.5.4/src/notochord/app/preset-zeno.toml
+-rw-r--r--   0        0        0     4413 2024-05-15 20:23:17.998802 notochord-0.5.4/src/notochord/app/server.py
+-rw-r--r--   0        0        0     3073 2023-11-28 17:22:02.567375 notochord-0.5.4/src/notochord/app/simple_harmonizer.py
+-rw-r--r--   0        0        0    19149 2024-05-29 15:47:16.043206 notochord-0.5.4/src/notochord/app/txalaparta.py
+-rw-r--r--   0        0        0    10631 2024-04-24 13:59:31.572536 notochord-0.5.4/src/notochord/data.py
+-rw-r--r--   0        0        0    12790 2023-11-28 17:22:02.567536 notochord-0.5.4/src/notochord/distributions.py
+-rw-r--r--   0        0        0    48080 2024-05-29 15:49:03.736312 notochord-0.5.4/src/notochord/model.py
+-rw-r--r--   0        0        0    12706 2024-04-24 13:59:31.573908 notochord-0.5.4/src/notochord/perform.py
+-rw-r--r--   0        0        0     2528 2023-11-28 17:22:02.567874 notochord-0.5.4/src/notochord/rnn.py
+-rw-r--r--   0        0        0    13940 2024-04-24 13:59:31.574327 notochord-0.5.4/src/notochord/train.py
+-rw-r--r--   0        0        0     2488 2023-11-28 17:22:02.568040 notochord-0.5.4/src/notochord/util.py
+-rw-r--r--   0        0        0     6028 1970-01-01 00:00:00.000000 notochord-0.5.4/PKG-INFO
```

### Comparing `notochord-0.5.3/LICENSE` & `notochord-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `notochord-0.5.3/README.md` & `notochord-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `notochord-0.5.3/pyproject.toml` & `notochord-0.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "notochord"
-version = "0.5.3"
+version = "0.5.4"
 description = "Notochord is a real-time neural network model for MIDI performances."
 authors = ["Victor Shepardson <victor.shepardson@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
```

### Comparing `notochord-0.5.3/src/notochord/__main__.py` & `notochord-0.5.4/src/notochord/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 def help():
     print("""
     available subcommands:
         server: run the Notochord API OSC server
         homunculus: run the Notochord homunculus TUI
         harmonizer: run the Notochord harmonizer TUI
         improviser: run the Notochord improviser TUI
+        txalaparta: run the txalaparta app
         files: show the location of Notochord models and config files on disk
     """)
 
 def _main():
     # print(sys.argv)
     try:
         if sys.argv[1] == 'server':
@@ -26,14 +27,17 @@
             run(homunculus)
         if sys.argv[1] == 'harmonizer':
             sys.argv = sys.argv[1:]
             run(harmonizer)
         if sys.argv[1] == 'improviser':
             sys.argv = sys.argv[1:]
             run(improviser)
+        if sys.argv[1] == 'txalaparta':
+            sys.argv = sys.argv[1:]
+            run(txalaparta)
         if sys.argv[1] == 'files':
             d = Notochord.user_data_dir()
             print(d)
             # os.system(f"open '{d}'")
             subprocess.run(('open', d))
         else:
             help()
```

### Comparing `notochord-0.5.3/src/notochord/app/harmonizer.py` & `notochord-0.5.4/src/notochord/app/harmonizer.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.3/src/notochord/app/homunculus.css` & `notochord-0.5.4/src/notochord/app/homunculus.css`

 * *Files identical despite different names*

### Comparing `notochord-0.5.3/src/notochord/app/homunculus.py` & `notochord-0.5.4/src/notochord/app/homunculus.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.3/src/notochord/app/homunculus.toml` & `notochord-0.5.4/src/notochord/app/homunculus.toml`

 * *Files identical despite different names*

### Comparing `notochord-0.5.3/src/notochord/app/improviser-txala.py` & `notochord-0.5.4/src/notochord/app/txalaparta.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 
 from notochord import Notochord, MIDIConfig, NotoPerformance
 from iipyper import OSC, MIDI, run, Stopwatch, repeat, cleanup, TUI, profile, lock
 
 from rich.panel import Panel
 from rich.pretty import Pretty
 from textual.reactive import reactive
-from textual.widgets import Header, Footer, Static, Button, TextLog
+from textual.widgets import Header, Footer, Static, Button, Log
 
 ### def TUI components ###
-class NotoLog(TextLog):
+class NotoLog(Log):
     value = reactive('')
     def watch_value(self, time: float) -> None:
         self.write(self.value)
 
 class NotoPrediction(Static):
     value = reactive(None)
     def watch_value(self, time: float) -> None:
@@ -56,15 +56,15 @@
         yield NotoLog(id='note')
         yield NotoPrediction(id='prediction')
         yield NotoControl()
         yield Footer()
 ### end def TUI components###
 
 def main(
-    checkpoint="artifacts/noto-txala-011-0020.ckpt", # Notochord checkpoint
+    checkpoint="txala-latest.ckpt", # Notochord checkpoint
     player_config:Dict[int,int]=None, # map MIDI channel : GM instrument
     noto_config:Dict[int,int]=None, # map MIDI channel : GM instrument
     pitch_set=(41,43,45), # MIDI pitches used
 
     initial_mute=False, # start with Notochord muted
     initial_query=False, # let Notochord start playing immediately
 
@@ -93,15 +93,16 @@
 
     osc_port=None, # if supplied, listen for OSC to set controls on this port
     osc_host='', # leave this as empty string to get all traffic on the port
 
     use_tui=True, # run textual UI
     predict_player=True, # forecasted next events can be for player (preserves model distribution, but can lead to Notochord deciding not to play)
     auto_query=True, # query notochord whenever it is unmuted and there is no pending event. generally should be True except for testing purposes.
-    testing=False
+    testing=False,
+    verbose=0
     ):
     """
     Args:
         checkpoint: path to notochord model checkpoint.
 
         player_config: mapping from MIDI channels to MIDI instruments controlled
             by the player.
@@ -248,15 +249,16 @@
         side = int(event['inst']//2)
         if side==state['last_side']:
             state['run_length'] += 1
         else:
             state['run_length'] = 1
 
         state['last_side'] = side
-        print(f'{state["run_length"]=}')
+        if verbose > 0:
+            print(f'{state["run_length"]=}')
 
         # send out as MIDI
         if send:
             midi.send(
                 'note_on' if vel > 0 else 'note_off', 
                 note=event['pitch'], velocity=vel, channel=channel)
 
@@ -305,26 +307,28 @@
     # @lock
     def noto_query(delay=0):
         counts = history.inst_counts(
             n=n_recent, insts=noto_map.insts | player_map.insts)
         # print(counts)
         player_count = sum(counts[i] for i in player_map.insts)
         noto_count = sum(counts[i] for i in noto_map.insts)
-        print(f'player: {player_count}')
-        print(f'noto: {noto_count}')
+        if verbose > 0:
+            print(f'player: {player_count}')
+            print(f'noto: {noto_count}')
         total_count = player_count + noto_count
 
         all_insts = noto_map.insts 
         if predict_player:
             all_insts = all_insts | player_map.insts
 
         steer_time = 1-controls.get('steer_rate', 0.5)
         tqt = (max(0,steer_time-0.5), min(1, steer_time+0.5))
 
-        print(tqt)
+        if verbose > 1:
+            print(tqt)
 
         # if using nominal time,
         # *subtract* estimated feed latency to min_time; (TODO: really should
         #   set no min time when querying, use stopwatch when re-querying...)
         # if using actual time, *add* estimated query latency
         time_offset = -5e-3 if nominal_time else 10e-3
         min_time = stopwatch.read()+time_offset+delay
@@ -342,15 +346,16 @@
             #         insts = player_map.insts
             #     elif noto_count <= player_count - n_margin:
             #         insts = noto_map.insts
 
         if len(insts)==0:
             insts = all_insts
 
-        print(f'{insts=}')
+        if verbose > 1:
+            print(f'{insts=}')
 
         # bal_insts = set(counts.index[counts <= counts.min()+n_margin])
         # if balance_sample and len(bal_insts)>0:
         #     insts = bal_insts
         # else:
         #     insts = all_insts
 
@@ -367,15 +372,16 @@
             # but we sample instrument first
             # under the assumption that the instrument constraint is
             # 'stronger' than the time constraint
             query_method = noto.query_itpv_onsets
 
         max_t = None if max_time is None else max(max_time, min_time+0.2)
 
-        print(min_time, max_t)
+        if verbose > 1:
+            print(min_time, max_t)
 
         pending.event = query_method(
             include_pitch=pitch_set,
             include_inst=list(insts),
             min_time=min_time, max_time=max_t,
             truncate_quantile_time=tqt,
             min_vel=80, max_vel=120,
@@ -415,15 +421,16 @@
         #     controls['steer_pitch'] = msg.value/127
         #     print(f"{controls['steer_pitch']=}")
         # if msg.control==2:
         #     controls['steer_density'] = msg.value/127
         #     print(f"{controls['steer_density']=}")
         if msg.control==3:
             controls['steer_rate'] = msg.value/127
-            print(f"{controls['steer_rate']=}")
+            if verbose > 0:
+                print(f"{controls['steer_rate']=}")
 
         if msg.control==4:
             noto_reset()
         if msg.control==5:
             noto_query()
         if msg.control==6:
             noto_mute()
```

### Comparing `notochord-0.5.3/src/notochord/app/improviser.py` & `notochord-0.5.4/src/notochord/app/improviser.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.3/src/notochord/app/preset-zeno.toml` & `notochord-0.5.4/src/notochord/app/preset-zeno.toml`

 * *Files identical despite different names*

### Comparing `notochord-0.5.3/src/notochord/app/server.py` & `notochord-0.5.4/src/notochord/app/server.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.3/src/notochord/app/simple_harmonizer.py` & `notochord-0.5.4/src/notochord/app/simple_harmonizer.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.3/src/notochord/data.py` & `notochord-0.5.4/src/notochord/data.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.3/src/notochord/distributions.py` & `notochord-0.5.4/src/notochord/distributions.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.3/src/notochord/model.py` & `notochord-0.5.4/src/notochord/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1203,25 +1203,32 @@
         create a Notochord from a checkpoint file containing 
         hyperparameters and model weights.
 
         Args:
             path: file path to Notochord model
         """
         if path=="notochord-latest.ckpt":
+            url = 'https://github.com/Intelligent-Instruments-Lab/iil-python-tools/releases/download/notochord-v0.4.0/notochord_lakh_50G_deep.pt'
+        elif path=="txala-latest.ckpt":
+            url = 'https://github.com/Intelligent-Instruments-Lab/notochord/releases/download/notochord-v0.5.4/noto-txala-011-0020.ckpt'
+        else:
+            url = None
+
+        if url is not None:
             d = Notochord.user_data_dir()
             path = d / path
             # maybe download
             if not path.is_file():
                 while True:
                     answer = input("Do you want to download a notochord model? (y/n)")
                     if answer.lower() in ["y","yes"]:
-                        download_url('https://github.com/Intelligent-Instruments-Lab/iil-python-tools/releases/download/notochord-v0.4.0/notochord_lakh_50G_deep.pt', path)
+                        download_url(url, path)
                         print(f'saved to {path}')
                         break
                     if answer.lower() in ["n","no"]:
                         break
-            # path = 
+        # path = 
         checkpoint = torch.load(path, map_location=torch.device('cpu'))
         model = cls(**checkpoint['kw']['model'])
         model.load_state_dict(checkpoint['model_state'], strict=False)
         return model
```

### Comparing `notochord-0.5.3/src/notochord/perform.py` & `notochord-0.5.4/src/notochord/perform.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.3/src/notochord/rnn.py` & `notochord-0.5.4/src/notochord/rnn.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.3/src/notochord/train.py` & `notochord-0.5.4/src/notochord/train.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.3/src/notochord/util.py` & `notochord-0.5.4/src/notochord/util.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.3/PKG-INFO` & `notochord-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notochord
-Version: 0.5.3
+Version: 0.5.4
 Summary: Notochord is a real-time neural network model for MIDI performances.
 License: MIT
 Author: Victor Shepardson
 Author-email: victor.shepardson@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

