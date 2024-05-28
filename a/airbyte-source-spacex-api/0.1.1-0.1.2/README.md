# Comparing `tmp/airbyte-source-spacex-api-0.1.1.tar.gz` & `tmp/airbyte_source_spacex_api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-spacex-api-0.1.1.tar", last modified: Wed Jan 31 17:56:20 2024, max compression
+gzip compressed data, was "airbyte_source_spacex_api-0.1.2.tar", max compression
```

## Comparing `airbyte-source-spacex-api-0.1.1.tar` & `airbyte_source_spacex_api-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,8 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 17:56:20.504897 airbyte-source-spacex-api-0.1.1/
--rw-r--r--   0 root         (0) root         (0)     5189 2024-01-31 17:56:20.504897 airbyte-source-spacex-api-0.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5138 2024-01-31 17:51:56.000000 airbyte-source-spacex-api-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 17:56:20.504897 airbyte-source-spacex-api-0.1.1/airbyte_source_spacex_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5189 2024-01-31 17:56:20.000000 airbyte-source-spacex-api-0.1.1/airbyte_source_spacex_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      692 2024-01-31 17:56:20.000000 airbyte-source-spacex-api-0.1.1/airbyte_source_spacex_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-31 17:56:20.000000 airbyte-source-spacex-api-0.1.1/airbyte_source_spacex_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-01-31 17:56:20.000000 airbyte-source-spacex-api-0.1.1/airbyte_source_spacex_api.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       78 2024-01-31 17:56:20.000000 airbyte-source-spacex-api-0.1.1/airbyte_source_spacex_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       36 2024-01-31 17:56:20.000000 airbyte-source-spacex-api-0.1.1/airbyte_source_spacex_api.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 17:56:20.504897 airbyte-source-spacex-api-0.1.1/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-31 17:51:56.000000 airbyte-source-spacex-api-0.1.1/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)       49 2024-01-31 17:51:56.000000 airbyte-source-spacex-api-0.1.1/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-01-31 17:51:56.000000 airbyte-source-spacex-api-0.1.1/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)     2673 2024-01-31 17:51:56.000000 airbyte-source-spacex-api-0.1.1/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)       55 2024-01-31 17:51:56.000000 airbyte-source-spacex-api-0.1.1/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)       39 2024-01-31 17:51:56.000000 airbyte-source-spacex-api-0.1.1/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-31 17:51:56.000000 airbyte-source-spacex-api-0.1.1/integration_tests/sample_state.json
--rw-r--r--   0 root         (0) root         (0)     5070 2024-01-31 17:56:20.504897 airbyte-source-spacex-api-0.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      933 2024-01-31 17:56:18.000000 airbyte-source-spacex-api-0.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 17:56:20.504897 airbyte-source-spacex-api-0.1.1/source_spacex_api/
--rw-r--r--   0 root         (0) root         (0)      130 2024-01-31 17:51:56.000000 airbyte-source-spacex-api-0.1.1/source_spacex_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41239 2024-01-31 17:51:56.000000 airbyte-source-spacex-api-0.1.1/source_spacex_api/manifest.yaml
--rw-r--r--   0 root         (0) root         (0)      240 2024-01-31 17:51:56.000000 airbyte-source-spacex-api-0.1.1/source_spacex_api/run.py
--rw-r--r--   0 root         (0) root         (0)      478 2024-01-31 17:51:56.000000 airbyte-source-spacex-api-0.1.1/source_spacex_api/source.py
+-rw-r--r--   0        0        0     4582 2024-05-28 22:04:00.975483 airbyte_source_spacex_api-0.1.2/README.md
+-rw-r--r--   0        0        0      138 2024-05-28 22:04:00.975483 airbyte_source_spacex_api-0.1.2/main.py
+-rw-r--r--   0        0        0      779 2024-05-28 22:07:58.567688 airbyte_source_spacex_api-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      130 2024-05-28 22:04:00.975483 airbyte_source_spacex_api-0.1.2/source_spacex_api/__init__.py
+-rw-r--r--   0        0        0    35523 2024-05-28 22:04:00.975483 airbyte_source_spacex_api-0.1.2/source_spacex_api/manifest.yaml
+-rw-r--r--   0        0        0      231 2024-05-28 22:04:00.975483 airbyte_source_spacex_api-0.1.2/source_spacex_api/run.py
+-rw-r--r--   0        0        0      478 2024-05-28 22:04:00.975483 airbyte_source_spacex_api-0.1.2/source_spacex_api/source.py
+-rw-r--r--   0        0        0     5296 1970-01-01 00:00:00.000000 airbyte_source_spacex_api-0.1.2/PKG-INFO
```

### Comparing `airbyte-source-spacex-api-0.1.1/PKG-INFO` & `airbyte_source_spacex_api-0.1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,91 +1,122 @@
 Metadata-Version: 2.1
 Name: airbyte-source-spacex-api
-Version: 0.1.1
-Summary: Source implementation for Spacex Api.
+Version: 0.1.2
+Summary: Source implementation for spacex-api.
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
+Requires-Dist: airbyte-cdk (>=0,<1)
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/spacex-api
+Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk~=0.1
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.1; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
 
 # Spacex Api Source
 
 This is the repository for the Spacex Api configuration based source connector.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/spacex-api).
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/spacex-api).
 
+## Local development
 
-**To iterate on this connector, make sure to complete this prerequisites section.**
+### Prerequisites
 
+* Python (`^3.9`)
+* Poetry (`^1.7`) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
-From this connector directory, create a virtual environment:
-```
-python -m venv .venv
-```
 
-This will generate a virtualenv for this module in `.venv/`. Make sure this venv is active in your
-development environment of choice. To activate it from the terminal, run:
-```
-source .venv/bin/activate
-pip install -r requirements.txt
+
+### Installing the connector
+
+From this connector directory, run:
+```bash
+poetry install --with dev
 ```
-If you are in an IDE, follow your IDE's instructions to activate the virtualenv.
 
-Note that while we are installing dependencies from `requirements.txt`, you should only edit `setup.py` for your dependencies. `requirements.txt` is
-used for editable installs (`pip install -e`) to pull in Python dependencies from the monorepo and will call `setup.py`.
-If this is mumbo jumbo to you, don't worry about it, just put your deps in `setup.py` but install using `pip install -r requirements.txt` and everything
-should work as you expect.
 
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/spacex-api)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_spacex_api/spec.yaml` file.
+### Create credentials
+
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/spacex-api)
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `spec` inside `source_spacex_api/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `integration_tests/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source spacex-api test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
 
+```
+poetry run source-spacex-api spec
+poetry run source-spacex-api check --config secrets/config.json
+poetry run source-spacex-api discover --config secrets/config.json
+poetry run source-spacex-api read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+```
+
+### Running tests
+
+To run tests locally, from the connector directory run:
 
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
-```bash
-airbyte-ci connectors --name=source-spacex-api build
+```
+poetry run pytest tests
 ```
 
-An image will be built with the tag `airbyte/source-spacex-api:dev`.
+### Building the docker image
 
-**Via `docker build`:**
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
-docker build -t airbyte/source-spacex-api:dev .
+airbyte-ci connectors --name=source-spacex-api build
 ```
 
