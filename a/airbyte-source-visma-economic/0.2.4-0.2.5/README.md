# Comparing `tmp/airbyte_source_visma_economic-0.2.4.tar.gz` & `tmp/airbyte_source_visma_economic-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_visma_economic-0.2.4.tar", max compression
+gzip compressed data, was "airbyte_source_visma_economic-0.2.5.tar", max compression
```

## Comparing `airbyte_source_visma_economic-0.2.4.tar` & `airbyte_source_visma_economic-0.2.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     4640 2024-05-01 18:27:50.017178 airbyte_source_visma_economic-0.2.4/README.md
--rw-r--r--   0        0        0      791 2024-05-01 18:31:25.093283 airbyte_source_visma_economic-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      138 2024-05-01 18:27:50.017178 airbyte_source_visma_economic-0.2.4/source_visma_economic/__init__.py
--rw-r--r--   0        0        0   101196 2024-05-01 18:27:50.017178 airbyte_source_visma_economic-0.2.4/source_visma_economic/manifest.yaml
--rw-r--r--   0        0        0      252 2024-05-01 18:27:50.017178 airbyte_source_visma_economic-0.2.4/source_visma_economic/run.py
--rw-r--r--   0        0        0      482 2024-05-01 18:27:50.017178 airbyte_source_visma_economic-0.2.4/source_visma_economic/source.py
--rw-r--r--   0        0        0     5368 1970-01-01 00:00:00.000000 airbyte_source_visma_economic-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     4650 2024-05-28 22:21:19.000000 airbyte_source_visma_economic-0.2.5/README.md
+-rw-r--r--   0        0        0      791 2024-05-28 23:57:29.396563 airbyte_source_visma_economic-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      138 2024-05-28 22:21:19.000000 airbyte_source_visma_economic-0.2.5/source_visma_economic/__init__.py
+-rw-r--r--   0        0        0    94958 2024-05-28 22:21:19.000000 airbyte_source_visma_economic-0.2.5/source_visma_economic/manifest.yaml
+-rw-r--r--   0        0        0      252 2024-05-28 22:21:19.000000 airbyte_source_visma_economic-0.2.5/source_visma_economic/run.py
+-rw-r--r--   0        0        0      482 2024-05-28 22:21:19.000000 airbyte_source_visma_economic-0.2.5/source_visma_economic/source.py
+-rw-r--r--   0        0        0     5378 1970-01-01 00:00:00.000000 airbyte_source_visma_economic-0.2.5/PKG-INFO
```

### Comparing `airbyte_source_visma_economic-0.2.4/README.md` & `airbyte_source_visma_economic-0.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,91 +1,104 @@
 # Visma-Economic source connector
 
-
 This is the repository for the Visma-Economic source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/visma-economic).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/visma-economic)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_visma_economic/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-visma-economic spec
 poetry run source-visma-economic check --config secrets/config.json
 poetry run source-visma-economic discover --config secrets/config.json
 poetry run source-visma-economic read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-visma-economic build
 ```
 
 An image will be available on your host with the tag `airbyte/source-visma-economic:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-visma-economic:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-visma-economic:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-visma-economic:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-visma-economic:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-visma-economic test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-visma-economic test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/visma-economic.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_visma_economic-0.2.4/pyproject.toml` & `airbyte_source_visma_economic-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.2.4"
+version = "0.2.5"
 name = "airbyte-source-visma-economic"
 description = "Source implementation for Visma Economic."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_visma_economic-0.2.4/source_visma_economic/manifest.yaml` & `airbyte_source_visma_economic-0.2.5/source_visma_economic/manifest.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,2653 +1,2705 @@
-version: "0.29.0"
+version: 0.79.1
+
+type: DeclarativeSource
+
+check:
+  type: CheckStream
+  stream_names:
+    - accounts
 
 definitions:
-  selector:
-    type: RecordSelector
-    extractor:
-      type: DpathExtractor
-      field_path: ["collection"]
-  requester:
+  streams:
+    accounts:
+      type: DeclarativeStream
+      name: accounts
+      primary_key:
+        - accountNumber
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: accounts
+          http_method: GET
+          request_parameters:
+            pagesize: "1000"
+          request_headers:
+            X-AppSecretToken: "{{config['app_secret_token']}}"
+            X-AgreementGrantToken: "{{config['agreement_grant_token']}}"
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path:
+              - collection
+        paginator:
+          type: DefaultPaginator
+          page_token_option:
+            type: RequestPath
+          pagination_strategy:
+            type: CursorPagination
+            cursor_value: "{{ response['pagination']['nextPage'] }}"
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/accounts"
+    customers:
+      type: DeclarativeStream
+      name: customers
+      primary_key:
+        - customerNumber
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: customers
+          http_method: GET
+          request_parameters:
+            pagesize: "1000"
+          request_headers:
+            X-AppSecretToken: "{{config['app_secret_token']}}"
+            X-AgreementGrantToken: "{{config['agreement_grant_token']}}"
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path:
+              - collection
+        paginator:
+          type: DefaultPaginator
+          page_token_option:
+            type: RequestPath
+          pagination_strategy:
+            type: CursorPagination
+            cursor_value: "{{ response['pagination']['nextPage'] }}"
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/customers"
+    products:
+      type: DeclarativeStream
+      name: products
+      primary_key:
+        - productNumber
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: products
+          http_method: GET
+          request_parameters:
+            pagesize: "1000"
+          request_headers:
+            X-AppSecretToken: "{{config['app_secret_token']}}"
+            X-AgreementGrantToken: "{{config['agreement_grant_token']}}"
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path:
+              - collection
+        paginator:
+          type: DefaultPaginator
+          page_token_option:
+            type: RequestPath
+          pagination_strategy:
+            type: CursorPagination
+            cursor_value: "{{ response['pagination']['nextPage'] }}"
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/products"
+    invoices_total:
+      type: DeclarativeStream
+      name: invoices_total
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: invoices/totals
+          http_method: GET
+          request_parameters:
+            pagesize: "1000"
+          request_headers:
+            X-AppSecretToken: "{{config['app_secret_token']}}"
+            X-AgreementGrantToken: "{{config['agreement_grant_token']}}"
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path: []
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/invoices_total"
+    invoices_paid:
+      type: DeclarativeStream
+      name: invoices_paid
+      primary_key:
+        - bookedInvoiceNumber
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: invoices/paid
+          http_method: GET
+          request_parameters:
+            pagesize: "1000"
+          request_headers:
+            X-AppSecretToken: "{{config['app_secret_token']}}"
+            X-AgreementGrantToken: "{{config['agreement_grant_token']}}"
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path:
+              - collection
+        paginator:
+          type: DefaultPaginator
+          page_token_option:
+            type: RequestPath
+          pagination_strategy:
+            type: CursorPagination
+            cursor_value: "{{ response['pagination']['nextPage'] }}"
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/invoices_paid"
+    invoices_booked:
+      type: DeclarativeStream
+      name: invoices_booked
+      primary_key:
+        - bookedInvoiceNumber
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: invoices/booked
+          http_method: GET
+          request_parameters:
+            pagesize: "1000"
+          request_headers:
+            X-AppSecretToken: "{{config['app_secret_token']}}"
+            X-AgreementGrantToken: "{{config['agreement_grant_token']}}"
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path:
+              - collection
+        paginator:
+          type: DefaultPaginator
+          page_token_option:
+            type: RequestPath
+          pagination_strategy:
+            type: CursorPagination
+            cursor_value: "{{ response['pagination']['nextPage'] }}"
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/invoices_booked"
+    invoices_booked_document:
+      type: DeclarativeStream
+      name: invoices_booked_document
+      primary_key:
+        - bookedInvoiceNumber
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: invoices/booked/{{ stream_slice.parent_id }}
+          http_method: GET
+          request_parameters:
+            pagesize: "1000"
+          request_headers:
+            X-AppSecretToken: "{{config['app_secret_token']}}"
+            X-AgreementGrantToken: "{{config['agreement_grant_token']}}"
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path: []
+        partition_router:
+          - type: SubstreamPartitionRouter
+            parent_stream_configs:
+              - type: ParentStreamConfig
+                parent_key: bookedInvoiceNumber
+                partition_field: parent_id
+                stream:
+                  $ref: "#/definitions/streams/invoices_booked"
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/invoices_booked_document"
+  base_requester:
     type: HttpRequester
-    url_base: "https://restapi.e-conomic.com/"
-    http_method: "GET"
-    request_headers:
-      X-AppSecretToken: "{{config['app_secret_token']}}"
-      X-AgreementGrantToken: "{{config['agreement_grant_token']}}"
-    request_parameters:
-      pagesize: "1000"
-  retriever:
-    type: SimpleRetriever
-    record_selector:
-      $ref: "#/definitions/selector"
-    paginator:
-      type: "DefaultPaginator"
-      pagination_strategy:
-        type: "CursorPagination"
-        cursor_value: "{{ response['pagination']['nextPage'] }}"
-      page_token_option:
-        type: "RequestPath"
-    requester:
-      $ref: "#/definitions/requester"
-  base_stream:
-    type: DeclarativeStream
-    retriever:
-      $ref: "#/definitions/retriever"
+    url_base: https://restapi.e-conomic.com/
+
+streams:
+  - $ref: "#/definitions/streams/accounts"
+  - $ref: "#/definitions/streams/customers"
+  - $ref: "#/definitions/streams/products"
+  - $ref: "#/definitions/streams/invoices_total"
+  - $ref: "#/definitions/streams/invoices_paid"
+  - $ref: "#/definitions/streams/invoices_booked"
+  - $ref: "#/definitions/streams/invoices_booked_document"
 
-  accounts_stream:
-    $ref: "#/definitions/base_stream"
-    name: "accounts"
-    primary_key: "accountNumber"
-    $parameters:
-      path: "accounts"
+spec:
+  type: Spec
+  connection_specification:
+    type: object
+    $schema: http://json-schema.org/draft-07/schema#
+    required:
+      - agreement_grant_token
+      - app_secret_token
+    properties:
+      agreement_grant_token:
+        type: string
+        title: Agreement Grant Token
+        description: Identifier for the grant issued by an agreement
+        airbyte_secret: true
+        order: 0
+      app_secret_token:
+        type: string
+        title: App Secret Token
+        description: Identification token for app accessing data
+        airbyte_secret: true
+        order: 1
+    additionalProperties: true
 
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: https://json-schema.org/draft-07/schema#
-        title: Accounts collection schema
-        description: A schema for retrieving the accounts of the chart of accounts.
+metadata:
+  autoImportSchema:
+    accounts: false
+    customers: false
+    products: false
+    invoices_total: false
+    invoices_paid: false
+    invoices_booked: false
+    invoices_booked_document: false
+
+schemas:
+  accounts:
+    type: object
+    $schema: https://json-schema.org/draft-07/schema#
+    additionalProperties: true
+    description: A schema for retrieving the accounts of the chart of accounts.
+    properties:
+      accountNumber:
+        type: integer
+        defaultsorting: ascending
+        description: The account's number.
+        filterable: true
+        sortable: true
+      accountType:
+        type: string
+        default: profitAndLoss
+        description: The type of account in the chart of accounts.
+        filterable: true
+        sortable: true
+      accountingYears:
+        type: string
+        description: A link to a list of accounting years for which the account is usable.
+        format: uri
+      accountsSummed:
+        type: array
+        description: >-
+          An array of the account intervals used for calculating the total for
+          this account.
+        items:
+          type: object
+          description: An account interval.
+          properties:
+            fromAccount:
+              type: object
+              description: The first account in the interval.
+              properties:
+                accountNumber:
+                  type: integer
+                  description: Account number of the first account in the interval.
+                self:
+                  type: string
+                  description: The unique self link of the first account in the interval.
+                  format: uri
+            toAccount:
+              type: object
+              description: The last account in the interval.
+              properties:
+                accountNumber:
+                  type: integer
+                  description: Account number of the last account in the interval.
+                self:
+                  type: string
+                  description: The unique self link of the last account in the interval.
+                  format: uri
+      balance:
+        type: number
+        description: The current balanace of the account.
+        filterable: true
+        maxDecimal: 2
+        sortable: true
+      barred:
+        type: boolean
+        description: Shows if the account is barred from being used.
+        filterable: true
+      blockDirectEntries:
+        type: boolean
+        description: Determines if the account can be manually updated with entries.
+        filterable: true
+        sortable: true
+      contraAccount:
         type: object
+        description: The default contra account of the account.
         properties:
           accountNumber:
             type: integer
-            filterable: true
-            sortable: true
-            defaultsorting: ascending
-            description: The account's number.
-          accountType:
-            type: string
-            default: profitAndLoss
-            filterable: true
-            sortable: true
-            description: The type of account in the chart of accounts.
-          balance:
-            type: number
-            maxDecimal: 2
-            filterable: true
-            sortable: true
-            description: The current balanace of the account.
-          draftBalance:
-            type: number
-            maxDecimals: 2
-            description:
-              The current balance of the account including draft (not yet
-              booked) entries.
-          barred:
-            type: boolean
-            filterable: true
-            description: Shows if the account is barred from being used.
-          blockDirectEntries:
-            type: boolean
-            sortable: true
-            filterable: true
-            description: Determines if the account can be manually updated with entries.
-          department:
-            description: The department associated with this account
-            type:
-              - "null"
-              - object
-          departmentalDistribution:
-            description: The distribution of the account by department
-            type:
-              - "null"
-              - object
-          contraAccount:
-            type: object
-            description: The default contra account of the account.
-            properties:
-              accountNumber:
-                type: integer
-                description: Account number of the contra account.
-              self:
-                type: string
-                format: uri
-                description: The unique self link of the contra account.
-          debitCredit:
-            enum:
-              - debit
-              - credit
-            default: debit
-            sortable: true
-            filterable: true
-            description: Describes the default update type of the account.
-          name:
-            type: string
-            sortable: true
-            filterable: true
-            description: The name of the account.
-          vatAccount:
-            description: Information about the VAT account
-            type: object
-            desciption: The default VAT code for this account.
-            properties:
-              vatCode:
-                type: string
-                description: The VAT code of the VAT account for this account.
-              self:
-                type: string
-                format: uri
-                description: The unique self link of the VAT code.
-          accountsSummed:
-            type: array
-            description:
-              An array of the account intervals used for calculating the
-              total for this account.
-            items:
-              type: object
-              description: An account interval.
-              properties:
-                fromAccount:
-                  type: object
-                  description: The first account in the interval.
-                  properties:
-                    accountNumber:
-                      type: integer
-                      description: Account number of the first account in the interval.
-                    self:
-                      type: string
-                      format: uri
-                      description:
-                        The unique self link of the first account in the
-                        interval.
-                toAccount:
-                  type: object
-                  description: The last account in the interval.
-                  properties:
-                    accountNumber:
-                      type: integer
-                      description: Account number of the last account in the interval.
-                    self:
-                      type: string
-                      format: uri
-                      description:
-                        The unique self link of the last account in the
-                        interval.
-          totalFromAccount:
-            type: object
-            description:
-              The account from which the sum total for this account is
-              calculated.
-            properties:
-              accountNumber:
-                type: integer
-                description: Account number of the first account.
-              self:
-                type: string
-                format: uri
-                description: The unique self link of the first account.
-          accountingYears:
+            description: Account number of the contra account.
+          self:
             type: string
+            description: The unique self link of the contra account.
             format: uri
-            description:
-              A link to a list of accounting years for which the account
-              is usable.
+      debitCredit:
+        default: debit
+        description: Describes the default update type of the account.
+        enum:
+          - debit
+          - credit
+        filterable: true
+        sortable: true
+      department:
+        type:
+          - "null"
+          - object
+        description: The department associated with this account
+      departmentalDistribution:
+        type:
+          - "null"
+          - object
+        description: The distribution of the account by department
+      draftBalance:
+        type: number
+        description: >-
+          The current balance of the account including draft (not yet booked)
+          entries.
+        maxDecimals: 2
+      name:
+        type: string
+        description: The name of the account.
+        filterable: true
+        sortable: true
+      openingAccount:
+        type:
+          - "null"
+          - object
+        description: Information about the opening account
+        properties:
+          accountNumber:
+            type: integer
+            description: The account number of the opening account
           self:
             type: string
+            description: The unique self link of the VAT code.
             format: uri
