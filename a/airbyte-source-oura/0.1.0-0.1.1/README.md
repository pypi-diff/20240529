# Comparing `tmp/airbyte-source-oura-0.1.0.tar.gz` & `tmp/airbyte_source_oura-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-oura-0.1.0.tar", last modified: Wed Jan 31 15:52:14 2024, max compression
+gzip compressed data, was "airbyte_source_oura-0.1.1.tar", max compression
```

## Comparing `airbyte-source-oura-0.1.0.tar` & `airbyte_source_oura-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,8 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 15:52:14.955434 airbyte-source-oura-0.1.0/
--rw-r--r--   0 root         (0) root         (0)     4132 2024-01-31 15:52:14.955434 airbyte-source-oura-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3961 2024-01-31 15:33:11.000000 airbyte-source-oura-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 15:52:14.955434 airbyte-source-oura-0.1.0/airbyte_source_oura.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4132 2024-01-31 15:52:14.000000 airbyte-source-oura-0.1.0/airbyte_source_oura.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      976 2024-01-31 15:52:14.000000 airbyte-source-oura-0.1.0/airbyte_source_oura.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-31 15:52:14.000000 airbyte-source-oura-0.1.0/airbyte_source_oura.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2024-01-31 15:52:14.000000 airbyte-source-oura-0.1.0/airbyte_source_oura.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       78 2024-01-31 15:52:14.000000 airbyte-source-oura-0.1.0/airbyte_source_oura.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-01-31 15:52:14.000000 airbyte-source-oura-0.1.0/airbyte_source_oura.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 15:52:14.951434 airbyte-source-oura-0.1.0/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-31 15:33:11.000000 airbyte-source-oura-0.1.0/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)       77 2024-01-31 15:33:11.000000 airbyte-source-oura-0.1.0/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      314 2024-01-31 15:33:11.000000 airbyte-source-oura-0.1.0/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)     1583 2024-01-31 15:33:11.000000 airbyte-source-oura-0.1.0/integration_tests/catalog.json
--rw-r--r--   0 root         (0) root         (0)      474 2024-01-31 15:33:11.000000 airbyte-source-oura-0.1.0/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)      121 2024-01-31 15:33:11.000000 airbyte-source-oura-0.1.0/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)      118 2024-01-31 15:33:11.000000 airbyte-source-oura-0.1.0/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)       63 2024-01-31 15:33:11.000000 airbyte-source-oura-0.1.0/integration_tests/sample_state.json
--rw-r--r--   0 root         (0) root         (0)     3998 2024-01-31 15:52:14.955434 airbyte-source-oura-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      915 2024-01-31 15:52:12.000000 airbyte-source-oura-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 15:52:14.951434 airbyte-source-oura-0.1.0/source_oura/
--rw-r--r--   0 root         (0) root         (0)      120 2024-01-31 15:33:11.000000 airbyte-source-oura-0.1.0/source_oura/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3283 2024-01-31 15:33:11.000000 airbyte-source-oura-0.1.0/source_oura/manifest.yaml
--rw-r--r--   0 root         (0) root         (0)      224 2024-01-31 15:33:11.000000 airbyte-source-oura-0.1.0/source_oura/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 15:52:14.955434 airbyte-source-oura-0.1.0/source_oura/schemas/
--rw-r--r--   0 root         (0) root         (0)     2584 2024-01-31 15:33:11.000000 airbyte-source-oura-0.1.0/source_oura/schemas/daily_activity.json
--rw-r--r--   0 root         (0) root         (0)     1124 2024-01-31 15:33:11.000000 airbyte-source-oura-0.1.0/source_oura/schemas/daily_readiness.json
--rw-r--r--   0 root         (0) root         (0)      901 2024-01-31 15:33:11.000000 airbyte-source-oura-0.1.0/source_oura/schemas/daily_sleep.json
--rw-r--r--   0 root         (0) root         (0)      298 2024-01-31 15:33:11.000000 airbyte-source-oura-0.1.0/source_oura/schemas/heart_rate.json
--rw-r--r--   0 root         (0) root         (0)      873 2024-01-31 15:33:11.000000 airbyte-source-oura-0.1.0/source_oura/schemas/sessions.json
--rw-r--r--   0 root         (0) root         (0)     2360 2024-01-31 15:33:11.000000 airbyte-source-oura-0.1.0/source_oura/schemas/sleep_periods.json
--rw-r--r--   0 root         (0) root         (0)      424 2024-01-31 15:33:11.000000 airbyte-source-oura-0.1.0/source_oura/schemas/tags.json
--rw-r--r--   0 root         (0) root         (0)      668 2024-01-31 15:33:11.000000 airbyte-source-oura-0.1.0/source_oura/schemas/workouts.json
--rw-r--r--   0 root         (0) root         (0)      473 2024-01-31 15:33:11.000000 airbyte-source-oura-0.1.0/source_oura/source.py
--rw-r--r--   0 root         (0) root         (0)      959 2024-01-31 15:33:11.000000 airbyte-source-oura-0.1.0/source_oura/spec.yaml
+-rw-r--r--   0        0        0     4454 2024-05-28 22:26:32.000000 airbyte_source_oura-0.1.1/README.md
+-rw-r--r--   0        0        0      132 2024-05-28 22:26:32.000000 airbyte_source_oura-0.1.1/main.py
+-rw-r--r--   0        0        0      759 2024-05-28 23:57:38.960224 airbyte_source_oura-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      120 2024-05-28 22:26:32.000000 airbyte_source_oura-0.1.1/source_oura/__init__.py
+-rw-r--r--   0        0        0    22021 2024-05-28 22:26:32.000000 airbyte_source_oura-0.1.1/source_oura/manifest.yaml
+-rw-r--r--   0        0        0      221 2024-05-28 22:26:32.000000 airbyte_source_oura-0.1.1/source_oura/run.py
+-rw-r--r--   0        0        0      473 2024-05-28 22:26:32.000000 airbyte_source_oura-0.1.1/source_oura/source.py
+-rw-r--r--   0        0        0     5151 1970-01-01 00:00:00.000000 airbyte_source_oura-0.1.1/PKG-INFO
```

### Comparing `airbyte-source-oura-0.1.0/README.md` & `airbyte_source_oura-0.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,67 +1,103 @@
 # Oura Source
 
 This is the repository for the Oura configuration based source connector.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/oura).
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/oura).
 
 ## Local development
 
