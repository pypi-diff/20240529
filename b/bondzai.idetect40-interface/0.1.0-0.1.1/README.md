# Comparing `tmp/bondzai.idetect40-interface-0.1.0.tar.gz` & `tmp/bondzai.idetect40-interface-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bondzai.idetect40-interface-0.1.0.tar", last modified: Thu Apr 25 09:34:58 2024, max compression
+gzip compressed data, was "bondzai.idetect40-interface-0.1.1.tar", last modified: Wed May 29 12:16:16 2024, max compression
```

## Comparing `bondzai.idetect40-interface-0.1.0.tar` & `bondzai.idetect40-interface-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 09:34:58.690033 bondzai.idetect40-interface-0.1.0/
--rw-rw-rw-   0        0        0      547 2023-10-17 12:30:45.000000 bondzai.idetect40-interface-0.1.0/NOTICE
--rw-rw-rw-   0        0        0      805 2024-04-25 09:34:58.690538 bondzai.idetect40-interface-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      360 2024-04-24 10:47:45.000000 bondzai.idetect40-interface-0.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-25 09:34:58.670652 bondzai.idetect40-interface-0.1.0/bondzai/
-drwxrwxrwx   0        0        0        0 2024-04-25 09:34:58.675994 bondzai.idetect40-interface-0.1.0/bondzai/idetect40_interface/
--rw-rw-rw-   0        0        0       22 2024-04-25 09:33:18.000000 bondzai.idetect40-interface-0.1.0/bondzai/idetect40_interface/__init__.py
--rw-rw-rw-   0        0        0    18666 2024-04-25 07:47:40.000000 bondzai.idetect40-interface-0.1.0/bondzai/idetect40_interface/exchange_table.py
--rw-rw-rw-   0        0        0    11553 2024-04-22 15:43:39.000000 bondzai.idetect40-interface-0.1.0/bondzai/idetect40_interface/socket.py
-drwxrwxrwx   0        0        0        0 2024-04-25 09:34:58.689430 bondzai.idetect40-interface-0.1.0/bondzai.idetect40_interface.egg-info/
--rw-rw-rw-   0        0        0      805 2024-04-25 09:34:58.000000 bondzai.idetect40-interface-0.1.0/bondzai.idetect40_interface.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      769 2024-04-25 09:34:58.000000 bondzai.idetect40-interface-0.1.0/bondzai.idetect40_interface.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 09:34:58.000000 bondzai.idetect40-interface-0.1.0/bondzai.idetect40_interface.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-25 09:34:58.000000 bondzai.idetect40-interface-0.1.0/bondzai.idetect40_interface.egg-info/namespace_packages.txt
--rw-rw-rw-   0        0        0       28 2024-04-25 09:34:58.000000 bondzai.idetect40-interface-0.1.0/bondzai.idetect40_interface.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-25 09:34:58.000000 bondzai.idetect40-interface-0.1.0/bondzai.idetect40_interface.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-25 09:34:58.000000 bondzai.idetect40-interface-0.1.0/bondzai.idetect40_interface.egg-info/zip-safe
--rw-rw-rw-   0        0        0       71 2023-10-17 12:30:45.000000 bondzai.idetect40-interface-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      733 2024-04-25 09:34:58.696677 bondzai.idetect40-interface-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0       36 2023-10-17 12:30:45.000000 bondzai.idetect40-interface-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 09:34:58.677613 bondzai.idetect40-interface-0.1.0/tests/
--rw-rw-rw-   0        0        0     5190 2024-04-25 07:48:00.000000 bondzai.idetect40-interface-0.1.0/tests/test_exchange_table.py
--rw-rw-rw-   0        0        0     5998 2024-04-24 10:33:37.000000 bondzai.idetect40-interface-0.1.0/tests/test_socket.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2024-05-29 12:16:16.483089 bondzai.idetect40-interface-0.1.1/
+-rw-r--r--   0 theo       (501) staff       (20)      547 2024-05-29 10:08:52.000000 bondzai.idetect40-interface-0.1.1/NOTICE
+-rw-r--r--   0 theo       (501) staff       (20)      789 2024-05-29 12:16:16.483166 bondzai.idetect40-interface-0.1.1/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)      360 2024-05-29 10:08:52.000000 bondzai.idetect40-interface-0.1.1/README.rst
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2024-05-29 12:16:16.479433 bondzai.idetect40-interface-0.1.1/bondzai/
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2024-05-29 12:16:16.481066 bondzai.idetect40-interface-0.1.1/bondzai/idetect40_interface/
+-rw-r--r--   0 theo       (501) staff       (20)       22 2024-05-29 12:15:59.000000 bondzai.idetect40-interface-0.1.1/bondzai/idetect40_interface/__init__.py
+-rw-r--r--   0 theo       (501) staff       (20)    19986 2024-05-29 11:09:58.000000 bondzai.idetect40-interface-0.1.1/bondzai/idetect40_interface/exchange_table.py
+-rw-r--r--   0 theo       (501) staff       (20)    11553 2024-05-29 10:08:52.000000 bondzai.idetect40-interface-0.1.1/bondzai/idetect40_interface/socket.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2024-05-29 12:16:16.482845 bondzai.idetect40-interface-0.1.1/bondzai.idetect40_interface.egg-info/
+-rw-r--r--   0 theo       (501) staff       (20)      789 2024-05-29 12:16:16.000000 bondzai.idetect40-interface-0.1.1/bondzai.idetect40_interface.egg-info/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)      595 2024-05-29 12:16:16.000000 bondzai.idetect40-interface-0.1.1/bondzai.idetect40_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2024-05-29 12:16:16.000000 bondzai.idetect40-interface-0.1.1/bondzai.idetect40_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 theo       (501) staff       (20)        8 2024-05-29 12:16:16.000000 bondzai.idetect40-interface-0.1.1/bondzai.idetect40_interface.egg-info/namespace_packages.txt
+-rw-r--r--   0 theo       (501) staff       (20)       35 2024-05-29 12:16:16.000000 bondzai.idetect40-interface-0.1.1/bondzai.idetect40_interface.egg-info/requires.txt
+-rw-r--r--   0 theo       (501) staff       (20)       19 2024-05-29 12:16:16.000000 bondzai.idetect40-interface-0.1.1/bondzai.idetect40_interface.egg-info/top_level.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2024-05-29 12:16:16.000000 bondzai.idetect40-interface-0.1.1/bondzai.idetect40_interface.egg-info/zip-safe
+-rw-r--r--   0 theo       (501) staff       (20)       71 2024-05-29 10:08:52.000000 bondzai.idetect40-interface-0.1.1/pyproject.toml
+-rw-r--r--   0 theo       (501) staff       (20)      731 2024-05-29 12:16:16.483467 bondzai.idetect40-interface-0.1.1/setup.cfg
+-rw-r--r--   0 theo       (501) staff       (20)       36 2024-05-29 12:14:27.000000 bondzai.idetect40-interface-0.1.1/setup.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2024-05-29 12:16:16.481711 bondzai.idetect40-interface-0.1.1/tests/
+-rw-r--r--   0 theo       (501) staff       (20)     6129 2024-05-29 10:52:46.000000 bondzai.idetect40-interface-0.1.1/tests/test_exchange_table.py
+-rw-r--r--   0 theo       (501) staff       (20)     5998 2024-05-29 10:08:52.000000 bondzai.idetect40-interface-0.1.1/tests/test_socket.py
```

### Comparing `bondzai.idetect40-interface-0.1.0/NOTICE` & `bondzai.idetect40-interface-0.1.1/NOTICE`

 * *Files identical despite different names*

### Comparing `bondzai.idetect40-interface-0.1.0/PKG-INFO` & `bondzai.idetect40-interface-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-Metadata-Version: 2.1
-Name: bondzai.idetect40-interface
-Version: 0.1.0
-Summary: Bondzai iDetect 4.0 interface
-Home-page: UNKNOWN
-Author: Bondzai
-License: Apache License 2.0
-Keywords: davinsy,bondzai,idetect40
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-License-File: NOTICE
-
-Bondzai iDetect 4.0 interface
-=============================
-
-Description
-~~~~~~~~~~~
-
-Bondzai iDetect 4.0 interface provides python library to communicate with one product instance via socket
-
-Installation
-~~~~~~~~~~~~
-
-.. code:: bash
-
-   pip install bondzai.idetect40-interface
-
-Usage
-~~~~~
-
-.. code:: python
-
-   from bondzai.idetect40_interface import socket
-
+Metadata-Version: 2.1
+Name: bondzai.idetect40-interface
+Version: 0.1.1
+Summary: Bondzai iDetect 4.0 interface
+Home-page: UNKNOWN
+Author: Bondzai
+License: Apache License 2.0
+Keywords: davinsy,bondzai,idetect40
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Provides-Extra: dev
+License-File: NOTICE
+
+Bondzai iDetect 4.0 interface
+=============================
+
+Description
+~~~~~~~~~~~
+
+Bondzai iDetect 4.0 interface provides python library to communicate with one product instance via socket
+
+Installation
+~~~~~~~~~~~~
+
+.. code:: bash
+
+   pip install bondzai.idetect40-interface
+
+Usage
+~~~~~
+
+.. code:: python
+
+   from bondzai.idetect40_interface import socket
+
```

### Comparing `bondzai.idetect40-interface-0.1.0/bondzai/idetect40_interface/exchange_table.py` & `bondzai.idetect40-interface-0.1.1/bondzai/idetect40_interface/exchange_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -113,14 +113,22 @@
 class Agent():
     """Agent element
     """
     def __init__(self, agent_id: int, source_nb: int):
         self.active = False
         self.agent_id = agent_id
         self.source_dict = {src_id: False for src_id in range(1, source_nb + 1)}
