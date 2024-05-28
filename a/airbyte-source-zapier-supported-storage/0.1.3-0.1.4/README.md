# Comparing `tmp/airbyte_source_zapier_supported_storage-0.1.3.tar.gz` & `tmp/airbyte_source_zapier_supported_storage-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_zapier_supported_storage-0.1.3.tar", max compression
+gzip compressed data, was "airbyte_source_zapier_supported_storage-0.1.4.tar", max compression
```

## Comparing `airbyte_source_zapier_supported_storage-0.1.3.tar` & `airbyte_source_zapier_supported_storage-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     4820 2024-04-20 23:35:47.000000 airbyte_source_zapier_supported_storage-0.1.3/README.md
--rw-r--r--   0        0        0      851 2024-04-21 00:13:02.668911 airbyte_source_zapier_supported_storage-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      156 2024-04-20 23:35:47.000000 airbyte_source_zapier_supported_storage-0.1.3/source_zapier_supported_storage/__init__.py
--rw-r--r--   0        0        0      870 2024-04-20 23:35:47.000000 airbyte_source_zapier_supported_storage-0.1.3/source_zapier_supported_storage/manifest.yaml
--rw-r--r--   0        0        0      280 2024-04-20 23:35:47.000000 airbyte_source_zapier_supported_storage-0.1.3/source_zapier_supported_storage/run.py
--rw-r--r--   0        0        0      491 2024-04-20 23:35:47.000000 airbyte_source_zapier_supported_storage-0.1.3/source_zapier_supported_storage/source.py
--rw-r--r--   0        0        0      418 2024-04-20 23:35:47.000000 airbyte_source_zapier_supported_storage-0.1.3/source_zapier_supported_storage/spec.yaml
--rw-r--r--   0        0        0     5578 1970-01-01 00:00:00.000000 airbyte_source_zapier_supported_storage-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     4830 2024-05-28 22:07:02.000000 airbyte_source_zapier_supported_storage-0.1.4/README.md
+-rw-r--r--   0        0        0      851 2024-05-28 22:28:09.873219 airbyte_source_zapier_supported_storage-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      156 2024-05-28 22:07:02.000000 airbyte_source_zapier_supported_storage-0.1.4/source_zapier_supported_storage/__init__.py
+-rw-r--r--   0        0        0     1416 2024-05-28 22:07:02.000000 airbyte_source_zapier_supported_storage-0.1.4/source_zapier_supported_storage/manifest.yaml
+-rw-r--r--   0        0        0      280 2024-05-28 22:07:02.000000 airbyte_source_zapier_supported_storage-0.1.4/source_zapier_supported_storage/run.py
+-rw-r--r--   0        0        0      491 2024-05-28 22:07:02.000000 airbyte_source_zapier_supported_storage-0.1.4/source_zapier_supported_storage/source.py
+-rw-r--r--   0        0        0     5588 1970-01-01 00:00:00.000000 airbyte_source_zapier_supported_storage-0.1.4/PKG-INFO
```

### Comparing `airbyte_source_zapier_supported_storage-0.1.3/README.md` & `airbyte_source_zapier_supported_storage-0.1.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,91 +1,104 @@
 # Zapier-Supported-Storage source connector
 
-
 This is the repository for the Zapier-Supported-Storage source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/zapier-supported-storage).
 
 ## Local development
 
 ### Prerequisites
-* Python (~=3.9)
-* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
+- Python (~=3.9)
+- Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
 ### Installing the connector
+
 From this connector directory, run:
+
 ```bash
 poetry install --with dev
 ```
 
-
 ### Create credentials
+
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/zapier-supported-storage)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_zapier_supported_storage/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-zapier-supported-storage spec
 poetry run source-zapier-supported-storage check --config secrets/config.json
 poetry run source-zapier-supported-storage discover --config secrets/config.json
 poetry run source-zapier-supported-storage read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
 ### Running unit tests
+
 To run unit tests locally, from the connector directory run:
+
 ```
 poetry run pytest unit_tests
 ```
 
 ### Building the docker image
+
 1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
 2. Run the following command to build the docker image:
+
 ```bash
 airbyte-ci connectors --name=source-zapier-supported-storage build
 ```
 
 An image will be available on your host with the tag `airbyte/source-zapier-supported-storage:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-zapier-supported-storage:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-zapier-supported-storage:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-zapier-supported-storage:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-zapier-supported-storage:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-zapier-supported-storage test
 ```
 
 ### Customizing acceptance Tests
+
 Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
 ### Dependency Management
-All of your dependencies should be managed via Poetry. 
+
+All of your dependencies should be managed via Poetry.
 To add a new dependency, run:
+
 ```bash
 poetry add <package-name>
 ```
 
 Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
 ## Publishing a new version of the connector
+
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
+
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-zapier-supported-storage test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/zapier-supported-storage.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_zapier_supported_storage-0.1.3/pyproject.toml` & `airbyte_source_zapier_supported_storage-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.1.3"
+version = "0.1.4"
 name = "airbyte-source-zapier-supported-storage"
 description = "Source implementation for Zapier Supported Storage."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_zapier_supported_storage-0.1.3/PKG-INFO` & `airbyte_source_zapier_supported_storage-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-zapier-supported-storage
-Version: 0.1.3
+Version: 0.1.4
 Summary: Source implementation for Zapier Supported Storage.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -15,96 +15,110 @@
 Requires-Dist: airbyte-cdk (==0.80.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/zapier-supported-storage
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Zapier-Supported-Storage source connector
 
-
 This is the repository for the Zapier-Supported-Storage source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/zapier-supported-storage).
 
 ## Local development
 
 ### Prerequisites
-* Python (~=3.9)
-* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
+- Python (~=3.9)
+- Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
 ### Installing the connector
+
 From this connector directory, run:
+
 ```bash
 poetry install --with dev
 ```
 
-
 ### Create credentials
+
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/zapier-supported-storage)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_zapier_supported_storage/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-zapier-supported-storage spec
 poetry run source-zapier-supported-storage check --config secrets/config.json
 poetry run source-zapier-supported-storage discover --config secrets/config.json
 poetry run source-zapier-supported-storage read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
 ### Running unit tests
+
 To run unit tests locally, from the connector directory run:
+
 ```
 poetry run pytest unit_tests
 ```
 
 ### Building the docker image
+
 1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
 2. Run the following command to build the docker image:
+
 ```bash
 airbyte-ci connectors --name=source-zapier-supported-storage build
 ```
 
 An image will be available on your host with the tag `airbyte/source-zapier-supported-storage:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-zapier-supported-storage:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-zapier-supported-storage:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-zapier-supported-storage:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-zapier-supported-storage:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-zapier-supported-storage test
 ```
 
 ### Customizing acceptance Tests
+
 Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
 ### Dependency Management
-All of your dependencies should be managed via Poetry. 
+
+All of your dependencies should be managed via Poetry.
 To add a new dependency, run:
+
 ```bash
 poetry add <package-name>
 ```
 
 Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
 ## Publishing a new version of the connector
+
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
+
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-zapier-supported-storage test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/zapier-supported-storage.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+
```

