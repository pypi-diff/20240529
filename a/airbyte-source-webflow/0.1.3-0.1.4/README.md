# Comparing `tmp/airbyte-source-webflow-0.1.3.tar.gz` & `tmp/airbyte_source_webflow-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-webflow-0.1.3.tar", last modified: Thu Feb  1 09:50:53 2024, max compression
+gzip compressed data, was "airbyte_source_webflow-0.1.4.tar", max compression
```

## Comparing `airbyte-source-webflow-0.1.3.tar` & `airbyte_source_webflow-0.1.4.tar`

### file list

```diff
@@ -1,32 +1,9 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 09:50:53.254876 airbyte-source-webflow-0.1.3/
--rw-r--r--   0 root         (0) root         (0)     5664 2024-02-01 09:50:53.254876 airbyte-source-webflow-0.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5679 2024-02-01 09:38:30.000000 airbyte-source-webflow-0.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 09:50:53.254876 airbyte-source-webflow-0.1.3/airbyte_source_webflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5664 2024-02-01 09:50:53.000000 airbyte-source-webflow-0.1.3/airbyte_source_webflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      833 2024-02-01 09:50:53.000000 airbyte-source-webflow-0.1.3/airbyte_source_webflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-01 09:50:53.000000 airbyte-source-webflow-0.1.3/airbyte_source_webflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2024-02-01 09:50:53.000000 airbyte-source-webflow-0.1.3/airbyte_source_webflow.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-01 09:50:53.000000 airbyte-source-webflow-0.1.3/airbyte_source_webflow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       44 2024-02-01 09:50:53.000000 airbyte-source-webflow-0.1.3/airbyte_source_webflow.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 09:50:53.254876 airbyte-source-webflow-0.1.3/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-02-01 09:38:30.000000 airbyte-source-webflow-0.1.3/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)       77 2024-02-01 09:38:30.000000 airbyte-source-webflow-0.1.3/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      314 2024-02-01 09:38:30.000000 airbyte-source-webflow-0.1.3/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)        3 2024-02-01 09:38:30.000000 airbyte-source-webflow-0.1.3/integration_tests/catalog.json
--rw-r--r--   0 root         (0) root         (0)      242 2024-02-01 09:38:30.000000 airbyte-source-webflow-0.1.3/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)       57 2024-02-01 09:38:30.000000 airbyte-source-webflow-0.1.3/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)       75 2024-02-01 09:38:30.000000 airbyte-source-webflow-0.1.3/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)       63 2024-02-01 09:38:30.000000 airbyte-source-webflow-0.1.3/integration_tests/sample_state.json
--rw-r--r--   0 root         (0) root         (0)     5566 2024-02-01 09:50:53.258876 airbyte-source-webflow-0.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      919 2024-02-01 09:50:51.000000 airbyte-source-webflow-0.1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 09:50:53.254876 airbyte-source-webflow-0.1.3/source_webflow/
--rw-r--r--   0 root         (0) root         (0)      126 2024-02-01 09:38:30.000000 airbyte-source-webflow-0.1.3/source_webflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)      893 2024-02-01 09:38:30.000000 airbyte-source-webflow-0.1.3/source_webflow/auth.py
--rw-r--r--   0 root         (0) root         (0)      233 2024-02-01 09:38:30.000000 airbyte-source-webflow-0.1.3/source_webflow/run.py
--rw-r--r--   0 root         (0) root         (0)    14604 2024-02-01 09:38:30.000000 airbyte-source-webflow-0.1.3/source_webflow/source.py
--rw-r--r--   0 root         (0) root         (0)      988 2024-02-01 09:38:30.000000 airbyte-source-webflow-0.1.3/source_webflow/spec.yaml
--rw-r--r--   0 root         (0) root         (0)     1258 2024-02-01 09:38:30.000000 airbyte-source-webflow-0.1.3/source_webflow/webflow_to_airbyte_mapping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 09:50:53.254876 airbyte-source-webflow-0.1.3/unit_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-02-01 09:38:30.000000 airbyte-source-webflow-0.1.3/unit_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1124 2024-02-01 09:38:30.000000 airbyte-source-webflow-0.1.3/unit_tests/test_source.py
--rw-r--r--   0 root         (0) root         (0)     2716 2024-02-01 09:38:30.000000 airbyte-source-webflow-0.1.3/unit_tests/test_streams.py
+-rw-r--r--   0        0        0     4514 2024-05-29 11:25:07.447665 airbyte_source_webflow-0.1.4/README.md
+-rw-r--r--   0        0        0      749 2024-05-29 11:29:12.503809 airbyte_source_webflow-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      126 2024-05-29 11:25:07.447665 airbyte_source_webflow-0.1.4/source_webflow/__init__.py
+-rw-r--r--   0        0        0      893 2024-05-29 11:25:07.447665 airbyte_source_webflow-0.1.4/source_webflow/auth.py
+-rw-r--r--   0        0        0      233 2024-05-29 11:25:07.447665 airbyte_source_webflow-0.1.4/source_webflow/run.py
+-rw-r--r--   0        0        0    14604 2024-05-29 11:25:07.447665 airbyte_source_webflow-0.1.4/source_webflow/source.py
+-rw-r--r--   0        0        0      988 2024-05-29 11:25:07.447665 airbyte_source_webflow-0.1.4/source_webflow/spec.yaml
+-rw-r--r--   0        0        0     1258 2024-05-29 11:25:07.447665 airbyte_source_webflow-0.1.4/source_webflow/webflow_to_airbyte_mapping.py
+-rw-r--r--   0        0        0     5221 1970-01-01 00:00:00.000000 airbyte_source_webflow-0.1.4/PKG-INFO
```

### Comparing `airbyte-source-webflow-0.1.3/PKG-INFO` & `airbyte_source_webflow-0.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,104 +1,110 @@
 Metadata-Version: 2.1
 Name: airbyte-source-webflow
