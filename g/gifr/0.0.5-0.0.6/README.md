# Comparing `tmp/gifr-0.0.5.tar.gz` & `tmp/gifr-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gifr-0.0.5.tar", last modified: Mon May 27 04:38:02 2024, max compression
+gzip compressed data, was "gifr-0.0.6.tar", last modified: Wed May 29 21:33:18 2024, max compression
```

## Comparing `gifr-0.0.5.tar` & `gifr-0.0.6.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-27 04:38:02.045384 gifr-0.0.5/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      637 2024-05-27 04:35:04.000000 gifr-0.0.5/CHANGES.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      430 2024-05-27 04:31:21.000000 gifr-0.0.5/DESCRIPTION.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:44:26.000000 gifr-0.0.5/MANIFEST.in
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1966 2024-05-27 04:38:02.045384 gifr-0.0.5/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    17039 2024-05-27 04:36:31.000000 gifr-0.0.5/README.md
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2024-05-27 04:38:02.045384 gifr-0.0.5/setup.cfg
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1492 2024-05-27 04:35:04.000000 gifr-0.0.5/setup.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-27 04:38:02.045384 gifr-0.0.5/src/
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-27 04:38:02.045384 gifr-0.0.5/src/gifr/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2023-10-30 02:28:46.000000 gifr-0.0.5/src/gifr/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3157 2024-05-27 04:31:32.000000 gifr-0.0.5/src/gifr/asr.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     4138 2023-11-02 03:43:18.000000 gifr-0.0.5/src/gifr/colors.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     7454 2023-11-12 00:01:32.000000 gifr-0.0.5/src/gifr/common.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1255 2023-11-02 03:53:09.000000 gifr-0.0.5/src/gifr/fonts.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     2940 2023-11-12 00:04:23.000000 gifr-0.0.5/src/gifr/image_classification.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6592 2023-11-12 00:04:23.000000 gifr-0.0.5/src/gifr/image_segmentation.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    10904 2023-11-12 00:04:23.000000 gifr-0.0.5/src/gifr/object_detection.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3113 2024-02-15 00:30:01.000000 gifr-0.0.5/src/gifr/text_classification.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     5737 2024-02-27 03:05:43.000000 gifr-0.0.5/src/gifr/text_generation.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-27 04:38:02.045384 gifr-0.0.5/src/gifr.egg-info/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1966 2024-05-27 04:38:01.000000 gifr-0.0.5/src/gifr.egg-info/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      498 2024-05-27 04:38:02.000000 gifr-0.0.5/src/gifr.egg-info/SOURCES.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2024-05-27 04:38:01.000000 gifr-0.0.5/src/gifr.egg-info/dependency_links.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      285 2024-05-27 04:38:01.000000 gifr-0.0.5/src/gifr.egg-info/entry_points.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       24 2024-05-27 04:38:01.000000 gifr-0.0.5/src/gifr.egg-info/requires.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        5 2024-05-27 04:38:01.000000 gifr-0.0.5/src/gifr.egg-info/top_level.txt
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-29 21:33:18.928341 gifr-0.0.6/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      765 2024-05-29 21:32:09.000000 gifr-0.0.6/CHANGES.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      485 2024-05-29 02:45:54.000000 gifr-0.0.6/DESCRIPTION.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:44:26.000000 gifr-0.0.6/MANIFEST.in
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     2205 2024-05-29 21:33:18.928341 gifr-0.0.6/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    21960 2024-05-29 02:43:48.000000 gifr-0.0.6/README.md
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2024-05-29 21:33:18.928341 gifr-0.0.6/setup.cfg
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1558 2024-05-29 21:32:51.000000 gifr-0.0.6/setup.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-29 21:33:18.924341 gifr-0.0.6/src/
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-29 21:33:18.928341 gifr-0.0.6/src/gifr/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2023-10-30 02:28:46.000000 gifr-0.0.6/src/gifr/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3440 2024-05-29 03:00:34.000000 gifr-0.0.6/src/gifr/asr.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     5518 2024-05-29 04:44:31.000000 gifr-0.0.6/src/gifr/asr_text_generation.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     4138 2023-11-02 03:43:18.000000 gifr-0.0.6/src/gifr/colors.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     8402 2024-05-29 02:52:45.000000 gifr-0.0.6/src/gifr/common.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1255 2023-11-02 03:53:09.000000 gifr-0.0.6/src/gifr/fonts.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     2940 2023-11-12 00:04:23.000000 gifr-0.0.6/src/gifr/image_classification.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6592 2023-11-12 00:04:23.000000 gifr-0.0.6/src/gifr/image_segmentation.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    10904 2023-11-12 00:04:23.000000 gifr-0.0.6/src/gifr/object_detection.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3113 2024-02-15 00:30:01.000000 gifr-0.0.6/src/gifr/text_classification.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6011 2024-05-29 03:00:34.000000 gifr-0.0.6/src/gifr/text_generation.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-29 21:33:18.928341 gifr-0.0.6/src/gifr.egg-info/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     2205 2024-05-29 21:33:18.000000 gifr-0.0.6/src/gifr.egg-info/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      530 2024-05-29 21:33:18.000000 gifr-0.0.6/src/gifr.egg-info/SOURCES.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2024-05-29 21:33:18.000000 gifr-0.0.6/src/gifr.egg-info/dependency_links.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      338 2024-05-29 21:33:18.000000 gifr-0.0.6/src/gifr.egg-info/entry_points.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       24 2024-05-29 21:33:18.000000 gifr-0.0.6/src/gifr.egg-info/requires.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        5 2024-05-29 21:33:18.000000 gifr-0.0.6/src/gifr.egg-info/top_level.txt
```

### Comparing `gifr-0.0.5/CHANGES.rst` & `gifr-0.0.6/CHANGES.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+0.0.6 (2024-05-30)
+------------------
+
+- added interface for automatic speech recognition (ASR) combined with text generation
+
+
 0.0.5 (2024-05-27)
 ------------------
 
 - added interface for automatic speech recognition (ASR)
 
 
 0.0.4 (2024-02-27)
