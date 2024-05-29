# Comparing `tmp/my_moodle-0.4.5.tar.gz` & `tmp/my_moodle-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_moodle-0.4.5.tar", last modified: Fri Apr 19 07:05:44 2024, max compression
+gzip compressed data, was "my_moodle-0.4.6.tar", last modified: Wed May 29 13:56:56 2024, max compression
```

## Comparing `my_moodle-0.4.5.tar` & `my_moodle-0.4.6.tar`

### file list

```diff
@@ -1,50 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 07:05:44.988799 my_moodle-0.4.5/
--rw-rw-rw-   0        0        0       36 2024-03-01 17:54:38.000000 my_moodle-0.4.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1842 2024-04-19 07:05:44.987793 my_moodle-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0       88 2024-03-01 02:03:47.000000 my_moodle-0.4.5/license
-drwxrwxrwx   0        0        0        0 2024-04-19 07:05:44.966308 my_moodle-0.4.5/my_moodle/
--rw-rw-rw-   0        0        0     1470 2024-04-19 06:58:15.000000 my_moodle-0.4.5/my_moodle/__init__.py
--rw-rw-rw-   0        0        0      322 2024-03-01 22:18:35.000000 my_moodle-0.4.5/my_moodle/__main__.py
--rw-rw-rw-   0        0        0     5053 2024-04-09 00:23:45.000000 my_moodle-0.4.5/my_moodle/api.py
--rw-rw-rw-   0        0        0      555 2024-04-01 03:19:50.000000 my_moodle-0.4.5/my_moodle/api_functions.py
--rw-rw-rw-   0        0        0     2825 2024-03-31 01:09:50.000000 my_moodle-0.4.5/my_moodle/config_utility.py
--rw-rw-rw-   0        0        0    12286 2024-04-03 02:33:59.000000 my_moodle-0.4.5/my_moodle/course_markdown_builder.py
--rw-rw-rw-   0        0        0      340 2024-03-31 18:28:26.000000 my_moodle-0.4.5/my_moodle/course_status.py
--rw-rw-rw-   0        0        0     1629 2024-04-19 00:15:14.000000 my_moodle-0.4.5/my_moodle/csv_utility.py
--rw-rw-rw-   0        0        0    10814 2024-04-08 19:04:03.000000 my_moodle-0.4.5/my_moodle/data_utility.py
--rw-rw-rw-   0        0        0     1393 2024-03-31 10:33:22.000000 my_moodle-0.4.5/my_moodle/enrolled_users_fields.py
--rw-rw-rw-   0        0        0     1254 2024-03-31 21:14:09.000000 my_moodle-0.4.5/my_moodle/json_utility.py
--rw-rw-rw-   0        0        0     6848 2024-03-31 11:21:10.000000 my_moodle-0.4.5/my_moodle/markdown_document.py
--rw-rw-rw-   0        0        0     3596 2024-03-31 17:05:15.000000 my_moodle-0.4.5/my_moodle/markdown_methods.py
--rw-rw-rw-   0        0        0     8694 2024-04-19 01:10:59.000000 my_moodle-0.4.5/my_moodle/moodle_data_downloader.py
--rw-rw-rw-   0        0        0     6500 2024-04-19 00:36:16.000000 my_moodle-0.4.5/my_moodle/moodle_json_downloader.py
--rw-rw-rw-   0        0        0     2552 2024-04-19 02:49:07.000000 my_moodle-0.4.5/my_moodle/notebook_utility.py
--rw-rw-rw-   0        0        0     4469 2024-04-19 01:34:39.000000 my_moodle-0.4.5/my_moodle/program_markdown_builder.py
--rw-rw-rw-   0        0        0     4470 2024-04-09 01:00:41.000000 my_moodle-0.4.5/my_moodle/project_structure.py
--rw-rw-rw-   0        0        0     1169 2024-04-19 01:43:28.000000 my_moodle-0.4.5/my_moodle/resource.json
--rw-rw-rw-   0        0        0     2221 2024-04-19 02:49:40.000000 my_moodle-0.4.5/my_moodle/resource_utility.py
--rw-rw-rw-   0        0        0     5517 2024-04-19 06:59:54.000000 my_moodle-0.4.5/my_moodle/update_utility.py
--rw-rw-rw-   0        0        0      157 2024-04-19 00:13:16.000000 my_moodle-0.4.5/my_moodle/version.py
--rw-rw-rw-   0        0        0     8987 2024-03-31 20:15:05.000000 my_moodle-0.4.5/my_moodle/wrapper.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:05:44.986550 my_moodle-0.4.5/my_moodle.egg-info/
--rw-rw-rw-   0        0        0     1842 2024-04-19 07:05:44.000000 my_moodle-0.4.5/my_moodle.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1185 2024-04-19 07:05:44.000000 my_moodle-0.4.5/my_moodle.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 07:05:44.000000 my_moodle-0.4.5/my_moodle.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-04-19 07:05:44.000000 my_moodle-0.4.5/my_moodle.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-19 07:05:44.000000 my_moodle-0.4.5/my_moodle.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1243 2024-03-31 22:19:42.000000 my_moodle-0.4.5/readme.md
--rw-rw-rw-   0        0        0       42 2024-04-19 07:05:44.988799 my_moodle-0.4.5/setup.cfg
--rw-rw-rw-   0        0        0      996 2024-04-19 00:13:16.000000 my_moodle-0.4.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:05:44.985773 my_moodle-0.4.5/tests/
--rw-rw-rw-   0        0        0     1531 2024-04-12 12:51:27.000000 my_moodle-0.4.5/tests/_.py
--rw-rw-rw-   0        0        0        0 2024-03-01 02:03:47.000000 my_moodle-0.4.5/tests/__init__.py
--rw-rw-rw-   0        0        0     2876 2024-04-12 12:51:34.000000 my_moodle-0.4.5/tests/api_test.py
--rw-rw-rw-   0        0        0     1015 2024-03-28 07:15:10.000000 my_moodle-0.4.5/tests/config_parser_test.py
--rw-rw-rw-   0        0        0     2104 2024-04-04 16:34:12.000000 my_moodle-0.4.5/tests/course_markdown_builder_test.py
--rw-rw-rw-   0        0        0     1636 2024-04-19 00:39:24.000000 my_moodle-0.4.5/tests/moodle_data_downloader_test.py
--rw-rw-rw-   0        0        0     1243 2024-03-31 20:27:00.000000 my_moodle-0.4.5/tests/moodle_data_utility_test.py
--rw-rw-rw-   0        0        0     1414 2024-04-19 00:35:51.000000 my_moodle-0.4.5/tests/moodle_json_downloader_test.py
--rw-rw-rw-   0        0        0     1768 2024-04-19 01:52:39.000000 my_moodle-0.4.5/tests/notebook_utility_test.py
--rw-rw-rw-   0        0        0     1476 2024-03-31 15:44:24.000000 my_moodle-0.4.5/tests/package_test.py
--rw-rw-rw-   0        0        0     1013 2024-03-30 20:11:27.000000 my_moodle-0.4.5/tests/program_markdown_builder_test.py
--rw-rw-rw-   0        0        0      659 2024-04-19 00:13:16.000000 my_moodle-0.4.5/tests/version_test.py
+drwxrwxrwx   0        0        0        0 2024-05-29 13:56:56.639650 my_moodle-0.4.6/
+-rw-rw-rw-   0        0        0       36 2024-03-01 17:54:38.000000 my_moodle-0.4.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1780 2024-05-29 13:56:56.638652 my_moodle-0.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0       88 2024-03-01 02:03:47.000000 my_moodle-0.4.6/license
+drwxrwxrwx   0        0        0        0 2024-05-29 13:56:56.612299 my_moodle-0.4.6/my_moodle/
+-rw-rw-rw-   0        0        0     1107 2024-05-29 10:38:36.000000 my_moodle-0.4.6/my_moodle/__init__.py
+-rw-rw-rw-   0        0        0      324 2024-05-24 23:51:01.000000 my_moodle-0.4.6/my_moodle/__main__.py
+-rw-rw-rw-   0        0        0      184 2024-05-29 13:34:18.000000 my_moodle-0.4.6/my_moodle/api.py
+-rw-rw-rw-   0        0        0      193 2024-05-29 13:34:21.000000 my_moodle-0.4.6/my_moodle/api_functions.py
+-rw-rw-rw-   0        0        0      648 2024-05-29 10:07:10.000000 my_moodle-0.4.6/my_moodle/config_utility.py
+-rw-rw-rw-   0        0        0      198 2024-05-29 13:51:48.000000 my_moodle-0.4.6/my_moodle/course_markdown_builder.py
+-rw-rw-rw-   0        0        0      270 2024-05-29 10:26:25.000000 my_moodle-0.4.6/my_moodle/course_status.py
+-rw-rw-rw-   0        0        0      180 2024-05-29 13:51:45.000000 my_moodle-0.4.6/my_moodle/csv_utility.py
+-rw-rw-rw-   0        0        0     3306 2024-05-29 13:38:44.000000 my_moodle-0.4.6/my_moodle/data_utility.py
+-rw-rw-rw-   0        0        0      198 2024-05-29 13:34:48.000000 my_moodle-0.4.6/my_moodle/enrolled_users_fields.py
+-rw-rw-rw-   0        0        0      182 2024-05-29 13:34:08.000000 my_moodle-0.4.6/my_moodle/json_utility.py
+-rw-rw-rw-   0        0        0      192 2024-05-29 13:34:27.000000 my_moodle-0.4.6/my_moodle/markdown_document.py
+-rw-rw-rw-   0        0        0      182 2024-05-29 13:34:45.000000 my_moodle-0.4.6/my_moodle/markdown_methods.py
+-rw-rw-rw-   0        0        0     1262 2024-05-29 13:40:27.000000 my_moodle-0.4.6/my_moodle/moodle_data_downloader.py
+-rw-rw-rw-   0        0        0      200 2024-05-29 13:34:40.000000 my_moodle-0.4.6/my_moodle/moodle_json_downloader.py
+-rw-rw-rw-   0        0        0     2411 2024-05-29 13:31:54.000000 my_moodle-0.4.6/my_moodle/notebook_utility.py
+-rw-rw-rw-   0        0        0      200 2024-05-29 13:34:33.000000 my_moodle-0.4.6/my_moodle/program_markdown_builder.py
+-rw-rw-rw-   0        0        0      230 2024-05-29 13:34:36.000000 my_moodle-0.4.6/my_moodle/project_structure.py
+-rw-rw-rw-   0        0        0     1169 2024-04-19 01:43:28.000000 my_moodle-0.4.6/my_moodle/resource.json
+-rw-rw-rw-   0        0        0     2562 2024-05-29 10:30:00.000000 my_moodle-0.4.6/my_moodle/resource_utility.py
+-rw-rw-rw-   0        0        0     5658 2024-05-25 00:03:24.000000 my_moodle-0.4.6/my_moodle/update_utility.py
+-rw-rw-rw-   0        0        0      157 2024-05-27 17:53:13.000000 my_moodle-0.4.6/my_moodle/version.py
+-rw-rw-rw-   0        0        0      200 2024-05-29 13:34:29.000000 my_moodle-0.4.6/my_moodle/wrapper.py
+drwxrwxrwx   0        0        0        0 2024-05-29 13:56:56.637654 my_moodle-0.4.6/my_moodle.egg-info/
+-rw-rw-rw-   0        0        0     1780 2024-05-29 13:56:56.000000 my_moodle-0.4.6/my_moodle.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      932 2024-05-29 13:56:56.000000 my_moodle-0.4.6/my_moodle.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 13:56:56.000000 my_moodle-0.4.6/my_moodle.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-29 13:56:56.000000 my_moodle-0.4.6/my_moodle.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-29 13:56:56.000000 my_moodle-0.4.6/my_moodle.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1243 2024-05-27 17:54:38.000000 my_moodle-0.4.6/readme.md
+-rw-rw-rw-   0        0        0       42 2024-05-29 13:56:56.639650 my_moodle-0.4.6/setup.cfg
+-rw-rw-rw-   0        0        0      960 2024-05-29 13:56:36.000000 my_moodle-0.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 13:56:56.635640 my_moodle-0.4.6/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-01 02:03:47.000000 my_moodle-0.4.6/tests/__init__.py
+-rw-rw-rw-   0        0        0     1247 2024-05-29 09:53:41.000000 my_moodle-0.4.6/tests/main_test.py
+-rw-rw-rw-   0        0        0     1433 2024-05-29 13:51:49.000000 my_moodle-0.4.6/tests/notebook_test.py
+-rw-rw-rw-   0        0        0      659 2024-05-27 17:53:13.000000 my_moodle-0.4.6/tests/version_test.py
```

### Comparing `my_moodle-0.4.5/PKG-INFO` & `my_moodle-0.4.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: my-moodle
-Version: 0.4.5
+Version: 0.4.6
 Summary: Download Moodle Course content.
 Home-page: https://github.com/marcocrowe/my-moodle-py-pi/
 Author: Mark Crowe
 Author-email: 66536097+marcocrowe@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/marcocrowe/my-moodle-py-pi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: license
