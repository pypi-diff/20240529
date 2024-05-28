# Comparing `tmp/airbyte_source_orbit-0.3.4.tar.gz` & `tmp/airbyte_source_orbit-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_orbit-0.3.4.tar", max compression
+gzip compressed data, was "airbyte_source_orbit-0.3.5.tar", max compression
```

## Comparing `airbyte_source_orbit-0.3.4.tar` & `airbyte_source_orbit-0.3.5.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     4478 2024-05-01 19:03:43.977019 airbyte_source_orbit-0.3.4/README.md
--rw-r--r--   0        0        0      737 2024-05-01 19:07:10.870770 airbyte_source_orbit-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      122 2024-05-01 19:03:43.977019 airbyte_source_orbit-0.3.4/source_orbit/__init__.py
--rw-r--r--   0        0        0    13428 2024-05-01 19:03:43.977019 airbyte_source_orbit-0.3.4/source_orbit/manifest.yaml
--rw-r--r--   0        0        0      227 2024-05-01 19:03:43.977019 airbyte_source_orbit-0.3.4/source_orbit/run.py
--rw-r--r--   0        0        0      474 2024-05-01 19:03:43.977019 airbyte_source_orbit-0.3.4/source_orbit/source.py
--rw-r--r--   0        0        0      880 2024-05-01 19:03:43.977019 airbyte_source_orbit-0.3.4/source_orbit/spec.yaml
--rw-r--r--   0        0        0     5179 1970-01-01 00:00:00.000000 airbyte_source_orbit-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     4488 2024-05-28 22:16:25.000000 airbyte_source_orbit-0.3.5/README.md
+-rw-r--r--   0        0        0      737 2024-05-28 23:56:01.034308 airbyte_source_orbit-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      122 2024-05-28 22:16:25.000000 airbyte_source_orbit-0.3.5/source_orbit/__init__.py
+-rw-r--r--   0        0        0    13386 2024-05-28 22:16:25.000000 airbyte_source_orbit-0.3.5/source_orbit/manifest.yaml
+-rw-r--r--   0        0        0      227 2024-05-28 22:16:25.000000 airbyte_source_orbit-0.3.5/source_orbit/run.py
+-rw-r--r--   0        0        0      474 2024-05-28 22:16:25.000000 airbyte_source_orbit-0.3.5/source_orbit/source.py
+-rw-r--r--   0        0        0     5189 1970-01-01 00:00:00.000000 airbyte_source_orbit-0.3.5/PKG-INFO
```

### Comparing `airbyte_source_orbit-0.3.4/README.md` & `airbyte_source_orbit-0.3.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,91 +1,104 @@
 # Orbit source connector
 
-
 This is the repository for the Orbit source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/orbit).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/orbit)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_orbit/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-orbit spec
 poetry run source-orbit check --config secrets/config.json
 poetry run source-orbit discover --config secrets/config.json
 poetry run source-orbit read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-orbit build
 ```
 
 An image will be available on your host with the tag `airbyte/source-orbit:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-orbit:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-orbit:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-orbit:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-orbit:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-orbit test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-orbit test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/orbit.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_orbit-0.3.4/pyproject.toml` & `airbyte_source_orbit-0.3.5/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.3.4"
+version = "0.3.5"
 name = "airbyte-source-orbit"
 description = "Source implementation for Orbit."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_orbit-0.3.4/source_orbit/manifest.yaml` & `airbyte_source_orbit-0.3.5/source_orbit/manifest.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,424 +1,473 @@
-version: "0.52.0"
+version: 0.79.1
+
+type: DeclarativeSource
+
+check:
+  type: CheckStream
+  stream_names:
+    - workspace
 
 definitions:
-  selector:
-    type: RecordSelector
-    extractor:
-      type: DpathExtractor
-      field_path: ["data"]
-  requester:
+  streams:
+    workspace:
+      type: DeclarativeStream
+      name: workspace
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: workspaces/{{config['workspace']}}
+          http_method: GET
+          request_parameters:
+            start_date: "{{ config.get('start_date') }}"
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path:
+              - data
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/workspace"
+    members:
+      type: DeclarativeStream
+      name: members
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: "{{config['workspace']}}/members"
+          http_method: GET
+          request_parameters:
+            start_date: "{{ config.get('start_date') }}"
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path:
+              - data
+        paginator:
+          type: DefaultPaginator
+          page_token_option:
+            type: RequestOption
+            inject_into: request_parameter
+            field_name: page
+          page_size_option:
+            type: RequestOption
+            inject_into: request_parameter
+            field_name: items
+          pagination_strategy:
+            type: PageIncrement
+            start_from_page: 1
+            page_size: 100
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/members"
+  base_requester:
     type: HttpRequester