```

### Comparing `gifr-0.0.5/PKG-INFO` & `gifr-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 Metadata-Version: 1.1
 Name: gifr
-Version: 0.0.5
+Version: 0.0.6
 Summary: gradio interfaces for Deep Learning Docker images that use Redis for receiving data to make predictions on.
 Home-page: https://github.com/waikato-datamining/gifr
 Author: Peter Reutemann
 Author-email: fracpete@waikato.ac.nz
 License: MIT License
 Description: `gradio <https://www.gradio.app/>`__ interfaces for Deep Learning Docker images that
         use Redis for receiving data to make predictions on.
         
         `https://www.data-mining.co.nz/docker-images/ <https://www.data-mining.co.nz/docker-images/>`__
         
         Interfaces are available for:
         
         - automatic speech recognition (ASR)
+        - automatic speech recognition (ASR) + text generation
         - image classification
         - image segmentation
         - object detection/instance segmentation
         - text classification
         - text generation
         
         
         Changelog
         =========
         
+        0.0.6 (2024-05-30)
+        ------------------
+        
+        - added interface for automatic speech recognition (ASR) combined with text generation
+        
+        
         0.0.5 (2024-05-27)
         ------------------
         
         - added interface for automatic speech recognition (ASR)
         
         
         0.0.4 (2024-02-27)
```

### Comparing `gifr-0.0.5/README.md` & `gifr-0.0.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -39,16 +39,16 @@
 ```
 usage: gifr-asr [-h] [--redis_host HOST] [--redis_port PORT] [--redis_db DB]
                 [--model_channel_in CHANNEL] [--model_channel_out CHANNEL]
                 [--timeout SECONDS] [--title TITLE] [--description DESC]
                 [--launch_browser] [--share_interface]
                 [--logging_level {DEBUG,INFO,WARN,ERROR,CRITICAL}]
 
-Automatic Speech Recognition (ASR) interface. Allows the user to enter text
-and display the text transcribed by the model.
+Automatic Speech Recognition (ASR) interface. Allows the user to record/upload
+audio and display the text transcribed by the model.
 
 optional arguments:
   -h, --help            show this help message and exit
   --redis_host HOST     The host with the redis server. (default: localhost)
   --redis_port PORT     The port of the redis server. (default: 6379)
   --redis_db DB         The redis database to use. (default: 0)
   --model_channel_in CHANNEL
@@ -68,14 +68,103 @@
                         tab of the default browser. (default: False)
   --share_interface     Whether to publicly share the interface at
                         https://XYZ.gradio.live/. (default: False)
   --logging_level {DEBUG,INFO,WARN,ERROR,CRITICAL}
                         The logging level to use (default: WARN)
 ```
 