-Requires-Dist: ipython==8.15.0
-Requires-Dist: pandas==2.0.3
-Requires-Dist: requests==2.31.0
+Requires-Dist: requests==2.32.2
 
 
 # [My Moodle](https://pypi.org/project/my-moodle/ "My Moodle")
 
 A Python package to download data from Moodle.
 
 ## Sample Usage
```

### Comparing `my_moodle-0.4.5/my_moodle/__init__.py` & `my_moodle-0.4.6/my_moodle/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,38 @@
 """
 Copyright © 2024 Mark Crowe <https://github.com/marcocrowe>. All rights reserved.
 Moodle data downloader package.
 """
 
+# noinspection PyPep8Naming
 from . import api_functions as ApiFunctions
+# noinspection PyPep8Naming
 from . import config_utility as ConfigUtility
+# noinspection PyPep8Naming
 from . import csv_utility as CsvUtility
+# noinspection PyPep8Naming
 from . import data_utility as DataUtility
+# noinspection PyPep8Naming
 from . import json_utility as JsonUtility
 from . import markdown_methods
+# noinspection PyPep8Naming
 from . import notebook_utility as NotebookUtility
-from .api import Api
-from .course_markdown_builder import CourseMarkdownBuilder
 from .course_status import CourseStatus
-from .enrolled_users_fields import EnrolledUsersFields
-from .markdown_document import MarkdownDocument
 from .moodle_data_downloader import MoodleDataDownloader