+        self.tool_id = None
+        self.cycle_iteration = None
+
+    def set_tool_id(self, tool_id: int):
+        self.tool_id = tool_id
+
+    def set_cycle_iteration(self, iteration: int):
+        self.cycle_iteration = iteration
     
     def set_state(self, active: bool):
         """Set agent state
 
         Args:
             active (bool): If True, the agent is agent else not
         """
@@ -164,60 +172,82 @@
     
     def to_dict(self) -> dict:
         """Convert agent to dict
 
         Returns:
             dict: dict representation of agent
         """
-        d = {"active": self.active, "sources": self.source_dict}
-        return d
+        return {
+            "active": self.active, 
+            "sources": self.source_dict,
+            "tool_id": self.tool_id, 
+            "cycle_iteration": self.cycle_iteration
+        }
     
     def __eq__(self, other) -> bool:
-        eq = self.active == other.active and self.agent_id == other.agent_id
+        eq = self.active == other.active and self.agent_id == other.agent_id \
+            and self.tool_id == other.tool_id and self.cycle_iteration == other.cycle_iteration
+        
         for source_id, active in self.source_dict.items():
             eq = eq and other.source_dict[source_id] == active
+        
         return eq
 
 
 class ExchangeTable:
     """Generic exchange table
     """
     def __init__(self, descriptor: dict, msg: bytearray = None):
         self.system_running = False
         self.process_ongoing = False
         self.heartbeat = False
         self.nb_sources = descriptor["agents"]["nb_sources"]