+### Automatic Speech Recognition (ASR) + Text generation
+
+![Screenshot automatic speech recognition with text generation](doc/img/asr_textgen.png)
+
+```
+usage: gifr-textgen [-h] [--redis_host HOST] [--redis_port PORT]
+                    [--redis_db DB] [--model_channel_in CHANNEL]
+                    [--model_channel_out CHANNEL] [--sleep_time SECONDS]
+                    [--timeout SECONDS] [--title TITLE] [--description DESC]
+                    [--launch_browser] [--share_interface]
+                    [--logging_level {DEBUG,INFO,WARN,ERROR,CRITICAL}]
+                    [--audio_channel_in CHANNEL] [--audio_channel_out CHANNEL]
+                    [--text_channel_in CHANNEL] [--text_channel_out CHANNEL]
+                    [--send_text FIELD] [--json_response]
+                    [--receive_prediction FIELD] [--history_on]
+                    [--send_history FIELD] [--send_turns FIELD]
+                    [--receive_history FIELD] [--receive_turns FIELD]
+                    [--clean_response]
+
+Combined Automatic Speech Recognition (ASR) and text generation interface.
+Allows the user to record/upload audio, which gets transcribed and the
+transcription fed into the text generation model. The generated text is then
+displayed.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --redis_host HOST     The host with the redis server. (default: localhost)
+  --redis_port PORT     The port of the redis server. (default: 6379)
+  --redis_db DB         The redis database to use. (default: 0)
+  --model_channel_in CHANNEL
+                        The channel to send the data to for making
+                        predictions. (default: model_channel_in)
+  --model_channel_out CHANNEL
+                        The channel to receive the predictions on. (default:
+                        model_channel_out)
+  --sleep_time SECONDS  The sleep time in seconds for the pub-sub thread.
+                        (default: 0.01)
+  --timeout SECONDS     The number of seconds to wait for a response.
+                        (default: 1.0)
+  --title TITLE         The title to use for interface. (default: ASR+Text
+                        generation)
+  --description DESC    The description to use in the interface. (default:
+                        First transcribes the recorded/uploaded audio and then
+                        sends the transcript to the model to complete and
+                        displays the result.)
+  --launch_browser      Whether to automatically launch the interface in a new
+                        tab of the default browser. (default: False)
+  --share_interface     Whether to publicly share the interface at
+                        https://XYZ.gradio.live/. (default: False)
+  --logging_level {DEBUG,INFO,WARN,ERROR,CRITICAL}
+                        The logging level to use (default: WARN)
+  --audio_channel_in CHANNEL
+                        The channel to send the audio to for transcribing.
+                        (default: audio)
+  --audio_channel_out CHANNEL
+                        The channel to receive the transcriptions on.
+                        (default: transcription)
+  --text_channel_in CHANNEL
+                        The channel to send the text to for making
+                        predictions. (default: text)
+  --text_channel_out CHANNEL
+                        The channel to receive the text predictions on.
+                        (default: prediction)
+  --send_text FIELD     The field name in the JSON prompt used for sending the
+                        text, ignored if not provided. (default: prompt)
+  --json_response       Whether the reponse is a JSON object. (default: False)
+  --receive_prediction FIELD
+                        The field name in the JSON response used for receiving
+                        the predicted text, ignored if not provided. (default:
+                        text)
+  --history_on          Whether to keep track of the interactions. (default:
+                        False)
+  --send_history FIELD  The field name in the JSON query to use for sending
+                        the input history, ignored if not provided. (default:
+                        None)
+  --send_turns FIELD    The field name in the JSON query to use for sending
+                        the number of turns in the interaction, ignored if not
+                        provided. (default: None)
+  --receive_history FIELD
+                        The field name in the JSON response used for receiving
+                        the input history, ignored if not provided. (default:
+                        None)
+  --receive_turns FIELD
+                        The field name in the JSON response used for receiving
+                        the number of turns in the interaction, ignored if not
+                        provided. (default: None)
+  --clean_response      Whether to clean up the response. (default: False)
+```
+
 ### Image classification
 
 ![Screenshot image classification](doc/img/imgcls.png)
 
 ```
 usage: gifr-imgcls [-h] [--redis_host HOST] [--redis_port PORT]
                    [--redis_db DB] [--model_channel_in CHANNEL]
```

### Comparing `gifr-0.0.5/setup.py` & `gifr-0.0.6/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -32,20 +32,21 @@
     packages=find_namespace_packages(where='src'),
     install_requires=[
         "gradio",
         "redis",
         "opex",
         "scipy",
     ],
