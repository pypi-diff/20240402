# Comparing `tmp/dbt_common-1.0.0b1.tar.gz` & `tmp/dbt_common-1.0.0b2.tar.gz`

## Comparing `dbt_common-1.0.0b1.tar` & `dbt_common-1.0.0b2.tar`

### file list

```diff
@@ -1,100 +1,101 @@
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/CHANGELOG.md
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/codecov.yml
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/__init__.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/constants.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/context.py
--rw-r--r--   0        0        0     5254 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/dataclass_schema.py
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/helper_types.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/invocation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/py.typed
--rw-r--r--   0        0        0    13954 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/semver.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/tests.py
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/ui.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/clients/__init__.py
--rw-r--r--   0        0        0    12947 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/clients/_jinja_blocks.py
--rw-r--r--   0        0        0     9124 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/clients/agate_helper.py
--rw-r--r--   0        0        0    18502 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/clients/jinja.py
--rw-r--r--   0        0        0    19513 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/clients/system.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/contracts/__init__.py
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/contracts/constraints.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/contracts/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/contracts/config/__init__.py
--rw-r--r--   0        0        0     8356 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/contracts/config/base.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/contracts/config/materialization.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/contracts/config/metadata.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/contracts/config/properties.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/events/README.md
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/events/__init__.py
--rw-r--r--   0        0        0     5448 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/events/base_types.py
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/events/contextvars.py
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/events/event_handler.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/events/event_manager.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/events/event_manager_client.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/events/format.py
--rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/events/functions.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/events/helpers.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/events/interfaces.py
--rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/events/logger.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/events/types.proto
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/events/types.py
--rw-r--r--   0        0        0     5569 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/events/types_pb2.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/exceptions/__init__.py
--rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/exceptions/base.py
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/exceptions/cache.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/exceptions/connection.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/exceptions/contracts.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/exceptions/events.py
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/exceptions/jinja.py
--rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/exceptions/macros.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/exceptions/system.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/utils/__init__.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/utils/casting.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/utils/connection.py
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/utils/dict.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/utils/encoding.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/utils/executor.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/utils/formatting.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/dbt_common/utils/jinja.py
--rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/docs/arch/adr-0001-build-tooling.md
--rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/agate/__init__.pyi
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/agate/data_types.pyi
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/colorama/__init__.pyi
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/isodate/__init__.pyi
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/mashumaro/__init__.pyi
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/mashumaro/config.pyi
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/mashumaro/dialect.pyi
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/mashumaro/exceptions.pyi
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/mashumaro/helper.pyi
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/mashumaro/types.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/mashumaro/core/__init__.pyi
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/mashumaro/core/const.pyi
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/mashumaro/core/helpers.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/mashumaro/core/meta/__init__.pyi
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/mashumaro/core/meta/helpers.pyi
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/mashumaro/core/meta/mixin.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/mashumaro/core/meta/code/__init__.pyi
--rw-r--r--   0        0        0     6150 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/mashumaro/core/meta/code/builder.pyi
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/mashumaro/core/meta/code/lines.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/mashumaro/core/meta/types/__init__.pyi
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/mashumaro/core/meta/types/common.pyi
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/mashumaro/core/meta/types/pack.pyi
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/mashumaro/core/meta/types/unpack.pyi
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/mashumaro/jsonschema/__init__.pyi
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/mashumaro/jsonschema/annotations.pyi
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/mashumaro/jsonschema/builder.pyi
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/mashumaro/jsonschema/dialects.pyi
--rw-r--r--   0        0        0     5864 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/mashumaro/jsonschema/models.pyi
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/mashumaro/jsonschema/schema.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/mashumaro/mixins/__init__.pyi
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/mashumaro/mixins/dict.pyi
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/mashumaro/mixins/json.pyi
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/mashumaro/mixins/msgpack.pyi
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/mashumaro/mixins/orjson.pyi
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/mashumaro/mixins/toml.pyi
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/third-party-stubs/mashumaro/mixins/yaml.pyi
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/LICENSE
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/README.md
--rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/pyproject.toml
--rw-r--r--   0        0        0     3797 2020-02-02 00:00:00.000000 dbt_common-1.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/CHANGELOG.md
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/codecov.yml
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/__init__.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/constants.py
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/context.py
+-rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/dataclass_schema.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/helper_types.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/invocation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/py.typed
+-rw-r--r--   0        0        0     7015 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/record.py
+-rw-r--r--   0        0        0    13954 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/semver.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/tests.py
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/ui.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/clients/__init__.py
+-rw-r--r--   0        0        0    12947 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/clients/_jinja_blocks.py
+-rw-r--r--   0        0        0     9124 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/clients/agate_helper.py
+-rw-r--r--   0        0        0    18502 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/clients/jinja.py
+-rw-r--r--   0        0        0    23014 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/clients/system.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/contracts/__init__.py
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/contracts/constraints.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/contracts/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/contracts/config/__init__.py
+-rw-r--r--   0        0        0     8356 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/contracts/config/base.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/contracts/config/materialization.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/contracts/config/metadata.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/contracts/config/properties.py
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/events/README.md
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/events/__init__.py
+-rw-r--r--   0        0        0     5448 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/events/base_types.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/events/contextvars.py
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/events/event_handler.py
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/events/event_manager.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/events/event_manager_client.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/events/format.py
+-rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/events/functions.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/events/helpers.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/events/interfaces.py
+-rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/events/logger.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/events/types.proto
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/events/types.py
+-rw-r--r--   0        0        0     5569 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/events/types_pb2.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/exceptions/__init__.py
+-rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/exceptions/base.py
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/exceptions/cache.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/exceptions/connection.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/exceptions/contracts.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/exceptions/events.py
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/exceptions/jinja.py
+-rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/exceptions/macros.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/exceptions/system.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/utils/__init__.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/utils/casting.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/utils/connection.py
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/utils/dict.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/utils/encoding.py
+-rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/utils/executor.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/utils/formatting.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/dbt_common/utils/jinja.py
+-rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/docs/arch/adr-0001-build-tooling.md
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/agate/__init__.pyi
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/agate/data_types.pyi
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/colorama/__init__.pyi
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/isodate/__init__.pyi
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/mashumaro/__init__.pyi
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/mashumaro/config.pyi
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/mashumaro/dialect.pyi
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/mashumaro/exceptions.pyi
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/mashumaro/helper.pyi
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/mashumaro/types.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/mashumaro/core/__init__.pyi
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/mashumaro/core/const.pyi
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/mashumaro/core/helpers.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/mashumaro/core/meta/__init__.pyi
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/mashumaro/core/meta/helpers.pyi
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/mashumaro/core/meta/mixin.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/mashumaro/core/meta/code/__init__.pyi
+-rw-r--r--   0        0        0     6150 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/mashumaro/core/meta/code/builder.pyi
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/mashumaro/core/meta/code/lines.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/mashumaro/core/meta/types/__init__.pyi
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/mashumaro/core/meta/types/common.pyi
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/mashumaro/core/meta/types/pack.pyi
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/mashumaro/core/meta/types/unpack.pyi
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/mashumaro/jsonschema/__init__.pyi
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/mashumaro/jsonschema/annotations.pyi
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/mashumaro/jsonschema/builder.pyi
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/mashumaro/jsonschema/dialects.pyi
+-rw-r--r--   0        0        0     5864 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/mashumaro/jsonschema/models.pyi
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/mashumaro/jsonschema/schema.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/mashumaro/mixins/__init__.pyi
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/mashumaro/mixins/dict.pyi
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/mashumaro/mixins/json.pyi
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/mashumaro/mixins/msgpack.pyi
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/mashumaro/mixins/orjson.pyi
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/mashumaro/mixins/toml.pyi
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/third-party-stubs/mashumaro/mixins/yaml.pyi
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/LICENSE
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/README.md
+-rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 dbt_common-1.0.0b2/PKG-INFO
```

