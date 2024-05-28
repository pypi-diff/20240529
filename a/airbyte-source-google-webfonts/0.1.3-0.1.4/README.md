# Comparing `tmp/airbyte_source_google_webfonts-0.1.3.tar.gz` & `tmp/airbyte_source_google_webfonts-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_google_webfonts-0.1.3.tar", max compression
+gzip compressed data, was "airbyte_source_google_webfonts-0.1.4.tar", max compression
```

## Comparing `airbyte_source_google_webfonts-0.1.3.tar` & `airbyte_source_google_webfonts-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     4658 2024-05-01 18:48:12.547733 airbyte_source_google_webfonts-0.1.3/README.md
--rw-r--r--   0        0        0      797 2024-05-01 18:51:38.326741 airbyte_source_google_webfonts-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      140 2024-05-01 18:48:12.547733 airbyte_source_google_webfonts-0.1.3/source_google_webfonts/__init__.py
--rw-r--r--   0        0        0     4930 2024-05-01 18:48:12.547733 airbyte_source_google_webfonts-0.1.3/source_google_webfonts/manifest.yaml
--rw-r--r--   0        0        0      255 2024-05-01 18:48:12.547733 airbyte_source_google_webfonts-0.1.3/source_google_webfonts/run.py
--rw-r--r--   0        0        0      483 2024-05-01 18:48:12.547733 airbyte_source_google_webfonts-0.1.3/source_google_webfonts/source.py
--rw-r--r--   0        0        0      714 2024-05-01 18:48:12.547733 airbyte_source_google_webfonts-0.1.3/source_google_webfonts/spec.yaml
--rw-r--r--   0        0        0     5389 1970-01-01 00:00:00.000000 airbyte_source_google_webfonts-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     4668 2024-05-28 20:38:20.000000 airbyte_source_google_webfonts-0.1.4/README.md
+-rw-r--r--   0        0        0      797 2024-05-28 22:05:35.996772 airbyte_source_google_webfonts-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      140 2024-05-28 20:38:20.000000 airbyte_source_google_webfonts-0.1.4/source_google_webfonts/__init__.py
+-rw-r--r--   0        0        0     5251 2024-05-28 20:38:20.000000 airbyte_source_google_webfonts-0.1.4/source_google_webfonts/manifest.yaml
+-rw-r--r--   0        0        0      241 2024-05-28 20:38:20.000000 airbyte_source_google_webfonts-0.1.4/source_google_webfonts/run.py
+-rw-r--r--   0        0        0      483 2024-05-28 20:38:20.000000 airbyte_source_google_webfonts-0.1.4/source_google_webfonts/source.py
+-rw-r--r--   0        0        0     5399 1970-01-01 00:00:00.000000 airbyte_source_google_webfonts-0.1.4/PKG-INFO
```

### Comparing `airbyte_source_google_webfonts-0.1.3/README.md` & `airbyte_source_google_webfonts-0.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,91 +1,104 @@
 # Google-Webfonts source connector
 
