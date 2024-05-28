# Comparing `tmp/airbyte-source-freshsales-1.0.0.tar.gz` & `tmp/airbyte_source_freshsales-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-freshsales-1.0.0.tar", last modified: Wed Jan 31 09:53:44 2024, max compression
+gzip compressed data, was "airbyte_source_freshsales-1.0.1.tar", max compression
```

## Comparing `airbyte-source-freshsales-1.0.0.tar` & `airbyte_source_freshsales-1.0.1.tar`

### file list

```diff
@@ -1,35 +1,8 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 09:53:44.484950 airbyte-source-freshsales-1.0.0/
--rw-r--r--   0 root         (0) root         (0)     5444 2024-01-31 09:53:44.484950 airbyte-source-freshsales-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5426 2024-01-31 09:40:47.000000 airbyte-source-freshsales-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 09:53:44.484950 airbyte-source-freshsales-1.0.0/airbyte_source_freshsales.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5444 2024-01-31 09:53:44.000000 airbyte-source-freshsales-1.0.0/airbyte_source_freshsales.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1080 2024-01-31 09:53:44.000000 airbyte-source-freshsales-1.0.0/airbyte_source_freshsales.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-31 09:53:44.000000 airbyte-source-freshsales-1.0.0/airbyte_source_freshsales.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-01-31 09:53:44.000000 airbyte-source-freshsales-1.0.0/airbyte_source_freshsales.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       78 2024-01-31 09:53:44.000000 airbyte-source-freshsales-1.0.0/airbyte_source_freshsales.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       36 2024-01-31 09:53:44.000000 airbyte-source-freshsales-1.0.0/airbyte_source_freshsales.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 09:53:44.480950 airbyte-source-freshsales-1.0.0/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-31 09:40:47.000000 airbyte-source-freshsales-1.0.0/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      314 2024-01-31 09:40:47.000000 airbyte-source-freshsales-1.0.0/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)     2488 2024-01-31 09:40:47.000000 airbyte-source-freshsales-1.0.0/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)      159 2024-01-31 09:40:47.000000 airbyte-source-freshsales-1.0.0/integration_tests/integration_test.py
--rw-r--r--   0 root         (0) root         (0)       44 2024-01-31 09:40:47.000000 airbyte-source-freshsales-1.0.0/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)       68 2024-01-31 09:40:47.000000 airbyte-source-freshsales-1.0.0/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)     5333 2024-01-31 09:53:44.484950 airbyte-source-freshsales-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      933 2024-01-31 09:53:42.000000 airbyte-source-freshsales-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 09:53:44.480950 airbyte-source-freshsales-1.0.0/source_freshsales/
--rw-r--r--   0 root         (0) root         (0)      132 2024-01-31 09:40:47.000000 airbyte-source-freshsales-1.0.0/source_freshsales/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8114 2024-01-31 09:40:47.000000 airbyte-source-freshsales-1.0.0/source_freshsales/manifest.yaml
--rw-r--r--   0 root         (0) root         (0)      242 2024-01-31 09:40:47.000000 airbyte-source-freshsales-1.0.0/source_freshsales/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 09:53:44.484950 airbyte-source-freshsales-1.0.0/source_freshsales/schemas/
--rw-r--r--   0 root         (0) root         (0)     3288 2024-01-31 09:40:47.000000 airbyte-source-freshsales-1.0.0/source_freshsales/schemas/accounts.json
--rw-r--r--   0 root         (0) root         (0)     1005 2024-01-31 09:40:47.000000 airbyte-source-freshsales-1.0.0/source_freshsales/schemas/completed_tasks.json
--rw-r--r--   0 root         (0) root         (0)     4170 2024-01-31 09:40:47.000000 airbyte-source-freshsales-1.0.0/source_freshsales/schemas/contacts.json
--rw-r--r--   0 root         (0) root         (0)     2776 2024-01-31 09:40:47.000000 airbyte-source-freshsales-1.0.0/source_freshsales/schemas/lost_deals.json
--rw-r--r--   0 root         (0) root         (0)     2776 2024-01-31 09:40:47.000000 airbyte-source-freshsales-1.0.0/source_freshsales/schemas/open_deals.json
--rw-r--r--   0 root         (0) root         (0)     1005 2024-01-31 09:40:47.000000 airbyte-source-freshsales-1.0.0/source_freshsales/schemas/open_tasks.json
--rw-r--r--   0 root         (0) root         (0)     1802 2024-01-31 09:40:47.000000 airbyte-source-freshsales-1.0.0/source_freshsales/schemas/past_appointments.json
--rw-r--r--   0 root         (0) root         (0)     1802 2024-01-31 09:40:47.000000 airbyte-source-freshsales-1.0.0/source_freshsales/schemas/upcoming_appointments.json
--rw-r--r--   0 root         (0) root         (0)     2776 2024-01-31 09:40:47.000000 airbyte-source-freshsales-1.0.0/source_freshsales/schemas/won_deals.json
--rw-r--r--   0 root         (0) root         (0)      478 2024-01-31 09:40:47.000000 airbyte-source-freshsales-1.0.0/source_freshsales/source.py
--rw-r--r--   0 root         (0) root         (0)      748 2024-01-31 09:40:47.000000 airbyte-source-freshsales-1.0.0/source_freshsales/spec.yaml
+-rw-r--r--   0        0        0     4567 2024-05-28 22:05:23.771201 airbyte_source_freshsales-1.0.1/README.md
+-rw-r--r--   0        0        0      138 2024-05-28 22:05:23.771201 airbyte_source_freshsales-1.0.1/main.py
+-rw-r--r--   0        0        0      779 2024-05-28 22:09:45.105685 airbyte_source_freshsales-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      132 2024-05-28 22:05:23.771201 airbyte_source_freshsales-1.0.1/source_freshsales/__init__.py
+-rw-r--r--   0        0        0    47946 2024-05-28 22:05:23.771201 airbyte_source_freshsales-1.0.1/source_freshsales/manifest.yaml
+-rw-r--r--   0        0        0      233 2024-05-28 22:05:23.771201 airbyte_source_freshsales-1.0.1/source_freshsales/run.py
+-rw-r--r--   0        0        0      479 2024-05-28 22:05:23.771201 airbyte_source_freshsales-1.0.1/source_freshsales/source.py
+-rw-r--r--   0        0        0     5281 1970-01-01 00:00:00.000000 airbyte_source_freshsales-1.0.1/PKG-INFO
```

### Comparing `airbyte-source-freshsales-1.0.0/PKG-INFO` & `airbyte_source_freshsales-1.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,99 +1,122 @@
 Metadata-Version: 2.1
 Name: airbyte-source-freshsales