### Comparing `dbt_common-1.0.0b1/dbt_common/context.py` & `dbt_common-1.0.0b2/dbt_common/context.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from dbt_common.constants import SECRET_ENV_PREFIX
 
 
 class InvocationContext:
     def __init__(self, env: Mapping[str, str]):
         self._env = env
         self._env_secrets: Optional[List[str]] = None
+        self.recorder = None
         # This class will also eventually manage the invocation_id, flags, event manager, etc.
 
     @property
     def env(self) -> Mapping[str, str]:
         return self._env
 
     @property
```

### Comparing `dbt_common-1.0.0b1/dbt_common/dataclass_schema.py` & `dbt_common-1.0.0b2/dbt_common/dataclass_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     serialization_strategy = {
         datetime: DateTimeSerialization(),
     }
     json_schema = {
         "additionalProperties": False,
     }
     serialize_by_alias = True
+    lazy_compilation = True
 
 
 # This class pulls in DataClassDictMixin from Mashumaro. The 'to_dict'
 # and 'from_dict' methods come from Mashumaro.
 class dbtClassMixin(DataClassDictMixin):
     """Convert and validate JSON schemas.
```

### Comparing `dbt_common-1.0.0b1/dbt_common/helper_types.py` & `dbt_common-1.0.0b2/dbt_common/helper_types.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/semver.py` & `dbt_common-1.0.0b2/dbt_common/semver.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/ui.py` & `dbt_common-1.0.0b2/dbt_common/ui.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/clients/_jinja_blocks.py` & `dbt_common-1.0.0b2/dbt_common/clients/_jinja_blocks.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/clients/agate_helper.py` & `dbt_common-1.0.0b2/dbt_common/clients/agate_helper.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/clients/jinja.py` & `dbt_common-1.0.0b2/dbt_common/clients/jinja.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/clients/system.py` & `dbt_common-1.0.0b2/dbt_common/clients/system.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import dbt_common.exceptions.base
+import dataclasses
 import errno
 import fnmatch
 import functools
 import json
 import os
 import os.path
 import re
@@ -21,24 +22,69 @@
     SystemCouldNotWrite,
     SystemExecutingCmd,
     SystemStdOut,
     SystemStdErr,
     SystemReportReturnCode,
 )
 from dbt_common.exceptions import DbtInternalError
+from dbt_common.record import record_function, Recorder, Record
 from dbt_common.utils.connection import connection_exception_retry
+
 from pathspec import PathSpec  # type: ignore
 
 if sys.platform == "win32":
     from ctypes import WinDLL, c_bool
 else:
     WinDLL = None
     c_bool = None
 
 
+@dataclasses.dataclass
+class FindMatchingParams:
+    root_path: str
+    relative_paths_to_search: List[str]
+    file_pattern: str
+    # ignore_spec: Optional[PathSpec] = None
+
+    def __init__(
+        self,
+        root_path: str,
+        relative_paths_to_search: List[str],
+        file_pattern: str,
+        ignore_spec: Optional[Any] = None,
+    ):
+        self.root_path = root_path
+        rps = list(relative_paths_to_search)
+        rps.sort()
+        self.relative_paths_to_search = rps
+        self.file_pattern = file_pattern
+
+    def _include(self) -> bool:
+        # Do not record or replay filesystem searches that were performed against
+        # files which are actually part of dbt's implementation.
+        return (
+            "dbt/include/global_project" not in self.root_path
+            and "/plugins/postgres/dbt/include/" not in self.root_path
+        )
+
+
+@dataclasses.dataclass
+class FindMatchingResult:
+    matches: List[Dict[str, Any]]
+
+
+@Recorder.register_record_type
+class FindMatchingRecord(Record):
+    """Record of calls to the directory search function find_matching()"""
+
+    params_cls = FindMatchingParams
+    result_cls = FindMatchingResult
+
+
+@record_function(FindMatchingRecord)
 def find_matching(
     root_path: str,
     relative_paths_to_search: List[str],
     file_pattern: str,
     ignore_spec: Optional[PathSpec] = None,
 ) -> List[Dict[str, Any]]:
     """Return file info from paths and patterns.
