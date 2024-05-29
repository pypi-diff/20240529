# Comparing `tmp/nrich-0.1.0.tar.gz` & `tmp/nrich-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrich-0.1.0.tar", max compression
+gzip compressed data, was "nrich-0.1.2.tar", max compression
```

## Comparing `nrich-0.1.0.tar` & `nrich-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35148 2023-09-22 19:26:46.425773 nrich-0.1.0/LICENSE
--rw-r--r--   0        0        0     1187 2023-09-22 19:26:46.426299 nrich-0.1.0/README.md
--rw-r--r--   0        0        0      388 2023-09-22 19:26:46.430458 nrich-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       61 2023-09-22 19:26:46.430957 nrich-0.1.0/src/nrich/__init__.py
--rw-r--r--   0        0        0     1670 2023-09-22 19:26:46.431660 nrich-0.1.0/src/nrich/__main__.py
--rw-r--r--   0        0        0      747 2023-09-22 19:26:46.432226 nrich-0.1.0/src/nrich/models.py
--rwxr-xr-x   0        0        0     4830 2023-09-22 19:26:46.432946 nrich-0.1.0/src/nrich/nrich.py
--rwxr-xr-x   0        0        0      851 2023-09-22 19:26:46.433730 nrich-0.1.0/src/nrich/parse_internetdb.py
--rw-r--r--   0        0        0     1589 1970-01-01 00:00:00.000000 nrich-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-05-29 08:13:29.114514 nrich-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2165 2024-05-29 08:13:29.114514 nrich-0.1.2/README.md
+-rw-r--r--   0        0        0      388 2024-05-29 08:13:29.118515 nrich-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       61 2024-05-29 08:13:29.118515 nrich-0.1.2/src/nrich/__init__.py
+-rw-r--r--   0        0        0     1670 2024-05-29 08:13:29.118515 nrich-0.1.2/src/nrich/__main__.py
+-rw-r--r--   0        0        0      747 2024-05-29 08:13:29.118515 nrich-0.1.2/src/nrich/models.py
+-rwxr-xr-x   0        0        0     4830 2024-05-29 08:13:29.118515 nrich-0.1.2/src/nrich/nrich.py
+-rwxr-xr-x   0        0        0      851 2024-05-29 08:13:29.118515 nrich-0.1.2/src/nrich/parse_internetdb.py
+-rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 nrich-0.1.2/PKG-INFO
```

### Comparing `nrich-0.1.0/LICENSE` & `nrich-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nrich-0.1.0/src/nrich/__main__.py` & `nrich-0.1.2/src/nrich/__main__.py`

 * *Files identical despite different names*

### Comparing `nrich-0.1.0/src/nrich/models.py` & `nrich-0.1.2/src/nrich/models.py`

 * *Files identical despite different names*

### Comparing `nrich-0.1.0/src/nrich/nrich.py` & `nrich-0.1.2/src/nrich/nrich.py`

 * *Files identical despite different names*

### Comparing `nrich-0.1.0/src/nrich/parse_internetdb.py` & `nrich-0.1.2/src/nrich/parse_internetdb.py`

 * *Files identical despite different names*

### Comparing `nrich-0.1.0/PKG-INFO` & `nrich-0.1.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,15 @@
-Metadata-Version: 2.1
-Name: nrich
-Version: 0.1.0
-Summary: Python equivalant of the rust nrich program. Simple async Python program to interact with the Shodan InternetDB API.
-License: GPLv3
-Author: pimvh
-Requires-Python: ==3.11.4
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Requires-Dist: aiohttp (==3.8.5)
-Description-Content-Type: text/markdown
+# Nrich
 
-# nrich.py
-
-Python equivalent of the rust [nrich](https://gitlab.com/shodan-public/nrich) program, developed by Shodan. Simple async Python program to interact with the Shodan InternetDB API.
+Python equivalent of the Rust [nrich](https://gitlab.com/shodan-public/nrich) program, developed by Shodan. Simple async Python program to interact with the Shodan InternetDB API.
 
 In addition to the official tool, you can specify subnets, and this tool just unpacks them.
 
 ## Usage
 
-### nrich.py
-
 `nrich --help`:
 
 ```
 usage: nrich.py [-h] [-input-file INPUT_FILE] [-output-file OUTPUT_FILE] [-output-type {json,str}] [-skip_missing]
 
 options:
   -h, --help            show this help message and exit
@@ -32,31 +18,54 @@
   -output-file OUTPUT_FILE, -o OUTPUT_FILE
                         file to write IPs to
   -output-type {json,str}, -t {json,str}
                         Format to output in
   -skip_missing, -s     skip IPs with no information on them.
 ```
 
+### Standalone
+
+To run this program as a standalone tool, run:
+
+```
+python3 -m nrich <your command>
+```
+
+For example, you can get the InternetDB information for a single IP, with the following command:
+
+```
+echo -e "<< your IP HERE>>\n" | python3 -m nrich
+INFO:root:creating queue and IPlookup object...
+INFO:root:creating tasks...
+INFO:ShodanLookupper:Starting session...
+INFO:root:running tasks...
+INFO:ShodanLookupper:Got response: ShodanResult(ip=None, cpes=[], hostnames=[], ports=[], tags=[], vulns=[], detail='No information available', empty=False)...
+{"ip": null, "cpes": [], "hostnames": [], "ports": [], "tags": [], "vulns": [], "detail": "No information available", "empty": false}
+```
+
+Any stdout piped input will be consumed by Shodan, when it is a file that contains IPs, line by line. Refer to the `--help` statement for usage when you want to consume files instead.
+
 ### parse_internetdb.py
 
 Example script to parse the shodan internet.db output
 
-# Installation
+## Installation
 
-Make a virtual environment and install dependencies, like so:
+This package is available via PyPi. In order to install you can use the following command
 
 ```
-python3 -m venv venv
-source ./venv/bin/activate
-pip install -r requirements.txt
+pip install nrich
 ```
 
-## Nix users
+### Nix users
+
+For users of nix a flake is avaible. Have a look at flake.nix for the targets.
+
+If you just want a shell where the package is available, run:
 
 ```
 nix develop
 ```
 
 # License
 
 GPLv3, see license.txt
-
```

