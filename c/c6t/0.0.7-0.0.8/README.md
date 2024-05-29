# Comparing `tmp/c6t-0.0.7.tar.gz` & `tmp/c6t-0.0.8.tar.gz`

## Comparing `c6t-0.0.7.tar` & `c6t-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 c6t-0.0.7/.python-version
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 c6t-0.0.7/requirements-dev.lock
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 c6t-0.0.7/requirements.lock
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 c6t-0.0.7/.github/dependabot.yml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 c6t-0.0.7/.github/workflows/dump-env.yml
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 c6t-0.0.7/src/c6t/__init__.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 c6t-0.0.7/src/c6t/__main__.py
--rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 c6t-0.0.7/src/c6t/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.7/src/c6t/api/__init__.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 c6t-0.0.7/src/c6t/api/agent_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.7/src/c6t/configure/__init__.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 c6t-0.0.7/src/c6t/configure/credentials.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.7/src/c6t/external/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.7/src/c6t/external/integrations/scw/__init__.py
--rw-r--r--   0        0        0     5991 2020-02-02 00:00:00.000000 c6t-0.0.7/src/c6t/external/integrations/scw/contrast_api.py
--rw-r--r--   0        0        0     8891 2020-02-02 00:00:00.000000 c6t-0.0.7/src/c6t/external/integrations/scw/contrast_scw.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 c6t-0.0.7/src/c6t/templates/contrast_security.yaml.j2
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 c6t-0.0.7/src/c6t/templates/contrast_security_env.yaml.j2
--rw-r--r--   0        0        0    14560 2020-02-02 00:00:00.000000 c6t-0.0.7/src/c6t/ui/auth.py
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 c6t-0.0.7/.gitignore
--rw-r--r--   0        0        0    11353 2020-02-02 00:00:00.000000 c6t-0.0.7/LICENSE
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 c6t-0.0.7/README.md
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 c6t-0.0.7/pyproject.toml
--rw-r--r--   0        0        0    14734 2020-02-02 00:00:00.000000 c6t-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 c6t-0.0.8/.python-version
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 c6t-0.0.8/requirements-dev.lock
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 c6t-0.0.8/requirements.lock
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 c6t-0.0.8/.github/dependabot.yml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 c6t-0.0.8/.github/workflows/dump-env.yml
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 c6t-0.0.8/src/c6t/__init__.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 c6t-0.0.8/src/c6t/__main__.py
+-rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 c6t-0.0.8/src/c6t/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.8/src/c6t/api/__init__.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 c6t-0.0.8/src/c6t/api/agent_config.py
+-rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 c6t-0.0.8/src/c6t/api/maven_repo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.8/src/c6t/configure/__init__.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 c6t-0.0.8/src/c6t/configure/credentials.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.8/src/c6t/external/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.8/src/c6t/external/integrations/scw/__init__.py
+-rw-r--r--   0        0        0     5991 2020-02-02 00:00:00.000000 c6t-0.0.8/src/c6t/external/integrations/scw/contrast_api.py
+-rw-r--r--   0        0        0     8891 2020-02-02 00:00:00.000000 c6t-0.0.8/src/c6t/external/integrations/scw/contrast_scw.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 c6t-0.0.8/src/c6t/templates/contrast_security.yaml.j2
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 c6t-0.0.8/src/c6t/templates/contrast_security_env.yaml.j2
+-rw-r--r--   0        0        0    14560 2020-02-02 00:00:00.000000 c6t-0.0.8/src/c6t/ui/auth.py
+-rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 c6t-0.0.8/.gitignore
+-rw-r--r--   0        0        0    11353 2020-02-02 00:00:00.000000 c6t-0.0.8/LICENSE
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 c6t-0.0.8/README.md
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 c6t-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0    14793 2020-02-02 00:00:00.000000 c6t-0.0.8/PKG-INFO
```

### Comparing `c6t-0.0.7/requirements-dev.lock` & `c6t-0.0.8/requirements-dev.lock`

 * *Files 18% similar despite different names*

```diff
@@ -14,26 +14,30 @@
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via black
     # via typer
+cssselect==1.2.0
+    # via types-lxml
 exceptiongroup==1.2.1
     # via pytest
 gitdb==4.0.11
     # via gitpython
 gitpython==3.1.43
     # via c6t
 idna==3.7
     # via requests
 iniconfig==2.0.0
     # via pytest
 jinja2==3.1.4
     # via c6t