@@ -90,14 +136,42 @@
                             "modification_time": modification_time,
                         }
                     )
 
     return matching
 
 
+@dataclasses.dataclass
+class LoadFileParams:
+    path: str
+    strip: bool = True
+
+    def _include(self) -> bool:
+        # Do not record or replay file reads that were performed against files
+        # which are actually part of dbt's implementation.
+        return (
+            "dbt/include/global_project" not in self.path
+            and "/plugins/postgres/dbt/include/" not in self.path
+        )
+
+
+@dataclasses.dataclass
+class LoadFileResult:
+    contents: str
+
+
+@Recorder.register_record_type
+class LoadFileRecord(Record):
+    """Record of file load operation"""
+
+    params_cls = LoadFileParams
+    result_cls = LoadFileResult
+
+
+@record_function(LoadFileRecord)
 def load_file_contents(path: str, strip: bool = True) -> str:
     path = convert_path(path)
     with open(path, "rb") as handle:
         to_return = handle.read().decode("utf-8")
 
     if strip:
         to_return = to_return.strip()
@@ -160,14 +234,37 @@
     os.symlink(source, link_path)
 
 
 def supports_symlinks() -> bool:
     return getattr(os, "symlink", None) is not None
 
 
+@dataclasses.dataclass
+class WriteFileParams:
+    path: str
+    contents: str
+
+    def _include(self) -> bool:
+        # Do not record or replay file reads that were performed against files
+        # which are actually part of dbt's implementation.
+        return (
+            "dbt/include/global_project" not in self.path
+            and "/plugins/postgres/dbt/include/" not in self.path
+        )
+
+
+@Recorder.register_record_type
+class WriteFileRecord(Record):
+    """Record of a file write operation."""
+
+    params_cls = WriteFileParams
+    result_cls = None
+
+
+@record_function(WriteFileRecord)
 def write_file(path: str, contents: str = "") -> bool:
     path = convert_path(path)
     try:
         make_directory(os.path.dirname(path))
         with open(path, "w", encoding="utf-8") as f:
             f.write(str(contents))
     except Exception as exc:
