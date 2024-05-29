# Comparing `tmp/linien_common-2.0.2.tar.gz` & `tmp/linien_common-2.0.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linien_common-2.0.2.tar", last modified: Tue May 14 13:14:32 2024, max compression
+gzip compressed data, was "linien_common-2.0.3rc1.tar", last modified: Wed May 29 11:52:15 2024, max compression
```

## Comparing `linien_common-2.0.2.tar` & `linien_common-2.0.3rc1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:14:32.670764 linien_common-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-14 13:14:32.670764 linien_common-2.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:14:32.670764 linien_common-2.0.2/linien_common/
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-14 13:14:26.000000 linien_common-2.0.2/linien_common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9767 2024-05-14 13:14:26.000000 linien_common-2.0.2/linien_common/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-14 13:14:26.000000 linien_common-2.0.2/linien_common/communication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-14 13:14:26.000000 linien_common-2.0.2/linien_common/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-14 13:14:26.000000 linien_common-2.0.2/linien_common/influxdb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:14:32.670764 linien_common-2.0.2/linien_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-14 13:14:32.000000 linien_common-2.0.2/linien_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-14 13:14:32.000000 linien_common-2.0.2/linien_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:14:32.000000 linien_common-2.0.2/linien_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-14 13:14:32.000000 linien_common-2.0.2/linien_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 13:14:32.000000 linien_common-2.0.2/linien_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-14 13:14:26.000000 linien_common-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 13:14:32.670764 linien_common-2.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:52:15.894358 linien_common-2.0.3rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-29 11:52:15.894358 linien_common-2.0.3rc1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:52:15.894358 linien_common-2.0.3rc1/linien_common/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-29 11:52:11.000000 linien_common-2.0.3rc1/linien_common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9767 2024-05-29 11:52:11.000000 linien_common-2.0.3rc1/linien_common/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-29 11:52:11.000000 linien_common-2.0.3rc1/linien_common/communication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-29 11:52:11.000000 linien_common-2.0.3rc1/linien_common/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-05-29 11:52:11.000000 linien_common-2.0.3rc1/linien_common/influxdb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:52:15.894358 linien_common-2.0.3rc1/linien_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-29 11:52:15.000000 linien_common-2.0.3rc1/linien_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-29 11:52:15.000000 linien_common-2.0.3rc1/linien_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 11:52:15.000000 linien_common-2.0.3rc1/linien_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-29 11:52:15.000000 linien_common-2.0.3rc1/linien_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-29 11:52:15.000000 linien_common-2.0.3rc1/linien_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-29 11:52:11.000000 linien_common-2.0.3rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 11:52:15.894358 linien_common-2.0.3rc1/setup.cfg
```

### Comparing `linien_common-2.0.2/PKG-INFO` & `linien_common-2.0.3rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-common
-Version: 2.0.2
+Version: 2.0.3rc1
 Summary: Shared components of the Linien spectroscopy lock application.
 Author-email: Benjamin Wiegand <benjamin.wiegand@physik.hu-berlin.de>, Bastian Leykauf <leykauf@physik.hu-berlin.de>, Robert Jördens <rj@quartiq.de>, Christian Freier <christian.freier@gmail.com>, Doron Behar <doron.behar@gmail.com>
 Maintainer-email: Bastian Leykauf <leykauf@physik.hu-berlin.de>
 Project-URL: Homepage, https://github.com/linien-org/linien
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `linien_common-2.0.2/linien_common/__init__.py` & `linien_common-2.0.3rc1/linien_common/__init__.py`

 * *Files identical despite different names*

### Comparing `linien_common-2.0.2/linien_common/common.py` & `linien_common-2.0.3rc1/linien_common/common.py`

 * *Files identical despite different names*

### Comparing `linien_common-2.0.2/linien_common/communication.py` & `linien_common-2.0.3rc1/linien_common/communication.py`

 * *Files identical despite different names*

### Comparing `linien_common-2.0.2/linien_common/config.py` & `linien_common-2.0.3rc1/linien_common/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,21 +11,37 @@
 # Linien is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
-
+import logging
 from pathlib import Path
 
 from appdirs import AppDirs
 
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.DEBUG)
+
 ACQUISITION_PORT = 19321
 SERVER_PORT = 18862
 DEFAULT_SWEEP_SPEED = (125 * 2048) << 6
 
 USER_DATA_PATH = Path(AppDirs("linien").user_data_dir)
 USER_DATA_PATH.mkdir(parents=True, exist_ok=True)
 
 LOG_FILE_PATH = USER_DATA_PATH / "linien.log"
 LOG_FILE_PATH.parent.mkdir(parents=True, exist_ok=True)
+
+
+def create_backup_file(filename: Path) -> None:
+    """Rename the file to a unique filename."""
+    i = 0
+    while True:
+        backup_filename = filename.parent / f"{filename.stem}.backup{i}"
+        if not backup_filename.exists():
+            break
+        i += 1
+
+    filename.rename(backup_filename)
+    logger.info(f"{filename} has been saved as {backup_filename}.")
```

### Comparing `linien_common-2.0.2/linien_common/influxdb.py` & `linien_common-2.0.3rc1/linien_common/influxdb.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 import json
 import logging
 from dataclasses import dataclass
 
-from .config import USER_DATA_PATH
+from .config import USER_DATA_PATH, create_backup_file
 
 CREDENTIAL_STORE_FILENAME = "influxdb_credentials.json"
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
 
@@ -65,7 +65,11 @@
             org=data["org"],
             token=data["token"],
             bucket=data["bucket"],
             measurement=data["measurement"],
         )
     except FileNotFoundError:
         return InfluxDBCredentials()
+    except json.JSONDecodeError:
+        logger.error(f"Credentials file {filename} was corrupted.")
+        create_backup_file(filename)
+        return InfluxDBCredentials()
```

### Comparing `linien_common-2.0.2/linien_common.egg-info/PKG-INFO` & `linien_common-2.0.3rc1/linien_common.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-common
-Version: 2.0.2
+Version: 2.0.3rc1
 Summary: Shared components of the Linien spectroscopy lock application.
 Author-email: Benjamin Wiegand <benjamin.wiegand@physik.hu-berlin.de>, Bastian Leykauf <leykauf@physik.hu-berlin.de>, Robert Jördens <rj@quartiq.de>, Christian Freier <christian.freier@gmail.com>, Doron Behar <doron.behar@gmail.com>
 Maintainer-email: Bastian Leykauf <leykauf@physik.hu-berlin.de>
 Project-URL: Homepage, https://github.com/linien-org/linien
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `linien_common-2.0.2/pyproject.toml` & `linien_common-2.0.3rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "linien-common"
-version = "2.0.2"
+version = "2.0.3rc1"
 authors = [
     { name = "Benjamin Wiegand", email = "benjamin.wiegand@physik.hu-berlin.de" },
     { name = "Bastian Leykauf", email = "leykauf@physik.hu-berlin.de" },
     { name = "Robert Jördens", email = "rj@quartiq.de" },
     { name = "Christian Freier", email = "christian.freier@gmail.com" },
     { name = "Doron Behar", email = "doron.behar@gmail.com" },
 ]
```

