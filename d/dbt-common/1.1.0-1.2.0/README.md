# Comparing `tmp/dbt_common-1.1.0.tar.gz` & `tmp/dbt_common-1.2.0.tar.gz`

## Comparing `dbt_common-1.1.0.tar` & `dbt_common-1.2.0.tar`

### file list

```diff
@@ -1,103 +1,104 @@
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 dbt_common-1.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 dbt_common-1.1.0/codecov.yml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/__init__.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/constants.py
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/context.py
--rw-r--r--   0        0        0     5523 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/dataclass_schema.py
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/helper_types.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/invocation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/py.typed
--rw-r--r--   0        0        0     7002 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/record.py
--rw-r--r--   0        0        0    13954 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/semver.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/tests.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/ui.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/clients/__init__.py
--rw-r--r--   0        0        0    12947 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/clients/_jinja_blocks.py
--rw-r--r--   0        0        0     9124 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/clients/agate_helper.py
--rw-r--r--   0        0        0    18502 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/clients/jinja.py
--rw-r--r--   0        0        0    23014 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/clients/system.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/contracts/__init__.py
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/contracts/constraints.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/contracts/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/contracts/config/__init__.py
--rw-r--r--   0        0        0     8356 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/contracts/config/base.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/contracts/config/materialization.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/contracts/config/metadata.py
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/contracts/config/properties.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/events/README.md
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/events/__init__.py
--rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/events/base_types.py
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/events/contextvars.py
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/events/event_handler.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/events/event_manager.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/events/event_manager_client.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/events/format.py
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/events/functions.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/events/helpers.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/events/interfaces.py
--rw-r--r--   0        0        0     6728 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/events/logger.py
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/events/types.proto
--rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/events/types.py
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/events/types_pb2.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/exceptions/__init__.py
--rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/exceptions/base.py
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/exceptions/cache.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/exceptions/connection.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/exceptions/contracts.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/exceptions/events.py
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/exceptions/jinja.py
--rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/exceptions/macros.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/exceptions/system.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/utils/__init__.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/utils/casting.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/utils/connection.py
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/utils/dict.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/utils/encoding.py
--rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/utils/executor.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/utils/formatting.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 dbt_common-1.1.0/dbt_common/utils/jinja.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 dbt_common-1.1.0/docs/README.md
--rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 dbt_common-1.1.0/docs/arch/adr-0001-build-tooling.md
--rw-r--r--   0        0        0     4829 2020-02-02 00:00:00.000000 dbt_common-1.1.0/docs/guides/record_replay.md
--rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/agate/__init__.pyi
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/agate/data_types.pyi
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/colorama/__init__.pyi
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/isodate/__init__.pyi
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/mashumaro/__init__.pyi
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/mashumaro/config.pyi
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/mashumaro/dialect.pyi
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/mashumaro/exceptions.pyi
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/mashumaro/helper.pyi
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/mashumaro/types.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/mashumaro/core/__init__.pyi
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/mashumaro/core/const.pyi
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/mashumaro/core/helpers.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/mashumaro/core/meta/__init__.pyi
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/mashumaro/core/meta/helpers.pyi
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/mashumaro/core/meta/mixin.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/mashumaro/core/meta/code/__init__.pyi
--rw-r--r--   0        0        0     6150 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/mashumaro/core/meta/code/builder.pyi
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/mashumaro/core/meta/code/lines.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/mashumaro/core/meta/types/__init__.pyi
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/mashumaro/core/meta/types/common.pyi
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/mashumaro/core/meta/types/pack.pyi
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/mashumaro/core/meta/types/unpack.pyi
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/mashumaro/jsonschema/__init__.pyi
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/mashumaro/jsonschema/annotations.pyi
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/mashumaro/jsonschema/builder.pyi
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/mashumaro/jsonschema/dialects.pyi
--rw-r--r--   0        0        0     5914 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/mashumaro/jsonschema/models.pyi
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/mashumaro/jsonschema/schema.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/mashumaro/mixins/__init__.pyi
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/mashumaro/mixins/dict.pyi
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/mashumaro/mixins/json.pyi
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/mashumaro/mixins/msgpack.pyi
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/mashumaro/mixins/orjson.pyi
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/mashumaro/mixins/toml.pyi
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 dbt_common-1.1.0/third-party-stubs/mashumaro/mixins/yaml.pyi
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 dbt_common-1.1.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dbt_common-1.1.0/LICENSE
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 dbt_common-1.1.0/README.md
--rw-r--r--   0        0        0     4881 2020-02-02 00:00:00.000000 dbt_common-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 dbt_common-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 dbt_common-1.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 dbt_common-1.2.0/codecov.yml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/__init__.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/constants.py
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/context.py
+-rw-r--r--   0        0        0     5523 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/dataclass_schema.py
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/helper_types.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/invocation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/py.typed
+-rw-r--r--   0        0        0     8204 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/record.py
+-rw-r--r--   0        0        0    13954 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/semver.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/tests.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/ui.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/clients/__init__.py
+-rw-r--r--   0        0        0    12947 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/clients/_jinja_blocks.py
+-rw-r--r--   0        0        0     9124 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/clients/agate_helper.py
+-rw-r--r--   0        0        0    18502 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/clients/jinja.py
+-rw-r--r--   0        0        0    23014 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/clients/system.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/contracts/__init__.py
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/contracts/constraints.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/contracts/metadata.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/contracts/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/contracts/config/__init__.py
+-rw-r--r--   0        0        0     8356 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/contracts/config/base.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/contracts/config/materialization.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/contracts/config/metadata.py
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/contracts/config/properties.py
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/events/README.md
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/events/__init__.py
+-rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/events/base_types.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/events/contextvars.py
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/events/event_handler.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/events/event_manager.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/events/event_manager_client.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/events/format.py
+-rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/events/functions.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/events/helpers.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/events/interfaces.py
+-rw-r--r--   0        0        0     6728 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/events/logger.py
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/events/types.proto
+-rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/events/types.py
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/events/types_pb2.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/exceptions/__init__.py
+-rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/exceptions/base.py
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/exceptions/cache.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/exceptions/connection.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/exceptions/contracts.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/exceptions/events.py
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/exceptions/jinja.py
+-rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/exceptions/macros.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/exceptions/system.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/utils/__init__.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/utils/casting.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/utils/connection.py
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/utils/dict.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/utils/encoding.py
+-rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/utils/executor.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/utils/formatting.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 dbt_common-1.2.0/dbt_common/utils/jinja.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 dbt_common-1.2.0/docs/README.md
+-rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 dbt_common-1.2.0/docs/arch/adr-0001-build-tooling.md
+-rw-r--r--   0        0        0     5463 2020-02-02 00:00:00.000000 dbt_common-1.2.0/docs/guides/record_replay.md
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/agate/__init__.pyi
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/agate/data_types.pyi
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/colorama/__init__.pyi
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/isodate/__init__.pyi
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/mashumaro/__init__.pyi
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/mashumaro/config.pyi
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/mashumaro/dialect.pyi
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/mashumaro/exceptions.pyi
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/mashumaro/helper.pyi
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/mashumaro/types.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/mashumaro/core/__init__.pyi
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/mashumaro/core/const.pyi
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/mashumaro/core/helpers.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/mashumaro/core/meta/__init__.pyi
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/mashumaro/core/meta/helpers.pyi
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/mashumaro/core/meta/mixin.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/mashumaro/core/meta/code/__init__.pyi
+-rw-r--r--   0        0        0     6150 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/mashumaro/core/meta/code/builder.pyi
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/mashumaro/core/meta/code/lines.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/mashumaro/core/meta/types/__init__.pyi
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/mashumaro/core/meta/types/common.pyi
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/mashumaro/core/meta/types/pack.pyi
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/mashumaro/core/meta/types/unpack.pyi
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/mashumaro/jsonschema/__init__.pyi
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/mashumaro/jsonschema/annotations.pyi
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/mashumaro/jsonschema/builder.pyi
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/mashumaro/jsonschema/dialects.pyi
+-rw-r--r--   0        0        0     5914 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/mashumaro/jsonschema/models.pyi
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/mashumaro/jsonschema/schema.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/mashumaro/mixins/__init__.pyi
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/mashumaro/mixins/dict.pyi
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/mashumaro/mixins/json.pyi
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/mashumaro/mixins/msgpack.pyi
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/mashumaro/mixins/orjson.pyi
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/mashumaro/mixins/toml.pyi
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 dbt_common-1.2.0/third-party-stubs/mashumaro/mixins/yaml.pyi
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 dbt_common-1.2.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dbt_common-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 dbt_common-1.2.0/README.md
+-rw-r--r--   0        0        0     4881 2020-02-02 00:00:00.000000 dbt_common-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 dbt_common-1.2.0/PKG-INFO
```

