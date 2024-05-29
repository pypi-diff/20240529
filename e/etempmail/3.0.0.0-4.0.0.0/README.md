# Comparing `tmp/etempmail-3.0.0.0.tar.gz` & `tmp/etempmail-4.0.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etempmail-3.0.0.0.tar", last modified: Mon Aug 14 12:39:40 2023, max compression
+gzip compressed data, was "etempmail-4.0.0.0.tar", last modified: Wed May 29 14:35:52 2024, max compression
```

## Comparing `etempmail-3.0.0.0.tar` & `etempmail-4.0.0.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-14 12:39:40.269691 etempmail-3.0.0.0/
--rw-rw-rw-   0        0        0     1836 2023-08-14 12:39:40.269127 etempmail-3.0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1264 2023-08-14 12:33:17.000000 etempmail-3.0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-14 12:39:40.259488 etempmail-3.0.0.0/etempmail/
--rw-rw-rw-   0        0        0     3499 2023-08-14 12:35:25.000000 etempmail-3.0.0.0/etempmail/TempMail.py
--rw-rw-rw-   0        0        0      401 2023-08-14 12:07:29.000000 etempmail-3.0.0.0/etempmail/TempMailException.py
--rw-rw-rw-   0        0        0      100 2023-08-14 12:07:29.000000 etempmail-3.0.0.0/etempmail/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-14 12:39:40.265557 etempmail-3.0.0.0/etempmail.egg-info/
--rw-rw-rw-   0        0        0     1836 2023-08-14 12:39:40.000000 etempmail-3.0.0.0/etempmail.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-08-14 12:39:40.000000 etempmail-3.0.0.0/etempmail.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-14 12:39:40.000000 etempmail-3.0.0.0/etempmail.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-08-14 12:39:40.000000 etempmail-3.0.0.0/etempmail.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-08-14 12:39:40.000000 etempmail-3.0.0.0/etempmail.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-14 12:39:40.269691 etempmail-3.0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      960 2023-08-14 12:11:36.000000 etempmail-3.0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:35:52.481554 etempmail-4.0.0.0/
+-rw-rw-rw-   0        0        0     1091 2024-05-29 14:01:02.000000 etempmail-4.0.0.0/LICENSE
+-rw-rw-rw-   0        0        0     1961 2024-05-29 14:35:52.480554 etempmail-4.0.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1340 2024-05-29 14:32:44.000000 etempmail-4.0.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 14:35:52.471040 etempmail-4.0.0.0/etempmail/
+-rw-rw-rw-   0        0        0     2820 2024-05-29 14:34:30.000000 etempmail-4.0.0.0/etempmail/TempMail.py
+-rw-rw-rw-   0        0        0      401 2024-05-29 14:01:02.000000 etempmail-4.0.0.0/etempmail/TempMailException.py
+-rw-rw-rw-   0        0        0      100 2024-05-29 14:01:02.000000 etempmail-4.0.0.0/etempmail/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:35:52.479555 etempmail-4.0.0.0/etempmail.egg-info/
+-rw-rw-rw-   0        0        0     1961 2024-05-29 14:35:52.000000 etempmail-4.0.0.0/etempmail.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-05-29 14:35:52.000000 etempmail-4.0.0.0/etempmail.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 14:35:52.000000 etempmail-4.0.0.0/etempmail.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-29 14:35:52.000000 etempmail-4.0.0.0/etempmail.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-29 14:35:52.000000 etempmail-4.0.0.0/etempmail.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 14:35:52.481554 etempmail-4.0.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      953 2024-05-29 14:21:48.000000 etempmail-4.0.0.0/setup.py
```

### Comparing `etempmail-3.0.0.0/PKG-INFO` & `etempmail-4.0.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 Metadata-Version: 2.1
 Name: etempmail
-Version: 3.0.0.0
-Summary: A simple Python module to get free disposable temporary email address
+Version: 4.0.0.0
+Summary: A simple module to get free disposable temporary email address
 Home-page: https://github.com/mahelbir/etempmail
 Author: Mahmuthan Elbir
 Author-email: me@mahmuthanelbir.com.tr
 License: MIT
 Keywords: temp mail,temporary mail,disposable mail,temp email,etempmail,etempmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests~=2.28.2
 