-    url_base: "https://app.orbit.love/api/v1/"
-    http_method: "GET"
+    url_base: https://app.orbit.love/api/v1/
     authenticator:
       type: BearerAuthenticator
       api_token: "{{ config['api_token'] }}"
-    request_parameters:
-      start_date: "{{ config.get('start_date') }}"
-  retriever:
-    type: SimpleRetriever
-    record_selector:
-      $ref: "#/definitions/selector"
-    paginator:
-      type: NoPagination
-    requester:
-      $ref: "#/definitions/requester"
 
-  base_stream:
-    type: DeclarativeStream
-    retriever:
-      $ref: "#/definitions/retriever"
+streams:
+  - $ref: "#/definitions/streams/workspace"
+  - $ref: "#/definitions/streams/members"
+
+spec:
+  type: Spec
+  connection_specification:
+    type: object
+    $schema: http://json-schema.org/draft-07/schema#
+    required:
+      - api_token
+      - workspace
+    properties:
+      api_token:
+        type: string
+        airbyte_secret: true
+        title: API Token
+        description: >-
+          Authorizes you to work with Orbit workspaces associated with the
+          token.
+        order: 0
+      workspace:
+        type: string
+        title: Workspace
+        description: >-
+          The unique name of the workspace that your API token is associated
+          with.
+        order: 1
+      start_date:
+        type: string
+        title: Start Date
+        description: >-
+          Date in the format 2022-06-26. Only load members whose last activities
+          are after this date.
+        pattern: ^[0-9]{4}-[0-9]{2}-[0-9]{2}$
+        order: 2
+    additionalProperties: true
 
-  workspace_stream:
-    $ref: "#/definitions/base_stream"
-    name: "workspace"
-    primary_key: "id"
-    $parameters:
-      path: "workspaces/{{config['workspace']}}"
+metadata:
+  autoImportSchema:
+    workspace: false
+    members: false
 
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/draft-07/schema#
-        type: object
+schemas:
+  workspace:
+    type: object
+    $schema: http://json-schema.org/draft-07/schema#
+    additionalProperties: true
+    properties:
+      type:
+        type:
+          - "null"
+          - string
+        description: The type of entity, in this case, it's 'workspace'
+      attributes:
+        type:
+          - "null"
+          - object
         additionalProperties: true
+        description: Attributes related to the workspace
         properties:
-          id:
-            description: The unique identifier for the workspace
+          activities_count:
+            type:
+              - "null"
+              - integer
+            description: The total number of activities in the workspace
+          created_at:
+            type:
+              - "null"
+              - string
+            description: Date and time when the workspace was created
+          members_count:
+            type:
+              - "null"
+              - integer
+            description: The total number of members in the workspace
+          name:
             type:
               - "null"
               - string
-          type:
-            description: The type of entity, in this case, it's 'workspace'
+            description: The name of the workspace
+          slug:
             type:
               - "null"
               - string
-          relationships:
-            description: Relationships of the workspace with other entities
-            type: object
+            description: A unique identifier for the workspace
+          tags:
+            type:
+              - "null"
+              - object
+            additionalProperties: true
+            description: Tags associated with the workspace
+            properties: {}
+          updated_at:
+            type:
+              - "null"
+              - string
+            description: Date and time when the workspace was last updated
+      id:
+        type:
+          - "null"
+          - string
+        description: The unique identifier for the workspace
+      relationships:
+        type: object
+        description: Relationships of the workspace with other entities
+        properties:
+          last_activity:
+            type:
+              - "null"
+              - object
+            description: Information about the last activity in the workspace
             properties:
-              last_member:
-                description: Information about the last member who joined the workspace
-                type:
-                  - "null"
-                  - object
-                properties:
-                  data:
-                    description: Details of the last member
-                    type:
-                      - "null"
-                      - object
-              last_activity:
-                description: Information about the last activity in the workspace
+              data:
                 type:
                   - "null"
                   - object