-    version="0.0.5",
+    version="0.0.6",
     author='Peter Reutemann',
     author_email='fracpete@waikato.ac.nz',
     entry_points={
         "console_scripts": [
             "gifr-asr=gifr.asr:sys_main",
+            "gifr-asr-textgen=gifr.asr_text_generation:sys_main",
             "gifr-imgcls=gifr.image_classification:sys_main",
             "gifr-imgseg=gifr.image_segmentation:sys_main",
             "gifr-objdet=gifr.object_detection:sys_main",
             "gifr-textclass=gifr.text_classification:sys_main",
             "gifr-textgen=gifr.text_generation:sys_main",
         ],
     },
```

### Comparing `gifr-0.0.5/src/gifr/asr.py` & `gifr-0.0.6/src/gifr/asr.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,35 +12,39 @@
 PROG: str = "gifr-asr"
 
 _logger = logging.getLogger(PROG)
 
 state: State = None
 
 
-def predict(audio) -> str:
+def predict(audio, channel_out: str = None, channel_in: str = None) -> str:
     """
     Sends the audio file to the model and returns the transcribed text.
 
     :param audio: the audio file to send
     :type audio: str
+    :param channel_out: for overriding the state's out channel
+    :type channel_out: str
+    :param channel_in: for overriding the state's in channel
+    :type channel_in: str
     :return: the transcription result
     :rtype: str
     """
     global state
 
     sr, y = audio
     y = y.astype(np.float32)
     y /= np.max(np.abs(y))
     buf = io.BytesIO()
     write(buf, sr, y)
 
     state.logger.info("Transcribing...")
 
     # perform query
-    result = make_prediction(state, buf.getvalue())
+    result = make_prediction(state, buf.getvalue(), channel_in=channel_in, channel_out=channel_out)
 
     # parse response
     if result is None:
         result = "no result"
     else:
         try:
             result = result.decode()
@@ -87,15 +91,15 @@
     The main method for parsing command-line arguments.
 
     :param args: the commandline arguments, uses sys.argv if not supplied
     :type args: list
     """
     global state
     init_logging()
-    parser = create_parser("Automatic Speech Recognition (ASR) interface. Allows the user to enter text "
+    parser = create_parser("Automatic Speech Recognition (ASR) interface. Allows the user to record/upload audio "
                            + "and display the text transcribed by the model.",
                            PROG, model_channel_in="audio", model_channel_out="transcription",
                            timeout=2.0, ui_title="Automatic Speech Recognition (ASR)",
                            ui_desc="Sends the recorded/uploaded audio to the model to transcribe and displays the result.")
     parsed = parser.parse_args(args=args)
     set_logging_level(_logger, parsed.logging_level)
     state = init_state(parsed)
```

### Comparing `gifr-0.0.5/src/gifr/colors.py` & `gifr-0.0.6/src/gifr/colors.py`

 * *Files identical despite different names*

### Comparing `gifr-0.0.5/src/gifr/common.py` & `gifr-0.0.6/src/gifr/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,19 +25,20 @@
 """ environment variable for the global default logging level. """
 
 
 @dataclass
 class State:
     connection: redis.Redis = None
     pubsub = None
-    channel_out: str = "redis_in"
-    channel_in: str = "redis_out"
+    channel_out: str = None
+    channel_in: str = None
     timeout: float = 5.0
     title: str = "gifr"
     description: str = ""
+    sleep_time: float = 0.01
     data = None
     logger: logging.Logger = None
     params: dict = field(default_factory=dict)
 
 
 def str_to_logging_level(level: str) -> int:
     """
@@ -84,47 +85,52 @@
     :type level: str
     """
     logger.setLevel(str_to_logging_level(level))
 
 
 def create_parser(description: str, prog: str, host: str = "localhost", port: int = 6379, db: int = 0,
                   model_channel_in: str = "model_channel_in", model_channel_out: str = "model_channel_out",
-                  timeout: float = 5.0, ui_title: str = "gifr", ui_desc: str = "") -> argparse.ArgumentParser:
+                  timeout: float = 5.0, ui_title: str = "gifr", ui_desc: str = "", sleep_time: float = 0.01) -> argparse.ArgumentParser:
     """
     Creates a base parser with options for redis.
 
     :param description: the description of the program
     :type description: str
     :param prog: the command-line program
     :type prog: str
     :param host: the default redis host
     :type host: str
     :param port: the default redis port
     :type port: int
     :param db: the redis database to use
     :type db: int