-from .moodle_json_downloader import MoodleJsonDownloader
-from .program_markdown_builder import ProgramMarkdownBuilder
 from .update_utility import update_my_moodle_template
 from .version import __version__
-from .wrapper import Course, MoodleFile
 from .__main__ import main
 
 __all__ = [
-    "Api",
     "ApiFunctions",
     "ConfigUtility",
-    "Course",
-    "CourseMarkdownBuilder",
     "CourseStatus",
     "CsvUtility",
     "DataUtility",
-    "EnrolledUsersFields",
     "JsonUtility",
     "main",
     "markdown_methods",
-    "MarkdownDocument",
     "MoodleDataDownloader",
-    "MoodleFile",
-    "MoodleJsonDownloader",
     "NotebookUtility",
-    "ProgramMarkdownBuilder",
     "update_my_moodle_template",
     "__version__",
 ]
```

### Comparing `my_moodle-0.4.5/my_moodle/notebook_utility.py` & `my_moodle-0.4.6/my_moodle/notebook_utility.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """
 Copyright © 2024 Mark Crowe <https://github.com/marcocrowe>. All rights reserved.
 Notebook utility
 """
 
 from os import linesep
-from IPython.display import display
-from IPython.core.display import HTML
 from .resource_utility import PackageResources
 
 
 def create_jupyter_notebook_header(
     github_username: str,
     repository: str,
     notebook_filepath: str,
@@ -60,23 +58,19 @@
 
 
 def display_jupyter_notebook_header(
     github_username: str,
     repository: str,
     notebook_filepath: str = "notebook-main.ipynb",
     branch: str = "master",
-) -> None:
+) -> str:
     """Display an edit online header for Jupyter Notebook.
 
     Args:
         github_username (str): The GitHub username
         repository (str): The repository name
         notebook_filepath (str): The notebook filepath relative to the repository root
         branch (str, optional): The branch name. Defaults to 'master'.
     """
