# Comparing `tmp/pydantic_core-2.8.0.tar.gz` & `tmp/pydantic_core-2.9.0.tar.gz`

## Comparing `pydantic_core-2.8.0.tar` & `pydantic_core-2.9.0.tar`

### file list

```diff
@@ -1,217 +1,219 @@
--rw-r--r--   0        0        0     1701 1970-01-01 00:00:00.000000 pydantic_core-2.8.0/Cargo.toml
--rw-r--r--   0     1001      127      312 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/.cargo/config.toml
--rw-r--r--   0     1001      127     1080 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/LICENSE
--rw-r--r--   0     1001      127     5345 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/Makefile
--rw-r--r--   0     1001      127     5101 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/README.md
--rw-r--r--   0     1001      127     1380 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/build.rs
--rw-r--r--   0     1001      127     9568 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/generate_self_schema.py
--rw-r--r--   0     1001      127     3495 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/pyproject.toml
--rw-r--r--   0     1001      127     4111 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/python/pydantic_core/__init__.py
--rw-r--r--   0     1001      127    29859 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/python/pydantic_core/_pydantic_core.pyi
--rw-r--r--   0     1001      127   133490 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/python/pydantic_core/core_schema.py
--rw-r--r--   0     1001      127        0 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/python/pydantic_core/py.typed
--rw-r--r--   0     1001      127     3065 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/argument_markers.rs
--rw-r--r--   0     1001      127     5820 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/build_tools.rs
--rw-r--r--   0     1001      127     4578 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/definitions.rs
--rw-r--r--   0     1001      127     5457 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/errors/line_error.rs
--rw-r--r--   0     1001      127     7101 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/errors/location.rs
--rw-r--r--   0     1001      127     1092 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/errors/mod.rs
--rw-r--r--   0     1001      127    32978 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/errors/types.rs
--rw-r--r--   0     1001      127    21894 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/errors/validation_exception.rs
--rw-r--r--   0     1001      127     5338 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/errors/value_exception.rs
--rw-r--r--   0     1001      127    18168 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/input/datetime.rs
--rw-r--r--   0     1001      127    10098 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/input/input_abstract.rs
--rw-r--r--   0     1001      127    21328 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/input/input_json.rs
--rw-r--r--   0     1001      127    30872 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/input/input_python.rs
--rw-r--r--   0     1001      127      982 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/input/mod.rs
--rw-r--r--   0     1001      127     7886 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/input/parse_json.rs
--rw-r--r--   0     1001      127    32922 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/input/return_enums.rs
--rw-r--r--   0     1001      127     5542 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/input/shared.rs
--rw-r--r--   0     1001      127     1522 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/lazy_index_map.rs
--rw-r--r--   0     1001      127     3415 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/lib.rs
--rw-r--r--   0     1001      127    17853 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/lookup_key.rs
--rw-r--r--   0     1001      127     2092 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/py_gc.rs
--rw-r--r--   0     1001      127     2484 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/recursion_guard.rs
--rw-r--r--   0     1001      127     6289 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/computed_fields.rs
--rw-r--r--   0     1001      127     5845 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/config.rs
--rw-r--r--   0     1001      127     2779 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/errors.rs
--rw-r--r--   0     1001      127    11523 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/extra.rs
--rw-r--r--   0     1001      127    12970 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/fields.rs
--rw-r--r--   0     1001      127    14571 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/filter.rs
--rw-r--r--   0     1001      127    26776 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/infer.rs
--rw-r--r--   0     1001      127     7818 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/mod.rs
--rw-r--r--   0     1001      127    15916 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/ob_type.rs
--rw-r--r--   0     1001      127    17545 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/shared.rs
--rw-r--r--   0     1001      127     1460 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/type_serializers/any.rs
--rw-r--r--   0     1001      127     2550 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/type_serializers/bytes.rs
--rw-r--r--   0     1001      127     6414 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/type_serializers/dataclass.rs
--rw-r--r--   0     1001      127     4534 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/type_serializers/datetime_etc.rs
--rw-r--r--   0     1001      127     2655 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/type_serializers/decimal.rs
--rw-r--r--   0     1001      127     3267 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/type_serializers/definitions.rs
--rw-r--r--   0     1001      127     5334 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/type_serializers/dict.rs
--rw-r--r--   0     1001      127     6637 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/type_serializers/format.rs
--rw-r--r--   0     1001      127    22406 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/type_serializers/function.rs
--rw-r--r--   0     1001      127     7408 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/type_serializers/generator.rs
--rw-r--r--   0     1001      127     3015 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/type_serializers/json.rs
--rw-r--r--   0     1001      127     2232 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/type_serializers/json_or_python.rs
--rw-r--r--   0     1001      127     4112 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/type_serializers/list.rs
--rw-r--r--   0     1001      127     5683 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/type_serializers/literal.rs
--rw-r--r--   0     1001      127     1018 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/type_serializers/mod.rs
--rw-r--r--   0     1001      127     8445 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/type_serializers/model.rs
--rw-r--r--   0     1001      127     2445 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/type_serializers/nullable.rs
--rw-r--r--   0     1001      127     3513 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/type_serializers/other.rs
--rw-r--r--   0     1001      127     4554 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/type_serializers/set_frozenset.rs
--rw-r--r--   0     1001      127     6017 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/type_serializers/simple.rs
--rw-r--r--   0     1001      127     2617 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/type_serializers/string.rs
--rw-r--r--   0     1001      127     2720 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/type_serializers/timedelta.rs
--rw-r--r--   0     1001      127    12889 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/type_serializers/tuple.rs
--rw-r--r--   0     1001      127     2935 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/type_serializers/typed_dict.rs
--rw-r--r--   0     1001      127     7230 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/type_serializers/union.rs
--rw-r--r--   0     1001      127     3163 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/type_serializers/url.rs
--rw-r--r--   0     1001      127     2771 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/type_serializers/uuid.rs
--rw-r--r--   0     1001      127     2124 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/serializers/type_serializers/with_default.rs
--rw-r--r--   0     1001      127     2745 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/tools.rs
--rw-r--r--   0     1001      127    16394 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/url.rs
--rw-r--r--   0     1001      127     1334 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/any.rs
--rw-r--r--   0     1001      127    15488 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/arguments.rs
--rw-r--r--   0     1001      127     1574 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/bool.rs
--rw-r--r--   0     1001      127     3882 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/bytes.rs
--rw-r--r--   0     1001      127     4282 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/call.rs
--rw-r--r--   0     1001      127     1414 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/callable.rs
--rw-r--r--   0     1001      127     3236 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/chain.rs
--rw-r--r--   0     1001      127     3837 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/custom_error.rs
--rw-r--r--   0     1001      127    26935 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/dataclass.rs
--rw-r--r--   0     1001      127     6832 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/date.rs
--rw-r--r--   0     1001      127    10335 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/datetime.rs
--rw-r--r--   0     1001      127    10324 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/decimal.rs
--rw-r--r--   0     1001      127     6137 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/definitions.rs
--rw-r--r--   0     1001      127     5940 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/dict.rs
--rw-r--r--   0     1001      127     6798 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/float.rs
--rw-r--r--   0     1001      127     1916 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/frozenset.rs
--rw-r--r--   0     1001      127    19225 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/function.rs
--rw-r--r--   0     1001      127    11981 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/generator.rs
--rw-r--r--   0     1001      127     5351 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/int.rs
--rw-r--r--   0     1001      127     3050 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/is_instance.rs
--rw-r--r--   0     1001      127     2150 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/is_subclass.rs
--rw-r--r--   0     1001      127     2485 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/json.rs
--rw-r--r--   0     1001      127     2432 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/json_or_python.rs
--rw-r--r--   0     1001      127     2602 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/lax_or_strict.rs
--rw-r--r--   0     1001      127     5671 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/list.rs
--rw-r--r--   0     1001      127     7940 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/literal.rs
--rw-r--r--   0     1001      127    23486 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/mod.rs
--rw-r--r--   0     1001      127    14133 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/model.rs
--rw-r--r--   0     1001      127    18504 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/model_fields.rs
--rw-r--r--   0     1001      127     1383 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/none.rs
--rw-r--r--   0     1001      127     1841 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/nullable.rs
--rw-r--r--   0     1001      127     2909 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/set.rs
--rw-r--r--   0     1001      127     6485 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/string.rs
--rw-r--r--   0     1001      127     4066 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/time.rs
--rw-r--r--   0     1001      127     5163 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/timedelta.rs
--rw-r--r--   0     1001      127     9471 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/tuple.rs
--rw-r--r--   0     1001      127    13352 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/typed_dict.rs
--rw-r--r--   0     1001      127    20768 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/union.rs
--rw-r--r--   0     1001      127    18790 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/url.rs
--rw-r--r--   0     1001      127     6943 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/uuid.rs
--rw-r--r--   0     1001      127     2476 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/validation_state.rs
--rw-r--r--   0     1001      127     6827 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/src/validators/with_default.rs
--rw-r--r--   0     1001      127        0 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/__init__.py
--rw-r--r--   0     1001      127        0 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/benchmarks/__init__.py
--rw-r--r--   0     1001      127    16108 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/benchmarks/complete_schema.py
--rw-r--r--   0     1001      127     5110 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/benchmarks/test_complete_benchmark.py
--rw-r--r--   0     1001      127    45782 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/benchmarks/test_micro_benchmarks.py
--rw-r--r--   0     1001      127    14403 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/benchmarks/test_serialization_micro.py
--rw-r--r--   0     1001      127     4703 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/conftest.py
--rw-r--r--   0     1001      127     3272 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/emscripten_runner.js
--rw-r--r--   0     1001      127       72 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/requirements-linting.txt
--rw-r--r--   0     1001      127      906 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/requirements.txt
--rw-r--r--   0     1001      127        0 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/serializers/__init__.py
--rw-r--r--   0     1001      127    24645 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/serializers/test_any.py
--rw-r--r--   0     1001      127     4342 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/serializers/test_bytes.py
--rw-r--r--   0     1001      127     6333 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/serializers/test_dataclasses.py
--rw-r--r--   0     1001      127     5271 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/serializers/test_datetime.py
--rw-r--r--   0     1001      127     2175 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/serializers/test_decimal.py
--rw-r--r--   0     1001      127     4202 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/serializers/test_definitions.py
--rw-r--r--   0     1001      127     4681 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/serializers/test_definitions_recursive.py
--rw-r--r--   0     1001      127     7509 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/serializers/test_dict.py
--rw-r--r--   0     1001      127     4659 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/serializers/test_format.py
--rw-r--r--   0     1001      127    22892 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/serializers/test_functions.py
--rw-r--r--   0     1001      127     5424 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/serializers/test_generator.py
--rw-r--r--   0     1001      127     1853 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/serializers/test_json.py
--rw-r--r--   0     1001      127     1198 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/serializers/test_json_or_python.py
--rw-r--r--   0     1001      127    18387 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/serializers/test_list_tuple.py
--rw-r--r--   0     1001      127     2513 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/serializers/test_literal.py
--rw-r--r--   0     1001      127      517 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/serializers/test_misc.py
--rw-r--r--   0     1001      127    35459 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/serializers/test_model.py
--rw-r--r--   0     1001      127     5749 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/serializers/test_model_root.py
--rw-r--r--   0     1001      127      953 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/serializers/test_none.py
--rw-r--r--   0     1001      127      566 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/serializers/test_nullable.py
--rw-r--r--   0     1001      127     2174 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/serializers/test_other.py
--rw-r--r--   0     1001      127     2052 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/serializers/test_set_frozenset.py
--rw-r--r--   0     1001      127     4026 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/serializers/test_simple.py
--rw-r--r--   0     1001      127     2503 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/serializers/test_string.py
--rw-r--r--   0     1001      127     2083 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/serializers/test_timedelta.py
--rw-r--r--   0     1001      127    13155 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/serializers/test_typed_dict.py
--rw-r--r--   0     1001      127    15018 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/serializers/test_union.py
--rw-r--r--   0     1001      127     4287 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/serializers/test_url.py
--rw-r--r--   0     1001      127     2646 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/serializers/test_uuid.py
--rw-r--r--   0     1001      127     2972 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/test.rs
--rw-r--r--   0     1001      127     4782 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/test_build.py
--rw-r--r--   0     1001      127     4675 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/test_config.py
--rw-r--r--   0     1001      127     1246 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/test_docstrings.py
--rw-r--r--   0     1001      127    44390 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/test_errors.py
--rw-r--r--   0     1001      127     1979 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/test_garbage_collection.py
--rw-r--r--   0     1001      127     6269 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/test_hypothesis.py
--rw-r--r--   0     1001      127     2184 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/test_isinstance.py
--rw-r--r--   0     1001      127    12266 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/test_json.py
--rw-r--r--   0     1001      127     7055 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/test_misc.py
--rw-r--r--   0     1001      127    13682 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/test_schema_functions.py
--rw-r--r--   0     1001      127     1795 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/test_strict.py
--rw-r--r--   0     1001      127     9425 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/test_typing.py
--rw-r--r--   0     1001      127     6894 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/test_tzinfo.py
--rw-r--r--   0     1001      127     5013 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/test_validation_context.py
--rw-r--r--   0     1001      127        0 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/__init__.py
--rw-r--r--   0     1001      127    35676 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_arguments.py
--rw-r--r--   0     1001      127     4108 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_bool.py
--rw-r--r--   0     1001      127     4396 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_bytes.py
--rw-r--r--   0     1001      127     7161 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_call.py
--rw-r--r--   0     1001      127     1492 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_callable.py
--rw-r--r--   0     1001      127     4083 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_chain.py
--rw-r--r--   0     1001      127     1699 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_custom_error.py
--rw-r--r--   0     1001      127    52705 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_dataclasses.py
--rw-r--r--   0     1001      127    12314 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_date.py
--rw-r--r--   0     1001      127    21572 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_datetime.py
--rw-r--r--   0     1001      127    15823 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_decimal.py
--rw-r--r--   0     1001      127     5097 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_definitions.py
--rw-r--r--   0     1001      127    32263 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_definitions_recursive.py
--rw-r--r--   0     1001      127     9074 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_dict.py
--rw-r--r--   0     1001      127    12981 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_float.py
--rw-r--r--   0     1001      127    11389 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_frozenset.py
--rw-r--r--   0     1001      127    30880 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_function.py
--rw-r--r--   0     1001      127     6819 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_generator.py
--rw-r--r--   0     1001      127    15798 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_int.py
--rw-r--r--   0     1001      127     5991 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_is_instance.py
--rw-r--r--   0     1001      127     2065 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_is_subclass.py
--rw-r--r--   0     1001      127     5260 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_json.py
--rw-r--r--   0     1001      127     1027 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_json_or_python.py
--rw-r--r--   0     1001      127     1640 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_lax_or_strict.py
--rw-r--r--   0     1001      127    17251 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_list.py
--rw-r--r--   0     1001      127    12324 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_literal.py
--rw-r--r--   0     1001      127    39234 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_model.py
--rw-r--r--   0     1001      127    62233 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_model_fields.py
--rw-r--r--   0     1001      127    15939 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_model_init.py
--rw-r--r--   0     1001      127     7123 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_model_root.py
--rw-r--r--   0     1001      127      760 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_none.py
--rw-r--r--   0     1001      127     1941 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_nullable.py
--rw-r--r--   0     1001      127    10405 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_set.py
--rw-r--r--   0     1001      127     9722 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_string.py
--rw-r--r--   0     1001      127    22645 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_tagged_union.py
--rw-r--r--   0     1001      127    13038 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_time.py
--rw-r--r--   0     1001      127    14114 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_timedelta.py
--rw-r--r--   0     1001      127    18169 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_tuple.py
--rw-r--r--   0     1001      127    42896 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_typed_dict.py
--rw-r--r--   0     1001      127    18546 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_union.py
--rw-r--r--   0     1001      127    56241 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_url.py
--rw-r--r--   0     1001      127     9013 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_uuid.py
--rw-r--r--   0     1001      127    22764 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/tests/validators/test_with_default.py
--rw-r--r--   0     1001      127    16481 2023-09-18 20:38:51.000000 pydantic_core-2.8.0/Cargo.lock
--rw-r--r--   0        0        0     6513 1970-01-01 00:00:00.000000 pydantic_core-2.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1701 1970-01-01 00:00:00.000000 pydantic_core-2.9.0/Cargo.toml
+-rw-r--r--   0     1001      127      312 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/.cargo/config.toml
+-rw-r--r--   0     1001      127     1080 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/LICENSE
+-rw-r--r--   0     1001      127     5345 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/Makefile
+-rw-r--r--   0     1001      127     5101 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/README.md
+-rw-r--r--   0     1001      127     1380 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/build.rs
+-rw-r--r--   0     1001      127     9568 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/generate_self_schema.py
+-rw-r--r--   0     1001      127     3495 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/pyproject.toml
+-rw-r--r--   0     1001      127     4111 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/python/pydantic_core/__init__.py
+-rw-r--r--   0     1001      127    31314 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/python/pydantic_core/_pydantic_core.pyi
+-rw-r--r--   0     1001      127   133663 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/python/pydantic_core/core_schema.py
+-rw-r--r--   0     1001      127        0 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/python/pydantic_core/py.typed
+-rw-r--r--   0     1001      127     3065 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/argument_markers.rs
+-rw-r--r--   0     1001      127     5842 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/build_tools.rs
+-rw-r--r--   0     1001      127     4578 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/definitions.rs
+-rw-r--r--   0     1001      127     5457 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/errors/line_error.rs
+-rw-r--r--   0     1001      127     7101 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/errors/location.rs
+-rw-r--r--   0     1001      127     1081 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/errors/mod.rs
+-rw-r--r--   0     1001      127    32582 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/errors/types.rs
+-rw-r--r--   0     1001      127    22319 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/errors/validation_exception.rs
+-rw-r--r--   0     1001      127     5320 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/errors/value_exception.rs
+-rw-r--r--   0     1001      127    18168 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/input/datetime.rs
+-rw-r--r--   0     1001      127    11411 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/input/input_abstract.rs
+-rw-r--r--   0     1001      127    19228 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/input/input_json.rs
+-rw-r--r--   0     1001      127    31403 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/input/input_python.rs
+-rw-r--r--   0     1001      127     7910 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/input/input_string.rs
+-rw-r--r--   0     1001      127     1098 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/input/mod.rs
+-rw-r--r--   0     1001      127     7886 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/input/parse_json.rs
+-rw-r--r--   0     1001      127    34174 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/input/return_enums.rs
+-rw-r--r--   0     1001      127     5701 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/input/shared.rs
+-rw-r--r--   0     1001      127     1522 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/lazy_index_map.rs
+-rw-r--r--   0     1001      127     3415 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/lib.rs
+-rw-r--r--   0     1001      127    18852 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/lookup_key.rs
+-rw-r--r--   0     1001      127     2092 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/py_gc.rs
+-rw-r--r--   0     1001      127     2484 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/recursion_guard.rs
+-rw-r--r--   0     1001      127     6289 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/computed_fields.rs
+-rw-r--r--   0     1001      127     5845 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/config.rs
+-rw-r--r--   0     1001      127     2779 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/errors.rs
+-rw-r--r--   0     1001      127    11523 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/extra.rs
+-rw-r--r--   0     1001      127    12970 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/fields.rs
+-rw-r--r--   0     1001      127    14571 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/filter.rs
+-rw-r--r--   0     1001      127    26776 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/infer.rs
+-rw-r--r--   0     1001      127     7818 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/mod.rs
+-rw-r--r--   0     1001      127    15916 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/ob_type.rs
+-rw-r--r--   0     1001      127    17608 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/shared.rs
+-rw-r--r--   0     1001      127     1460 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/type_serializers/any.rs
+-rw-r--r--   0     1001      127     2550 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/type_serializers/bytes.rs
+-rw-r--r--   0     1001      127     6477 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/type_serializers/dataclass.rs
+-rw-r--r--   0     1001      127     4534 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/type_serializers/datetime_etc.rs
+-rw-r--r--   0     1001      127     2655 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/type_serializers/decimal.rs
+-rw-r--r--   0     1001      127     3537 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/type_serializers/definitions.rs
+-rw-r--r--   0     1001      127     5334 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/type_serializers/dict.rs
+-rw-r--r--   0     1001      127     6637 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/type_serializers/format.rs
+-rw-r--r--   0     1001      127    22406 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/type_serializers/function.rs
+-rw-r--r--   0     1001      127     7408 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/type_serializers/generator.rs
+-rw-r--r--   0     1001      127     3015 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/type_serializers/json.rs
+-rw-r--r--   0     1001      127     2232 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/type_serializers/json_or_python.rs
+-rw-r--r--   0     1001      127     4112 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/type_serializers/list.rs
+-rw-r--r--   0     1001      127     5683 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/type_serializers/literal.rs
+-rw-r--r--   0     1001      127     1018 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/type_serializers/mod.rs
+-rw-r--r--   0     1001      127     8508 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/type_serializers/model.rs
+-rw-r--r--   0     1001      127     2518 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/type_serializers/nullable.rs
+-rw-r--r--   0     1001      127     3513 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/type_serializers/other.rs
+-rw-r--r--   0     1001      127     4554 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/type_serializers/set_frozenset.rs
+-rw-r--r--   0     1001      127     6017 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/type_serializers/simple.rs
+-rw-r--r--   0     1001      127     2617 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/type_serializers/string.rs
+-rw-r--r--   0     1001      127     2720 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/type_serializers/timedelta.rs
+-rw-r--r--   0     1001      127    12889 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/type_serializers/tuple.rs
+-rw-r--r--   0     1001      127     2935 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/type_serializers/typed_dict.rs
+-rw-r--r--   0     1001      127     7382 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/type_serializers/union.rs
+-rw-r--r--   0     1001      127     3163 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/type_serializers/url.rs
+-rw-r--r--   0     1001      127     2771 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/type_serializers/uuid.rs
+-rw-r--r--   0     1001      127     2197 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/serializers/type_serializers/with_default.rs
+-rw-r--r--   0     1001      127     2745 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/tools.rs
+-rw-r--r--   0     1001      127    16394 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/url.rs
+-rw-r--r--   0     1001      127     1334 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/any.rs
+-rw-r--r--   0     1001      127    15556 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/arguments.rs
+-rw-r--r--   0     1001      127     1574 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/bool.rs
+-rw-r--r--   0     1001      127     3882 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/bytes.rs
+-rw-r--r--   0     1001      127     4282 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/call.rs
+-rw-r--r--   0     1001      127     1414 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/callable.rs
+-rw-r--r--   0     1001      127     3236 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/chain.rs
+-rw-r--r--   0     1001      127     3837 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/custom_error.rs
+-rw-r--r--   0     1001      127    28362 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/dataclass.rs
+-rw-r--r--   0     1001      127     6832 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/date.rs
+-rw-r--r--   0     1001      127    10335 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/datetime.rs
+-rw-r--r--   0     1001      127    10324 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/decimal.rs
+-rw-r--r--   0     1001      127     6137 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/definitions.rs
+-rw-r--r--   0     1001      127     6323 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/dict.rs
+-rw-r--r--   0     1001      127     6798 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/float.rs
+-rw-r--r--   0     1001      127     1916 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/frozenset.rs
+-rw-r--r--   0     1001      127    19237 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/function.rs
+-rw-r--r--   0     1001      127    11988 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/generator.rs
+-rw-r--r--   0     1001      127     5351 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/int.rs
+-rw-r--r--   0     1001      127     3050 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/is_instance.rs
+-rw-r--r--   0     1001      127     2150 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/is_subclass.rs
+-rw-r--r--   0     1001      127     2485 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/json.rs
+-rw-r--r--   0     1001      127     2424 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/json_or_python.rs
+-rw-r--r--   0     1001      127     2602 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/lax_or_strict.rs
+-rw-r--r--   0     1001      127     5671 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/list.rs
+-rw-r--r--   0     1001      127     7940 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/literal.rs
+-rw-r--r--   0     1001      127    24211 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/mod.rs
+-rw-r--r--   0     1001      127    14133 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/model.rs
+-rw-r--r--   0     1001      127    18960 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/model_fields.rs
+-rw-r--r--   0     1001      127     1383 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/none.rs
+-rw-r--r--   0     1001      127     1841 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/nullable.rs
+-rw-r--r--   0     1001      127     2909 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/set.rs
+-rw-r--r--   0     1001      127     6904 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/string.rs
+-rw-r--r--   0     1001      127     4066 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/time.rs
+-rw-r--r--   0     1001      127     5163 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/timedelta.rs
+-rw-r--r--   0     1001      127     9471 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/tuple.rs
+-rw-r--r--   0     1001      127    14144 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/typed_dict.rs
+-rw-r--r--   0     1001      127    20862 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/union.rs
+-rw-r--r--   0     1001      127    18804 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/url.rs
+-rw-r--r--   0     1001      127     6943 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/uuid.rs
+-rw-r--r--   0     1001      127     2536 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/validation_state.rs
+-rw-r--r--   0     1001      127     6827 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/src/validators/with_default.rs
+-rw-r--r--   0     1001      127        0 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/__init__.py
+-rw-r--r--   0     1001      127        0 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/benchmarks/__init__.py
+-rw-r--r--   0     1001      127    16108 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/benchmarks/complete_schema.py
+-rw-r--r--   0     1001      127     5110 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/benchmarks/test_complete_benchmark.py
+-rw-r--r--   0     1001      127    45782 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/benchmarks/test_micro_benchmarks.py
+-rw-r--r--   0     1001      127    14403 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/benchmarks/test_serialization_micro.py
+-rw-r--r--   0     1001      127     4883 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/conftest.py
+-rw-r--r--   0     1001      127     3272 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/emscripten_runner.js
+-rw-r--r--   0     1001      127       72 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/requirements-linting.txt
+-rw-r--r--   0     1001      127      906 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/requirements.txt
+-rw-r--r--   0     1001      127        0 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/serializers/__init__.py
+-rw-r--r--   0     1001      127    24645 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/serializers/test_any.py
+-rw-r--r--   0     1001      127     4342 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/serializers/test_bytes.py
+-rw-r--r--   0     1001      127     6333 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/serializers/test_dataclasses.py
+-rw-r--r--   0     1001      127     5271 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/serializers/test_datetime.py
+-rw-r--r--   0     1001      127     2175 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/serializers/test_decimal.py
+-rw-r--r--   0     1001      127     4202 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/serializers/test_definitions.py
+-rw-r--r--   0     1001      127     4681 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/serializers/test_definitions_recursive.py
+-rw-r--r--   0     1001      127     7509 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/serializers/test_dict.py
+-rw-r--r--   0     1001      127     4659 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/serializers/test_format.py
+-rw-r--r--   0     1001      127    22892 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/serializers/test_functions.py
+-rw-r--r--   0     1001      127     5424 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/serializers/test_generator.py
+-rw-r--r--   0     1001      127     1853 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/serializers/test_json.py
+-rw-r--r--   0     1001      127     1198 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/serializers/test_json_or_python.py
+-rw-r--r--   0     1001      127    18387 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/serializers/test_list_tuple.py
+-rw-r--r--   0     1001      127     2513 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/serializers/test_literal.py
+-rw-r--r--   0     1001      127      517 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/serializers/test_misc.py
+-rw-r--r--   0     1001      127    35459 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/serializers/test_model.py
+-rw-r--r--   0     1001      127     5749 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/serializers/test_model_root.py
+-rw-r--r--   0     1001      127      953 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/serializers/test_none.py
+-rw-r--r--   0     1001      127      566 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/serializers/test_nullable.py
+-rw-r--r--   0     1001      127     2174 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/serializers/test_other.py
+-rw-r--r--   0     1001      127     2052 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/serializers/test_set_frozenset.py
+-rw-r--r--   0     1001      127     4026 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/serializers/test_simple.py
+-rw-r--r--   0     1001      127     2503 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/serializers/test_string.py
+-rw-r--r--   0     1001      127     2083 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/serializers/test_timedelta.py
+-rw-r--r--   0     1001      127    13155 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/serializers/test_typed_dict.py
+-rw-r--r--   0     1001      127    16779 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/serializers/test_union.py
+-rw-r--r--   0     1001      127     4287 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/serializers/test_url.py
+-rw-r--r--   0     1001      127     2646 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/serializers/test_uuid.py
+-rw-r--r--   0     1001      127     2972 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/test.rs
+-rw-r--r--   0     1001      127     4782 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/test_build.py
+-rw-r--r--   0     1001      127     4675 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/test_config.py
+-rw-r--r--   0     1001      127     1246 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/test_docstrings.py
+-rw-r--r--   0     1001      127    44959 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/test_errors.py
+-rw-r--r--   0     1001      127     1979 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/test_garbage_collection.py
+-rw-r--r--   0     1001      127     6269 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/test_hypothesis.py
+-rw-r--r--   0     1001      127     2184 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/test_isinstance.py
+-rw-r--r--   0     1001      127    12266 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/test_json.py
+-rw-r--r--   0     1001      127     7055 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/test_misc.py
+-rw-r--r--   0     1001      127    13682 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/test_schema_functions.py
+-rw-r--r--   0     1001      127     1795 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/test_strict.py
+-rw-r--r--   0     1001      127     9425 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/test_typing.py
+-rw-r--r--   0     1001      127     6894 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/test_tzinfo.py
+-rw-r--r--   0     1001      127     4794 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/test_validate_strings.py
+-rw-r--r--   0     1001      127     5013 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/test_validation_context.py
+-rw-r--r--   0     1001      127        0 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/__init__.py
+-rw-r--r--   0     1001      127    35676 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_arguments.py
+-rw-r--r--   0     1001      127     4198 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_bool.py
+-rw-r--r--   0     1001      127     4396 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_bytes.py
+-rw-r--r--   0     1001      127     7161 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_call.py
+-rw-r--r--   0     1001      127     1492 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_callable.py
+-rw-r--r--   0     1001      127     4083 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_chain.py
+-rw-r--r--   0     1001      127     1699 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_custom_error.py
+-rw-r--r--   0     1001      127    52705 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_dataclasses.py
+-rw-r--r--   0     1001      127    12314 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_date.py
+-rw-r--r--   0     1001      127    21572 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_datetime.py
+-rw-r--r--   0     1001      127    15823 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_decimal.py
+-rw-r--r--   0     1001      127     5097 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_definitions.py
+-rw-r--r--   0     1001      127    32263 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_definitions_recursive.py
+-rw-r--r--   0     1001      127     9074 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_dict.py
+-rw-r--r--   0     1001      127    13067 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_float.py
+-rw-r--r--   0     1001      127    11389 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_frozenset.py
+-rw-r--r--   0     1001      127    31694 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_function.py
+-rw-r--r--   0     1001      127     6819 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_generator.py
+-rw-r--r--   0     1001      127    15876 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_int.py
+-rw-r--r--   0     1001      127     5991 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_is_instance.py
+-rw-r--r--   0     1001      127     2065 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_is_subclass.py
+-rw-r--r--   0     1001      127     5545 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_json.py
+-rw-r--r--   0     1001      127     1027 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_json_or_python.py
+-rw-r--r--   0     1001      127     1640 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_lax_or_strict.py
+-rw-r--r--   0     1001      127    17251 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_list.py
+-rw-r--r--   0     1001      127    12324 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_literal.py
+-rw-r--r--   0     1001      127    39234 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_model.py
+-rw-r--r--   0     1001      127    62233 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_model_fields.py
+-rw-r--r--   0     1001      127    15939 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_model_init.py
+-rw-r--r--   0     1001      127     7123 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_model_root.py
+-rw-r--r--   0     1001      127      760 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_none.py
+-rw-r--r--   0     1001      127     1941 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_nullable.py
+-rw-r--r--   0     1001      127    10405 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_set.py
+-rw-r--r--   0     1001      127    11101 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_string.py
+-rw-r--r--   0     1001      127    22645 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_tagged_union.py
+-rw-r--r--   0     1001      127    13038 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_time.py
+-rw-r--r--   0     1001      127    14114 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_timedelta.py
+-rw-r--r--   0     1001      127    18169 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_tuple.py
+-rw-r--r--   0     1001      127    42896 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_typed_dict.py
+-rw-r--r--   0     1001      127    18598 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_union.py
+-rw-r--r--   0     1001      127    56241 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_url.py
+-rw-r--r--   0     1001      127     9013 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_uuid.py
+-rw-r--r--   0     1001      127    22764 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/tests/validators/test_with_default.py
+-rw-r--r--   0     1001      127    16481 2023-09-20 14:51:38.000000 pydantic_core-2.9.0/Cargo.lock
+-rw-r--r--   0        0        0     6513 1970-01-01 00:00:00.000000 pydantic_core-2.9.0/PKG-INFO
```

