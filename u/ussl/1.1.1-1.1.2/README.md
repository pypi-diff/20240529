# Comparing `tmp/ussl-1.1.1.tar.gz` & `tmp/ussl-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ussl-1.1.1.tar", last modified: Fri Apr 26 10:24:44 2024, max compression
+gzip compressed data, was "dist\ussl-1.1.2.tar", last modified: Wed May 29 08:14:40 2024, max compression
```

## Comparing `ussl-1.1.1.tar` & `ussl-1.1.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 10:24:44.211096 ussl-1.1.1/
--rw-rw-rw-   0        0        0    15145 2024-04-26 10:24:44.205865 ussl-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    14493 2024-03-01 08:27:08.000000 ussl-1.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-26 10:24:44.211096 ussl-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1681 2024-04-26 10:24:31.000000 ussl-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-26 10:24:44.157381 ussl-1.1.1/ussl/
--rw-rw-rw-   0        0        0       49 2024-03-01 08:27:08.000000 ussl-1.1.1/ussl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 10:24:44.177040 ussl-1.1.1/ussl/exceptions/
--rw-rw-rw-   0        0        0      305 2024-03-01 08:27:08.000000 ussl-1.1.1/ussl/exceptions/__init__.py
--rw-rw-rw-   0        0        0     1369 2024-04-26 07:05:38.000000 ussl-1.1.1/ussl/exceptions/main.py
--rw-rw-rw-   0        0        0     1126 2024-03-01 08:27:08.000000 ussl-1.1.1/ussl/exceptions/protocol_exc.py
--rw-rw-rw-   0        0        0     1084 2024-03-01 08:27:08.000000 ussl-1.1.1/ussl/exceptions/validation_exc.py
-drwxrwxrwx   0        0        0        0 2024-04-26 10:24:44.179042 ussl-1.1.1/ussl/model/
--rw-rw-rw-   0        0        0     4312 2024-04-26 07:05:38.000000 ussl-1.1.1/ussl/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 10:24:44.182945 ussl-1.1.1/ussl/postprocessing/
--rw-rw-rw-   0        0        0        0 2024-03-01 08:27:08.000000 ussl-1.1.1/ussl/postprocessing/__init__.py
--rw-rw-rw-   0        0        0     6999 2024-04-26 07:05:38.000000 ussl-1.1.1/ussl/postprocessing/base.py
-drwxrwxrwx   0        0        0        0 2024-04-26 10:24:44.198877 ussl-1.1.1/ussl/protocol/
--rw-rw-rw-   0        0        0      673 2024-04-26 07:05:38.000000 ussl-1.1.1/ussl/protocol/__init__.py
--rw-rw-rw-   0        0        0      562 2024-04-26 07:05:38.000000 ussl-1.1.1/ussl/protocol/base.py
--rw-rw-rw-   0        0        0     1480 2024-04-26 07:05:38.000000 ussl-1.1.1/ussl/protocol/ldap.py
--rw-rw-rw-   0        0        0     3999 2024-04-26 07:05:38.000000 ussl-1.1.1/ussl/protocol/ssh.py
--rw-rw-rw-   0        0        0        0 2024-01-24 09:57:50.000000 ussl-1.1.1/ussl/protocol/winexe.py
--rw-rw-rw-   0        0        0     6120 2024-04-26 07:05:38.000000 ussl-1.1.1/ussl/protocol/winrm.py
--rw-rw-rw-   0        0        0        0 2024-01-24 09:57:50.000000 ussl-1.1.1/ussl/protocol/wmi.py
-drwxrwxrwx   0        0        0        0 2024-04-26 10:24:44.199876 ussl-1.1.1/ussl/transport/
--rw-rw-rw-   0        0        0     1508 2024-03-01 08:27:08.000000 ussl-1.1.1/ussl/transport/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 10:24:44.202448 ussl-1.1.1/ussl/utils/
--rw-rw-rw-   0        0        0     6424 2024-03-01 08:27:08.000000 ussl-1.1.1/ussl/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 10:24:44.167336 ussl-1.1.1/ussl.egg-info/
--rw-rw-rw-   0        0        0    15145 2024-04-26 10:24:44.000000 ussl-1.1.1/ussl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      584 2024-04-26 10:24:44.000000 ussl-1.1.1/ussl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 10:24:44.000000 ussl-1.1.1/ussl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2024-04-26 10:24:44.000000 ussl-1.1.1/ussl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-26 10:24:44.000000 ussl-1.1.1/ussl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 08:14:40.939039 ussl-1.1.2/
+-rw-rw-rw-   0        0        0    15145 2024-05-29 08:14:40.933957 ussl-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    14493 2024-03-01 08:27:08.000000 ussl-1.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-29 08:14:40.939039 ussl-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     2233 2024-05-29 08:14:26.000000 ussl-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:14:40.888211 ussl-1.1.2/ussl/
+-rw-rw-rw-   0        0        0       49 2024-03-01 08:27:08.000000 ussl-1.1.2/ussl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:14:40.906903 ussl-1.1.2/ussl/exceptions/
+-rw-rw-rw-   0        0        0      305 2024-03-01 08:27:08.000000 ussl-1.1.2/ussl/exceptions/__init__.py
+-rw-rw-rw-   0        0        0     1369 2024-05-22 08:57:11.000000 ussl-1.1.2/ussl/exceptions/main.py
+-rw-rw-rw-   0        0        0     1126 2024-03-01 08:27:08.000000 ussl-1.1.2/ussl/exceptions/protocol_exc.py
+-rw-rw-rw-   0        0        0     1084 2024-03-01 08:27:08.000000 ussl-1.1.2/ussl/exceptions/validation_exc.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:14:40.909669 ussl-1.1.2/ussl/model/
+-rw-rw-rw-   0        0        0     4596 2024-05-29 08:13:26.000000 ussl-1.1.2/ussl/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:14:40.913052 ussl-1.1.2/ussl/postprocessing/
+-rw-rw-rw-   0        0        0        0 2024-03-01 08:27:08.000000 ussl-1.1.2/ussl/postprocessing/__init__.py
+-rw-rw-rw-   0        0        0     7260 2024-05-29 08:13:26.000000 ussl-1.1.2/ussl/postprocessing/base.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:14:40.926767 ussl-1.1.2/ussl/protocol/
+-rw-rw-rw-   0        0        0      798 2024-05-29 08:13:26.000000 ussl-1.1.2/ussl/protocol/__init__.py
+-rw-rw-rw-   0        0        0      711 2024-05-29 08:13:26.000000 ussl-1.1.2/ussl/protocol/base.py
+-rw-rw-rw-   0        0        0     1534 2024-05-29 08:13:26.000000 ussl-1.1.2/ussl/protocol/ldap.py
+-rw-rw-rw-   0        0        0     4610 2024-05-29 08:13:26.000000 ussl-1.1.2/ussl/protocol/ssh.py
+-rw-rw-rw-   0        0        0        0 2024-01-24 09:57:50.000000 ussl-1.1.2/ussl/protocol/winexe.py
+-rw-rw-rw-   0        0        0     8202 2024-05-29 08:13:26.000000 ussl-1.1.2/ussl/protocol/winrm.py
+-rw-rw-rw-   0        0        0      303 2024-05-29 08:13:26.000000 ussl-1.1.2/ussl/protocol/wmi.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:14:40.928101 ussl-1.1.2/ussl/transport/
+-rw-rw-rw-   0        0        0     1508 2024-03-01 08:27:08.000000 ussl-1.1.2/ussl/transport/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:14:40.931045 ussl-1.1.2/ussl/utils/
+-rw-rw-rw-   0        0        0     6424 2024-03-01 08:27:08.000000 ussl-1.1.2/ussl/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:14:40.897403 ussl-1.1.2/ussl.egg-info/
+-rw-rw-rw-   0        0        0    15145 2024-05-29 08:14:40.000000 ussl-1.1.2/ussl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      584 2024-05-29 08:14:40.000000 ussl-1.1.2/ussl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 08:14:40.000000 ussl-1.1.2/ussl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2024-05-29 08:14:40.000000 ussl-1.1.2/ussl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-29 08:14:40.000000 ussl-1.1.2/ussl.egg-info/top_level.txt
```

### Comparing `ussl-1.1.1/PKG-INFO` & `ussl-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ussl
-Version: 1.1.1
+Version: 1.1.2
 Summary: Пакет разработчиков USSC-SOC для упрощения взаимодействия с АРМ, серверами и сетевыми устройствами
 Author: ussc soc dev team
 Author-email: iushangaraev@ussc.ru, pbikkuzhina@ussc.ru
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
```

### Comparing `ussl-1.1.1/README.md` & `ussl-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ussl-1.1.1/setup.py` & `ussl-1.1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 import logging
 import sys