-    display(
-        HTML(
-            create_jupyter_notebook_header(
-                github_username, repository, notebook_filepath, branch
-            )
-        )
+    return create_jupyter_notebook_header(
+        github_username, repository, notebook_filepath, branch
     )
```

### Comparing `my_moodle-0.4.5/my_moodle/resource.json` & `my_moodle-0.4.6/my_moodle/resource.json`

 * *Files identical despite different names*

### Comparing `my_moodle-0.4.5/my_moodle/update_utility.py` & `my_moodle-0.4.6/my_moodle/update_utility.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     downloaded_file_path: str, version: str, download_directory: str
 ) -> str:
     """Extract the downloaded zip file to the temporary directory.
 
     Args:
         downloaded_file_path (str): The path to the downloaded zip file
         version (str): The release version
+        download_directory (str): The directory to extract the zip file
 
     Returns:
         str: The path to the extracted directory
     """
     extract_dir = os.path.join(download_directory, f"my-moodle-{version}")
     shutil.unpack_archive(downloaded_file_path, extract_dir, "zip")
 
@@ -99,14 +100,15 @@
 
     Args:
         api_url (str): The GitHub API URL
         app_directory_path (str): The path to the application directory
         current_version (str): The current version of the application
         base_download_url (str): The base download URL
         backup_dir (str): The backup directory