-#### Create credentials
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/oura)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_oura/spec.yaml` file.
-Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+### Prerequisites
+
+* Python (`^3.9`)
+* Poetry (`^1.7`) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source oura test creds`
-and place them into `secrets/config.json`.
 
-### Locally running the connector docker image
 
+### Installing the connector
 
-#### Build
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+From this connector directory, run:
 ```bash
-airbyte-ci connectors --name=source-oura build
+poetry install --with dev
 ```
 
-An image will be built with the tag `airbyte/source-oura:dev`.
 
-**Via `docker build`:**
+### Create credentials
+
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/oura)
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `src/source_oura/spec.yaml` file.
+Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
+See `sample_files/sample_config.json` for a sample config file.
+
+
+### Locally running the connector
+
+```
+poetry run source-oura spec
+poetry run source-oura check --config secrets/config.json
+poetry run source-oura discover --config secrets/config.json
+poetry run source-oura read --config secrets/config.json --catalog sample_files/configured_catalog.json
+```
+
+### Running tests
+
+To run tests locally, from the connector directory run:
+
+```
+poetry run pytest tests
+```
+
+### Building the docker image
+
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
-docker build -t airbyte/source-oura:dev .
+airbyte-ci connectors --name=source-oura build
 ```
 
-#### Run
+An image will be available on your host with the tag `airbyte/source-oura:dev`.
+
+
+### Running as a docker container
+
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-oura:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-oura:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-oura:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-oura:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
-## Testing
+### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-oura test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-oura test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/oura.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/oura.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

