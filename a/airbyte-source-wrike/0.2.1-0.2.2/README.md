# Comparing `tmp/airbyte_source_wrike-0.2.1.tar.gz` & `tmp/airbyte_source_wrike-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_wrike-0.2.1.tar", max compression
+gzip compressed data, was "airbyte_source_wrike-0.2.2.tar", max compression
```

## Comparing `airbyte_source_wrike-0.2.1.tar` & `airbyte_source_wrike-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,8 @@
--rw-r--r--   0        0        0     3979 2024-05-02 09:23:08.000000 airbyte_source_wrike-0.2.1/README.md
--rw-r--r--   0        0        0      731 2024-05-02 09:38:15.538648 airbyte_source_wrike-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      122 2024-05-02 09:23:08.000000 airbyte_source_wrike-0.2.1/source_wrike/__init__.py
--rw-r--r--   0        0        0     2158 2024-05-02 09:23:08.000000 airbyte_source_wrike-0.2.1/source_wrike/manifest.yaml
--rw-r--r--   0        0        0      227 2024-05-02 09:23:08.000000 airbyte_source_wrike-0.2.1/source_wrike/run.py
--rw-r--r--   0        0        0      543 2024-05-02 09:23:08.000000 airbyte_source_wrike-0.2.1/source_wrike/schemas/comments.json
--rw-r--r--   0        0        0     1596 2024-05-02 09:23:08.000000 airbyte_source_wrike-0.2.1/source_wrike/schemas/contacts.json
--rw-r--r--   0        0        0     1401 2024-05-02 09:23:08.000000 airbyte_source_wrike-0.2.1/source_wrike/schemas/customfields.json
--rw-r--r--   0        0        0     1050 2024-05-02 09:23:08.000000 airbyte_source_wrike-0.2.1/source_wrike/schemas/folders.json
--rw-r--r--   0        0        0     1974 2024-05-02 09:23:08.000000 airbyte_source_wrike-0.2.1/source_wrike/schemas/tasks.json
--rw-r--r--   0        0        0     1099 2024-05-02 09:23:08.000000 airbyte_source_wrike-0.2.1/source_wrike/schemas/workflows.json
--rw-r--r--   0        0        0      474 2024-05-02 09:23:08.000000 airbyte_source_wrike-0.2.1/source_wrike/source.py
--rw-r--r--   0        0        0     1075 2024-05-02 09:23:08.000000 airbyte_source_wrike-0.2.1/source_wrike/spec.yaml
--rw-r--r--   0        0        0     4678 1970-01-01 00:00:00.000000 airbyte_source_wrike-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     4472 2024-05-28 20:12:08.000000 airbyte_source_wrike-0.2.2/README.md
+-rw-r--r--   0        0        0      133 2024-05-28 20:12:08.000000 airbyte_source_wrike-0.2.2/main.py
+-rw-r--r--   0        0        0      760 2024-05-28 22:09:53.929170 airbyte_source_wrike-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      122 2024-05-28 20:12:08.000000 airbyte_source_wrike-0.2.2/source_wrike/__init__.py
+-rw-r--r--   0        0        0    15883 2024-05-28 20:12:08.000000 airbyte_source_wrike-0.2.2/source_wrike/manifest.yaml
+-rw-r--r--   0        0        0      223 2024-05-28 20:12:08.000000 airbyte_source_wrike-0.2.2/source_wrike/run.py
+-rw-r--r--   0        0        0      474 2024-05-28 20:12:08.000000 airbyte_source_wrike-0.2.2/source_wrike/source.py
+-rw-r--r--   0        0        0     5171 1970-01-01 00:00:00.000000 airbyte_source_wrike-0.2.2/PKG-INFO
```

### Comparing `airbyte_source_wrike-0.2.1/README.md` & `airbyte_source_wrike-0.2.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,103 @@
 # Wrike Source
 
 This is the repository for the Wrike configuration based source connector.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/wrike).
 
 ## Local development
 