@@ -191,19 +288,36 @@
             fire_event(SystemCouldNotWrite(path=path, reason=reason, exc=str(exc)))
         else:
             raise
     return True
 
 
 def read_json(path: str) -> Dict[str, Any]:
-    return json.loads(load_file_contents(path))
+    path = convert_path(path)
+    with open(path, "r") as f:
+        return json.load(f)
 
 
 def write_json(path: str, data: Dict[str, Any]) -> bool:
-    return write_file(path, json.dumps(data, cls=dbt_common.utils.encoding.JSONEncoder))
+    path = convert_path(path)
+    try:
+        make_directory(os.path.dirname(path))
+        with open(path, "w", encoding="utf-8") as f:
+            json.dump(data, f, cls=dbt_common.utils.encoding.JSONEncoder)
+    except Exception as exc:
+        # See write_file() for an explanation of this error handling.
+        if os.name == "nt":
+            if getattr(exc, "winerror", 0) == 3:
+                reason = "Path was too long"
+            else:
+                reason = "Path was possibly too long"
+            fire_event(SystemCouldNotWrite(path=path, reason=reason, exc=str(exc)))
+        else:
+            raise
+    return True
 
 
 def _windows_rmdir_readonly(func: Callable[[str], Any], path: str, exc: Tuple[Any, OSError, Any]):
     exception_val = exc[1]
     if exception_val.errno == errno.EACCES:
         os.chmod(path, stat.S_IWUSR)
         func(path)
@@ -569,7 +683,28 @@
 def rmtree(path):
     """Recursively remove the path.
 
     On permissions errors on windows, try to remove the read-only flag and try again.
     """
     path = convert_path(path)
     return shutil.rmtree(path, onerror=chmod_and_retry)