-                properties:
-                  data:
-                    description: Details of the last activity
-                    type:
-                      - "null"
-                      - object
-              repositories:
-                description: List of repositories associated with the workspace
+                description: Details of the last activity
+          last_member:
+            type:
+              - "null"
+              - object
+            description: Information about the last member who joined the workspace
+            properties:
+              data:
                 type:
                   - "null"
                   - object
-                properties:
-                  data:
-                    description: Details of the repositories
-                    type:
-                      - "null"
-                      - array
-          attributes:
-            description: Attributes related to the workspace
+                description: Details of the last member
+          repositories:
             type:
               - "null"
               - object
-            additionalProperties: true
+            description: List of repositories associated with the workspace
             properties:
-              name:
-                description: The name of the workspace
-                type:
-                  - "null"
-                  - string
-              slug:
-                description: A unique identifier for the workspace
-                type:
-                  - "null"
-                  - string
-              updated_at:
-                description: Date and time when the workspace was last updated
-                type:
-                  - "null"
-                  - string
-              created_at:
-                description: Date and time when the workspace was created
-                type:
-                  - "null"
-                  - string
-              members_count:
-                description: The total number of members in the workspace
-                type:
-                  - "null"
-                  - integer
-              activities_count:
-                description: The total number of activities in the workspace
+              data:
                 type:
                   - "null"
-                  - integer
-              tags:
-                description: Tags associated with the workspace
-                type:
-                  - "null"
-                  - object
-                additionalProperties: true
-                properties: {}
-  members_stream:
-    $ref: "#/definitions/base_stream"
-    name: "members"
-    primary_key: "id"
-    $parameters:
-      path: "{{config['workspace']}}/members"
-    retriever:
-      $ref: "#/definitions/retriever"
-      paginator:
-        type: "DefaultPaginator"
-        pagination_strategy:
-          type: PageIncrement
-          start_from_page: 1
-          page_size: 100
-        page_token_option:
-          type: RequestOption
-          inject_into: request_parameter
-          field_name: page
-        page_size_option:
-          inject_into: request_parameter
-          field_name: items
-          type: RequestOption
-
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/draft-07/schema#
-        type: object
+                  - array
+                description: Details of the repositories
+  members:
+    type: object
+    $schema: http://json-schema.org/draft-07/schema#
+    additionalProperties: true
+    properties:
+      type:
+        type:
+          - "null"
+          - string
+        description: Type of entity, in this case, the member
+      attributes:
+        type:
+          - "null"
+          - object
         additionalProperties: true
+        description: Contains the main attributes data of the member
         properties:
+          activities_count:
+            type:
+              - "null"
+              - integer
+            description: Total number of activities performed by the member
+          activities_score:
+            type:
+              - "null"
+              - number
+            description: Score calculated based on the member's activities
+          avatar_url:
+            type:
+              - "null"
+              - string
+            description: URL of the member's avatar image
+          bio:
+            type:
+              - "null"
+              - string
+            description: Member's biography or description
+          birthday:
+            type:
+              - "null"
+              - string
+            description: Date of birth of the member
+          company:
+            type:
+              - "null"
+              - string
+            description: Name of the company the member is associated with
+          created:
+            type:
+              - "null"
+              - boolean
+            description: Creation timestamp of the member
+          created_at:
+            type:
+              - "null"
+              - string
+            description: Timestamp when the member was created
+          deleted_at:
+            type:
+              - "null"
+              - string
+            description: Timestamp when the member was deleted, if applicable
+          devto:
+            type:
+              - "null"
+              - string
+            description: DEV.TO profile link of the member
+          discord:
+            type:
+              - "null"
+              - string
+            description: Discord profile link of the member
+          discourse:
+            type:
+              - "null"
+              - string
+            description: Discourse profile link of the member
+          email:
+            type:
+              - "null"
+              - string
+            description: Email address of the member
+          first_activity_occurred_at:
+            type:
+              - "null"
+              - string
+            description: Timestamp of the first activity performed by the member
+          github:
+            type:
+              - "null"
+              - string
+            description: GitHub profile link of the member
+          github_followers:
+            type:
+              - "null"
+              - integer
+            description: Number of followers on GitHub
           id:
+            type:
+              - "null"
+              - string
             description: Unique identifier for the member
+          languages:
+            type:
+              - "null"
+              - array
+            description: List of programming languages known by the member
+            items:
+              type:
+                - "null"
+                - string
+          last_activity_occurred_at:
             type:
               - "null"
               - string
