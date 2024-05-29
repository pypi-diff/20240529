# Comparing `tmp/pybalebot-0.0.1.tar.gz` & `tmp/pybalebot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybalebot-0.0.1.tar", last modified: Wed May 29 00:08:26 2024, max compression
+gzip compressed data, was "pybalebot-0.0.2.tar", last modified: Wed May 29 12:43:58 2024, max compression
```

## Comparing `pybalebot-0.0.1.tar` & `pybalebot-0.0.2.tar`

### file list

```diff
@@ -1,33 +1,56 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 00:08:26.805078 pybalebot-0.0.1/
--rw-rw-rw-   0        0        0     3044 2024-05-29 00:08:26.804102 pybalebot-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1884 2024-05-29 00:07:30.000000 pybalebot-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 00:08:26.765030 pybalebot-0.0.1/pybalebot/
--rw-rw-rw-   0        0        0       56 2024-05-28 21:16:01.000000 pybalebot-0.0.1/pybalebot/__init__.py
--rw-rw-rw-   0        0        0     3410 2024-05-29 00:06:21.000000 pybalebot-0.0.1/pybalebot/api.py
--rw-rw-rw-   0        0        0     2005 2024-05-29 00:06:27.000000 pybalebot-0.0.1/pybalebot/client.py
--rw-rw-rw-   0        0        0      357 2024-05-28 18:40:53.000000 pybalebot-0.0.1/pybalebot/errors.py
--rw-rw-rw-   0        0        0    11117 2024-05-29 00:01:43.000000 pybalebot-0.0.1/pybalebot/filters.py
-drwxrwxrwx   0        0        0        0 2024-05-29 00:08:26.793368 pybalebot-0.0.1/pybalebot/methods/
--rw-rw-rw-   0        0        0      161 2024-05-28 21:30:10.000000 pybalebot-0.0.1/pybalebot/methods/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 00:08:26.797271 pybalebot-0.0.1/pybalebot/methods/messages/
--rw-rw-rw-   0        0        0      159 2024-05-28 21:37:14.000000 pybalebot-0.0.1/pybalebot/methods/messages/__init__.py
--rw-rw-rw-   0        0        0      416 2024-05-28 21:39:07.000000 pybalebot-0.0.1/pybalebot/methods/messages/edit_message_text.py
--rw-rw-rw-   0        0        0      528 2024-05-28 21:29:31.000000 pybalebot-0.0.1/pybalebot/methods/messages/send_message.py
-drwxrwxrwx   0        0        0        0 2024-05-29 00:08:26.798248 pybalebot-0.0.1/pybalebot/methods/updates/
--rw-rw-rw-   0        0        0       84 2024-05-28 18:49:44.000000 pybalebot-0.0.1/pybalebot/methods/updates/__init__.py
--rw-rw-rw-   0        0        0      296 2024-05-28 20:42:52.000000 pybalebot-0.0.1/pybalebot/methods/updates/get_updates.py
-drwxrwxrwx   0        0        0        0 2024-05-29 00:08:26.800198 pybalebot-0.0.1/pybalebot/methods/users/
--rw-rw-rw-   0        0        0       69 2024-05-28 21:06:54.000000 pybalebot-0.0.1/pybalebot/methods/users/__init__.py
--rw-rw-rw-   0        0        0      129 2024-05-28 21:18:48.000000 pybalebot-0.0.1/pybalebot/methods/users/get_me.py
-drwxrwxrwx   0        0        0        0 2024-05-29 00:08:26.802151 pybalebot-0.0.1/pybalebot/types/
--rw-rw-rw-   0        0        0       58 2024-05-28 19:56:13.000000 pybalebot-0.0.1/pybalebot/types/__init__.py
--rw-rw-rw-   0        0        0     6529 2024-05-28 21:43:57.000000 pybalebot-0.0.1/pybalebot/types/message.py
--rw-rw-rw-   0        0        0     5914 2024-05-28 19:42:55.000000 pybalebot-0.0.1/pybalebot/types/results.py
-drwxrwxrwx   0        0        0        0 2024-05-29 00:08:26.803134 pybalebot-0.0.1/pybalebot.egg-info/
--rw-rw-rw-   0        0        0     3044 2024-05-29 00:08:26.000000 pybalebot-0.0.1/pybalebot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      673 2024-05-29 00:08:26.000000 pybalebot-0.0.1/pybalebot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 00:08:26.000000 pybalebot-0.0.1/pybalebot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-29 00:08:26.000000 pybalebot-0.0.1/pybalebot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-29 00:08:26.000000 pybalebot-0.0.1/pybalebot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 00:08:26.805078 pybalebot-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1533 2024-05-28 16:32:14.000000 pybalebot-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:43:58.838329 pybalebot-0.0.2/
+-rw-rw-rw-   0        0        0     3048 2024-05-29 12:43:58.837354 pybalebot-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1888 2024-05-29 12:43:10.000000 pybalebot-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 12:43:58.781659 pybalebot-0.0.2/pybalebot/
+-rw-rw-rw-   0        0        0      112 2024-05-29 12:43:40.000000 pybalebot-0.0.2/pybalebot/__init__.py
+-rw-rw-rw-   0        0        0     4136 2024-05-29 12:38:23.000000 pybalebot-0.0.2/pybalebot/api.py
+-rw-rw-rw-   0        0        0     2004 2024-05-29 12:36:03.000000 pybalebot-0.0.2/pybalebot/client.py
+-rw-rw-rw-   0        0        0      357 2024-05-28 18:40:53.000000 pybalebot-0.0.2/pybalebot/errors.py
+-rw-rw-rw-   0        0        0    12012 2024-05-29 12:36:09.000000 pybalebot-0.0.2/pybalebot/filters.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:43:58.810965 pybalebot-0.0.2/pybalebot/methods/
+-rw-rw-rw-   0        0        0      198 2024-05-29 12:33:52.000000 pybalebot-0.0.2/pybalebot/methods/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:43:58.818773 pybalebot-0.0.2/pybalebot/methods/chats/
+-rw-rw-rw-   0        0        0      564 2024-05-29 10:35:30.000000 pybalebot-0.0.2/pybalebot/methods/chats/__init__.py
+-rw-rw-rw-   0        0        0      332 2024-05-29 09:26:07.000000 pybalebot-0.0.2/pybalebot/methods/chats/ban_chat_member.py
+-rw-rw-rw-   0        0        0      236 2024-05-29 09:50:52.000000 pybalebot-0.0.2/pybalebot/methods/chats/get_chat.py
+-rw-rw-rw-   0        0        0      291 2024-05-29 10:35:12.000000 pybalebot-0.0.2/pybalebot/methods/chats/get_chat_administrators.py
+-rw-rw-rw-   0        0        0      283 2024-05-29 09:54:53.000000 pybalebot-0.0.2/pybalebot/methods/chats/get_chat_member_count.py
+-rw-rw-rw-   0        0        0      275 2024-05-29 09:47:43.000000 pybalebot-0.0.2/pybalebot/methods/chats/leave_chat.py
+-rw-rw-rw-   0        0        0      344 2024-05-29 09:37:50.000000 pybalebot-0.0.2/pybalebot/methods/chats/promote_chat_member.py
+-rw-rw-rw-   0        0        0      326 2024-05-29 09:43:41.000000 pybalebot-0.0.2/pybalebot/methods/chats/set_chat_photo.py
+-rw-rw-rw-   0        0        0      473 2024-05-29 09:29:10.000000 pybalebot-0.0.2/pybalebot/methods/chats/unban_chat_member.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:43:58.822714 pybalebot-0.0.2/pybalebot/methods/messages/
+-rw-rw-rw-   0        0        0      394 2024-05-29 09:34:58.000000 pybalebot-0.0.2/pybalebot/methods/messages/__init__.py
+-rw-rw-rw-   0        0        0      455 2024-05-29 07:46:15.000000 pybalebot-0.0.2/pybalebot/methods/messages/copy_message.py
+-rw-rw-rw-   0        0        0      340 2024-05-29 09:34:04.000000 pybalebot-0.0.2/pybalebot/methods/messages/delete_message.py
+-rw-rw-rw-   0        0        0      416 2024-05-28 21:39:07.000000 pybalebot-0.0.2/pybalebot/methods/messages/edit_message_text.py
+-rw-rw-rw-   0        0        0      464 2024-05-29 07:43:58.000000 pybalebot-0.0.2/pybalebot/methods/messages/forward_message.py
+-rw-rw-rw-   0        0        0      768 2024-05-29 12:32:00.000000 pybalebot-0.0.2/pybalebot/methods/messages/send_message.py
+-rw-rw-rw-   0        0        0     2032 2024-05-29 08:44:35.000000 pybalebot-0.0.2/pybalebot/methods/messages/send_photo.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:43:58.827594 pybalebot-0.0.2/pybalebot/methods/updates/
+-rw-rw-rw-   0        0        0      261 2024-05-29 12:38:10.000000 pybalebot-0.0.2/pybalebot/methods/updates/__init__.py
+-rw-rw-rw-   0        0        0      296 2024-05-28 20:42:52.000000 pybalebot-0.0.2/pybalebot/methods/updates/get_updates.py
+-rw-rw-rw-   0        0        0      157 2024-05-29 07:34:51.000000 pybalebot-0.0.2/pybalebot/methods/updates/get_webhook_info.py
+-rw-rw-rw-   0        0        0      181 2024-05-29 07:32:36.000000 pybalebot-0.0.2/pybalebot/methods/updates/set_webhook.py
+-rw-rw-rw-   0        0        0      184 2024-05-29 07:36:34.000000 pybalebot-0.0.2/pybalebot/methods/updates/webhook_info.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:43:58.828570 pybalebot-0.0.2/pybalebot/methods/users/
+-rw-rw-rw-   0        0        0       69 2024-05-28 21:06:54.000000 pybalebot-0.0.2/pybalebot/methods/users/__init__.py
+-rw-rw-rw-   0        0        0      129 2024-05-28 21:18:48.000000 pybalebot-0.0.2/pybalebot/methods/users/get_me.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:43:58.835401 pybalebot-0.0.2/pybalebot/types/
+-rw-rw-rw-   0        0        0      331 2024-05-29 08:32:11.000000 pybalebot-0.0.2/pybalebot/types/__init__.py
+-rw-rw-rw-   0        0        0      481 2024-05-29 08:13:01.000000 pybalebot-0.0.2/pybalebot/types/inline_keyboard_button.py
+-rw-rw-rw-   0        0        0      374 2024-05-29 08:14:00.000000 pybalebot-0.0.2/pybalebot/types/inline_keyboard_markup.py
+-rw-rw-rw-   0        0        0        0 2024-05-29 12:33:17.000000 pybalebot-0.0.2/pybalebot/types/input_file.py
+-rw-rw-rw-   0        0        0      440 2024-05-29 08:14:30.000000 pybalebot-0.0.2/pybalebot/types/keyboard_button.py
+-rw-rw-rw-   0        0        0     4278 2024-05-29 12:42:00.000000 pybalebot-0.0.2/pybalebot/types/message.py
+-rw-rw-rw-   0        0        0      718 2024-05-29 08:23:19.000000 pybalebot-0.0.2/pybalebot/types/reply_keyboard_markup.py
+-rw-rw-rw-   0        0        0      340 2024-05-29 08:23:53.000000 pybalebot-0.0.2/pybalebot/types/reply_keyboard_remove.py
+-rw-rw-rw-   0        0        0     5914 2024-05-28 19:42:55.000000 pybalebot-0.0.2/pybalebot/types/results.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:43:58.836378 pybalebot-0.0.2/pybalebot.egg-info/
+-rw-rw-rw-   0        0        0     3048 2024-05-29 12:43:58.000000 pybalebot-0.0.2/pybalebot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1595 2024-05-29 12:43:58.000000 pybalebot-0.0.2/pybalebot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 12:43:58.000000 pybalebot-0.0.2/pybalebot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-29 12:43:58.000000 pybalebot-0.0.2/pybalebot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-29 12:43:58.000000 pybalebot-0.0.2/pybalebot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 12:43:58.838329 pybalebot-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1533 2024-05-29 12:43:19.000000 pybalebot-0.0.2/setup.py
```

### Comparing `pybalebot-0.0.1/PKG-INFO` & `pybalebot-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybalebot
-Version: 0.0.1
+Version: 0.0.2
 Summary: Modern and fully asynchronous framework for Bale Bot API
 Home-page: https://github.com/shayanheidari01/pybalebot
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: pybalebot,bale,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -44,15 +44,15 @@
     </a>
     •
     <a href="https://t.me/rubika_library">
         News
     </a>
 </p>
 