+
+
+@dataclasses.dataclass
+class GetEnvParams:
+    pass
+
+
+@dataclasses.dataclass
+class GetEnvResult:
+    env: Dict[str, str]
+
+
+@Recorder.register_record_type
+class GetEnvRecord(Record):
+    params_cls = GetEnvParams
+    result_cls = GetEnvResult
+
+
+@record_function(GetEnvRecord)
+def get_env() -> Dict[str, str]:
+    return dict(os.environ)
```

### Comparing `dbt_common-1.0.0b1/dbt_common/contracts/constraints.py` & `dbt_common-1.0.0b2/dbt_common/contracts/constraints.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/contracts/util.py` & `dbt_common-1.0.0b2/dbt_common/contracts/util.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/contracts/config/base.py` & `dbt_common-1.0.0b2/dbt_common/contracts/config/base.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/contracts/config/metadata.py` & `dbt_common-1.0.0b2/dbt_common/contracts/config/metadata.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/contracts/config/properties.py` & `dbt_common-1.0.0b2/dbt_common/contracts/config/properties.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/events/README.md` & `dbt_common-1.0.0b2/dbt_common/events/README.md`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/events/base_types.py` & `dbt_common-1.0.0b2/dbt_common/events/base_types.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/events/contextvars.py` & `dbt_common-1.0.0b2/dbt_common/events/contextvars.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/events/event_handler.py` & `dbt_common-1.0.0b2/dbt_common/events/event_handler.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/events/event_manager.py` & `dbt_common-1.0.0b2/dbt_common/events/event_manager.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/events/event_manager_client.py` & `dbt_common-1.0.0b2/dbt_common/events/event_manager_client.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/events/format.py` & `dbt_common-1.0.0b2/dbt_common/events/format.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/events/functions.py` & `dbt_common-1.0.0b2/dbt_common/events/functions.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/events/logger.py` & `dbt_common-1.0.0b2/dbt_common/events/logger.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/events/types.proto` & `dbt_common-1.0.0b2/dbt_common/events/types.proto`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/events/types.py` & `dbt_common-1.0.0b2/dbt_common/events/types.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/events/types_pb2.py` & `dbt_common-1.0.0b2/dbt_common/events/types_pb2.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/exceptions/base.py` & `dbt_common-1.0.0b2/dbt_common/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/exceptions/cache.py` & `dbt_common-1.0.0b2/dbt_common/exceptions/cache.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/exceptions/contracts.py` & `dbt_common-1.0.0b2/dbt_common/exceptions/contracts.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/exceptions/jinja.py` & `dbt_common-1.0.0b2/dbt_common/exceptions/jinja.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/exceptions/macros.py` & `dbt_common-1.0.0b2/dbt_common/exceptions/macros.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/exceptions/system.py` & `dbt_common-1.0.0b2/dbt_common/exceptions/system.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/utils/__init__.py` & `dbt_common-1.0.0b2/dbt_common/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/utils/casting.py` & `dbt_common-1.0.0b2/dbt_common/utils/casting.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/utils/connection.py` & `dbt_common-1.0.0b2/dbt_common/utils/connection.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/utils/dict.py` & `dbt_common-1.0.0b2/dbt_common/utils/dict.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/utils/encoding.py` & `dbt_common-1.0.0b2/dbt_common/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/dbt_common/utils/executor.py` & `dbt_common-1.0.0b2/dbt_common/utils/executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,10 +70,10 @@
 
 def executor(config: HasThreadingConfig) -> ConnectingExecutor:
     if config.args.single_threaded:
         return SingleThreadedExecutor()
     else:
         return MultiThreadedExecutor(
             max_workers=config.threads,
-            initializer=_thread_initializer,
-            initargs=(get_invocation_context(),),
+            initializer=_thread_initializer,  # type: ignore
+            initargs=(get_invocation_context(),),  # type: ignore
         )