-        self.agents = {agent_id: Agent(agent_id, self.nb_sources) 
-                       for agent_id in range(1, descriptor["agents"]["nb_agents"] + 1)}
-        self.attributes = [Attribute(attr["name"], AttributeDataType(attr["type"]), attr["size"]) 
-                           for attr in descriptor["attributes"]]
+        self.agents = {
+            agent_id: Agent(agent_id, self.nb_sources) 
+            for agent_id in range(1, descriptor["agents"]["nb_agents"] + 1)
+        }
+        self.attributes = [
+            Attribute(attr["name"], AttributeDataType(attr["type"]), attr["size"]) 
+            for attr in descriptor["attributes"]
+        ]
         if msg is not None:
             self.init_from_msg(msg)
     
     def init_from_msg(self, msg: bytearray):
         """Set bytes message info into table
 
         Args:
             binary (bytearray): message as array of bytes
         """
         byte_offset = 0
         msg_int_list = [int(byte) for byte in msg]
         self._set_system_word(int_to_bool_list(msg_int_list[0]) + int_to_bool_list(msg_int_list[1]))
         byte_offset += 2
+
         agent_bin_table = msg_int_list[byte_offset:byte_offset + 2 * len(self.agents)]
         for index in range(0, len(agent_bin_table), 2):
             agent_bin_data = int_to_bool_list(agent_bin_table[index]) + int_to_bool_list(agent_bin_table[index + 1])
             agent_id = index // 2 + 1
             self.set_agent_state(agent_id, agent_bin_data[0])
             for source_id in range(1, self.nb_sources + 1):
                 self.set_source_state(agent_id, source_id, agent_bin_data[source_id])
             byte_offset += 2
+
+        pm_data_table = msg_int_list[byte_offset:byte_offset + 4 * len(self.agents)]
+        agent_idx = 1
+        for idx in range(0, len(pm_data_table), 4):
+            self.agents[agent_idx].set_tool_id(int.from_bytes(pm_data_table[idx:idx + 2], byteorder="little"))
+            self.agents[agent_idx].set_cycle_iteration(int.from_bytes(pm_data_table[idx + 2:idx + 4], byteorder="little"))
+            byte_offset += 4
+            agent_idx += 1
+
         byte_offset += self._set_result_word(msg_int_list[byte_offset: byte_offset + 6])
         attr_bin_table = msg[byte_offset:]
         idx = 0
