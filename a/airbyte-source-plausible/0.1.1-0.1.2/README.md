# Comparing `tmp/airbyte_source_plausible-0.1.1.tar.gz` & `tmp/airbyte_source_plausible-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_plausible-0.1.1.tar", max compression
+gzip compressed data, was "airbyte_source_plausible-0.1.2.tar", max compression
```

## Comparing `airbyte_source_plausible-0.1.1.tar` & `airbyte_source_plausible-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     4550 2024-05-24 22:59:31.953217 airbyte_source_plausible-0.1.1/README.md
--rw-r--r--   0        0        0      760 2024-05-24 23:04:56.268013 airbyte_source_plausible-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      130 2024-05-24 22:59:31.953217 airbyte_source_plausible-0.1.1/source_plausible/__init__.py
--rw-r--r--   0        0        0     1314 2024-05-24 22:59:31.953217 airbyte_source_plausible-0.1.1/source_plausible/manifest.yaml
--rw-r--r--   0        0        0      239 2024-05-24 22:59:31.953217 airbyte_source_plausible-0.1.1/source_plausible/run.py
--rw-r--r--   0        0        0      954 2024-05-24 22:59:31.953217 airbyte_source_plausible-0.1.1/source_plausible/schemas/stats.json
--rw-r--r--   0        0        0      478 2024-05-24 22:59:31.953217 airbyte_source_plausible-0.1.1/source_plausible/source.py
--rw-r--r--   0        0        0     1286 2024-05-24 22:59:31.953217 airbyte_source_plausible-0.1.1/source_plausible/spec.yaml
--rw-r--r--   0        0        0     5262 1970-01-01 00:00:00.000000 airbyte_source_plausible-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     4552 2024-05-28 20:10:51.000000 airbyte_source_plausible-0.1.2/README.md
+-rw-r--r--   0        0        0      137 2024-05-28 20:10:51.000000 airbyte_source_plausible-0.1.2/main.py
+-rw-r--r--   0        0        0      789 2024-05-28 22:27:39.095546 airbyte_source_plausible-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      130 2024-05-28 20:10:51.000000 airbyte_source_plausible-0.1.2/source_plausible/__init__.py
+-rw-r--r--   0        0        0     3485 2024-05-28 20:10:51.000000 airbyte_source_plausible-0.1.2/source_plausible/manifest.yaml
+-rw-r--r--   0        0        0      231 2024-05-28 20:10:51.000000 airbyte_source_plausible-0.1.2/source_plausible/run.py
+-rw-r--r--   0        0        0      478 2024-05-28 20:10:51.000000 airbyte_source_plausible-0.1.2/source_plausible/source.py
+-rw-r--r--   0        0        0     5264 1970-01-01 00:00:00.000000 airbyte_source_plausible-0.1.2/PKG-INFO
```

### Comparing `airbyte_source_plausible-0.1.1/README.md` & `airbyte_source_plausible-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,78 +1,88 @@
 # Plausible source connector
 
-
-This is the repository for the Plausible source connector, written in Python.
+This is the repository for the Plausible configuration based source connector.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/plausible).
 
 ## Local development
 
 ### Prerequisites
-* Python (~=3.9)
-* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
+
+* Python (`^3.9`)
+* Poetry (`^1.7`) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
 
 ### Installing the connector
+
 From this connector directory, run:
 ```bash
 poetry install --with dev
 ```
 
 
 ### Create credentials
+
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/plausible)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_plausible/spec.yaml` file.
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `src/source_plausible/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
 
 ### Locally running the connector
+
 ```
 poetry run source-plausible spec
 poetry run source-plausible check --config secrets/config.json
 poetry run source-plausible discover --config secrets/config.json
 poetry run source-plausible read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
-### Running unit tests
-To run unit tests locally, from the connector directory run:
+### Running tests
+
+To run tests locally, from the connector directory run:
+
 ```
-poetry run pytest unit_tests
+poetry run pytest tests
 ```
 
 ### Building the docker image
+
 1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
 2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-plausible build
 ```
 
 An image will be available on your host with the tag `airbyte/source-plausible:dev`.
 
 
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-plausible:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-plausible:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-plausible:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-plausible:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-plausible test
 ```
 
 ### Customizing acceptance Tests
+
 Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
 ### Dependency Management
+
 All of your dependencies should be managed via Poetry. 
 To add a new dependency, run:
 ```bash
 poetry add <package-name>
 ```
 
 Please commit the changes to `pyproject.toml` and `poetry.lock` files.
```

### Comparing `airbyte_source_plausible-0.1.1/pyproject.toml` & `airbyte_source_plausible-0.1.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.1.1"
+version = "0.1.2"
 name = "airbyte-source-plausible"
 description = "Source implementation for Plausible."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
 documentation = "https://docs.airbyte.com/integrations/sources/plausible"
 homepage = "https://airbyte.com"
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_plausible" },
+    { include = "main.py" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
 airbyte-cdk = "1.0.0"
 
 [tool.poetry.scripts]
```

### Comparing `airbyte_source_plausible-0.1.1/PKG-INFO` & `airbyte_source_plausible-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-plausible
-Version: 0.1.1
+Version: 0.1.2
 Summary: Source implementation for Plausible.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -15,83 +15,93 @@
 Requires-Dist: airbyte-cdk (==1.0.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/plausible
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Plausible source connector
 
-
-This is the repository for the Plausible source connector, written in Python.
+This is the repository for the Plausible configuration based source connector.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/plausible).
 
 ## Local development
 
 ### Prerequisites
-* Python (~=3.9)
-* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
+
+* Python (`^3.9`)
+* Poetry (`^1.7`) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
 
 ### Installing the connector
+
 From this connector directory, run:
 ```bash
 poetry install --with dev
 ```
 
 
 ### Create credentials
+
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/plausible)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_plausible/spec.yaml` file.
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `src/source_plausible/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
 
 ### Locally running the connector
+
 ```
 poetry run source-plausible spec
 poetry run source-plausible check --config secrets/config.json
 poetry run source-plausible discover --config secrets/config.json
 poetry run source-plausible read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
-### Running unit tests
-To run unit tests locally, from the connector directory run:
+### Running tests
+
+To run tests locally, from the connector directory run:
+
 ```
-poetry run pytest unit_tests
+poetry run pytest tests
 ```
 
 ### Building the docker image
+
 1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
 2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-plausible build
 ```
 
 An image will be available on your host with the tag `airbyte/source-plausible:dev`.
 
 
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-plausible:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-plausible:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-plausible:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-plausible:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-plausible test
 ```
 
 ### Customizing acceptance Tests
+
 Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
 ### Dependency Management
+
 All of your dependencies should be managed via Poetry. 
 To add a new dependency, run:
 ```bash
 poetry add <package-name>
 ```
 
 Please commit the changes to `pyproject.toml` and `poetry.lock` files.
```