### Comparing `dbt_common-1.1.0/dbt_common/context.py` & `dbt_common-1.2.0/dbt_common/context.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/dataclass_schema.py` & `dbt_common-1.2.0/dbt_common/dataclass_schema.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/helper_types.py` & `dbt_common-1.2.0/dbt_common/helper_types.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/record.py` & `dbt_common-1.2.0/dbt_common/record.py`

 * *Files 12% similar despite different names*

```diff
@@ -55,22 +55,26 @@
 
     pass
 
 
 class RecorderMode(Enum):
     RECORD = 1
     REPLAY = 2
+    RECORD_QUERIES = 3
 
 
 class Recorder:
     _record_cls_by_name: Dict[str, Type] = {}
     _record_name_by_params_name: Dict[str, str] = {}
 
-    def __init__(self, mode: RecorderMode, recording_path: Optional[str] = None) -> None:
+    def __init__(
+        self, mode: RecorderMode, types: Optional[List], recording_path: Optional[str] = None
+    ) -> None:
         self.mode = mode
+        self.types = types
         self._records_by_type: Dict[str, List[Record]] = {}
         self._replay_diffs: List["Diff"] = []
 
         if recording_path is not None:
             self._records_by_type = self.load(recording_path)
 
     @classmethod
@@ -114,21 +118,22 @@
     def load(cls, file_name: str) -> Dict[str, List[Record]]:
         with open(file_name) as file:
             loaded_dct = json.load(file)
 
         records_by_type: Dict[str, List[Record]] = {}
 
         for record_type_name in loaded_dct:
+            # TODO: this breaks with QueryRecord on replay since it's
+            # not in common so isn't part of cls._record_cls_by_name yet
             record_cls = cls._record_cls_by_name[record_type_name]
             rec_list = []
             for record_dct in loaded_dct[record_type_name]:
                 rec = record_cls.from_dict(record_dct)
                 rec_list.append(rec)  # type: ignore
             records_by_type[record_type_name] = rec_list
-
         return records_by_type
 
     def expect_record(self, params: Any) -> Any:
         record = self.pop_matching_record(params)
 
         if record is None:
             raise Exception()
@@ -143,25 +148,52 @@
         )
 
     def print_diffs(self) -> None:
         print(repr(self._replay_diffs))
 
 
 def get_record_mode_from_env() -> Optional[RecorderMode]:
-    replay_val = os.environ.get("DBT_REPLAY")
-    if replay_val is not None and replay_val != "0" and replay_val.lower() != "false":
-        return RecorderMode.REPLAY
+    """
+    Get the record mode from the environment variables.
+
+    If the mode is not set to 'RECORD' or 'REPLAY', return None.
+    Expected format: 'DBT_RECORDER_MODE=RECORD'
+    """
+    record_mode = os.environ.get("DBT_RECORDER_MODE")
 
-    record_val = os.environ.get("DBT_RECORD")
-    if record_val is not None and record_val != "0" and record_val.lower() != "false":
+    if record_mode is None:
+        return None
+
+    if record_mode.lower() == "record":
         return RecorderMode.RECORD
+    # replaying requires a file path, otherwise treat as noop
+    elif record_mode.lower() == "replay" and os.environ.get("DBT_RECORDER_FILE_PATH") is not None:
+        return RecorderMode.REPLAY
 
+    # if you don't specify record/replay it's a noop
     return None
 
 
+def get_record_types_from_env() -> Optional[List]:
+    """
+    Get the record subset from the environment variables.
+
+    If no types are provided, there will be no filtering.
+    Invalid types will be ignored.
+    Expected format: 'DBT_RECORDER_TYPES=QueryRecord,FileLoadRecord,OtherRecord'
+    """
+    record_types_str = os.environ.get("DBT_RECORDER_TYPES")
+
+    # if all is specified we don't want any type filtering
+    if record_types_str is None or record_types_str.lower == "all":
+        return None
+
+    return record_types_str.split(",")
+
+
 def record_function(record_type, method=False, tuple_result=False):
     def record_function_inner(func_to_record):
         # To avoid runtime overhead and other unpleasantness, we only apply the
         # record/replay decorator if a relevant env var is set.
         if get_record_mode_from_env() is None:
             return func_to_record
 
@@ -172,14 +204,17 @@
                 recorder = get_invocation_context().recorder
             except LookupError:
                 pass
 
             if recorder is None:
                 return func_to_record(*args, **kwargs)
 
+            if recorder.types is not None and record_type.__name__ not in recorder.types:
+                return func_to_record(*args, **kwargs)
+
             # For methods, peel off the 'self' argument before calling the
             # params constructor.
             param_args = args[1:] if method else args
 
             params = record_type.params_cls(*param_args, **kwargs)
 
             include = True
```