### Comparing `pydantic_core-2.8.0/Cargo.toml` & `pydantic_core-2.9.0/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pydantic-core"
-version = "2.8.0"
+version = "2.9.0"
 edition = "2021"
 license = "MIT"
 homepage = "https://github.com/pydantic/pydantic-core"
 repository = "https://github.com/pydantic/pydantic-core.git"
 readme = "README.md"
 include = [
     "/pyproject.toml",
```

### Comparing `pydantic_core-2.8.0/LICENSE` & `pydantic_core-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/Makefile` & `pydantic_core-2.9.0/Makefile`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/README.md` & `pydantic_core-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/build.rs` & `pydantic_core-2.9.0/build.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/generate_self_schema.py` & `pydantic_core-2.9.0/generate_self_schema.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/pyproject.toml` & `pydantic_core-2.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/python/pydantic_core/__init__.py` & `pydantic_core-2.9.0/python/pydantic_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/python/pydantic_core/_pydantic_core.pyi` & `pydantic_core-2.9.0/python/pydantic_core/_pydantic_core.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,16 @@
 __version__: str
 build_profile: str
 build_info: str
 _recursion_limit: int
 
 _T = TypeVar('_T', default=Any, covariant=True)
 
+_StringInput: TypeAlias = 'dict[str, _StringInput]'
+
 @final
 class Some(Generic[_T]):
     """
     Similar to Rust's [`Option::Some`](https://doc.rust-lang.org/std/option/enum.Option.html) type, this
     identifies a value as being present, and provides a way to access it.
 
     Generally used in a union with `None` to different between "some value which could be None" and no value.
@@ -167,14 +169,37 @@
         Raises:
             ValidationError: If validation fails or if the JSON data is invalid.
             Exception: Other error types maybe raised if internal errors occur.
 
         Returns:
             The validated Python object.
         """
+    def validate_strings(
+        self, input: _StringInput, *, strict: bool | None = None, context: 'dict[str, Any] | None' = None
+    ) -> Any:
+        """
+        Validate a string against the schema and return the validated Python object.
+
+        This is similar to `validate_json` but applies to scenarios where the input will be a string but not
+        JSON data, e.g. URL fragments, query parameters, etc.
+
+        Arguments:
+            input: The input as a string, or bytes/bytearray if `strict=False`.
+            strict: Whether to validate the object in strict mode.
+                If `None`, the value of [`CoreConfig.strict`][pydantic_core.core_schema.CoreConfig] is used.
+            context: The context to use for validation, this is passed to functional validators as
+                [`info.context`][pydantic_core.core_schema.ValidationInfo.context].
+
+        Raises:
+            ValidationError: If validation fails or if the JSON data is invalid.
+            Exception: Other error types maybe raised if internal errors occur.
+
+        Returns:
+            The validated Python object.
+        """
     def validate_assignment(
         self,
         obj: Any,
         field_name: str,
         field_value: Any,
         *,
         strict: bool | None = None,
@@ -676,59 +701,70 @@
     which detail why validation failed.
     """
 
     @staticmethod
     def from_exception_data(
         title: str,
         line_errors: list[InitErrorDetails],
-        error_mode: Literal['python', 'json'] = 'python',
+        input_type: Literal['python', 'json'] = 'python',
         hide_input: bool = False,
     ) -> ValidationError:
         """
         Python constructor for a Validation Error.
 
         The API for constructing validation errors will probably change in the future,
         hence the static method rather than `__init__`.
 
         Arguments:
             title: The title of the error, as used in the heading of `str(validation_error)`
             line_errors: A list of [`InitErrorDetails`][pydantic_core.InitErrorDetails] which contain information
                 about errors that occurred during validation.
-            error_mode: Whether the error is for a Python object or JSON.
+            input_type: Whether the error is for a Python object or JSON.
             hide_input: Whether to hide the input value in the error message.
         """
     @property
     def title(self) -> str:
         """
         The title of the error, as used in the heading of `str(validation_error)`.
         """
     def error_count(self) -> int:
         """
         Returns:
             The number of errors in the validation error.
         """
-    def errors(self, *, include_url: bool = True, include_context: bool = True) -> list[ErrorDetails]:
+    def errors(
+        self, *, include_url: bool = True, include_context: bool = True, include_input: bool = True
+    ) -> list[ErrorDetails]:
         """
         Details about each error in the validation error.
 
         Args:
             include_url: Whether to include a URL to documentation on the error each error.
             include_context: Whether to include the context of each error.
+            include_input: Whether to include the input value of each error.
 
         Returns:
             A list of [`ErrorDetails`][pydantic_core.ErrorDetails] for each error in the validation error.
         """
-    def json(self, *, indent: int | None = None, include_url: bool = True, include_context: bool = True) -> str:
+    def json(
+        self,
+        *,
+        indent: int | None = None,
+        include_url: bool = True,
+        include_context: bool = True,
+        include_input: bool = True,
+    ) -> str:
         """
         Same as [`errors()`][pydantic_core.ValidationError.errors] but returns a JSON string.
 
         Args:
             indent: The number of spaces to indent the JSON by, or `None` for no indentation - compact JSON.
             include_url: Whether to include a URL to documentation on the error each error.
             include_context: Whether to include the context of each error.
+            include_input: Whether to include the input value of each error.
 
         Returns:
             a JSON string.
         """
 
 @final
 class PydanticCustomError(ValueError):
```

### Comparing `pydantic_core-2.8.0/python/pydantic_core/core_schema.py` & `pydantic_core-2.9.0/python/pydantic_core/core_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,15 @@
         str_to_upper: Whether to convert string fields to uppercase.
         allow_inf_nan: Whether to allow infinity and NaN values for float fields. Default is `True`.
         ser_json_timedelta: The serialization option for `timedelta` values. Default is 'iso8601'.
         ser_json_bytes: The serialization option for `bytes` values. Default is 'utf8'.
         hide_input_in_errors: Whether to hide input data from `ValidationError` representation.
         validation_error_cause: Whether to add user-python excs to the __cause__ of a ValidationError.
             Requires exceptiongroup backport pre Python 3.11.
+        coerce_numbers_to_str: Whether to enable coercion of any `Number` type to `str` (not applicable in `strict` mode).
     """
 
     title: str
     strict: bool
     # settings related to typed dicts, model fields, dataclass fields
     extra_fields_behavior: ExtraBehavior
     typed_dict_total: bool  # default: True
@@ -91,14 +92,15 @@
     allow_inf_nan: bool  # default: True
     # the config options are used to customise serialization to JSON
     ser_json_timedelta: Literal['iso8601', 'float']  # default: 'iso8601'
     ser_json_bytes: Literal['utf8', 'base64']  # default: 'utf8'
     # used to hide input data from ValidationError repr
     hide_input_in_errors: bool
     validation_error_cause: bool  # default: False
+    coerce_numbers_to_str: bool  # default: False
 
 
 IncExCall: TypeAlias = 'set[int | str] | dict[int | str, IncExCall] | None'
 
 
 class SerializationInfo(Protocol):
     @property
```

### Comparing `pydantic_core-2.8.0/src/argument_markers.rs` & `pydantic_core-2.9.0/src/argument_markers.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/build_tools.rs` & `pydantic_core-2.9.0/src/build_tools.rs`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 use std::fmt;
 
 use pyo3::exceptions::PyException;
 use pyo3::prelude::*;
 use pyo3::types::{PyDict, PyList, PyString};
 use pyo3::{intern, FromPyObject, PyErrArguments};
 
-use crate::errors::{ErrorMode, ValError};
+use crate::errors::ValError;
+use crate::input::InputType;
 use crate::tools::SchemaDict;
 use crate::ValidationError;
 
 pub fn schema_or_config<'py, T>(
     schema: &'py PyDict,
     config: Option<&'py PyDict>,
     schema_key: &PyString,
@@ -82,15 +83,15 @@
     }
 
     pub fn from_val_error(py: Python, error: ValError) -> PyErr {
         match error {
             ValError::LineErrors(raw_errors) => {
                 let line_errors = raw_errors.into_iter().map(|e| e.into_py(py)).collect();
                 let validation_error =
-                    ValidationError::new(line_errors, "Schema".to_object(py), ErrorMode::Python, false);
+                    ValidationError::new(line_errors, "Schema".to_object(py), InputType::Python, false);
                 let schema_error = SchemaError(SchemaErrorEnum::ValidationError(validation_error));
                 match Py::new(py, schema_error) {
                     Ok(err) => PyErr::from_value(err.into_ref(py)),
                     Err(err) => err,
                 }
             }
             ValError::InternalErr(err) => err,
@@ -120,15 +121,15 @@
             SchemaErrorEnum::ValidationError(error) => error.error_count(),
         }
     }
 
     fn errors(&self, py: Python) -> PyResult<Py<PyList>> {
         match &self.0 {
             SchemaErrorEnum::Message(_) => Ok(PyList::empty(py).into_py(py)),
-            SchemaErrorEnum::ValidationError(error) => error.errors(py, false, false),
+            SchemaErrorEnum::ValidationError(error) => error.errors(py, false, false, true),
         }
     }
 
     fn __str__(&self, py: Python) -> String {
         match &self.0 {
             SchemaErrorEnum::Message(message) => message.clone(),
             SchemaErrorEnum::ValidationError(error) => error.display(py, Some("Invalid Schema:"), false),
```

### Comparing `pydantic_core-2.8.0/src/definitions.rs` & `pydantic_core-2.9.0/src/definitions.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/errors/line_error.rs` & `pydantic_core-2.9.0/src/errors/line_error.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/errors/location.rs` & `pydantic_core-2.9.0/src/errors/location.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/errors/mod.rs` & `pydantic_core-2.9.0/src/errors/mod.rs`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 mod location;
 mod types;
 mod validation_exception;
 mod value_exception;
 
 pub use self::line_error::{InputValue, ValError, ValLineError, ValResult};
 pub use self::location::LocItem;
-pub use self::types::{list_all_errors, ErrorMode, ErrorType, ErrorTypeDefaults, Number};
+pub use self::types::{list_all_errors, ErrorType, ErrorTypeDefaults, Number};
 pub use self::validation_exception::ValidationError;
 pub use self::value_exception::{PydanticCustomError, PydanticKnownError, PydanticOmit, PydanticUseDefault};
 
 pub fn py_err_string(py: Python, err: PyErr) -> String {
     let value = err.value(py);
     match value.get_type().name() {
         Ok(type_name) => match value.str() {
```

### Comparing `pydantic_core-2.8.0/src/errors/types.rs` & `pydantic_core-2.9.0/src/errors/types.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,60 +1,43 @@
 use std::any::type_name;
 use std::borrow::Cow;
 use std::fmt;
 
-use ahash::AHashMap;
-use num_bigint::BigInt;
-use pyo3::exceptions::{PyKeyError, PyTypeError, PyValueError};
+use pyo3::exceptions::{PyKeyError, PyTypeError};
 use pyo3::once_cell::GILOnceCell;
 use pyo3::prelude::*;
 use pyo3::types::{PyDict, PyList};
 
-use crate::input::Int;
-use crate::tools::{extract_i64, py_err, py_error_type};
+use ahash::AHashMap;
+use num_bigint::BigInt;
 use strum::{Display, EnumMessage, IntoEnumIterator};
 use strum_macros::EnumIter;
 
-use super::PydanticCustomError;
-
-#[derive(Clone, Debug)]
-pub enum ErrorMode {
-    Python,
-    Json,
-}
-
-impl TryFrom<&str> for ErrorMode {
-    type Error = PyErr;
+use crate::input::{InputType, Int};
+use crate::tools::{extract_i64, py_err, py_error_type};
 
-    fn try_from(error_mode: &str) -> PyResult<Self> {
-        match error_mode {
-            "python" => Ok(Self::Python),
-            "json" => Ok(Self::Json),
-            s => py_err!(PyValueError; "Invalid error mode: {}", s),
-        }
-    }
-}
+use super::PydanticCustomError;
 
 #[pyfunction]
 pub fn list_all_errors(py: Python) -> PyResult<&PyList> {
     let mut errors: Vec<&PyDict> = Vec::with_capacity(100);
     for error_type in ErrorType::iter() {
         if !matches!(error_type, ErrorType::CustomError { .. }) {
             let d = PyDict::new(py);
             d.set_item("type", error_type.to_string())?;
             let message_template_python = error_type.message_template_python();
             d.set_item("message_template_python", message_template_python)?;
             d.set_item(
                 "example_message_python",
-                error_type.render_message(py, &ErrorMode::Python)?,
+                error_type.render_message(py, InputType::Python)?,
             )?;
             let message_template_json = error_type.message_template_json();
             if message_template_python != message_template_json {
                 d.set_item("message_template_json", message_template_json)?;
-                d.set_item("example_message_json", error_type.render_message(py, &ErrorMode::Json)?)?;
+                d.set_item("example_message_json", error_type.render_message(py, InputType::Json)?)?;
             }
             d.set_item("example_context", error_type.py_dict(py)?)?;
             errors.push(d);
         }
     }
     Ok(PyList::new(py, errors))
 }
@@ -619,18 +602,18 @@
     pub fn type_string(&self) -> String {
         match self {
             Self::CustomError { error_type, .. } => error_type.clone(),
             _ => self.to_string(),
         }
     }
 
-    pub fn render_message(&self, py: Python, error_mode: &ErrorMode) -> PyResult<String> {
-        let tmpl = match error_mode {
-            ErrorMode::Python => self.message_template_python(),
-            ErrorMode::Json => self.message_template_json(),
+    pub fn render_message(&self, py: Python, input_type: InputType) -> PyResult<String> {
+        let tmpl = match input_type {
+            InputType::Python => self.message_template_python(),
+            _ => self.message_template_json(),
         };
         match self {
             Self::NoSuchAttribute { attribute, .. } => render!(tmpl, attribute),
             Self::JsonInvalid { error, .. } => render!(tmpl, error),
             Self::GetAttributeError { error, .. } => render!(tmpl, error),
             Self::ModelType { class_name, .. } => render!(tmpl, class_name),
             Self::DataclassType { class_name, .. } => render!(tmpl, class_name),
```

### Comparing `pydantic_core-2.8.0/src/errors/validation_exception.rs` & `pydantic_core-2.9.0/src/errors/validation_exception.rs`

 * *Files 5% similar despite different names*

```diff
@@ -12,64 +12,63 @@
 use serde::{Serialize, Serializer};
 
 use serde_json::ser::PrettyFormatter;
 
 use crate::build_tools::py_schema_error_type;
 use crate::errors::LocItem;
 use crate::get_pydantic_version;
+use crate::input::InputType;
 use crate::serializers::{SerMode, SerializationState};
 use crate::tools::{safe_repr, SchemaDict};
 
 use super::line_error::ValLineError;
 use super::location::Location;
-use super::types::{ErrorMode, ErrorType};
+use super::types::ErrorType;
 use super::value_exception::PydanticCustomError;
 use super::{InputValue, ValError};
 
 #[pyclass(extends=PyValueError, module="pydantic_core._pydantic_core")]
 #[derive(Clone)]
 #[cfg_attr(debug_assertions, derive(Debug))]
 pub struct ValidationError {
     line_errors: Vec<PyLineError>,
     title: PyObject,
-    error_mode: ErrorMode,
+    input_type: InputType,
     hide_input: bool,
 }
 
 impl ValidationError {
-    pub fn new(line_errors: Vec<PyLineError>, title: PyObject, error_mode: ErrorMode, hide_input: bool) -> Self {
+    pub fn new(line_errors: Vec<PyLineError>, title: PyObject, input_type: InputType, hide_input: bool) -> Self {
         Self {
             line_errors,
             title,
-            error_mode,
+            input_type,
             hide_input,
         }
     }
 
     pub fn from_val_error(
         py: Python,
         title: PyObject,
-        error_mode: ErrorMode,
+        input_type: InputType,
         error: ValError,
         outer_location: Option<LocItem>,
         hide_input: bool,
         validation_error_cause: bool,
     ) -> PyErr {
         match error {
             ValError::LineErrors(raw_errors) => {
                 let line_errors: Vec<PyLineError> = match outer_location {
                     Some(outer_location) => raw_errors
                         .into_iter()
                         .map(|e| e.with_outer_location(outer_location.clone()).into_py(py))
                         .collect(),
                     None => raw_errors.into_iter().map(|e| e.into_py(py)).collect(),
                 };
-
-                let validation_error = Self::new(line_errors, title, error_mode, hide_input);
-
+                let validation_error = Self::new(line_errors, title, input_type, hide_input);
                 match Py::new(py, validation_error) {
                     Ok(err) => {
                         if validation_error_cause {
                             // Will return an import error if the backport was needed and not installed:
                             if let Some(cause_problem) = ValidationError::maybe_add_cause(err.borrow(py), py) {
                                 return cause_problem;
                             }
@@ -83,15 +82,15 @@
             ValError::Omit => Self::omit_error(),
             ValError::UseDefault => Self::use_default_error(),
         }
     }
 
     pub fn display(&self, py: Python, prefix_override: Option<&'static str>, hide_input: bool) -> String {
         let url_prefix = get_url_prefix(py, include_url_env(py));
-        let line_errors = pretty_py_line_errors(py, &self.error_mode, self.line_errors.iter(), url_prefix, hide_input);
+        let line_errors = pretty_py_line_errors(py, self.input_type, self.line_errors.iter(), url_prefix, hide_input);
         if let Some(prefix) = prefix_override {
             format!("{prefix}\n{line_errors}")
         } else {
             let count = self.line_errors.len();
             let plural = if count == 1 { "" } else { "s" };
             let title: &str = self.title.extract(py).unwrap();
             format!("{count} validation error{plural} for {title}\n{line_errors}")
@@ -234,86 +233,94 @@
             .into()
     }
 }
 
 #[pymethods]
 impl ValidationError {
     #[staticmethod]
-    #[pyo3(signature = (title, line_errors, error_mode="python", hide_input=false))]
+    #[pyo3(signature = (title, line_errors, input_type="python", hide_input=false))]
     fn from_exception_data(
         py: Python,
         title: PyObject,
         line_errors: &PyList,
-        error_mode: &str,
+        input_type: &str,
         hide_input: bool,
     ) -> PyResult<Py<Self>> {
         Py::new(
             py,
             Self {
                 line_errors: line_errors.iter().map(PyLineError::try_from).collect::<PyResult<_>>()?,
                 title,
-                error_mode: ErrorMode::try_from(error_mode)?,
+                input_type: InputType::try_from(input_type)?,
                 hide_input,
             },
         )
     }
 
     #[getter]
     fn title(&self, py: Python) -> PyObject {
         self.title.clone_ref(py)
     }
 
     pub fn error_count(&self) -> usize {
         self.line_errors.len()
     }
 
-    #[pyo3(signature = (*, include_url = true, include_context = true))]
-    pub fn errors(&self, py: Python, include_url: bool, include_context: bool) -> PyResult<Py<PyList>> {
+    #[pyo3(signature = (*, include_url = true, include_context = true, include_input = true))]
+    pub fn errors(
+        &self,
+        py: Python,
+        include_url: bool,
+        include_context: bool,
+        include_input: bool,
+    ) -> PyResult<Py<PyList>> {
         let url_prefix = get_url_prefix(py, include_url);
         let mut iteration_error = None;
         let list = PyList::new(
             py,
             // PyList::new takes ExactSizeIterator, so if an error occurs during iteration we
             // fill the list with None before returning the error; the list will then be thrown
             // away safely.
             self.line_errors.iter().map(|e| -> PyObject {
                 if iteration_error.is_some() {
                     return py.None();
                 }
-                e.as_dict(py, url_prefix, include_context, &self.error_mode)
+                e.as_dict(py, url_prefix, include_context, self.input_type, include_input)
                     .unwrap_or_else(|err| {
                         iteration_error = Some(err);
                         py.None()
                     })
             }),
         );
         if let Some(err) = iteration_error {
             Err(err)
         } else {
             Ok(list.into())
         }
     }
 
-    #[pyo3(signature = (*, indent = None, include_url = true, include_context = true))]
+    #[pyo3(signature = (*, indent = None, include_url = true, include_context = true, include_input = true))]
     pub fn json<'py>(
         &self,
         py: Python<'py>,
         indent: Option<usize>,
         include_url: bool,
         include_context: bool,
+        include_input: bool,
     ) -> PyResult<&'py PyString> {
         let state = SerializationState::new("iso8601", "utf8")?;
         let extra = state.extra(py, &SerMode::Json, true, false, false, true, None);
         let serializer = ValidationErrorSerializer {
             py,
             line_errors: &self.line_errors,
             url_prefix: get_url_prefix(py, include_url),
             include_context,
+            include_input,
             extra: &extra,
-            error_mode: &self.error_mode,
+            input_type: &self.input_type,
         };
 
         let writer: Vec<u8> = Vec::with_capacity(self.line_errors.len() * 200);
         let bytes = match indent {
             Some(indent) => {
                 let indent = vec![b' '; indent];
                 let formatter = PrettyFormatter::with_indent(&indent);
@@ -383,21 +390,21 @@
             write!($out, ", input_value={}", $value)?;
         }
     };
 }
 
 pub fn pretty_py_line_errors<'a>(
     py: Python,
-    error_mode: &ErrorMode,
+    input_type: InputType,
     line_errors_iter: impl Iterator<Item = &'a PyLineError>,
     url_prefix: Option<&str>,
     hide_input: bool,
 ) -> String {
     line_errors_iter
-        .map(|i| i.pretty(py, error_mode, url_prefix, hide_input))
+        .map(|i| i.pretty(py, input_type, url_prefix, hide_input))
         .collect::<Result<Vec<_>, _>>()
         .unwrap_or_else(|err| vec![format!("[error formatting line errors: {err}]")])
         .join("\n")
 }
 
 /// `PyLineError` are the public version of `ValLineError`, as help and used in `ValidationError`s
 #[pyclass]
@@ -473,21 +480,24 @@
     }
 
     pub fn as_dict(
         &self,
         py: Python,
         url_prefix: Option<&str>,
         include_context: bool,
-        error_mode: &ErrorMode,
+        input_type: InputType,
+        include_input: bool,
     ) -> PyResult<PyObject> {
         let dict = PyDict::new(py);
         dict.set_item("type", self.error_type.type_string())?;
         dict.set_item("loc", self.location.to_object(py))?;
-        dict.set_item("msg", self.error_type.render_message(py, error_mode)?)?;
-        dict.set_item("input", &self.input_value)?;
+        dict.set_item("msg", self.error_type.render_message(py, input_type)?)?;
+        if include_input {
+            dict.set_item("input", &self.input_value)?;
+        }
         if include_context {
             if let Some(context) = self.error_type.py_dict(py)? {
                 dict.set_item("ctx", context)?;
             }
         }
         if let Some(url_prefix) = url_prefix {
             match self.error_type {
@@ -501,22 +511,22 @@
         }
         Ok(dict.into_py(py))
     }
 
     fn pretty(
         &self,
         py: Python,
-        error_mode: &ErrorMode,
+        input_type: InputType,
         url_prefix: Option<&str>,
         hide_input: bool,
     ) -> Result<String, fmt::Error> {
         let mut output = String::with_capacity(200);
         write!(output, "{}", self.location)?;
 
-        let message = match self.error_type.render_message(py, error_mode) {
+        let message = match self.error_type.render_message(py, input_type) {
             Ok(message) => message,
             Err(err) => format!("(error rendering message: {err})"),
         };
         write!(output, "  {message} [type={}", self.error_type.type_string())?;
 
         if !hide_input {
             let input_value = self.input_value.as_ref(py);
@@ -560,78 +570,80 @@
 }
 
 struct ValidationErrorSerializer<'py> {
     py: Python<'py>,
     line_errors: &'py [PyLineError],
     url_prefix: Option<&'py str>,
     include_context: bool,
+    include_input: bool,
     extra: &'py crate::serializers::Extra<'py>,
-    error_mode: &'py ErrorMode,
+    input_type: &'py InputType,
 }
 
 impl<'py> Serialize for ValidationErrorSerializer<'py> {
     fn serialize<S>(&self, serializer: S) -> Result<S::Ok, S::Error>
     where
         S: Serializer,
     {
         let mut seq = serializer.serialize_seq(Some(self.line_errors.len()))?;
         for line_error in self.line_errors {
             let line_s = PyLineErrorSerializer {
                 py: self.py,
                 line_error,
                 url_prefix: self.url_prefix,
                 include_context: self.include_context,
+                include_input: self.include_input,
                 extra: self.extra,
-                error_mode: self.error_mode,
+                input_type: self.input_type,
             };
             seq.serialize_element(&line_s)?;
         }
         seq.end()
     }
 }
 
 struct PyLineErrorSerializer<'py> {
     py: Python<'py>,
     line_error: &'py PyLineError,
     url_prefix: Option<&'py str>,
     include_context: bool,
+    include_input: bool,
     extra: &'py crate::serializers::Extra<'py>,
-    error_mode: &'py ErrorMode,
+    input_type: &'py InputType,
 }
 
 impl<'py> Serialize for PyLineErrorSerializer<'py> {
     fn serialize<S>(&self, serializer: S) -> Result<S::Ok, S::Error>
     where
         S: Serializer,
     {
         let py = self.py;
-        let mut size = 4;
-        if self.url_prefix.is_some() {
-            size += 1;
-        }
-        if self.include_context {
-            size += 1;
-        }
+        let size = 3 + [self.url_prefix.is_some(), self.include_context, self.include_input]
+            .into_iter()
+            .filter(|b| *b)
+            .count();
         let mut map = serializer.serialize_map(Some(size))?;
 
         map.serialize_entry("type", &self.line_error.error_type.type_string())?;
 
         map.serialize_entry("loc", &self.line_error.location)?;
 
         let msg = self
             .line_error
             .error_type
-            .render_message(py, self.error_mode)
+            .render_message(py, *self.input_type)
             .map_err(py_err_json::<S>)?;
         map.serialize_entry("msg", &msg)?;
 
-        map.serialize_entry(
-            "input",
-            &self.extra.serialize_infer(self.line_error.input_value.as_ref(py)),
-        )?;
+        if self.include_input {
+            map.serialize_entry(
+                "input",
+                &self.extra.serialize_infer(self.line_error.input_value.as_ref(py)),
+            )?;
+        }
 
         if self.include_context {
             if let Some(context) = self.line_error.error_type.py_dict(py).map_err(py_err_json::<S>)? {
                 map.serialize_entry("ctx", &self.extra.serialize_infer(context.as_ref(py)))?;
             }
         }
         if let Some(url_prefix) = self.url_prefix {
```

### Comparing `pydantic_core-2.8.0/src/errors/value_exception.rs` & `pydantic_core-2.9.0/src/errors/value_exception.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-use crate::errors::ErrorMode;
 use pyo3::exceptions::{PyException, PyValueError};
 use pyo3::prelude::*;
 use pyo3::types::{PyDict, PyString};
 
-use crate::input::Input;
+use crate::input::{Input, InputType};
 use crate::tools::extract_i64;
 
 use super::{ErrorType, ValError};
 
 #[pyclass(extends=PyException, module="pydantic_core._pydantic_core")]
 #[derive(Debug, Clone)]
 pub struct PydanticOmit {}
@@ -160,15 +159,15 @@
 
     #[getter]
     pub fn context(&self, py: Python) -> PyResult<Option<Py<PyDict>>> {
         self.error_type.py_dict(py)
     }
 
     pub fn message(&self, py: Python) -> PyResult<String> {
-        self.error_type.render_message(py, &ErrorMode::Python)
+        self.error_type.render_message(py, InputType::Python)
     }
 
     fn __str__(&self, py: Python) -> PyResult<String> {
         self.message(py)
     }
 
     fn __repr__(&self, py: Python) -> PyResult<String> {
```

### Comparing `pydantic_core-2.8.0/src/input/datetime.rs` & `pydantic_core-2.9.0/src/input/datetime.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/input/input_abstract.rs` & `pydantic_core-2.9.0/src/input/input_abstract.rs`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,47 @@
 use std::fmt;
 
+use pyo3::exceptions::PyValueError;
 use pyo3::types::{PyDict, PyType};
 use pyo3::{intern, prelude::*};
 
 use crate::errors::{InputValue, LocItem, ValResult};
+use crate::tools::py_err;
 use crate::{PyMultiHostUrl, PyUrl};
 
 use super::datetime::{EitherDate, EitherDateTime, EitherTime, EitherTimedelta};
 use super::return_enums::{EitherBytes, EitherInt, EitherString};
 use super::{EitherFloat, GenericArguments, GenericIterable, GenericIterator, GenericMapping, JsonInput};
 
 #[derive(Debug, Clone, Copy)]
 pub enum InputType {
     Python,
     Json,
+    String,
 }
 
 impl IntoPy<PyObject> for InputType {
     fn into_py(self, py: Python<'_>) -> PyObject {
         match self {
             Self::Json => intern!(py, "json").into(),
             Self::Python => intern!(py, "python").into(),
+            Self::String => intern!(py, "string").into(),
+        }
+    }
+}
+
+impl TryFrom<&str> for InputType {
+    type Error = PyErr;
+
+    fn try_from(error_mode: &str) -> PyResult<Self> {
+        match error_mode {
+            "python" => Ok(Self::Python),
+            "json" => Ok(Self::Json),
+            "string" => Ok(Self::String),
+            s => py_err!(PyValueError; "Invalid error mode: {}", s),
         }
     }
 }
 
 /// all types have three methods: `validate_*`, `strict_*`, `lax_*`
 /// the convention is to either implement:
 /// * `strict_*` & `lax_*` if they have different behavior
@@ -34,15 +51,17 @@
 
     fn as_error_value(&'a self) -> InputValue<'a>;
 
     fn identity(&self) -> Option<usize> {
         None
     }
 
-    fn is_none(&self) -> bool;
+    fn is_none(&self) -> bool {
+        false
+    }
 
     fn input_is_instance(&self, _class: &PyType) -> Option<&PyAny> {
         None
     }
 
     fn is_python(&self) -> bool {
         false
@@ -68,24 +87,24 @@
 
     fn validate_args(&'a self) -> ValResult<'a, GenericArguments<'a>>;
 
     fn validate_dataclass_args(&'a self, dataclass_name: &str) -> ValResult<'a, GenericArguments<'a>>;
 
     fn parse_json(&'a self) -> ValResult<'a, JsonInput>;
 
-    fn validate_str(&'a self, strict: bool) -> ValResult<EitherString<'a>> {
+    fn validate_str(&'a self, strict: bool, coerce_numbers_to_str: bool) -> ValResult<EitherString<'a>> {
         if strict {
             self.strict_str()
         } else {
-            self.lax_str()
+            self.lax_str(coerce_numbers_to_str)
         }
     }
     fn strict_str(&'a self) -> ValResult<EitherString<'a>>;
     #[cfg_attr(has_coverage_attribute, coverage(off))]
-    fn lax_str(&'a self) -> ValResult<EitherString<'a>> {
+    fn lax_str(&'a self, _coerce_numbers_to_str: bool) -> ValResult<EitherString<'a>> {
         self.strict_str()
     }
 
     fn validate_bytes(&'a self, strict: bool) -> ValResult<EitherBytes<'a>> {
         if strict {
             self.strict_bytes()
         } else {
@@ -316,7 +335,23 @@
     fn lax_timedelta(
         &self,
         microseconds_overflow_behavior: speedate::MicrosecondsPrecisionOverflowBehavior,
     ) -> ValResult<EitherTimedelta> {
         self.strict_timedelta(microseconds_overflow_behavior)
     }
 }
+
+/// The problem to solve here is that iterating a `StringMapping` returns an owned
+/// `StringMapping`, but all the other iterators return references. By introducing
+/// this trait we abstract over whether the return value from the iterator is owned
+/// or borrowed; all we care about is that we can borrow it again with `borrow_input`
+/// for some lifetime 'a.
+///
+/// This lifetime `'a` is shorter than the original lifetime `'data` of the input,
+/// which is only a problem in error branches. To resolve we have to call `into_owned`
+/// to extend out the lifetime to match the original input.
+pub trait BorrowInput {
+    type Input<'a>: Input<'a>
+    where
+        Self: 'a;
+    fn borrow_input(&self) -> &Self::Input<'_>;
+}
```

### Comparing `pydantic_core-2.8.0/src/input/input_json.rs` & `pydantic_core-2.9.0/src/input/input_json.rs`

 * *Files 10% similar despite different names*

```diff
@@ -8,19 +8,18 @@
 use crate::errors::{ErrorType, ErrorTypeDefaults, InputValue, LocItem, ValError, ValResult};
 use crate::validators::decimal::create_decimal;
 
 use super::datetime::{
     bytes_as_date, bytes_as_datetime, bytes_as_time, bytes_as_timedelta, float_as_datetime, float_as_duration,
     float_as_time, int_as_datetime, int_as_duration, int_as_time, EitherDate, EitherDateTime, EitherTime,
 };
-use super::parse_json::JsonArray;
-use super::shared::{float_as_int, int_as_bool, map_json_err, str_as_bool, str_as_float, str_as_int};
+use super::shared::{float_as_int, int_as_bool, map_json_err, str_as_bool, str_as_float, str_as_int, string_to_vec};
 use super::{
-    EitherBytes, EitherFloat, EitherInt, EitherString, EitherTimedelta, GenericArguments, GenericIterable,
-    GenericIterator, GenericMapping, Input, JsonArgs, JsonInput,
+    BorrowInput, EitherBytes, EitherFloat, EitherInt, EitherString, EitherTimedelta, GenericArguments, GenericIterable,
+    GenericIterator, GenericMapping, Input, JsonArgs, JsonArray, JsonInput,
 };
 
 impl<'a> Input<'a> for JsonInput {
     /// This is required by since JSON object keys are always strings, I don't think it can be called
     #[cfg_attr(has_coverage_attribute, coverage(off))]
     fn as_loc_item(&self) -> LocItem {
         match self {
@@ -85,17 +84,21 @@
 
     fn strict_str(&'a self) -> ValResult<EitherString<'a>> {
         match self {
             JsonInput::String(s) => Ok(s.as_str().into()),
             _ => Err(ValError::new(ErrorTypeDefaults::StringType, self)),
         }
     }
-    fn lax_str(&'a self) -> ValResult<EitherString<'a>> {
+    fn lax_str(&'a self, coerce_numbers_to_str: bool) -> ValResult<EitherString<'a>> {
         match self {
             JsonInput::String(s) => Ok(s.as_str().into()),
+            JsonInput::BigInt(v) if coerce_numbers_to_str => Ok(v.to_string().into()),
+            JsonInput::Float(v) if coerce_numbers_to_str => Ok(v.to_string().into()),
+            JsonInput::Int(v) if coerce_numbers_to_str => Ok(v.to_string().into()),
+            JsonInput::Uint(v) if coerce_numbers_to_str => Ok(v.to_string().into()),
             _ => Err(ValError::new(ErrorTypeDefaults::StringType, self)),
         }
     }
 
     fn validate_bytes(&'a self, _strict: bool) -> ValResult<EitherBytes<'a>> {
         match self {
             JsonInput::String(s) => Ok(s.as_bytes().into()),
@@ -351,29 +354,33 @@
             JsonInput::Int(v) => Ok(int_as_duration(self, *v)?.into()),
             JsonInput::Float(v) => Ok(float_as_duration(self, *v)?.into()),
             _ => Err(ValError::new(ErrorTypeDefaults::TimeDeltaType, self)),
         }
     }
 }
 
+impl BorrowInput for &'_ JsonInput {
+    type Input<'a> = JsonInput where Self: 'a;
+    fn borrow_input(&self) -> &Self::Input<'_> {
+        self
+    }
+}
+
+/// TODO: it would be good to get JsonInput and StringMapping string variants to go through this
+/// implementation
 /// Required for Dict keys so the string can behave like an Input
 impl<'a> Input<'a> for String {
     fn as_loc_item(&self) -> LocItem {
         self.to_string().into()
     }
 
     fn as_error_value(&'a self) -> InputValue<'a> {
         InputValue::String(self)
     }
 
-    #[cfg_attr(has_coverage_attribute, coverage(off))]
-    fn is_none(&self) -> bool {
-        false
-    }
-
     fn as_kwargs(&'a self, _py: Python<'a>) -> Option<&'a PyDict> {
         None
     }
 
     #[cfg_attr(has_coverage_attribute, coverage(off))]
     fn validate_args(&'a self) -> ValResult<'a, GenericArguments<'a>> {
         Err(ValError::new(ErrorTypeDefaults::ArgumentsType, self))
@@ -391,165 +398,109 @@
         ))
     }
 
     fn parse_json(&'a self) -> ValResult<'a, JsonInput> {
         serde_json::from_str(self.as_str()).map_err(|e| map_json_err(self, e))
     }
 
-    fn validate_str(&'a self, _strict: bool) -> ValResult<EitherString<'a>> {
-        Ok(self.as_str().into())
-    }
     fn strict_str(&'a self) -> ValResult<EitherString<'a>> {
-        self.validate_str(false)
+        Ok(self.as_str().into())
     }
 
-    fn validate_bytes(&'a self, _strict: bool) -> ValResult<EitherBytes<'a>> {
-        Ok(self.as_bytes().into())
-    }
-    #[cfg_attr(has_coverage_attribute, coverage(off))]
     fn strict_bytes(&'a self) -> ValResult<EitherBytes<'a>> {
-        self.validate_bytes(false)
+        Ok(self.as_bytes().into())
     }
 
     fn strict_bool(&self) -> ValResult<bool> {
-        Err(ValError::new(ErrorTypeDefaults::BoolType, self))
-    }
-    fn lax_bool(&self) -> ValResult<bool> {
         str_as_bool(self, self)
     }
 
     fn strict_int(&'a self) -> ValResult<EitherInt<'a>> {
-        Err(ValError::new(ErrorTypeDefaults::IntType, self))
-    }
-    fn lax_int(&'a self) -> ValResult<EitherInt<'a>> {
         match self.parse() {
             Ok(i) => Ok(EitherInt::I64(i)),
             Err(_) => Err(ValError::new(ErrorTypeDefaults::IntParsing, self)),
         }
     }
 
-    #[cfg_attr(has_coverage_attribute, coverage(off))]
     fn ultra_strict_float(&'a self) -> ValResult<EitherFloat<'a>> {
         self.strict_float()
     }
-    #[cfg_attr(has_coverage_attribute, coverage(off))]
     fn strict_float(&'a self) -> ValResult<EitherFloat<'a>> {
-        Err(ValError::new(ErrorTypeDefaults::FloatType, self))
-    }
-    fn lax_float(&'a self) -> ValResult<EitherFloat<'a>> {
         str_as_float(self, self)
     }
 
     fn strict_decimal(&'a self, py: Python<'a>) -> ValResult<&'a PyAny> {
         create_decimal(self.to_object(py).into_ref(py), self, py)
     }
 
     #[cfg_attr(has_coverage_attribute, coverage(off))]
-    fn validate_dict(&'a self, _strict: bool) -> ValResult<GenericMapping<'a>> {
-        Err(ValError::new(ErrorTypeDefaults::DictType, self))
-    }
-    #[cfg_attr(has_coverage_attribute, coverage(off))]
     fn strict_dict(&'a self) -> ValResult<GenericMapping<'a>> {
-        self.validate_dict(false)
+        Err(ValError::new(ErrorTypeDefaults::DictType, self))
     }
 
     #[cfg_attr(has_coverage_attribute, coverage(off))]
-    fn validate_list(&'a self, _strict: bool) -> ValResult<GenericIterable<'a>> {
-        Err(ValError::new(ErrorTypeDefaults::ListType, self))
-    }
-    #[cfg_attr(has_coverage_attribute, coverage(off))]
     fn strict_list(&'a self) -> ValResult<GenericIterable<'a>> {
-        self.validate_list(false)
+        Err(ValError::new(ErrorTypeDefaults::ListType, self))
     }
 
     #[cfg_attr(has_coverage_attribute, coverage(off))]
-    fn validate_tuple(&'a self, _strict: bool) -> ValResult<GenericIterable<'a>> {
-        Err(ValError::new(ErrorTypeDefaults::TupleType, self))
-    }
-    #[cfg_attr(has_coverage_attribute, coverage(off))]
     fn strict_tuple(&'a self) -> ValResult<GenericIterable<'a>> {
-        self.validate_tuple(false)
+        Err(ValError::new(ErrorTypeDefaults::TupleType, self))
     }
 
     #[cfg_attr(has_coverage_attribute, coverage(off))]
-    fn validate_set(&'a self, _strict: bool) -> ValResult<GenericIterable<'a>> {
-        Err(ValError::new(ErrorTypeDefaults::SetType, self))
-    }
-    #[cfg_attr(has_coverage_attribute, coverage(off))]
     fn strict_set(&'a self) -> ValResult<GenericIterable<'a>> {
-        self.validate_set(false)
+        Err(ValError::new(ErrorTypeDefaults::SetType, self))
     }
 
     #[cfg_attr(has_coverage_attribute, coverage(off))]
-    fn validate_frozenset(&'a self, _strict: bool) -> ValResult<GenericIterable<'a>> {
-        Err(ValError::new(ErrorTypeDefaults::FrozenSetType, self))
-    }
-    #[cfg_attr(has_coverage_attribute, coverage(off))]
     fn strict_frozenset(&'a self) -> ValResult<GenericIterable<'a>> {
-        self.validate_frozenset(false)
+        Err(ValError::new(ErrorTypeDefaults::FrozenSetType, self))
     }
 
     fn extract_generic_iterable(&'a self) -> ValResult<GenericIterable<'a>> {
         Ok(GenericIterable::JsonString(self))
     }
 
     fn validate_iter(&self) -> ValResult<GenericIterator> {
         Ok(string_to_vec(self).into())
     }
 
-    fn validate_date(&self, _strict: bool) -> ValResult<EitherDate> {
-        bytes_as_date(self, self.as_bytes())
-    }
-    #[cfg_attr(has_coverage_attribute, coverage(off))]
     fn strict_date(&self) -> ValResult<EitherDate> {
-        self.validate_date(false)
+        bytes_as_date(self, self.as_bytes())
     }
 
-    fn validate_time(
-        &self,
-        _strict: bool,
-        microseconds_overflow_behavior: speedate::MicrosecondsPrecisionOverflowBehavior,
-    ) -> ValResult<EitherTime> {
-        bytes_as_time(self, self.as_bytes(), microseconds_overflow_behavior)
-    }
-    #[cfg_attr(has_coverage_attribute, coverage(off))]
     fn strict_time(
         &self,
-        microseconds_overflow_behavior: speedate::MicrosecondsPrecisionOverflowBehavior,
+        microseconds_overflow_behavior: MicrosecondsPrecisionOverflowBehavior,
     ) -> ValResult<EitherTime> {
-        self.validate_time(false, microseconds_overflow_behavior)
+        bytes_as_time(self, self.as_bytes(), microseconds_overflow_behavior)
     }
 
-    fn validate_datetime(
-        &self,
-        _strict: bool,
-        microseconds_overflow_behavior: speedate::MicrosecondsPrecisionOverflowBehavior,
-    ) -> ValResult<EitherDateTime> {
-        bytes_as_datetime(self, self.as_bytes(), microseconds_overflow_behavior)
-    }
-    #[cfg_attr(has_coverage_attribute, coverage(off))]
     fn strict_datetime(
         &self,
-        microseconds_overflow_behavior: speedate::MicrosecondsPrecisionOverflowBehavior,
+        microseconds_overflow_behavior: MicrosecondsPrecisionOverflowBehavior,
     ) -> ValResult<EitherDateTime> {
-        self.validate_datetime(false, microseconds_overflow_behavior)
+        bytes_as_datetime(self, self.as_bytes(), microseconds_overflow_behavior)
     }
 
-    fn validate_timedelta(
+    fn strict_timedelta(
         &self,
-        _strict: bool,
-        microseconds_overflow_behavior: speedate::MicrosecondsPrecisionOverflowBehavior,
+        microseconds_overflow_behavior: MicrosecondsPrecisionOverflowBehavior,
     ) -> ValResult<EitherTimedelta> {
         bytes_as_timedelta(self, self.as_bytes(), microseconds_overflow_behavior)
     }
-    #[cfg_attr(has_coverage_attribute, coverage(off))]
-    fn strict_timedelta(
-        &self,
-        microseconds_overflow_behavior: speedate::MicrosecondsPrecisionOverflowBehavior,
-    ) -> ValResult<EitherTimedelta> {
-        self.validate_timedelta(false, microseconds_overflow_behavior)
+}
+
+impl BorrowInput for &'_ String {
+    type Input<'a> = String where Self: 'a;
+    fn borrow_input(&self) -> &Self::Input<'_> {
+        self
     }
 }
 
-fn string_to_vec(s: &str) -> JsonArray {
-    JsonArray::new(s.chars().map(|c| JsonInput::String(c.to_string())).collect())
+impl BorrowInput for String {
+    type Input<'a> = String where Self: 'a;
+    fn borrow_input(&self) -> &Self::Input<'_> {
+        self
+    }
 }
```

### Comparing `pydantic_core-2.8.0/src/input/input_python.rs` & `pydantic_core-2.9.0/src/input/input_python.rs`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 use super::datetime::{
     bytes_as_date, bytes_as_datetime, bytes_as_time, bytes_as_timedelta, date_as_datetime, float_as_datetime,
     float_as_duration, float_as_time, int_as_datetime, int_as_duration, int_as_time, EitherDate, EitherDateTime,
     EitherTime,
 };
 use super::shared::{decimal_as_int, float_as_int, int_as_bool, map_json_err, str_as_bool, str_as_float, str_as_int};
 use super::{
-    py_string_str, EitherBytes, EitherFloat, EitherInt, EitherString, EitherTimedelta, GenericArguments,
+    py_string_str, BorrowInput, EitherBytes, EitherFloat, EitherInt, EitherString, EitherTimedelta, GenericArguments,
     GenericIterable, GenericIterator, GenericMapping, Input, JsonInput, PyArgs,
 };
 
 #[cfg(not(PyPy))]
 macro_rules! extract_dict_keys {
     ($py:expr, $obj:ident) => {
         $obj.downcast::<PyDictKeys>()
@@ -180,54 +180,54 @@
         }
     }
 
     fn parse_json(&'a self) -> ValResult<'a, JsonInput> {
         if let Ok(py_bytes) = self.downcast::<PyBytes>() {
             serde_json::from_slice(py_bytes.as_bytes()).map_err(|e| map_json_err(self, e))
         } else if let Ok(py_str) = self.downcast::<PyString>() {
-            let str = py_str.to_str()?;
+            let str = py_string_str(py_str)?;
             serde_json::from_str(str).map_err(|e| map_json_err(self, e))
         } else if let Ok(py_byte_array) = self.downcast::<PyByteArray>() {
             // Safety: from_slice does not run arbitrary Python code and the GIL is held so the
             // bytes array will not be mutated while from_slice is reading it
             serde_json::from_slice(unsafe { py_byte_array.as_bytes() }).map_err(|e| map_json_err(self, e))
         } else {
             Err(ValError::new(ErrorTypeDefaults::JsonType, self))
         }
     }
 
     fn strict_str(&'a self) -> ValResult<EitherString<'a>> {
-        if let Ok(py_str) = <PyString as PyTryFrom>::try_from_exact(self) {
+        if let Ok(py_str) = PyString::try_from_exact(self) {
             Ok(py_str.into())
         } else if let Ok(py_str) = self.downcast::<PyString>() {
             // force to a rust string to make sure behavior is consistent whether or not we go via a
             // rust string in StrConstrainedValidator - e.g. to_lower
             Ok(py_string_str(py_str)?.into())
         } else {
             Err(ValError::new(ErrorTypeDefaults::StringType, self))
         }
     }
 
     fn exact_str(&'a self) -> ValResult<EitherString<'a>> {
-        if let Ok(py_str) = <PyString as PyTryFrom>::try_from_exact(self) {
+        if let Ok(py_str) = PyString::try_from_exact(self) {
             Ok(EitherString::Py(py_str))
         } else {
             Err(ValError::new(ErrorTypeDefaults::IntType, self))
         }
     }
 
     fn exact_int(&'a self) -> ValResult<EitherInt<'a>> {
         if PyInt::is_exact_type_of(self) {
             Ok(EitherInt::Py(self))
         } else {
             Err(ValError::new(ErrorTypeDefaults::IntType, self))
         }
     }
 
-    fn lax_str(&'a self) -> ValResult<EitherString<'a>> {
+    fn lax_str(&'a self, coerce_numbers_to_str: bool) -> ValResult<EitherString<'a>> {
         if let Ok(py_str) = <PyString as PyTryFrom>::try_from_exact(self) {
             Ok(py_str.into())
         } else if let Ok(py_str) = self.downcast::<PyString>() {
             // force to a rust string to make sure behaviour is consistent whether or not we go via a
             // rust string in StrConstrainedValidator - e.g. to_lower
             Ok(py_string_str(py_str)?.into())
         } else if let Ok(bytes) = self.downcast::<PyBytes>() {
@@ -242,14 +242,23 @@
             let s = match from_utf8(unsafe { py_byte_array.as_bytes() }) {
                 // Why Python not Rust? to avoid an unnecessary allocation on the Rust side, the
                 // final output needs to be Python anyway.
                 Ok(s) => PyString::new(self.py(), s),
                 Err(_) => return Err(ValError::new(ErrorTypeDefaults::StringUnicode, self)),
             };
             Ok(s.into())
+        } else if coerce_numbers_to_str && {
+            let py = self.py();
+            let decimal_type: Py<PyType> = get_decimal_type(py);
+
+            self.is_instance_of::<PyInt>()
+                || self.is_instance_of::<PyFloat>()
+                || self.is_instance(decimal_type.as_ref(py)).unwrap_or_default()
+        } {
+            Ok(self.str()?.into())
         } else {
             Err(ValError::new(ErrorTypeDefaults::StringType, self))
         }
     }
 
     fn strict_bytes(&'a self) -> ValResult<EitherBytes<'a>> {
         if let Ok(py_bytes) = self.downcast::<PyBytes>() {
@@ -706,14 +715,21 @@
             Ok(float_as_duration(self, float)?.into())
         } else {
             Err(ValError::new(ErrorTypeDefaults::TimeDeltaType, self))
         }
     }
 }
 
+impl BorrowInput for &'_ PyAny {
+    type Input<'a> = PyAny where Self: 'a;
+    fn borrow_input(&self) -> &Self::Input<'_> {
+        self
+    }
+}
+
 /// Best effort check of whether it's likely to make sense to inspect obj for attributes and iterate over it
 /// with `obj.dir()`
 fn from_attributes_applicable(obj: &PyAny) -> bool {
     let module_name = match obj.get_type().getattr(intern!(obj.py(), "__module__")) {
         Ok(module) => match module.extract::<&str>() {
             Ok(s) => s,
             Err(_) => return false,
```

### Comparing `pydantic_core-2.8.0/src/input/parse_json.rs` & `pydantic_core-2.9.0/src/input/parse_json.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/input/return_enums.rs` & `pydantic_core-2.9.0/src/input/return_enums.rs`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 use pyo3::PyTypeInfo;
 use serde::{ser::Error, Serialize, Serializer};
 
 use crate::errors::{py_err_string, ErrorType, ErrorTypeDefaults, InputValue, ValError, ValLineError, ValResult};
 use crate::tools::py_err;
 use crate::validators::{CombinedValidator, ValidationState, Validator};
 
+use super::input_string::StringMapping;
 use super::parse_json::{JsonArray, JsonInput, JsonObject};
 use super::{py_error_on_minusone, Input};
 
 /// Container for all the collections (sized iterable containers) types, which
 /// can mostly be converted to each other in lax mode.
 /// This mostly matches python's definition of `Collection`.
 #[cfg_attr(debug_assertions, derive(Debug))]
@@ -425,14 +426,15 @@
     }
 }
 
 #[cfg_attr(debug_assertions, derive(Debug))]
 pub enum GenericMapping<'a> {
     PyDict(&'a PyDict),
     PyMapping(&'a PyMapping),
+    StringMapping(&'a PyDict),
     PyGetAttr(&'a PyAny, Option<&'a PyDict>),
     JsonObject(&'a JsonObject),
 }
 
 derive_from!(GenericMapping, PyDict, PyDict);
 derive_from!(GenericMapping, PyMapping, PyMapping);
 derive_from!(GenericMapping, PyGetAttr, PyAny, None);
@@ -502,14 +504,46 @@
                 )
             }),
             Err(e) => Err(mapping_err(e, self.iter.py(), self.input)),
         })
     }
 }
 
+pub struct StringMappingGenericIterator<'py> {
+    dict_iter: PyDictIterator<'py>,
+}
+
+impl<'py> StringMappingGenericIterator<'py> {
+    pub fn new(dict: &'py PyDict) -> ValResult<'py, Self> {
+        Ok(Self { dict_iter: dict.iter() })
+    }
+}
+
+impl<'py> Iterator for StringMappingGenericIterator<'py> {
+    // key (the first member of the tuple could be a simple String)
+    type Item = ValResult<'py, (StringMapping<'py>, StringMapping<'py>)>;
+
+    fn next(&mut self) -> Option<Self::Item> {
+        match self.dict_iter.next() {
+            Some((py_key, py_value)) => {
+                let key = match StringMapping::new_key(py_key) {
+                    Ok(key) => key,
+                    Err(e) => return Some(Err(e)),
+                };
+                let value = match StringMapping::new_value(py_value) {
+                    Ok(value) => value,
+                    Err(e) => return Some(Err(e)),
+                };
+                Some(Ok((key, value)))
+            }
+            None => None,
+        }
+    }
+}
+
 pub struct AttributesGenericIterator<'py> {
     object: &'py PyAny,
     // PyO3 should export this type upstream
     attributes_iterator: <&'py PyList as IntoIterator>::IntoIter,
 }
 
 impl<'py> AttributesGenericIterator<'py> {
@@ -687,14 +721,15 @@
     }
 }
 
 #[cfg_attr(debug_assertions, derive(Debug))]
 pub enum GenericArguments<'a> {
     Py(PyArgs<'a>),
     Json(JsonArgs<'a>),
+    StringMapping(&'a PyDict),
 }
 
 impl<'a> From<PyArgs<'a>> for GenericArguments<'a> {
     fn from(s: PyArgs<'a>) -> GenericArguments<'a> {
         Self::Py(s)
     }
 }
@@ -729,14 +764,20 @@
 
 impl<'a> From<&'a str> for EitherString<'a> {
     fn from(data: &'a str) -> Self {
         Self::Cow(Cow::Borrowed(data))
     }
 }
 
+impl<'a> From<String> for EitherString<'a> {
+    fn from(data: String) -> Self {
+        Self::Cow(Cow::Owned(data))
+    }
+}
+
 impl<'a> From<&'a PyString> for EitherString<'a> {
     fn from(date: &'a PyString) -> Self {
         Self::Py(date)
     }
 }
 
 impl<'a> IntoPy<PyObject> for EitherString<'a> {
```

### Comparing `pydantic_core-2.8.0/src/input/shared.rs` & `pydantic_core-2.9.0/src/input/shared.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 use num_bigint::BigInt;
 use pyo3::{intern, PyAny, Python};
 
 use crate::errors::{ErrorType, ErrorTypeDefaults, ValError, ValResult};
-use crate::input::EitherInt;
 
-use super::{EitherFloat, Input};
+use super::parse_json::{JsonArray, JsonInput};
+use super::{EitherFloat, EitherInt, Input};
 
 pub fn map_json_err<'a>(input: &'a impl Input<'a>, error: serde_json::Error) -> ValError<'a> {
     ValError::new(
         ErrorType::JsonInvalid {
             error: error.to_string(),
             context: None,
         },
@@ -146,7 +146,11 @@
         .call_method0(intern!(py, "as_integer_ratio"))?
         .extract::<(&PyAny, &PyAny)>()?;
     if denominator.extract::<i64>().map_or(true, |d| d != 1) {
         return Err(ValError::new(ErrorTypeDefaults::IntFromFloat, input));
     }
     Ok(EitherInt::Py(numerator))
 }
+
+pub fn string_to_vec(s: &str) -> JsonArray {
+    JsonArray::new(s.chars().map(|c| JsonInput::String(c.to_string())).collect())
+}
```

### Comparing `pydantic_core-2.8.0/src/lazy_index_map.rs` & `pydantic_core-2.9.0/src/lazy_index_map.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/lib.rs` & `pydantic_core-2.9.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/lookup_key.rs` & `pydantic_core-2.9.0/src/lookup_key.rs`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 use std::fmt;
 
 use pyo3::exceptions::{PyAttributeError, PyTypeError};
 use pyo3::prelude::*;
 use pyo3::types::{PyDict, PyList, PyMapping, PyString};
 
 use crate::build_tools::py_schema_err;
-use crate::errors::{ErrorType, ValLineError};
-use crate::input::{Input, JsonInput, JsonObject};
+use crate::errors::{py_err_string, ErrorType, ValError, ValLineError, ValResult};
+use crate::input::{Input, JsonInput, JsonObject, StringMapping};
 use crate::tools::{extract_i64, py_err};
 
 /// Used for getting items from python dicts, python objects, or JSON objects, in different ways
 #[derive(Debug, Clone)]
 pub(crate) enum LookupKey {
     /// simply look up a key in a dict, equivalent to `d.get(key)`
     /// we save both the string and pystring to save creating the pystring for python
@@ -105,15 +105,15 @@
             path: LookupPath::from_str(py, key, opt_py_key),
         }
     }
 
     pub fn py_get_dict_item<'data, 's>(
         &'s self,
         dict: &'data PyDict,
-    ) -> PyResult<Option<(&'s LookupPath, &'data PyAny)>> {
+    ) -> ValResult<'data, Option<(&'s LookupPath, &'data PyAny)>> {
         match self {
             Self::Simple { py_key, path, .. } => match dict.get_item(py_key) {
                 Some(value) => Ok(Some((path, value))),
                 None => Ok(None),
             },
             Self::Choice {
                 py_key1,
@@ -139,18 +139,30 @@
                 }
                 // got to the end of path_choices, without a match, return None
                 Ok(None)
             }
         }
     }
 
+    pub fn py_get_string_mapping_item<'data, 's>(
+        &'s self,
+        dict: &'data PyDict,
+    ) -> ValResult<'data, Option<(&'s LookupPath, StringMapping<'data>)>> {
+        if let Some((path, py_any)) = self.py_get_dict_item(dict)? {
+            let value = StringMapping::new_value(py_any)?;
+            Ok(Some((path, value)))
+        } else {
+            Ok(None)
+        }
+    }
+
     pub fn py_get_mapping_item<'data, 's>(
         &'s self,
         dict: &'data PyMapping,
-    ) -> PyResult<Option<(&'s LookupPath, &'data PyAny)>> {
+    ) -> ValResult<'data, Option<(&'s LookupPath, &'data PyAny)>> {
         match self {
             Self::Simple { py_key, path, .. } => match dict.get_item(py_key) {
                 Ok(value) => Ok(Some((path, value))),
                 _ => Ok(None),
             },
             Self::Choice {
                 py_key1,
@@ -180,14 +192,31 @@
         }
     }
 
     pub fn py_get_attr<'data, 's>(
         &'s self,
         obj: &'data PyAny,
         kwargs: Option<&'data PyDict>,
+    ) -> ValResult<'data, Option<(&'s LookupPath, &'data PyAny)>> {
+        match self._py_get_attr(obj, kwargs) {
+            Ok(v) => Ok(v),
+            Err(err) => {
+                let error = py_err_string(obj.py(), err);
+                Err(ValError::new(
+                    ErrorType::GetAttributeError { error, context: None },
+                    obj,
+                ))
+            }
+        }
+    }
+
+    pub fn _py_get_attr<'data, 's>(
+        &'s self,
+        obj: &'data PyAny,
+        kwargs: Option<&'data PyDict>,
     ) -> PyResult<Option<(&'s LookupPath, &'data PyAny)>> {
         if let Some(dict) = kwargs {
             if let Ok(Some(item)) = self.py_get_dict_item(dict) {
                 return Ok(Some(item));
             }
         }
 
@@ -231,15 +260,15 @@
             }
         }
     }
 
     pub fn json_get<'data, 's>(
         &'s self,
         dict: &'data JsonObject,
-    ) -> PyResult<Option<(&'s LookupPath, &'data JsonInput)>> {
+    ) -> ValResult<'data, Option<(&'s LookupPath, &'data JsonInput)>> {
         match self {
             Self::Simple { key, path, .. } => match dict.get(key) {
                 Some(value) => Ok(Some((path, value))),
                 None => Ok(None),
             },
             Self::Choice {
                 key1,
```

### Comparing `pydantic_core-2.8.0/src/py_gc.rs` & `pydantic_core-2.9.0/src/py_gc.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/recursion_guard.rs` & `pydantic_core-2.9.0/src/recursion_guard.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/serializers/computed_fields.rs` & `pydantic_core-2.9.0/src/serializers/computed_fields.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/serializers/config.rs` & `pydantic_core-2.9.0/src/serializers/config.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/serializers/errors.rs` & `pydantic_core-2.9.0/src/serializers/errors.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/serializers/extra.rs` & `pydantic_core-2.9.0/src/serializers/extra.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/serializers/fields.rs` & `pydantic_core-2.9.0/src/serializers/fields.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/serializers/filter.rs` & `pydantic_core-2.9.0/src/serializers/filter.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/serializers/infer.rs` & `pydantic_core-2.9.0/src/serializers/infer.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/serializers/mod.rs` & `pydantic_core-2.9.0/src/serializers/mod.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/serializers/ob_type.rs` & `pydantic_core-2.9.0/src/serializers/ob_type.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/serializers/shared.rs` & `pydantic_core-2.9.0/src/serializers/shared.rs`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 use enum_dispatch::enum_dispatch;
 use serde::Serialize;
 use serde_json::ser::PrettyFormatter;
 
 use crate::build_tools::py_schema_err;
 use crate::build_tools::py_schema_error_type;
-use crate::definitions::DefinitionsBuilder;
+use crate::definitions::{Definitions, DefinitionsBuilder};
 use crate::py_gc::PyGcTraverse;
 use crate::tools::{py_err, SchemaDict};
 
 use super::errors::se_err_py_err;
 use super::extra::Extra;
 use super::infer::infer_json_key;
 use super::ob_type::{IsType, ObType};
@@ -289,15 +289,15 @@
         exclude: Option<&PyAny>,
         extra: &Extra,
     ) -> Result<S::Ok, S::Error>;
 
     fn get_name(&self) -> &str;
 
     /// Used by union serializers to decide if it's worth trying again while allowing subclasses
-    fn retry_with_lax_check(&self) -> bool {
+    fn retry_with_lax_check(&self, _definitions: &Definitions<CombinedSerializer>) -> bool {
         false
     }
 
     fn get_default(&self, _py: Python) -> PyResult<Option<PyObject>> {
         Ok(None)
     }
 }
```

### Comparing `pydantic_core-2.8.0/src/serializers/type_serializers/any.rs` & `pydantic_core-2.9.0/src/serializers/type_serializers/any.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/serializers/type_serializers/bytes.rs` & `pydantic_core-2.9.0/src/serializers/type_serializers/bytes.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/serializers/type_serializers/dataclass.rs` & `pydantic_core-2.9.0/src/serializers/type_serializers/dataclass.rs`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 use pyo3::prelude::*;
 use pyo3::types::{PyDict, PyList, PyString, PyType};
 use std::borrow::Cow;
 
 use ahash::AHashMap;
 
 use crate::build_tools::{py_schema_error_type, ExtraBehavior};
-use crate::definitions::DefinitionsBuilder;
+use crate::definitions::{Definitions, DefinitionsBuilder};
 use crate::tools::SchemaDict;
 
 use super::{
     infer_json_key, infer_json_key_known, infer_serialize, infer_to_python, py_err_se_err, BuildSerializer,
     CombinedSerializer, ComputedFields, Extra, FieldsMode, GeneralFieldsSerializer, ObType, SerCheck, SerField,
     TypeSerializer,
 };
@@ -175,11 +175,11 @@
         }
     }
 
     fn get_name(&self) -> &str {
         &self.name
     }
 
-    fn retry_with_lax_check(&self) -> bool {
+    fn retry_with_lax_check(&self, _definitions: &Definitions<CombinedSerializer>) -> bool {
         true
     }
 }
```

### Comparing `pydantic_core-2.8.0/src/serializers/type_serializers/datetime_etc.rs` & `pydantic_core-2.9.0/src/serializers/type_serializers/datetime_etc.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/serializers/type_serializers/decimal.rs` & `pydantic_core-2.9.0/src/serializers/type_serializers/decimal.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/serializers/type_serializers/definitions.rs` & `pydantic_core-2.9.0/src/serializers/type_serializers/definitions.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 use std::borrow::Cow;
 
 use pyo3::intern;
 use pyo3::prelude::*;
 use pyo3::types::{PyDict, PyList};
 
+use crate::definitions::Definitions;
 use crate::definitions::DefinitionsBuilder;
 
 use crate::tools::SchemaDict;
 
 use super::{py_err_se_err, BuildSerializer, CombinedSerializer, Extra, TypeSerializer};
 
 #[derive(Debug, Clone)]
@@ -92,8 +93,13 @@
         extra.rec_guard.pop(value_id, self.serializer_id);
         r
     }
 
     fn get_name(&self) -> &str {
         Self::EXPECTED_TYPE
     }
+
+    fn retry_with_lax_check(&self, definitions: &Definitions<CombinedSerializer>) -> bool {
+        let comb_serializer = definitions.get(self.serializer_id).unwrap();
+        comb_serializer.retry_with_lax_check(definitions)
+    }
 }
```

### Comparing `pydantic_core-2.8.0/src/serializers/type_serializers/dict.rs` & `pydantic_core-2.9.0/src/serializers/type_serializers/dict.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/serializers/type_serializers/format.rs` & `pydantic_core-2.9.0/src/serializers/type_serializers/format.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/serializers/type_serializers/function.rs` & `pydantic_core-2.9.0/src/serializers/type_serializers/function.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/serializers/type_serializers/generator.rs` & `pydantic_core-2.9.0/src/serializers/type_serializers/generator.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/serializers/type_serializers/json.rs` & `pydantic_core-2.9.0/src/serializers/type_serializers/json.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/serializers/type_serializers/json_or_python.rs` & `pydantic_core-2.9.0/src/serializers/type_serializers/json_or_python.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/serializers/type_serializers/list.rs` & `pydantic_core-2.9.0/src/serializers/type_serializers/list.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/serializers/type_serializers/literal.rs` & `pydantic_core-2.9.0/src/serializers/type_serializers/literal.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/serializers/type_serializers/mod.rs` & `pydantic_core-2.9.0/src/serializers/type_serializers/mod.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/serializers/type_serializers/model.rs` & `pydantic_core-2.9.0/src/serializers/type_serializers/model.rs`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 use super::{
     infer_json_key, infer_json_key_known, infer_serialize, infer_to_python, py_err_se_err, BuildSerializer,
     CombinedSerializer, ComputedFields, Extra, FieldsMode, GeneralFieldsSerializer, ObType, SerCheck, SerField,
     TypeSerializer,
 };
 use crate::build_tools::py_schema_err;
 use crate::build_tools::{py_schema_error_type, ExtraBehavior};
-use crate::definitions::DefinitionsBuilder;
+use crate::definitions::{Definitions, DefinitionsBuilder};
 use crate::serializers::errors::PydanticSerializationUnexpectedValue;
 use crate::tools::SchemaDict;
 
 const ROOT_FIELD: &str = "root";
 
 pub struct ModelFieldsBuilder;
 
@@ -224,11 +224,11 @@
         }
     }
 
     fn get_name(&self) -> &str {
         &self.name
     }
 
-    fn retry_with_lax_check(&self) -> bool {
+    fn retry_with_lax_check(&self, _definitions: &Definitions<CombinedSerializer>) -> bool {
         true
     }
 }
```

### Comparing `pydantic_core-2.8.0/src/serializers/type_serializers/nullable.rs` & `pydantic_core-2.9.0/src/serializers/type_serializers/nullable.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 use std::borrow::Cow;
 
 use pyo3::intern;
 use pyo3::prelude::*;
 use pyo3::types::PyDict;
 
-use crate::definitions::DefinitionsBuilder;
+use crate::definitions::{Definitions, DefinitionsBuilder};
 use crate::tools::SchemaDict;
 
 use super::{infer_json_key_known, BuildSerializer, CombinedSerializer, Extra, IsType, ObType, TypeSerializer};
 
 #[derive(Debug, Clone)]
 pub struct NullableSerializer {
     serializer: Box<CombinedSerializer>,
@@ -71,11 +71,11 @@
         }
     }
 
     fn get_name(&self) -> &str {
         Self::EXPECTED_TYPE
     }
 
-    fn retry_with_lax_check(&self) -> bool {
-        self.serializer.retry_with_lax_check()
+    fn retry_with_lax_check(&self, definitions: &Definitions<CombinedSerializer>) -> bool {
+        self.serializer.retry_with_lax_check(definitions)
     }
 }
```

### Comparing `pydantic_core-2.8.0/src/serializers/type_serializers/other.rs` & `pydantic_core-2.9.0/src/serializers/type_serializers/other.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/serializers/type_serializers/set_frozenset.rs` & `pydantic_core-2.9.0/src/serializers/type_serializers/set_frozenset.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/serializers/type_serializers/simple.rs` & `pydantic_core-2.9.0/src/serializers/type_serializers/simple.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/serializers/type_serializers/string.rs` & `pydantic_core-2.9.0/src/serializers/type_serializers/string.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/serializers/type_serializers/timedelta.rs` & `pydantic_core-2.9.0/src/serializers/type_serializers/timedelta.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/serializers/type_serializers/tuple.rs` & `pydantic_core-2.9.0/src/serializers/type_serializers/tuple.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/serializers/type_serializers/typed_dict.rs` & `pydantic_core-2.9.0/src/serializers/type_serializers/typed_dict.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/serializers/type_serializers/union.rs` & `pydantic_core-2.9.0/src/serializers/type_serializers/union.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 use pyo3::intern;
 use pyo3::prelude::*;
 use pyo3::types::{PyDict, PyList, PyTuple};
 use std::borrow::Cow;
 
 use crate::build_tools::py_schema_err;
-use crate::definitions::DefinitionsBuilder;
+use crate::definitions::{Definitions, DefinitionsBuilder};
 use crate::tools::SchemaDict;
 use crate::PydanticSerializationUnexpectedValue;
 
 use super::{
     infer_json_key, infer_serialize, infer_to_python, py_err_se_err, BuildSerializer, CombinedSerializer, Extra,
     SerCheck, TypeSerializer,
 };
@@ -83,15 +83,15 @@
                 Ok(v) => return Ok(v),
                 Err(err) => match err.is_instance_of::<PydanticSerializationUnexpectedValue>(value.py()) {
                     true => (),
                     false => return Err(err),
                 },
             }
         }
-        if self.retry_with_lax_check() {
+        if self.retry_with_lax_check(extra.definitions) {
             new_extra.check = SerCheck::Lax;
             for comb_serializer in &self.choices {
                 match comb_serializer.to_python(value, include, exclude, &new_extra) {
                     Ok(v) => return Ok(v),
                     Err(err) => match err.is_instance_of::<PydanticSerializationUnexpectedValue>(value.py()) {
                         true => (),
                         false => return Err(err),
@@ -112,15 +112,15 @@
                 Ok(v) => return Ok(v),
                 Err(err) => match err.is_instance_of::<PydanticSerializationUnexpectedValue>(key.py()) {
                     true => (),
                     false => return Err(err),
                 },
             }
         }
-        if self.retry_with_lax_check() {
+        if self.retry_with_lax_check(extra.definitions) {
             new_extra.check = SerCheck::Lax;
             for comb_serializer in &self.choices {
                 match comb_serializer.json_key(key, &new_extra) {
                     Ok(v) => return Ok(v),
                     Err(err) => match err.is_instance_of::<PydanticSerializationUnexpectedValue>(key.py()) {
                         true => (),
                         false => return Err(err),
@@ -149,15 +149,15 @@
                 Ok(v) => return infer_serialize(v.as_ref(py), serializer, None, None, extra),
                 Err(err) => match err.is_instance_of::<PydanticSerializationUnexpectedValue>(py) {
                     true => (),
                     false => return Err(py_err_se_err(err)),
                 },
             }
         }
-        if self.retry_with_lax_check() {
+        if self.retry_with_lax_check(extra.definitions) {
             new_extra.check = SerCheck::Lax;
             for comb_serializer in &self.choices {
                 match comb_serializer.to_python(value, include, exclude, &new_extra) {
                     Ok(v) => return infer_serialize(v.as_ref(py), serializer, None, None, extra),
                     Err(err) => match err.is_instance_of::<PydanticSerializationUnexpectedValue>(py) {
                         true => (),
                         false => return Err(py_err_se_err(err)),
@@ -170,16 +170,18 @@
         infer_serialize(value, serializer, include, exclude, extra)
     }
 
     fn get_name(&self) -> &str {
         &self.name
     }
 
-    fn retry_with_lax_check(&self) -> bool {
-        self.choices.iter().any(TypeSerializer::retry_with_lax_check)
+    fn retry_with_lax_check(&self, definitions: &Definitions<CombinedSerializer>) -> bool {
+        self.choices
+            .iter()
+            .any(|choice| choice.retry_with_lax_check(definitions))
     }
 }
 
 pub struct TaggedUnionBuilder;
 
 impl BuildSerializer for TaggedUnionBuilder {
     const EXPECTED_TYPE: &'static str = "tagged-union";
```

### Comparing `pydantic_core-2.8.0/src/serializers/type_serializers/url.rs` & `pydantic_core-2.9.0/src/serializers/type_serializers/url.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/serializers/type_serializers/uuid.rs` & `pydantic_core-2.9.0/src/serializers/type_serializers/uuid.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/serializers/type_serializers/with_default.rs` & `pydantic_core-2.9.0/src/serializers/type_serializers/with_default.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 use std::borrow::Cow;
 
 use pyo3::intern;
 use pyo3::prelude::*;
 use pyo3::types::PyDict;
 
-use crate::definitions::DefinitionsBuilder;
+use crate::definitions::{Definitions, DefinitionsBuilder};
 use crate::tools::SchemaDict;
 use crate::validators::DefaultType;
 
 use super::{BuildSerializer, CombinedSerializer, Extra, TypeSerializer};
 
 #[derive(Debug, Clone)]
 pub struct WithDefaultSerializer {
@@ -63,15 +63,15 @@
             .serde_serialize(value, serializer, include, exclude, extra)
     }
 
     fn get_name(&self) -> &str {
         Self::EXPECTED_TYPE
     }
 
-    fn retry_with_lax_check(&self) -> bool {
-        self.serializer.retry_with_lax_check()
+    fn retry_with_lax_check(&self, definitions: &Definitions<CombinedSerializer>) -> bool {
+        self.serializer.retry_with_lax_check(definitions)
     }
 
     fn get_default(&self, py: Python) -> PyResult<Option<PyObject>> {
         self.default.default_value(py)
     }
 }
```

### Comparing `pydantic_core-2.8.0/src/tools.rs` & `pydantic_core-2.9.0/src/tools.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/url.rs` & `pydantic_core-2.9.0/src/url.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/validators/any.rs` & `pydantic_core-2.9.0/src/validators/any.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/validators/arguments.rs` & `pydantic_core-2.9.0/src/validators/arguments.rs`

 * *Files 1% similar despite different names*

```diff
@@ -319,14 +319,15 @@
                     }
                 }
             }};
         }
         match args {
             GenericArguments::Py(a) => process!(a, py_get_dict_item, py_get, py_slice),
             GenericArguments::Json(a) => process!(a, json_get, json_get, json_slice),
+            GenericArguments::StringMapping(_) => unimplemented!(),
         }
         if !errors.is_empty() {
             Err(ValError::LineErrors(errors))
         } else {
             Ok((PyTuple::new(py, output_args), output_kwargs).to_object(py))
         }
     }
```

### Comparing `pydantic_core-2.8.0/src/validators/bool.rs` & `pydantic_core-2.9.0/src/validators/bool.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/validators/bytes.rs` & `pydantic_core-2.9.0/src/validators/bytes.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/validators/call.rs` & `pydantic_core-2.9.0/src/validators/call.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/validators/callable.rs` & `pydantic_core-2.9.0/src/validators/callable.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/validators/chain.rs` & `pydantic_core-2.9.0/src/validators/chain.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/validators/custom_error.rs` & `pydantic_core-2.9.0/src/validators/custom_error.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/validators/dataclass.rs` & `pydantic_core-2.9.0/src/validators/dataclass.rs`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 use pyo3::types::{PyDict, PyList, PyString, PyTuple, PyType};
 
 use ahash::AHashSet;
 
 use crate::build_tools::py_schema_err;
 use crate::build_tools::{is_strict, schema_or_config_same, ExtraBehavior};
 use crate::errors::{ErrorType, ErrorTypeDefaults, ValError, ValLineError, ValResult};
-use crate::input::{GenericArguments, Input};
+use crate::input::{BorrowInput, GenericArguments, Input};
 use crate::lookup_key::LookupKey;
 use crate::tools::SchemaDict;
 use crate::validators::function::convert_err;
 
 use super::arguments::{json_get, json_slice, py_get, py_slice};
 use super::model::{create_class, force_setattr, Revalidate};
 use super::{
@@ -184,23 +184,29 @@
                             let mut kw_value = None;
                             if let Some(kwargs) = $args.kwargs {
                                 if let Some((lookup_path, value)) = field.lookup_key.$get_method(kwargs)? {
                                     used_keys.insert(lookup_path.first_key());
                                     kw_value = Some((lookup_path, value));
                                 }
                             }
+                            let kw_value = kw_value
+                                .as_ref()
+                                .map(|(path, value)| (path, value.borrow_input()));
 
                             match (pos_value, kw_value) {
                                 // found both positional and keyword arguments, error
                                 (Some(_), Some((_, kw_value))) => {
-                                    errors.push(ValLineError::new_with_loc(
-                                        ErrorTypeDefaults::MultipleArgumentValues,
-                                        kw_value,
-                                        field.name.clone(),
-                                    ));
+                                    errors.push(
+                                        ValLineError::new_with_loc(
+                                            ErrorTypeDefaults::MultipleArgumentValues,
+                                            kw_value,
+                                            field.name.clone(),
+                                        )
+                                        .into_owned(py),
+                                    );
                                 }
                                 // found a positional argument, validate it
                                 (Some(pos_value), None) => match field.validator.validate(py, pos_value, state) {
                                     Ok(value) => set_item!(field, value),
                                     Err(ValError::LineErrors(line_errors)) => {
                                         errors.extend(
                                             line_errors
@@ -212,18 +218,20 @@
                                 },
                                 // found a keyword argument, validate it
                                 (None, Some((lookup_path, kw_value))) => {
                                     match field.validator.validate(py, kw_value, state) {
                                         Ok(value) => set_item!(field, value),
                                         Err(ValError::LineErrors(line_errors)) => {
                                             errors.extend(line_errors.into_iter().map(|err| {
-                                                lookup_path.apply_error_loc(err, self.loc_by_alias, &field.name)
+                                                lookup_path
+                                                    .apply_error_loc(err, self.loc_by_alias, &field.name)
+                                                    .into_owned(py)
                                             }));
                                         }
-                                        Err(err) => return Err(err),
+                                        Err(err) => return Err(err.into_owned(py)),
                                     }
                                 }
                                 // found neither, check if there is a default value, otherwise error
                                 (None, None) => {
                                     if let Some(value) =
                                         field
                                             .validator
@@ -263,19 +271,22 @@
                                 for (raw_key, value) in kwargs.iter() {
                                     match raw_key.strict_str() {
                                         Ok(either_str) => {
                                             if !used_keys.contains(either_str.as_cow()?.as_ref()) {
                                                 // Unknown / extra field
                                                 match self.extra_behavior {
                                                     ExtraBehavior::Forbid => {
-                                                        errors.push(ValLineError::new_with_loc(
-                                                            ErrorTypeDefaults::UnexpectedKeywordArgument,
-                                                            value,
-                                                            raw_key.as_loc_item(),
-                                                        ));
+                                                        errors.push(
+                                                            ValLineError::new_with_loc(
+                                                                ErrorTypeDefaults::UnexpectedKeywordArgument,
+                                                                value,
+                                                                raw_key.as_loc_item(),
+                                                            )
+                                                            .into_owned(py),
+                                                        );
                                                     }
                                                     ExtraBehavior::Ignore => {}
                                                     ExtraBehavior::Allow => {
                                                         if let Some(ref validator) = self.extras_validator {
                                                             match validator.validate(py, value, state) {
                                                                 Ok(value) => output_dict
                                                                     .set_item(either_str.as_py_string(py), value)?,
@@ -306,17 +317,32 @@
                                         Err(err) => return Err(err),
                                     }
                                 }
                             }
                         }
                     }};
                 }
+
                 match args {
                     GenericArguments::Py(a) => process!(a, py_get_dict_item, py_get, py_slice),
                     GenericArguments::Json(a) => process!(a, json_get, json_get, json_slice),
+                    GenericArguments::StringMapping(a) => {
+                        // StringMapping cannot pass positional args, so wrap the PyDict
+                        // in a type with guaranteed empty args array for sake of the process
+                        // macro
+                        struct StringMappingArgs<'a> {
+                            args: Option<&'a PyTuple>,
+                            kwargs: Option<&'a PyDict>,
+                        }
+                        let a = StringMappingArgs {
+                            args: None,
+                            kwargs: Some(a),
+                        };
+                        process!(a, py_get_string_mapping_item, py_get, py_slice);
+                    }
                 }
                 Ok(())
             },
         )?;
         if errors.is_empty() {
             if let Some(init_only_args) = init_only_args {
                 Ok((output_dict, PyTuple::new(py, init_only_args)).to_object(py))
```

### Comparing `pydantic_core-2.8.0/src/validators/date.rs` & `pydantic_core-2.9.0/src/validators/date.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/validators/datetime.rs` & `pydantic_core-2.9.0/src/validators/datetime.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/validators/decimal.rs` & `pydantic_core-2.9.0/src/validators/decimal.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/validators/definitions.rs` & `pydantic_core-2.9.0/src/validators/definitions.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/validators/dict.rs` & `pydantic_core-2.9.0/src/validators/dict.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 use pyo3::intern;
 use pyo3::prelude::*;
 use pyo3::types::PyDict;
 
 use crate::build_tools::is_strict;
 use crate::errors::{ValError, ValLineError, ValResult};
-use crate::input::{DictGenericIterator, GenericMapping, Input, JsonObjectGenericIterator, MappingGenericIterator};
+use crate::input::BorrowInput;
+use crate::input::{
+    DictGenericIterator, GenericMapping, Input, JsonObjectGenericIterator, MappingGenericIterator,
+    StringMappingGenericIterator,
+};
 
 use crate::tools::SchemaDict;
 
 use super::any::AnyValidator;
 use super::list::length_check;
 use super::{build_validator, BuildValidator, CombinedValidator, DefinitionsBuilder, ValidationState, Validator};
 
@@ -74,14 +78,17 @@
         match dict {
             GenericMapping::PyDict(py_dict) => {
                 self.validate_generic_mapping(py, input, DictGenericIterator::new(py_dict)?, state)
             }
             GenericMapping::PyMapping(mapping) => {
                 self.validate_generic_mapping(py, input, MappingGenericIterator::new(mapping)?, state)
             }
+            GenericMapping::StringMapping(dict) => {
+                self.validate_generic_mapping(py, input, StringMappingGenericIterator::new(dict)?, state)
+            }
             GenericMapping::PyGetAttr(_, _) => unreachable!(),
             GenericMapping::JsonObject(json_object) => {
                 self.validate_generic_mapping(py, input, JsonObjectGenericIterator::new(json_object)?, state)
             }
         }
     }
 
@@ -109,51 +116,52 @@
 }
 
 impl DictValidator {
     fn validate_generic_mapping<'s, 'data>(
         &'s self,
         py: Python<'data>,
         input: &'data impl Input<'data>,
-        mapping_iter: impl Iterator<
-            Item = ValResult<'data, (&'data (impl Input<'data> + 'data), &'data (impl Input<'data> + 'data))>,
-        >,
+        mapping_iter: impl Iterator<Item = ValResult<'data, (impl BorrowInput + 'data, impl BorrowInput + 'data)>>,
         state: &mut ValidationState,
     ) -> ValResult<'data, PyObject> {
         let output = PyDict::new(py);
         let mut errors: Vec<ValLineError> = Vec::new();
 
         let key_validator = self.key_validator.as_ref();
         let value_validator = self.value_validator.as_ref();
         for item_result in mapping_iter {
             let (key, value) = item_result?;
+            let key = key.borrow_input();
+            let value = value.borrow_input();
             let output_key = match key_validator.validate(py, key, state) {
                 Ok(value) => Some(value),
                 Err(ValError::LineErrors(line_errors)) => {
                     for err in line_errors {
                         // these are added in reverse order so [key] is shunted along by the second call
                         errors.push(
                             err.with_outer_location("[key]".into())
-                                .with_outer_location(key.as_loc_item()),
+                                .with_outer_location(key.as_loc_item())
+                                .into_owned(py),
                         );
                     }
                     None
                 }
                 Err(ValError::Omit) => continue,
-                Err(err) => return Err(err),
+                Err(err) => return Err(err.into_owned(py)),
             };
             let output_value = match value_validator.validate(py, value, state) {
                 Ok(value) => Some(value),
                 Err(ValError::LineErrors(line_errors)) => {
                     for err in line_errors {
-                        errors.push(err.with_outer_location(key.as_loc_item()));
+                        errors.push(err.with_outer_location(key.as_loc_item()).into_owned(py));
                     }
                     None
                 }
                 Err(ValError::Omit) => continue,
-                Err(err) => return Err(err),
+                Err(err) => return Err(err.into_owned(py)),
             };
             if let (Some(key), Some(value)) = (output_key, output_value) {
                 output.set_item(key, value)?;
             }
         }
 
         if errors.is_empty() {
```

### Comparing `pydantic_core-2.8.0/src/validators/float.rs` & `pydantic_core-2.9.0/src/validators/float.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/validators/frozenset.rs` & `pydantic_core-2.9.0/src/validators/frozenset.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/validators/function.rs` & `pydantic_core-2.9.0/src/validators/function.rs`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
             fn validate<'data>(
                 &self,
                 py: Python<'data>,
                 input: &'data impl Input<'data>,
                 state: &mut ValidationState<'_>,
             ) -> ValResult<'data, PyObject> {
                 let validate = |v, s: &mut ValidationState<'_>| self.validator.validate(py, v, s);
-                self._validate(validate, py, input.to_object(py).into_ref(py), state)
+                self._validate(validate, py, input, state)
             }
             fn validate_assignment<'data>(
                 &self,
                 py: Python<'data>,
                 obj: &'data PyAny,
                 field_name: &'data str,
                 field_value: &'data PyAny,
@@ -154,15 +154,15 @@
 impl_build!(FunctionBeforeValidator, "function-before");
 
 impl FunctionBeforeValidator {
     fn _validate<'s, 'data>(
         &'s self,
         call: impl FnOnce(&'data PyAny, &mut ValidationState<'_>) -> ValResult<'data, PyObject>,
         py: Python<'data>,
-        input: &'data PyAny,
+        input: &'data impl Input<'data>,
         state: &'s mut ValidationState<'_>,
     ) -> ValResult<'data, PyObject> {
         let r = if self.info_arg {
             let info = ValidationInfo::new(py, state.extra(), &self.config, self.field_name.clone());
             self.func.call1(py, (input.to_object(py), info))
         } else {
             self.func.call1(py, (input.to_object(py),))
@@ -183,19 +183,19 @@
     field_name: Option<Py<PyString>>,
     info_arg: bool,
 }
 
 impl_build!(FunctionAfterValidator, "function-after");
 
 impl FunctionAfterValidator {
-    fn _validate<'s, 'data>(
+    fn _validate<'s, 'data, I: Input<'data>>(
         &'s self,
-        call: impl FnOnce(&'data PyAny, &mut ValidationState<'_>) -> ValResult<'data, PyObject>,
+        call: impl FnOnce(&'data I, &mut ValidationState<'_>) -> ValResult<'data, PyObject>,
         py: Python<'data>,
-        input: &'data PyAny,
+        input: &'data I,
         state: &mut ValidationState<'_>,
     ) -> ValResult<'data, PyObject> {
         let v = call(input, state)?;
         let r = if self.info_arg {
             let info = ValidationInfo::new(py, state.extra(), &self.config, self.field_name.clone());
             self.func.call1(py, (v.to_object(py), info))
         } else {
@@ -322,15 +322,15 @@
 }
 
 impl FunctionWrapValidator {
     fn _validate<'s, 'data>(
         &'s self,
         handler: &'s PyAny,
         py: Python<'data>,
-        input: &'data PyAny,
+        input: &'data impl Input<'data>,
         state: &mut ValidationState,
     ) -> ValResult<'data, PyObject> {
         let r = if self.info_arg {
             let info = ValidationInfo::new(py, state.extra(), &self.config, self.field_name.clone());
             self.func.call1(py, (input.to_object(py), handler, info))
         } else {
             self.func.call1(py, (input.to_object(py), handler))
@@ -540,15 +540,15 @@
 impl ValidationInfo {
     fn new(py: Python, extra: &Extra, config: &PyObject, field_name: Option<Py<PyString>>) -> Self {
         Self {
             config: config.clone_ref(py),
             context: extra.context.map(Into::into),
             field_name,
             data: extra.data.map(Into::into),
-            mode: extra.mode,
+            mode: extra.input_type,
         }
     }
 }
 
 #[pymethods]
 impl ValidationInfo {
     #[getter]
```

### Comparing `pydantic_core-2.8.0/src/validators/generator.rs` & `pydantic_core-2.9.0/src/validators/generator.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use std::fmt;
 
 use pyo3::prelude::*;
 use pyo3::types::PyDict;
 
-use crate::errors::{ErrorMode, ErrorType, LocItem, ValError, ValResult};
+use crate::errors::{ErrorType, LocItem, ValError, ValResult};
 use crate::input::{GenericIterator, Input};
 use crate::recursion_guard::RecursionGuard;
 use crate::tools::SchemaDict;
 use crate::ValidationError;
 
 use super::list::get_items_schema;
 use super::{BuildValidator, CombinedValidator, DefinitionsBuilder, Extra, InputType, ValidationState, Validator};
@@ -149,15 +149,15 @@
                                             context: None,
                                         },
                                         $iter.input_as_error_value(py),
                                     );
                                     return Err(ValidationError::from_val_error(
                                         py,
                                         "ValidatorIterator".to_object(py),
-                                        ErrorMode::Python,
+                                        InputType::Python,
                                         val_error,
                                         None,
                                         hide_input_in_errors,
                                         validation_error_cause,
                                     ));
                                 }
                             }
@@ -176,15 +176,15 @@
                                         context: None,
                                     },
                                     $iter.input_as_error_value(py),
                                 );
                                 return Err(ValidationError::from_val_error(
                                     py,
                                     "ValidatorIterator".to_object(py),
-                                    ErrorMode::Python,
+                                    InputType::Python,
                                     val_error,
                                     None,
                                     hide_input_in_errors,
                                     validation_error_cause,
                                 ));
                             }
                         }
@@ -258,45 +258,45 @@
             definitions: state.definitions.to_vec(),
             data: extra.data.map(|d| d.into_py(py)),
             strict: extra.strict,
             from_attributes: extra.from_attributes,
             context: extra.context.map(|d| d.into_py(py)),
             self_instance: extra.self_instance.map(|d| d.into_py(py)),
             recursion_guard: state.recursion_guard.clone(),
-            validation_mode: extra.mode,
+            validation_mode: extra.input_type,
             hide_input_in_errors,
             validation_error_cause,
         }
     }
 
     pub fn validate_assignment<'data>(
         &mut self,
         py: Python<'data>,
         model: &'data PyAny,
         field_name: &'data str,
         field_value: &'data PyAny,
         outer_location: Option<LocItem>,
     ) -> PyResult<PyObject> {
         let extra = Extra {
-            mode: self.validation_mode,
+            input_type: self.validation_mode,
             data: self.data.as_ref().map(|data| data.as_ref(py)),
             strict: self.strict,
             ultra_strict: false,
             from_attributes: self.from_attributes,
             context: self.context.as_ref().map(|data| data.as_ref(py)),
             self_instance: self.self_instance.as_ref().map(|data| data.as_ref(py)),
         };
         let mut state = ValidationState::new(extra, &self.definitions, &mut self.recursion_guard);
         self.validator
             .validate_assignment(py, model, field_name, field_value, &mut state)
             .map_err(|e| {
                 ValidationError::from_val_error(
                     py,
                     self.name.to_object(py),
-                    ErrorMode::Python,
+                    InputType::Python,
                     e,
                     outer_location,
                     self.hide_input_in_errors,
                     self.validation_error_cause,
                 )
             })
     }
@@ -304,28 +304,28 @@
     pub fn validate<'data>(
         &mut self,
         py: Python<'data>,
         input: &'data impl Input<'data>,
         outer_location: Option<LocItem>,
     ) -> PyResult<PyObject> {
         let extra = Extra {
-            mode: self.validation_mode,
+            input_type: self.validation_mode,
             data: self.data.as_ref().map(|data| data.as_ref(py)),
             strict: self.strict,
             ultra_strict: false,
             from_attributes: self.from_attributes,
             context: self.context.as_ref().map(|data| data.as_ref(py)),
             self_instance: self.self_instance.as_ref().map(|data| data.as_ref(py)),
         };
         let mut state = ValidationState::new(extra, &self.definitions, &mut self.recursion_guard);
         self.validator.validate(py, input, &mut state).map_err(|e| {
             ValidationError::from_val_error(
                 py,
                 self.name.to_object(py),
-                ErrorMode::Python,
+                InputType::Python,
                 e,
                 outer_location,
                 self.hide_input_in_errors,
                 self.validation_error_cause,
             )
         })
     }
```

### Comparing `pydantic_core-2.8.0/src/validators/int.rs` & `pydantic_core-2.9.0/src/validators/int.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/validators/is_instance.rs` & `pydantic_core-2.9.0/src/validators/is_instance.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/validators/is_subclass.rs` & `pydantic_core-2.9.0/src/validators/is_subclass.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/validators/json.rs` & `pydantic_core-2.9.0/src/validators/json.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/validators/json_or_python.rs` & `pydantic_core-2.9.0/src/validators/json_or_python.rs`

 * *Files 8% similar despite different names*

```diff
@@ -53,17 +53,17 @@
 impl Validator for JsonOrPython {
     fn validate<'data>(
         &self,
         py: Python<'data>,
         input: &'data impl Input<'data>,
         state: &mut ValidationState,
     ) -> ValResult<'data, PyObject> {
-        match state.extra().mode {
+        match state.extra().input_type {
             InputType::Python => self.python.validate(py, input, state),
-            InputType::Json => self.json.validate(py, input, state),
+            _ => self.json.validate(py, input, state),
         }
     }
 
     fn different_strict_behavior(
         &self,
         definitions: Option<&DefinitionsBuilder<CombinedValidator>>,
         ultra_strict: bool,
```

### Comparing `pydantic_core-2.8.0/src/validators/lax_or_strict.rs` & `pydantic_core-2.9.0/src/validators/lax_or_strict.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/validators/list.rs` & `pydantic_core-2.9.0/src/validators/list.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/validators/literal.rs` & `pydantic_core-2.9.0/src/validators/literal.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/validators/mod.rs` & `pydantic_core-2.9.0/src/validators/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 use pyo3::once_cell::GILOnceCell;
 use pyo3::prelude::*;
 use pyo3::types::{PyAny, PyDict, PyTuple, PyType};
 use pyo3::{intern, PyTraverseError, PyVisit};
 
 use crate::build_tools::{py_schema_err, py_schema_error_type, SchemaError};
 use crate::definitions::DefinitionsBuilder;
-use crate::errors::{ErrorMode, LocItem, ValError, ValResult, ValidationError};
-use crate::input::{Input, InputType};
+use crate::errors::{LocItem, ValError, ValResult, ValidationError};
+use crate::input::{Input, InputType, StringMapping};
 use crate::py_gc::PyGcTraverse;
 use crate::recursion_guard::RecursionGuard;
 use crate::tools::SchemaDict;
 
 mod any;
 mod arguments;
 mod bool;
@@ -166,15 +166,15 @@
             InputType::Python,
             strict,
             from_attributes,
             context,
             self_instance,
             &mut RecursionGuard::default(),
         )
-        .map_err(|e| self.prepare_validation_err(py, e, ErrorMode::Python))
+        .map_err(|e| self.prepare_validation_err(py, e, InputType::Python))
     }
 
     #[pyo3(signature = (input, *, strict=None, from_attributes=None, context=None, self_instance=None))]
     pub fn isinstance_python(
         &self,
         py: Python,
         input: &PyAny,
@@ -219,16 +219,34 @@
                     InputType::Json,
                     strict,
                     None,
                     context,
                     self_instance,
                     recursion_guard,
                 )
-                .map_err(|e| self.prepare_validation_err(py, e, ErrorMode::Json)),
-            Err(err) => Err(self.prepare_validation_err(py, err, ErrorMode::Json)),
+                .map_err(|e| self.prepare_validation_err(py, e, InputType::Json)),
+            Err(err) => Err(self.prepare_validation_err(py, err, InputType::Json)),
+        }
+    }
+
+    #[pyo3(signature = (input, *, strict=None, context=None))]
+    pub fn validate_strings(
+        &self,
+        py: Python,
+        input: &PyAny,
+        strict: Option<bool>,
+        context: Option<&PyAny>,
+    ) -> PyResult<PyObject> {
+        let t = InputType::String;
+        let string_mapping = StringMapping::new_value(input).map_err(|e| self.prepare_validation_err(py, e, t))?;
+
+        let recursion_guard = &mut RecursionGuard::default();
+        match self._validate(py, &string_mapping, t, strict, None, context, None, recursion_guard) {
+            Ok(r) => Ok(r),
+            Err(e) => Err(self.prepare_validation_err(py, e, t)),
         }
     }
 
     #[allow(clippy::too_many_arguments)]
     #[pyo3(signature = (obj, field_name, field_value, *, strict=None, from_attributes=None, context=None))]
     pub fn validate_assignment(
         &self,
@@ -237,34 +255,34 @@
         field_name: &str,
         field_value: &PyAny,
         strict: Option<bool>,
         from_attributes: Option<bool>,
         context: Option<&PyAny>,
     ) -> PyResult<PyObject> {
         let extra = Extra {
-            mode: InputType::Python,
+            input_type: InputType::Python,
             data: None,
             strict,
             from_attributes,
             ultra_strict: false,
             context,
             self_instance: None,
         };
 
         let guard = &mut RecursionGuard::default();
         let mut state = ValidationState::new(extra, &self.definitions, guard);
         self.validator
             .validate_assignment(py, obj, field_name, field_value, &mut state)
-            .map_err(|e| self.prepare_validation_err(py, e, ErrorMode::Python))
+            .map_err(|e| self.prepare_validation_err(py, e, InputType::Python))
     }
 
     #[pyo3(signature = (*, strict=None, context=None))]
     pub fn get_default_value(&self, py: Python, strict: Option<bool>, context: Option<&PyAny>) -> PyResult<PyObject> {
         let extra = Extra {
-            mode: InputType::Python,
+            input_type: InputType::Python,
             data: None,
             strict,
             from_attributes: None,
             ultra_strict: false,
             context,
             self_instance: None,
         };
@@ -272,15 +290,15 @@
         let mut state = ValidationState::new(extra, &self.definitions, recursion_guard);
         let r = self.validator.default_value(py, None::<i64>, &mut state);
         match r {
             Ok(maybe_default) => match maybe_default {
                 Some(v) => Ok(PySome::new(v).into_py(py)),
                 None => Ok(py.None().into_py(py)),
             },
-            Err(e) => Err(self.prepare_validation_err(py, e, ErrorMode::Python)),
+            Err(e) => Err(self.prepare_validation_err(py, e, InputType::Python)),
         }
     }
 
     pub fn __repr__(&self, py: Python) -> String {
         format!(
             "SchemaValidator(title={:?}, validator={:#?}, definitions={:#?})",
             self.title.extract::<&str>(py).unwrap(),
@@ -301,37 +319,37 @@
 
 impl SchemaValidator {
     #[allow(clippy::too_many_arguments)]
     fn _validate<'s, 'data>(
         &'data self,
         py: Python<'data>,
         input: &'data impl Input<'data>,
-        mode: InputType,
+        input_type: InputType,
         strict: Option<bool>,
         from_attributes: Option<bool>,
         context: Option<&'data PyAny>,
         self_instance: Option<&PyAny>,
         recursion_guard: &'data mut RecursionGuard,
     ) -> ValResult<'data, PyObject>
     where
         's: 'data,
     {
         let mut state = ValidationState::new(
-            Extra::new(strict, from_attributes, context, self_instance, mode),
+            Extra::new(strict, from_attributes, context, self_instance, input_type),
             &self.definitions,
             recursion_guard,
         );
         self.validator.validate(py, input, &mut state)
     }
 
-    fn prepare_validation_err(&self, py: Python, error: ValError, error_mode: ErrorMode) -> PyErr {
+    fn prepare_validation_err(&self, py: Python, error: ValError, input_type: InputType) -> PyErr {
         ValidationError::from_val_error(
             py,
             self.title.clone_ref(py),
-            error_mode,
+            input_type,
             error,
             None,
             self.hide_input_in_errors,
             self.validation_error_cause,
         )
     }
 }
@@ -529,15 +547,15 @@
 }
 
 /// More (mostly immutable) data to pass between validators, should probably be class `Context`,
 /// but that would confuse it with context as per pydantic/pydantic#1549
 #[derive(Debug)]
 pub struct Extra<'a> {
     /// Validation mode
-    pub mode: InputType,
+    pub input_type: InputType,
     /// This is used as the `data` kwargs to validator functions
     pub data: Option<&'a PyDict>,
     /// whether we're in strict or lax mode
     pub strict: Option<bool>,
     /// whether we're in ultra-strict mode, only used occasionally in unions
     pub ultra_strict: bool,
     /// Validation time setting of `from_attributes`
@@ -550,32 +568,32 @@
 
 impl<'a> Extra<'a> {
     pub fn new(
         strict: Option<bool>,
         from_attributes: Option<bool>,
         context: Option<&'a PyAny>,
         self_instance: Option<&'a PyAny>,
-        mode: InputType,
+        input_type: InputType,
     ) -> Self {
         Extra {
-            mode,
+            input_type,
             data: None,
             strict,
             ultra_strict: false,
             from_attributes,
             context,
             self_instance,
         }
     }
 }
 
 impl<'a> Extra<'a> {
     pub fn as_strict(&self, ultra_strict: bool) -> Self {
         Self {
-            mode: self.mode,
+            input_type: self.input_type,
             data: self.data,
             strict: Some(true),
             ultra_strict,
             from_attributes: self.from_attributes,
             context: self.context,
             self_instance: self.self_instance,
         }
```

### Comparing `pydantic_core-2.8.0/src/validators/model.rs` & `pydantic_core-2.9.0/src/validators/model.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/validators/model_fields.rs` & `pydantic_core-2.9.0/src/validators/model_fields.rs`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 use pyo3::prelude::*;
 use pyo3::types::{PyDict, PySet, PyString, PyType};
 
 use ahash::AHashSet;
 
 use crate::build_tools::py_schema_err;
 use crate::build_tools::{is_strict, schema_or_config_same, ExtraBehavior};
-use crate::errors::{py_err_string, ErrorType, ErrorTypeDefaults, ValError, ValLineError, ValResult};
+use crate::errors::{ErrorType, ErrorTypeDefaults, ValError, ValLineError, ValResult};
 use crate::input::{
-    AttributesGenericIterator, DictGenericIterator, GenericMapping, Input, JsonObjectGenericIterator,
-    MappingGenericIterator,
+    AttributesGenericIterator, BorrowInput, DictGenericIterator, GenericMapping, Input, JsonObjectGenericIterator,
+    MappingGenericIterator, StringMappingGenericIterator,
 };
 use crate::lookup_key::LookupKey;
 use crate::tools::SchemaDict;
 
 use super::ValidationState;
 use super::{build_validator, BuildValidator, CombinedValidator, DefinitionsBuilder, Extra, Validator};
 
@@ -176,47 +176,43 @@
                 match state.with_new_extra(Extra {
                     data: Some(model_dict),
                     ..*state.extra()
                 }, |state| {
                     for field in &self.fields {
                         let op_key_value = match field.lookup_key.$get_method($dict $(, $kwargs )? ) {
                             Ok(v) => v,
-                            Err(err) => {
-                                errors.push(ValLineError::new_with_loc(
-                                    ErrorType::GetAttributeError {
-                                        error: py_err_string(py, err),
-                                        context: None,
-                                    },
-                                    input,
-                                    field.name.clone(),
-                                ));
+                            Err(ValError::LineErrors(line_errors)) => {
+                                for err in line_errors {
+                                    errors.push(err.with_outer_location(field.name.as_loc_item()));
+                                }
                                 continue;
                             }
+                            Err(err) => return ControlFlow::Break(err),
                         };
                         if let Some((lookup_path, value)) = op_key_value {
                             if let Some(ref mut used_keys) = used_keys {
                                 // key is "used" whether or not validation passes, since we want to skip this key in
                                 // extra logic either way
                                 used_keys.insert(lookup_path.first_key());
                             }
-                            match field
-                                .validator
-                                .validate(py, value, state)
-                            {
+                            match field.validator.validate(py, value.borrow_input(), state) {
                                 Ok(value) => {
                                     control_flow!(model_dict.set_item(&field.name_py, value))?;
                                     fields_set_vec.push(field.name_py.clone_ref(py));
                                 }
                                 Err(ValError::Omit) => continue,
                                 Err(ValError::LineErrors(line_errors)) => {
                                     for err in line_errors {
-                                        errors.push(lookup_path.apply_error_loc(err, self.loc_by_alias, &field.name));
+                                        errors.push(
+                                            lookup_path.apply_error_loc(err, self.loc_by_alias, &field.name)
+                                            .into_owned(py)
+                                        );
                                     }
                                 }
-                                Err(err) => return ControlFlow::Break(err),
+                                Err(err) => return ControlFlow::Break(err.into_owned(py)),
                             }
                             continue;
                         } else if let Some(value) = control_flow!(field.validator.default_value(py, Some(field.name.as_str()), state))? {
                             control_flow!(model_dict.set_item(&field.name_py, value))?;
                         } else {
                             errors.push(field.lookup_key.error(
                                 ErrorTypeDefaults::Missing,
@@ -238,49 +234,55 @@
                         let (raw_key, value) = item_result?;
                         let either_str = match raw_key.strict_str() {
                             Ok(k) => k,
                             Err(ValError::LineErrors(line_errors)) => {
                                 for err in line_errors {
                                     errors.push(
                                         err.with_outer_location(raw_key.as_loc_item())
-                                            .with_type(ErrorTypeDefaults::InvalidKey),
+                                            .with_type(ErrorTypeDefaults::InvalidKey)
+                                            .into_owned(py)
                                     );
                                 }
                                 continue;
                             }
-                            Err(err) => return Err(err),
+                            Err(err) => return Err(err.into_owned(py)),
                         };
-                        if used_keys.contains(either_str.as_cow()?.as_ref()) {
+                        let cow = either_str.as_cow().map_err(|err| err.into_owned(py))?;
+                        if used_keys.contains(cow.as_ref()) {
                             continue;
                         }
 
+                        let value = value.borrow_input();
                         // Unknown / extra field
                         match self.extra_behavior {
                             ExtraBehavior::Forbid => {
-                                errors.push(ValLineError::new_with_loc(
-                                    ErrorTypeDefaults::ExtraForbidden,
-                                    value,
-                                    raw_key.as_loc_item(),
-                                ));
+                                errors.push(
+                                    ValLineError::new_with_loc(
+                                        ErrorTypeDefaults::ExtraForbidden,
+                                        value,
+                                        raw_key.as_loc_item(),
+                                    )
+                                    .into_owned(py)
+                                );
                             }
                             ExtraBehavior::Ignore => {}
                             ExtraBehavior::Allow => {
                             let py_key = either_str.as_py_string(py);
                                 if let Some(ref validator) = self.extras_validator {
                                     match validator.validate(py, value, state) {
                                         Ok(value) => {
                                             model_extra_dict.set_item(py_key, value)?;
                                             fields_set_vec.push(py_key.into_py(py));
                                         }
                                         Err(ValError::LineErrors(line_errors)) => {
                                             for err in line_errors {
-                                                errors.push(err.with_outer_location(raw_key.as_loc_item()));
+                                                errors.push(err.with_outer_location(raw_key.as_loc_item()).into_owned(py));
                                             }
                                         }
-                                        Err(err) => return Err(err),
+                                        Err(err) => return Err(err.into_owned(py)),
                                     }
                                 } else {
                                     model_extra_dict.set_item(py_key, value.to_object(py))?;
                                     fields_set_vec.push(py_key.into_py(py));
                                 };
                             }
                         }
@@ -289,16 +291,17 @@
                         model_extra_dict_op = Some(model_extra_dict);
                     }
                 }
             }};
         }
         match dict {
             GenericMapping::PyDict(d) => process!(d, py_get_dict_item, DictGenericIterator),
-            GenericMapping::PyGetAttr(d, kwargs) => process!(d, py_get_attr, AttributesGenericIterator, kwargs),
             GenericMapping::PyMapping(d) => process!(d, py_get_mapping_item, MappingGenericIterator),
+            GenericMapping::StringMapping(d) => process!(d, py_get_string_mapping_item, StringMappingGenericIterator),
+            GenericMapping::PyGetAttr(d, kwargs) => process!(d, py_get_attr, AttributesGenericIterator, kwargs),
             GenericMapping::JsonObject(d) => process!(d, json_get, JsonObjectGenericIterator),
         }
 
         if !errors.is_empty() {
             Err(ValError::LineErrors(errors))
         } else {
             let fields_set = PySet::new(py, &fields_set_vec)?;
```

### Comparing `pydantic_core-2.8.0/src/validators/none.rs` & `pydantic_core-2.9.0/src/validators/none.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/validators/nullable.rs` & `pydantic_core-2.9.0/src/validators/nullable.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/validators/set.rs` & `pydantic_core-2.9.0/src/validators/set.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/validators/string.rs` & `pydantic_core-2.9.0/src/validators/string.rs`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 use crate::tools::SchemaDict;
 
 use super::{BuildValidator, CombinedValidator, DefinitionsBuilder, ValidationState, Validator};
 
 #[derive(Debug, Clone)]
 pub struct StrValidator {
     strict: bool,
+    coerce_numbers_to_str: bool,
 }
 
 impl BuildValidator for StrValidator {
     const EXPECTED_TYPE: &'static str = "str";
 
     fn build(
         schema: &PyDict,
@@ -26,14 +27,15 @@
         let con_str_validator = StrConstrainedValidator::build(schema, config)?;
 
         if con_str_validator.has_constraints_set() {
             Ok(con_str_validator.into())
         } else {
             Ok(Self {
                 strict: con_str_validator.strict,
+                coerce_numbers_to_str: con_str_validator.coerce_numbers_to_str,
             }
             .into())
         }
     }
 }
 
 impl_py_gc_traverse!(StrValidator {});
@@ -41,15 +43,15 @@
 impl Validator for StrValidator {
     fn validate<'data>(
         &self,
         py: Python<'data>,
         input: &'data impl Input<'data>,
         state: &mut ValidationState,
     ) -> ValResult<'data, PyObject> {
-        let either_str = input.validate_str(state.strict_or(self.strict))?;
+        let either_str = input.validate_str(state.strict_or(self.strict), self.coerce_numbers_to_str)?;
         Ok(either_str.into_py(py))
     }
 
     fn different_strict_behavior(
         &self,
         _definitions: Option<&DefinitionsBuilder<CombinedValidator>>,
         ultra_strict: bool,
@@ -72,26 +74,27 @@
     strict: bool,
     pattern: Option<Regex>,
     max_length: Option<usize>,
     min_length: Option<usize>,
     strip_whitespace: bool,
     to_lower: bool,
     to_upper: bool,
+    coerce_numbers_to_str: bool,
 }
 
 impl_py_gc_traverse!(StrConstrainedValidator {});
 
 impl Validator for StrConstrainedValidator {
     fn validate<'data>(
         &self,
         py: Python<'data>,
         input: &'data impl Input<'data>,
         state: &mut ValidationState,
     ) -> ValResult<'data, PyObject> {
-        let either_str = input.validate_str(state.strict_or(self.strict))?;
+        let either_str = input.validate_str(state.strict_or(self.strict), self.coerce_numbers_to_str)?;
         let cow = either_str.as_cow()?;
         let mut str = cow.as_ref();
         if self.strip_whitespace {
             str = str.trim();
         }
 
         let str_len: Option<usize> = if self.min_length.is_some() | self.max_length.is_some() {
@@ -184,22 +187,28 @@
         )?
         .unwrap_or(false);
         let to_lower: bool =
             schema_or_config(schema, config, intern!(py, "to_lower"), intern!(py, "str_to_lower"))?.unwrap_or(false);
         let to_upper: bool =
             schema_or_config(schema, config, intern!(py, "to_upper"), intern!(py, "str_to_upper"))?.unwrap_or(false);
 
+        let coerce_numbers_to_str = config
+            .and_then(|c| c.get_item("coerce_numbers_to_str"))
+            .and_then(|v| v.is_true().ok())
+            .unwrap_or(false);
+
         Ok(Self {
             strict: is_strict(schema, config)?,
             pattern,
             min_length,
             max_length,
             strip_whitespace,
             to_lower,
             to_upper,
+            coerce_numbers_to_str,
         })
     }
 
     // whether any of the constraints/customisations are actually enabled
     // except strict which can be set on StrValidator
     fn has_constraints_set(&self) -> bool {
         self.pattern.is_some()
```

### Comparing `pydantic_core-2.8.0/src/validators/time.rs` & `pydantic_core-2.9.0/src/validators/time.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/validators/timedelta.rs` & `pydantic_core-2.9.0/src/validators/timedelta.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/validators/tuple.rs` & `pydantic_core-2.9.0/src/validators/tuple.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/validators/typed_dict.rs` & `pydantic_core-2.9.0/src/validators/typed_dict.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
+use std::ops::ControlFlow;
+
 use pyo3::intern;
 use pyo3::prelude::*;
 use pyo3::types::{PyDict, PyString};
 
 use ahash::AHashSet;
 
 use crate::build_tools::py_schema_err;
 use crate::build_tools::{is_strict, schema_or_config, schema_or_config_same, ExtraBehavior};
-use crate::errors::{py_err_string, ErrorType, ErrorTypeDefaults, ValError, ValLineError, ValResult};
+use crate::errors::{ErrorTypeDefaults, ValError, ValLineError, ValResult};
 use crate::input::{
-    AttributesGenericIterator, DictGenericIterator, GenericMapping, Input, JsonObjectGenericIterator,
-    MappingGenericIterator,
+    AttributesGenericIterator, BorrowInput, DictGenericIterator, GenericMapping, Input, JsonObjectGenericIterator,
+    MappingGenericIterator, StringMappingGenericIterator,
 };
 use crate::lookup_key::LookupKey;
 use crate::tools::SchemaDict;
 
 use super::{
     build_validator, BuildValidator, CombinedValidator, DefinitionsBuilder, Extra, ValidationState, Validator,
 };
 
-use std::ops::ControlFlow;
-
 #[derive(Debug, Clone)]
 struct TypedDictField {
     name: String,
     lookup_key: LookupKey,
     name_py: Py<PyString>,
     required: bool,
     validator: CombinedValidator,
@@ -177,43 +177,43 @@
                 match state.with_new_extra(Extra {
                     data: Some(output_dict),
                     ..*state.extra()
                 }, |state| {
                     for field in &self.fields {
                         let op_key_value = match field.lookup_key.$get_method($dict $(, $kwargs )? ) {
                             Ok(v) => v,
-                            Err(err) => {
-                                errors.push(ValLineError::new_with_loc(
-                                    ErrorType::GetAttributeError {
-                                        error: py_err_string(py, err),
-                                        context: None,
-                                    },
-                                    input,
-                                    field.name.clone(),
-                                ));
+                            Err(ValError::LineErrors(line_errors)) => {
+                                for err in line_errors {
+                                    errors.push(err.with_outer_location(field.name.as_loc_item()));
+                                }
                                 continue;
                             }
+                            Err(err) => return ControlFlow::Break(err),
                         };
                         if let Some((lookup_path, value)) = op_key_value {
                             if let Some(ref mut used_keys) = used_keys {
                                 // key is "used" whether or not validation passes, since we want to skip this key in
                                 // extra logic either way
                                 used_keys.insert(lookup_path.first_key());
                             }
-                            match field.validator.validate(py, value, state) {
+                            match field.validator.validate(py, value.borrow_input(), state) {
                                 Ok(value) => {
                                     control_flow!(output_dict.set_item(&field.name_py, value))?;
                                 }
                                 Err(ValError::Omit) => continue,
                                 Err(ValError::LineErrors(line_errors)) => {
                                     for err in line_errors {
-                                        errors.push(lookup_path.apply_error_loc(err, self.loc_by_alias, &field.name));
+                                        errors.push(
+                                            lookup_path
+                                            .apply_error_loc(err, self.loc_by_alias, &field.name)
+                                            .into_owned(py)
+                                        );
                                     }
                                 }
-                                Err(err) => return ControlFlow::Break(err),
+                                Err(err) => return ControlFlow::Break(err.into_owned(py)),
                             }
                             continue;
                         } else if let Some(value) = control_flow!(field.validator.default_value(py, Some(field.name.as_str()), state))? {
                             control_flow!(output_dict.set_item(&field.name_py, value))?;
                         } else if field.required {
                             errors.push(field.lookup_key.error(
                                 ErrorTypeDefaults::Missing,
@@ -234,62 +234,73 @@
                         let (raw_key, value) = item_result?;
                         let either_str = match raw_key.strict_str() {
                             Ok(k) => k,
                             Err(ValError::LineErrors(line_errors)) => {
                                 for err in line_errors {
                                     errors.push(
                                         err.with_outer_location(raw_key.as_loc_item())
-                                            .with_type(ErrorTypeDefaults::InvalidKey),
+                                            .with_type(ErrorTypeDefaults::InvalidKey)
+                                            .into_owned(py)
                                     );
                                 }
                                 continue;
                             }
-                            Err(err) => return Err(err),
+                            Err(err) => return Err(err.into_owned(py)),
                         };
-                        if used_keys.contains(either_str.as_cow()?.as_ref()) {
+                        let cow = either_str.as_cow().map_err(|err| err.into_owned(py))?;
+                        if used_keys.contains(cow.as_ref()) {
                             continue;
                         }
 
+                        let value = value.borrow_input();
                         // Unknown / extra field
                         match self.extra_behavior {
                             ExtraBehavior::Forbid => {
-                                errors.push(ValLineError::new_with_loc(
-                                    ErrorTypeDefaults::ExtraForbidden,
-                                    value,
-                                    raw_key.as_loc_item(),
-                                ));
+                                errors.push(
+                                    ValLineError::new_with_loc(
+                                        ErrorTypeDefaults::ExtraForbidden,
+                                        value,
+                                        raw_key.as_loc_item(),
+                                    )
+                                    .into_owned(py)
+                                );
                             }
                             ExtraBehavior::Ignore => {}
                             ExtraBehavior::Allow => {
                             let py_key = either_str.as_py_string(py);
                                 if let Some(ref validator) = self.extras_validator {
                                     match validator.validate(py, value, state) {
                                         Ok(value) => {
                                             output_dict.set_item(py_key, value)?;
                                         }
                                         Err(ValError::LineErrors(line_errors)) => {
                                             for err in line_errors {
-                                                errors.push(err.with_outer_location(raw_key.as_loc_item()));
+                                                errors.push(
+                                                    err
+                                                    .with_outer_location(raw_key.as_loc_item())
+                                                    .into_owned(py)
+                                                );
                                             }
                                         }
-                                        Err(err) => return Err(err),
+                                        Err(err) => return Err(err.into_owned(py)),
                                     }
                                 } else {
                                     output_dict.set_item(py_key, value.to_object(py))?;
                                 };
                             }
                         }
                     }
                 }
             }};
         }
         match dict {
             GenericMapping::PyDict(d) => process!(d, py_get_dict_item, DictGenericIterator),
-            GenericMapping::PyGetAttr(d, kwargs) => process!(d, py_get_attr, AttributesGenericIterator, kwargs),
             GenericMapping::PyMapping(d) => process!(d, py_get_mapping_item, MappingGenericIterator),
+            GenericMapping::StringMapping(d) => process!(d, py_get_string_mapping_item, StringMappingGenericIterator),
+            GenericMapping::PyGetAttr(d, kwargs) => process!(d, py_get_attr, AttributesGenericIterator, kwargs),
             GenericMapping::JsonObject(d) => process!(d, json_get, JsonObjectGenericIterator),
         }
 
         if !errors.is_empty() {
             Err(ValError::LineErrors(errors))
         } else {
             Ok(output_dict.to_object(py))
```

### Comparing `pydantic_core-2.8.0/src/validators/union.rs` & `pydantic_core-2.9.0/src/validators/union.rs`

 * *Files 0% similar despite different names*

```diff
@@ -451,16 +451,17 @@
                         }
                     }};
                 }
                 let from_attributes = state.extra().from_attributes.unwrap_or(self.from_attributes);
                 let dict = input.validate_model_fields(self.strict, from_attributes)?;
                 let tag = match dict {
                     GenericMapping::PyDict(dict) => find_validator!(py_get_dict_item, dict),
-                    GenericMapping::PyGetAttr(obj, kwargs) => find_validator!(py_get_attr, obj, kwargs),
                     GenericMapping::PyMapping(mapping) => find_validator!(py_get_mapping_item, mapping),
+                    GenericMapping::StringMapping(d) => find_validator!(py_get_dict_item, d),
+                    GenericMapping::PyGetAttr(obj, kwargs) => find_validator!(py_get_attr, obj, kwargs),
                     GenericMapping::JsonObject(mapping) => find_validator!(json_get, mapping),
                 }?;
                 self.find_call_validator(py, tag, input, state)
             }
             Discriminator::Function(ref func) => {
                 let tag = func.call1(py, (input.to_object(py),))?;
                 if tag.is_none(py) {
```

### Comparing `pydantic_core-2.8.0/src/validators/url.rs` & `pydantic_core-2.9.0/src/validators/url.rs`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     fn complete(&mut self, _definitions: &DefinitionsBuilder<CombinedValidator>) -> PyResult<()> {
         Ok(())
     }
 }
 
 impl UrlValidator {
     fn get_url<'s, 'data>(&'s self, input: &'data impl Input<'data>, strict: bool) -> ValResult<'data, Url> {
-        match input.validate_str(strict) {
+        match input.validate_str(strict, false) {
             Ok(either_str) => {
                 let cow = either_str.as_cow()?;
                 let url_str = cow.as_ref();
 
                 self.check_length(input, url_str)?;
 
                 parse_url(url_str, input, strict)
@@ -247,15 +247,15 @@
     fn complete(&mut self, _definitions: &DefinitionsBuilder<CombinedValidator>) -> PyResult<()> {
         Ok(())
     }
 }
 
 impl MultiHostUrlValidator {
     fn get_url<'s, 'data>(&'s self, input: &'data impl Input<'data>, strict: bool) -> ValResult<'data, PyMultiHostUrl> {
-        match input.validate_str(strict) {
+        match input.validate_str(strict, false) {
             Ok(either_str) => {
                 let cow = either_str.as_cow()?;
                 let url_str = cow.as_ref();
 
                 self.check_length(input, || url_str.len())?;
 
                 parse_multihost_url(url_str, input, strict)
```

### Comparing `pydantic_core-2.8.0/src/validators/uuid.rs` & `pydantic_core-2.9.0/src/validators/uuid.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/src/validators/validation_state.rs` & `pydantic_core-2.9.0/src/validators/validation_state.rs`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     /// Temporarily rebinds the extra field by calling `f` to modify extra.
     ///
     /// When `ValidationStateWithReboundExtra` drops, the extra field is restored to its original value.
     pub fn rebind_extra<'state>(
         &'state mut self,
         f: impl FnOnce(&mut Extra<'a>),
     ) -> ValidationStateWithReboundExtra<'state, 'a> {
+        #[allow(clippy::unnecessary_struct_initialization)]
         let old_extra = Extra { ..self.extra };
         f(&mut self.extra);
         ValidationStateWithReboundExtra { state: self, old_extra }
     }
 
     pub fn extra(&self) -> &'_ Extra<'a> {
         &self.extra
```

### Comparing `pydantic_core-2.8.0/src/validators/with_default.rs` & `pydantic_core-2.9.0/src/validators/with_default.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/benchmarks/complete_schema.py` & `pydantic_core-2.9.0/tests/benchmarks/complete_schema.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/benchmarks/test_complete_benchmark.py` & `pydantic_core-2.9.0/tests/benchmarks/test_complete_benchmark.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/benchmarks/test_micro_benchmarks.py` & `pydantic_core-2.9.0/tests/benchmarks/test_micro_benchmarks.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/benchmarks/test_serialization_micro.py` & `pydantic_core-2.9.0/tests/benchmarks/test_serialization_micro.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/conftest.py` & `pydantic_core-2.9.0/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,17 @@
     ):
         self.validator = SchemaValidator(schema, config)
         self.validator_type = validator_type
 
     def validate_python(self, py_input, strict: bool | None = None, context: Any = None):
         return self.validator.validate_python(py_input, strict=strict, context=context)
 
+    def validate_json(self, json_str: str, strict: bool | None = None, context: Any = None):
+        return self.validator.validate_json(json_str, strict=strict, context=context)
+
     def validate_test(self, py_input, strict: bool | None = None, context: Any = None):
         if self.validator_type == 'json':
             return self.validator.validate_json(
                 json.dumps(py_input, default=json_default), strict=strict, context=context
             )
         else:
             assert self.validator_type == 'python', self.validator_type
```

### Comparing `pydantic_core-2.8.0/tests/emscripten_runner.js` & `pydantic_core-2.9.0/tests/emscripten_runner.js`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/requirements.txt` & `pydantic_core-2.9.0/tests/requirements.txt`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/serializers/test_any.py` & `pydantic_core-2.9.0/tests/serializers/test_any.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/serializers/test_bytes.py` & `pydantic_core-2.9.0/tests/serializers/test_bytes.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/serializers/test_dataclasses.py` & `pydantic_core-2.9.0/tests/serializers/test_dataclasses.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/serializers/test_datetime.py` & `pydantic_core-2.9.0/tests/serializers/test_datetime.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/serializers/test_decimal.py` & `pydantic_core-2.9.0/tests/serializers/test_decimal.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/serializers/test_definitions.py` & `pydantic_core-2.9.0/tests/serializers/test_definitions.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/serializers/test_definitions_recursive.py` & `pydantic_core-2.9.0/tests/serializers/test_definitions_recursive.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/serializers/test_dict.py` & `pydantic_core-2.9.0/tests/serializers/test_dict.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/serializers/test_format.py` & `pydantic_core-2.9.0/tests/serializers/test_format.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/serializers/test_functions.py` & `pydantic_core-2.9.0/tests/serializers/test_functions.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/serializers/test_generator.py` & `pydantic_core-2.9.0/tests/serializers/test_generator.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/serializers/test_json.py` & `pydantic_core-2.9.0/tests/serializers/test_json.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/serializers/test_json_or_python.py` & `pydantic_core-2.9.0/tests/serializers/test_json_or_python.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/serializers/test_list_tuple.py` & `pydantic_core-2.9.0/tests/serializers/test_list_tuple.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/serializers/test_literal.py` & `pydantic_core-2.9.0/tests/serializers/test_literal.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/serializers/test_misc.py` & `pydantic_core-2.9.0/tests/serializers/test_misc.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/serializers/test_model.py` & `pydantic_core-2.9.0/tests/serializers/test_model.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/serializers/test_model_root.py` & `pydantic_core-2.9.0/tests/serializers/test_model_root.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/serializers/test_none.py` & `pydantic_core-2.9.0/tests/serializers/test_none.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/serializers/test_nullable.py` & `pydantic_core-2.9.0/tests/serializers/test_nullable.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/serializers/test_other.py` & `pydantic_core-2.9.0/tests/serializers/test_other.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/serializers/test_set_frozenset.py` & `pydantic_core-2.9.0/tests/serializers/test_set_frozenset.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/serializers/test_simple.py` & `pydantic_core-2.9.0/tests/serializers/test_simple.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/serializers/test_string.py` & `pydantic_core-2.9.0/tests/serializers/test_string.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/serializers/test_timedelta.py` & `pydantic_core-2.9.0/tests/serializers/test_timedelta.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/serializers/test_typed_dict.py` & `pydantic_core-2.9.0/tests/serializers/test_typed_dict.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/serializers/test_union.py` & `pydantic_core-2.9.0/tests/serializers/test_union.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import dataclasses
 import json
 import re
-from typing import Union
+from typing import Any, ClassVar, Union
 
 import pytest
 from typing_extensions import Literal
 
 from pydantic_core import PydanticSerializationUnexpectedValue, SchemaSerializer, core_schema
 
 
@@ -397,7 +397,60 @@
         )
     )
 
     m = Model(value=data, value_types_reversed=data)
 
     assert s.to_python(m) == {'value': data, 'value_types_reversed': data}
     assert s.to_json(m) == f'{{"value":{json_value},"value_types_reversed":{json_value}}}'.encode()
+
+
+def test_union_serializes_model_subclass_from_definition() -> None:
+    class BaseModel:
+        __slots__ = '__dict__', '__pydantic_fields_set__', '__pydantic_extra__', '__pydantic_private__'
+
+        def __init__(self, **kwargs: Any):
+            for key, value in kwargs.items():
+                setattr(self, key, value)
+
+    class User(BaseModel):
+        name: str
+
+    class DBUser(User):
+        password: str
+        __pydantic_serializer__: ClassVar[SchemaSerializer]
+
+    DBUser.__pydantic_serializer__ = SchemaSerializer(
+        core_schema.model_schema(
+            DBUser,
+            core_schema.model_fields_schema(
+                {
+                    'name': core_schema.model_field(core_schema.str_schema()),
+                    'password': core_schema.model_field(core_schema.str_schema()),
+                }
+            ),
+        )
+    )
+
+    class Item(BaseModel):
+        price: float
+
+    s = SchemaSerializer(
+        core_schema.definitions_schema(
+            core_schema.union_schema(
+                [core_schema.definition_reference_schema('User'), core_schema.definition_reference_schema('Item')]
+            ),
+            [
+                core_schema.model_schema(
+                    User,
+                    core_schema.model_fields_schema({'name': core_schema.model_field(core_schema.str_schema())}),
+                    ref='User',
+                ),
+                core_schema.model_schema(
+                    Item,
+                    core_schema.model_fields_schema({'price': core_schema.model_field(core_schema.float_schema())}),
+                    ref='Item',
+                ),
+            ],
+        )
+    )
+
+    assert s.to_python(DBUser(name='John', password='secret')) == {'name': 'John'}
```

### Comparing `pydantic_core-2.8.0/tests/serializers/test_url.py` & `pydantic_core-2.9.0/tests/serializers/test_url.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/serializers/test_uuid.py` & `pydantic_core-2.9.0/tests/serializers/test_uuid.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/test.rs` & `pydantic_core-2.9.0/tests/test.rs`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/test_build.py` & `pydantic_core-2.9.0/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/test_config.py` & `pydantic_core-2.9.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/test_docstrings.py` & `pydantic_core-2.9.0/tests/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/test_errors.py` & `pydantic_core-2.9.0/tests/test_errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1066,7 +1066,25 @@
     assert str(exc_info.value) == (
         "1 validation error for typed-dict\n"
         "`foo.bar`.0\n"
         "  Input should be a valid integer, unable to parse string as an integer "
         "[type=int_parsing, input_value='x', input_type=str]\n"
         f'    For further information visit https://errors.pydantic.dev/{pydantic_version}/v/int_parsing'
     )
+
+
+def test_hide_input_in_error() -> None:
+    s = SchemaValidator({'type': 'int'})
+    with pytest.raises(ValidationError) as exc_info:
+        s.validate_python('definitely not an int')
+
+    for error in exc_info.value.errors(include_input=False):
+        assert 'input' not in error
+
+
+def test_hide_input_in_json() -> None:
+    s = SchemaValidator({'type': 'int'})
+    with pytest.raises(ValidationError) as exc_info:
+        s.validate_python('definitely not an int')
+
+    for error in exc_info.value.errors(include_input=False):
+        assert 'input' not in error
```

### Comparing `pydantic_core-2.8.0/tests/test_garbage_collection.py` & `pydantic_core-2.9.0/tests/test_garbage_collection.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/test_hypothesis.py` & `pydantic_core-2.9.0/tests/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/test_isinstance.py` & `pydantic_core-2.9.0/tests/test_isinstance.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/test_json.py` & `pydantic_core-2.9.0/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/test_misc.py` & `pydantic_core-2.9.0/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/test_schema_functions.py` & `pydantic_core-2.9.0/tests/test_schema_functions.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/test_strict.py` & `pydantic_core-2.9.0/tests/test_strict.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/test_typing.py` & `pydantic_core-2.9.0/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/test_tzinfo.py` & `pydantic_core-2.9.0/tests/test_tzinfo.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/test_validation_context.py` & `pydantic_core-2.9.0/tests/test_validation_context.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_arguments.py` & `pydantic_core-2.9.0/tests/validators/test_arguments.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_bool.py` & `pydantic_core-2.9.0/tests/validators/test_bool.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,16 @@
 
 def test_bool_key(py_and_json: PyAndJson):
     v = py_and_json({'type': 'dict', 'keys_schema': {'type': 'bool'}, 'values_schema': {'type': 'int'}})
     assert v.validate_test({True: 1, False: 2}) == {True: 1, False: 2}
     assert v.validate_test({'true': 1, 'off': 2}) == {True: 1, False: 2}
     assert v.validate_test({'true': 1, 'off': 2}, strict=False) == {True: 1, False: 2}
     with pytest.raises(ValidationError, match='Input should be a valid boolean'):
-        v.validate_test({'true': 1, 'off': 2}, strict=True)
+        v.validate_python({'true': 1, 'off': 2}, strict=True)
+    assert v.validate_json('{"true": 1, "off": 2}', strict=True) == {True: 1, False: 2}
 
 
 def test_validate_assignment_not_supported() -> None:
     """
     This test is not bool specific, the implementation is the
     same for all validators (it's the default impl on the Validator trait).
     But we need to test this somewhere, so it is going in the bool tests for now.
```

### Comparing `pydantic_core-2.8.0/tests/validators/test_bytes.py` & `pydantic_core-2.9.0/tests/validators/test_bytes.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_call.py` & `pydantic_core-2.9.0/tests/validators/test_call.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_callable.py` & `pydantic_core-2.9.0/tests/validators/test_callable.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_chain.py` & `pydantic_core-2.9.0/tests/validators/test_chain.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_custom_error.py` & `pydantic_core-2.9.0/tests/validators/test_custom_error.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_dataclasses.py` & `pydantic_core-2.9.0/tests/validators/test_dataclasses.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_date.py` & `pydantic_core-2.9.0/tests/validators/test_date.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_datetime.py` & `pydantic_core-2.9.0/tests/validators/test_datetime.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_decimal.py` & `pydantic_core-2.9.0/tests/validators/test_decimal.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_definitions.py` & `pydantic_core-2.9.0/tests/validators/test_definitions.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_definitions_recursive.py` & `pydantic_core-2.9.0/tests/validators/test_definitions_recursive.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_dict.py` & `pydantic_core-2.9.0/tests/validators/test_dict.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_float.py` & `pydantic_core-2.9.0/tests/validators/test_float.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,16 @@
 
 
 def test_float_key(py_and_json: PyAndJson):
     v = py_and_json({'type': 'dict', 'keys_schema': {'type': 'float'}, 'values_schema': {'type': 'int'}})
     assert v.validate_test({'1': 1, '2': 2}) == {1: 1, 2: 2}
     assert v.validate_test({'1.5': 1, '2.4': 2}) == {1.5: 1, 2.4: 2}
     with pytest.raises(ValidationError, match='Input should be a valid number'):
-        v.validate_test({'1.5': 1, '2.5': 2}, strict=True)
+        v.validate_python({'1.5': 1, '2.5': 2}, strict=True)
+    assert v.validate_json('{"1.5": 1, "2.5": 2}', strict=True) == {1.5: 1, 2.5: 2}
 
 
 @pytest.mark.parametrize(
     'input_value,allow_inf_nan,expected',
     [
         ('NaN', True, FunctionCheck(math.isnan)),
         ('NaN', False, Err("Input should be a finite number [type=finite_number, input_value='NaN', input_type=str]")),
```

### Comparing `pydantic_core-2.8.0/tests/validators/test_frozenset.py` & `pydantic_core-2.9.0/tests/validators/test_frozenset.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_function.py` & `pydantic_core-2.9.0/tests/validators/test_function.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 import platform
 import re
 from copy import deepcopy
 from typing import Any, Dict, List, Type, Union
 
 import pytest
 from dirty_equals import HasRepr
@@ -196,26 +197,32 @@
         assert repr(validator) == str(validator)
         return plain_repr(validator)
 
     v = SchemaValidator(
         {'type': 'function-wrap', 'function': {'type': 'general', 'function': f}, 'schema': {'type': 'str'}}
     )
 
-    assert v.validate_python('input value') == 'ValidatorCallable(Str(StrValidator{strict:false}))'
+    assert (
+        v.validate_python('input value')
+        == 'ValidatorCallable(Str(StrValidator{strict:false,coerce_numbers_to_str:false}))'
+    )
 
 
 def test_function_wrap_str():
     def f(input_value, validator, info):
         return plain_repr(validator)
 
     v = SchemaValidator(
         {'type': 'function-wrap', 'function': {'type': 'general', 'function': f}, 'schema': {'type': 'str'}}
     )
 
-    assert v.validate_python('input value') == 'ValidatorCallable(Str(StrValidator{strict:false}))'
+    assert (
+        v.validate_python('input value')
+        == 'ValidatorCallable(Str(StrValidator{strict:false,coerce_numbers_to_str:false}))'
+    )
 
 
 def test_function_wrap_not_callable():
     with pytest.raises(SchemaError, match='function-wrap.function.typed-dict.function\n  Input should be callable'):
         SchemaValidator(
             {'type': 'function-wrap', 'function': {'type': 'general', 'function': []}, 'schema': {'type': 'str'}}
         )
@@ -967,7 +974,25 @@
     v.validate_python(Foo())
 
     # insert_assert(reprs)
     assert reprs == [
         'ValidationInfo(config=None, context=None)',
         "FieldValidationInfo(config=None, context=None, field_name='x')",
     ]
+
+
+def test_function_after_doesnt_change_mode() -> None:
+    # https://github.com/pydantic/pydantic/issues/7468 - function-after was
+    # incorrectly forcing Python validation mode
+
+    def identity(v):
+        return v
+
+    schema = core_schema.no_info_after_validator_function(identity, core_schema.date_schema(strict=True))
+    v = SchemaValidator(schema)
+
+    # this input should be valid JSON input, but isn't valid Python input, so
+    # the following tests will pass if the after_validator is not
+    # forcing the mode to Python
+    assert v.validate_json(b'"2000-01-01"') == datetime.date(2000, 1, 1)
+    with pytest.raises(ValidationError):
+        v.validate_python(b'"2000-01-01"')
```

### Comparing `pydantic_core-2.8.0/tests/validators/test_generator.py` & `pydantic_core-2.9.0/tests/validators/test_generator.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_int.py` & `pydantic_core-2.9.0/tests/validators/test_int.py`

 * *Files 1% similar despite different names*

```diff
@@ -398,15 +398,16 @@
         v.validate_json('nan')
 
 
 def test_int_key(py_and_json: PyAndJson):
     v = py_and_json({'type': 'dict', 'keys_schema': {'type': 'int'}, 'values_schema': {'type': 'int'}})
     assert v.validate_test({'1': 1, '2': 2}) == {1: 1, 2: 2}
     with pytest.raises(ValidationError, match='Input should be a valid integer'):
-        v.validate_test({'1': 1, '2': 2}, strict=True)
+        v.validate_python({'1': 1, '2': 2}, strict=True)
+    assert v.validate_json('{"1": 1, "2": 2}', strict=True) == {1: 1, 2: 2}
 
 
 def test_string_as_int_with_underscores() -> None:
     v = SchemaValidator({'type': 'int'})
     assert v.validate_python('1_000_000') == 1_000_000
     assert v.validate_json('"1_000_000"') == 1_000_000
```

### Comparing `pydantic_core-2.8.0/tests/validators/test_is_instance.py` & `pydantic_core-2.9.0/tests/validators/test_is_instance.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_is_subclass.py` & `pydantic_core-2.9.0/tests/validators/test_is_subclass.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_json.py` & `pydantic_core-2.9.0/tests/validators/test_json.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,34 +46,41 @@
 
 
 @pytest.mark.parametrize(
     'input_value,expected',
     [
         ('{"a": 1}', {'a': 1}),
         (b'{"a": 1}', {'a': 1}),
+        (
+            '🐈 Hello \ud800World',
+            Err(
+                'Input should be a valid string, unable to parse raw data as a unicode string '
+                "[type=string_unicode, input_value='🐈 Hello \\ud800World', input_type=str]"
+            ),
+        ),
         (bytearray(b'{"a": 1}'), {'a': 1}),
         (
             'xx',
             Err(
                 'Invalid JSON: expected value at line 1 column 1 '
-                "[type=json_invalid, input_value='xx', input_type=str"
+                "[type=json_invalid, input_value='xx', input_type=str]"
             ),
         ),
         (
             b'xx',
             Err(
                 'Invalid JSON: expected value at line 1 column 1 '
-                "[type=json_invalid, input_value=b'xx', input_type=bytes"
+                "[type=json_invalid, input_value=b'xx', input_type=bytes]"
             ),
         ),
         (
             bytearray(b'xx'),
             Err(
                 'Invalid JSON: expected value at line 1 column 1 '
-                "[type=json_invalid, input_value=bytearray(b'xx'), input_type=bytearray"
+                "[type=json_invalid, input_value=bytearray(b'xx'), input_type=bytearray]"
             ),
         ),
     ],
 )
 def test_any_python(input_value, expected):
     v = SchemaValidator(core_schema.json_schema())
     if isinstance(expected, Err):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pydantic_core-2.8.0/tests/validators/test_json_or_python.py` & `pydantic_core-2.9.0/tests/validators/test_json_or_python.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_lax_or_strict.py` & `pydantic_core-2.9.0/tests/validators/test_lax_or_strict.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_list.py` & `pydantic_core-2.9.0/tests/validators/test_list.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_literal.py` & `pydantic_core-2.9.0/tests/validators/test_literal.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_model.py` & `pydantic_core-2.9.0/tests/validators/test_model.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_model_fields.py` & `pydantic_core-2.9.0/tests/validators/test_model_fields.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_model_init.py` & `pydantic_core-2.9.0/tests/validators/test_model_init.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_model_root.py` & `pydantic_core-2.9.0/tests/validators/test_model_root.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_none.py` & `pydantic_core-2.9.0/tests/validators/test_none.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_nullable.py` & `pydantic_core-2.9.0/tests/validators/test_nullable.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_set.py` & `pydantic_core-2.9.0/tests/validators/test_set.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_string.py` & `pydantic_core-2.9.0/tests/validators/test_string.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 from decimal import Decimal
+from numbers import Number
 from typing import Any, Dict, Union
 
 import pytest
 
 from pydantic_core import SchemaError, SchemaValidator, ValidationError, core_schema
 
 from ..conftest import Err, PyAndJson, plain_repr
@@ -197,15 +198,18 @@
             'ctx': {'pattern': '11'},
         }
     ]
 
 
 def test_default_validator():
     v = SchemaValidator(core_schema.str_schema(strict=True, to_lower=False), {'str_strip_whitespace': False})
-    assert plain_repr(v) == 'SchemaValidator(title="str",validator=Str(StrValidator{strict:true}),definitions=[])'
+    assert (
+        plain_repr(v)
+        == 'SchemaValidator(title="str",validator=Str(StrValidator{strict:true,coerce_numbers_to_str:false}),definitions=[])'
+    )
 
 
 @pytest.fixture(scope='session', name='FruitEnum')
 def fruit_enum_fixture():
     from enum import Enum
 
     class FruitEnum(str, Enum):
@@ -249,7 +253,47 @@
     # unions do a first pass in strict mode
     # so verify that they don't match the str schema in strict mode
     # and preserve the type
     v = SchemaValidator(core_schema.union_schema([core_schema.str_schema(), core_schema.int_schema()]))
 
     assert not isinstance(v.validate_python(StrSubclass('')), StrSubclass)
     assert not isinstance(v.validate_python(StrSubclass(''), strict=True), StrSubclass)
+
+
+def test_coerce_numbers_to_str_disabled_in_strict_mode() -> None:
+    config = core_schema.CoreConfig(coerce_numbers_to_str=True)
+
+    v = SchemaValidator(core_schema.str_schema(strict=True), config)
+    with pytest.raises(ValidationError):
+        v.validate_python(42)
+    with pytest.raises(ValidationError):
+        v.validate_json('42')
+
+
+@pytest.mark.parametrize(
+    ('number', 'expected_str'),
+    [
+        pytest.param(42, '42', id='42'),
+        pytest.param(42.0, '42.0', id='42.0'),
+        pytest.param(Decimal('42.0'), '42.0', id="Decimal('42.0')"),
+    ],
+)
+def test_coerce_numbers_to_str(number: Number, expected_str: str) -> None:
+    config = core_schema.CoreConfig(coerce_numbers_to_str=True)
+
+    v = SchemaValidator(core_schema.str_schema(), config)
+    assert v.validate_python(number) == expected_str
+
+
+@pytest.mark.parametrize(
+    ('number', 'expected_str'),
+    [
+        pytest.param('42', '42', id='42'),
+        pytest.param('42.0', '42', id='42.0'),
+        pytest.param('42.13', '42.13', id='42.13'),
+    ],
+)
+def test_coerce_numbers_to_str_from_json(number: str, expected_str: str) -> None:
+    config = core_schema.CoreConfig(coerce_numbers_to_str=True)
+
+    v = SchemaValidator(core_schema.str_schema(), config)
+    assert v.validate_json(number) == expected_str
```

### Comparing `pydantic_core-2.8.0/tests/validators/test_tagged_union.py` & `pydantic_core-2.9.0/tests/validators/test_tagged_union.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_time.py` & `pydantic_core-2.9.0/tests/validators/test_time.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_timedelta.py` & `pydantic_core-2.9.0/tests/validators/test_timedelta.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_tuple.py` & `pydantic_core-2.9.0/tests/validators/test_tuple.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_typed_dict.py` & `pydantic_core-2.9.0/tests/validators/test_typed_dict.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_union.py` & `pydantic_core-2.9.0/tests/validators/test_union.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,15 +252,18 @@
     msg = r'Error building "union" validator:\s+SchemaError: One or more union choices required'
     with pytest.raises(SchemaError, match=msg):
         SchemaValidator({'type': 'union', 'choices': []})
 
 
 def test_one_choice():
     v = SchemaValidator({'type': 'union', 'choices': [{'type': 'str'}]})
-    assert plain_repr(v) == 'SchemaValidator(title="str",validator=Str(StrValidator{strict:false}),definitions=[])'
+    assert (
+        plain_repr(v)
+        == 'SchemaValidator(title="str",validator=Str(StrValidator{strict:false,coerce_numbers_to_str:false}),definitions=[])'
+    )
     assert v.validate_python('hello') == 'hello'
 
 
 def test_strict_union():
     v = SchemaValidator({'type': 'union', 'strict': True, 'choices': [{'type': 'bool'}, {'type': 'int'}]})
     assert v.validate_python(1) == 1
     assert v.validate_python(123) == 123
```

### Comparing `pydantic_core-2.8.0/tests/validators/test_url.py` & `pydantic_core-2.9.0/tests/validators/test_url.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_uuid.py` & `pydantic_core-2.9.0/tests/validators/test_uuid.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/tests/validators/test_with_default.py` & `pydantic_core-2.9.0/tests/validators/test_with_default.py`

 * *Files identical despite different names*

### Comparing `pydantic_core-2.8.0/Cargo.lock` & `pydantic_core-2.9.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -238,15 +238,15 @@
 checksum = "78803b62cbf1f46fde80d7c0e803111524b9877184cfe7c3033659490ac7a7da"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pydantic-core"
-version = "2.8.0"
+version = "2.9.0"
 dependencies = [
  "ahash",
  "base64",
  "enum_dispatch",
  "idna",
  "num-bigint",
  "pyo3",
```

### Comparing `pydantic_core-2.8.0/PKG-INFO` & `pydantic_core-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic_core
-Version: 2.8.0
+Version: 2.9.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