+import platform
 
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 
 if 'win' in sys.platform.lower():
     logging.info('For the LDAP protocol to work correctly, install the dependency:')
-    logging.info('\tpip install https://github.com/cgohlke/python-ldap-build/releases/download/v3.4.4/python_ldap-3.4.4-cp38-cp38-win_amd64.whl')
+    if not platform.python_version().startswith('3.8'):
+        logging.info('Find the version you need on https://github.com/cgohlke/python-ldap-build/releases/')
+    if platform.architecture()[0] == '64bit':
+        logging.info('\tpip install https://github.com/cgohlke/python-ldap-build/releases/download/v3.4.4/python_ldap-3.4.4-cp38-cp38-win_amd64.whl')
+    elif platform.architecture()[0] == '32bit':
+        logging.info('\tpip install https://github.com/cgohlke/python-ldap-build/releases/download/v3.4.4/python_ldap-3.4.4-cp38-cp38-win32.whl')
+    else:
+        logging.info('Find the version you need on https://github.com/cgohlke/python-ldap-build/releases/')
+
 
 setup(
     name='ussl',
     author='ussc soc dev team',
     author_email='iushangaraev@ussc.ru, pbikkuzhina@ussc.ru',
     description='Пакет разработчиков USSC-SOC для упрощения взаимодействия с АРМ, серверами и сетевыми устройствами',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.1.1',
+    version='1.1.2',
     python_requires='>=3.8.0',
     packages=[
         'ussl',
         'ussl.model',
         'ussl.postprocessing',
         'ussl.protocol',
         'ussl.transport',
```

### Comparing `ussl-1.1.1/ussl/exceptions/main.py` & `ussl-1.1.2/ussl/exceptions/main.py`

 * *Files identical despite different names*

### Comparing `ussl-1.1.1/ussl/exceptions/protocol_exc.py` & `ussl-1.1.2/ussl/exceptions/protocol_exc.py`

 * *Files identical despite different names*

### Comparing `ussl-1.1.1/ussl/exceptions/validation_exc.py` & `ussl-1.1.2/ussl/exceptions/validation_exc.py`

 * *Files identical despite different names*

### Comparing `ussl-1.1.1/ussl/model/__init__.py` & `ussl-1.1.2/ussl/model/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,36 +3,39 @@
 
 
 @dataclass
 class Response:
     """
     Класс, описывающий ответ от конечной системы.
 
-        ``result``: содержит исходный ответ от целевой системы;
-        ``text``: содержится форматированный ответ от целевой системы;
-        ``status``: содержится статус выполнения переданной команды.
+        ``result``: содержит результат выполнения переданной команды;
+        ``stdout``: содержится форматированный ответ от целевой системы;
+        ``stderr``: содержится ошибка выполнения переданной команды;
+        ``status_code``: содержится статус код выполнения переданной команды.
     """
     result: str
-    text: Optional[str] = None
-    status: Optional[bool] = None
+    stdout: Optional[str] = None
+    stderr: Optional[str] = None
+    status_code: Optional[int] = None
 
 
 @dataclass
 class Query:
     """
     Класс, описывающий запросы, передаваемые конечной системе.
 
         ``command``: содержит командe, которую необходимо выполнить;
         ``timeout``: содержит время, отведенное на выпонение команды;
         ``expects``: содержит регулярные выражения, которые описывают
         ожидаемый ответ от конечной системы;
+        ``shell_type``: содержит тип команды (cmd, powershell, и т.д.);
         ``sudo``: содержит пароль от супер пользователя или enable.
     """
     command: str
-    timeout: int = None
+    timeout: Optional[int] = None
     shell_type: Optional[str] = 'cmd'
     sudo: Optional[str] = None
 
 
 @dataclass
 class Protocol:
     """
```

### Comparing `ussl-1.1.1/ussl/postprocessing/base.py` & `ussl-1.1.2/ussl/postprocessing/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,22 +23,24 @@
     """
     Является базовым классом для всех скриптов, участвующих в обогащении и реагировании. При использовании класса
     необходимо реализовать метод ``function``. Автоматически принимаемые значения: ``input_json``: Первым аргументом
     принимает информацию, переданную на вход плейбука; ``secrets``: Вторым аргументом приниает секреты.
     ``ensure_ascii``: Указывает, должны ли символы не из набора ASCII быть экранированы. По умолчанию False.
     ``DEBUG_MODE``: Режим отладки выключает обработку исключений (кроме валидации данных) в формат json для вывода
     всего StackTrace (по умолчанию False).
+    ``RETURN_CODE_IGNORE``: Режим обработки ошибок, при котором из скрипта не будет выводиться ненулевой status_code.
     """
     inputs_model: Type[Schema] = None
     secrets_model: Type[Schema] = None
     ensure_ascii: bool = False
     _input_json: dict = None
     _secrets: dict = None
 
     DEBUG_MODE = False
+    RETURN_CODE_IGNORE = False
 
     def __init__(self, ensure_ascii: bool = False) -> None:
         """
         Инициализирует экземпляр класса.
         Вызывает чтение и валидацию данных. А также, выполнение функции скрипта.
         Args:
             ``ensure_ascii (bool)``: Указывает, должны ли символы не из набора ASCII быть экранированы. По умолчанию False
@@ -140,8 +142,9 @@
         # Обновляем входной JSON новыми аргументами
         self._input_json.update(kwargs)
 
         # Выводим входной JSON в форматированном виде
         print(json.dumps(self._input_json, ensure_ascii=self.ensure_ascii))
 
         # Завершаем выполнение скрипта с кодом 0 в случае успешного выполнения или ненулевым в случае ошибки
-        exit(return_code)
+        if not self.RETURN_CODE_IGNORE:
+            exit(return_code)
```

### Comparing `ussl-1.1.1/ussl/protocol/__init__.py` & `ussl-1.1.2/ussl/protocol/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import logging
 import sys
 
 from .winrm import WinRMProtocol
 from .ssh import SSHProtocol
 
+INTERFACES = {
+    'ssh': SSHProtocol,
+    # 'winexe': WinexeProtocol,
+    # 'wmi': WMIProtocol,
+    'winrm': WinRMProtocol
+}
+
 try:
     from .ldap import LDAPProtocol
+    INTERFACES['ldap'] = LDAPProtocol
 except ImportError:
     logging.warning('For the LDAP protocol to work correctly, install the dependency:')
     if 'win' in sys.platform.lower():
         logging.warning('\tpip install https://github.com/cgohlke/python-ldap-build/releases/download/v3.4.4/python_ldap-3.4.4-cp38-cp38-win_amd64.whl')
+        logging.info('Or find the version you need on https://github.com/cgohlke/python-ldap-build/releases/')
     else:
         logging.warning('\tpip install python-ldap==3.4.4')
-
-INTERFACES = {
-    'ssh': SSHProtocol,
-    # 'winexe': WinexeProtocol,
-    # 'wmi': WMIProtocol,
-    'winrm': WinRMProtocol,
-    'ldap': LDAPProtocol,
-}
```

### Comparing `ussl-1.1.1/ussl/protocol/ldap.py` & `ussl-1.1.2/ussl/protocol/ldap.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,28 +7,29 @@
 from .base import BaseProtocol
 from ..exceptions import CredentialsError, ConnectionFailed, ExecutionError
 
 
 class LDAPProtocol(BaseProtocol):
     name = 'ldap'
 
-    def __init__(self):
+    def __init__(self, protocol: Optional[Protocol] = None):
+        super().__init__(protocol)
         self.base: Optional[str] = None
         self.con: Optional[LDAPObject] = None
 
-    def connect(self, protocol: Protocol) -> LDAPObject:
+    def connect(self) -> None:
+        protocol = self.protocol
         server = f'ldap://{protocol.host}'
         ldap_login = f'{protocol.username}@{protocol.domain}'
         self.base = ', '.join(f'dc={i}' for i in protocol.domain.split('.'))
         try:
             self.con = ldap.initialize(server, bytes_mode=False)
             self.con.protocol_version = ldap.VERSION3
             self.con.set_option(ldap.OPT_REFERRALS, 0)
             self.con.simple_bind_s(ldap_login, protocol.password)
-            return self.con
         except ldap.INVALID_CREDENTIALS as e:
             raise CredentialsError(str(e))
         except ldap.SERVER_DOWN as e:
             raise ConnectionFailed(str(e))
         except Exception as e:
             raise ExecutionError(str(e))
 
@@ -36,8 +37,8 @@
         try:
             self.con.unbind()
         except Exception as e:
             raise ExecutionError("Unknown error while closing connection: " + str(e))
         self.con = None
 
     def execute(self, query: Query) -> Response:
-        pass
+        pass
```

### Comparing `ussl-1.1.1/ussl/protocol/ssh.py` & `ussl-1.1.2/ussl/protocol/ssh.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import io
 import socket
 import time
-from typing import Optional
+from typing import Optional, Self, Union
 
 import paramiko
 from paramiko.rsakey import RSAKey
 from paramiko.ssh_exception import AuthenticationException, SSHException
 
 from ..model import Protocol, Query, Response
 from .base import BaseProtocol
@@ -26,43 +26,48 @@
     :param EXEC_COMMAND_TIMEOUT: an optional timeout (in seconds)
         for execute command
     """
 
     SSH_CONNECT_TIMEOUT: int = 60
     EXEC_COMMAND_TIMEOUT: int = 60
 
+    _connection: Optional[paramiko.SSHClient] = None
+
     def __init__(self, protocol: Optional[Protocol] = None):
+        super().__init__(protocol)
         if not self._connection and protocol:
-            self.connect(protocol)
+            self.connect()
 
-    def connect(self, protocol: Protocol):
+    def connect(self):
         """Open SSH connection to remote host.
 
         :raises: CreateSSHConnectionError: if failed authentication
             or connection or establishing an SSH session
         """
+        protocol = self.protocol
         host = protocol.host
         login = protocol.username
+        domain = protocol.domain
+        if domain is not None:
+            login = f'{login}@{domain}'
         password = protocol.password
-        port = protocol.port
+        port = protocol.port or 22
         ssh_key = protocol.pem_file
         try:
+            self._connection = paramiko.SSHClient()
+            self._connection.set_missing_host_key_policy(paramiko.AutoAddPolicy())
             if password:
-                self._connection = paramiko.SSHClient()
-                self._connection.set_missing_host_key_policy(paramiko.AutoAddPolicy())
                 self._connection.connect(
                     hostname=host, username=login,
                     password=password, port=port,
                     look_for_keys=False, allow_agent=False,
                     timeout=SSHProtocol.SSH_CONNECT_TIMEOUT
                 )
             elif ssh_key:
                 keyfile = io.StringIO(ssh_key)
-                self._connection = paramiko.SSHClient()
-                self._connection.set_missing_host_key_policy(paramiko.AutoAddPolicy())
                 self._connection.connect(
                     host, port, login,
                     pkey=RSAKey.from_private_key(keyfile),
                     timeout=SSHProtocol.SSH_CONNECT_TIMEOUT,
                     look_for_keys=False,
                     allow_agent=False
                 )
@@ -75,35 +80,46 @@
 
     def close(self):
         """Close SSH connection."""
         if self._connection is not None:
             self._connection.close()
             self._connection = None
 
-    def __enter__(self):
+    def __enter__(self) -> Self:
         self.connect()
         return self
 
     def __exit__(self, exc_type: Exception, *args):
-        self.close()
+        self.close()  ## TODO: fix
         if exc_type is not None:
             return False
         return True
 
-    def execute(self, query: Query) -> Response:
+    def execute(self, query: Union[Query, str]) -> Response:
+        if isinstance(query, str):
+            query = Query(command=query)
         command = query.command
         sudo = query.sudo
-        timeout = query.timeout
+        timeout = query.timeout if query.timeout else SSHProtocol.EXEC_COMMAND_TIMEOUT
         if self._connection is None:
             self.connect()
         stdin, stdout, err = self._connection.exec_command(
             command=command,
             timeout=timeout)
         if sudo:
             stdin.write(sudo + "\n")
             stdin.flush()
             time.sleep(1)
+        stdout = stdout.read().decode('utf-8')
         error = err.read().decode('utf-8')
         if not stdout and error:
-            raise ExecutionError(error + stdout.read().decode('utf-8') + f'\nCommand: {command}')
+            if self.EXECUTE_ERROR_IGNORE:
+                return Response(result=f'Command "{command}" executed failed',
+                                status_code=1,
+                                stderr=error,
+                                stdout=stdout)
+            raise ExecutionError(error + stdout + f'\nCommand: {command}')
         else:
-            return Response(result=stdout.read().decode('utf-8'), status=True, text='Command executed successfully')
+            return Response(result='Command executed successfully',
+                            status_code=0,
+                            stdout=stdout,
+                            stderr=error)
```

### Comparing `ussl-1.1.1/ussl/transport/__init__.py` & `ussl-1.1.2/ussl/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `ussl-1.1.1/ussl/utils/__init__.py` & `ussl-1.1.2/ussl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ussl-1.1.1/ussl.egg-info/PKG-INFO` & `ussl-1.1.2/ussl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ussl
-Version: 1.1.1
+Version: 1.1.2
 Summary: Пакет разработчиков USSC-SOC для упрощения взаимодействия с АРМ, серверами и сетевыми устройствами
 Author: ussc soc dev team
 Author-email: iushangaraev@ussc.ru, pbikkuzhina@ussc.ru
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
```

### Comparing `ussl-1.1.1/ussl.egg-info/SOURCES.txt` & `ussl-1.1.2/ussl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