-            description: A unique reference to the account resource.
-          openingAccount:
-            description: Information about the opening account
-            type:
-              - "null"
-              - object
-            properties:
-              accountNumber:
-                description: The account number of the opening account
-                type: integer
-              self:
-                type: string
-                format: uri
-                description: The unique self link of the VAT code.
-  customers_stream:
-    $ref: "#/definitions/base_stream"
-    name: "customers"
-    primary_key: "customerNumber"
-    $parameters:
-      path: "customers"
-
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: https://json-schema.org/draft-07/schema#
-        title: Customer collection GET schema
-        description: A schema for fetching a collection of customer, aka. Debtor.
+      self:
+        type: string
+        description: A unique reference to the account resource.
+        format: uri
+      totalFromAccount:
         type: object
+        description: The account from which the sum total for this account is calculated.
         properties:
-          address:
-            type: string
-            sortable: true
-            filterable: true
-            description: Address for the customer including street and number.
-          balance:
-            type: number
-            readOnly: true
-            sortable: true
-            filterable: true
-            description: The outstanding amount for this customer.
-          dueAmount:
-            description: The total amount that the customer owes
-            type:
-              - "null"
-              - number
-          barred:
-            type: boolean
-            filterable: true
-            description:
-              Boolean indication of whether the customer is barred from
-              invoicing.
-          city:
+          accountNumber:
+            type: integer
+            description: Account number of the first account.
+          self:
             type: string
-            sortable: true
-            filterable: true
-            description: The customer's city.
-          corporateIdentificationNumber:
+            description: The unique self link of the first account.
+            format: uri
+      vatAccount:
+        type: object
+        desciption: The default VAT code for this account.
+        description: Information about the VAT account
+        properties:
+          self:
             type: string
-            sortable: true
-            filterable: true
-            description: Corporate Identification Number. For example CVR in Denmark.
-          pNumber:
+            description: The unique self link of the VAT code.
+            format: uri
+          vatCode:
             type: string
-            minLength: 10
-            description:
-              Extension of corporate identification number (CVR). Identifying
-              separate production unit (p-nummer).
-          country:
+            description: The VAT code of the VAT account for this account.
+    title: Accounts collection schema
+  customers:
+    type: object
+    $schema: https://json-schema.org/draft-07/schema#
+    additionalProperties: true
+    description: A schema for fetching a collection of customer, aka. Debtor.
+    properties:
+      address:
+        type: string
+        description: Address for the customer including street and number.
+        filterable: true
+        sortable: true
+      attention:
+        type: object
+        description: The customer's person of attention.
+        properties:
+          customerContactNumber:
+            type: integer
+            description: The unique identifier of the customer employee.
+          self:
             type: string
-            sortable: true
-            filterable: true
-            description: The customer's country.
-          creditLimit:
-            type: number
-            sortable: true
-            filterable: true
-            description:
-              A maximum credit for this customer. Once the maximum is reached
-              or passed in connection with an order/quotation/invoice for this customer
-              you see a warning in e-conomic.
-          currency:
+            description: A unique link reference to the customer employee item.
+            format: uri
+      balance:
+        type: number
+        description: The outstanding amount for this customer.
+        filterable: true
+        readOnly: true
+        sortable: true
+      barred:
+        type: boolean
+        description: Boolean indication of whether the customer is barred from invoicing.
+        filterable: true
+      city:
+        type: string
+        description: The customer's city.
+        filterable: true
+        sortable: true
+      contacts:
+        type: string
+        description: A unique link reference to the customer contacts items.
+        format: uri
+      corporateIdentificationNumber:
+        type: string
+        description: Corporate Identification Number. For example CVR in Denmark.
+        filterable: true
+        sortable: true
+      country:
+        type: string
+        description: The customer's country.
+        filterable: true
+        sortable: true
+      creditLimit:
+        type: number
+        description: >-
+          A maximum credit for this customer. Once the maximum is reached or
+          passed in connection with an order/quotation/invoice for this customer
+          you see a warning in e-conomic.
+        filterable: true
+        sortable: true
+      currency:
+        type: string
+        description: Default payment currency.
+        filterable: true
+        minLength: 3
+        sortable: true
+      customerContact:
+        type: object
+        description: Reference to main contact employee at customer.
+        properties:
+          customerContactNumber:
+            type: integer
+            description: The unique identifier of the customer contact.
+          self:
             type: string
-            minLength: 3
-            sortable: true
-            filterable: true
-            description: Default payment currency.
-          customerNumber:
+            description: A unique link reference to the customer contact item.
+            format: uri
+      customerGroup:
+        type: object
+        description: Reference to the customer group this customer is attached to.
+        properties:
+          customerGroupNumber:
             type: integer
-            maximum: 999999999
-            minimum: 1
-            sortable: true
-            filterable: true
-            description:
-              The customer number is a positive unique numerical identifier
-              with a maximum of 9 digits.
-          ean:
+            description: The unique identifier of the customer group.
+          self:
             type: string
-            sortable: true
-            filterable: true
-            description:
-              European Article Number. EAN is used for invoicing the Danish
-              public sector.
-          email:
+            description: A unique link reference to the customer group item.
+            format: uri
+      customerNumber:
+        type: integer
+        description: >-
+          The customer number is a positive unique numerical identifier with a
+          maximum of 9 digits.
+        filterable: true
+        maximum: 999999999
+        minimum: 1
+        sortable: true
+      defaultDeliveryLocation:
+        type: object
+        description: Customers default delivery location.
+        properties:
+          deliveryLocationNumber:
+            type: integer
+            description: The unique identifier of the delivery location.
+          self:
             type: string
-            sortable: true
-            filterable: true
-            description:
-              "Customer e-mail address where e-conomic invoices should
-              be emailed. Note: you can specify multiple email addresses in this field,
-              separated by a space. If you need to send a copy of the invoice or write
-              to other e-mail addresses, you can also create one or more customer
-              contacts."
-          lastUpdated:
+            description: A unique link reference to the delivery location.
+            format: uri
+      deliveryLocations:
+        type: string
+        description: A unique link reference to the customer delivery locations items.
+        format: uri
+      dueAmount:
+        type:
+          - "null"
+          - number
+        description: The total amount that the customer owes
+      eInvoicingDisabledByDefault:
+        type: boolean
+        description: >-
+          Boolean indication of whether the default sending method should be
+          email instead of e-invoice. This property is updatable only by using
+          PATCH to /customers/:customerNumber
+        readonly: false
+      ean:
+        type: string
+        description: >-
+          European Article Number. EAN is used for invoicing the Danish public
+          sector.
+        filterable: true
+        sortable: true
+      email:
+        type: string
+        description: >-
+          Customer e-mail address where e-conomic invoices should be emailed.
+          Note: you can specify multiple email addresses in this field,
+          separated by a space. If you need to send a copy of the invoice or
+          write to other e-mail addresses, you can also create one or more
+          customer contacts.
+        filterable: true
+        sortable: true
+      invoices:
+        type: object
+        properties:
+          booked:
             type: string
-            format: full-date
-            pattern: \d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}Z
-            sortable: true
-            filterable: true
-            description:
-              The date this customer was last updated. The date is formatted
-              according to ISO-8601.
-          name:
+            description: The unique reference to the booked invoices for this customer.
+            format: uri
+          drafts:
             type: string
-            minLength: 1
-            sortable: true
-            filterable: true
-            description: The customer name.
-          publicEntryNumber:
+            description: The unique reference to the draft invoices for this customer.
+            format: uri
+          self:
             type: string
-            sortable: true
-            filterable: true
-            description:
-              The public entry number is used for electronic invoicing,
-              to define the account invoices will be registered on at the customer.
-          telephoneAndFaxNumber:
+            description: >-
+              A unique link reference to the invoices resource for this
+              customer.
+            format: uri
+      lastUpdated:
+        type: string
+        description: >-
+          The date this customer was last updated. The date is formatted
+          according to ISO-8601.
+        filterable: true
+        format: full-date
+        pattern: \d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}Z
+        sortable: true
+      layout:
+        type: object
+        description: >-
+          Layout to be applied for invoices and other documents for this
+          customer.
+        properties:
+          layoutNumber:
+            type: integer
+            description: The unique identifier of the layout.
+          self:
             type: string
-            sortable: true
-            filterable: true
-            description: The customer's telephone and/or fax number.
-          mobilePhone:
+            description: A unique link reference to the layout item.
+            format: uri
+      mobilePhone:
+        type: string
+        description: The customer's mobile phone number.
+        filterable: true
+        sortable: true
+      name:
+        type: string
+        description: The customer name.
+        filterable: true
+        minLength: 1
+        sortable: true
+      pNumber:
+        type: string
+        description: >-
+          Extension of corporate identification number (CVR). Identifying
+          separate production unit (p-nummer).
+        minLength: 10
+      paymentTerms:
+        type: object
+        description: The default payment terms for the customer.
+        properties:
+          paymentTermsNumber:
+            type: integer
+            description: The unique identifier of the payment terms.
+          self:
             type: string
-            sortable: true
-            filterable: true
-            description: The customer's mobile phone number.
-          eInvoicingDisabledByDefault:
-            type: boolean
-            readonly: false
-            description:
-              Boolean indication of whether the default sending method
-              should be email instead of e-invoice. This property is updatable only
-              by using PATCH to /customers/:customerNumber
-          vatNumber:
+            description: A unique link reference to the payment terms item.
+            format: uri
+      publicEntryNumber:
+        type: string
+        description: >-
+          The public entry number is used for electronic invoicing, to define
+          the account invoices will be registered on at the customer.
+        filterable: true
+        sortable: true
+      salesPerson:
+        type: object
+        description: Reference to the employee responsible for contact with this customer.
+        properties:
+          employeeNumber:
+            type: integer
+            description: The unique identifier of the employee.
+          self:
             type: string
-            sortable: true
-            filterable: true
-            description:
-              The customer's value added tax identification number. This
-              field is only available to agreements in Sweden, UK, Germany, Poland
-              and Finland. Not to be mistaken for the danish CVR number, which is
-              defined on the corporateIdentificationNumber property.
-          website:
+            description: A unique link reference to the employee resource.
+            format: uri
+      self:
+        type: string
+        description: The unique self reference of the customer resource.
+        format: uri
+      telephoneAndFaxNumber:
+        type: string
+        description: The customer's telephone and/or fax number.
+        filterable: true
+        sortable: true
+      templates:
+        type: object
+        properties:
+          invoice:
             type: string
-            sortable: true
-            filterable: true
-            description: Customer website, if applicable.
-          zip:
+            description: The unique reference to the invoice template.
+            format: uri
+          invoiceLine:
             type: string
-            sortable: true
-            filterable: true
-            description: The customer's postcode.
-          contacts:
+            description: The unique reference to the invoiceLine template.
+            format: uri
+          self:
             type: string
+            description: A unique link reference to the templates resource.
             format: uri
-            description: A unique link reference to the customer contacts items.
-          deliveryLocations:
+      totals:
+        type: object
+        properties:
+          booked:
             type: string
+            description: >-
+              The unique reference to the booked invoice totals for this
+              customer.
             format: uri
-            description:
-              A unique link reference to the customer delivery locations
-              items.
-          defaultDeliveryLocation:
-            type: object
-            description: Customers default delivery location.
-            properties:
-              deliveryLocationNumber:
-                type: integer
-                description: The unique identifier of the delivery location.
-              self:
-                type: string
-                format: uri
-                description: A unique link reference to the delivery location.
-          attention:
-            type: object
-            description: The customer's person of attention.
-            properties:
-              customerContactNumber:
-                type: integer
-                description: The unique identifier of the customer employee.
-              self:
-                type: string
-                format: uri
-                description: A unique link reference to the customer employee item.
-          customerContact:
-            type: object
-            description: Reference to main contact employee at customer.
-            properties:
-              customerContactNumber:
-                type: integer
-                description: The unique identifier of the customer contact.
-              self:
-                type: string
-                format: uri
-                description: A unique link reference to the customer contact item.
-          customerGroup:
-            type: object
-            description:
-              Reference to the customer group this customer is attached
-              to.
-            properties:
-              customerGroupNumber:
-                type: integer
-                description: The unique identifier of the customer group.
-              self:
-                type: string
-                format: uri
-                description: A unique link reference to the customer group item.
-          layout:
-            type: object
-            description:
-              Layout to be applied for invoices and other documents for
-              this customer.
-            properties:
-              layoutNumber:
-                type: integer
-                description: The unique identifier of the layout.
-              self:
-                type: string
-                format: uri
-                description: A unique link reference to the layout item.
-          paymentTerms:
-            type: object
-            description: The default payment terms for the customer.
-            properties:
-              paymentTermsNumber:
-                type: integer
-                description: The unique identifier of the payment terms.
-              self:
-                type: string
-                format: uri
-                description: A unique link reference to the payment terms item.
-          salesPerson:
-            type: object
-            description:
-              Reference to the employee responsible for contact with this
+          drafts:
+            type: string
+            description: >-
+              The unique reference to the draft invoice totals for this
               customer.
-            properties:
-              employeeNumber:
-                type: integer
-                description: The unique identifier of the employee.
-              self:
-                type: string
-                format: uri
-                description: A unique link reference to the employee resource.
-          vatZone:
-            type: object
-            description:
-              "Indicates in which VAT-zone the customer is located (e.g.:
-              domestically, in Europe or elsewhere abroad)."
-            properties:
-              vatZoneNumber:
-                type: integer
-                description: The unique identifier of the VAT-zone.
-              self:
-                type: string
-                format: uri
-                description: A unique link reference to the VAT-zone item.
-          templates:
-            type: object
-            description: ""
-            properties:
-              invoice:
-                type: string
-                format: uri
-                description: The unique reference to the invoice template.
-              invoiceLine:
-                type: string
-                format: uri
-                description: The unique reference to the invoiceLine template.
-              self:
-                type: string
-                format: uri
-                description: A unique link reference to the templates resource.
-          totals:
-            type: object
-            description: ""
-            properties:
-              drafts:
-                type: string
-                format: uri
-                description:
-                  The unique reference to the draft invoice totals for
-                  this customer.
-              booked:
-                type: string
-                format: uri
-                description:
-                  The unique reference to the booked invoice totals for
-                  this customer.
-              self:
-                type: string
-                format: uri
-                description:
-                  A unique link reference to the totals resource for this
-                  customer.
-          invoices:
-            type: object
-            description: ""
-            properties:
-              drafts:
-                type: string
-                format: uri
-                description: The unique reference to the draft invoices for this customer.
-              booked:
-                type: string
-                format: uri
-                description:
-                  The unique reference to the booked invoices for this
-                  customer.
-              self:
-                type: string
-                format: uri
-                description:
-                  A unique link reference to the invoices resource for
-                  this customer.
+            format: uri
           self:
             type: string
+            description: A unique link reference to the totals resource for this customer.
             format: uri
-            description: The unique self reference of the customer resource.
-  products_stream:
-    $ref: "#/definitions/base_stream"
-    name: "products"
-    primary_key: "productNumber"
-    $parameters:
-      path: "products"
-
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: https://json-schema.org/draft-07/schema#
-        title: Products collection GET schema
+      vatNumber:
+        type: string
+        description: >-
+          The customer's value added tax identification number. This field is
+          only available to agreements in Sweden, UK, Germany, Poland and
+          Finland. Not to be mistaken for the danish CVR number, which is
+          defined on the corporateIdentificationNumber property.
+        filterable: true
+        sortable: true
+      vatZone:
         type: object
-        description: A schema for retrieval of a collection of products.
+        description: >-
+          Indicates in which VAT-zone the customer is located (e.g.:
+          domestically, in Europe or elsewhere abroad).
         properties:
-          productNumber:
+          self:
             type: string
-            minLength: 1
+            description: A unique link reference to the VAT-zone item.
+            format: uri
+          vatZoneNumber:
+            type: integer
+            description: The unique identifier of the VAT-zone.
+      website:
+        type: string
+        description: Customer website, if applicable.
+        filterable: true
+        sortable: true
+      zip:
+        type: string
+        description: The customer's postcode.
+        filterable: true
+        sortable: true
+    title: Customer collection GET schema
+  products:
+    type: object
+    $schema: https://json-schema.org/draft-07/schema#
+    additionalProperties: true
+    description: A schema for retrieval of a collection of products.
+    properties:
+      barCode:
+        type: string
+        description: >-
+          String representation of a machine readable barcode symbol that
+          represents this product.
+        filterable: true
+        sortable: true
+      barred:
+        type: boolean
+        description: >-
+          If this value is true, then the product can no longer be sold, and
+          trying to book an invoice with this product will not be possible.
+        filterable: true
+        sortable: true
+      costPrice:
+        type: number
+        description: >-
+          The cost of the goods. If you have the inventory module enabled, this
+          is read-only and will just be ignored.
+        filterable: true
+        maxDecimal: 2
+        sortable: true
+      departmentalDistribution:
+        type: object
+        description: >-
+          A departmental distribution defines which departments this entry is
+          distributed between. This requires the departments module to be
+          enabled.
+        properties:
+          departmentalDistributionNumber:
+            type: integer
+            description: A unique identifier of the departmental distribution.
             filterable: true