-#### Create credentials
+### Prerequisites
+
+* Python (`^3.9`)
+* Poetry (`^1.7`) - installation instructions [here](https://python-poetry.org/docs/#installation)
+
+
+
+### Installing the connector
+
+From this connector directory, run:
+```bash
+poetry install --with dev
+```
+
+
+### Create credentials
+
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/wrike)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_wrike/spec.yaml` file.
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `src/source_wrike/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source wrike test creds`
-and place them into `secrets/config.json`.
 
-### Locally running the connector docker image
+### Locally running the connector
 
+```
+poetry run source-wrike spec
+poetry run source-wrike check --config secrets/config.json
+poetry run source-wrike discover --config secrets/config.json
+poetry run source-wrike read --config secrets/config.json --catalog sample_files/configured_catalog.json
+```
 
-#### Build
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
-```bash
-airbyte-ci connectors --name=source-wrike build
+### Running tests
+
+To run tests locally, from the connector directory run:
+
+```
+poetry run pytest tests
 ```
 
-An image will be built with the tag `airbyte/source-wrike:dev`.
+### Building the docker image
 
-**Via `docker build`:**
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
-docker build -t airbyte/source-wrike:dev .
+airbyte-ci connectors --name=source-wrike build
 ```
 
-#### Run
+An image will be available on your host with the tag `airbyte/source-wrike:dev`.
+
+
+### Running as a docker container
+
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-wrike:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-wrike:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-wrike:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-wrike:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
-## Testing
+### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-wrike test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-wrike test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/wrike.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/wrike.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_wrike-0.2.1/pyproject.toml` & `airbyte_source_wrike-0.2.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.2.1"
+version = "0.2.2"
 name = "airbyte-source-wrike"
 description = "Source implementation for Wrike."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
 documentation = "https://docs.airbyte.com/integrations/sources/wrike"
 homepage = "https://airbyte.com"
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_wrike" },
+    { include = "main.py" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
 airbyte-cdk = "^0"
 
 [tool.poetry.scripts]
```

### Comparing `airbyte_source_wrike-0.2.1/PKG-INFO` & `airbyte_source_wrike-0.2.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-wrike
-Version: 0.2.1
+Version: 0.2.2
 Summary: Source implementation for Wrike.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -20,68 +20,103 @@
 # Wrike Source
 
 This is the repository for the Wrike configuration based source connector.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/wrike).
 
 ## Local development
 
-#### Create credentials
+### Prerequisites
+
+* Python (`^3.9`)
+* Poetry (`^1.7`) - installation instructions [here](https://python-poetry.org/docs/#installation)
+
+
+
+### Installing the connector
+
+From this connector directory, run:
+```bash
+poetry install --with dev
+```
+
+
+### Create credentials
+
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/wrike)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_wrike/spec.yaml` file.
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `src/source_wrike/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source wrike test creds`
-and place them into `secrets/config.json`.
 
-### Locally running the connector docker image
+### Locally running the connector
 
+```
+poetry run source-wrike spec
+poetry run source-wrike check --config secrets/config.json
+poetry run source-wrike discover --config secrets/config.json
+poetry run source-wrike read --config secrets/config.json --catalog sample_files/configured_catalog.json
+```
 
-#### Build
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
-```bash
-airbyte-ci connectors --name=source-wrike build
+### Running tests
+
+To run tests locally, from the connector directory run:
+
+```
+poetry run pytest tests
 ```
 
-An image will be built with the tag `airbyte/source-wrike:dev`.
+### Building the docker image
 
-**Via `docker build`:**
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
-docker build -t airbyte/source-wrike:dev .
+airbyte-ci connectors --name=source-wrike build
 ```
 
-#### Run
+An image will be available on your host with the tag `airbyte/source-wrike:dev`.
+
+
+### Running as a docker container
+
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-wrike:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-wrike:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-wrike:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-wrike:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
-## Testing
+### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-wrike test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-wrike test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/wrike.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/wrike.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-
-
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

