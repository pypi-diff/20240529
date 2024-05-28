# Comparing `tmp/ebb_events-0.3.4.tar.gz` & `tmp/ebb_events-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebb_events-0.3.4.tar", max compression
+gzip compressed data, was "ebb_events-0.3.5.tar", max compression
```

## Comparing `ebb_events-0.3.4.tar` & `ebb_events-0.3.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1071 2024-05-06 20:14:00.489414 ebb_events-0.3.4/LICENSE
--rw-r--r--   0        0        0     9163 2024-05-20 19:44:17.149941 ebb_events-0.3.4/README.md
--rw-r--r--   0        0        0        0 2024-04-19 21:49:16.587650 ebb_events-0.3.4/ebb_events/__init__.py
--rw-r--r--   0        0        0     8886 2024-05-15 20:31:26.930793 ebb_events-0.3.4/ebb_events/builders/event_builder.py
--rw-r--r--   0        0        0    10777 2024-05-17 17:46:46.038249 ebb_events-0.3.4/ebb_events/consumers/event_consumer.py
--rw-r--r--   0        0        0      174 2024-04-22 19:12:51.110543 ebb_events-0.3.4/ebb_events/enums.py
--rw-r--r--   0        0        0      875 2024-05-20 19:44:17.150314 ebb_events-0.3.4/ebb_events/event_payload_utils.py
--rw-r--r--   0        0        0     3194 2024-05-20 19:44:17.150658 ebb_events-0.3.4/ebb_events/event_schema.py
--rw-r--r--   0        0        0      383 2024-05-06 17:16:47.746622 ebb_events-0.3.4/ebb_events/exceptions.py
--rw-r--r--   0        0        0      263 2024-05-14 16:56:47.898608 ebb_events-0.3.4/ebb_events/field_constants.py
--rw-r--r--   0        0        0      571 2024-05-20 19:44:17.150966 ebb_events-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     9661 1970-01-01 00:00:00.000000 ebb_events-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-06 20:14:00.489414 ebb_events-0.3.5/LICENSE
+-rw-r--r--   0        0        0     9175 2024-05-28 22:43:36.277500 ebb_events-0.3.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 21:49:16.587650 ebb_events-0.3.5/ebb_events/__init__.py
+-rw-r--r--   0        0        0     8886 2024-05-15 20:31:26.930793 ebb_events-0.3.5/ebb_events/builders/event_builder.py
+-rw-r--r--   0        0        0    10777 2024-05-17 17:46:46.038249 ebb_events-0.3.5/ebb_events/consumers/event_consumer.py
+-rw-r--r--   0        0        0      174 2024-04-22 19:12:51.110543 ebb_events-0.3.5/ebb_events/enums.py
+-rw-r--r--   0        0        0      875 2024-05-20 19:44:17.150314 ebb_events-0.3.5/ebb_events/event_payload_utils.py
+-rw-r--r--   0        0        0     3194 2024-05-20 19:44:17.150658 ebb_events-0.3.5/ebb_events/event_schema.py
+-rw-r--r--   0        0        0      383 2024-05-06 17:16:47.746622 ebb_events-0.3.5/ebb_events/exceptions.py
+-rw-r--r--   0        0        0      263 2024-05-14 16:56:47.898608 ebb_events-0.3.5/ebb_events/field_constants.py
+-rw-r--r--   0        0        0      571 2024-05-28 22:43:36.277792 ebb_events-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     9673 1970-01-01 00:00:00.000000 ebb_events-0.3.5/PKG-INFO
```

### Comparing `ebb_events-0.3.4/LICENSE` & `ebb_events-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ebb_events-0.3.4/README.md` & `ebb_events-0.3.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 * Dashes (not underscores)
 * Alphanumeric topics only (Illegal characters: #, +, *, \<spaces\>)
 * No leading “/”
 * 50 character maximum per topic section (256 maximum total)
 
 ### Topic Hierarchy Explained:
 1. **\<organization\>:** The highest level in the hierarchy representing the \<organization\> that is publishing and owning this event.
-    * Example: `ebb`
+    * Example: `ebbcarbon`
 2. **\<system-id\>:** The unique \<system-id\> from which this message is originating. The \<system-id\> should be unique and un-changing (e.g. don't rely on things like geographic location if the producer might move locations).
     * Example: `system-name`
 3. **\<event-type\>:** The specific type of event being published. As of now, we support four event-types.
     * `data`: Sensor readings and measurements
     * `state`: Sensor current state (e.g. online status, battery life, memory, power, etc.)
     * `config`: Sensor setup (e.g. calibration coefficients, calibration date, physical location, configured outputs/fields, etc.)
     * `cmd`: Instructions for subscribing clients
@@ -63,15 +63,15 @@
     * Example: `system-name` is made up of 4 subsystems, 3 of which are different "my-subsystem-name" subsystems -> the various "my-subsystem-name" subsystems could be labeled `my-subsystem-name-01`, `my-subsystem-name-02`, and `my-subsystem-name-03`
 5. **\<device-id\>:** The unique identity of a device _as it relates to the subsystem_ on which it lives. This is _not_ the device's serial number or physical unique ID since the physical device might be replaced.
     * Example: `my-subsystem-name-01` has sensors ("my-sensor") in slots 01, 02, and 03. Therefore \<device-id\> could be `my-sensor-02`
         * If the physical "my-sensor" in slot 02 fails and is replaced with a new "my-sensor", even though the serial number is now different, the \<device-id\> in your topic would remain the same because this part of the topic refers to the \<device-id\> as it relates to the overall subsystem, not as it relates to the physical device itself.
         * The new "my-sensor" is still `my-sensor-02`.
 ### Topic Example:
 For a data message being published by one of Ebb's edge-nodes with measurements from "my-sensor" in sensor slot 02 of subsystem 1, which makes up system-name:
-* `ebb/system-name/data/subsystem-1/my-sensor-02`
+* `ebbcarbon/system-name/data/subsystem-1/my-sensor-02`
 
 # Event Payload Structure:
 This package defines the event payload schema to follow for all event types. The schema includes relavant metadata in the EventEnvelope and the actual message information in the "data" field of the payload. Specific message structures of the "data" field differ based on event type and the context of the event. The envelope + data make up the overall event payload. All MQTT event messages that are published and consumed should subscribe to this general structure making it easier to share data across organizations and systems. Names of payload fields follow attribute names from [CloudEvents](https://cloudevents.io/) as well.
 
 ### Event Payload:
 Structure shared by all event messages regardless of event type
 ```python
```

### Comparing `ebb_events-0.3.4/ebb_events/builders/event_builder.py` & `ebb_events-0.3.5/ebb_events/builders/event_builder.py`

 * *Files identical despite different names*

### Comparing `ebb_events-0.3.4/ebb_events/consumers/event_consumer.py` & `ebb_events-0.3.5/ebb_events/consumers/event_consumer.py`

 * *Files identical despite different names*

### Comparing `ebb_events-0.3.4/ebb_events/event_payload_utils.py` & `ebb_events-0.3.5/ebb_events/event_payload_utils.py`

 * *Files identical despite different names*

### Comparing `ebb_events-0.3.4/ebb_events/event_schema.py` & `ebb_events-0.3.5/ebb_events/event_schema.py`

 * *Files identical despite different names*

### Comparing `ebb_events-0.3.4/pyproject.toml` & `ebb_events-0.3.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ebb-events"
-version = "0.3.4"
+version = "0.3.5"
 description = "Package for building and standardizing MQTT event messages."
 authors = ["Ryan Bloom <ryan.bloom@ebbcarbon.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 marshmallow = "^3.21.1"
```

### Comparing `ebb_events-0.3.4/PKG-INFO` & `ebb_events-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebb-events
-Version: 0.3.4
+Version: 0.3.5
 Summary: Package for building and standardizing MQTT event messages.
 Author: Ryan Bloom
 Author-email: ryan.bloom@ebbcarbon.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -61,15 +61,15 @@
 * Dashes (not underscores)
 * Alphanumeric topics only (Illegal characters: #, +, *, \<spaces\>)
 * No leading “/”
 * 50 character maximum per topic section (256 maximum total)
 
 ### Topic Hierarchy Explained:
 1. **\<organization\>:** The highest level in the hierarchy representing the \<organization\> that is publishing and owning this event.
-    * Example: `ebb`
+    * Example: `ebbcarbon`
 2. **\<system-id\>:** The unique \<system-id\> from which this message is originating. The \<system-id\> should be unique and un-changing (e.g. don't rely on things like geographic location if the producer might move locations).
     * Example: `system-name`
 3. **\<event-type\>:** The specific type of event being published. As of now, we support four event-types.
     * `data`: Sensor readings and measurements
     * `state`: Sensor current state (e.g. online status, battery life, memory, power, etc.)
     * `config`: Sensor setup (e.g. calibration coefficients, calibration date, physical location, configured outputs/fields, etc.)
     * `cmd`: Instructions for subscribing clients
@@ -77,15 +77,15 @@
     * Example: `system-name` is made up of 4 subsystems, 3 of which are different "my-subsystem-name" subsystems -> the various "my-subsystem-name" subsystems could be labeled `my-subsystem-name-01`, `my-subsystem-name-02`, and `my-subsystem-name-03`
 5. **\<device-id\>:** The unique identity of a device _as it relates to the subsystem_ on which it lives. This is _not_ the device's serial number or physical unique ID since the physical device might be replaced.
     * Example: `my-subsystem-name-01` has sensors ("my-sensor") in slots 01, 02, and 03. Therefore \<device-id\> could be `my-sensor-02`
         * If the physical "my-sensor" in slot 02 fails and is replaced with a new "my-sensor", even though the serial number is now different, the \<device-id\> in your topic would remain the same because this part of the topic refers to the \<device-id\> as it relates to the overall subsystem, not as it relates to the physical device itself.
         * The new "my-sensor" is still `my-sensor-02`.
 ### Topic Example:
 For a data message being published by one of Ebb's edge-nodes with measurements from "my-sensor" in sensor slot 02 of subsystem 1, which makes up system-name:
-* `ebb/system-name/data/subsystem-1/my-sensor-02`
+* `ebbcarbon/system-name/data/subsystem-1/my-sensor-02`
 
 # Event Payload Structure:
 This package defines the event payload schema to follow for all event types. The schema includes relavant metadata in the EventEnvelope and the actual message information in the "data" field of the payload. Specific message structures of the "data" field differ based on event type and the context of the event. The envelope + data make up the overall event payload. All MQTT event messages that are published and consumed should subscribe to this general structure making it easier to share data across organizations and systems. Names of payload fields follow attribute names from [CloudEvents](https://cloudevents.io/) as well.
 
 ### Event Payload:
 Structure shared by all event messages regardless of event type
 ```python
```