-            sortable: true
-            description: Unique alphanumeric product number.
-          description:
+            minimum: 1
+          distributionType:
             type: string
-            filterable: true
-            sortable: true
-            description: Free text description of product.
-          name:
+            description: Type of the distribution
+          self:
             type: string
-            minLength: 1
-            filterable: true
-            sortable: true
-            description: Descriptive name of the product.
-          costPrice:
+            description: A unique reference to the departmental distribution resource.
+            format: uri
+      description:
+        type: string
+        description: Free text description of product.
+        filterable: true
+        sortable: true
+      inventory:
+        type: object
+        description: >-
+          A collection of properties that are only applicable if the inventory
+          module is enabled.
+        properties:
+          available:
             type: number
-            filterable: true
-            sortable: true
+            description: >-
+              The number of units available to sell. This is the difference
+              between the amount in stock and the amount ordered by customers.
             maxDecimal: 2
-            description:
-              The cost of the goods. If you have the inventory module enabled,
-              this is read-only and will just be ignored.
-          recommendedPrice:
+            readOnly: true
+          grossWeight:
             type: number
+            description: The gross weight of the product.
             filterable: true
+            maxDecimal: 2
+            readOnly: true
             sortable: true
+          inStock:
+            type: number
+            description: >-
+              The number of units in stock including any that have been ordered
+              by customers.
             maxDecimal: 2
-            description: Recommended retail price of the goods.
-          salesPrice:
+            readOnly: true
+          inventoryLastUpdated:
+            type: string
+            description: The last time this product was updated with regards to inventory.
+            readOnly: true
+          netWeight:
             type: number
+            description: The net weight of the product.
             filterable: true
+            maxDecimal: 2
+            readOnly: true
             sortable: true
+          orderedByCustomers:
+            type: number
+            description: >-
+              The number of units that have been ordered by customers, but
+              haven't been sold yet.
             maxDecimal: 2
-            description:
-              This is the unit net price that will appear on invoice lines
-              when a product is added to an invoice line.
-          minimumStock:
-            description:
-              The minimum quantity of this product that should be kept
-              in stock to ensure availability.
-            type:
-              - "null"
-              - number
-          pricing:
-            description:
-              Pricing information for the product including cost, selling
-              price, and currency.
-            type:
-              - "null"
-              - object
-          barCode:
-            type: string
+            readOnly: true
+          orderedFromSuppliers:
+            type: number
+            description: >-
+              The number of units that have been ordered from your suppliers,
+              but haven't been delivered to you yet.
+            maxDecimal: 2
+            readOnly: true
+          packageVolume:
+            type: number
+            description: The volume the shipped package makes up.
             filterable: true
+            maxDecimal: 2
             sortable: true
-            description:
-              String representation of a machine readable barcode symbol
-              that represents this product.
-          barred:
-            type: boolean
+          recommendedCostPrice:
+            type: number
+            description: The recommendedCostPrice of the product.
             filterable: true
-            sortable: true
-            description:
-              If this value is true, then the product can no longer be
-              sold, and trying to book an invoice with this product will not be possible.
-          lastUpdated:
+            maxDecimal: 2
+      invoices:
+        type: object
+        description: >-
+          A collection of convenience links to invoices that contains this
+          product.
+        properties:
+          booked:
             type: string
-            filterable: true
-            sortable: true
-            readOnly: true
-            description:
-              The last time the product was updated, either directly or
-              through inventory changed. The date is formatted according to ISO-8601.
-          invoices:
+            description: A unique reference to the booked invoices containing this product.
+            format: uri
+          drafts:
+            type: string
+            description: A unique reference to the draft invoices containing this product.
+            format: uri
+      lastUpdated:
+        type: string
+        description: >-
+          The last time the product was updated, either directly or through
+          inventory changed. The date is formatted according to ISO-8601.
+        filterable: true
+        readOnly: true
+        sortable: true
+      minimumStock:
+        type:
+          - "null"
+          - number
+        description: >-
+          The minimum quantity of this product that should be kept in stock to
+          ensure availability.
+      name:
+        type: string
+        description: Descriptive name of the product.
+        filterable: true
+        minLength: 1
+        sortable: true
+      pricing:
+        type:
+          - "null"
+          - object
+        description: >-
+          Pricing information for the product including cost, selling price, and
+          currency.
+      productGroup:
+        type: object
+        description: A reference to the product group this product is contained within.
+        properties:
+          accrual:
             type: object
-            description:
-              A collection of convenience links to invoices that contains
-              this product.
+            description: >-
+              A reference to the accrual account this product group is connected
+              to.
             properties:
-              drafts:
+              accountNumber:
+                type: integer
+                description: Unique number identifying the accruals account.
+                readOnly: true
+              accountType:
                 type: string
-                format: uri
-                description:
-                  A unique reference to the draft invoices containing this
-                  product.
-              booked:
+                description: The type of account in the chart of accounts.
+                readOnly: true
+              accountingYears:
                 type: string
+                description: >-
+                  A link to a list of accounting years for which the account is
+                  usable.
                 format: uri
-                description:
-                  A unique reference to the booked invoices containing
-                  this product.
-          inventory:
-            type: object
-            description:
-              A collection of properties that are only applicable if the
-              inventory module is enabled.
-            properties:
-              available:
-                type: number
                 readOnly: true
-                maxDecimal: 2
-                description:
-                  The number of units available to sell. This is the difference
-                  between the amount in stock and the amount ordered by customers.
-              inStock:
-                type: number
+              accountsSummed:
+                type: array
+                description: >-
+                  An array of the account intervals used for calculating the
+                  total for this account.
+                items:
+                  type: object
+                  description: An account interval.
+                  properties:
+                    fromAccount:
+                      type: object
+                      description: The first account in the interval.
+                      properties:
+                        accountNumber:
+                          type: integer
+                          description: Account number of the first account in the interval.
+                          readOnly: true
+                        self:
+                          type: string
+                          description: >-
+                            The unique self link of the first account in the
+                            interval.
+                          format: uri
+                          readOnly: true
+                      readOnly: true
+                    toAccount:
+                      type: object
+                      description: The last account in the interval.
+                      properties:
+                        accountNumber:
+                          type: integer
+                          description: Account number of the last account in the interval.
+                          readOnly: true
+                        self:
+                          type: string
+                          description: >-
+                            The unique self link of the last account in the
+                            interval.
+                          format: uri
+                          readOnly: true
+                      readOnly: true
+                  readOnly: true
                 readOnly: true
-                maxDecimal: 2
-                description:
-                  The number of units in stock including any that have
-                  been ordered by customers.
-              orderedByCustomers:
+              balance:
                 type: number
-                readOnly: true
+                description: The current balance of the accruals account.
                 maxDecimal: 2
-                description:
-                  The number of units that have been ordered by customers,
-                  but haven't been sold yet.
-              orderedFromSuppliers:
-                type: number
                 readOnly: true
-                maxDecimal: 2
-                description:
-                  The number of units that have been ordered from your
-                  suppliers, but haven't been delivered to you yet.
-              packageVolume:
-                type: number
-                filterable: true
-                sortable: true
-                maxDecimal: 2
-                description: The volume the shipped package makes up.
-              grossWeight:
-                type: number
-                filterable: true
-                sortable: true
-                maxDecimal: 2
+              barred:
+                type: boolean
+                description: Shows if the account is barred from being used.
                 readOnly: true
-                description: The gross weight of the product.
-              netWeight:
-                type: number
-                filterable: true
-                sortable: true
-                maxDecimal: 2
+              blockDirectEntries:
+                type: boolean
+                description: >-
+                  Determines if the account can be manually updated with
+                  entries.
                 readOnly: true
-                description: The net weight of the product.
-              inventoryLastUpdated:
+              contraAccount:
+                type: object
+                description: The default contra account of the account.
+                properties:
+                  accountNumber:
+                    type: integer
+                    description: Account number of the contra account.
+                    readOnly: true
+                  self:
+                    type: string
+                    description: The unique self link of the contra account.
+                    format: uri
+                    readOnly: true
+                readOnly: true
+              debitCredit:
                 type: string
+                description: Describes the default update type of the account.
                 readOnly: true
-                description:
-                  The last time this product was updated with regards to
-                  inventory.
-              recommendedCostPrice:
+              draftBalance:
                 type: number
-                filterable: true
-                maxDecimal: 2
-                description: The recommendedCostPrice of the product.
-          unit:
-            type: object
-            description: A reference to the unit this product is counted in.
-            properties:
-              unitNumber:
-                type: integer
-                filterable: true
-                description: Unique number identifying the unit.
-              name:
-                type: string
-                description: The name of the unit.
-              self:
-                type: string
-                format: uri
-                description: A unique reference to the unit resource.
-          productGroup:
-            type: object
-            description:
-              A reference to the product group this product is contained
-              within.
-            properties:
-              productGroupNumber:
-                type: integer
-                filterable: true
-                description: Unique number identifying the product group.
+                description: >-
+                  The current balance of the account including draft (not yet
+                  booked) entries.
+                maxDecimals: 2
+                readOnly: true
               name:
                 type: string
-                minLength: 1
-                description: Descriptive name of the product group.
-              salesAccounts:
-                type: string
-                format: uri
+                description: The name of the account.
                 readOnly: true
-                description:
-                  A reference to the sales accounts in this product group
-                  resource.
-              products:
-                type: string
-                format: uri
-                readOnly: true
-                description: A reference to the products in this product group resource.
-              inventoryEnabled:
-                type: boolean
-                readOnly: true
-                description: States if the product group is inventory enabled or not.
-              accrual:
+              totalFromAccount:
                 type: object
-                readOnly: true
-                description:
-                  A reference to the accrual account this product group
-                  is connected to.
+                description: >-
+                  The account from which the sum total for this account is
+                  calculated.
                 properties:
                   accountNumber:
                     type: integer
+                    description: Account number of the first account.
                     readOnly: true
-                    description: Unique number identifying the accruals account.
-                  accountType:
-                    type: string
-                    readOnly: true
-                    description: The type of account in the chart of accounts.
-                  balance:
-                    type: number
-                    maxDecimal: 2
-                    readOnly: true
-                    description: The current balance of the accruals account.
-                  draftBalance:
-                    type: number
-                    maxDecimals: 2
-                    readOnly: true
-                    description:
-                      The current balance of the account including draft
-                      (not yet booked) entries.
-                  barred:
-                    type: boolean
-                    readOnly: true
-                    description: Shows if the account is barred from being used.
-                  blockDirectEntries:
-                    type: boolean
-                    readOnly: true
-                    description:
-                      Determines if the account can be manually updated
-                      with entries.
-                  contraAccount:
-                    type: object
-                    readOnly: true
-                    description: The default contra account of the account.
-                    properties:
-                      accountNumber:
-                        type: integer
-                        readOnly: true
-                        description: Account number of the contra account.
-                      self:
-                        type: string
-                        format: uri
-                        readOnly: true
-                        description: The unique self link of the contra account.
-                  debitCredit:
+                  self:
                     type: string
+                    description: The unique self link of the first account.
+                    format: uri
                     readOnly: true
-                    description: Describes the default update type of the account.
-                  name:
+                readOnly: true
+              vatAccount:
+                type: object
+                desciption: The default VAT code for this account.
+                properties:
+                  self:
                     type: string
+                    description: The unique self link of the VAT code.
+                    format: uri
                     readOnly: true
-                    description: The name of the account.
-                  vatAccount:
-                    type: object
-                    readOnly: true
-                    desciption: The default VAT code for this account.
-                    properties:
-                      vatCode:
-                        type: string
-                        readOnly: true
-                        description: The VAT code of the VAT account for this account.
-                      self:
-                        type: string
-                        format: uri
-                        readOnly: true
-                        description: The unique self link of the VAT code.
-                  accountsSummed:
-                    type: array
-                    readOnly: true
-                    description:
-                      An array of the account intervals used for calculating
-                      the total for this account.
-                    items:
-                      type: object
-                      readOnly: true
-                      description: An account interval.
-                      properties:
-                        fromAccount:
-                          type: object
-                          readOnly: true
-                          description: The first account in the interval.
-                          properties:
-                            accountNumber:
-                              type: integer
-                              readOnly: true
-                              description:
-                                Account number of the first account in
-                                the interval.
-                            self:
-                              type: string
-                              format: uri
-                              readOnly: true
-                              description:
-                                The unique self link of the first account
-                                in the interval.
-                        toAccount:
-                          type: object
-                          readOnly: true
-                          description: The last account in the interval.
-                          properties:
-                            accountNumber:
-                              type: integer
-                              readOnly: true
-                              description:
-                                Account number of the last account in the
-                                interval.
-                            self:
-                              type: string
-                              format: uri
-                              readOnly: true
-                              description:
-                                The unique self link of the last account
-                                in the interval.
-                  totalFromAccount:
-                    type: object
-                    readOnly: true
-                    description:
-                      The account from which the sum total for this account
-                      is calculated.
-                    properties:
-                      accountNumber:
-                        type: integer
-                        readOnly: true
-                        description: Account number of the first account.
-                      self:
-                        type: string
-                        format: uri
-                        readOnly: true
-                        description: The unique self link of the first account.
-                  accountingYears:
+                  vatCode:
                     type: string
-                    format: uri
+                    description: The VAT code of the VAT account for this account.
                     readOnly: true
-                    description:
-                      A link to a list of accounting years for which the
-                      account is usable.
-                self:
-                  type: string
-                  format: uri
-                  readOnly: true
-                  description: A unique reference to the accruals account resource.
-              self:
-                type: string
-                format: uri
-                description: A unique reference to the product group resource.
-          departmentalDistribution:
-            type: object
-            description:
-              A departmental distribution defines which departments this
-              entry is distributed between. This requires the departments module to
-              be enabled.
-            properties:
-              departmentalDistributionNumber:
-                type: integer
-                filterable: true
-                minimum: 1
-                description: A unique identifier of the departmental distribution.
-              distributionType:
-                type: string
-                description: Type of the distribution
-              self:
-                type: string
-                format: uri
-                description: A unique reference to the departmental distribution resource.
+                readOnly: true
+            readOnly: true
+            self:
+              type: string
+              description: A unique reference to the accruals account resource.
+              format: uri
+              readOnly: true
+          inventoryEnabled:
+            type: boolean
+            description: States if the product group is inventory enabled or not.
+            readOnly: true
+          name:
+            type: string
+            description: Descriptive name of the product group.
+            minLength: 1
+          productGroupNumber:
+            type: integer
+            description: Unique number identifying the product group.
+            filterable: true
+          products:
+            type: string
+            description: A reference to the products in this product group resource.
+            format: uri
+            readOnly: true
+          salesAccounts:
+            type: string
+            description: A reference to the sales accounts in this product group resource.
+            format: uri
+            readOnly: true
           self:
             type: string
+            description: A unique reference to the product group resource.
             format: uri
-            description: A unique reference to this product resource.
-  invoices_total_stream:
-    $ref: "#/definitions/base_stream"
-    name: "invoices_total"
-    primary_key: ""
-    retriever:
-      $ref: "#/definitions/retriever"
-      record_selector:
-        type: RecordSelector
-        extractor:
-          type: DpathExtractor
-          field_path: []
-      paginator:
-        type: NoPagination
-    $parameters:
-      path: "invoices/totals"
-
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: https://json-schema.org/draft-07/schema#
-        title: Invoice totals GET schema
-        description: A schema for retrieval of the totals of invoices.
+      productNumber:
+        type: string
+        description: Unique alphanumeric product number.
+        filterable: true
+        minLength: 1
+        sortable: true
+      recommendedPrice:
+        type: number
+        description: Recommended retail price of the goods.
+        filterable: true
+        maxDecimal: 2
+        sortable: true
+      salesPrice:
+        type: number
+        description: >-
+          This is the unit net price that will appear on invoice lines when a
+          product is added to an invoice line.
+        filterable: true
+        maxDecimal: 2
+        sortable: true
+      self:
+        type: string
+        description: A unique reference to this product resource.
+        format: uri
+      unit:
         type: object