```

### Comparing `dbt_common-1.0.0b1/dbt_common/utils/jinja.py` & `dbt_common-1.0.0b2/dbt_common/utils/jinja.py`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/docs/arch/adr-0001-build-tooling.md` & `dbt_common-1.0.0b2/docs/arch/adr-0001-build-tooling.md`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/third-party-stubs/agate/__init__.pyi` & `dbt_common-1.0.0b2/third-party-stubs/agate/__init__.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/third-party-stubs/agate/data_types.pyi` & `dbt_common-1.0.0b2/third-party-stubs/agate/data_types.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/third-party-stubs/mashumaro/config.pyi` & `dbt_common-1.0.0b2/third-party-stubs/mashumaro/config.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/third-party-stubs/mashumaro/exceptions.pyi` & `dbt_common-1.0.0b2/third-party-stubs/mashumaro/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/third-party-stubs/mashumaro/helper.pyi` & `dbt_common-1.0.0b2/third-party-stubs/mashumaro/helper.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/third-party-stubs/mashumaro/types.pyi` & `dbt_common-1.0.0b2/third-party-stubs/mashumaro/types.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/third-party-stubs/mashumaro/core/meta/helpers.pyi` & `dbt_common-1.0.0b2/third-party-stubs/mashumaro/core/meta/helpers.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/third-party-stubs/mashumaro/core/meta/code/builder.pyi` & `dbt_common-1.0.0b2/third-party-stubs/mashumaro/core/meta/code/builder.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/third-party-stubs/mashumaro/core/meta/types/common.pyi` & `dbt_common-1.0.0b2/third-party-stubs/mashumaro/core/meta/types/common.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/third-party-stubs/mashumaro/core/meta/types/unpack.pyi` & `dbt_common-1.0.0b2/third-party-stubs/mashumaro/core/meta/types/unpack.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/third-party-stubs/mashumaro/jsonschema/annotations.pyi` & `dbt_common-1.0.0b2/third-party-stubs/mashumaro/jsonschema/annotations.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/third-party-stubs/mashumaro/jsonschema/builder.pyi` & `dbt_common-1.0.0b2/third-party-stubs/mashumaro/jsonschema/builder.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/third-party-stubs/mashumaro/jsonschema/dialects.pyi` & `dbt_common-1.0.0b2/third-party-stubs/mashumaro/jsonschema/dialects.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/third-party-stubs/mashumaro/jsonschema/models.pyi` & `dbt_common-1.0.0b2/third-party-stubs/mashumaro/jsonschema/models.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/third-party-stubs/mashumaro/jsonschema/schema.pyi` & `dbt_common-1.0.0b2/third-party-stubs/mashumaro/jsonschema/schema.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/third-party-stubs/mashumaro/mixins/dict.pyi` & `dbt_common-1.0.0b2/third-party-stubs/mashumaro/mixins/dict.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/third-party-stubs/mashumaro/mixins/json.pyi` & `dbt_common-1.0.0b2/third-party-stubs/mashumaro/mixins/json.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/third-party-stubs/mashumaro/mixins/msgpack.pyi` & `dbt_common-1.0.0b2/third-party-stubs/mashumaro/mixins/msgpack.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/third-party-stubs/mashumaro/mixins/orjson.pyi` & `dbt_common-1.0.0b2/third-party-stubs/mashumaro/mixins/orjson.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/third-party-stubs/mashumaro/mixins/toml.pyi` & `dbt_common-1.0.0b2/third-party-stubs/mashumaro/mixins/toml.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/third-party-stubs/mashumaro/mixins/yaml.pyi` & `dbt_common-1.0.0b2/third-party-stubs/mashumaro/mixins/yaml.pyi`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/.gitignore` & `dbt_common-1.0.0b2/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/LICENSE` & `dbt_common-1.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_common-1.0.0b1/pyproject.toml` & `dbt_common-1.0.0b2/pyproject.toml`

 * *Files identical despite different names*