-# ETempMail
+# etempmail
 
-A simple Python module to get free disposable temporary email address.
+[![PyPI](https://img.shields.io/pypi/v/etempmail)](https://pypi.org/project/etempmail/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/etempmail)](https://pypi.org/project/etempmail/)
+[![PyPI - License](https://img.shields.io/pypi/l/etempmail)](https://pypi.org/project/etempmail/)
+
+A simple module to get free disposable temporary email address.
 
 ## Installation
 
 To install etempmail use pip:
 
 ```bash
 pip install etempmail
@@ -27,37 +33,37 @@
 
 ## Usage
 
 ```python
 from etempmail import TempMail
 
 # recovery: str = None, url: str = 'https://etempmail.com', debug_response: bool = True
-temp_mail = TempMail()  # or TempMail('WHHKSIX7915')
+temp_mail = TempMail()  # or TempMail('OGFHVIX7915')
 
-print(temp_mail.domains())  # response -> (domain_id, domain_name)
-# [('5', 'istanbultaksi.xyz'), ('4', 'privmail.com'), ('2', 'mailers.edu.pl')]
 print(temp_mail.id)
 # 7915
+
 print(temp_mail.email)
-# sidavm5dhc@istanbultaksi.xyz
+# sidavm5dhc@upperbox.xyz
+
 print(temp_mail.recovery)
-# WHHKSIX7915
+# OGFHVIX7915
+
 print(temp_mail.inbox())
 # [{'subject': 'test', 'from': 'Anonymousemail <noreply@gmail.com>', 'date': '16/08/2022 19:40:47', 'body': 'Test Body Code: 123'}]
 
-temp_mail.recover('LHKXDMG7910')  # Recover email address
-temp_mail.change()  # Change email address by random domain
-temp_mail.change(4)  # Change email address by domain_id
+temp_mail.recover('OGFHVSZ115741')  # Recover email address
+temp_mail.change()  # Change email address
 ```
 
 ## Note
 
-You can use the following websites and similars
+You can use the following domains or similar:
 
 + https://etempmail.com
 + https://gecicimail.com.tr
 + https://toprakmail.com
 + https://segamail.com
 
 ## License
 
-The MIT License (MIT). Please see [License File](LISENCE) for more information.
+The MIT License (MIT). Please see [License File](LICENSE) for more information.
```

### Comparing `etempmail-3.0.0.0/README.md` & `etempmail-4.0.0.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,14 @@
-# ETempMail
+# etempmail
 
-A simple Python module to get free disposable temporary email address.
+[![PyPI](https://img.shields.io/pypi/v/etempmail)](https://pypi.org/project/etempmail/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/etempmail)](https://pypi.org/project/etempmail/)
+[![PyPI - License](https://img.shields.io/pypi/l/etempmail)](https://pypi.org/project/etempmail/)
+
+A simple module to get free disposable temporary email address.
 
 ## Installation
 
 To install etempmail use pip:
 
 ```bash
 pip install etempmail
@@ -12,37 +16,37 @@
 
 ## Usage
 
 ```python
 from etempmail import TempMail
 
 # recovery: str = None, url: str = 'https://etempmail.com', debug_response: bool = True
-temp_mail = TempMail()  # or TempMail('WHHKSIX7915')
+temp_mail = TempMail()  # or TempMail('OGFHVIX7915')
 
-print(temp_mail.domains())  # response -> (domain_id, domain_name)
-# [('5', 'istanbultaksi.xyz'), ('4', 'privmail.com'), ('2', 'mailers.edu.pl')]
 print(temp_mail.id)
 # 7915
+
 print(temp_mail.email)
-# sidavm5dhc@istanbultaksi.xyz
+# sidavm5dhc@upperbox.xyz
+
 print(temp_mail.recovery)
-# WHHKSIX7915
+# OGFHVIX7915
+
 print(temp_mail.inbox())
 # [{'subject': 'test', 'from': 'Anonymousemail <noreply@gmail.com>', 'date': '16/08/2022 19:40:47', 'body': 'Test Body Code: 123'}]
 
-temp_mail.recover('LHKXDMG7910')  # Recover email address
-temp_mail.change()  # Change email address by random domain
-temp_mail.change(4)  # Change email address by domain_id
+temp_mail.recover('OGFHVSZ115741')  # Recover email address
+temp_mail.change()  # Change email address
 ```
 
 ## Note
 
-You can use the following websites and similars
+You can use the following domains or similar:
 
 + https://etempmail.com
 + https://gecicimail.com.tr
 + https://toprakmail.com
 + https://segamail.com
 
 ## License
 
-The MIT License (MIT). Please see [License File](LISENCE) for more information.
+The MIT License (MIT). Please see [License File](LICENSE) for more information.
```

### Comparing `etempmail-3.0.0.0/etempmail/TempMail.py` & `etempmail-4.0.0.0/etempmail/TempMail.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,82 +1,71 @@
-from requests import session, get
-from json import loads as json_decode
-from re import findall
+import requests
+
 from etempmail.TempMailException import TempMailException
 
 
 class TempMail:
     id = None
     email = None
     recovery = None
 
     def __init__(self, recovery: str = None, url: str = 'https://etempmail.com', debug_response: bool = True):
         self.debug_response = debug_response
         self.url = url
-        self.__session = session()
+        self.__session = requests.session()
         self.__headers = {
-            'accept': 'application/json',
-            'accept-language': 'en-US',
+            'accept': '*/*',
+            'accept-language': 'en-US,en;q=0.8',
             'origin': self.url,
-            'referer': self.url,
-            'sec-ch-ua': '"Not/A)Brand";v="99", "Opera";v="101", "Chromium";v="115"',
+            'priority': 'u=1, i',
+            'referer': self.url + '/',
+            'sec-ch-ua': '"Google Chrome";v="125", "Chromium";v="125", "Not.A/Brand";v="24"',
             'sec-ch-ua-mobile': '?0',
             'sec-ch-ua-platform': '"Windows"',
             'sec-fetch-dest': 'empty',
             'sec-fetch-mode': 'cors',
             'sec-fetch-site': 'same-origin',
-            'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/115.0.0.0 Safari/537.36 OPR/101.0.0.0',
+            'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/125.0.0.0 Safari/537.36',
+            'x-kl-ajax-request': 'Ajax_Request',
             'x-requested-with': 'XMLHttpRequest',
         }
         if recovery:
             self.recover(recovery)
         else:
             self.__get_email()
 
     def __get_email(self):
         response = self.__session.post(f'{self.url}/getEmailAddress', headers=self.__headers)
         try:
-            json = json_decode(response.content)
+            json = response.json()
             self.id = int(json['id'])
             self.email = json['address']
             self.recovery = json['recover_key']
         except Exception:
             raise TempMailException('get_email', 'request', response, self.debug_response)
 
-    def domains(self) -> list:
-        response = get(self.url, headers=self.__headers)
-        if response.status_code != 200:
-            raise TempMailException('domains', 'request', response, self.debug_response)
-        else:
-            return findall(r'<option value="(\d+)".*?>(.+?)</option>', response.text)
-
     def inbox(self) -> list:
         response = self.__session.post(f'{self.url}/getInbox', headers=self.__headers)
         try:
-            json = json_decode(response.content)
+            json = response.json()
             return json
         except Exception:
             raise TempMailException('inbox', 'request', response, self.debug_response)
 
     def recover(self, recovery: str):
         if recovery:
             response = self.__session.post(f'{self.url}/recoverEmailAddress', headers=self.__headers, data={
                 'key': recovery
             })
             try:
-                json = json_decode(response.content)
+                json = response.json()
             except Exception:
                 raise TempMailException('recovery', 'request', response, self.debug_response)
             if not json['success']:
                 raise TempMailException('recovery', 'key', response, self.debug_response)
         self.__get_email()
 
-    def change(self, domain_id: str | int = None):
-        if not domain_id:
-            response = self.__session.post(f'{self.url}/deleteEmailAddress', headers=self.__headers)
-        else:
-            response = self.__session.post(f'{self.url}/changeEmailAddress', headers=self.__headers, data={
-                'id': domain_id
-            }, allow_redirects=False)
-        if (not domain_id and response.status_code != 200) or (domain_id and response.status_code != 302):
+    def change(self):
+        response = self.__session.post(f'{self.url}/deleteEmailAddress', headers=self.__headers)
+        if response.status_code != 200:
             raise TempMailException('change', 'request', response)
         self.__get_email()
```

### Comparing `etempmail-3.0.0.0/etempmail.egg-info/PKG-INFO` & `etempmail-4.0.0.0/etempmail.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 Metadata-Version: 2.1
 Name: etempmail
-Version: 3.0.0.0
-Summary: A simple Python module to get free disposable temporary email address
+Version: 4.0.0.0
+Summary: A simple module to get free disposable temporary email address
 Home-page: https://github.com/mahelbir/etempmail
 Author: Mahmuthan Elbir
 Author-email: me@mahmuthanelbir.com.tr
 License: MIT
 Keywords: temp mail,temporary mail,disposable mail,temp email,etempmail,etempmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests~=2.28.2
 
-# ETempMail
+# etempmail
 
-A simple Python module to get free disposable temporary email address.
+[![PyPI](https://img.shields.io/pypi/v/etempmail)](https://pypi.org/project/etempmail/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/etempmail)](https://pypi.org/project/etempmail/)
+[![PyPI - License](https://img.shields.io/pypi/l/etempmail)](https://pypi.org/project/etempmail/)
+
+A simple module to get free disposable temporary email address.
 
 ## Installation
 
 To install etempmail use pip:
 
 ```bash
 pip install etempmail
@@ -27,37 +33,37 @@
 
 ## Usage
 
 ```python
 from etempmail import TempMail
 
 # recovery: str = None, url: str = 'https://etempmail.com', debug_response: bool = True
-temp_mail = TempMail()  # or TempMail('WHHKSIX7915')
+temp_mail = TempMail()  # or TempMail('OGFHVIX7915')
 
-print(temp_mail.domains())  # response -> (domain_id, domain_name)
-# [('5', 'istanbultaksi.xyz'), ('4', 'privmail.com'), ('2', 'mailers.edu.pl')]
 print(temp_mail.id)
 # 7915
+
 print(temp_mail.email)
-# sidavm5dhc@istanbultaksi.xyz
+# sidavm5dhc@upperbox.xyz
+
 print(temp_mail.recovery)
-# WHHKSIX7915
+# OGFHVIX7915
+
 print(temp_mail.inbox())
 # [{'subject': 'test', 'from': 'Anonymousemail <noreply@gmail.com>', 'date': '16/08/2022 19:40:47', 'body': 'Test Body Code: 123'}]
 
-temp_mail.recover('LHKXDMG7910')  # Recover email address
-temp_mail.change()  # Change email address by random domain
-temp_mail.change(4)  # Change email address by domain_id
+temp_mail.recover('OGFHVSZ115741')  # Recover email address
+temp_mail.change()  # Change email address
 ```
 
 ## Note
 
-You can use the following websites and similars
+You can use the following domains or similar:
 
 + https://etempmail.com
 + https://gecicimail.com.tr
 + https://toprakmail.com
 + https://segamail.com
 
 ## License
 
-The MIT License (MIT). Please see [License File](LISENCE) for more information.
+The MIT License (MIT). Please see [License File](LICENSE) for more information.
```

### Comparing `etempmail-3.0.0.0/setup.py` & `etempmail-4.0.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 pkg_name = "etempmail"
 setuptools.setup(
     name=pkg_name,
-    version="3.0.0.0",
+    version="4.0.0.0",
     author="Mahmuthan Elbir",
     author_email="me@mahmuthanelbir.com.tr",
-    description="A simple Python module to get free disposable temporary email address",
+    description="A simple module to get free disposable temporary email address",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=['temp mail', 'temporary mail', 'disposable mail', 'temp email', 'etempmail', 'etempmail.com'],
     license="MIT",
     url="https://github.com/mahelbir/etempmail",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=[pkg_name],
     include_package_data=True,
     install_requires=[
-        "requests~=2.31.0"
+        "requests~=2.28.2"
     ],
     python_requires=">=3.7"
 )
```