+An image will be available on your host with the tag `airbyte/source-spacex-api:dev`.
+
+
+### Running as a docker container
+
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-spacex-api:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-spacex-api:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-spacex-api:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-spacex-api:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-spacex-api test
 ```
 
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+### Customizing acceptance Tests
+
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+### Dependency Management
+
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
+
+## Publishing a new version of the connector
 
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-spacex-api test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/spacex-api.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/spacex-api.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-spacex-api-0.1.1/README.md` & `airbyte_source_spacex_api-0.1.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,91 +1,103 @@
 # Spacex Api Source
 
 This is the repository for the Spacex Api configuration based source connector.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/spacex-api).
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/spacex-api).
 
 ## Local development
 
 ### Prerequisites
-**To iterate on this connector, make sure to complete this prerequisites section.**
 
-#### Minimum Python version required `= 3.9.0`
+* Python (`^3.9`)
+* Poetry (`^1.7`) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
-#### Build & Activate Virtual Environment and install dependencies
-From this connector directory, create a virtual environment:
-```
-python -m venv .venv
-```
 
-This will generate a virtualenv for this module in `.venv/`. Make sure this venv is active in your
-development environment of choice. To activate it from the terminal, run:
-```
-source .venv/bin/activate
-pip install -r requirements.txt
+
+### Installing the connector
+
+From this connector directory, run:
+```bash
+poetry install --with dev
 ```
-If you are in an IDE, follow your IDE's instructions to activate the virtualenv.
 
-Note that while we are installing dependencies from `requirements.txt`, you should only edit `setup.py` for your dependencies. `requirements.txt` is
-used for editable installs (`pip install -e`) to pull in Python dependencies from the monorepo and will call `setup.py`.
-If this is mumbo jumbo to you, don't worry about it, just put your deps in `setup.py` but install using `pip install -r requirements.txt` and everything
-should work as you expect.
 
-#### Create credentials
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/spacex-api)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_spacex_api/spec.yaml` file.
+### Create credentials
+
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/spacex-api)
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `spec` inside `source_spacex_api/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `integration_tests/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source spacex-api test creds`
-and place them into `secrets/config.json`.
 
-### Locally running the connector docker image
+### Locally running the connector
 
+```
+poetry run source-spacex-api spec
+poetry run source-spacex-api check --config secrets/config.json
+poetry run source-spacex-api discover --config secrets/config.json
+poetry run source-spacex-api read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+```
+
+### Running tests
+
+To run tests locally, from the connector directory run:
 
-#### Build
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
-```bash
-airbyte-ci connectors --name=source-spacex-api build
+```
+poetry run pytest tests
 ```
 
-An image will be built with the tag `airbyte/source-spacex-api:dev`.
+### Building the docker image
 
-**Via `docker build`:**
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
-docker build -t airbyte/source-spacex-api:dev .
+airbyte-ci connectors --name=source-spacex-api build
 ```
 