-Version: 1.0.0
-Summary: Source implementation for Freshsales.
+Version: 1.0.1
+Summary: Source implementation for freshsales.
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
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/freshsales
+Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk~=0.1
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.2; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
 
 # Freshsales Source
 
-This is the repository for the Freshsales source connector, written in Python.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/freshsales).
+This is the repository for the Freshsales configuration based source connector.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/freshsales).
 
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
-pip install '.[tests]'
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
 
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/freshsales)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_freshsales/spec.json` file.
+### Create credentials
+
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/freshsales)
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `src/source_freshsales/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
+
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source freshsales test creds`
-and place them into `secrets/config.json`.
+### Locally running the connector
 
 ```
-python main.py spec
-python main.py check --config secrets/config.json
-python main.py discover --config secrets/config.json
-python main.py read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+poetry run source-freshsales spec
+poetry run source-freshsales check --config secrets/config.json
+poetry run source-freshsales discover --config secrets/config.json
+poetry run source-freshsales read --config secrets/config.json --catalog integration_tests/configured_catalog.json
 ```
 
+### Running tests
 
+To run tests locally, from the connector directory run:
 
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
-```bash
-airbyte-ci connectors --name=source-freshsales build
+```
+poetry run pytest tests
 ```
 
-An image will be built with the tag `airbyte/source-freshsales:dev`.
+### Building the docker image
 
-**Via `docker build`:**
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
-docker build -t airbyte/source-freshsales:dev .
+airbyte-ci connectors --name=source-freshsales build
 ```
 
+An image will be available on your host with the tag `airbyte/source-freshsales:dev`.
+
+
+### Running as a docker container
+
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-freshsales:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-freshsales:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-freshsales:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-freshsales:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-freshsales test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-freshsales test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/freshsales.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/freshsales.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-freshsales-1.0.0/README.md` & `airbyte_source_freshsales-1.0.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,99 +1,103 @@
 # Freshsales Source
 
-This is the repository for the Freshsales source connector, written in Python.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/freshsales).
+This is the repository for the Freshsales configuration based source connector.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/freshsales).
 
 ## Local development
 
 ### Prerequisites
-**To iterate on this connector, make sure to complete this prerequisites section.**
 
-#### Minimum Python version required `= 3.7.0`
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
-pip install '.[tests]'
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
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/freshsales)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_freshsales/spec.json` file.
+### Create credentials
+
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/freshsales)
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `src/source_freshsales/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source freshsales test creds`
-and place them into `secrets/config.json`.
 
 ### Locally running the connector
+
 ```
-python main.py spec
-python main.py check --config secrets/config.json
-python main.py discover --config secrets/config.json
-python main.py read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+poetry run source-freshsales spec
+poetry run source-freshsales check --config secrets/config.json
+poetry run source-freshsales discover --config secrets/config.json
+poetry run source-freshsales read --config secrets/config.json --catalog integration_tests/configured_catalog.json
 ```
 
-### Locally running the connector docker image
+### Running tests
 
+To run tests locally, from the connector directory run:
 
-#### Build
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
-```bash
-airbyte-ci connectors --name=source-freshsales build
+```
+poetry run pytest tests
 ```
 
-An image will be built with the tag `airbyte/source-freshsales:dev`.
+### Building the docker image
 
-**Via `docker build`:**
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
-docker build -t airbyte/source-freshsales:dev .
+airbyte-ci connectors --name=source-freshsales build
 ```
 
-#### Run
+An image will be available on your host with the tag `airbyte/source-freshsales:dev`.
+
+
+### Running as a docker container
+
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-freshsales:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-freshsales:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-freshsales:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-freshsales:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
-## Testing
+### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-freshsales test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-freshsales test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/freshsales.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/freshsales.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