-Version: 0.1.3
+Version: 0.1.4
 Summary: Source implementation for Webflow.
+Home-page: https://airbyte.com
+License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
+Requires-Python: >=3.9,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: airbyte-cdk (==0.80.0)
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/webflow
+Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.1; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
 
-# Webflow Source
-
-This is the repository for the Webflow source connector, written in Python.
-For information about how to use this connector within Airbyte, see [Webflow source documentation](https://docs.airbyte.io/integrations/sources/webflow).
+# Webflow source connector
 
 
-A detailed tutorial has been written about this implementation. See: [Build a connector to extract data from the Webflow API](https://airbyte.com/tutorials/extract-data-from-the-webflow-api)
+This is the repository for the Webflow source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/webflow).
 
+## Local development
 
-- Webflow v1 API Key
+### Prerequisites
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
 
-From this connector directory, create a virtual environment:
-```
-python -m venv .venv
-```
-
-This will generate a virtualenv for this module in `.venv/`. Make sure this venv is active in your
-development environment of choice. To activate it from the terminal, run:
-```
-source .venv/bin/activate
-pip install -r requirements.txt
-pip install '.[tests]'
+### Installing the connector
+From this connector directory, run:
+```bash
+poetry install --with dev
 ```
-If you are in an IDE, follow your IDE's instructions to activate the virtualenv.
 
-Note that while we are installing dependencies from `requirements.txt`, you should only edit `setup.py` for your dependencies. `requirements.txt` is
-used for editable installs (`pip install -e`) to pull in Python dependencies from the monorepo and will call `setup.py`.
-If this is mumbo jumbo to you, don't worry about it, just put your deps in `setup.py` but install using `pip install -r requirements.txt` and everything
-should work as you expect.
 
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/webflow)
+### Create credentials
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/webflow)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_webflow/spec.yaml` file.
-Note that any directory named `secrets` is git-ignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
-
-For more information about creating Webflow credentials, see [the documentation](https://docs.airbyte.io/integrations/sources/webflow).
+Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source webflow test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
 ```
-python main.py spec
-python main.py check --config secrets/config.json
-python main.py discover --config secrets/config.json
-python main.py read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+poetry run source-webflow spec
+poetry run source-webflow check --config secrets/config.json
+poetry run source-webflow discover --config secrets/config.json
+poetry run source-webflow read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
+### Running unit tests
+To run unit tests locally, from the connector directory run:
+```
+poetry run pytest unit_tests
+```
 
-
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+### Building the docker image
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-webflow build
 ```
 
-An image will be built with the tag `airbyte/source-webflow:dev`.
+An image will be available on your host with the tag `airbyte/source-webflow:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-webflow:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-webflow:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-webflow:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-webflow:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-webflow:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-webflow test
 ```
 
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+### Customizing acceptance Tests
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+### Dependency Management
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
+## Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-webflow test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/webflow.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/webflow.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-webflow-0.1.3/source_webflow/auth.py` & `airbyte_source_webflow-0.1.4/source_webflow/auth.py`

 * *Files identical despite different names*

### Comparing `airbyte-source-webflow-0.1.3/source_webflow/source.py` & `airbyte_source_webflow-0.1.4/source_webflow/source.py`

 * *Files identical despite different names*

### Comparing `airbyte-source-webflow-0.1.3/source_webflow/spec.yaml` & `airbyte_source_webflow-0.1.4/source_webflow/spec.yaml`

 * *Files identical despite different names*

### Comparing `airbyte-source-webflow-0.1.3/source_webflow/webflow_to_airbyte_mapping.py` & `airbyte_source_webflow-0.1.4/source_webflow/webflow_to_airbyte_mapping.py`

 * *Files identical despite different names*