+
         for attribute in self.attributes:
             byte_len = len(attribute)
             value_array = attr_bin_table[idx: idx + byte_len]
             idx += byte_to_word_length(byte_len) * 2
             if attribute.type == AttributeDataType.STRING:
                 value = str(value_array.decode("utf8")).rstrip("\x00")
             elif attribute.type == AttributeDataType.INT:
@@ -232,15 +262,15 @@
         """Get size of the table
 
         Returns:
             int: size of the table in bytes
         """
         nb_agent = len(self.agents)
         system_size = 2
-        agent_size = nb_agent * 2
+        agent_size = nb_agent * 6
         attribute_size = sum([byte_to_word_length(len(attr)) * 2 for attr in self.attributes])
         output_size = system_size + agent_size + attribute_size
         return output_size
     
     def set_system_running(self, running: bool):
         """Set system running
 
@@ -403,34 +433,45 @@
     
     def to_msg(self) -> bytearray:
         """Convert table to a bytearray
         Returns:
             bytearray: message as array of bytes
         """
         byte_array = bytearray()
+        pm_byte_array = bytearray()
+
         system_word = self._get_system_word()
         byte_array.extend([bool_list_to_int(system_word[:7]), bool_list_to_int(system_word[7:])])
+
         for agent_id in range(1, len(self.agents) + 1):
             agent_integer = int(self.get_agent_state(agent_id))
             for source_id in range(1, self.nb_sources + 1):
                 agent_integer += int(self.get_source_state(agent_id, source_id)) * 2 ** (source_id)
             byte_array += agent_integer.to_bytes(2, "little")
+
+            tool_id = int(self.agents[agent_id].tool_id)
+            cycle_iteration = int(self.agents[agent_id].cycle_iteration)
+            pm_byte_array += tool_id.to_bytes(2, "little") + cycle_iteration.to_bytes(2, "little")
+
+        byte_array.extend(pm_byte_array)
         byte_array.extend(self._get_result_word())
+
         for attribute in self.attributes:
             byte_nb = int(np.ceil(attribute.size / 16)) * 2
             value = attribute.value
             if attribute.type == AttributeDataType.STRING:
                 value_array = attribute.value.encode("utf8")
             elif attribute.type ==  AttributeDataType.INT:
                 value_array = attribute.value.to_bytes(int(attribute.size / 8), byteorder="little")
             elif attribute.type ==  AttributeDataType.FLOAT:
                 value_array = struct.pack('f',value)
             elif attribute.type ==  AttributeDataType.BOOL:
                 value_array = struct.pack("?", value)
             byte_array += bytearray(value_array) + int(0).to_bytes(byte_nb - len(value_array), byteorder="little")
+
         return byte_array
     
     def __eq__(self, other):
         eq = self.system_running == other.system_running
         eq = eq and self.process_ongoing == other.process_ongoing
         eq = eq and self.heartbeat == other.heartbeat
         for agent_id, agent in self.agents.items():
@@ -441,21 +482,27 @@
     
     def to_dict(self) -> dict:
         """Convert exchange table to dict
 
         Returns:
             dict: dict representation of v
         """
-        d = {"system": {"running": self.system_running, 
-                        "process_ongoing": self.process_ongoing, 
-                        "heart_beat": self.heartbeat},
-             "agents": {agent_id: agent.to_dict() for agent_id, agent in self.agents.items()},
-             "attributes": {attribute.name: attribute.value for attribute in self.attributes}}
-        return d
-
+        return {
+            "system": {
+                "running": self.system_running, 
+                "process_ongoing": self.process_ongoing, 
+                "heart_beat": self.heartbeat
+            },
+            "agents": {
+                agent_id: agent.to_dict() for agent_id, agent in self.agents.items()
+            },
+            "attributes": {
+                attribute.name: attribute.value for attribute in self.attributes
+            }
+        }
 
 
 class PLCTable(ExchangeTable):
     """Exchange table used on PLC side
     """
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
```

### Comparing `bondzai.idetect40-interface-0.1.0/bondzai/idetect40_interface/socket.py` & `bondzai.idetect40-interface-0.1.1/bondzai/idetect40_interface/socket.py`

 * *Files identical despite different names*

### Comparing `bondzai.idetect40-interface-0.1.0/bondzai.idetect40_interface.egg-info/PKG-INFO` & `bondzai.idetect40-interface-0.1.1/bondzai.idetect40_interface.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-Metadata-Version: 2.1
-Name: bondzai.idetect40-interface
-Version: 0.1.0
-Summary: Bondzai iDetect 4.0 interface
-Home-page: UNKNOWN
-Author: Bondzai
-License: Apache License 2.0
-Keywords: davinsy,bondzai,idetect40
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-License-File: NOTICE
-
-Bondzai iDetect 4.0 interface
-=============================
-
-Description
-~~~~~~~~~~~
-
-Bondzai iDetect 4.0 interface provides python library to communicate with one product instance via socket
-
-Installation
-~~~~~~~~~~~~
-
-.. code:: bash
-
-   pip install bondzai.idetect40-interface
-
-Usage
-~~~~~
-
-.. code:: python
-
-   from bondzai.idetect40_interface import socket
-
+Metadata-Version: 2.1
+Name: bondzai.idetect40-interface
+Version: 0.1.1
+Summary: Bondzai iDetect 4.0 interface
+Home-page: UNKNOWN
+Author: Bondzai
+License: Apache License 2.0
+Keywords: davinsy,bondzai,idetect40
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Provides-Extra: dev
+License-File: NOTICE
+
+Bondzai iDetect 4.0 interface
+=============================
+
+Description
+~~~~~~~~~~~
+
+Bondzai iDetect 4.0 interface provides python library to communicate with one product instance via socket
+
+Installation
+~~~~~~~~~~~~
+
+.. code:: bash
+
+   pip install bondzai.idetect40-interface
+
+Usage
+~~~~~
+
+.. code:: python
+
+   from bondzai.idetect40_interface import socket
+
```

### Comparing `bondzai.idetect40-interface-0.1.0/bondzai.idetect40_interface.egg-info/SOURCES.txt` & `bondzai.idetect40-interface-0.1.1/bondzai.idetect40_interface.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -10,13 +10,8 @@
 ./tests/test_socket.py
 bondzai.idetect40_interface.egg-info/PKG-INFO
 bondzai.idetect40_interface.egg-info/SOURCES.txt
 bondzai.idetect40_interface.egg-info/dependency_links.txt
 bondzai.idetect40_interface.egg-info/namespace_packages.txt
 bondzai.idetect40_interface.egg-info/requires.txt
 bondzai.idetect40_interface.egg-info/top_level.txt
-bondzai.idetect40_interface.egg-info/zip-safe
-bondzai/idetect40_interface/__init__.py
-bondzai/idetect40_interface/exchange_table.py
-bondzai/idetect40_interface/socket.py
-tests/test_exchange_table.py
-tests/test_socket.py
+bondzai.idetect40_interface.egg-info/zip-safe
```

### Comparing `bondzai.idetect40-interface-0.1.0/setup.cfg` & `bondzai.idetect40-interface-0.1.1/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2062 6f6e 647a 6169 2e69 6465 7465   = bondzai.idete
-00000020: 6374 3430 2d69 6e74 6572 6661 6365 0d0a  ct40-interface..
-00000030: 7665 7273 696f 6e20 3d20 6174 7472 3a20  version = attr: 
-00000040: 626f 6e64 7a61 692e 6964 6574 6563 7434  bondzai.idetect4
-00000050: 305f 696e 7465 7266 6163 652e 5f5f 7665  0_interface.__ve
-00000060: 7273 696f 6e5f 5f0d 0a61 7574 686f 7220  rsion__..author 
-00000070: 3d20 426f 6e64 7a61 690d 0a64 6573 6372  = Bondzai..descr
-00000080: 6970 7469 6f6e 203d 2042 6f6e 647a 6169  iption = Bondzai
-00000090: 2069 4465 7465 6374 2034 2e30 2069 6e74   iDetect 4.0 int
-000000a0: 6572 6661 6365 0d0a 6c6f 6e67 5f64 6573  erface..long_des
-000000b0: 6372 6970 7469 6f6e 203d 2066 696c 653a  cription = file:
-000000c0: 2052 4541 444d 452e 7273 740d 0a6b 6579   README.rst..key
-000000d0: 776f 7264 7320 3d20 6461 7669 6e73 792c  words = davinsy,
-000000e0: 2062 6f6e 647a 6169 2c20 6964 6574 6563   bondzai, idetec
-000000f0: 7434 300d 0a6c 6963 656e 7365 203d 2041  t40..license = A
-00000100: 7061 6368 6520 4c69 6365 6e73 6520 322e  pache License 2.
-00000110: 300d 0a6c 6963 656e 7365 5f66 696c 6573  0..license_files
-00000120: 203d 200d 0a09 4c49 4345 4e53 450d 0a09   = ...LICENSE...
-00000130: 4e4f 5449 4345 0d0a 636c 6173 7369 6669  NOTICE..classifi
-00000140: 6572 7320 3d20 0d0a 0950 726f 6772 616d  ers = ...Program
-00000150: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000160: 2050 7974 686f 6e20 3a3a 2033 0d0a 094c   Python :: 3...L
-00000170: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
-00000180: 7072 6f76 6564 203a 3a20 4170 6163 6865  proved :: Apache
-00000190: 2053 6f66 7477 6172 6520 4c69 6365 6e73   Software Licens
-000001a0: 650d 0a09 4f70 6572 6174 696e 6720 5379  e...Operating Sy
-000001b0: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
-000001c0: 656e 6465 6e74 0d0a 0d0a 5b6f 7074 696f  endent....[optio
-000001d0: 6e73 5d0d 0a70 6163 6b61 6765 7320 3d20  ns]..packages = 
-000001e0: 6669 6e64 5f6e 616d 6573 7061 6365 3a0d  find_namespace:.
-000001f0: 0a70 6163 6b61 6765 5f64 6972 203d 200d  .package_dir = .
-00000200: 0a09 3d20 2e0d 0a7a 6970 5f73 6166 6520  ..= ...zip_safe 
-00000210: 3d20 5472 7565 0d0a 696e 636c 7564 655f  = True..include_
-00000220: 7061 636b 6167 655f 6461 7461 203d 2054  package_data = T
-00000230: 7275 650d 0a6e 616d 6573 7061 6365 5f70  rue..namespace_p
-00000240: 6163 6b61 6765 7320 3d20 0d0a 0962 6f6e  ackages = ...bon
-00000250: 647a 6169 0d0a 696e 7374 616c 6c5f 7265  dzai..install_re
-00000260: 7175 6972 6573 203d 200d 0a09 7079 7465  quires = ...pyte
-00000270: 7374 3d3d 372e 322e 300d 0a09 6e75 6d70  st==7.2.0...nump
-00000280: 793d 3d31 2e32 352e 300d 0a0d 0a5b 6f70  y==1.25.0....[op
-00000290: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
-000002a0: 696e 645d 0d0a 7768 6572 6520 3d20 2e0d  ind]..where = ..
-000002b0: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
-000002c0: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
-000002d0: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 626f 6e64 7a61 692e 6964 6574 6563  = bondzai.idetec
+00000020: 7434 302d 696e 7465 7266 6163 650a 7665  t40-interface.ve
+00000030: 7273 696f 6e20 3d20 6174 7472 3a20 626f  rsion = attr: bo
+00000040: 6e64 7a61 692e 6964 6574 6563 7434 305f  ndzai.idetect40_
+00000050: 696e 7465 7266 6163 652e 5f5f 7665 7273  interface.__vers
+00000060: 696f 6e5f 5f0a 6175 7468 6f72 203d 2042  ion__.author = B
+00000070: 6f6e 647a 6169 0a64 6573 6372 6970 7469  ondzai.descripti
+00000080: 6f6e 203d 2042 6f6e 647a 6169 2069 4465  on = Bondzai iDe
+00000090: 7465 6374 2034 2e30 2069 6e74 6572 6661  tect 4.0 interfa
+000000a0: 6365 0a6c 6f6e 675f 6465 7363 7269 7074  ce.long_descript
+000000b0: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
+000000c0: 4d45 2e72 7374 0a6b 6579 776f 7264 7320  ME.rst.keywords 
+000000d0: 3d20 6461 7669 6e73 792c 2062 6f6e 647a  = davinsy, bondz
+000000e0: 6169 2c20 6964 6574 6563 7434 300a 6c69  ai, idetect40.li
+000000f0: 6365 6e73 6520 3d20 4170 6163 6865 204c  cense = Apache L
+00000100: 6963 656e 7365 2032 2e30 0a6c 6963 656e  icense 2.0.licen
+00000110: 7365 5f66 696c 6573 203d 200a 094c 4943  se_files = ..LIC
+00000120: 454e 5345 0a09 4e4f 5449 4345 0a63 6c61  ENSE..NOTICE.cla
+00000130: 7373 6966 6965 7273 203d 200a 0950 726f  ssifiers = ..Pro
+00000140: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000150: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000160: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
+00000170: 2041 7070 726f 7665 6420 3a3a 2041 7061   Approved :: Apa
+00000180: 6368 6520 536f 6674 7761 7265 204c 6963  che Software Lic
+00000190: 656e 7365 0a09 4f70 6572 6174 696e 6720  ense..Operating 
+000001a0: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
+000001b0: 6570 656e 6465 6e74 0a0a 5b6f 7074 696f  ependent..[optio
+000001c0: 6e73 5d0a 7061 636b 6167 6573 203d 2066  ns].packages = f
+000001d0: 696e 645f 6e61 6d65 7370 6163 653a 0a70  ind_namespace:.p
+000001e0: 6163 6b61 6765 5f64 6972 203d 200a 093d  ackage_dir = ..=
+000001f0: 202e 0a7a 6970 5f73 6166 6520 3d20 5472   ..zip_safe = Tr
+00000200: 7565 0a69 6e63 6c75 6465 5f70 6163 6b61  ue.include_packa
+00000210: 6765 5f64 6174 6120 3d20 5472 7565 0a6e  ge_data = True.n
+00000220: 616d 6573 7061 6365 5f70 6163 6b61 6765  amespace_package
+00000230: 7320 3d20 0a09 626f 6e64 7a61 690a 696e  s = ..bondzai.in
+00000240: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
+00000250: 200a 096e 756d 7079 3d3d 312e 3235 2e30   ..numpy==1.25.0
+00000260: 0a0a 5b6f 7074 696f 6e73 2e65 7874 7261  ..[options.extra
+00000270: 735f 7265 7175 6972 655d 0a64 6576 203d  s_require].dev =
+00000280: 200a 0970 7974 6573 743d 3d37 2e32 2e30   ..pytest==7.2.0
+00000290: 0a0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
+000002a0: 6765 732e 6669 6e64 5d0a 7768 6572 6520  ges.find].where 
+000002b0: 3d20 2e0a 0a5b 6567 675f 696e 666f 5d0a  = ...[egg_info].
+000002c0: 7461 675f 6275 696c 6420 3d20 0a74 6167  tag_build = .tag
+000002d0: 5f64 6174 6520 3d20 300a 0a              _date = 0..
```

### Comparing `bondzai.idetect40-interface-0.1.0/tests/test_exchange_table.py` & `bondzai.idetect40-interface-0.1.1/tests/test_exchange_table.py`

 * *Files 22% similar despite different names*

```diff
@@ -52,55 +52,107 @@
         table.set_ack_result(d["system"]["ack_result"])
         table.set_ack_exception(d["system"]["ack_exception"])
     table.set_system_running(d["system"]["running"])
     table.set_process_ongoing(d["system"]["process_ongoing"])
     table.set_heart_beat(d["system"]["heart_beat"])
     for agent_id, agent_dict in d["agents"].items():
         table.set_agent_state(agent_id, agent_dict["active"])
+        table.agents[agent_id].set_tool_id(agent_dict["tool_id"])
+        table.agents[agent_id].set_cycle_iteration(agent_dict["cycle_iteration"])
         for source_id, scr_active in agent_dict["sources"].items():
             table.set_source_state(agent_id, source_id, scr_active)
     for attribute_name, value in d["attributes"].items():
         table.set_attribute_value(attribute_name, value)
     return table
     
 
 
 class Test_ExchangeTable():
     is_connected = False
     error_code = 7
     plc_table_dict = {
-        "system": {"running": True, "process_ongoing": False, "heart_beat": False, 
-                   "ack_result": True, "ack_exception": True},
+        "system": {
+            "running": True, "process_ongoing": False, "heart_beat": False, 
+            "ack_result": True, "ack_exception": True
+        },
         "agents": {
-            1: {"active": True, "sources": {1: True, 2: False, 3: True, 4: False}},
-            2: {"active": True, "sources": {1: False, 2: False, 3: True, 4: False}},
-            3: {"active": False, "sources": {1: True, 2: True, 3: True, 4: False}},
-            4: {"active": False, "sources": {1: True, 2: False, 3: True, 4: True}}
+            1: {"active": True, "sources": {1: True, 2: False, 3: True, 4: False}, "tool_id": 0, "cycle_iteration": 0},
+            2: {"active": True, "sources": {1: False, 2: False, 3: True, 4: False}, "tool_id": 0, "cycle_iteration": 0},
+            3: {"active": False, "sources": {1: True, 2: True, 3: True, 4: False}, "tool_id": 1, "cycle_iteration": 88},
+            4: {"active": False, "sources": {1: True, 2: False, 3: True, 4: True}, "tool_id": 2, "cycle_iteration": 5}
         },
-        "attributes": {"serial number": 12, "vehicule type": "abc", "temperature": 48.70000076293945, 
-                       "over pressure": False}
+        "attributes": {
+            "serial number": 12, "vehicule type": "abc", "temperature": 48.70000076293945, 
+            "over pressure": False
         }
+    }
     plc_table = table_from_dict(TEST_DESCRIPTOR, plc_table_dict)
-    plc_table_msg = bytearray([25, 0, 11, 0, 9, 0, 14, 0, 26, 0, 12, 0, 97, 98, 99, 0, 205, 204, 66, 66, 0, 0])
+    plc_table_msg = bytearray([
+        25, 0, 
+        11, 0, 
+        9, 0, 
+        14, 0, 
+        26, 0, 
+        0, 0, 
+        0, 0, 
+        0, 0, 
+        0, 0, 
+        1, 0, 
+        88, 0, 
+        2, 0, 
+        5, 0, 
+        12, 0, 
+        97, 98, 
+        99, 0, 
+        205, 204, 
+        66, 66, 
+        0, 0
+    ])
     i40_table_dict = {
-        "system": {"running": True, "process_ongoing": False, "heart_beat": False, "exception_occured": True, 
-                "exception": error_code},
+        "system": {
+            "running": True, "process_ongoing": False, "heart_beat": False, "exception_occured": True, 
+            "exception": error_code
+        },
         "agents": {
-        1: {"active": True, "sources": {1: True, 2: False, 3: True, 4: False}},
-        2: {"active": True, "sources": {1: False, 2: False, 3: True, 4: False}},
-        3: {"active": False, "sources": {1: True, 2: True, 3: True, 4: False}},
-        4: {"active": False, "sources": {1: True, 2: False, 3: True, 4: True}}
+            1: {"active": True, "sources": {1: True, 2: False, 3: True, 4: False}, "tool_id": 0, "cycle_iteration": 0},
+            2: {"active": True, "sources": {1: False, 2: False, 3: True, 4: False}, "tool_id": 0, "cycle_iteration": 0},
+            3: {"active": False, "sources": {1: True, 2: True, 3: True, 4: False}, "tool_id": 1, "cycle_iteration": 88},
+            4: {"active": False, "sources": {1: True, 2: False, 3: True, 4: True}, "tool_id": 2, "cycle_iteration": 5}
         },
         "result": {"agent_id": 1, "source_id": 3, "key_id": 1, "value_id": 6, "category_id": 4},
-        "attributes": {"serial number": 12, "vehicule type": "ab", "temperature": 48.70000076293945, 
-                       "over pressure": False}
-        } 
+        "attributes": {
+            "serial number": 12, "vehicule type": "ab", "temperature": 48.70000076293945, 
+            "over pressure": False
+        }
+    } 
     i40_table = table_from_dict(TEST_DESCRIPTOR, i40_table_dict)
-    i40_table_msg = bytearray([9, error_code, 11, 0, 9, 0, 14, 0, 26, 0, 1, 3, 1, 6, 4, 0, 12, 0, 97, 98, 0, 0, 205, 
-                                  204, 66, 66, 0, 0])
+    i40_table_msg = bytearray([
+        9, error_code, 
+        11, 0, 
+        9, 0, 
+        14, 0, 
+        26, 0,
+        0, 0, 
+        0, 0, 
+        0, 0, 
+        0, 0, 
+        1, 0, 
+        88, 0, 
+        2, 0, 
+        5, 0, 
+        1, 3,
+        1, 6,
+        4, 0, 
+        12, 0, 
+        97, 98,
+        0, 0, 
+        205, 204, 
+        66, 66, 
+        0, 0
+    ])
            
     def test_msg_to_table(self):
         table_from_msg = PLCTable(TEST_DESCRIPTOR, self.plc_table_msg)
         assert self.plc_table == table_from_msg
         table_from_msg = I40Table(TEST_DESCRIPTOR, self.i40_table_msg)
         assert self.i40_table == table_from_msg
```

### Comparing `bondzai.idetect40-interface-0.1.0/tests/test_socket.py` & `bondzai.idetect40-interface-0.1.1/tests/test_socket.py`

 * *Files identical despite different names*