+        description: A reference to the unit this product is counted in.
         properties:
-          drafts:
+          name:
+            type: string
+            description: The name of the unit.
+          self:
+            type: string
+            description: A unique reference to the unit resource.
+            format: uri
+          unitNumber:
+            type: integer
+            description: Unique number identifying the unit.
+            filterable: true
+    title: Products collection GET schema
+  invoices_total:
+    type: object
+    $schema: https://json-schema.org/draft-07/schema#
+    additionalProperties: true
+    description: A schema for retrieval of the totals of invoices.
+    properties:
+      booked:
+        type: object
+        description: The totals for booked invoices.
+        properties:
+          description:
+            type: string
+            description: A short description about this object.
+          invoiceCount:
+            type: integer
+            description: The number of booked invoices.
+          netAmountInBaseCurrency:
+            type: number
+            description: >-
+              The total invoice amount for all booked invoices in the base
+              currency of the agreement before all taxes and discounts have been
+              applied.
+            maxDecimal: 2
+          paid:
             type: object
-            description: The totals for draft invoices.
+            description: The totals for booked and paid invoices.
             properties:
-              netAmountInBaseCurrency:
-                type: number
-                maxDecimal: 2
-                description:
-                  The total invoice amount for all draft invoices in the
-                  base currency of the agreement before all taxes and discounts have
-                  been applied.
-              invoiceCount:
-                type: integer
-                description: The number of draft invoices.
               description:
                 type: string
                 description: A short description about this object.
+              invoiceCount:
+                type: integer
+                description: The number of booked and paid invoices.
+              netAmountInBaseCurrency:
+                type: number
+                description: >-
+                  The total invoice amount for all booked and paid invoices in
+                  the base currency of the agreement before all taxes and
+                  discounts have been applied.
+                maxDecimal: 2
               self:
                 type: string
+                description: A reference to the invoices totals booked paid resource.
                 format: uri
-                description: A reference to the invoices totals draft resource.
-          booked:
+          self:
+            type: string
+            description: A reference to the invoices totals booked resource.
+            format: uri
+          unpaid:
             type: object
-            description: The totals for booked invoices.
+            description: The totals for booked and unpaid invoices.
             properties:
-              netAmountInBaseCurrency:
+              description:
+                type: string
+                description: A short description about this object.
+              grossRemainderInBaseCurrency:
                 type: number
+                description: >-
+                  The gross total remaining to be paid on the booked unpaid
+                  invoices
                 maxDecimal: 2
-                description:
-                  The total invoice amount for all booked invoices in the
-                  base currency of the agreement before all taxes and discounts have
-                  been applied.
               invoiceCount:
                 type: integer
-                description: The number of booked invoices.
-              description:
-                type: string
-                description: A short description about this object.
-              paid:
+                description: The number of booked and unpaid invoices.
+              netAmountInBaseCurrency:
+                type: number
+                description: >-
+                  The total invoice amount for all booked and unpaid invoices in
+                  the base currency of the agreement before all taxes and
+                  discounts have been applied.
+                maxDecimal: 2
+              notOverdue:
                 type: object
-                description: The totals for booked and paid invoices.
+                description: >-
+                  Totals for unpaid booked invoices where due date still hasn't
+                  been surpassed. This includes invoices that are due today.
                 properties:
-                  netAmountInBaseCurrency:
-                    type: number
-                    maxDecimal: 2
-                    description:
-                      The total invoice amount for all booked and paid
-                      invoices in the base currency of the agreement before all taxes
-                      and discounts have been applied.
-                  invoiceCount:
-                    type: integer
-                    description: The number of booked and paid invoices.
                   description:
                     type: string
                     description: A short description about this object.
-                  self:
-                    type: string
-                    format: uri
-                    description: A reference to the invoices totals booked paid resource.
-              unpaid:
-                type: object
-                description: The totals for booked and unpaid invoices.
-                properties:
+                  invoiceCount:
+                    type: integer
+                    description: >-
+                      The number of  unpaid booked invoices where due date still
+                      hasn't been surpassed. This includes invoices that are due
+                      today.
                   netAmountInBaseCurrency:
                     type: number
+                    description: >-
+                      The total invoice amount for unpaid booked invoices where
+                      due date still hasn't been surpassed. in the base currency
+                      of the agreement before all taxes and discounts have been
+                      applied.
                     maxDecimal: 2
-                    description:
-                      The total invoice amount for all booked and unpaid
-                      invoices in the base currency of the agreement before all taxes
-                      and discounts have been applied.
+                  self:
+                    type: string
+                    description: >-
+                      A reference to the invoices totals booked unpaid not
+                      overdue resource.
+                    format: uri
+              overdue:
+                type: object
+                description: >-
+                  Totals for unpaid booked invoices where due date has been
+                  surpassed.
+                properties:
+                  description:
+                    type: string
+                    description: A short description about this object.
                   grossRemainderInBaseCurrency:
                     type: number
+                    description: >-
+                      The gross total remaining to be paid on the booked, unpaid
+                      and overdue invoices
                     maxDecimal: 2
-                    description:
-                      The gross total remaining to be paid on the booked
-                      unpaid invoices
                   invoiceCount:
                     type: integer
-                    description: The number of booked and unpaid invoices.
-                  description:
-                    type: string
-                    description: A short description about this object.
-                  overdue:
-                    type: object
-                    description:
-                      Totals for unpaid booked invoices where due date
-                      has been surpassed.
-                    properties:
-                      netAmountInBaseCurrency:
-                        type: number
-                        maxDecimal: 2
-                        description:
-                          The total invoice amount for unpaid booked invoices
-                          where due date has been surpassed in the base currency of
-                          the agreement before all taxes and discounts have been applied.
-                      grossRemainderInBaseCurrency:
-                        type: number
-                        maxDecimal: 2
-                        description:
-                          The gross total remaining to be paid on the booked,
-                          unpaid and overdue invoices
-                      invoiceCount:
-                        type: integer
-                        description:
-                          The number of unpaid booked invoices where due
-                          date has been surpassed.
-                      description:
-                        type: string
-                        description: A short description about this object.
-                      self:
-                        type: string
-                        format: uri
-                        description:
-                          A reference to the invoices totals booked unpaid
-                          overdue resource.
-                  notOverdue:
-                    type: object
-                    description:
-                      Totals for unpaid booked invoices where due date
-                      still hasn't been surpassed. This includes invoices that are
-                      due today.
-                    properties:
-                      netAmountInBaseCurrency:
-                        type: number
-                        maxDecimal: 2
-                        description:
-                          The total invoice amount for unpaid booked invoices
-                          where due date still hasn't been surpassed. in the base
-                          currency of the agreement before all taxes and discounts
-                          have been applied.
-                      invoiceCount:
-                        type: integer
-                        description:
-                          The number of  unpaid booked invoices where due
-                          date still hasn't been surpassed. This includes invoices
-                          that are due today.
-                      description:
-                        type: string
-                        description: A short description about this object.
-                      self:
-                        type: string
-                        format: uri
-                        description:
-                          A reference to the invoices totals booked unpaid
-                          not overdue resource.
+                    description: >-
+                      The number of unpaid booked invoices where due date has
+                      been surpassed.
+                  netAmountInBaseCurrency:
+                    type: number
+                    description: >-
+                      The total invoice amount for unpaid booked invoices where
+                      due date has been surpassed in the base currency of the
+                      agreement before all taxes and discounts have been
+                      applied.
+                    maxDecimal: 2
                   self:
                     type: string
-                    format: uri
-                    description:
-                      A reference to the invoices totals booked unpaid
+                    description: >-
+                      A reference to the invoices totals booked unpaid overdue
                       resource.
+                    format: uri
               self:
                 type: string
+                description: A reference to the invoices totals booked unpaid resource.
                 format: uri
-                description: A reference to the invoices totals booked resource.
-          predefinedPeriodFilters:
-            type: object
-            description: The totals for draft invoices.
-            properties:
-              lastFifteenDays:
-                type: object
-                description: Filter the totals to only include the last fifteen days.
-                properties:
-                  description:
-                    type: string
-                    description: A short description about this object.
-                  self:
-                    type: string
-                    format: uri
-                    description:
-                      A reference to the invoices totals for the last 15
-                      days resource.
-              lastMonth:
-                type: object
-                description:
-                  Filter the totals to only include invoices from the last
-                  calendar month.
-                properties:
-                  description:
-                    type: string
-                    description: A short description about this object.
-                  self:
-                    type: string
-                    format: uri
-                    description:
-                      A reference to the invoices totals for the last month
-                      resource.
-              lastSevenDays:
-                type: object
-                description: Filter the totals to only include the last 7 days days.
-                properties:
-                  description:
-                    type: string
-                    description: A short description about this object.
-                  self:
-                    type: string
-                    format: uri
-                    description:
-                      A reference to the invoices totals for the last 7
-                      days resource.
-              lastThirtyDays:
-                type: object
-                description: Filter the totals to only include the last 30 days days.
-                properties:
-                  description:
-                    type: string
-                    description: A short description about this object.
-                  self:
-                    type: string
-                    format: uri
-                    description:
-                      A reference to the invoices totals for the last 30
-                      days resource.
-              lastWeek:
-                type: object
-                description:
-                  Filter the totals to only include invoices from the previous
-                  week, starting last Monday.
-                properties:
-                  description:
-                    type: string
-                    description: A short description about this object.
-                  self:
-                    type: string
-                    format: uri
-                    description:
-                      A reference to the invoices totals for the last week
-                      resource.
-              lastYear:
-                type: object
-                description:
-                  Filter the totals to only include invoices from last
-                  calendar year.
-                properties:
-                  description:
-                    type: string
-                    description: A short description about this object.
-                  self:
-                    type: string
-                    format: uri
-                    description:
-                      A reference to the invoices totals for the last year
-                      resource.
-              thisMonth:
-                type: object
-                description:
-                  Filter the totals to only include invoices from this
-                  calendar month.
-                properties:
-                  description:
-                    type: string
-                    description: A short description about this object.
-                  self:
-                    type: string
-                    format: uri
-                    description:
-                      A reference to the invoices totals for this calendar
-                      month resource.
-              thisWeek:
-                type: object
-                description:
-                  Filter the totals to only include invoices from this
-                  week, starting Monday.
-                properties:
-                  description:
-                    type: string
-                    description: A short description about this object.
-                  self:
-                    type: string
-                    format: uri
-                    description:
-                      A reference to the invoices totals for this week
-                      resource.
-              thisYear:
-                type: object
-                description:
-                  Filter the totals to only include invoices from this
-                  calendar years.
-                properties:
-                  description:
-                    type: string
-                    description: A short description about this object.
-                  self:
-                    type: string
-                    format: uri
-                    description:
-                      A reference to the invoices totals for this calendar
-                      year resource.
-          self:
-            type: string
-            format: uri
-            description: A reference to the invoices totals booked resource.
-  invoices_paid_stream:
-    $ref: "#/definitions/base_stream"
-    name: "invoices_paid"
-    primary_key: "bookedInvoiceNumber"
-    $parameters:
-      path: "invoices/paid"
-
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: https://json-schema.org/draft-07/schema#
-        title: Paid invoice
+      drafts:
         type: object
+        description: The totals for draft invoices.
         properties:
-          bookedInvoiceNumber:
-            type: integer
-            minimum: 1
-            filterable: true
-            sortable: true
-            description: A reference number for the booked invoice document.
-          exchangeRate:
-            description: The exchange rate used for currency conversion, if applicable.
-            type:
-              - "null"
-              - number
-          orderNumber:
-            description: The unique order number associated with the invoice.
-            type:
-              - "null"
-              - integer
-          grossAmountInBaseCurrency:
-            description: The total gross amount of the invoice in the base currency.
-            type:
-              - "null"
-              - number
-          date:
-            type: string
-            format: full-date
-            pattern: \d{4}-\d{2}-\d{2}
-            filterable: true
-            sortable: true
-            description: Invoice issue date. Format according to ISO-8601 (YYYY-MM-DD).
-          currency:
+          description:
             type: string
-            pattern: "[a-zA-Z]{3}"
-            filterable: true
-            sortable: true
-            description: The ISO 4217 currency code of the invoice.
-          netAmount:
-            type: number
-            maxDecimal: 2
-            description:
-              The total invoice amount in the invoice currency before all
-              taxes and discounts have been applied. For a credit note this amount
-              will be negative.
+            description: A short description about this object.
+          invoiceCount:
+            type: integer
+            description: The number of draft invoices.
           netAmountInBaseCurrency:
             type: number
+            description: >-
+              The total invoice amount for all draft invoices in the base
+              currency of the agreement before all taxes and discounts have been
+              applied.
             maxDecimal: 2
-            description:
-              The total invoice amount in the base currency of the agreement
-              before all taxes and discounts have been applied. For a credit note
-              this amount will be negative.
-          grossAmount:
-            type: number
-            maxDecimal: 2
-            description:
-              The total invoice amount in the invoice currency after all
-              taxes and discounts have been applied. For a credit note this amount
-              will be negative.
-          vatAmount:
-            type: number
-            maxDecimal: 2
-            description:
-              The total amount of VAT on the invoice in the invoice currency.
-              This will have the same sign as net amount
-          roundingAmount:
-            type: number
-            maxDecimal: 2
-            description:
-              The total rounding error, if any, on the invoice in base
-              currency.
-          remainder:
-            type: number
-            maxDecimal: 2
-            readonly: true
-            description: Remaining amount to be paid.
-          remainderInBaseCurrency:
-            type: number
-            maxDecimal: 2
-            readonly: true
-            description: Remaining amount to be paid in base currency.
-          dueDate:
+          self:
             type: string
-            format: full-date
-            pattern: \d{4}-\d{2}-\d{2}
-            description:
-              The date the invoice is due for payment. Format according
-              to ISO-8601 (YYYY-MM-DD). This is only used if the terms of payment
-              is of type 'duedate'.
-          paymentTerms:
+            description: A reference to the invoices totals draft resource.
+            format: uri
+      predefinedPeriodFilters:
+        type: object
+        description: The totals for draft invoices.
+        properties:
+          lastFifteenDays:
             type: object
-            description: The terms of payment for the invoice.
+            description: Filter the totals to only include the last fifteen days.
             properties:
-              paymentTermsNumber:
-                type: integer
-                minimum: 0
-                filterable: true
-                sortable: true
-                description: A unique identifier of the payment term.
-              daysOfCredit:
-                type: integer
-                minimum: 0
-                description:
-                  The number of days of credit on the invoice. This field
-                  is only valid if terms of payment is not of type 'duedate
-              name:
-                type: string
-                maxLength: 50
-                description: The name of the payment terms.
-              paymentTermsType:
+              description:
                 type: string
-                maxLength: 30
-                description: The type the payment term.
+                description: A short description about this object.
               self:
                 type: string
+                description: >-
+                  A reference to the invoices totals for the last 15 days
+                  resource.
                 format: uri
-                description: A unique reference to the payment term resource.
-          customer:
+          lastMonth:
             type: object
-            description: The customer being invoiced.
+            description: >-
+              Filter the totals to only include invoices from the last calendar
+              month.
             properties:
-              customerNumber:
-                type: integer
-                maximum: 999999999
-                minimum: 1
-                filterable: true
-                sortable: true
-                description:
-                  The customer id number. The customer id number can be
-                  either positive or negative, but it can't be zero.
+              description:
+                type: string
+                description: A short description about this object.
               self:
                 type: string
+                description: >-
+                  A reference to the invoices totals for the last month
+                  resource.
                 format: uri
-                description: A unique reference to the customer resource.
-          recipient:
+          lastSevenDays:
             type: object
-            description:
-              The actual recipient of the invoice. This may be the same
-              info found on the customer (and will probably be so in most cases) but
-              it may also be a different recipient. For instance, the customer placing
-              the order may be ACME Headquarters, but the recipient of the invoice
-              may be ACME IT.
+            description: Filter the totals to only include the last 7 days days.
             properties:
-              name:
-                type: string
-                maxLength: 250
-                filterable: true
-                sortable: true
-                description: The name of the actual recipient.
-              address:
-                type: string
-                maxLength: 250
-                filterable: true
-                sortable: true
-                description: The street address of the actual recipient.
-              zip:
-                type: string
-                maxLength: 50
-                filterable: true
-                sortable: true
-                description: The zip code of the actual recipient.
-              city:
-                type: string
-                maxLength: 250
-                filterable: true
-                sortable: true
-                description: The city of the actual recipient.
-              country:
-                type: string
-                maxLength: 50
-                filterable: true
-                sortable: true
-                description: The country of the actual recipient.
-              ean:
-                type: string
-                maxLength: 13
-                filterable: true
-                sortable: true
-                description: The 'European Article Number' of the actual recipient.
-              publicEntryNumber:
+              description:
                 type: string
-                maxLength: 40
-                filterable: true
-                sortable: true
-                description: The public entry number of the actual recipient.
-              attention:
-                type: object
-                description: The person to whom this invoice is addressed.
-                properties:
-                  customerContactNumber:
-                    type: integer
-                    description: Unique identifier of the customer employee.
-                  self:
-                    type: string
-                    format: uri
-                    description: A unique reference to the customer employee.
-              vatZone:
-                type: object
-                description: Recipient vat zone.
-                properties:
-                  vatZoneNumber:
-                    type: integer
-                    filterable: true
-                    sortable: true
-                    description: Unique identifier of the vat zone.
-                  self:
-                    type: string
-                    format: uri
-                    description: A unique reference to the vat zone.
-              cvr:
+                description: A short description about this object.
+              self:
                 type: string
-                description:
-                  The Corporate Identification Number of the recipient
-                  for example CVR in Denmark.
-                maxLength: 40
-          deliveryLocation:
+                description: >-
+                  A reference to the invoices totals for the last 7 days
+                  resource.
+                format: uri
+          lastThirtyDays:
             type: object
-            description:
-              A reference to the place of delivery for the goods on the
-              invoice
+            description: Filter the totals to only include the last 30 days days.
             properties:
-              deliveryLocationNumber:
-                type: integer
-                filterable: true
-                sortable: true
-                description: A unique identifier for the delivery location.
+              description:
+                type: string
+                description: A short description about this object.
               self:
                 type: string
+                description: >-
+                  A reference to the invoices totals for the last 30 days
+                  resource.
                 format: uri
-                description: A unique reference to the delivery location resource.
-          delivery:
-            description:
-              Information related to the delivery of the products/services
-              from the invoice.
+          lastWeek:
             type: object
+            description: >-
+              Filter the totals to only include invoices from the previous week,
+              starting last Monday.
             properties:
-              address:
-                type: string
-                maxLength: 255
-                filterable: true
-                sortable: true
-                description:
-                  Street address where the goods must be delivered to the
-                  customer.
-              zip:
-                type: string
-                maxLength: 30
-                filterable: true
-                sortable: true
-                description: The zip code of the place of delivery.
-              city:
-                type: string
-                maxLength: 50
-                filterable: true
-                sortable: true
-                description: The city of the place of delivery
-              country:
-                type: string
-                maxLength: 50
-                filterable: true
-                sortable: true
-                description: The country of the place of delivery
-              deliveryTerms:
+              description:
                 type: string
-                maxLength: 100
-                filterable: true
-                sortable: true
-                description: Details about the terms of delivery.
-              deliveryDate:
+                description: A short description about this object.
+              self:
                 type: string
-                format: full-date
-                pattern: \d{4}-\d{2}-\d{2}
-                filterable: true
-                sortable: true
-                description: The date of delivery.
-          notes:
+                description: A reference to the invoices totals for the last week resource.
+                format: uri
+          lastYear:
             type: object
-            description: Notes on the invoice.
+            description: >-
+              Filter the totals to only include invoices from last calendar
+              year.
             properties:
-              heading:
-                type: string
-                maxLength: 250
-                filterable: true
-                sortable: true
-                description:
-                  The invoice heading. Usually displayed at the top of
-                  the invoice.
-              textLine1:
+              description:
                 type: string
-                maxLength: 1000
-                filterable: true
-                sortable: true
-                description:
-                  The first line of supplementary text on the invoice.
-                  This is usually displayed right under the heading in a smaller font.
-              textLine2:
+                description: A short description about this object.
+              self:
                 type: string
-                maxLength: 1000
-                filterable: true
-                sortable: true
-                description:
-                  The second line of supplementary text in the notes on
-                  the invoice. This is usually displayed as a footer on the invoice.
-          references:
+                description: A reference to the invoices totals for the last year resource.
+                format: uri
+          thisMonth:
             type: object
-            description: Customer and company references related to this invoice.
+            description: >-
+              Filter the totals to only include invoices from this calendar
+              month.
             properties:
-              customerContact:
-                type: object
-                description:
-                  The customer contact is a reference to the employee at
-                  the customer to contact regarding the invoice.
-                properties:
-                  customerContactNumber:
-                    type: integer
-                    minimum: 0
-                    description: Unique identifier of the customer contact.
-                  customer:
-                    type: object
-                    description: The customer this contact belongs to.
-                    properties:
-                      customerNumber:
-                        type: integer
-                        maximum: 999999999
-                        minimum: 1
-                        filterable: true
-                        sortable: true
-                        description:
-                          The customer id number. The customer id number
-                          can be either positive or negative, but it can't be zero.
-                      self:
-                        type: string
-                        format: uri
-                        description: A unique reference to the customer resource.
-                  self:
-                    type: string
-                    format: uri
-                    description: A unique reference to the customer contact resource.
-              salesPerson:
-                type: object
-                description:
-                  The sales person is a reference to the employee who sold
-                  the goods on the invoice. This is also the person who is credited
-                  with this sale in reports.
-                properties:
-                  employeeNumber:
-                    type: integer
-                    minimum: 1
-                    filterable: true
-                    sortable: true
-                    description: Unique identifier of the employee.
-                  self:
-                    type: string
-                    format: uri
-                    description: A unique reference to the employee resource.
-              vendorReference:
-                type: object
-                description: A reference to any second employee involved in the sale.
-                properties:
-                  employeeNumber:
-                    type: integer
-                    minimum: 1
-                    filterable: true
-                    sortable: true
-                    description: Unique identifier of the employee.
-                  self:
-                    type: string
-                    format: uri
-                    description: A unique reference to the employee resource.
-              other:
+              description:
                 type: string
-                maxLength: 250
-                filterable: true
-                sortable: true
-                description:
-                  A text field that can be used to save any custom reference
-                  on the invoice.
-          pdf:
-            type: object
-            description: References a pdf representation of this invoice.
-            properties:
-              download:
+                description: A short description about this object.
+              self:
                 type: string
+                description: >-
+                  A reference to the invoices totals for this calendar month
+                  resource.
                 format: uri
-                description:
-                  The unique reference of the pdf representation for this
-                  booked invoice.
-          layout:
+          thisWeek:
             type: object
-            description: Layout to be applied for this invoice.
+            description: >-
+              Filter the totals to only include invoices from this week,
+              starting Monday.
             properties:
-              layoutNumber:
-                type: integer
-                description: The unique identifier of the layout.
+              description:
+                type: string
+                description: A short description about this object.
               self:
                 type: string
+                description: A reference to the invoices totals for this week resource.
                 format: uri
-                description: A unique link reference to the layout item.
-          project:
-            description: Details of the project or client related to the invoice.
+          thisYear:
             type: object
+            description: >-
+              Filter the totals to only include invoices from this calendar
+              years.
             properties:
-              projectNumber:
-                type: integer
-                minimum: 1
-                description: A unique identifier of the project.
+              description:
+                type: string
+                description: A short description about this object.
               self:
                 type: string
+                description: >-
+                  A reference to the invoices totals for this calendar year
+                  resource.
                 format: uri
-                description: A unique reference to the project resource.
-          sent:
+      self:
+        type: string
+        description: A reference to the invoices totals booked resource.
+        format: uri
+    title: Invoice totals GET schema
+  invoices_paid:
+    type: object
+    $schema: https://json-schema.org/draft-07/schema#
+    additionalProperties: true
+    properties:
+      bookedInvoiceNumber:
+        type: integer
+        description: A reference number for the booked invoice document.
+        filterable: true
+        minimum: 1
+        sortable: true
+      currency:
+        type: string
+        description: The ISO 4217 currency code of the invoice.
+        filterable: true
+        pattern: "[a-zA-Z]{3}"
+        sortable: true
+      customer:
+        type: object
+        description: The customer being invoiced.
+        properties:
+          customerNumber:
+            type: integer
+            description: >-
+              The customer id number. The customer id number can be either
+              positive or negative, but it can't be zero.
+            filterable: true
+            maximum: 999999999
+            minimum: 1
+            sortable: true
+          self:
             type: string
+            description: A unique reference to the customer resource.
             format: uri
-            description:
-              A convenience link to see if the invoice has been sent or
-              not.
+      date:
+        type: string
+        description: Invoice issue date. Format according to ISO-8601 (YYYY-MM-DD).
+        filterable: true
+        format: full-date
+        pattern: \d{4}-\d{2}-\d{2}
+        sortable: true
+      delivery:
+        type: object
+        description: >-
+          Information related to the delivery of the products/services from the
+          invoice.
+        properties:
+          address:
+            type: string
+            description: Street address where the goods must be delivered to the customer.
+            filterable: true
+            maxLength: 255
+            sortable: true
+          city:
+            type: string
+            description: The city of the place of delivery
+            filterable: true
+            maxLength: 50
+            sortable: true
+          country:
+            type: string
+            description: The country of the place of delivery
+            filterable: true
+            maxLength: 50
+            sortable: true
+          deliveryDate:
+            type: string
+            description: The date of delivery.
+            filterable: true
+            format: full-date
+            pattern: \d{4}-\d{2}-\d{2}
+            sortable: true
+          deliveryTerms:
+            type: string
+            description: Details about the terms of delivery.
+            filterable: true
+            maxLength: 100
+            sortable: true
+          zip:
+            type: string
+            description: The zip code of the place of delivery.
+            filterable: true
+            maxLength: 30
+            sortable: true
+      deliveryLocation:
+        type: object
+        description: A reference to the place of delivery for the goods on the invoice
+        properties:
+          deliveryLocationNumber:
+            type: integer
+            description: A unique identifier for the delivery location.
+            filterable: true
+            sortable: true
           self:
             type: string
+            description: A unique reference to the delivery location resource.
             format: uri
-            description: The unique self reference of the booked invoice.
-  invoices_booked_stream:
-    $ref: "#/definitions/base_stream"
-    name: "invoices_booked"
-    primary_key: "bookedInvoiceNumber"
-    $parameters:
-      path: "invoices/booked"
-
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: https://json-schema.org/draft-07/schema#
-        title: Booked invoice collection schema
-        description: A schema for retrieving a collection of booked invoices.
+      dueDate:
+        type: string
+        description: >-
+          The date the invoice is due for payment. Format according to ISO-8601
+          (YYYY-MM-DD). This is only used if the terms of payment is of type
+          'duedate'.
+        format: full-date
+        pattern: \d{4}-\d{2}-\d{2}
+      exchangeRate:
+        type:
+          - "null"
+          - number
+        description: The exchange rate used for currency conversion, if applicable.
+      grossAmount:
+        type: number
+        description: >-
+          The total invoice amount in the invoice currency after all taxes and
+          discounts have been applied. For a credit note this amount will be
+          negative.
+        maxDecimal: 2
+      grossAmountInBaseCurrency:
+        type:
+          - "null"
+          - number
+        description: The total gross amount of the invoice in the base currency.
+      layout:
         type: object
+        description: Layout to be applied for this invoice.
         properties:
-          bookedInvoiceNumber:
+          layoutNumber:
             type: integer
-            minimum: 1
+            description: The unique identifier of the layout.
+          self:
+            type: string
+            description: A unique link reference to the layout item.
+            format: uri
+      netAmount:
+        type: number
+        description: >-
+          The total invoice amount in the invoice currency before all taxes and
+          discounts have been applied. For a credit note this amount will be
+          negative.
+        maxDecimal: 2
+      netAmountInBaseCurrency:
+        type: number
+        description: >-
+          The total invoice amount in the base currency of the agreement before
+          all taxes and discounts have been applied. For a credit note this
+          amount will be negative.
+        maxDecimal: 2
+      notes:
+        type: object
+        description: Notes on the invoice.
+        properties:
+          heading:
+            type: string
+            description: The invoice heading. Usually displayed at the top of the invoice.
             filterable: true
+            maxLength: 250
             sortable: true
-            description: A reference number for the booked invoice document.
-          orderNumber:
-            description: The unique order number associated with the invoice.
-            type:
-              - "null"
-              - integer
-          date:
+          textLine1:
             type: string
-            format: full-date
-            pattern: \d{4}-\d{2}-\d{2}
+            description: >-
+              The first line of supplementary text on the invoice. This is
+              usually displayed right under the heading in a smaller font.
             filterable: true
+            maxLength: 1000
             sortable: true
-            description: Invoice issue date. Format according to ISO-8601 (YYYY-MM-DD).
-          currency:
+          textLine2:
             type: string
-            pattern: "[a-zA-Z]{3}"
+            description: >-
+              The second line of supplementary text in the notes on the invoice.
+              This is usually displayed as a footer on the invoice.
             filterable: true
+            maxLength: 1000
             sortable: true
-            description: The ISO 4217 currency code of the invoice.
-          exchangeRate:
-            type: number
+      orderNumber:
+        type:
+          - "null"
+          - integer
+        description: The unique order number associated with the invoice.
+      paymentTerms:
+        type: object
+        description: The terms of payment for the invoice.
+        properties:
+          daysOfCredit:
+            type: integer
+            description: >-
+              The number of days of credit on the invoice. This field is only
+              valid if terms of payment is not of type 'duedate
+            minimum: 0
+          name:
+            type: string
+            description: The name of the payment terms.
+            maxLength: 50
+          paymentTermsNumber:
+            type: integer
+            description: A unique identifier of the payment term.
             filterable: true
+            minimum: 0
             sortable: true
-            maxDecimal: 6
-            description:
-              The exchange rate between the invoice currency and the base
-              currency of the agreement. The exchange rate expresses how much it will
-              cost in base currency to buy 100 units of the invoice currency.
-          netAmount:
-            type: number
-            maxDecimal: 2
-            description:
-              The total invoice amount in the invoice currency before all
-              taxes and discounts have been applied. For a credit note this amount
-              will be negative.
-          netAmountInBaseCurrency:
-            type: number
-            maxDecimal: 2
-            description:
-              The total invoice amount in the base currency of the agreement
-              before all taxes and discounts have been applied. For a credit note
-              this amount will be negative.
-          grossAmount:
-            type: number
-            maxDecimal: 2
-            description:
-              The total invoice amount in the invoice currency after all
-              taxes and discounts have been applied. For a credit note this amount
-              will be negative.
-          grossAmountInBaseCurrency:
-            type: number
-            maxDecimal: 2
-            description:
-              The total invoice amount in the base currency of the agreement
-              after all taxes and discounts have been applied. For a credit note this
-              amount will be negative.
-          vatAmount:
-            type: number
-            maxDecimal: 2
-            description:
-              The total amount of VAT on the invoice in the invoice currency.
-              This will have the same sign as net amount
-          roundingAmount:
-            type: number
-            maxDecimal: 2
-            description:
-              The total rounding error, if any, on the invoice in base
-              currency.
-          remainder:
-            type: number
-            maxDecimal: 2
-            readonly: true
-            description: Remaining amount to be paid.
-          remainderInBaseCurrency:
-            type: number
-            maxDecimal: 2
-            readonly: true
-            description: Remaining amount to be paid in base currency.
-          dueDate:
+          paymentTermsType:
             type: string
-            format: full-date
-            pattern: \d{4}-\d{2}-\d{2}
-            description:
-              The date the invoice is due for payment. Only used if the
-              terms of payment is of type 'duedate', in which case it is mandatory.
-              Format according to ISO-8601 (YYYY-MM-DD).
-          paymentTerms:
+            description: The type the payment term.
+            maxLength: 30
+          self:
+            type: string
+            description: A unique reference to the payment term resource.
+            format: uri
+      pdf:
+        type: object
+        description: References a pdf representation of this invoice.
+        properties:
+          download:
+            type: string
+            description: >-
+              The unique reference of the pdf representation for this booked
+              invoice.
+            format: uri
+      project:
+        type: object
+        description: Details of the project or client related to the invoice.
+        properties:
+          projectNumber:
+            type: integer
+            description: A unique identifier of the project.
+            minimum: 1
+          self:
+            type: string
+            description: A unique reference to the project resource.
+            format: uri
+      recipient:
+        type: object
+        description: >-
+          The actual recipient of the invoice. This may be the same info found
+          on the customer (and will probably be so in most cases) but it may
+          also be a different recipient. For instance, the customer placing the
+          order may be ACME Headquarters, but the recipient of the invoice may
+          be ACME IT.
+        properties:
+          address:
+            type: string
+            description: The street address of the actual recipient.
+            filterable: true
+            maxLength: 250
+            sortable: true
+          attention:
             type: object