+lxml==5.2.2
+    # via c6t
 markdown-it-py==3.0.0
     # via rich
 markupsafe==2.1.5
     # via jinja2
 mdurl==0.1.2
     # via markdown-it-py
 mypy==1.10.0
@@ -71,20 +75,27 @@
     # via gitdb
 tomli==2.0.1
     # via black
     # via mypy
     # via pytest
 typer==0.12.3
     # via c6t
+types-beautifulsoup4==4.12.0.20240511
+    # via types-lxml
+types-html5lib==1.1.11.20240228
+    # via types-beautifulsoup4
+types-lxml==2024.4.14
+    # via c6t
 types-requests==2.31.0.20240406
     # via c6t
 typing-extensions==4.11.0
     # via annotated-types
     # via black
     # via mypy
     # via rich
     # via typer
+    # via types-lxml
 urllib3==2.2.1
     # via requests
     # via types-requests
 wcwidth==0.2.13
     # via prompt-toolkit
```

### Comparing `c6t-0.0.7/requirements.lock` & `c6t-0.0.8/requirements.lock`

 * *Files 10% similar despite different names*

```diff
@@ -12,22 +12,26 @@
     # via c6t
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via typer
+cssselect==1.2.0
+    # via types-lxml
 gitdb==4.0.11
     # via gitpython
 gitpython==3.1.43
     # via c6t
 idna==3.7
     # via requests
 jinja2==3.1.4
     # via c6t
+lxml==5.2.2
+    # via c6t
 markdown-it-py==3.0.0
     # via rich
 markupsafe==2.1.5
     # via jinja2
 mdurl==0.1.2
     # via markdown-it-py
 prompt-toolkit==3.0.36
@@ -46,18 +50,25 @@
 shellingham==1.5.4
     # via c6t
     # via typer
 smmap==5.0.1
     # via gitdb
 typer==0.12.3
     # via c6t
+types-beautifulsoup4==4.12.0.20240511
+    # via types-lxml
+types-html5lib==1.1.11.20240228
+    # via types-beautifulsoup4
+types-lxml==2024.4.14
+    # via c6t
 types-requests==2.31.0.20240406
     # via c6t
 typing-extensions==4.11.0
     # via annotated-types
     # via rich
     # via typer
+    # via types-lxml
 urllib3==2.2.1
     # via requests
     # via types-requests
 wcwidth==0.2.13
     # via prompt-toolkit
```

### Comparing `c6t-0.0.7/.github/dependabot.yml` & `c6t-0.0.8/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `c6t-0.0.7/src/c6t/cli.py` & `c6t-0.0.8/src/c6t/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from typing import Optional
+from pathlib import Path
 
 import typer
 import yaml
 from git.repo import Repo
 from git.exc import InvalidGitRepositoryError
 from jinja2 import Environment, PackageLoader
 
 from rich import print as rprint
 
 import questionary
 
 from c6t.configure.credentials import ContrastAPICredentials
 from c6t.ui.auth import ContrastUIAuthManager
 from c6t.api.agent_config import AgentConfig
-
+from c6t.api.maven_repo import download_java_agent_from_repo
 from c6t.external.integrations.scw.contrast_scw import scw_create, scw_delete
 
 app = typer.Typer()
 integrations_app = typer.Typer()
 scw_integration_app = typer.Typer()
 app.add_typer(
     integrations_app, name="integrations", help="Integrations with other tools"
@@ -159,14 +160,33 @@
         agent_config.write_agent_config_to_file(path=path, text=rendered_yaml_text)
     elif type == "env":
         if path is None:
             path = "contrast.env"
         agent_config.write_agent_config_to_file(path=path, text=rendered_env_text)
 
 
+@app.command("download-agent")
+def download_agent(
+    language: str = "JAVA",
+    repository_url: str = "https://repo1.maven.org/maven2",
+    version: str = "latest",
+    target_dir: Path = Path("."),
+) -> None:
+    """
+    Download the Contrast agent for the specified language.
+    """
+    if language == "JAVA":
+        rprint(f"Downloading Contrast agent ({version})...")
+        download_java_agent_from_repo(
+            repository_url=repository_url, version=version, target_dir=target_dir
+        )
+    else:
+        rprint("Unsupported language")
+
+
 @scw_integration_app.command("create")
 def scw(profile: str = "default") -> None:
     """
     Populate vulnerability references with Secure Code Warrior links.
     """
     rprint("Creating SCW links...")
     scw_create(profile=profile)
```