-          fake:
-            description: Indicates if the member data is fake or real
+            description: Timestamp of the last activity performed by the member
+          linkedin:
             type:
               - "null"
               - string
-          type:
-            description: Type of entity, in this case, the member
+            description: LinkedIn profile link of the member
+          location:
             type:
               - "null"
               - string
-          attributes:
-            description: Contains the main attributes data of the member
+            description: Current location of the member
+          love:
             type:
               - "null"
-              - object
-            additionalProperties: true
-            properties:
-              activities_count:
-                description: Total number of activities performed by the member
-                type:
-                  - "null"
-                  - integer
-              activities_score:
-                description: Score calculated based on the member's activities
-                type:
-                  - "null"
-                  - number
-              avatar_url:
-                description: URL of the member's avatar image
-                type:
-                  - "null"
-                  - string
-              bio:
-                description: Member's biography or description
-                type:
-                  - "null"
-                  - string
-              birthday:
-                description: Date of birth of the member
-                type:
-                  - "null"
-                  - string
-              company:
-                description: Name of the company the member is associated with
-                type:
-                  - "null"
-                  - string
-              title:
-                description: Job title or role of the member
-                type:
-                  - "null"
-                  - string
-              created_at:
-                description: Timestamp when the member was created
-                type:
-                  - "null"
-                  - string
-              deleted_at:
-                description: Timestamp when the member was deleted, if applicable
-                type:
-                  - "null"
-                  - string
-              first_activity_occurred_at:
-                description: Timestamp of the first activity performed by the member
-                type:
-                  - "null"
-                  - string
-              last_activity_occurred_at:
-                description: Timestamp of the last activity performed by the member
-                type:
-                  - "null"
-                  - string
-              location:
-                description: Current location of the member
-                type:
-                  - "null"
-                  - string
-              name:
-                description: Full name of the member
-                type:
-                  - "null"
-                  - string
-              pronouns:
-                description: Preferred pronouns of the member
-                type:
-                  - "null"
-                  - string
-              reach:
-                description: Extent of influence or reach the member has
-                type:
-                  - "null"
-                  - integer
-              shipping_address:
-                description: Shipping address details of the member
-                type:
-                  - "null"
-                  - string
-              slug:
-                description: Unique string used in URLs to identify the member
-                type:
-                  - "null"
-                  - string
-              source:
-                description: Source or platform from which the member originated
-                type:
-                  - "null"
-                  - string
-              tag_list:
-                description: List of tags associated with the member
-                type:
-                  - "null"
-                  - array
-                items:
-                  type:
-                    - "null"
-                    - string
-              tags:
-                description: Additional tags associated with the member for categorization
-                type:
-                  - "null"
-                  - array
-                items:
-                  type:
-                    - "null"
-                    - string
-              teammate:
-                description: Indicates if the member is a teammate within an organization
-                type: boolean
-              tshirt:
-                description: T-shirt size preference of the member
-                type:
-                  - "null"
-                  - string
-              updated_at:
-                description: Timestamp of the last update to the member profile
-                type:
-                  - "null"
-                  - string
-              merged_at:
-                description: Timestamp when the member's data was merged
-                type:
-                  - "null"
-                  - string
-              url:
-                description: URL of the member profile
-                type:
-                  - "null"
-                  - string
-              orbit_url:
-                description: URL to access the member's Orbit profile
-                type:
-                  - "null"
-                  - string
-              created:
-                description: Creation timestamp of the member
-                type:
-                  - "null"
-                  - boolean
-              id:
-                description: Unique identifier for the member
-                type:
-                  - "null"
-                  - string
-              orbit_level:
-                description: Level of engagement with Orbit platform
-                type:
-                  - "null"
-                  - integer
-              love:
-                description:
-                  Measure of appreciation or positive feedback received
-                  by the member
-                type:
-                  - "null"
-                  - string
-              twitter:
-                description: Twitter profile link of the member
-                type:
-                  - "null"
-                  - string
-              github:
-                description: GitHub profile link of the member
-                type:
-                  - "null"
-                  - string
-              discourse:
-                description: Discourse profile link of the member
-                type:
-                  - "null"
-                  - string
-              email:
-                description: Email address of the member
-                type:
-                  - "null"
-                  - string
-              devto:
-                description: DEV.TO profile link of the member
-                type:
-                  - "null"
-                  - string
-              linkedin:
-                description: LinkedIn profile link of the member
-                type:
-                  - "null"
-                  - string
-              discord:
-                description: Discord profile link of the member
-                type:
-                  - "null"
-                  - string
-              github_followers:
-                description: Number of followers on GitHub
-                type:
-                  - "null"
-                  - integer
-              twitter_followers:
-                description: Number of followers on Twitter
-                type:
-                  - "null"
-                  - integer
-              topics:
-                description: List of topics of interest to the member
-                type:
-                  - "null"
-                  - array
-                items:
-                  type:
-                    - "null"
-                    - string
-              languages:
-                description: List of programming languages known by the member
-                type:
-                  - "null"
-                  - array
-                items:
-                  type:
-                    - "null"
-                    - string
-          relationships:
-            description: Contains the relationship data of the member
+              - string
+            description: >-
+              Measure of appreciation or positive feedback received by the
+              member
+          merged_at:
             type:
               - "null"