-            description: The terms of payment for the invoice.
+            description: The person to whom this invoice is addressed.
             properties:
-              paymentTermsNumber:
-                type: integer
-                minimum: 0
-                filterable: true
-                sortable: true
-                description: A unique identifier of the payment term.
-              daysOfCredit:
+              customerContactNumber:
                 type: integer
-                minimum: 0
-                description:
-                  The number of days of credit on the invoice. This field
-                  is only valid if terms of payment is not of type 'duedate
-              name:
-                type: string
-                description: The name of the payment terms.
-              paymentTermsType:
-                enum:
-                  - net
-                  - invoiceMonth
-                  - paidInCash
-                  - prepaid
-                  - dueDate
-                  - factoring
-                  - invoiceWeekStartingSunday
-                  - invoiceWeekStartingMonday
-                  - creditcard
-                description: The type of payment term.
+                description: Unique identifier of the customer employee.
               self:
                 type: string
+                description: A unique reference to the customer employee.
                 format: uri
-                description: A unique reference to the payment term resource.
-          customer:
+          city:
+            type: string
+            description: The city of the actual recipient.
+            filterable: true
+            maxLength: 250
+            sortable: true
+          country:
+            type: string
+            description: The country of the actual recipient.
+            filterable: true
+            maxLength: 50
+            sortable: true
+          cvr:
+            type: string
+            description: >-
+              The Corporate Identification Number of the recipient for example
+              CVR in Denmark.
+            maxLength: 40
+          ean:
+            type: string
+            description: The 'European Article Number' of the actual recipient.
+            filterable: true
+            maxLength: 13
+            sortable: true
+          name:
+            type: string
+            description: The name of the actual recipient.
+            filterable: true
+            maxLength: 250
+            sortable: true
+          publicEntryNumber:
+            type: string
+            description: The public entry number of the actual recipient.
+            filterable: true
+            maxLength: 40
+            sortable: true
+          vatZone:
             type: object
-            description: The customer being invoiced.
+            description: Recipient vat zone.
             properties:
-              customerNumber:
-                type: integer
-                maximum: 999999999
-                minimum: 1
-                filterable: true
-                sortable: true
-                description:
-                  The customer id number. The customer id number can be
-                  either positive or negative, but it can't be zero.
               self:
                 type: string
+                description: A unique reference to the vat zone.
                 format: uri
-                description: A unique reference to the customer resource.
-          recipient:
-            type: object
-            description:
-              The actual recipient of the invoice. This may be the same
-              info found on the customer (and will probably be so in most cases) but
-              it may also be a different recipient. For instance, the customer placing
-              the order may be ACME Headquarters, but the recipient of the invoice
-              may be ACME IT.
-            properties:
-              name:
-                type: string
-                filterable: true
-                sortable: true
-                description: The name of the actual recipient.
-              address:
-                type: string
-                filterable: true
-                sortable: true
-                description: The street address of the actual recipient.
-              zip:
-                type: string
-                filterable: true
-                sortable: true
-                description: The zip code of the actual recipient.
-              city:
-                type: string
-                filterable: true
-                sortable: true
-                description: The city of the actual recipient.
-              country:
-                type: string
-                filterable: true
-                sortable: true
-                description: The country of the actual recipient.
-              ean:
-                type: string
-                filterable: true
-                sortable: true
-                description: The 'European Article Number' of the actual recipient.
-              publicEntryNumber:
-                type: string
-                filterable: true
-                sortable: true
-                description: The public entry number of the actual recipient.
-              attention:
-                type: object
-                description: The person to whom this invoice is addressed.
-                properties:
-                  customerContactNumber:
-                    type: integer
-                    description: Unique identifier of the customer employee.
-                  self:
-                    type: string
-                    format: uri
-                    description: A unique reference to the customer employee.
-              vatZone:
-                type: object
-                description: Recipient vat zone.
-                properties:
-                  vatZoneNumber:
-                    type: integer
-                    filterable: true
-                    sortable: true
-                    description: Unique identifier of the vat zone.
-                  self:
-                    type: string
-                    format: uri
-                    description: A unique reference to the vat zone.
-              cvr:
-                type: string
-                description:
-                  The Corporate Identification Number of the recipient
-                  for example CVR in Denmark.
-          deliveryLocation:
-            type: object
-            description:
-              A reference to the place of delivery for the goods on the
-              invoice
-            properties:
-              deliveryLocationNumber:
+              vatZoneNumber:
                 type: integer
+                description: Unique identifier of the vat zone.
                 filterable: true
                 sortable: true
-                description: A unique identifier for the delivery location.
-              self:
-                type: string
-                format: uri
-                description: A unique reference to the delivery location resource.
-          delivery:
-            description: Details related to the delivery of the invoice.
-            type: object
-            properties:
-              address:
-                type: string
-                filterable: true
-                sortable: true
-                description:
-                  Street address where the goods must be delivered to the
-                  customer.
-              zip:
-                type: string
-                filterable: true
-                sortable: true
-                description: The zip code of the place of delivery.
-              city:
-                type: string
-                filterable: true
-                sortable: true
-                description: The city of the place of delivery
-              country:
-                type: string
-                filterable: true
-                sortable: true
-                description: The country of the place of delivery
-              deliveryTerms:
-                type: string
-                filterable: true
-                sortable: true
-                description: Details about the terms of delivery.
-              deliveryDate:
-                type: string
-                format: full-date
-                pattern: \d{4}-\d{2}-\d{2}
-                filterable: true
-                sortable: true
-                description: The date of delivery.
-          notes:
-            type: object
-            description: Notes on the invoice.
-            properties:
-              heading:
-                type: string
-                filterable: true
-                sortable: true
-                description:
-                  The invoice heading. Usually displayed at the top of
-                  the invoice.
-              textLine1:
-                type: string
-                filterable: true
-                sortable: true
-                description:
-                  The first line of supplementary text on the invoice.
-                  This is usually displayed right under the heading in a smaller font.
-              textLine2:
-                type: string
-                filterable: true
-                sortable: true
-                description:
-                  The second line of supplementary text in the notes on
-                  the invoice. This is usually displayed as a footer on the invoice.
-          references:
+          zip:
+            type: string
+            description: The zip code of the actual recipient.
+            filterable: true
+            maxLength: 50
+            sortable: true
+      references:
+        type: object
+        description: Customer and company references related to this invoice.
+        properties:
+          customerContact:
             type: object
-            description: Customer and company references related to this invoice.
+            description: >-
+              The customer contact is a reference to the employee at the
+              customer to contact regarding the invoice.
             properties:
-              customerContact:
+              customer:
                 type: object
-                description:
-                  The customer contact is a reference to the employee at
-                  the customer to contact regarding the invoice.
+                description: The customer this contact belongs to.
                 properties:
-                  customerContactNumber:
+                  customerNumber:
                     type: integer
-                    minimum: 0
-                    description: Unique identifier of the customer contact.
-                  customer:
-                    type: object
-                    description: The customer this contact belongs to.
-                    properties:
-                      customerNumber:
-                        type: integer
-                        maximum: 999999999
-                        minimum: 1
-                        filterable: true
-                        sortable: true
-                        description:
-                          The customer id number. The customer id number
-                          can be either positive or negative, but it can't be zero.
-                      self:
-                        type: string
-                        format: uri
-                        description: A unique reference to the customer resource.
-                  self:
-                    type: string
-                    format: uri
-                    description: A unique reference to the customer contact resource.
-              salesPerson:
-                type: object
-                description:
-                  The sales person is a reference to the employee who sold
-                  the goods on the invoice. This is also the person who is credited
-                  with this sale in reports.
-                properties:
-                  employeeNumber:
-                    type: integer
-                    minimum: 1
+                    description: >-
+                      The customer id number. The customer id number can be
+                      either positive or negative, but it can't be zero.
                     filterable: true
-                    sortable: true
-                    description: Unique identifier of the employee.
-                  self:
-                    type: string
-                    format: uri
-                    description: A unique reference to the employee resource.
-              vendorReference:
-                type: object
-                description: A reference to any second employee involved in the sale.
-                properties:
-                  employeeNumber:
-                    type: integer
+                    maximum: 999999999
                     minimum: 1
-                    filterable: true
                     sortable: true
-                    description: Unique identifier of the employee.
                   self:
                     type: string
+                    description: A unique reference to the customer resource.
                     format: uri
-                    description: A unique reference to the employee resource.
-              other:
-                type: string
-                filterable: true
-                sortable: true
-                description:
-                  A text field that can be used to save any custom reference
-                  on the invoice.
-          pdf:
-            type: object
-            description: References a pdf representation of this invoice.
-            properties:
+              customerContactNumber:
+                type: integer
+                description: Unique identifier of the customer contact.
+                minimum: 0
               self:
                 type: string
+                description: A unique reference to the customer contact resource.
                 format: uri
-                description:
-                  The unique reference of the pdf representation for this
-                  booked invoice.
-          layout:
+          other:
+            type: string
+            description: >-
+              A text field that can be used to save any custom reference on the
+              invoice.
+            filterable: true
+            maxLength: 250
+            sortable: true
+          salesPerson:
             type: object
-            description: Layout to be applied for this invoice.
+            description: >-
+              The sales person is a reference to the employee who sold the goods
+              on the invoice. This is also the person who is credited with this
+              sale in reports.
             properties:
-              layoutNumber:
+              employeeNumber:
                 type: integer
-                description: The unique identifier of the layout.
+                description: Unique identifier of the employee.
+                filterable: true
+                minimum: 1
+                sortable: true
               self:
                 type: string
+                description: A unique reference to the employee resource.
                 format: uri
-                description: A unique link reference to the layout item.
-          project:
-            description: Information regarding the project associated with the invoice.
+          vendorReference:
             type: object
+            description: A reference to any second employee involved in the sale.
             properties:
-              projectNumber:
+              employeeNumber:
                 type: integer
+                description: Unique identifier of the employee.
+                filterable: true
                 minimum: 1
-                description: A unique identifier of the project.
+                sortable: true
               self:
                 type: string
+                description: A unique reference to the employee resource.
                 format: uri
-                description: A unique reference to the project resource.
-          sent:
+      remainder:
+        type: number
+        description: Remaining amount to be paid.
+        maxDecimal: 2
+        readonly: true
+      remainderInBaseCurrency:
+        type: number
+        description: Remaining amount to be paid in base currency.
+        maxDecimal: 2
+        readonly: true
+      roundingAmount:
+        type: number
+        description: The total rounding error, if any, on the invoice in base currency.
+        maxDecimal: 2
+      self:
+        type: string
+        description: The unique self reference of the booked invoice.
+        format: uri
+      sent:
+        type: string
+        description: A convenience link to see if the invoice has been sent or not.
+        format: uri
+      vatAmount:
+        type: number
+        description: >-
+          The total amount of VAT on the invoice in the invoice currency. This
+          will have the same sign as net amount
+        maxDecimal: 2
+    title: Paid invoice
+  invoices_booked:
+    type: object
+    $schema: https://json-schema.org/draft-07/schema#
+    additionalProperties: true
+    description: A schema for retrieving a collection of booked invoices.
+    properties:
+      bookedInvoiceNumber:
+        type: integer
+        description: A reference number for the booked invoice document.
+        filterable: true
+        minimum: 1
+        sortable: true
+      currency:
+        type: string
+        description: The ISO 4217 currency code of the invoice.
+        filterable: true
+        pattern: "[a-zA-Z]{3}"
+        sortable: true
+      customer:
+        type: object
+        description: The customer being invoiced.
+        properties:
+          customerNumber:
+            type: integer
+            description: >-
+              The customer id number. The customer id number can be either
+              positive or negative, but it can't be zero.
+            filterable: true
+            maximum: 999999999
+            minimum: 1
+            sortable: true
+          self:
             type: string
+            description: A unique reference to the customer resource.
             format: uri
-            description:
-              A convenience link to see if the invoice has been sent or
-              not.
+      date:
+        type: string
+        description: Invoice issue date. Format according to ISO-8601 (YYYY-MM-DD).
+        filterable: true
+        format: full-date
+        pattern: \d{4}-\d{2}-\d{2}
+        sortable: true
+      delivery:
+        type: object
+        description: Details related to the delivery of the invoice.
+        properties:
+          address:
+            type: string
+            description: Street address where the goods must be delivered to the customer.
+            filterable: true
+            sortable: true
+          city:
+            type: string
+            description: The city of the place of delivery
+            filterable: true
+            sortable: true
+          country:
+            type: string
+            description: The country of the place of delivery
+            filterable: true
+            sortable: true
+          deliveryDate:
+            type: string
+            description: The date of delivery.
+            filterable: true
+            format: full-date
+            pattern: \d{4}-\d{2}-\d{2}
+            sortable: true
+          deliveryTerms:
+            type: string
+            description: Details about the terms of delivery.
+            filterable: true
+            sortable: true
+          zip:
+            type: string
+            description: The zip code of the place of delivery.
+            filterable: true
+            sortable: true
+      deliveryLocation:
+        type: object
+        description: A reference to the place of delivery for the goods on the invoice
+        properties:
+          deliveryLocationNumber:
+            type: integer
+            description: A unique identifier for the delivery location.
+            filterable: true
+            sortable: true
           self:
             type: string
+            description: A unique reference to the delivery location resource.
             format: uri
-            description: The unique self reference of the booked invoice.
-  invoices_booked_document_stream:
-    name: "invoices_booked_document"
-    primary_key: "bookedInvoiceNumber"
-    retriever:
-      $ref: "#/definitions/retriever"
-      requester:
-        $ref: "#/definitions/requester"
-        path: "invoices/booked/{{ stream_slice.parent_id }}"
-      record_selector:
-        type: RecordSelector
-        extractor:
-          type: DpathExtractor
-          field_path: []
-      paginator:
-        type: NoPagination
-      partition_router:
-        type: SubstreamPartitionRouter
-        parent_stream_configs:
-          - stream: "#/definitions/invoices_booked_stream"
-            parent_key: "bookedInvoiceNumber"
-            partition_field: "parent_id"
-
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: https://json-schema.org/draft-07/schema#
-        title: Booked invoice schema
-        description: A schema for retrieving a booked invoice.
+      dueDate:
+        type: string
+        description: >-
+          The date the invoice is due for payment. Only used if the terms of
+          payment is of type 'duedate', in which case it is mandatory. Format
+          according to ISO-8601 (YYYY-MM-DD).
+        format: full-date
+        pattern: \d{4}-\d{2}-\d{2}
+      exchangeRate:
+        type: number
+        description: >-
+          The exchange rate between the invoice currency and the base currency
+          of the agreement. The exchange rate expresses how much it will cost in
+          base currency to buy 100 units of the invoice currency.
+        filterable: true
+        maxDecimal: 6
+        sortable: true
+      grossAmount:
+        type: number
+        description: >-
+          The total invoice amount in the invoice currency after all taxes and
+          discounts have been applied. For a credit note this amount will be
+          negative.
+        maxDecimal: 2
+      grossAmountInBaseCurrency:
+        type: number
+        description: >-
+          The total invoice amount in the base currency of the agreement after
+          all taxes and discounts have been applied. For a credit note this
+          amount will be negative.
+        maxDecimal: 2
+      layout:
         type: object
+        description: Layout to be applied for this invoice.
         properties:
-          bookedInvoiceNumber:
+          layoutNumber:
             type: integer