### Comparing `dbt_common-1.1.0/dbt_common/semver.py` & `dbt_common-1.2.0/dbt_common/semver.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/ui.py` & `dbt_common-1.2.0/dbt_common/ui.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/clients/_jinja_blocks.py` & `dbt_common-1.2.0/dbt_common/clients/_jinja_blocks.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/clients/agate_helper.py` & `dbt_common-1.2.0/dbt_common/clients/agate_helper.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/clients/jinja.py` & `dbt_common-1.2.0/dbt_common/clients/jinja.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/clients/system.py` & `dbt_common-1.2.0/dbt_common/clients/system.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/contracts/constraints.py` & `dbt_common-1.2.0/dbt_common/contracts/constraints.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/contracts/util.py` & `dbt_common-1.2.0/dbt_common/contracts/util.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/contracts/config/base.py` & `dbt_common-1.2.0/dbt_common/contracts/config/base.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/contracts/config/metadata.py` & `dbt_common-1.2.0/dbt_common/contracts/config/metadata.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/contracts/config/properties.py` & `dbt_common-1.2.0/dbt_common/contracts/config/properties.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/events/README.md` & `dbt_common-1.2.0/dbt_common/events/README.md`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/events/base_types.py` & `dbt_common-1.2.0/dbt_common/events/base_types.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/events/contextvars.py` & `dbt_common-1.2.0/dbt_common/events/contextvars.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/events/event_handler.py` & `dbt_common-1.2.0/dbt_common/events/event_handler.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/events/event_manager.py` & `dbt_common-1.2.0/dbt_common/events/event_manager.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/events/event_manager_client.py` & `dbt_common-1.2.0/dbt_common/events/event_manager_client.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/events/format.py` & `dbt_common-1.2.0/dbt_common/events/format.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/events/functions.py` & `dbt_common-1.2.0/dbt_common/events/functions.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/events/logger.py` & `dbt_common-1.2.0/dbt_common/events/logger.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/events/types.proto` & `dbt_common-1.2.0/dbt_common/events/types.proto`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/events/types.py` & `dbt_common-1.2.0/dbt_common/events/types.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/events/types_pb2.py` & `dbt_common-1.2.0/dbt_common/events/types_pb2.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/exceptions/base.py` & `dbt_common-1.2.0/dbt_common/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/exceptions/cache.py` & `dbt_common-1.2.0/dbt_common/exceptions/cache.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/exceptions/contracts.py` & `dbt_common-1.2.0/dbt_common/exceptions/contracts.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/exceptions/jinja.py` & `dbt_common-1.2.0/dbt_common/exceptions/jinja.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/exceptions/macros.py` & `dbt_common-1.2.0/dbt_common/exceptions/macros.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/exceptions/system.py` & `dbt_common-1.2.0/dbt_common/exceptions/system.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/utils/__init__.py` & `dbt_common-1.2.0/dbt_common/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/utils/casting.py` & `dbt_common-1.2.0/dbt_common/utils/casting.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/utils/connection.py` & `dbt_common-1.2.0/dbt_common/utils/connection.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/utils/dict.py` & `dbt_common-1.2.0/dbt_common/utils/dict.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/utils/encoding.py` & `dbt_common-1.2.0/dbt_common/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/utils/executor.py` & `dbt_common-1.2.0/dbt_common/utils/executor.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/dbt_common/utils/jinja.py` & `dbt_common-1.2.0/dbt_common/utils/jinja.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/docs/arch/adr-0001-build-tooling.md` & `dbt_common-1.2.0/docs/arch/adr-0001-build-tooling.md`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/docs/guides/record_replay.md` & `dbt_common-1.2.0/docs/guides/record_replay.md`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,30 @@
 ```
 When record and replay are disabled, this decorator is a no-op, but when one of them is enabled it implements the behaviors described above.  
   
 Note also the `LoadFileRecord` class passed as a parameter to this decorator. This is (and must be) a class with the two properties `params_cls`, and `result_cls` specified. The class itself is registered with the record/replay mechanism by annotating it with `@Recorder.register_record_type`.  
   
 The final detail needed is to define the classes specified by `params_cls` and `result_cls`, which must be dataclasses with properties whose order and names correspond to the parameters passed to the recorded function. In this case those are the `LoadFileParams` and `LoadFileResult` classes, respectively.
 
-With these decorators applied and classes defined, dbt is able to record all file access during a run, and mock out the accesses during replay, isolating dbt from actually loading files. At least it would if dbt only used this function for all file access, which is only mostly true. We hope to continue improving the usefulness of this mechanism by adding more recorded functions and routing more operations through them.  
+With these decorators applied and classes defined, dbt is able to record all file access during a run, and mock out the accesses during replay, isolating dbt from actually loading files. At least it would if dbt only used this function for all file access, which is only mostly true. We hope to continue improving the usefulness of this mechanism by adding more recorded functions and routing more operations through them.
+
+## How to record/replay
+If `DBT_RECORDER_MODE` is not `replay` or `record`, case insensitive, this is a no-op.  Invalid values are ignored and do not throw exceptions.
+
+`DBT_RECODER_TYPES` is optional.  It indicates which types to filter the results by and expects a list of strings values for the `Record` subclasses.  Any invalid types will be ignored.  `all` is a valid type and behaves the same as not populating the env var.
+
+
+```bash
+DBT_RECORDER_MODE=record DBT_RECODER_TYPES=QueryRecord,GetEnvRecord dbt run
+```
+
+replay need the file to replay
+```bash
+DBT_RECORDER_MODE=replay DBT_RECORDER_FILE_PATH=recording.json dbt run
+```
 
 ## Final Thoughts
   
 We are aware of the potential limitations of this mechanism, since it makes several strong assumptions, not least of which are:
   
 1. Every important interaction with an external system can be modeled as a function call.  
 2. Every important interaction can be recorded without creating an impractically large output file.
```