-    :param model_channel_in: the redis channel to send the data to for making predictions
+    :param model_channel_in: the redis channel to send the data to for making predictions, skips adding parameter if None
     :type model_channel_in: str
-    :param model_channel_out: the redis channel to receive the predictions on
+    :param model_channel_out: the redis channel to receive the predictions on, skips adding parameter if None
     :type model_channel_out: str
     :param timeout: the number of seconds to wait for a prediction
     :type timeout: float
     :param ui_title: the title to use for the interface
     :type ui_title: str
     :param ui_desc: the description to use in the interface
     :type ui_desc: str
+    :param sleep_time: the sleep time for the pubsub thread
+    :type sleep_time: float
     """
     parser = argparse.ArgumentParser(
         description=description, prog=prog, formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument("--redis_host", metavar="HOST", help="The host with the redis server.", default=host, type=str, required=False)
     parser.add_argument("--redis_port", metavar="PORT", help="The port of the redis server.", default=port, type=int, required=False)
     parser.add_argument("--redis_db", metavar="DB", help="The redis database to use.", default=db, type=int, required=False)
-    parser.add_argument("--model_channel_in", metavar="CHANNEL", help="The channel to send the data to for making predictions.", default=model_channel_in, type=str, required=False)
-    parser.add_argument("--model_channel_out", metavar="CHANNEL", help="The channel to receive the predictions on.", default=model_channel_out, type=str, required=False)
-    parser.add_argument("--timeout", metavar="SECONDS", help="The number of seconds to wait for a prediction.", default=timeout, type=float, required=False)
+    if model_channel_in is not None:
+        parser.add_argument("--model_channel_in", metavar="CHANNEL", help="The channel to send the data to for making predictions.", default=model_channel_in, type=str, required=False)
+    if model_channel_out is not None:
+        parser.add_argument("--model_channel_out", metavar="CHANNEL", help="The channel to receive the predictions on.", default=model_channel_out, type=str, required=False)
+    parser.add_argument("--sleep_time", metavar="SECONDS", help="The sleep time in seconds for the pub-sub thread.", default=sleep_time, type=float, required=False)
+    parser.add_argument("--timeout", metavar="SECONDS", help="The number of seconds to wait for a response.", default=timeout, type=float, required=False)
     parser.add_argument("--title", metavar="TITLE", help="The title to use for interface.", default=ui_title, type=str, required=False)
     parser.add_argument("--description", metavar="DESC", help="The description to use in the interface.", default=ui_desc, type=str, required=False)
     parser.add_argument("--launch_browser", action="store_true", help="Whether to automatically launch the interface in a new tab of the default browser.")
     parser.add_argument("--share_interface", action="store_true", help="Whether to publicly share the interface at https://XYZ.gradio.live/.")
     parser.add_argument("--logging_level", choices=LOGGING_LEVELS, default=LOGGING_WARN, help="The logging level to use")
     return parser
 
@@ -136,51 +142,63 @@
     :param ns: the parsed options
     :type ns: argparse.Namespace
     :return: the state container
     :rtype: State
     """
     result = State(
         connection=redis.Redis(host=ns.redis_host, port=ns.redis_port, db=ns.redis_db),
-        channel_in=ns.model_channel_in,
-        channel_out=ns.model_channel_out,
         timeout=ns.timeout,
         title=ns.title,
         description=ns.description,
+        sleep_time=ns.sleep_time,
     )
 
     for att in dir(ns):
         if att.startswith("_"):
             continue
-        if att in ["redis_host", "redis_port", "redis_db", "model_channel_in", "model_channel_out", "timeout", "title", "description"]:
+        if att == "model_channel_in":
+            result.channel_in = ns.model_channel_in
+        if att == "model_channel_out":
+            result.channel_in = ns.model_channel_out
+        if att in ["redis_host", "redis_port", "redis_db", "timeout", "title", "description", "sleep_time", "model_channel_in", "model_channel_out"]:
             continue
         result.params[att] = getattr(ns, att)
 
     return result
 
 
-def make_prediction(state: State, data):
+def make_prediction(state: State, data, channel_out: str = None, channel_in: str = None):
     """
     Makes a prediction by broadcasting the data and waiting for a result coming through.
 
     :param state: the state to use to broadcasting/listening
     :type state: State
     :param data: the data to send
+    :param channel_out: for overriding the state's out channel
+    :type channel_out: str
+    :param channel_in: for overriding the state's in channel
+    :type channel_in: str
     :return: the received data, None if failed or timeout
     """