-            minimum: 1
+            description: The unique identifier of the layout.
+          self:
+            type: string
+            description: A unique link reference to the layout item.
+            format: uri
+      netAmount:
+        type: number
+        description: >-
+          The total invoice amount in the invoice currency before all taxes and
+          discounts have been applied. For a credit note this amount will be
+          negative.
+        maxDecimal: 2
+      netAmountInBaseCurrency:
+        type: number
+        description: >-
+          The total invoice amount in the base currency of the agreement before
+          all taxes and discounts have been applied. For a credit note this
+          amount will be negative.
+        maxDecimal: 2
+      notes:
+        type: object
+        description: Notes on the invoice.
+        properties:
+          heading:
+            type: string
+            description: The invoice heading. Usually displayed at the top of the invoice.
             filterable: true
             sortable: true
-            description: A reference number for the booked invoice document.
-          orderNumber:
-            description: The order number related to the invoice
-            type:
-              - "null"
-              - integer
-          date:
+          textLine1:
             type: string
-            format: full-date
-            pattern: \d{4}-\d{2}-\d{2}
+            description: >-
+              The first line of supplementary text on the invoice. This is
+              usually displayed right under the heading in a smaller font.
             filterable: true
             sortable: true
-            description: Invoice issue date. Format according to ISO-8601 (YYYY-MM-DD).
-          currency:
+          textLine2:
             type: string
-            pattern: "[a-zA-Z]{3}"
+            description: >-
+              The second line of supplementary text in the notes on the invoice.
+              This is usually displayed as a footer on the invoice.
             filterable: true
             sortable: true
-            description: The ISO 4217 currency code of the invoice.
-          exchangeRate:
-            type: number
+      orderNumber:
+        type:
+          - "null"
+          - integer
+        description: The unique order number associated with the invoice.
+      paymentTerms:
+        type: object
+        description: The terms of payment for the invoice.
+        properties:
+          daysOfCredit:
+            type: integer
+            description: >-
+              The number of days of credit on the invoice. This field is only
+              valid if terms of payment is not of type 'duedate
+            minimum: 0
+          name:
+            type: string
+            description: The name of the payment terms.
+          paymentTermsNumber:
+            type: integer
+            description: A unique identifier of the payment term.
             filterable: true
+            minimum: 0
             sortable: true
-            maxDecimal: 6
-            description:
-              The exchange rate between the invoice currency and the base
-              currency of the agreement. The exchange rate expresses how much it will
-              cost in base currency to buy 100 units of the invoice currency.
-          netAmount:
-            type: number
-            maxDecimal: 2
-            description:
-              The total invoice amount in the invoice currency before all
-              taxes and discounts have been applied. For a credit note this amount
-              will be negative.
-          netAmountInBaseCurrency:
-            type: number
-            maxDecimal: 2
-            description:
-              The total invoice amount in the base currency of the agreement
-              before all taxes and discounts have been applied. For a credit note
-              this amount will be negative.
-          grossAmount:
-            type: number
-            maxDecimal: 2
-            description:
-              The total invoice amount in the invoice currency after all
-              taxes and discounts have been applied. For a credit note this amount
-              will be negative.
-          grossAmountInBaseCurrency:
-            type: number
-            maxDecimal: 2
-            description:
-              The total invoice amount in the base currency of the agreement
-              after all taxes and discounts have been applied. For a credit note this
-              amount will be negative.
-          vatAmount:
-            type: number
-            maxDecimal: 2
-            description:
-              The total amount of VAT on the invoice in the invoice currency.
-              This will have the same sign as net amount
-          roundingAmount:
-            type: number
-            maxDecimal: 2
-            description:
-              The total rounding error, if any, on the invoice in base
-              currency.
-          remainder:
-            type: number
-            maxDecimal: 2
-            readonly: true
-            description: Remaining amount to be paid.
-          remainderInBaseCurrency:
-            type: number
-            maxDecimal: 2
-            readonly: true
-            description: Remaining amount to be paid in base currency.
-          dueDate:
+          paymentTermsType:
+            description: The type of payment term.
+            enum:
+              - net
+              - invoiceMonth
+              - paidInCash
+              - prepaid
+              - dueDate
+              - factoring
+              - invoiceWeekStartingSunday
+              - invoiceWeekStartingMonday
+              - creditcard
+          self:
             type: string
-            format: full-date
-            pattern: \d{4}-\d{2}-\d{2}
-            description:
-              The date the invoice is due for payment. Only used if the
-              terms of payment is of type 'duedate', in which case it is mandatory.
-              Format according to ISO-8601 (YYYY-MM-DD).
-          paymentTerms:
+            description: A unique reference to the payment term resource.
+            format: uri
+      pdf:
+        type: object
+        description: References a pdf representation of this invoice.
+        properties:
+          self:
+            type: string
+            description: >-
+              The unique reference of the pdf representation for this booked
+              invoice.
+            format: uri
+      project:
+        type: object
+        description: Information regarding the project associated with the invoice.
+        properties:
+          projectNumber:
+            type: integer
+            description: A unique identifier of the project.
+            minimum: 1
+          self:
+            type: string
+            description: A unique reference to the project resource.
+            format: uri
+      recipient:
+        type: object
+        description: >-
+          The actual recipient of the invoice. This may be the same info found
+          on the customer (and will probably be so in most cases) but it may
+          also be a different recipient. For instance, the customer placing the
+          order may be ACME Headquarters, but the recipient of the invoice may
+          be ACME IT.
+        properties:
+          address:
+            type: string
+            description: The street address of the actual recipient.
+            filterable: true
+            sortable: true
+          attention:
             type: object
-            description: The terms of payment for the invoice.
+            description: The person to whom this invoice is addressed.
             properties:
-              paymentTermsNumber:
-                type: integer
-                minimum: 0
-                filterable: true
-                sortable: true
-                description: A unique identifier of the payment term.
-              daysOfCredit:
+              customerContactNumber:
                 type: integer
-                minimum: 0
-                description:
-                  The number of days of credit on the invoice. This field
-                  is only valid if terms of payment is not of type 'duedate
-              name:
-                type: string
-                description: The name of the payment terms.
-              paymentTermsType:
-                type: string
-                description: The type of payment term.
+                description: Unique identifier of the customer employee.
               self:
                 type: string
+                description: A unique reference to the customer employee.
                 format: uri
-                description: A unique reference to the payment term resource.
-          customer:
+          city:
+            type: string
+            description: The city of the actual recipient.
+            filterable: true
+            sortable: true
+          country:
+            type: string
+            description: The country of the actual recipient.
+            filterable: true
+            sortable: true
+          cvr:
+            type: string
+            description: >-
+              The Corporate Identification Number of the recipient for example
+              CVR in Denmark.
+          ean:
+            type: string
+            description: The 'European Article Number' of the actual recipient.
+            filterable: true
+            sortable: true
+          name:
+            type: string
+            description: The name of the actual recipient.
+            filterable: true
+            sortable: true
+          publicEntryNumber:
+            type: string
+            description: The public entry number of the actual recipient.
+            filterable: true
+            sortable: true
+          vatZone:
             type: object
-            description: The customer being invoiced.
+            description: Recipient vat zone.
             properties:
-              customerNumber:
-                type: integer
-                maximum: 999999999
-                minimum: 1
-                filterable: true
-                sortable: true
-                description:
-                  The customer number is a positive unique numerical identifier
-                  with a maximum of 9 digits.
               self:
                 type: string
+                description: A unique reference to the vat zone.
                 format: uri
-                description: A unique reference to the customer resource.
-          recipient:
-            type: object
-            description:
-              The actual recipient of the invoice. This may be the same
-              info found on the customer (and will probably be so in most cases) but
-              it may also be a different recipient. For instance, the customer placing
-              the order may be ACME Headquarters, but the recipient of the invoice
-              may be ACME IT.
-            properties:
-              name:
-                type: string
-                filterable: true
-                sortable: true
-                description: The name of the actual recipient.
-                empty: true
-              address:
-                type: string
-                filterable: true
-                sortable: true
-                description: The street address of the actual recipient.
-                empty: true
-              zip:
-                type: string
-                filterable: true
-                sortable: true
-                description: The zip code of the actual recipient.
-                empty: true
-              city:
-                type: string
-                filterable: true
-                sortable: true
-                description: The city of the actual recipient.
-                empty: true
-              country:
-                type: string
-                filterable: true
-                sortable: true
-                description: The country of the actual recipient.
-              ean:
-                type: string
-                filterable: true
-                sortable: true
-                description: The 'European Article Number' of the actual recipient.
-              publicEntryNumber:
-                type: string
+              vatZoneNumber:
+                type: integer
+                description: Unique identifier of the vat zone.
                 filterable: true
                 sortable: true
-                description: The public entry number of the actual recipient.
-              attention:
-                type: object
-                description: The person to whom this invoice is addressed.
-                properties:
-                  customerContactNumber:
-                    type: integer
-                    description: Unique identifier of the customer employee.
-                  self:
-                    type: string
-                    format: uri
-                    description: A unique reference to the customer employee.
-              vatZone:
+          zip:
+            type: string
+            description: The zip code of the actual recipient.
+            filterable: true
+            sortable: true
+      references:
+        type: object
+        description: Customer and company references related to this invoice.
+        properties:
+          customerContact:
+            type: object
+            description: >-
+              The customer contact is a reference to the employee at the
+              customer to contact regarding the invoice.
+            properties:
+              customer:
                 type: object
-                description: Recipient vat zone.
+                description: The customer this contact belongs to.
                 properties:
-                  vatZoneNumber:
+                  customerNumber:
                     type: integer
+                    description: >-
+                      The customer id number. The customer id number can be
+                      either positive or negative, but it can't be zero.
                     filterable: true
+                    maximum: 999999999
+                    minimum: 1
                     sortable: true
-                    description: Unique identifier of the vat zone.
                   self:
                     type: string
+                    description: A unique reference to the customer resource.
                     format: uri
-                    description: A unique reference to the vat zone.
-              cvr:
+              customerContactNumber:
+                type: integer
+                description: Unique identifier of the customer contact.
+                minimum: 0
+              self:
                 type: string
-                description:
-                  The Corporate Identification Number of the recipient
-                  for example CVR in Denmark.
-          deliveryLocation:
+                description: A unique reference to the customer contact resource.
+                format: uri
+          other:
+            type: string
+            description: >-
+              A text field that can be used to save any custom reference on the
+              invoice.
+            filterable: true
+            sortable: true
+          salesPerson:
             type: object
-            description:
-              A reference to the place of delivery for the goods on the
-              invoice
+            description: >-
+              The sales person is a reference to the employee who sold the goods
+              on the invoice. This is also the person who is credited with this
+              sale in reports.
             properties:
-              deliveryLocationNumber:
+              employeeNumber:
                 type: integer
+                description: Unique identifier of the employee.
                 filterable: true
+                minimum: 1
                 sortable: true
-                description: A unique identifier for the delivery location.
               self:
                 type: string
+                description: A unique reference to the employee resource.
                 format: uri
-                description: A unique reference to the delivery location resource.
-          delivery:
-            description: Details of the delivery associated with the invoice
+          vendorReference:
             type: object
+            description: A reference to any second employee involved in the sale.
             properties:
-              address:
-                type: string
-                filterable: true
-                sortable: true
-                description:
-                  Street address where the goods must be delivered to the
-                  customer.
-              zip:
-                type: string
-                filterable: true
-                sortable: true
-                description: The zip code of the place of delivery.
-              city:
-                type: string
-                filterable: true
-                sortable: true
-                description: The city of the place of delivery
-              country:
-                type: string
-                filterable: true
-                sortable: true
-                description: The country of the place of delivery
-              deliveryTerms:
-                type: string
+              employeeNumber:
+                type: integer
+                description: Unique identifier of the employee.
                 filterable: true
+                minimum: 1
                 sortable: true
-                description: Details about the terms of delivery.
-              deliveryDate:
+              self:
                 type: string