### Comparing `dbt_common-1.1.0/third-party-stubs/agate/__init__.pyi` & `dbt_common-1.2.0/third-party-stubs/agate/__init__.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/third-party-stubs/agate/data_types.pyi` & `dbt_common-1.2.0/third-party-stubs/agate/data_types.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/third-party-stubs/mashumaro/config.pyi` & `dbt_common-1.2.0/third-party-stubs/mashumaro/config.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/third-party-stubs/mashumaro/exceptions.pyi` & `dbt_common-1.2.0/third-party-stubs/mashumaro/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/third-party-stubs/mashumaro/helper.pyi` & `dbt_common-1.2.0/third-party-stubs/mashumaro/helper.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/third-party-stubs/mashumaro/types.pyi` & `dbt_common-1.2.0/third-party-stubs/mashumaro/types.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/third-party-stubs/mashumaro/core/meta/helpers.pyi` & `dbt_common-1.2.0/third-party-stubs/mashumaro/core/meta/helpers.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/third-party-stubs/mashumaro/core/meta/code/builder.pyi` & `dbt_common-1.2.0/third-party-stubs/mashumaro/core/meta/code/builder.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/third-party-stubs/mashumaro/core/meta/types/common.pyi` & `dbt_common-1.2.0/third-party-stubs/mashumaro/core/meta/types/common.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/third-party-stubs/mashumaro/core/meta/types/unpack.pyi` & `dbt_common-1.2.0/third-party-stubs/mashumaro/core/meta/types/unpack.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/third-party-stubs/mashumaro/jsonschema/annotations.pyi` & `dbt_common-1.2.0/third-party-stubs/mashumaro/jsonschema/annotations.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/third-party-stubs/mashumaro/jsonschema/builder.pyi` & `dbt_common-1.2.0/third-party-stubs/mashumaro/jsonschema/builder.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/third-party-stubs/mashumaro/jsonschema/dialects.pyi` & `dbt_common-1.2.0/third-party-stubs/mashumaro/jsonschema/dialects.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/third-party-stubs/mashumaro/jsonschema/models.pyi` & `dbt_common-1.2.0/third-party-stubs/mashumaro/jsonschema/models.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/third-party-stubs/mashumaro/jsonschema/schema.pyi` & `dbt_common-1.2.0/third-party-stubs/mashumaro/jsonschema/schema.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/third-party-stubs/mashumaro/mixins/dict.pyi` & `dbt_common-1.2.0/third-party-stubs/mashumaro/mixins/dict.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/third-party-stubs/mashumaro/mixins/json.pyi` & `dbt_common-1.2.0/third-party-stubs/mashumaro/mixins/json.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/third-party-stubs/mashumaro/mixins/msgpack.pyi` & `dbt_common-1.2.0/third-party-stubs/mashumaro/mixins/msgpack.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/third-party-stubs/mashumaro/mixins/orjson.pyi` & `dbt_common-1.2.0/third-party-stubs/mashumaro/mixins/orjson.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/third-party-stubs/mashumaro/mixins/toml.pyi` & `dbt_common-1.2.0/third-party-stubs/mashumaro/mixins/toml.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/third-party-stubs/mashumaro/mixins/yaml.pyi` & `dbt_common-1.2.0/third-party-stubs/mashumaro/mixins/yaml.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/.gitignore` & `dbt_common-1.2.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -153,8 +153,8 @@
 cython_debug/
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-#.idea/
+.idea/
```

### Comparing `dbt_common-1.1.0/LICENSE` & `dbt_common-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/README.md` & `dbt_common-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/pyproject.toml` & `dbt_common-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dbt_common-1.1.0/PKG-INFO` & `dbt_common-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dbt-common
-Version: 1.1.0
+Version: 1.2.0
 Summary: The shared common utilities that dbt-core and adapter implementations use
 Project-URL: Homepage, https://github.com/dbt-labs/dbt-common
 Project-URL: Repository, https://github.com/dbt-labs/dbt-common.git
 Project-URL: Issues, https://github.com/dbt-labs/dbt-common/issues
 Project-URL: Changelog, https://github.com/dbt-labs/dbt-common/blob/main/CHANGELOG.md
 Author-email: dbt Labs <info@dbtlabs.com>
 Maintainer-email: dbt Labs <info@dbtlabs.com>
```