-## Rubpy
+## PyBaleBot
 
 > Modern and fully asynchronous framework for Bale Bot API
 
 ### Using Async
 ```python
 from pybalebot import Client, filters
 from pybalebot.types import Message
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pybalebot Version: 0.0.1 Summary: Modern and fully
+Metadata-Version: 2.1 Name: pybalebot Version: 0.0.2 Summary: Modern and fully
 asynchronous framework for Bale Bot API Home-page: https://github.com/
 shayanheidari01/pybalebot Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Keywords: pybalebot,bale,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
@@ -13,23 +13,23 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application
 Frameworks Requires-Python: ~=3.7 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
                                   _[_p_y_b_a_l_e_b_o_t_]
                         BBaallee AAPPII FFrraammeewwoorrkk ffoorr PPyytthhoonn
                _H_o_m_e_p_a_g_e_ â¢ _D_o_c_u_m_e_n_t_a_t_i_o_n_ â¢ _R_e_l_e_a_s_e_s_ â¢ _N_e_w_s
-## Rubpy > Modern and fully asynchronous framework for Bale Bot API ### Using
-Async ```python from pybalebot import Client, filters from pybalebot.types
-import Message bot_token = "123456789:**********************" app = Client
-("my_bot", bot_token=bot_token) @app.on_message(filters.text) async def hello
-(client, message: Message): await message.reply("Hello from PyBaleBot!")
-app.run() ``` **PyBaleBot** is a modern, elegant and asynchronous framework. It
-enables you to easily interact with the main Bale API through a user account
-(custom client) or a bot identity (bot API alternative) using Python. ### Key
-Features - **Ready**: Install PyBaleBot with pip and start building your
-applications right away. - **Easy**: Makes the Bale API simple and intuitive,
-while still allowing advanced usages. - **Elegant**: Low-level details are
-abstracted and re-presented in a more convenient way. - **Fast**: Boosted up by
-aiohttp, a high-performance http library written in C. - **Async**: Fully
-asynchronous (also usable synchronously if wanted, for convenience). -
-**Powerful**: Full access to Bale's API to execute any official client action
-and more. ### Installing ``` bash pip3 install -U pybalebot ```
+## PyBaleBot > Modern and fully asynchronous framework for Bale Bot API ###
+Using Async ```python from pybalebot import Client, filters from
+pybalebot.types import Message bot_token = "123456789:**********************"
+app = Client("my_bot", bot_token=bot_token) @app.on_message(filters.text) async
+def hello(client, message: Message): await message.reply("Hello from
+PyBaleBot!") app.run() ``` **PyBaleBot** is a modern, elegant and asynchronous
+framework. It enables you to easily interact with the main Bale API through a
+user account (custom client) or a bot identity (bot API alternative) using
+Python. ### Key Features - **Ready**: Install PyBaleBot with pip and start
+building your applications right away. - **Easy**: Makes the Bale API simple
+and intuitive, while still allowing advanced usages. - **Elegant**: Low-level
+details are abstracted and re-presented in a more convenient way. - **Fast**:
+Boosted up by aiohttp, a high-performance http library written in C. -
+**Async**: Fully asynchronous (also usable synchronously if wanted, for
+convenience). - **Powerful**: Full access to Bale's API to execute any official
+client action and more. ### Installing ``` bash pip3 install -U pybalebot ```
```

### Comparing `pybalebot-0.0.1/README.md` & `pybalebot-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     </a>
     •
     <a href="https://t.me/rubika_library">
         News
     </a>
 </p>
 
-## Rubpy
+## PyBaleBot
 
 > Modern and fully asynchronous framework for Bale Bot API
 
 ### Using Async
 ```python
 from pybalebot import Client, filters
 from pybalebot.types import Message
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
                                   _[_p_y_b_a_l_e_b_o_t_]
                         BBaallee AAPPII FFrraammeewwoorrkk ffoorr PPyytthhoonn
                _H_o_m_e_p_a_g_e_ â¢ _D_o_c_u_m_e_n_t_a_t_i_o_n_ â¢ _R_e_l_e_a_s_e_s_ â¢ _N_e_w_s
-## Rubpy > Modern and fully asynchronous framework for Bale Bot API ### Using
-Async ```python from pybalebot import Client, filters from pybalebot.types
-import Message bot_token = "123456789:**********************" app = Client
-("my_bot", bot_token=bot_token) @app.on_message(filters.text) async def hello
-(client, message: Message): await message.reply("Hello from PyBaleBot!")
-app.run() ``` **PyBaleBot** is a modern, elegant and asynchronous framework. It
-enables you to easily interact with the main Bale API through a user account
-(custom client) or a bot identity (bot API alternative) using Python. ### Key
-Features - **Ready**: Install PyBaleBot with pip and start building your
-applications right away. - **Easy**: Makes the Bale API simple and intuitive,
-while still allowing advanced usages. - **Elegant**: Low-level details are
-abstracted and re-presented in a more convenient way. - **Fast**: Boosted up by
-aiohttp, a high-performance http library written in C. - **Async**: Fully
-asynchronous (also usable synchronously if wanted, for convenience). -
-**Powerful**: Full access to Bale's API to execute any official client action
-and more. ### Installing ``` bash pip3 install -U pybalebot ```
+## PyBaleBot > Modern and fully asynchronous framework for Bale Bot API ###
+Using Async ```python from pybalebot import Client, filters from
+pybalebot.types import Message bot_token = "123456789:**********************"
+app = Client("my_bot", bot_token=bot_token) @app.on_message(filters.text) async
+def hello(client, message: Message): await message.reply("Hello from
+PyBaleBot!") app.run() ``` **PyBaleBot** is a modern, elegant and asynchronous
+framework. It enables you to easily interact with the main Bale API through a
+user account (custom client) or a bot identity (bot API alternative) using
+Python. ### Key Features - **Ready**: Install PyBaleBot with pip and start
+building your applications right away. - **Easy**: Makes the Bale API simple
+and intuitive, while still allowing advanced usages. - **Elegant**: Low-level
+details are abstracted and re-presented in a more convenient way. - **Fast**:
+Boosted up by aiohttp, a high-performance http library written in C. -
+**Async**: Fully asynchronous (also usable synchronously if wanted, for
+convenience). - **Powerful**: Full access to Bale's API to execute any official
+client action and more. ### Installing ``` bash pip3 install -U pybalebot ```
```

### Comparing `pybalebot-0.0.1/pybalebot/api.py` & `pybalebot-0.0.2/pybalebot/api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import aiohttp
 import inspect
 import asyncio
+import pybalebot
 from .errors import RPCError
 from .filters import Filter
 from .types import Results, Message
 
 class BaleAPI:
     BASE_URL = 'https://tapi.bale.ai'
 
     def __init__(self, client=None) -> None:
         """
         Initialize the BaleAPI instance.
         
         :param client: The client instance which contains bot_token and other configurations.
         """
-        self.client = client
+        self.client: "pybalebot.Client" = client
         self.offset = 0
         self.session = aiohttp.ClientSession(
             base_url=client.base_url or self.BASE_URL,
             connector=aiohttp.TCPConnector(),
             timeout=aiohttp.ClientTimeout(total=20)
         )
 
@@ -51,32 +52,48 @@
 
     async def process_update(self, update: Results):
         """
         Process an update from the Bale API.
 
         :param update: The update data.
         """
-        update_data = update.message.to_dict
-        update_message = Message(update_data)
+        update_message = Message(update.original_update)
         update_message.client = self.client
+
         for handler, filters in self.client.handlers.copy().items():
             filter_results = []
             for filter_func in filters:
-                if isinstance(filter_func, Filter):
-                    result = await filter_func(client=self.client, message=update_message)
-                else:
-                    result = await filter_func(self.client, update_message) if inspect.iscoroutinefunction(filter_func) else filter_func(self.client, update_message)
-                filter_results.append(result)
+                try:
+                    if isinstance(filter_func, Filter):
+                        result = await filter_func(self.client, update_message)
+                    else:
+                        result = await filter_func(self.client, update_message) if inspect.iscoroutinefunction(filter_func) else filter_func(self.client, update_message)
+                    filter_results.append(result)
+                except Exception as e:
+                    # Debugging: Print the filter_func and error message
+                    print(f"Error in filter function {filter_func}: {e}")
+                    filter_results.append(False)
+
             if all(filter_results):
-                await handler(self.client, update_message)
+                try:
+                    # Ensure handler is not None
+                    if handler is None:
+                        raise TypeError("Handler is None")
+                    
+                    # Call the handler
+                    await handler(self.client, update_message)
+                except Exception as e:
+                    # Debugging: Print the handler and error message
+                    print(f"Error in handler {handler}: {e}")
 
     async def get_updates(self):
         """
         Continuously fetch updates from the Bale API and process them.
         """
+        await self.client.set_webhook()
         while True:
             try:
                 updates = await self.client.get_updates(offset=self.offset)
                 updates_result = updates.result
 
                 if updates_result:
                     self.offset = updates_result[-1].update_id + 1
```

### Comparing `pybalebot-0.0.1/pybalebot/client.py` & `pybalebot-0.0.2/pybalebot/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         Connect to the Bale API and retrieve bot information.
         """
         if self.bot_token is None:
             self.bot_token = input('Please enter your bot token: ')
 
         self.api = BaleAPI(client=self)
         self.me = await self.get_me()
-        print(f'connect to  the Bale API with {self.me.username} bot\n')
+        print(f'connect to the Bale API with {self.me.username} bot\n')
 
     async def stop(self):
         """
         Stop the client by closing the Bale API session.
         """
         await self.api.close()
```

### Comparing `pybalebot-0.0.1/pybalebot/filters.py` & `pybalebot-0.0.2/pybalebot/filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import re
 import inspect
 from typing import Union, List, Callable, Awaitable, Pattern
+
+import pybalebot
 from .types import Message
 
 COMMAND_RE = re.compile(r"([\"'])(.*?)(?<!\\)\1|(\S+)")
 
 class Filter:
     def __init__(self, func: Union[Callable, Awaitable]):
         """
@@ -283,15 +285,15 @@
     def reply(self):
         """
         Check if the message is a reply to another message.
 
         :return: A reply filter.
         """
         async def func(client, message):
-            return isinstance(message.reply_to_message, dict)
+            return bool(message.reply_to_message)
         return Filter(func)
 
     def command(self, commands: Union[str, List[str]], prefixes: Union[str, List[str]] = "/", case_sensitive: bool = False):
         """
         Check if the message contains a command.
 
         :param commands: The commands to check.
@@ -354,22 +356,44 @@
             if message.text is None:
                 return False
             message['pattern_match'] = compiled_pattern.match(message.text)
             return bool(message['pattern_match'])
         
         return Filter(func)
 
+    def user(self, users: Union[str, int, List[Union[str, int]]]):
+        """
+        Check if the message is from a specific user private chat or other chats.
+
+        :param users: The user id or list of user ids to check.
+        :return: A user filter.
+        """
+        chat_ids = users if isinstance(users, list) else [users]
+        async def func(client, message: Message) -> bool:
+            return message.message.find_keys('from').id in chat_ids
+        return Filter(func)
+
     def chat(self, chats: Union[str, int, List[Union[str, int]]]):
         """
         Check if the message is from a specific chat or chats.
 
         :param chats: The chat or list of chats to check.
         :return: A chat filter.
         """
         chat_ids = chats if isinstance(chats, list) else [chats]
         
         async def func(client, message: Message) -> bool:
             return message.chat.id in chat_ids
         
         return Filter(func)
 
+    @property
+    def admin(self):
+        async def func(client: "pybalebot.Client", message: Message):
+            admins = await client.get_chat_administrators(message.chat.id)
+            for result in admins.result:
+                if message.message['from']['id'] == result.user.id:
+                    return True
+            return False
+        return Filter(func)
+
 filters = Filters()
```

### Comparing `pybalebot-0.0.1/pybalebot/types/message.py` & `pybalebot-0.0.2/pybalebot/types/results.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import json
 
-
-class Message:
+class Results:
     def __str__(self) -> str:
         return self.jsonify(indent=2)
 
     def __getattr__(self, name):
         return self.find_keys(keys=name)
 
     def __setitem__(self, key, value):
@@ -15,15 +14,15 @@
         return self.original_update[key]
 
     def __lts__(self, update: list, *args, **kwargs):
         for index, element in enumerate(update):
             if isinstance(element, list):
                 update[index] = self.__lts__(update=element)
             elif isinstance(element, dict):
-                update[index] = Message(update=element)
+                update[index] = Results(update=element)
             else:
                 update[index] = element
         return update
 
     def __init__(self, update: dict, *args, **kwargs) -> None:
         self.client = update.get('client')
         self.original_update = update
@@ -41,15 +40,15 @@
             keys = [keys]
 
         if isinstance(original_update, dict):
             for key in keys:
                 try:
                     update = original_update[key]
                     if isinstance(update, dict):
-                        update = Message(update=update)
+                        update = Results(update=update)
                     elif isinstance(update, list):
                         update = self.__lts__(update=update)
                     return update
                 except KeyError:
                     pass
             original_update = original_update.values()
 
@@ -197,18 +196,8 @@
     @property
     def author_guid(self):
         return self.message.author_object_guid
 
     @property
     def is_text(self):
         message = self.message
-        return message is not None and message.type == 'Text'
-
-    async def reply_text(self, text: str, chat_id: int=None, reply_to_message_id: int = None):
-        result = await self.client.send_message(chat_id or self.chat.id, text, reply_to_message_id=reply_to_message_id or self.message_id)
-        result['client'] = self.client
-        return Message(result.to_dict)
-
-    async def edit_text(self, text: str, chat_id: int=None, message_id: int = None):
-        result = await self.client.edit_message_text(text, chat_id or self.chat.id, message_id=message_id or self.message_id)
-        result['client'] = self.client
-        return Message(result.to_dict)
+        return message is not None and message.type == 'Text'
```

### Comparing `pybalebot-0.0.1/pybalebot.egg-info/PKG-INFO` & `pybalebot-0.0.2/pybalebot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybalebot
-Version: 0.0.1
+Version: 0.0.2
 Summary: Modern and fully asynchronous framework for Bale Bot API
 Home-page: https://github.com/shayanheidari01/pybalebot
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: pybalebot,bale,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -44,15 +44,15 @@
     </a>
     •
     <a href="https://t.me/rubika_library">
         News
     </a>
 </p>
 
-## Rubpy
+## PyBaleBot
 
 > Modern and fully asynchronous framework for Bale Bot API
 
 ### Using Async
 ```python
 from pybalebot import Client, filters
 from pybalebot.types import Message
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pybalebot Version: 0.0.1 Summary: Modern and fully
+Metadata-Version: 2.1 Name: pybalebot Version: 0.0.2 Summary: Modern and fully
 asynchronous framework for Bale Bot API Home-page: https://github.com/
 shayanheidari01/pybalebot Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Keywords: pybalebot,bale,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
@@ -13,23 +13,23 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application
 Frameworks Requires-Python: ~=3.7 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
                                   _[_p_y_b_a_l_e_b_o_t_]
                         BBaallee AAPPII FFrraammeewwoorrkk ffoorr PPyytthhoonn
                _H_o_m_e_p_a_g_e_ â¢ _D_o_c_u_m_e_n_t_a_t_i_o_n_ â¢ _R_e_l_e_a_s_e_s_ â¢ _N_e_w_s
-## Rubpy > Modern and fully asynchronous framework for Bale Bot API ### Using
-Async ```python from pybalebot import Client, filters from pybalebot.types
-import Message bot_token = "123456789:**********************" app = Client
-("my_bot", bot_token=bot_token) @app.on_message(filters.text) async def hello
-(client, message: Message): await message.reply("Hello from PyBaleBot!")
-app.run() ``` **PyBaleBot** is a modern, elegant and asynchronous framework. It
-enables you to easily interact with the main Bale API through a user account
-(custom client) or a bot identity (bot API alternative) using Python. ### Key
-Features - **Ready**: Install PyBaleBot with pip and start building your
-applications right away. - **Easy**: Makes the Bale API simple and intuitive,
-while still allowing advanced usages. - **Elegant**: Low-level details are
-abstracted and re-presented in a more convenient way. - **Fast**: Boosted up by
-aiohttp, a high-performance http library written in C. - **Async**: Fully
-asynchronous (also usable synchronously if wanted, for convenience). -
-**Powerful**: Full access to Bale's API to execute any official client action
-and more. ### Installing ``` bash pip3 install -U pybalebot ```
+## PyBaleBot > Modern and fully asynchronous framework for Bale Bot API ###
+Using Async ```python from pybalebot import Client, filters from
+pybalebot.types import Message bot_token = "123456789:**********************"
+app = Client("my_bot", bot_token=bot_token) @app.on_message(filters.text) async
+def hello(client, message: Message): await message.reply("Hello from
+PyBaleBot!") app.run() ``` **PyBaleBot** is a modern, elegant and asynchronous
+framework. It enables you to easily interact with the main Bale API through a
+user account (custom client) or a bot identity (bot API alternative) using
+Python. ### Key Features - **Ready**: Install PyBaleBot with pip and start
+building your applications right away. - **Easy**: Makes the Bale API simple
+and intuitive, while still allowing advanced usages. - **Elegant**: Low-level
+details are abstracted and re-presented in a more convenient way. - **Fast**:
+Boosted up by aiohttp, a high-performance http library written in C. -
+**Async**: Fully asynchronous (also usable synchronously if wanted, for
+convenience). - **Powerful**: Full access to Bale's API to execute any official
+client action and more. ### Installing ``` bash pip3 install -U pybalebot ```
```

### Comparing `pybalebot-0.0.1/setup.py` & `pybalebot-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requirements = ['aiohttp']
 
 with open('README.md', encoding='UTF-8') as f:
     readme = f.read()
 
 setup(
     name = 'pybalebot',
-    version = '0.0.1',
+    version = '0.0.2',
     author='Shayan Heidari',
     author_email = 'contact@shayanheidari.info',
     description = 'Modern and fully asynchronous framework for Bale Bot API',
     keywords = ['pybalebot', 'bale', 'chat', 'bot', 'robot', 'asyncio'],
     long_description = readme,
     python_requires='~=3.7',
     long_description_content_type = 'text/markdown',
```