-                format: full-date
-                pattern: \d{4}-\d{2}-\d{2}
-                filterable: true
-                sortable: true
-                description: The date of delivery.
-          notes:
+                description: A unique reference to the employee resource.
+                format: uri
+      remainder:
+        type: number
+        description: Remaining amount to be paid.
+        maxDecimal: 2
+        readonly: true
+      remainderInBaseCurrency:
+        type: number
+        description: Remaining amount to be paid in base currency.
+        maxDecimal: 2
+        readonly: true
+      roundingAmount:
+        type: number
+        description: The total rounding error, if any, on the invoice in base currency.
+        maxDecimal: 2
+      self:
+        type: string
+        description: The unique self reference of the booked invoice.
+        format: uri
+      sent:
+        type: string
+        description: A convenience link to see if the invoice has been sent or not.
+        format: uri
+      vatAmount:
+        type: number
+        description: >-
+          The total amount of VAT on the invoice in the invoice currency. This
+          will have the same sign as net amount
+        maxDecimal: 2
+    title: Booked invoice collection schema
+  invoices_booked_document:
+    type: object
+    $schema: https://json-schema.org/draft-07/schema#
+    additionalProperties: true
+    description: A schema for retrieving a booked invoice.
+    properties:
+      bookedInvoiceNumber:
+        type: integer
+        description: A reference number for the booked invoice document.
+        filterable: true
+        minimum: 1
+        sortable: true
+      currency:
+        type: string
+        description: The ISO 4217 currency code of the invoice.
+        filterable: true
+        pattern: "[a-zA-Z]{3}"
+        sortable: true
+      customer:
+        type: object
+        description: The customer being invoiced.
+        properties:
+          customerNumber:
+            type: integer
+            description: >-
+              The customer number is a positive unique numerical identifier with
+              a maximum of 9 digits.
+            filterable: true
+            maximum: 999999999
+            minimum: 1
+            sortable: true
+          self:
+            type: string
+            description: A unique reference to the customer resource.
+            format: uri
+      date:
+        type: string
+        description: Invoice issue date. Format according to ISO-8601 (YYYY-MM-DD).
+        filterable: true
+        format: full-date
+        pattern: \d{4}-\d{2}-\d{2}
+        sortable: true
+      delivery:
+        type: object
+        description: Details of the delivery associated with the invoice
+        properties:
+          address:
+            type: string
+            description: Street address where the goods must be delivered to the customer.
+            filterable: true
+            sortable: true
+          city:
+            type: string
+            description: The city of the place of delivery
+            filterable: true
+            sortable: true
+          country:
+            type: string
+            description: The country of the place of delivery
+            filterable: true
+            sortable: true
+          deliveryDate:
+            type: string
+            description: The date of delivery.
+            filterable: true
+            format: full-date
+            pattern: \d{4}-\d{2}-\d{2}
+            sortable: true
+          deliveryTerms:
+            type: string
+            description: Details about the terms of delivery.
+            filterable: true
+            sortable: true
+          zip:
+            type: string
+            description: The zip code of the place of delivery.
+            filterable: true
+            sortable: true
+      deliveryLocation:
+        type: object
+        description: A reference to the place of delivery for the goods on the invoice
+        properties:
+          deliveryLocationNumber:
+            type: integer
+            description: A unique identifier for the delivery location.
+            filterable: true
+            sortable: true
+          self:
+            type: string
+            description: A unique reference to the delivery location resource.
+            format: uri
+      dueDate:
+        type: string
+        description: >-
+          The date the invoice is due for payment. Only used if the terms of
+          payment is of type 'duedate', in which case it is mandatory. Format
+          according to ISO-8601 (YYYY-MM-DD).
+        format: full-date
+        pattern: \d{4}-\d{2}-\d{2}
+      exchangeRate:
+        type: number
+        description: >-
+          The exchange rate between the invoice currency and the base currency
+          of the agreement. The exchange rate expresses how much it will cost in
+          base currency to buy 100 units of the invoice currency.
+        filterable: true
+        maxDecimal: 6
+        sortable: true
+      grossAmount:
+        type: number
+        description: >-
+          The total invoice amount in the invoice currency after all taxes and
+          discounts have been applied. For a credit note this amount will be
+          negative.
+        maxDecimal: 2
+      grossAmountInBaseCurrency:
+        type: number
+        description: >-
+          The total invoice amount in the base currency of the agreement after
+          all taxes and discounts have been applied. For a credit note this
+          amount will be negative.
+        maxDecimal: 2
+      layout:
+        type: object
+        description: Layout to be applied for this invoice.
+        properties:
+          layoutNumber:
+            type: integer
+            description: The unique identifier of the layout.
+          self:
+            type: string
+            description: A unique link reference to the layout item.
+            format: uri
+      lines:
+        type: array
+        description: An array containing the specific invoice lines.
+        items:
+          type: object
+          description: An array of the invoice lines that make up the invoice.
+          properties:
+            deliveryDate:
+              type: string
+              description: >-
+                Invoice delivery date. The date is formatted according to
+                ISO-8601.
+              filterable: true
+              format: full-date
+              pattern: \d{4}-\d{2}-\d{2}
+              sortable: true
+            departmentalDistribution:
+              type: object
+              properties:
+                departmentalDistributionNumber:
+                  type: integer
+                  description: A unique identifier of the departmental distribution.
+                  minimum: 1
+                self:
+                  type: string
+                  description: >-
+                    A unique reference to the departmental distribution
+                    resource.
+                  format: uri
+            description:
+              type: string
+              description: A description of the product or service sold.
+            discountPercentage:
+              type: number
+              description: A line discount expressed as a percentage.
+              maxDecimal: 2
+            lineNumber:
+              type: integer
+              description: The line number is a unique number within the invoice.
+              minimum: 0
+            product:
+              type: object
+              description: The product or service offered on the invoice line.
+              properties:
+                productNumber:
+                  type: string
+                  description: >-
+                    The unique product number. This can be a stock keeping unit
+                    identifier (SKU).
+                self:
+                  type: string
+                  description: A unique reference to the product resource.
+                  format: uri
+            quantity:
+              type: number
+              description: The number of units of goods on the invoice line.
+              maxDecimal: 2
+            sortKey:
+              type: integer
+              description: >-
+                A sort key used to sort the lines in ascending order within the
+                invoice.
+              minimum: 0
+            totalNetAmount:
+              type: number
+              description: >-
+                The total invoice line amount in the invoice currency before all
+                taxes and discounts have been applied. For a credit note this
+                amount will be negative.
+              maxDecimal: 2
+            unit:
+              type: object
+              description: The unit of measure applied to the invoice line.
+              properties:
+                name:
+                  type: string
+                  description: >-
+                    The name of the unit (e.g. 'kg' for weight or 'l' for
+                    volume).
+                self:
+                  type: string
+                  description: A unique reference to the unit resource.
+                  format: uri
+                unitNumber:
+                  type: integer
+                  description: The unique identifier of the unit.
+                  minimum: 0
+            unitCostPrice:
+              type: number
+              description: >-
+                The cost price of 1 unit of the goods or services in the invoice
+                currency.
+              maxDecimal: 2
+            unitNetPrice:
+              type: number
+              description: >-
+                The price of 1 unit of the goods or services on the invoice line
+                in the invoice currency.
+              maxDecimal: 2
+            vatAmount:
+              type: number
+              description: >-
+                The total amount of VAT on the invoice line in the invoice
+                currency. This will have the same sign as total net amount
+              maxDecimal: 2
+            vatRate:
+              type: number
+              description: The VAT rate in % used to calculate the vat amount on this line.
+              maxDecimal: 6
+        title: Invoice lines
+      netAmount:
+        type: number
+        description: >-
+          The total invoice amount in the invoice currency before all taxes and
+          discounts have been applied. For a credit note this amount will be
+          negative.
+        maxDecimal: 2
+      netAmountInBaseCurrency:
+        type: number
+        description: >-
+          The total invoice amount in the base currency of the agreement before
+          all taxes and discounts have been applied. For a credit note this
+          amount will be negative.
+        maxDecimal: 2
+      notes:
+        type: object
+        description: Notes on the invoice.
+        properties:
+          heading:
+            type: string
+            description: The invoice heading. Usually displayed at the top of the invoice.
+            filterable: true
+            sortable: true
+          textLine1:
+            type: string
+            description: >-
+              The first line of supplementary text on the invoice. This is
+              usually displayed right under the heading in a smaller font.
+            filterable: true
+            sortable: true
+          textLine2:
+            type: string
+            description: >-
+              The second line of supplementary text in the notes on the invoice.
+              This is usually displayed as a footer on the invoice.
+            filterable: true
+            sortable: true
+      orderNumber:
+        type:
+          - "null"
+          - integer
+        description: The order number related to the invoice
+      paymentTerms:
+        type: object
+        description: The terms of payment for the invoice.
+        properties:
+          daysOfCredit:
+            type: integer
+            description: >-
+              The number of days of credit on the invoice. This field is only
+              valid if terms of payment is not of type 'duedate
+            minimum: 0
+          name:
+            type: string
+            description: The name of the payment terms.
+          paymentTermsNumber:
+            type: integer
+            description: A unique identifier of the payment term.
+            filterable: true
+            minimum: 0
+            sortable: true
+          paymentTermsType:
+            type: string
+            description: The type of payment term.
+          self:
+            type: string
+            description: A unique reference to the payment term resource.
+            format: uri
+      pdf:
+        type: object
+        description: References a pdf representation of this invoice.
+        properties:
+          self:
+            type: string
+            description: >-
+              The unique reference of the pdf representation for this booked
+              invoice.
+            format: uri
+      project:
+        type: object
+        description: Details of the project linked to the invoice
+        properties:
+          projectNumber:
+            type: integer
+            description: A unique identifier of the project.
+            minimum: 1
+          self:
+            type: string
+            description: A unique reference to the project resource.
+            format: uri
+      recipient:
+        type: object
+        description: >-
+          The actual recipient of the invoice. This may be the same info found
+          on the customer (and will probably be so in most cases) but it may
+          also be a different recipient. For instance, the customer placing the
+          order may be ACME Headquarters, but the recipient of the invoice may
+          be ACME IT.
+        properties:
+          address:
+            type: string
+            description: The street address of the actual recipient.
+            empty: true
+            filterable: true
+            sortable: true
+          attention:
             type: object
-            description: Notes on the invoice.
+            description: The person to whom this invoice is addressed.
             properties:
-              heading:
-                type: string
-                filterable: true
-                sortable: true
-                description:
-                  The invoice heading. Usually displayed at the top of
-                  the invoice.
-              textLine1:
-                type: string
-                filterable: true
-                sortable: true
-                description:
-                  The first line of supplementary text on the invoice.
-                  This is usually displayed right under the heading in a smaller font.
-              textLine2:
+              customerContactNumber:
+                type: integer
+                description: Unique identifier of the customer employee.
+              self:
                 type: string
-                filterable: true
-                sortable: true
-                description:
-                  The second line of supplementary text in the notes on
-                  the invoice. This is usually displayed as a footer on the invoice.
-          references:
+                description: A unique reference to the customer employee.
+                format: uri
+          city:
+            type: string
+            description: The city of the actual recipient.
+            empty: true
+            filterable: true
+            sortable: true
+          country:
+            type: string
+            description: The country of the actual recipient.
+            filterable: true
+            sortable: true
+          cvr:
+            type: string
+            description: >-
+              The Corporate Identification Number of the recipient for example
+              CVR in Denmark.
+          ean:
+            type: string
+            description: The 'European Article Number' of the actual recipient.
+            filterable: true
+            sortable: true
+          name:
+            type: string
+            description: The name of the actual recipient.
+            empty: true
+            filterable: true
+            sortable: true
+          publicEntryNumber:
+            type: string
+            description: The public entry number of the actual recipient.
+            filterable: true
+            sortable: true
+          vatZone:
             type: object
-            description: Customer and company references related to this invoice.
+            description: Recipient vat zone.
             properties:
-              customerContact:
-                type: object
-                description:
-                  The customer contact is a reference to the employee at
-                  the customer to contact regarding the invoice.
-                properties:
-                  customerContactNumber:
-                    type: integer
-                    minimum: 0
-                    description: Unique identifier of the customer contact.
-                  self:
-                    type: string
-                    format: uri
-                    description: A unique reference to the customer contact resource.
-              salesPerson:
-                type: object
-                description:
-                  The sales person is a reference to the employee who sold
-                  the goods on the invoice. This is also the person who is credited
-                  with this sale in reports.
-                properties:
-                  employeeNumber:
-                    type: integer
-                    minimum: 1
-                    filterable: true
-                    sortable: true
-                    description: Unique identifier of the employee.
-                  self:
-                    type: string
-                    format: uri
-                    description: A unique reference to the employee resource.
-              vendorReference:
-                type: object
-                description: A reference to any second employee involved in the sale.
-                properties:
-                  employeeNumber:
-                    type: integer
-                    minimum: 1
-                    filterable: true
-                    sortable: true
-                    description: Unique identifier of the employee.
-                  self:
-                    type: string
-                    format: uri
-                    description: A unique reference to the employee resource.
-              other:
+              self:
                 type: string
+                description: A unique reference to the vat zone.
+                format: uri
+              vatZoneNumber:
+                type: integer
+                description: Unique identifier of the vat zone.
                 filterable: true
                 sortable: true
-                description:
-                  A text field that can be used to save any custom reference
-                  on the invoice.
-          pdf:
+          zip:
+            type: string
+            description: The zip code of the actual recipient.
+            empty: true
+            filterable: true
+            sortable: true
+      references:
+        type: object
+        description: Customer and company references related to this invoice.
+        properties:
+          customerContact:
             type: object
-            description: References a pdf representation of this invoice.
+            description: >-
+              The customer contact is a reference to the employee at the
+              customer to contact regarding the invoice.
             properties:
+              customerContactNumber:
+                type: integer
+                description: Unique identifier of the customer contact.
+                minimum: 0
               self:
                 type: string
+                description: A unique reference to the customer contact resource.
                 format: uri
-                description:
-                  The unique reference of the pdf representation for this
-                  booked invoice.
-          layout:
+          other:
+            type: string
+            description: >-
+              A text field that can be used to save any custom reference on the
+              invoice.
+            filterable: true
+            sortable: true
+          salesPerson:
             type: object
-            description: Layout to be applied for this invoice.
+            description: >-
+              The sales person is a reference to the employee who sold the goods
+              on the invoice. This is also the person who is credited with this
+              sale in reports.
             properties:
-              layoutNumber:
+              employeeNumber:
                 type: integer
-                description: The unique identifier of the layout.
+                description: Unique identifier of the employee.
+                filterable: true
+                minimum: 1
+                sortable: true
               self:
                 type: string
+                description: A unique reference to the employee resource.
                 format: uri
-                description: A unique link reference to the layout item.
-          project:
-            description: Details of the project linked to the invoice
+          vendorReference:
             type: object
+            description: A reference to any second employee involved in the sale.
             properties:
-              projectNumber:
+              employeeNumber:
                 type: integer
+                description: Unique identifier of the employee.
+                filterable: true
                 minimum: 1
-                description: A unique identifier of the project.
+                sortable: true
               self:
                 type: string
+                description: A unique reference to the employee resource.
                 format: uri
-                description: A unique reference to the project resource.
-          lines:
-            title: Invoice lines
-            type: array
-            description: An array containing the specific invoice lines.
-            items:
-              type: object
-              description: An array of the invoice lines that make up the invoice.
-              properties:
-                lineNumber:
-                  type: integer
-                  description: The line number is a unique number within the invoice.
-                  minimum: 0
-                sortKey:
-                  type: integer
-                  description:
-                    A sort key used to sort the lines in ascending order
-                    within the invoice.
-                  minimum: 0
-                description:
-                  type: string
-                  description: A description of the product or service sold.
-                deliveryDate:
-                  type: string
-                  format: full-date
-                  pattern: \d{4}-\d{2}-\d{2}
-                  filterable: true
-                  sortable: true
-                  description:
-                    Invoice delivery date. The date is formatted according
-                    to ISO-8601.
-                quantity:
-                  type: number
-                  maxDecimal: 2
-                  description: The number of units of goods on the invoice line.
-                unitNetPrice:
-                  type: number
-                  maxDecimal: 2
-                  description:
-                    The price of 1 unit of the goods or services on the
-                    invoice line in the invoice currency.
-                discountPercentage:
-                  type: number
-                  maxDecimal: 2
-                  description: A line discount expressed as a percentage.
-                unitCostPrice:
-                  type: number
-                  maxDecimal: 2
-                  description:
-                    The cost price of 1 unit of the goods or services in
-                    the invoice currency.
-                vatRate:
-                  type: number
-                  maxDecimal: 6
-                  description:
-                    The VAT rate in % used to calculate the vat amount
-                    on this line.
-                vatAmount:
-                  type: number
-                  maxDecimal: 2
-                  description:
-                    The total amount of VAT on the invoice line in the
-                    invoice currency. This will have the same sign as total net amount
-                totalNetAmount:
-                  type: number
-                  maxDecimal: 2
-                  description:
-                    The total invoice line amount in the invoice currency
-                    before all taxes and discounts have been applied. For a credit
-                    note this amount will be negative.
-                unit:
-                  type: object
-                  description: The unit of measure applied to the invoice line.
-                  properties:
-                    unitNumber:
-                      type: integer
-                      description: The unique identifier of the unit.
-                      minimum: 0
-                    name:
-                      type: string
-                      description:
-                        The name of the unit (e.g. 'kg' for weight or 'l'
-                        for volume).
-                    self:
-                      type: string
-                      format: uri
-                      description: A unique reference to the unit resource.
-                product:
-                  type: object
-                  description: The product or service offered on the invoice line.
-                  properties:
-                    productNumber:
-                      type: string
-                      description:
-                        The unique product number. This can be a stock
-                        keeping unit identifier (SKU).
-                    self:
-                      type: string
-                      format: uri
-                      description: A unique reference to the product resource.
-                departmentalDistribution:
-                  type: object
-                  properties:
-                    departmentalDistributionNumber:
-                      type: integer
-                      minimum: 1
-                      description: A unique identifier of the departmental distribution.
-                    self:
-                      type: string
-                      format: uri
-                      description:
-                        A unique reference to the departmental distribution
-                        resource.
-          sent:
-            type: string
-            format: uri
-            description:
-              A convenience link to see if the invoice has been sent or
-              not.
-          self:
-            type: string
-            format: uri
-            description: The unique self reference of the booked invoice.
-streams:
-  - "#/definitions/accounts_stream"
-  - "#/definitions/customers_stream"
-  - "#/definitions/products_stream"
-  - "#/definitions/invoices_total_stream"
-  - "#/definitions/invoices_paid_stream"
-  - "#/definitions/invoices_booked_stream"
-  - "#/definitions/invoices_booked_document_stream"
-
-check:
-  type: CheckStream
-  stream_names:
-    - "accounts"
-
-spec:
-  type: Spec
-  documentationUrl: https://docs.airbyte.com/integrations/sources/visma-economic
-  connection_specification:
-    $schema: http://json-schema.org/draft-07/schema#
-    title: Visma E-conomic Spec
-    type: object
-    required:
-      - app_secret_token
-      - agreement_grant_token
-    properties:
-      app_secret_token:
-        title: App Secret Token
+      remainder:
+        type: number
+        description: Remaining amount to be paid.
+        maxDecimal: 2
+        readonly: true
+      remainderInBaseCurrency:
+        type: number
+        description: Remaining amount to be paid in base currency.
+        maxDecimal: 2
+        readonly: true
+      roundingAmount:
+        type: number
+        description: The total rounding error, if any, on the invoice in base currency.
+        maxDecimal: 2
+      self:
         type: string
-        description: Identification token for app accessing data
-        airbyte_secret: true
-      agreement_grant_token:
-        title: Agreement Grant Token
+        description: The unique self reference of the booked invoice.
+        format: uri
+      sent:
         type: string
-        description: Identifier for the grant issued by an agreement
-        airbyte_secret: true
+        description: A convenience link to see if the invoice has been sent or not.
+        format: uri
+      vatAmount:
+        type: number
+        description: >-
+          The total amount of VAT on the invoice in the invoice currency. This
+          will have the same sign as net amount
+        maxDecimal: 2
+    title: Booked invoice schema
```

### Comparing `airbyte_source_visma_economic-0.2.4/PKG-INFO` & `airbyte_source_visma_economic-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-visma-economic
-Version: 0.2.4
+Version: 0.2.5
 Summary: Source implementation for Visma Economic.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -15,96 +15,110 @@
 Requires-Dist: airbyte-cdk (==0.80.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/visma-economic
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Visma-Economic source connector
 
-
 This is the repository for the Visma-Economic source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/visma-economic).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/visma-economic)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_visma_economic/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-visma-economic spec
 poetry run source-visma-economic check --config secrets/config.json
 poetry run source-visma-economic discover --config secrets/config.json
 poetry run source-visma-economic read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-visma-economic build
 ```
 
 An image will be available on your host with the tag `airbyte/source-visma-economic:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-visma-economic:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-visma-economic:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-visma-economic:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-visma-economic:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-visma-economic test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-visma-economic test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/visma-economic.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+
```