### Comparing `c6t-0.0.7/src/c6t/api/agent_config.py` & `c6t-0.0.8/src/c6t/api/agent_config.py`

 * *Files identical despite different names*

### Comparing `c6t-0.0.7/src/c6t/configure/credentials.py` & `c6t-0.0.8/src/c6t/configure/credentials.py`

 * *Files identical despite different names*

### Comparing `c6t-0.0.7/src/c6t/external/integrations/scw/contrast_api.py` & `c6t-0.0.8/src/c6t/external/integrations/scw/contrast_api.py`

 * *Files identical despite different names*

### Comparing `c6t-0.0.7/src/c6t/external/integrations/scw/contrast_scw.py` & `c6t-0.0.8/src/c6t/external/integrations/scw/contrast_scw.py`

 * *Files identical despite different names*

### Comparing `c6t-0.0.7/src/c6t/templates/contrast_security.yaml.j2` & `c6t-0.0.8/src/c6t/templates/contrast_security.yaml.j2`

 * *Files identical despite different names*

### Comparing `c6t-0.0.7/src/c6t/templates/contrast_security_env.yaml.j2` & `c6t-0.0.8/src/c6t/templates/contrast_security_env.yaml.j2`

 * *Files identical despite different names*

### Comparing `c6t-0.0.7/src/c6t/ui/auth.py` & `c6t-0.0.8/src/c6t/ui/auth.py`

 * *Files identical despite different names*

### Comparing `c6t-0.0.7/.gitignore` & `c6t-0.0.8/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -165,9 +165,12 @@
 # Mac
 .DS_Store
 
 # Logs
 logs
 
 # Contrast Security
-contrast_security.yaml
+*.jar
 *.env
+*.sha1
+contrast_security.yaml
+maven-metadata.xml
```

### Comparing `c6t-0.0.7/LICENSE` & `c6t-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `c6t-0.0.7/README.md` & `c6t-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `c6t-0.0.7/pyproject.toml` & `c6t-0.0.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [project]
 name = "c6t"
-version = "0.0.7"
+version = "0.0.8"
 description = "Unofficial Administrative Command Line Interface for Contrast Security"
 authors = [
     { name = "Jonathan Harper", email = "39912347+jharper-sec@users.noreply.github.com" },
 ]
 dependencies = [
     "requests>=2.32.0",
     "shellingham>=1.5.4",
     "rich>=13.7.1",
-    "typer[all]>=0.12.3",
+    "typer>=0.12.3",
     "annotated-types>=0.6.0",
     "types-requests>=2.31.0.20240406",
     "jinja2>=3.1.4",
     "pyyaml>=6.0.1",
     "gitpython>=3.1.43",
     "questionary>=2.0.1",
+    "lxml>=5.2.2",
+    "types-lxml>=2024.4.14",
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = ">= 3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `c6t-0.0.7/PKG-INFO` & `c6t-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: c6t
-Version: 0.0.7
+Version: 0.0.8
 Summary: Unofficial Administrative Command Line Interface for Contrast Security
 Project-URL: Homepage, https://github.com/jharper-sec/c6t
 Project-URL: Issues, https://github.com/jharper-sec/c6t/issues
 Project-URL: Documentation, https://github.com/jharper-sec/c6t/blob/main/README.md
 Author-email: Jonathan Harper <39912347+jharper-sec@users.noreply.github.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
@@ -211,20 +211,22 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: annotated-types>=0.6.0
 Requires-Dist: gitpython>=3.1.43
 Requires-Dist: jinja2>=3.1.4
+Requires-Dist: lxml>=5.2.2
 Requires-Dist: pyyaml>=6.0.1
 Requires-Dist: questionary>=2.0.1
 Requires-Dist: requests>=2.32.0
 Requires-Dist: rich>=13.7.1
 Requires-Dist: shellingham>=1.5.4
-Requires-Dist: typer[all]>=0.12.3
+Requires-Dist: typer>=0.12.3
+Requires-Dist: types-lxml>=2024.4.14
 Requires-Dist: types-requests>=2.31.0.20240406
 Description-Content-Type: text/markdown
 
 ## c6t
 An unofficial Administrative Command Line Interface for Contrast Security
 
 ### Features
```