-              - object
-            additionalProperties: true
-            properties: {}
-streams:
-  - "#/definitions/workspace_stream"
-  - "#/definitions/members_stream"
-
-check:
-  type: CheckStream
-  stream_names:
-    - "workspace"
+              - string
+            description: Timestamp when the member's data was merged
+          name:
+            type:
+              - "null"
+              - string
+            description: Full name of the member
+          orbit_level:
+            type:
+              - "null"
+              - integer
+            description: Level of engagement with Orbit platform
+          orbit_url:
+            type:
+              - "null"
+              - string
+            description: URL to access the member's Orbit profile
+          pronouns:
+            type:
+              - "null"
+              - string
+            description: Preferred pronouns of the member
+          reach:
+            type:
+              - "null"
+              - integer
+            description: Extent of influence or reach the member has
+          shipping_address:
+            type:
+              - "null"
+              - string
+            description: Shipping address details of the member
+          slug:
+            type:
+              - "null"
+              - string
+            description: Unique string used in URLs to identify the member
+          source:
+            type:
+              - "null"
+              - string
+            description: Source or platform from which the member originated
+          tag_list:
+            type:
+              - "null"
+              - array
+            description: List of tags associated with the member
+            items:
+              type:
+                - "null"
+                - string
+          tags:
+            type:
+              - "null"
+              - array
+            description: Additional tags associated with the member for categorization
+            items:
+              type:
+                - "null"
+                - string
+          teammate:
+            type: boolean
+            description: Indicates if the member is a teammate within an organization
+          title:
+            type:
+              - "null"
+              - string
+            description: Job title or role of the member
+          topics:
+            type:
+              - "null"
+              - array
+            description: List of topics of interest to the member
+            items:
+              type:
+                - "null"
+                - string
+          tshirt:
+            type:
+              - "null"
+              - string
+            description: T-shirt size preference of the member
+          twitter:
+            type:
+              - "null"
+              - string
+            description: Twitter profile link of the member
+          twitter_followers:
+            type:
+              - "null"
+              - integer
+            description: Number of followers on Twitter
+          updated_at:
+            type:
+              - "null"
+              - string
+            description: Timestamp of the last update to the member profile
+          url:
+            type:
+              - "null"
+              - string
+            description: URL of the member profile
+      fake:
+        type:
+          - "null"
+          - string
+        description: Indicates if the member data is fake or real
+      id:
+        type:
+          - "null"
+          - string
+        description: Unique identifier for the member
+      relationships:
+        type:
+          - "null"
+          - object
+        additionalProperties: true
+        description: Contains the relationship data of the member
+        properties: {}
```

### Comparing `airbyte_source_orbit-0.3.4/PKG-INFO` & `airbyte_source_orbit-0.3.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-orbit
-Version: 0.3.4
+Version: 0.3.5
 Summary: Source implementation for Orbit.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -15,96 +15,110 @@
 Requires-Dist: airbyte-cdk (==0.80.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/orbit
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Orbit source connector
 
-
 This is the repository for the Orbit source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/orbit).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/orbit)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_orbit/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-orbit spec
 poetry run source-orbit check --config secrets/config.json
 poetry run source-orbit discover --config secrets/config.json
 poetry run source-orbit read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-orbit build
 ```
 
 An image will be available on your host with the tag `airbyte/source-orbit:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-orbit:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-orbit:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-orbit:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-orbit:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-orbit test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-orbit test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/orbit.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+
```