-
 This is the repository for the Google-Webfonts source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/google-webfonts).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/google-webfonts)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_google_webfonts/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-google-webfonts spec
 poetry run source-google-webfonts check --config secrets/config.json
 poetry run source-google-webfonts discover --config secrets/config.json
 poetry run source-google-webfonts read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-google-webfonts build
 ```
 
 An image will be available on your host with the tag `airbyte/source-google-webfonts:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-google-webfonts:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-google-webfonts:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-google-webfonts:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-google-webfonts:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-google-webfonts test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-google-webfonts test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/google-webfonts.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_google_webfonts-0.1.3/pyproject.toml` & `airbyte_source_google_webfonts-0.1.4/pyproject.toml`

 * *Files 18% similar despite different names*

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
 name = "airbyte-source-google-webfonts"
 description = "Source implementation for Google Webfonts."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_google_webfonts-0.1.3/source_google_webfonts/manifest.yaml` & `airbyte_source_google_webfonts-0.1.4/source_google_webfonts/manifest.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,148 +1,176 @@
-version: "0.29.0"
+version: 0.78.1
+
+type: DeclarativeSource
+
+check:
+  type: CheckStream
+  stream_names:
+    - fonts
 
 definitions:
-  selector:
-    extractor:
-      field_path: ["items"]
-  requester:
-    url_base: "https://webfonts.googleapis.com/v1"
-    http_method: "GET"
+  streams:
+    fonts:
+      type: DeclarativeStream
+      name: fonts
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: >-
+            /webfonts?key={{ config['api_key'] }}&sort={{ config['sort'] or
+            'SORT_UNDEFINED'}}&prettyPrint={{ config['prettyPrint'] or 
+            'true'}}&alt={{ config['alt'] or 'json'}}
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path:
+              - items
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/fonts"
+  base_requester:
+    type: HttpRequester
+    url_base: https://webfonts.googleapis.com/v1
     authenticator:
       type: ApiKeyAuthenticator
-      header: "apikey"
       api_token: "{{ config['api_key'] }}"
+      inject_into:
+        type: RequestOption
+        inject_into: header
+        field_name: apikey
 
-  retriever:
-    record_selector:
-      $ref: "#/definitions/selector"
-    paginator:
-      type: NoPagination
-    requester:
-      $ref: "#/definitions/requester"
-
-  base_stream:
-    retriever:
-      $ref: "#/definitions/retriever"
-
-  fonts_stream:
-    $ref: "#/definitions/base_stream"
-    $parameters:
-      name: "fonts"
-      path:
-        "/webfonts?key={{ config['api_key'] }}&sort={{ config['sort'] or 'SORT_UNDEFINED'}}&prettyPrint={{
-        config['prettyPrint'] or 'true'}}&alt={{ config['alt'] or 'json'}}"
-
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        definitions: {}
-        $schema: http://json-schema.org/draft-07/schema#
-        $id: https://example.com/object1666796406.json
-        title: Root
-        type: object
-        properties:
-          kind:
-            description: The API resource kind, always set to 'webfonts#webfontList'
-            $id: "#root/kind"
-            title: Kind
-            type: string
-            default: ""
-            pattern: ^.*$
-          items:
-            description: List of fonts available in the API
-            $id: "#root/items"
-            title: Items
-            type: array
-            default: []
-            items:
-              $id: "#root/items/items"
-              title: Items
+streams:
+  - $ref: "#/definitions/streams/fonts"
+
+spec:
+  type: Spec
+  connection_specification:
+    type: object
+    $schema: http://json-schema.org/draft-07/schema#
+    required:
+      - api_key
+    properties:
+      api_key:
+        type: string
+        title: API Key
+        airbyte_secret: true
+        description: >-
+          API key is required to access google apis, For getting your's goto
+          google console and generate api key for Webfonts
+        order: 0
+      alt:
+        type: string
+        description: Optional, Available params- json, media, proto
+        order: 1
+      prettyPrint:
+        type: string
+        description: Optional, boolean type
+        order: 2
+      sort:
+        type: string
+        description: Optional, to find how to sort
+        order: 3
+    additionalProperties: true
+
+metadata:
+  autoImportSchema:
+    fonts: false
+
+schemas:
+  fonts:
+    type: object
+    $id: https://example.com/object1666796406.json
+    $schema: http://json-schema.org/draft-07/schema#
+    additionalProperties: true
+    properties:
+      items:
+        type: array
+        $id: "#root/items"
+        default: []
+        description: List of fonts available in the API
+        items:
+          type: object
+          $id: "#root/items/items"
+          properties:
+            version:
+              type: string
+              $id: "#root/items/items/version"
+              description: Version of the font data
+              pattern: ^.*$
+              title: Version
+            category:
+              type: string
+              $id: "#root/items/items/category"
+              description: The category the font belongs to (e.g. 'sans-serif', 'serif')
+              pattern: ^.*$
+              title: Category
+            family:
+              type: string
+              $id: "#root/items/items/family"
+              description: The name of the font family (e.g. 'Roboto', 'Open Sans')
+              pattern: ^.*$
+              title: Family
+            files:
               type: object
+              $id: "#root/items/items/files"
+              description: Different file variants available for the font
               properties:
-                family:
-                  description: The name of the font family (e.g. 'Roboto', 'Open Sans')
-                  $id: "#root/items/items/family"
-                  title: Family
-                  type: string
-                  default: ""
-                  pattern: ^.*$
-                variants:
-                  description: Different styles and weights available for the font
-                  $id: "#root/items/items/variants"
-                  title: Variants
-                  type: array
-                  default: []
-                  items:
-                    $id: "#root/items/items/variants/items"
-                    title: Items
-                    type: string
-                    default: ""
-                    pattern: ^.*$
-                subsets:
-                  description: List of language subsets supported by the font
-                  $id: "#root/items/items/subsets"
-                  title: Subsets
-                  type: array
-                  default: []
-                  items:
-                    $id: "#root/items/items/subsets/items"
-                    title: Items
-                    type: string
-                    default: ""
-                    pattern: ^.*$
-                version:
-                  description: Version of the font data
-                  $id: "#root/items/items/version"
-                  title: Version
+                italic:
                   type: string
-                  default: ""
+                  $id: "#root/items/items/files/italic"
+                  description: URL to the italic font file
                   pattern: ^.*$
-                lastModified:
-                  description: Timestamp of the last modification date of the font
-                  $id: "#root/items/items/lastModified"
-                  title: Lastmodified
+                  title: Italic
+                regular:
                   type: string
-                  default: ""
+                  $id: "#root/items/items/files/regular"
+                  description: URL to the regular font file
                   pattern: ^.*$
-                files:
-                  description: Different file variants available for the font
-                  $id: "#root/items/items/files"
-                  title: Files
-                  type: object
-                  properties:
-                    regular:
-                      description: URL to the regular font file
-                      $id: "#root/items/items/files/regular"
-                      title: Regular
-                      type: string
-                      default: ""
-                      pattern: ^.*$
-                    italic:
-                      description: URL to the italic font file
-                      $id: "#root/items/items/files/italic"
-                      title: Italic
-                      type: string
-                      default: ""
-                      pattern: ^.*$
-                category:
-                  description:
-                    The category the font belongs to (e.g. 'sans-serif',
-                    'serif')
-                  $id: "#root/items/items/category"
-                  title: Category
-                  type: string
-                  default: ""
-                  pattern: ^.*$
-                kind:
-                  description: The resource kind, should always be 'webfonts#webfont'
-                  $id: "#root/items/items/kind"
-                  title: Kind
-                  type: string
-                  default: ""
-                  pattern: ^.*$
-streams:
-  - "#/definitions/fonts_stream"
-
-check:
-  stream_names:
-    - "fonts"
+                  title: Regular
+              title: Files
+            kind:
+              type: string
+              $id: "#root/items/items/kind"
+              description: The resource kind, should always be 'webfonts#webfont'
+              pattern: ^.*$
+              title: Kind
+            lastModified:
+              type: string
+              $id: "#root/items/items/lastModified"
+              description: Timestamp of the last modification date of the font
+              pattern: ^.*$
+              title: Lastmodified
+            subsets:
+              type: array
+              $id: "#root/items/items/subsets"
+              default: []
+              description: List of language subsets supported by the font
+              items:
+                type: string
+                $id: "#root/items/items/subsets/items"
+                pattern: ^.*$
+                title: Items
+              title: Subsets
+            variants:
+              type: array
+              $id: "#root/items/items/variants"
+              default: []
+              description: Different styles and weights available for the font
+              items:
+                type: string
+                $id: "#root/items/items/variants/items"
+                pattern: ^.*$
+                title: Items
+              title: Variants
+          title: Items
+        title: Items
+      kind:
+        type: string
+        $id: "#root/kind"
+        description: The API resource kind, always set to 'webfonts#webfontList'
+        pattern: ^.*$
+        title: Kind
+    title: Root
```

### Comparing `airbyte_source_google_webfonts-0.1.3/PKG-INFO` & `airbyte_source_google_webfonts-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-google-webfonts
-Version: 0.1.3
+Version: 0.1.4
 Summary: Source implementation for Google Webfonts.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -15,96 +15,110 @@
 Requires-Dist: airbyte-cdk (==0.80.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/google-webfonts
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Google-Webfonts source connector
 
-
 This is the repository for the Google-Webfonts source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/google-webfonts).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/google-webfonts)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_google_webfonts/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-google-webfonts spec
 poetry run source-google-webfonts check --config secrets/config.json
 poetry run source-google-webfonts discover --config secrets/config.json
 poetry run source-google-webfonts read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-google-webfonts build
 ```
 
 An image will be available on your host with the tag `airbyte/source-google-webfonts:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-google-webfonts:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-google-webfonts:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-google-webfonts:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-google-webfonts:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-google-webfonts test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-google-webfonts test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/google-webfonts.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+
```