-#### Run
+An image will be available on your host with the tag `airbyte/source-spacex-api:dev`.
+
+
+### Running as a docker container
+
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-spacex-api:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-spacex-api:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-spacex-api:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-spacex-api:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
-## Testing
+### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-spacex-api test
 ```
 
 ### Customizing acceptance Tests
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-## Dependency Management
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+### Dependency Management
+
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
+
+## Publishing a new version of the connector
 
-### Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-spacex-api test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/spacex-api.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/spacex-api.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-spacex-api-0.1.1/source_spacex_api/manifest.yaml` & `airbyte_source_spacex_api-0.1.2/source_spacex_api/manifest.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-version: 0.51.41
+version: 0.79.1
+
 type: DeclarativeSource
+
 check:
   type: CheckStream
   stream_names:
     - launches
     - capsules
     - company
     - crew
@@ -12,1704 +14,1676 @@
     - landpads
     - payloads
     - history
     - rockets
     - roadster
     - ships
     - starlink
+
+definitions:
+  streams:
+    launches:
+      type: DeclarativeStream
+      name: launches
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: /launches/{{config['options'] or config['id'] or 'latest'}}
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path: []
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/launches"
+    capsules:
+      type: DeclarativeStream
+      name: capsules
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: /capsules
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path: []
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/capsules"
+    company:
+      type: DeclarativeStream
+      name: company
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: /company
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path: []
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/company"
+    crew:
+      type: DeclarativeStream
+      name: crew
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: /crew
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path: []
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/crew"
+    cores:
+      type: DeclarativeStream
+      name: cores
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: /cores
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path: []
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/cores"
+    dragons:
+      type: DeclarativeStream
+      name: dragons
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: /dragons
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path: []
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/dragons"
+    landpads:
+      type: DeclarativeStream
+      name: landpads
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: /landpads
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path: []
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/landpads"
+    payloads:
+      type: DeclarativeStream
+      name: payloads
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: /payloads
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path: []
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/payloads"
+    history:
+      type: DeclarativeStream
+      name: history
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: /history
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path: []
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/history"
+    rockets:
+      type: DeclarativeStream
+      name: rockets
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: /rockets
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path: []
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/rockets"
+    roadster:
+      type: DeclarativeStream
+      name: roadster
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: /roadster
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path: []
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/roadster"
+    ships:
+      type: DeclarativeStream
+      name: ships
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: /ships
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path: []
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/ships"
+    starlink:
+      type: DeclarativeStream
+      name: starlink
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: /starlink
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path: []
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/starlink"
+  base_requester:
+    type: HttpRequester
+    url_base: https://api.spacexdata.com/v4/
+
 streams:
-  - type: DeclarativeStream
-    name: launches
-    primary_key:
-      - id
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/schema#
-        properties:
-          auto_update:
-            type: boolean
-          capsules:
-            items:
+  - $ref: "#/definitions/streams/launches"
+  - $ref: "#/definitions/streams/capsules"
+  - $ref: "#/definitions/streams/company"
+  - $ref: "#/definitions/streams/crew"
+  - $ref: "#/definitions/streams/cores"
+  - $ref: "#/definitions/streams/dragons"
+  - $ref: "#/definitions/streams/landpads"
+  - $ref: "#/definitions/streams/payloads"
+  - $ref: "#/definitions/streams/history"
+  - $ref: "#/definitions/streams/rockets"
+  - $ref: "#/definitions/streams/roadster"
+  - $ref: "#/definitions/streams/ships"
+  - $ref: "#/definitions/streams/starlink"
+
+spec:
+  type: Spec
+  connection_specification:
+    type: object
+    $schema: http://json-schema.org/draft-07/schema#
+    required: []
+    properties:
+      id:
+        type: string
+        title: Unique ID for specific source target
+        desciption: Optional, For a specific ID
+        order: 0
+      options:
+        type: string
+        title: Configuration options for endpoints
+        desciption: >-
+          Optional, Possible values for an endpoint. Example values for
+          launches-latest, upcoming, past
+        order: 1
+    additionalProperties: true
+
+metadata:
+  autoImportSchema:
+    launches: false
+    capsules: false
+    company: false
+    crew: false
+    cores: false
+    dragons: false
+    landpads: false
+    payloads: false
+    history: false
+    rockets: false
+    roadster: false
+    ships: false
+    starlink: false
+
+schemas:
+  launches:
+    type: object
+    $schema: http://json-schema.org/schema#
+    properties:
+      auto_update:
+        type: boolean
+      capsules:
+        type: array
+        items:
+          type:
+            - "null"
+            - string
+      cores:
+        type: array
+        items:
+          type: object
+          properties:
+            core:
               type:
                 - "null"
                 - string
+            flight:
+              type: number
+            gridfins:
+              type: boolean
+            landing_attempt:
+              type: boolean
+            landing_success:
+              type: boolean
+            landing_type:
+              type:
+                - "null"
+                - string
+            landpad:
+              type:
+                - "null"
+                - string
+            legs:
+              type: boolean
+            reused:
+              type: boolean
+      crew:
+        type: array
+        items:
+          type:
+            - "null"
+            - string
+      date_local:
+        type:
+          - "null"
+          - string
+      date_precision:
+        type:
+          - "null"
+          - string
+      date_unix:
+        type: number
+      date_utc:
+        type:
+          - "null"
+          - string
+      details:
+        type: string
+      failures:
+        type: array
+      fairings:
+        type: object
+        properties:
+          recovered:
+            type: boolean
+          recovery_attempt:
+            type: boolean
+          reused:
+            type: boolean
+          ships:
             type: array
-          cores:
-            items:
-              properties:
-                core:
-                  type:
-                    - "null"
-                    - string
-                flight:
-                  type: number
-                gridfins:
-                  type: boolean
-                landing_attempt:
-                  type: boolean
-                landing_success:
-                  type: boolean
-                landing_type:
-                  type:
-                    - "null"
-                    - string
-                landpad:
-                  type:
-                    - "null"
-                    - string
-                legs:
-                  type: boolean
-                reused:
-                  type: boolean
-              type: object
-            type: array
-          crew:
             items:
               type:
                 - "null"
                 - string
-            type: array
-          date_local:
-            type:
-              - "null"
-              - string
-          date_precision:
-            type:
-              - "null"
-              - string
-          date_unix:
-            type: number
-          date_utc:
-            type:
-              - "null"
-              - string
-          static_fire_date_unix:
-            type:
-              - "null"
-              - number
-          static_fire_date_utc:
+      flight_number:
+        type: number
+      id:
+        type:
+          - "null"
+          - string
+      launch_library_id:
+        type:
+          - "null"
+          - string
+      launchpad:
+        type:
+          - "null"
+          - string
+      links:
+        type: object
+        properties:
+          article:
             type:
               - "null"
               - string
-          window:
-            type:
-              - "null"
-              - number
-          details:
-            type: string
-          fairings:
+          flickr:
+            type: object
             properties:
-              recovered:
-                type: boolean
-              recovery_attempt:
-                type: boolean
-              reused:
-                type: boolean
-              ships:
+              original:
+                type: array
                 items:
                   type:
                     - "null"
                     - string
+              small:
                 type: array
+          patch:
             type: object
-          failures:
-            type: array
-          flight_number:
-            type: number
-          id:
-            type:
-              - "null"
-              - string
-          launch_library_id:
-            type:
-              - "null"
-              - string
-          launchpad:
-            type:
-              - "null"
-              - string
-          links:
             properties:
-              flickr:
-                properties:
-                  original:
-                    items:
-                      type:
-                        - "null"
-                        - string
-                    type: array
-                  small:
-                    type: array
-                type: object
-              patch:
-                properties:
-                  large:
-                    type:
-                      - "null"
-                      - string
-                  small:
-                    type:
-                      - "null"
-                      - string
-                type: object
-              reddit:
-                properties:
-                  launch:
-                    type:
-                      - "null"
-                      - string
-                type: object
-              article:
-                type:
-                  - "null"
-                  - string
-              webcast:
+              large:
                 type:
                   - "null"
                   - string
-              wikipedia:
+              small:
                 type:
                   - "null"
                   - string
-              youtube_id:
+          reddit:
+            type: object
+            properties:
+              launch:
                 type:
                   - "null"
                   - string
-            type: object
-          name:
-            type:
-              - "null"
-              - string
-          net:
-            type: boolean
-          payloads:
-            items:
-              type:
-                - "null"
-                - string
-            type: array
-          rocket:
-            type:
-              - "null"
-              - string
-          ships:
-            type: array
-          success:
-            type: boolean
-          tbd:
-            type: boolean
-          upcoming:
-            type: boolean
-        type: object
-    retriever:
-      type: SimpleRetriever
-      requester:
-        type: HttpRequester
-        url_base: https://api.spacexdata.com/v4/
-        path: /launches/{{config['options'] or config['id'] or 'latest'}}
-        http_method: GET
-        request_parameters: {}
-        request_headers: {}
-        authenticator:
-          type: NoAuth
-        request_body_json: {}
-      record_selector:
-        type: RecordSelector
-        extractor:
-          type: DpathExtractor
-          field_path: []
-      paginator:
-        type: NoPagination
-  - type: DeclarativeStream
-    name: capsules
-    primary_key:
-      - id
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/schema#
-        properties:
-          id:
+          webcast:
             type:
               - "null"
               - string
-          land_landings:
-            type: number
-          last_update:
-            type:
-              - "null"
-              - string
-          launches:
-            items:
-              type:
-                - "null"
-                - string
-            type: array
-          reuse_count:
-            type: number
-          serial:
+          wikipedia:
             type:
               - "null"
               - string
-          status:
+          youtube_id:
             type:
               - "null"
               - string
+      name:
+        type:
+          - "null"
+          - string
+      net:
+        type: boolean
+      payloads:
+        type: array
+        items:
           type:
-            type:
-              - "null"
-              - string
-          water_landings:
-            type: number
+            - "null"
+            - string
+      rocket:
+        type:
+          - "null"
+          - string
+      ships:
+        type: array
+      static_fire_date_unix:
+        type:
+          - "null"
+          - number
+      static_fire_date_utc:
+        type:
+          - "null"
+          - string
+      success:
+        type: boolean
+      tbd:
+        type: boolean
+      upcoming:
+        type: boolean
+      window:
+        type:
+          - "null"
+          - number
+    additionalProperties: true
+  capsules:
+    type: object
+    $schema: http://json-schema.org/schema#
+    properties:
+      type:
+        type:
+          - "null"
+          - string
+      id:
+        type:
+          - "null"
+          - string
+      land_landings:
+        type: number
+      last_update:
+        type:
+          - "null"
+          - string
+      launches:
+        type: array
+        items:
+          type:
+            - "null"
+            - string
+      reuse_count:
+        type: number
+      serial:
+        type:
+          - "null"
+          - string
+      status:
+        type:
+          - "null"
+          - string
+      water_landings:
+        type: number
+    additionalProperties: true
+  company:
+    type: object
+    $schema: http://json-schema.org/schema#
+    properties:
+      ceo:
+        type:
+          - "null"
+          - string
+      coo:
+        type:
+          - "null"
+          - string
+      cto:
+        type:
+          - "null"
+          - string
+      cto_propulsion:
+        type:
+          - "null"
+          - string
+      employees:
+        type: number
+      founded:
+        type: number
+      founder:
+        type:
+          - "null"
+          - string
+      headquarters:
         type: object
-    retriever:
-      type: SimpleRetriever
-      requester:
-        type: HttpRequester
-        url_base: https://api.spacexdata.com/v4/
-        path: /capsules
-        http_method: GET
-        request_parameters: {}
-        request_headers: {}
-        authenticator:
-          type: NoAuth
-        request_body_json: {}
-      record_selector:
-        type: RecordSelector
-        extractor:
-          type: DpathExtractor
-          field_path: []
-      paginator:
-        type: NoPagination
-  - type: DeclarativeStream
-    name: company
-    primary_key:
-      - id
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/schema#
         properties:
-          ceo:
+          address:
             type:
               - "null"
               - string
-          coo:
+          city:
             type:
               - "null"
               - string
-          cto:
+          state:
             type:
               - "null"
               - string
-          cto_propulsion:
-            type:
-              - "null"
-              - string
-          employees:
-            type: number
-          founded:
-            type: number
-          founder:
+      id:
+        type:
+          - "null"
+          - string
+      launch_sites:
+        type: number
+      links:
+        type: object
+        properties:
+          elon_twitter:
             type:
               - "null"
               - string
-          headquarters:
-            properties:
-              address:
-                type:
-                  - "null"
-                  - string
-              city:
-                type:
-                  - "null"
-                  - string
-              state:
-                type:
-                  - "null"
-                  - string
-            type: object
-          id:
+          flickr:
             type:
               - "null"
               - string
-          launch_sites:
-            type: number
-          links:
-            properties:
-              elon_twitter:
-                type:
-                  - "null"
-                  - string
-              flickr:
-                type:
-                  - "null"
-                  - string
-              twitter:
-                type:
-                  - "null"
-                  - string
-              website:
-                type:
-                  - "null"
-                  - string
-            type: object
-          name:
+          twitter:
             type:
               - "null"
               - string
-          summary:
+          website:
             type:
               - "null"
               - string
-          test_sites:
-            type: number
-          valuation:
+      name:
+        type:
+          - "null"
+          - string
+      summary:
+        type:
+          - "null"
+          - string
+      test_sites:
+        type: number
+      valuation:
+        type: number
+      vehicles:
+        type: number
+    additionalProperties: true
+  crew:
+    type: object
+    $schema: http://json-schema.org/schema#
+    properties:
+      agency:
+        type:
+          - "null"
+          - string
+      id:
+        type:
+          - "null"
+          - string
+      image:
+        type:
+          - "null"
+          - string
+      launches:
+        type: array
+        items:
+          type:
+            - "null"
+            - string
+      name:
+        type:
+          - "null"
+          - string
+      status:
+        type:
+          - "null"
+          - string
+      wikipedia:
+        type:
+          - "null"
+          - string
+    additionalProperties: true
+  cores:
+    type: object
+    $schema: http://json-schema.org/schema#
+    properties:
+      asds_attempts:
+        type: number
+      asds_landings:
+        type: number
+      block:
+        type:
+          - "null"
+          - number
+      id:
+        type:
+          - "null"
+          - string
+      last_update:
+        type:
+          - "null"
+          - string
+      launches:
+        type: array
+        items:
+          type:
+            - "null"
+            - string
+      reuse_count:
+        type: number
+      rtls_attempts:
+        type: number
+      rtls_landings:
+        type: number
+      serial:
+        type:
+          - "null"
+          - string
+      status:
+        type:
+          - "null"
+          - string
+    additionalProperties: true
+  dragons:
+    type: object
+    $schema: http://json-schema.org/schema#
+    properties:
+      type:
+        type:
+          - "null"
+          - string
+      active:
+        type: boolean
+      crew_capacity:
+        type: number
+      description:
+        type:
+          - "null"
+          - string
+      diameter:
+        type: object
+        properties:
+          feet:
             type: number
-          vehicles:
+          meters:
             type: number
+      dry_mass_kg:
+        type: number
+      dry_mass_lb:
+        type: number
+      first_flight:
+        type:
+          - "null"
+          - string
+      flickr_images:
+        type: array
+        items:
+          type:
+            - "null"
+            - string
+      heat_shield:
         type: object
-    retriever:
-      type: SimpleRetriever
-      requester:
-        type: HttpRequester
-        url_base: https://api.spacexdata.com/v4/
-        path: /company
-        http_method: GET
-        request_parameters: {}
-        request_headers: {}
-        authenticator:
-          type: NoAuth
-        request_body_json: {}
-      record_selector:
-        type: RecordSelector
-        extractor:
-          type: DpathExtractor
-          field_path: []
-      paginator:
-        type: NoPagination
-  - type: DeclarativeStream
-    name: crew
-    primary_key:
-      - id
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/schema#
         properties:
-          agency:
-            type:
-              - "null"
-              - string
-          id:
+          dev_partner:
             type:
               - "null"
               - string
-          image:
-            type:
-              - "null"
-              - string
-          launches:
-            items:
-              type:
-                - "null"
-                - string
-            type: array
-          name:
-            type:
-              - "null"
-              - string
-          status:
-            type:
-              - "null"
-              - string
-          wikipedia:
+          material:
             type:
               - "null"
               - string
+          size_meters:
+            type: number
+          temp_degrees:
+            type: number
+      height_w_trunk:
         type: object
-    retriever:
-      type: SimpleRetriever
-      requester:
-        type: HttpRequester
-        url_base: https://api.spacexdata.com/v4/
-        path: /crew
-        http_method: GET
-        request_parameters: {}
-        request_headers: {}
-        authenticator:
-          type: NoAuth
-        request_body_json: {}
-      record_selector:
-        type: RecordSelector
-        extractor:
-          type: DpathExtractor
-          field_path: []
-      paginator:
-        type: NoPagination
-  - type: DeclarativeStream
-    name: cores
-    primary_key:
-      - id
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/schema#
         properties:
-          asds_attempts:
+          feet:
             type: number
-          asds_landings:
-            type: number
-          block:
-            type:
-              - "null"
-              - number
-          id:
-            type:
-              - "null"
-              - string
-          last_update:
-            type:
-              - "null"
-              - string
-          launches:
-            items:
-              type:
-                - "null"
-                - string
-            type: array
-          reuse_count:
+          meters:
             type: number
-          rtls_attempts:
+      id:
+        type:
+          - "null"
+          - string
+      launch_payload_mass:
+        type: object
+        properties:
+          kg:
             type: number
-          rtls_landings:
+          lb:
             type: number
-          serial:
-            type:
-              - "null"
-              - string
-          status:
-            type:
-              - "null"
-              - string
+      launch_payload_vol:
         type: object
-    retriever:
-      type: SimpleRetriever
-      requester:
-        type: HttpRequester
-        url_base: https://api.spacexdata.com/v4/
-        path: /cores
-        http_method: GET
-        request_parameters: {}
-        request_headers: {}
-        authenticator:
-          type: NoAuth
-        request_body_json: {}
-      record_selector:
-        type: RecordSelector
-        extractor:
-          type: DpathExtractor
-          field_path: []
-      paginator:
-        type: NoPagination
-  - type: DeclarativeStream
-    name: dragons
-    primary_key:
-      - id
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/schema#
         properties:
-          active:
-            type: boolean
-          crew_capacity:
+          cubic_feet:
             type: number
-          description:
-            type:
-              - "null"
-              - string
-          diameter:
+          cubic_meters:
+            type: number
+      name:
+        type:
+          - "null"
+          - string
+      orbit_duration_yr:
+        type: number
+      pressurized_capsule:
+        type: object
+        properties:
+          payload_volume:
+            type: object
             properties:
-              feet:
+              cubic_feet:
                 type: number
-              meters:
+              cubic_meters:
                 type: number
-            type: object
-          dry_mass_kg:
+      return_payload_mass:
+        type: object
+        properties:
+          kg:
+            type: number
+          lb:
             type: number
-          dry_mass_lb:
+      return_payload_vol:
+        type: object
+        properties:
+          cubic_feet:
             type: number
-          first_flight:
+          cubic_meters:
+            type: number
+      sidewall_angle_deg:
+        type: number
+      thrusters:
+        type: array
+        items:
+          type: object
+          properties:
             type:
-              - "null"
-              - string
-          flickr_images:
-            items:
               type:
                 - "null"
                 - string
-            type: array
-          heat_shield:
-            properties:
-              dev_partner:
-                type:
-                  - "null"
-                  - string
-              material:
-                type:
-                  - "null"
-                  - string
-              size_meters:
-                type: number
-              temp_degrees:
-                type: number
-            type: object
-          height_w_trunk:
-            properties:
-              feet:
-                type: number
-              meters:
-                type: number
-            type: object
-          id:
-            type:
-              - "null"
-              - string
-          launch_payload_mass:
-            properties:
-              kg:
-                type: number
-              lb:
-                type: number
-            type: object
-          launch_payload_vol:
-            properties:
-              cubic_feet:
-                type: number
-              cubic_meters:
-                type: number
-            type: object
-          name:
-            type:
-              - "null"
-              - string
-          orbit_duration_yr:
-            type: number
-          pressurized_capsule:
-            properties:
-              payload_volume:
-                properties:
-                  cubic_feet:
-                    type: number
-                  cubic_meters:
-                    type: number
-                type: object
+            amount:
+              type: number
+            fuel_1:
+              type:
+                - "null"
+                - string
+            fuel_2:
+              type:
+                - "null"
+                - string
+            isp:
+              type: number
+            pods:
+              type: number
+            thrust:
+              type: object
+              properties:
+                kN:
+                  type: number
+                lbf:
+                  type: number
+      trunk:
+        type: object
+        properties:
+          cargo:
             type: object
-          return_payload_mass:
             properties:
-              kg:
-                type: number
-              lb:
+              solar_array:
                 type: number
+              unpressurized_cargo:
+                type: boolean
+          trunk_volume:
             type: object
-          return_payload_vol:
             properties:
               cubic_feet:
                 type: number
               cubic_meters:
                 type: number
-            type: object
-          sidewall_angle_deg:
-            type: number
-          thrusters:
-            items:
-              properties:
-                amount:
-                  type: number
-                fuel_1:
-                  type:
-                    - "null"
-                    - string
-                fuel_2:
-                  type:
-                    - "null"
-                    - string
-                isp:
-                  type: number
-                pods:
-                  type: number
-                thrust:
-                  properties:
-                    kN:
-                      type: number
-                    lbf:
-                      type: number
-                  type: object
-                type:
-                  type:
-                    - "null"
-                    - string
-              type: object
-            type: array
-          trunk:
-            properties:
-              cargo:
-                properties:
-                  solar_array:
-                    type: number
-                  unpressurized_cargo:
-                    type: boolean
-                type: object
-              trunk_volume:
-                properties:
-                  cubic_feet:
-                    type: number
-                  cubic_meters:
-                    type: number
-                type: object
-            type: object
-          type:
-            type:
-              - "null"
-              - string
-          wikipedia:
-            type:
-              - "null"
-              - string
+      wikipedia:
+        type:
+          - "null"
+          - string
+    additionalProperties: true
+  landpads:
+    type: object
+    $schema: http://json-schema.org/schema#
+    properties:
+      type:
+        type:
+          - "null"
+          - string
+      details:
+        type:
+          - "null"
+          - string
+      full_name:
+        type:
+          - "null"
+          - string
+      id:
+        type:
+          - "null"
+          - string
+      images:
         type: object
-    retriever:
-      type: SimpleRetriever
-      requester:
-        type: HttpRequester
-        url_base: https://api.spacexdata.com/v4/
-        path: /dragons
-        http_method: GET
-        request_parameters: {}
-        request_headers: {}
-        authenticator:
-          type: NoAuth
-        request_body_json: {}
-      record_selector:
-        type: RecordSelector
-        extractor:
-          type: DpathExtractor
-          field_path: []
-      paginator:
-        type: NoPagination
-  - type: DeclarativeStream
-    name: landpads
-    primary_key:
-      - id
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/schema#
-        properties:
-          details:
-            type:
-              - "null"
-              - string
-          full_name:
-            type:
-              - "null"
-              - string
-          id:
-            type:
-              - "null"
-              - string
-          images:
-            properties:
-              large:
-                items:
-                  type:
-                    - "null"
-                    - string
-                type: array
-            type: object
-          landing_attempts:
-            type: number
-          landing_successes:
-            type: number
-          latitude:
-            type: number
-          launches:
+        properties:
+          large:
+            type: array
             items:
               type:
                 - "null"
                 - string
-            type: array
-          locality:
-            type:
-              - "null"
-              - string
-          longitude:
-            type: number
-          name:
-            type:
-              - "null"
-              - string
-          region:
-            type:
-              - "null"
-              - string
-          status:
-            type:
-              - "null"
-              - string
+      landing_attempts:
+        type: number
+      landing_successes:
+        type: number
+      latitude:
+        type: number
+      launches:
+        type: array
+        items:
           type:
-            type:
-              - "null"
-              - string
-          wikipedia:
-            type:
-              - "null"
-              - string
+            - "null"
+            - string
+      locality:
+        type:
+          - "null"
+          - string
+      longitude:
+        type: number
+      name:
+        type:
+          - "null"
+          - string
+      region:
+        type:
+          - "null"
+          - string
+      status:
+        type:
+          - "null"
+          - string
+      wikipedia:
+        type:
+          - "null"
+          - string
+    additionalProperties: true
+  payloads:
+    type: object
+    $schema: http://json-schema.org/schema#
+    properties:
+      type:
+        type:
+          - "null"
+          - string
+      apoapsis_km:
+        type:
+          - "null"
+          - number
+      arg_of_pericenter:
+        type:
+          - "null"
+          - number
+      customers:
+        type: array
+        items:
+          type:
+            - "null"
+            - string
+      dragon:
         type: object
-    retriever:
-      type: SimpleRetriever
-      requester:
-        type: HttpRequester
-        url_base: https://api.spacexdata.com/v4/
-        path: /landpads
-        http_method: GET
-        request_parameters: {}
-        request_headers: {}
-        authenticator:
-          type: NoAuth
-        request_body_json: {}
-      record_selector:
-        type: RecordSelector
-        extractor:
-          type: DpathExtractor
-          field_path: []
-      paginator:
-        type: NoPagination
-  - type: DeclarativeStream
-    name: payloads
-    primary_key:
-      - id
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/schema#
         properties:
-          apoapsis_km:
-            type:
-              - "null"
-              - number
-          arg_of_pericenter:
-            type:
-              - "null"
-              - number
-          customers:
-            items:
-              type:
-                - "null"
-                - string
-            type: array
-          dragon:
-            properties:
-              capsule:
-                type:
-                  - "null"
-                  - string
-              flight_time_sec:
-                type:
-                  - "null"
-                  - number
-              land_landing:
-                type:
-                  - boolean
-                  - "null"
-              manifest:
-                type:
-                  - "null"
-                  - string
-              mass_returned_kg:
-                type:
-                  - "null"
-                  - number
-              mass_returned_lbs:
-                type:
-                  - "null"
-                  - number
-              water_landing:
-                type:
-                  - boolean
-                  - "null"
-            type: object
-          eccentricity:
-            type:
-              - "null"
-              - number
-          epoch:
-            type:
-              - "null"
-              - string
-          id:
-            type:
-              - "null"
-              - string
-          inclination_deg:
-            type:
-              - "null"
-              - number
-          launch:
+          capsule:
             type:
               - "null"
               - string
-          lifespan_years:
-            type:
-              - "null"
-              - number
-          longitude:
-            type:
-              - "null"
-              - number
-          manufacturers:
-            items:
-              type:
-                - "null"
-                - string
-            type: array
-          mass_kg:
-            type:
-              - "null"
-              - number
-          mass_lbs:
-            type:
-              - "null"
-              - number
-          mean_anomaly:
+          flight_time_sec:
             type:
               - "null"
               - number
-          mean_motion:
+          land_landing:
             type:
+              - boolean
               - "null"
-              - number
-          name:
-            type:
-              - "null"
-              - string
-          nationalities:
-            items:
-              type:
-                - "null"
-                - string
-            type: array
-          norad_ids:
-            items:
-              type: number
-            type: array
-          orbit:
+          manifest:
             type:
               - "null"
               - string
-          periapsis_km:
-            type:
-              - "null"
-              - number
-          period_min:
+          mass_returned_kg:
             type:
               - "null"
               - number
-          raan:
+          mass_returned_lbs:
             type:
               - "null"
               - number
-          reference_system:
-            type:
-              - "null"
-              - string
-          regime:
-            type:
-              - "null"
-              - string
-          reused:
-            type: boolean
-          semi_major_axis_km:
+          water_landing:
             type:
+              - boolean
               - "null"
-              - number
+      eccentricity:
+        type:
+          - "null"
+          - number
+      epoch:
+        type:
+          - "null"
+          - string
+      id:
+        type:
+          - "null"
+          - string
+      inclination_deg:
+        type:
+          - "null"
+          - number
+      launch:
+        type:
+          - "null"
+          - string
+      lifespan_years:
+        type:
+          - "null"
+          - number
+      longitude:
+        type:
+          - "null"
+          - number
+      manufacturers:
+        type: array
+        items:
           type:
-            type:
-              - "null"
-              - string
+            - "null"
+            - string
+      mass_kg:
+        type:
+          - "null"
+          - number
+      mass_lbs:
+        type:
+          - "null"
+          - number
+      mean_anomaly:
+        type:
+          - "null"
+          - number
+      mean_motion:
+        type:
+          - "null"
+          - number
+      name:
+        type:
+          - "null"
+          - string
+      nationalities:
+        type: array
+        items:
+          type:
+            - "null"
+            - string
+      norad_ids:
+        type: array
+        items:
+          type: number
+      orbit:
+        type:
+          - "null"
+          - string
+      periapsis_km:
+        type:
+          - "null"
+          - number
+      period_min:
+        type:
+          - "null"
+          - number
+      raan:
+        type:
+          - "null"
+          - number
+      reference_system:
+        type:
+          - "null"
+          - string
+      regime:
+        type:
+          - "null"
+          - string
+      reused:
+        type: boolean
+      semi_major_axis_km:
+        type:
+          - "null"
+          - number
+    additionalProperties: true
+  history:
+    type: object
+    $schema: http://json-schema.org/schema#
+    properties:
+      details:
+        type:
+          - "null"
+          - string
+      event_date_unix:
+        type: number
+      event_date_utc:
+        type:
+          - "null"
+          - string
+      id:
+        type:
+          - "null"
+          - string
+      links:
         type: object
-    retriever:
-      type: SimpleRetriever
-      requester:
-        type: HttpRequester
-        url_base: https://api.spacexdata.com/v4/
-        path: /payloads
-        http_method: GET
-        request_parameters: {}
-        request_headers: {}
-        authenticator:
-          type: NoAuth
-        request_body_json: {}
-      record_selector:
-        type: RecordSelector
-        extractor:
-          type: DpathExtractor
-          field_path: []
-      paginator:
-        type: NoPagination
-  - type: DeclarativeStream
-    name: history
-    primary_key:
-      - id
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/schema#
         properties:
-          details:
+          article:
             type:
               - "null"
               - string
-          event_date_unix:
+      title:
+        type:
+          - "null"
+          - string
+    additionalProperties: true
+  rockets:
+    type: object
+    $schema: http://json-schema.org/schema#
+    properties:
+      type:
+        type:
+          - "null"
+          - string
+      active:
+        type: boolean
+      boosters:
+        type: number
+      company:
+        type:
+          - "null"
+          - string
+      cost_per_launch:
+        type: number
+      country:
+        type:
+          - "null"
+          - string
+      description:
+        type:
+          - "null"
+          - string
+      diameter:
+        type: object
+        properties:
+          feet:
+            type: number
+          meters:
             type: number
-          event_date_utc:
+      engines:
+        type: object
+        properties:
+          version:
             type:
               - "null"
               - string
-          id:
+          type:
             type:
               - "null"
               - string
-          links:
-            properties:
-              article:
-                type:
-                  - "null"
-                  - string
-            type: object
-          title:
+          engine_loss_max:
             type:
               - "null"
-              - string
-        type: object
-    retriever:
-      type: SimpleRetriever
-      requester:
-        type: HttpRequester
-        url_base: https://api.spacexdata.com/v4/
-        path: /history
-        http_method: GET
-        request_parameters: {}
-        request_headers: {}
-        authenticator:
-          type: NoAuth
-        request_body_json: {}
-      record_selector:
-        type: RecordSelector
-        extractor:
-          type: DpathExtractor
-          field_path: []
-      paginator:
-        type: NoPagination
-  - type: DeclarativeStream
-    name: rockets
-    primary_key:
-      - id
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/schema#
-        properties:
-          active:
-            type: boolean
-          boosters:
-            type: number
-          company:
+              - number
+          isp:
+            type: object
+            properties:
+              sea_level:
+                type: number
+              vacuum:
+                type: number
+          layout:
             type:
               - "null"
               - string
-          cost_per_launch:
+          number:
             type: number
-          country:
+          propellant_1:
             type:
               - "null"
               - string
-          description:
+          propellant_2:
             type:
               - "null"
               - string
-          diameter:
-            properties:
-              feet:
-                type: number
-              meters:
-                type: number
-            type: object
-          engines:
-            properties:
-              engine_loss_max:
-                type:
-                  - "null"
-                  - number
-              isp:
-                properties:
-                  sea_level:
-                    type: number
-                  vacuum:
-                    type: number
-                type: object
-              layout:
-                type:
-                  - "null"
-                  - string
-              number:
-                type: number
-              propellant_1:
-                type:
-                  - "null"
-                  - string
-              propellant_2:
-                type:
-                  - "null"
-                  - string
-              thrust_sea_level:
-                properties:
-                  kN:
-                    type: number
-                  lbf:
-                    type: number
-                type: object
-              thrust_to_weight:
-                type: number
-              thrust_vacuum:
-                properties:
-                  kN:
-                    type: number
-                  lbf:
-                    type: number
-                type: object
-              type:
-                type:
-                  - "null"
-                  - string
-              version:
-                type:
-                  - "null"
-                  - string
+          thrust_sea_level:
             type: object
-          first_flight:
-            type:
-              - "null"
-              - string
-          first_stage:
             properties:
-              burn_time_sec:
-                type:
-                  - "null"
-                  - number
-              engines:
+              kN:
                 type: number
-              fuel_amount_tons:
+              lbf:
                 type: number
-              reusable:
-                type: boolean
-              thrust_sea_level:
-                properties:
-                  kN:
-                    type: number
-                  lbf:
-                    type: number
-                type: object
-              thrust_vacuum:
-                properties:
-                  kN:
-                    type: number
-                  lbf:
-                    type: number
-                type: object
+          thrust_to_weight:
+            type: number
+          thrust_vacuum:
             type: object
-          flickr_images:
-            items:
-              type:
-                - "null"
-                - string
-            type: array
-          height:
             properties:
-              feet:
+              kN:
                 type: number
-              meters:
+              lbf:
                 type: number
-            type: object
-          id:
+      first_flight:
+        type:
+          - "null"
+          - string
+      first_stage:
+        type: object
+        properties:
+          burn_time_sec:
             type:
               - "null"
-              - string
-          landing_legs:
-            properties:
-              material:
-                type:
-                  - "null"
-                  - string
-              number:
-                type: number
+              - number
+          engines:
+            type: number
+          fuel_amount_tons:
+            type: number
+          reusable:
+            type: boolean
+          thrust_sea_level:
             type: object
-          mass:
             properties:
-              kg:
+              kN:
                 type: number
-              lb:
+              lbf:
                 type: number
+          thrust_vacuum:
             type: object
-          name:
-            type:
-              - "null"
-              - string
-          payload_weights:
-            items:
-              properties:
-                id:
-                  type:
-                    - "null"
-                    - string
-                kg:
-                  type: number
-                lb:
-                  type: number
-                name:
-                  type:
-                    - "null"
-                    - string
-              type: object
-            type: array
-          second_stage:
             properties:
-              burn_time_sec:
-                type:
-                  - "null"
-                  - number
-              engines:
+              kN:
                 type: number
-              fuel_amount_tons:
+              lbf:
                 type: number
-              payloads:
-                properties:
-                  composite_fairing:
-                    properties:
-                      diameter:
-                        properties:
-                          feet:
-                            type:
-                              - "null"
-                              - number
-                          meters:
-                            type:
-                              - "null"
-                              - number
-                        type: object
-                      height:
-                        properties:
-                          feet:
-                            type:
-                              - "null"
-                              - number
-                          meters:
-                            type:
-                              - "null"
-                              - number
-                        type: object
-                    type: object
-                  option_1:
-                    type:
-                      - "null"
-                      - string
-                type: object
-              reusable:
-                type: boolean
-              thrust:
-                properties:
-                  kN:
-                    type: number
-                  lbf:
-                    type: number
-                type: object
-            type: object
-          stages:
+      flickr_images:
+        type: array
+        items:
+          type:
+            - "null"
+            - string
+      height:
+        type: object
+        properties:
+          feet:
             type: number
-          success_rate_pct:
+          meters:
             type: number
-          type:
-            type:
-              - "null"
-              - string
-          wikipedia:
-            type:
-              - "null"
-              - string
+      id:
+        type:
+          - "null"
+          - string
+      landing_legs:
         type: object
-    retriever:
-      type: SimpleRetriever
-      requester:
-        type: HttpRequester
-        url_base: https://api.spacexdata.com/v4/
-        path: /rockets
-        http_method: GET
-        request_parameters: {}
-        request_headers: {}
-        authenticator:
-          type: NoAuth
-        request_body_json: {}
-      record_selector:
-        type: RecordSelector
-        extractor:
-          type: DpathExtractor
-          field_path: []
-      paginator:
-        type: NoPagination
-  - type: DeclarativeStream
-    name: roadster
-    primary_key:
-      - id
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/schema#
-        properties:
-          apoapsis_au:
-            type: number
-          details:
+        properties:
+          material:
             type:
               - "null"
               - string
-          earth_distance_km:
-            type: number
-          earth_distance_mi:
+          number:
             type: number
-          eccentricity:
+      mass:
+        type: object
+        properties:
+          kg:
             type: number
-          epoch_jd:
+          lb:
             type: number
-          flickr_images:
-            items:
+      name:
+        type:
+          - "null"
+          - string
+      payload_weights:
+        type: array
+        items:
+          type: object
+          properties:
+            id:
               type:
                 - "null"
                 - string
-            type: array
-          id:
-            type:
-              - "null"
-              - string
-          inclination:
-            type: number
-          launch_date_unix:
-            type: number
-          launch_date_utc:
+            kg:
+              type: number
+            lb:
+              type: number
+            name:
+              type:
+                - "null"
+                - string
+      second_stage:
+        type: object
+        properties:
+          burn_time_sec:
             type:
               - "null"
-              - string
-          launch_mass_kg:
+              - number
+          engines:
             type: number
-          launch_mass_lbs:
+          fuel_amount_tons:
             type: number
-          longitude:
+          payloads:
+            type: object
+            properties:
+              composite_fairing:
+                type: object
+                properties:
+                  diameter:
+                    type: object
+                    properties:
+                      feet:
+                        type:
+                          - "null"
+                          - number
+                      meters:
+                        type:
+                          - "null"
+                          - number
+                  height:
+                    type: object
+                    properties:
+                      feet:
+                        type:
+                          - "null"
+                          - number
+                      meters:
+                        type:
+                          - "null"
+                          - number
+              option_1:
+                type:
+                  - "null"
+                  - string
+          reusable:
+            type: boolean
+          thrust:
+            type: object
+            properties:
+              kN:
+                type: number
+              lbf:
+                type: number
+      stages:
+        type: number
+      success_rate_pct:
+        type: number
+      wikipedia:
+        type:
+          - "null"
+          - string
+    additionalProperties: true
+  roadster:
+    type: object
+    $schema: http://json-schema.org/schema#
+    properties:
+      apoapsis_au:
+        type: number
+      details:
+        type:
+          - "null"
+          - string
+      earth_distance_km:
+        type: number
+      earth_distance_mi:
+        type: number
+      eccentricity:
+        type: number
+      epoch_jd:
+        type: number
+      flickr_images:
+        type: array
+        items:
+          type:
+            - "null"
+            - string
+      id:
+        type:
+          - "null"
+          - string
+      inclination:
+        type: number
+      launch_date_unix:
+        type: number
+      launch_date_utc:
+        type:
+          - "null"
+          - string
+      launch_mass_kg:
+        type: number
+      launch_mass_lbs:
+        type: number
+      longitude:
+        type: number
+      mars_distance_km:
+        type: number
+      mars_distance_mi:
+        type: number
+      name:
+        type:
+          - "null"
+          - string
+      norad_id:
+        type: number
+      orbit_type:
+        type:
+          - "null"
+          - string
+      periapsis_arg:
+        type: number
+      periapsis_au:
+        type: number
+      period_days:
+        type: number
+      semi_major_axis_au:
+        type: number
+      speed_kph:
+        type: number
+      speed_mph:
+        type: number
+      video:
+        type:
+          - "null"
+          - string
+      wikipedia:
+        type:
+          - "null"
+          - string
+    additionalProperties: true
+  ships:
+    type: object
+    $schema: http://json-schema.org/schema#
+    properties:
+      type:
+        type:
+          - "null"
+          - string
+      abs:
+        type:
+          - "null"
+          - number
+      active:
+        type: boolean
+      class:
+        type:
+          - "null"
+          - number
+      course_deg:
+        type:
+          - "null"
+          - number
+      home_port:
+        type:
+          - "null"
+          - string
+      id:
+        type:
+          - "null"
+          - string
+      image:
+        type:
+          - "null"
+          - string
+      imo:
+        type:
+          - "null"
+          - number
+      last_ais_update:
+        type:
+          - "null"
+          - string
+      latitude:
+        type:
+          - "null"
+          - number
+      launches:
+        type: array
+        items:
+          type:
+            - "null"
+            - string
+      legacy_id:
+        type:
+          - "null"
+          - string
+      link:
+        type:
+          - "null"
+          - string
+      longitude:
+        type:
+          - "null"
+          - number
+      mass_kg:
+        type:
+          - "null"
+          - number
+      mass_lbs:
+        type:
+          - "null"
+          - number
+      mmsi:
+        type:
+          - "null"
+          - number
+      model:
+        type:
+          - "null"
+          - string
+      name:
+        type:
+          - "null"
+          - string
+      roles:
+        type: array
+        items:
+          type:
+            - "null"
+            - string
+      speed_kn:
+        type:
+          - "null"
+          - number
+      status:
+        type:
+          - "null"
+          - string
+      year_built:
+        type:
+          - "null"
+          - number
+    additionalProperties: true
+  starlink:
+    type: object
+    $schema: http://json-schema.org/schema#
+    properties:
+      version:
+        type:
+          - "null"
+          - string
+      height_km:
+        type:
+          - "null"
+          - number
+      id:
+        type:
+          - "null"
+          - string
+      latitude:
+        type:
+          - "null"
+          - number
+      launch:
+        type:
+          - "null"
+          - string
+      longitude:
+        type:
+          - "null"
+          - number
+      spaceTrack:
+        type: object
+        properties:
+          APOAPSIS:
             type: number
-          mars_distance_km:
+          ARG_OF_PERICENTER:
             type: number
-          mars_distance_mi:
+          BSTAR:
             type: number
-          name:
+          CCSDS_OMM_VERS:
             type:
               - "null"
               - string
-          norad_id:
-            type: number
-          orbit_type:
+          CENTER_NAME:
             type:
               - "null"
               - string
-          periapsis_arg:
-            type: number
-          periapsis_au:
-            type: number
-          period_days:
-            type: number
-          semi_major_axis_au:
-            type: number
-          speed_kph:
-            type: number
-          speed_mph:
-            type: number
-          video:
+          CLASSIFICATION_TYPE:
             type:
               - "null"
               - string
-          wikipedia:
+          COMMENT:
             type:
               - "null"
               - string
-        type: object
-    retriever:
-      type: SimpleRetriever
-      requester:
-        type: HttpRequester
-        url_base: https://api.spacexdata.com/v4/
-        path: /roadster
-        http_method: GET
-        request_parameters: {}
-        request_headers: {}
-        authenticator:
-          type: NoAuth
-        request_body_json: {}
-      record_selector:
-        type: RecordSelector
-        extractor:
-          type: DpathExtractor
-          field_path: []
-      paginator:
-        type: NoPagination
-  - type: DeclarativeStream
-    name: ships
-    primary_key:
-      - id
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/schema#
-        properties:
-          abs:
-            type:
-              - "null"
-              - number
-          active:
-            type: boolean
-          class:
-            type:
-              - "null"
-              - number
-          home_port:
+          COUNTRY_CODE:
             type:
               - "null"
               - string
-          id:
+          CREATION_DATE:
             type:
               - "null"
               - string
-          image:
+          DECAYED:
+            type: number
+          DECAY_DATE:
             type:
               - "null"
               - string
-          imo:
-            type:
-              - "null"
-              - number
-          latitude:
-            type:
-              - "null"
-              - number
-          course_deg:
-            type:
-              - "null"
-              - number
-          last_ais_update:
+          ECCENTRICITY:
+            type: number
+          ELEMENT_SET_NO:
+            type: number
+          EPHEMERIS_TYPE:
+            type: number
+          EPOCH:
             type:
               - "null"
               - string
-          speed_kn:
-            type:
-              - "null"
-              - number
-          launches:
-            items:
-              type:
-                - "null"
-                - string
-            type: array
-          legacy_id:
+          FILE:
+            type: number
+          GP_ID:
+            type: number
+          INCLINATION:
+            type: number
+          LAUNCH_DATE:
             type:
               - "null"
               - string
-          link:
+          MEAN_ANOMALY:
+            type: number
+          MEAN_ELEMENT_THEORY:
             type:
               - "null"
               - string
-          longitude:
-            type:
-              - "null"
-              - number
-          mass_kg:
-            type:
-              - "null"
-              - number
-          mass_lbs:
-            type:
-              - "null"
-              - number
-          mmsi:
-            type:
-              - "null"
-              - number
-          model:
+          MEAN_MOTION:
+            type: number
+          MEAN_MOTION_DDOT:
+            type: number
+          MEAN_MOTION_DOT:
+            type: number
+          NORAD_CAT_ID:
+            type: number
+          OBJECT_ID:
             type:
               - "null"
               - string
-          name:
+          OBJECT_NAME:
             type:
               - "null"
               - string
-          roles:
-            items:
-              type:
-                - "null"
-                - string
-            type: array
-          status:
+          OBJECT_TYPE:
             type:
               - "null"
               - string
-          type:
+          ORIGINATOR:
             type:
               - "null"
               - string
-          year_built:
-            type:
-              - "null"
-              - number
-        type: object
-    retriever:
-      type: SimpleRetriever
-      requester:
-        type: HttpRequester
-        url_base: https://api.spacexdata.com/v4/
-        path: /ships
-        http_method: GET
-        request_parameters: {}
-        request_headers: {}
-        authenticator:
-          type: NoAuth
-        request_body_json: {}
-      record_selector:
-        type: RecordSelector
-        extractor:
-          type: DpathExtractor
-          field_path: []
-      paginator:
-        type: NoPagination
-  - type: DeclarativeStream
-    name: starlink
-    primary_key:
-      - id
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/schema#
-        properties:
-          height_km:
+          PERIAPSIS:
+            type: number
+          PERIOD:
+            type: number
+          RA_OF_ASC_NODE:
+            type: number
+          RCS_SIZE:
             type:
               - "null"
-              - number
-          id:
+              - string
+          REF_FRAME:
             type:
               - "null"
               - string
-          latitude:
+          REV_AT_EPOCH:
+            type: number
+          SEMIMAJOR_AXIS:
+            type: number
+          SITE:
             type:
               - "null"
-              - number
-          launch:
+              - string
+          TIME_SYSTEM:
             type:
               - "null"
               - string
-          longitude:
+          TLE_LINE0:
             type:
               - "null"
-              - number
-          spaceTrack:
-            properties:
-              APOAPSIS:
-                type: number
-              ARG_OF_PERICENTER:
-                type: number
-              BSTAR:
-                type: number
-              CCSDS_OMM_VERS:
-                type:
-                  - "null"
-                  - string
-              CENTER_NAME:
-                type:
-                  - "null"
-                  - string
-              CLASSIFICATION_TYPE:
-                type:
-                  - "null"
-                  - string
-              COMMENT:
-                type:
-                  - "null"
-                  - string
-              COUNTRY_CODE:
-                type:
-                  - "null"
-                  - string
-              CREATION_DATE:
-                type:
-                  - "null"
-                  - string
-              DECAYED:
-                type: number
-              DECAY_DATE:
-                type:
-                  - "null"
-                  - string
-              ECCENTRICITY:
-                type: number
-              ELEMENT_SET_NO:
-                type: number
-              EPHEMERIS_TYPE:
-                type: number
-              EPOCH:
-                type:
-                  - "null"
-                  - string
-              FILE:
-                type: number
-              GP_ID:
-                type: number
-              INCLINATION:
-                type: number
-              LAUNCH_DATE:
-                type:
-                  - "null"
-                  - string
-              MEAN_ANOMALY:
-                type: number
-              MEAN_ELEMENT_THEORY:
-                type:
-                  - "null"
-                  - string
-              MEAN_MOTION:
-                type: number
-              MEAN_MOTION_DDOT:
-                type: number
-              MEAN_MOTION_DOT:
-                type: number
-              NORAD_CAT_ID:
-                type: number
-              OBJECT_ID:
-                type:
-                  - "null"
-                  - string
-              OBJECT_NAME:
-                type:
-                  - "null"
-                  - string
-              OBJECT_TYPE:
-                type:
-                  - "null"
-                  - string
-              ORIGINATOR:
-                type:
-                  - "null"
-                  - string
-              PERIAPSIS:
-                type: number
-              PERIOD:
-                type: number
-              RA_OF_ASC_NODE:
-                type: number
-              RCS_SIZE:
-                type:
-                  - "null"
-                  - string
-              REF_FRAME:
-                type:
-                  - "null"
-                  - string
-              REV_AT_EPOCH:
-                type: number
-              SEMIMAJOR_AXIS:
-                type: number
-              SITE:
-                type:
-                  - "null"
-                  - string
-              TIME_SYSTEM:
-                type:
-                  - "null"
-                  - string
-              TLE_LINE0:
-                type:
-                  - "null"
-                  - string
-              TLE_LINE1:
-                type:
-                  - "null"
-                  - string
-              TLE_LINE2:
-                type:
-                  - "null"
-                  - string
-            type: object
-          velocity_kms:
+              - string
+          TLE_LINE1:
             type:
               - "null"
-              - number
-          version:
+              - string
+          TLE_LINE2:
             type:
               - "null"
               - string
-        type: object
-    retriever:
-      type: SimpleRetriever
-      requester:
-        type: HttpRequester
-        url_base: https://api.spacexdata.com/v4/
-        path: /starlink
-        http_method: GET
-        request_parameters: {}
-        request_headers: {}
-        authenticator:
-          type: NoAuth
-        request_body_json: {}
-      record_selector:
-        type: RecordSelector
-        extractor:
-          type: DpathExtractor
-          field_path: []
-      paginator:
-        type: NoPagination
-spec:
-  connection_specification:
-    $schema: http://json-schema.org/draft-07/schema#
-    type: object
-    required: []
-    properties:
-      id:
-        title: Unique ID for specific source target
-        type: string
-        desciption: Optional, For a specific ID
-        order: 0
-      options:
-        title: Configuration options for endpoints
-        type: string
-        desciption: >-
-          Optional, Possible values for an endpoint. Example values for
-          launches-latest, upcoming, past
-        order: 1
+      velocity_kms:
+        type:
+          - "null"
+          - number
     additionalProperties: true
-  type: Spec
-metadata:
-  autoImportSchema:
-    launches: false
-    capsules: false
-    company: false
-    crew: false
-    cores: false
-    dragons: false
-    landpads: false
-    payloads: false
-    history: false
-    rockets: false
-    roadster: false
-    ships: false
-    starlink: false
```