+    if channel_out is None:
+        channel_out = state.channel_out
+    if channel_in is None:
+        channel_in = state.channel_in
+
     def anon_handler(message):
         data = message['data']
         state.data = data
         state.pubsub_thread.stop()
         state.pubsub.close()
         state.pubsub = None
 
     state.pubsub = state.connection.pubsub()
-    state.pubsub.psubscribe(**{state.channel_out: anon_handler})
-    state.pubsub_thread = state.pubsub.run_in_thread(sleep_time=0.01)
-    state.connection.publish(state.channel_in, data)
+    state.pubsub.psubscribe(**{channel_out: anon_handler})
+    state.pubsub_thread = state.pubsub.run_in_thread(sleep_time=state.sleep_time)
+    state.connection.publish(channel_in, data)
 
     # wait for data to show up
     start = datetime.now()
     end = start
     no_data = False
     while state.pubsub is not None:
         sleep(0.01)
```

### Comparing `gifr-0.0.5/src/gifr/fonts.py` & `gifr-0.0.6/src/gifr/fonts.py`

 * *Files identical despite different names*

### Comparing `gifr-0.0.5/src/gifr/image_classification.py` & `gifr-0.0.6/src/gifr/image_classification.py`

 * *Files identical despite different names*

### Comparing `gifr-0.0.5/src/gifr/image_segmentation.py` & `gifr-0.0.6/src/gifr/image_segmentation.py`

 * *Files identical despite different names*

### Comparing `gifr-0.0.5/src/gifr/object_detection.py` & `gifr-0.0.6/src/gifr/object_detection.py`

 * *Files identical despite different names*

### Comparing `gifr-0.0.5/src/gifr/text_classification.py` & `gifr-0.0.6/src/gifr/text_classification.py`

 * *Files identical despite different names*

### Comparing `gifr-0.0.5/src/gifr/text_generation.py` & `gifr-0.0.6/src/gifr/text_generation.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,20 +10,24 @@
 PROG: str = "gifr-textgen"
 
 _logger = logging.getLogger(PROG)
 
 state: State = None
 
 
-def predict(text: str) -> str:
+def predict(text: str, channel_out: str = None, channel_in: str = None) -> str:
     """
     Sends the text to the model and returns the completed text.
 
     :param text: the text to send
     :type text: str
+    :param channel_out: for overriding the state's out channel
+    :type channel_out: str
+    :param channel_in: for overriding the state's in channel
+    :type channel_in: str
     :return: the prediction result
     :rtype: str
     """
     global state
     state.logger.info("Completing: %s" % text)
 
     # build query
@@ -31,15 +35,15 @@
     if state.params["history_on"]:
         if state.params["send_history"] is not None:
             d[state.params["send_history"]] = state.history
         if state.params["send_turns"] is not None:
             d[state.params["send_turns"]] = state.turns
 
     # perform query
-    result = make_prediction(state, json.dumps(d))
+    result = make_prediction(state, json.dumps(d), channel_in=channel_in, channel_out=channel_out)
 
     # parse response
     if result is None:
         result = "no result"
     else:
         if state.params["json_response"]:
             try:
```

### Comparing `gifr-0.0.5/src/gifr.egg-info/PKG-INFO` & `gifr-0.0.6/src/gifr.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 Metadata-Version: 1.1
 Name: gifr
-Version: 0.0.5
+Version: 0.0.6
 Summary: gradio interfaces for Deep Learning Docker images that use Redis for receiving data to make predictions on.
 Home-page: https://github.com/waikato-datamining/gifr
 Author: Peter Reutemann
 Author-email: fracpete@waikato.ac.nz
 License: MIT License
 Description: `gradio <https://www.gradio.app/>`__ interfaces for Deep Learning Docker images that
         use Redis for receiving data to make predictions on.
         
         `https://www.data-mining.co.nz/docker-images/ <https://www.data-mining.co.nz/docker-images/>`__
         
         Interfaces are available for:
         
         - automatic speech recognition (ASR)
+        - automatic speech recognition (ASR) + text generation
         - image classification
         - image segmentation
         - object detection/instance segmentation
         - text classification
         - text generation
         
         
         Changelog
         =========
         
+        0.0.6 (2024-05-30)
+        ------------------
+        
+        - added interface for automatic speech recognition (ASR) combined with text generation
+        
+        
         0.0.5 (2024-05-27)
         ------------------
         
         - added interface for automatic speech recognition (ASR)
         
         
         0.0.4 (2024-02-27)
```