+        download_directory (str): The temporary download directory
     """
     latest_version = fetch_latest_release(api_url)
 
     if not latest_version:
         print("Update failed: Unable to fetch latest release information.")
         return
```

### Comparing `my_moodle-0.4.5/my_moodle.egg-info/PKG-INFO` & `my_moodle-0.4.6/my_moodle.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: my-moodle
-Version: 0.4.5
+Version: 0.4.6
 Summary: Download Moodle Course content.
 Home-page: https://github.com/marcocrowe/my-moodle-py-pi/
 Author: Mark Crowe
 Author-email: 66536097+marcocrowe@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/marcocrowe/my-moodle-py-pi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: license
-Requires-Dist: ipython==8.15.0
-Requires-Dist: pandas==2.0.3
-Requires-Dist: requests==2.31.0
+Requires-Dist: requests==2.32.2
 
 
 # [My Moodle](https://pypi.org/project/my-moodle/ "My Moodle")
 
 A Python package to download data from Moodle.
 
 ## Sample Usage
```

### Comparing `my_moodle-0.4.5/my_moodle.egg-info/SOURCES.txt` & `my_moodle-0.4.6/my_moodle.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -26,19 +26,11 @@
 my_moodle/version.py
 my_moodle/wrapper.py
 my_moodle.egg-info/PKG-INFO
 my_moodle.egg-info/SOURCES.txt
 my_moodle.egg-info/dependency_links.txt
 my_moodle.egg-info/requires.txt
 my_moodle.egg-info/top_level.txt
-tests/_.py
 tests/__init__.py
-tests/api_test.py
-tests/config_parser_test.py
-tests/course_markdown_builder_test.py
-tests/moodle_data_downloader_test.py
-tests/moodle_data_utility_test.py
-tests/moodle_json_downloader_test.py
-tests/notebook_utility_test.py
-tests/package_test.py
-tests/program_markdown_builder_test.py
+tests/main_test.py
+tests/notebook_test.py
 tests/version_test.py
```

### Comparing `my_moodle-0.4.5/readme.md` & `my_moodle-0.4.6/readme.md`

 * *Files identical despite different names*

### Comparing `my_moodle-0.4.5/setup.py` & `my_moodle-0.4.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 Setuptools configuration for my-moodle package.
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name="my-moodle",
-    version="0.4.5",
+    version="0.4.6",
     author="Mark Crowe",
     author_email="66536097+marcocrowe@users.noreply.github.com",
     description="Download Moodle Course content.",
     long_description=open("readme.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/marcocrowe/my-moodle-py-pi/",
     project_urls={
         "Bug Tracker": "https://github.com/marcocrowe/my-moodle-py-pi/issues"
     },
     packages=find_packages(),
     package_data={'my_moodle': ['resource.json']},
-    install_requires=["ipython==8.15.0", "pandas==2.0.3", "requests==2.31.0"],
+    install_requires=["requests==2.32.2"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9",
 )
```

### Comparing `my_moodle-0.4.5/tests/version_test.py` & `my_moodle-0.4.6/tests/version_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 class TestVersion(unittest.TestCase):
     """Test case for version"""
 
     def test_version(self) -> None:
         """Test the version of the package"""
-        expected_version: str = "0.4.5"  # Update this value when the version changes
+        expected_version: str = "0.4.6"  # Update this value when the version changes
         self.assertEqual(
             __version__,
             expected_version,
             f"Expected version: {expected_version}, Actual version: {__version__}",
         )
```

