# Comparing `tmp/peakrdl-python-0.7.3.tar.gz` & `tmp/peakrdl-python-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peakrdl-python-0.7.3.tar", last modified: Fri Mar 29 15:45:41 2024, max compression
+gzip compressed data, was "peakrdl-python-0.7.4.tar", last modified: Tue Apr  2 13:25:32 2024, max compression
```

## Comparing `peakrdl-python-0.7.3.tar` & `peakrdl-python-0.7.4.tar`

### file list

```diff
@@ -1,119 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:45:41.224554 peakrdl-python-0.7.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:45:41.200554 peakrdl-python-0.7.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:45:41.204554 peakrdl-python-0.7.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/.github/workflows/action.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    42682 2024-03-29 15:45:41.220554 peakrdl-python-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:45:41.208554 peakrdl-python-0.7.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/docs/api_components.rst
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/docs/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/docs/customisation.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13188 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/docs/generated_package.rst
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/docs/genindex.rst
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:45:41.204554 peakrdl-python-0.7.3/example/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:45:41.208554 peakrdl-python-0.7.3/example/array_access/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/example/array_access/array_access.rdl
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/example/array_access/demo_array_access.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:45:41.208554 peakrdl-python-0.7.3/example/optimised_access/
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/example/optimised_access/demo_optimised_access.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/example/optimised_access/optimised_access.rdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:45:41.208554 peakrdl-python-0.7.3/example/overridden_names/
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/example/overridden_names/over_ridden_names.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/example/overridden_names/overridden_names.rdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:45:41.208554 peakrdl-python-0.7.3/example/simulating_callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/example/simulating_callbacks/chip_with_a_GPIO.rdl
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/example/simulating_callbacks/flashing_the_LED.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:45:41.208554 peakrdl-python-0.7.3/example/tranversing_address_map/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/example/tranversing_address_map/chip_with_registers.rdl
--rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/example/tranversing_address_map/dumping_register_state_to_json_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/example/tranversing_address_map/reg_dump.json
--rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/example/tranversing_address_map/reseting_registers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10786 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/example/tranversing_address_map/writing_register_state_from_json_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/generate_testcases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 15:45:41.224554 peakrdl-python-0.7.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:45:41.204554 peakrdl-python-0.7.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:45:41.212554 peakrdl-python-0.7.3/src/peakrdl_python/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/src/peakrdl_python/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/src/peakrdl_python/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/src/peakrdl_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/src/peakrdl_python/__peakrdl__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/src/peakrdl_python/_node_walkers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18309 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/src/peakrdl_python/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:45:41.212554 peakrdl-python-0.7.3/src/peakrdl_python/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/src/peakrdl_python/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17816 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/src/peakrdl_python/lib/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6940 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/src/peakrdl_python/lib/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    27632 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/src/peakrdl_python/lib/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    25879 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/src/peakrdl_python/lib/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    32949 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/src/peakrdl_python/lib/register.py
--rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/src/peakrdl_python/safe_name_utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     9992 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/src/peakrdl_python/systemrdl_node_utility_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:45:41.216554 peakrdl-python-0.7.3/src/peakrdl_python/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/src/peakrdl_python/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20912 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/src/peakrdl_python/templates/addrmap.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/src/peakrdl_python/templates/addrmap_field.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     4998 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/src/peakrdl_python/templates/addrmap_memory.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/src/peakrdl_python/templates/addrmap_register.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/src/peakrdl_python/templates/addrmap_simulation.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/src/peakrdl_python/templates/addrmap_simulation_tb.jinja
--rw-r--r--   0 runner    (1001) docker     (127)    79217 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/src/peakrdl_python/templates/addrmap_tb.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/src/peakrdl_python/templates/baseclass_tb.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/src/peakrdl_python/templates/header.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/src/peakrdl_python/templates/header_tb.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/src/peakrdl_python/templates/reg_definitions.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:45:41.220554 peakrdl-python-0.7.3/src/peakrdl_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    42682 2024-03-29 15:45:41.000000 peakrdl-python-0.7.3/src/peakrdl_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-03-29 15:45:41.000000 peakrdl-python-0.7.3/src/peakrdl_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 15:45:41.000000 peakrdl-python-0.7.3/src/peakrdl_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-29 15:45:41.000000 peakrdl-python-0.7.3/src/peakrdl_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-29 15:45:41.000000 peakrdl-python-0.7.3/src/peakrdl_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-29 15:45:41.000000 peakrdl-python-0.7.3/src/peakrdl_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:45:41.216554 peakrdl-python-0.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/.mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:45:41.216554 peakrdl-python-0.7.3/tests/alternative_template_toml/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/alternative_template_toml/peakrdl.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:45:41.216554 peakrdl-python-0.7.3/tests/alternative_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/alternative_templates/header.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/alternative_templates/header_tb.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)    17866 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/pylint.rc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:45:41.220554 peakrdl-python-0.7.3/tests/testcases/
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/testcases/RDLFormatCode_example.rdl
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/testcases/addr_map.rdl
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/testcases/all_register_access_types.rdl
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/testcases/basic.rdl
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/testcases/block_a.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/testcases/block_b.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/testcases/different_array_types.rdl
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/testcases/enum_example.rdl
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/testcases/example_issue_106.rdl
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/testcases/field_scope.rdl
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/testcases/field_with_overridden_reset.rdl
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/testcases/fields_with_HW_write.rdl
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/testcases/fields_with_reset_values.rdl
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/testcases/memories.rdl
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/testcases/memories_with_registers.rdl
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/testcases/msb0_and_lsb0.rdl
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/testcases/multi_block.rdl
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/testcases/multifile.rdl
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/testcases/name_clash.rdl
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/testcases/overridden_python_name.rdl
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/testcases/parametrised_readonly_and_readwrite.rdl
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/testcases/regfile_and_arrays.rdl
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/testcases/same_but_different_enum.rdl
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/testcases/signals_definitions_at_various_levels.rdl
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/testcases/simple.rdl
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/testcases/simple.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/testcases/sizes_registers.rdl
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/testcases/write_only_enum_with_undefined_reset.rdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:45:41.220554 peakrdl-python-0.7.3/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/unit_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7452 2024-03-29 15:45:37.000000 peakrdl-python-0.7.3/tests/unit_tests/test_array_indexing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.250208 peakrdl-python-0.7.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.226208 peakrdl-python-0.7.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.230208 peakrdl-python-0.7.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/.github/workflows/action.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    42719 2024-04-02 13:25:32.250208 peakrdl-python-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.234208 peakrdl-python-0.7.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/docs/api_components.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/docs/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/docs/customisation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/docs/design_decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/docs/design_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14790 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/docs/generated_package.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/docs/genindex.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7730 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.226208 peakrdl-python-0.7.4/example/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.234208 peakrdl-python-0.7.4/example/array_access/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/array_access/array_access.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/array_access/demo_array_access.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.234208 peakrdl-python-0.7.4/example/enumerated_fields/
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/enumerated_fields/demo_enumerated_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/enumerated_fields/enumerated_fields.rdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.234208 peakrdl-python-0.7.4/example/optimised_access/
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/optimised_access/demo_optimised_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/optimised_access/demo_optimised_array_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/optimised_access/optimised_access.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/optimised_access/optimised_array_access.rdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.234208 peakrdl-python-0.7.4/example/overridden_names/
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/overridden_names/over_ridden_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/overridden_names/overridden_names.rdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.234208 peakrdl-python-0.7.4/example/simulating_callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/simulating_callbacks/chip_with_a_GPIO.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)     5116 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/simulating_callbacks/flashing_the_LED.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.234208 peakrdl-python-0.7.4/example/tranversing_address_map/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/tranversing_address_map/chip_with_registers.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/tranversing_address_map/dumping_register_state_to_json_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/tranversing_address_map/reg_dump.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/tranversing_address_map/reseting_registers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10786 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/tranversing_address_map/writing_register_state_from_json_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.238208 peakrdl-python-0.7.4/example/why_ral/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/why_ral/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/why_ral/gpio.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/why_ral/hardware_sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/why_ral/with_hal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/why_ral/with_ral.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/why_ral/without_ral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9333 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/generate_and_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/generate_testcases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 13:25:32.250208 peakrdl-python-0.7.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.230208 peakrdl-python-0.7.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.238208 peakrdl-python-0.7.4/src/peakrdl_python/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/__peakrdl__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/_node_walkers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20125 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.242208 peakrdl-python-0.7.4/src/peakrdl_python/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32764 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/lib/async_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31244 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/lib/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7669 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/lib/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28611 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/lib/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35122 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/lib/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39506 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/lib/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/lib/utility_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11493 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/safe_name_utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/systemrdl_node_utility_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.242208 peakrdl-python-0.7.4/src/peakrdl_python/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22374 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/templates/addrmap.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/templates/addrmap_field.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/templates/addrmap_memory.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/templates/addrmap_register.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/templates/addrmap_simulation.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/templates/addrmap_simulation_tb.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)    86012 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/templates/addrmap_tb.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/templates/baseclass_tb.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/templates/header.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/templates/header_tb.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/templates/reg_definitions.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.250208 peakrdl-python-0.7.4/src/peakrdl_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42719 2024-04-02 13:25:32.000000 peakrdl-python-0.7.4/src/peakrdl_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-02 13:25:32.000000 peakrdl-python-0.7.4/src/peakrdl_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:25:32.000000 peakrdl-python-0.7.4/src/peakrdl_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-02 13:25:32.000000 peakrdl-python-0.7.4/src/peakrdl_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-02 13:25:32.000000 peakrdl-python-0.7.4/src/peakrdl_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-02 13:25:32.000000 peakrdl-python-0.7.4/src/peakrdl_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.242208 peakrdl-python-0.7.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/.mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.242208 peakrdl-python-0.7.4/tests/alternative_template_toml/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/alternative_template_toml/peakrdl.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.246208 peakrdl-python-0.7.4/tests/alternative_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/alternative_templates/header.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/alternative_templates/header_tb.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)    17866 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/pylint.rc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.250208 peakrdl-python-0.7.4/tests/testcases/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/RDLFormatCode_example.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/addr_map.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/all_register_access_types.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/basic.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/block_a.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/block_b.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/different_array_types.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/enum_example.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/example_issue_106.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/field_scope.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/field_with_overridden_reset.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/fields_with_HW_write.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/fields_with_reset_values.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/memories.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/memories_with_registers.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/msb0_and_lsb0.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/multi_block.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/multifile.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/name_clash.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/overridden_python_name.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/parametrised_readonly_and_readwrite.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/regfile_and_arrays.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/same_but_different_enum.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/signals_definitions_at_various_levels.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/simple.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/simple.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/sizes_registers.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/sizes_registers_array.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/write_only_enum_with_undefined_reset.rdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.250208 peakrdl-python-0.7.4/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/unit_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11836 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/unit_tests/simple_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/unit_tests/test_array_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11899 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/unit_tests/test_optimised_reg_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11473 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/unit_tests/test_reg.py
```

### Comparing `peakrdl-python-0.7.3/.github/workflows/action.yaml` & `peakrdl-python-0.7.4/.github/workflows/action.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -32,14 +32,15 @@
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install .
           python -m pip install -U pylint
 
       - name: Run Lint
+        #run: pylint --rcfile tests/pylint.rc src/peakrdl_python tests/unit_tests
         run: pylint --rcfile tests/pylint.rc src/peakrdl_python
 
   mypy:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python
@@ -55,14 +56,15 @@
       - name: Type Check
         run: mypy src/peakrdl_python --config-file=tests/.mypy.ini
 
   tests:
     needs:
       - mypy
       - lint
+
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: [3.7, 3.8, 3.9, "3.10", "3.11", "3.12"]
 
     steps:
     - uses: actions/checkout@v4
@@ -73,18 +75,17 @@
         python-version: ${{ matrix.python-version }}
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install .
 
-
     - name: Run Unit Tests
       run: |
-        python -m unittest discover -s tests/unit_tests
+        python -m unittest discover -s tests/unit_tests -t .
 
     - name: Generate testcases
       run: |
 
         # one of the test cases uses IPxact so we need the importer
         python -m pip install peakrdl-ipxact
         # the generated code is type checked with mypy so this is needed
@@ -146,14 +147,29 @@
         cd ../..
 
         cd example/array_access/
         peakrdl python array_access.rdl -o .
         python -m demo_array_access
 
         cd ../..
+
+        cd example/enumerated_fields/
+        peakrdl python enumerated_fields.rdl -o .
+        python -m demo_enumerated_fields
+
+
+        cd ../..
+
+        cd example/why_ral/
+        peakrdl python gpio.rdl -o .
+        python -m without_ral
+        python -m with_ral
+        python -m with_hal
+
+        cd ../..
   #-------------------------------------------------------------------------------
   build:
     needs:
       - tests
       - lint
       - mypy
     name: Build source distribution
```

### Comparing `peakrdl-python-0.7.3/.gitignore` & `peakrdl-python-0.7.4/.gitignore`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.3/.readthedocs.yaml` & `peakrdl-python-0.7.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.3/LICENSE` & `peakrdl-python-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.3/PKG-INFO` & `peakrdl-python-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: peakrdl-python
-Version: 0.7.3
-Summary: Generate python wrapper for a register model compiled SystemRDL input
+Version: 0.7.4
+Summary: Generate Python Register Access Layer (RAL) from SystemRDL
 Author: Keith Brady
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -678,15 +678,15 @@
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Source, https://github.com/krcb197/PeakRDL-python
 Project-URL: Tracker, https://github.com/krcb197/PeakRDL-python/issues
 Project-URL: Documentation, https://peakrdl-python.readthedocs.io/
 Project-URL: Changelog, https://github.com/krcb197/PeakRDL-python/releases
-Keywords: SystmRDL,PeakRDL,CSR,compiler,tool,registers,generator,Python
+Keywords: SystemRDL,PeakRDL,CSR,compiler,tool,registers,generator,Python
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -699,20 +699,21 @@
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: systemrdl-compiler>=1.24.0
 Requires-Dist: jinja2
 Requires-Dist: asynctest; python_version < "3.8"
+Requires-Dist: typing-extensions; python_version < "3.11"
 
 ![CI](https://github.com/krcb197/PeakRDL-python/actions/workflows/action.yaml/badge.svg)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/peakrdl-python.svg)](https://pypi.org/project/peakrdl-python)
 [![Documentation Status](https://readthedocs.org/projects/peakrdl-python/badge/?version=latest)](https://peakrdl-python.readthedocs.io/en/latest/?badge=latest)
 [![Downloads](https://static.pepy.tech/badge/peakrdl-python)](https://pepy.tech/project/peakrdl-python)
 
-# PeakRDL-python
-Generate Python wrapper for a register model compiled SystemRDL input
+# peakrdl-python
+Generate Python Register Access Layer (RAL) from SystemRDL
 
 ## Documentation
-See the [PeakRDL Python Documentation](https://peakrdl-python.readthedocs.io/) for more details
+See the [peakrdl-python Documentation](https://peakrdl-python.readthedocs.io/) for more details
```

### Comparing `peakrdl-python-0.7.3/README.md` & `peakrdl-python-0.7.4/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ![CI](https://github.com/krcb197/PeakRDL-python/actions/workflows/action.yaml/badge.svg)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/peakrdl-python.svg)](https://pypi.org/project/peakrdl-python)
 [![Documentation Status](https://readthedocs.org/projects/peakrdl-python/badge/?version=latest)](https://peakrdl-python.readthedocs.io/en/latest/?badge=latest)
 [![Downloads](https://static.pepy.tech/badge/peakrdl-python)](https://pepy.tech/project/peakrdl-python)
 
-# PeakRDL-python
-Generate Python wrapper for a register model compiled SystemRDL input
+# peakrdl-python
+Generate Python Register Access Layer (RAL) from SystemRDL
 
 ## Documentation
-See the [PeakRDL Python Documentation](https://peakrdl-python.readthedocs.io/) for more details
+See the [peakrdl-python Documentation](https://peakrdl-python.readthedocs.io/) for more details
```

### Comparing `peakrdl-python-0.7.3/docs/api.rst` & `peakrdl-python-0.7.4/docs/api.rst`

 * *Files 11% similar despite different names*

```diff
@@ -12,27 +12,27 @@
     * building HTML documentation with PeakRDL HTML
     * building UVM using PeakRDL UVM
 
 Example
 =======
 
 The following example shows the compiling an SystemRDL file and then generating
-the python register abstraction layer using PeakRDL Python.
+the python register access layer using PeakRDL Python.
 
 .. code-block:: python
 
     from systemrdl import RDLCompiler
     from peakrdl_python.exporter import PythonExporter
 
     # compile the systemRDL
     rdlc = RDLCompiler()
     rdlc.compile_file('basic.rdl')
     spec = rdlc.elaborate(top_def_name='basic').top
 
-    # generate the python package register abstraction layer
+    # generate the python package register access layer
     exporter = PythonExporter()
     exporter.export(node=spec, path='generated_code')
 
 
 PythonExporter
 ==============
```

### Comparing `peakrdl-python-0.7.3/docs/api_components.rst` & `peakrdl-python-0.7.4/docs/api_components.rst`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.3/docs/conf.py` & `peakrdl-python-0.7.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.3/docs/customisation.rst` & `peakrdl-python-0.7.4/docs/customisation.rst`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     from peakrdl_python.exporter import PythonExporter
 
     # compile the systemRDL
     rdlc = RDLCompiler()
     rdlc.compile_file('basic.rdl')
     spec = rdlc.elaborate(top_def_name='basic').top
 
-    # generate the python package register abstraction layer
+    # generate the python package register access layer
     exporter = PythonExporter(user_template_dir='my_company_headers')
     exporter.export(node=spec, path='generated_code')
 
 alternatively it can be generated from the PeakRDL, this requires the PeakRDL TOML config options
 to be setup, see `Configuring PeakRDL <https://peakrdl.readthedocs.io/en/latest/configuring.html>`_
 
 .. code-block::
```

### Comparing `peakrdl-python-0.7.3/docs/generated_package.rst` & `peakrdl-python-0.7.4/docs/generated_package.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,51 @@
 Generated Package
 *****************
 
 Output Structure
 ================
-PeakRDL Python generates a python packages from a System RDL design, structured
-as shown below. The ``root_name`` will be based on the top level address map name
-with the package was generated
+PeakRDL Python generates a python Register Access Layer (RAL) from a System RDL design. The
+generated python code is contained in a package, structured as shown below. The ``root_name``
+will be based on the top level address map name with the package was generated
 
 | ``<root_name>``
 | ├── ``lib``
 | ├── ``reg_model``
 | │ └── ``<root_name>.py``
 | └── ``tests``
 |   └── ``test_<root_name>.py``
 
 In the folder structure above:
 
-- ``<root_name>.py`` - This is the register abstraction layer code for the design
-- ``lib`` - This is a package of base classes used by the register abstraction layer
-- ``test_<root_name>.py`` - This is a set of autogenerated unittests to verify the register abstraction layer
-
-
+- ``<root_name>.py`` - This is the register access layer code for the design
+- ``lib`` - This is a package of base classes used by the register access layer
+- ``test_<root_name>.py`` - This is a set of autogenerated unittests to verify the register access layer
 
 
 Running the Unit Tests
 ======================
 
 There are many ways to run Python Unit tests. A good place to start is the ``unittest`` module
 included in the Python standard installation.
 
 Callbacks
 =========
 
-The Register Abstraction Layer will typically interfaced to a driver that
+The Register Access Layer will typically interfaced to a driver that
 allows accesses the chip. However, it can also be interfaced to a simulation
 of the device.
 
-In order to operate the register abstraction layer typically requires the following:
+In order to operate the register access layer typically requires the following:
 
 - A callback for a single register write, this not required if there is no writable register in
-  the register abstraction layer
+  the register access layer
 - A callback for a single register read, this not required if there is no writable register in
-  the register abstraction layer
+  the register access layer
 
-In addition the register abstraction layer can make use of block operations where a block of the
+In addition the register access layer can make use of block operations where a block of the
 address space is read in a single transaction. Not all drivers support these
 
 The examples of these two methods are included within the generated register
 access layer package so that it can be used from the console:
 
 .. code-block:: python
 
@@ -93,24 +91,24 @@
 
 In addition there is also an option to use ``async`` callbacks if the package is built
 ``asyncoutput`` set to True.
 
 Callback Set
 ------------
 
-The callbacks are passed into the register abstraction layer using either:
+The callbacks are passed into the register access layer using either:
 
 * ``NormalCallbackSet`` for standard python function callbacks
 * ``AsyncCallbackSet`` for async python function callbacks, these are called from the library using
   ``await``
 
-Using the Register Abstraction Layer
-====================================
+Using the Register Access Layer
+===============================
 
-The register abstraction layer package is intended to integrated into another
+The register access layer package is intended to integrated into another
 piece of code. That code could be a simple test script for blinking an LED on a
 GPIO or it could be a more complex application with a GUI.
 
 The following example is a chip that has a GPIO block. The GPIO block has two
 registers:
 
 1. one register that controls the direction of the GPIO pin, at address 0x4
@@ -127,27 +125,74 @@
 .. code-block:: bash
 
     peakrdl python chip_with_a_GPIO.rdl -o python_output
     python -m unittest discover -s python_output
 
 .. tip:: It is always good practice to run the unittests on the generated code.
 
-Once the register abstraction layer has been generated and it can be used. The following example
+Once the register access layer has been generated and it can be used. The following example
 does not actually use a device driver. Instead it chip simulator with a a Tkinter GUI,
 incorporating a RED circle to represent the LED. The chip simulator has read and write methods (
 equivalent to those offered by a device driver), these look at the address of the write and update
 the internal state of the simulator accordingly, the LED is then updated based on the state of the
 simulator.
 
 .. literalinclude :: ../example/simulating_callbacks/flashing_the_LED.py
    :language: python
 
+Enumerated Fields
+-----------------
+
+Enumerations are a good practice to implicitly encode that have special meanings which can not be
+easily understood from the field name. The SystemRDL enumerations are implemented using python
+
+.. literalinclude :: ../example/enumerated_fields/enumerated_fields.rdl
+   :language: systemrdl
+
+This systemRDL code can be built using the command line tool as follows (assuming it is stored in
+a file called ``enumerated_fields.rdl``):
+
+.. code-block:: bash
+
+    peakrdl python enumerated_fields.rdl -o .
+
+The following example shows the usage of the enumeration
+
+.. note::
+   In order to set the value of an enumerated field, using the ``write()`` method. The correct
+   enumerated class is needed. This can be retrieved from the field itself with the ``enum_cls``
+   property
+
+.. literalinclude :: ../example/enumerated_fields/demo_enumerated_fields.py
+   :language: python
+
+Array Access
+------------
+
+SystemRDL supports multi-dimensional arrays, the following example shows an definition with an 1D and 3D array with various methods to access individual elements of the array and use of the iterators to walk through elements in loops
+
+.. literalinclude :: ../example/array_access/array_access.rdl
+   :language: systemrdl
+
+This systemRDL code can be built using the command line tool as follows (assuming it is stored in
+a file called ``array_access.rdl``):
+
+.. code-block:: bash
+
+    peakrdl python array_access.rdl -o .
+
+.. literalinclude :: ../example/array_access/demo_array_access.py
+   :language: python
+
 Optimised Access
 ----------------
 
+Working with individual registers
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
 Each time the ``read`` or ``write`` method for a register field is accessed the hardware is read
 and or written (a write to a field will normally require a preceding read). When accessing multiple
 fields in the same register, it may be desirable to use one of the optimised access methods.
 
 Consider the following example of an GPIO block with 4 GPIO pins (configured in a single register):
 
 .. literalinclude :: ../example/optimised_access/optimised_access.rdl
@@ -160,28 +205,45 @@
 * using the register context manager
 
 Both demonstrated in the following code example:
 
 .. literalinclude :: ../example/optimised_access/demo_optimised_access.py
    :language: python
 
+Working with registers arrays
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+In many systems it is more efficient to read and write in block operations rather than using
+individual register access.
+
+Consider the following example of an GPIO block with 8 GPIO pins (configured in a 8 registers):
+
+.. literalinclude :: ../example/optimised_access/optimised_array_access.rdl
+   :language: systemrdl
+
+In order to configure all the GPIOs a range of operations are shown with the use of the context
+managers to make more efficient operations
+
+.. literalinclude :: ../example/optimised_access/demo_optimised_array_access.py
+   :language: python
+
 Walking the Structure
 ---------------------
 
-The following two example show how to use the generators within the register abstraction layer
+The following two example show how to use the generators within the register access layer
 package to traverse the structure.
 
 Both examples use the following register set which has a number of features to demonstrate the
 structures
 
 .. literalinclude :: ../example/tranversing_address_map/chip_with_registers.rdl
    :language: systemrdl
 
 This systemRDL code can be built using the command line tool as follows (assuming it is stored in
-a file called ``chip_with_registers.rdl``:
+a file called ``chip_with_registers.rdl``):
 
 .. code-block:: bash
 
    peakrdl python chip_with_registers.rdl -o chip_with_registers
 
 
 Traversing without Unrolling Loops
@@ -282,33 +344,14 @@
 The second example is setting every register in the address map back to its default values. In
 this case the loops are unrolled to conveniently access all the register without needing to
 worry if they are in an array or not.
 
 .. literalinclude :: ../example/tranversing_address_map/reseting_registers.py
    :language: python
 
-
-Array Access
-------------
-
-SystemRDL supports multi-dimensional arrays, the following example shows an definition with an 1D and 3D array with various methods to access individual elements of the array and use of the iterators to walk through elements in loops
-
-.. literalinclude :: ../example/array_access/array_access.rdl
-   :language: systemrdl
-
-This systemRDL code can be built using the command line tool as follows (assuming it is stored in
-a file called ``array_access.rdl``:
-
-.. code-block:: bash
-
-    peakrdl python array_access.rdl -o .
-
-.. literalinclude :: ../example/array_access/demo_array_access.py
-   :language: python
-
 Python Safe Names
 =================
 
 The systemRDL structure is converted to a python class structure, there are two concerns:
 
 * if any systemRDL node name is a python keyname
 * if any systemRDL node name clashes with part of the peakrdl_standard types, for example all register nodes have an ``address`` property that would clash with a field of that register called ``address``
```

### Comparing `peakrdl-python-0.7.3/example/array_access/demo_array_access.py` & `peakrdl-python-0.7.4/example/array_access/demo_array_access.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.3/example/optimised_access/demo_optimised_access.py` & `peakrdl-python-0.7.4/example/optimised_access/demo_optimised_access.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.3/example/optimised_access/optimised_access.rdl` & `peakrdl-python-0.7.4/example/optimised_access/optimised_access.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.3/example/overridden_names/over_ridden_names.py` & `peakrdl-python-0.7.4/example/overridden_names/over_ridden_names.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.3/example/simulating_callbacks/chip_with_a_GPIO.rdl` & `peakrdl-python-0.7.4/example/simulating_callbacks/chip_with_a_GPIO.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.3/example/simulating_callbacks/flashing_the_LED.py` & `peakrdl-python-0.7.4/example/simulating_callbacks/flashing_the_LED.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
                 self.LED.itemconfig(self.LED_inner, fill='red')
             else:
                 self.LED.itemconfig(self.LED_inner, fill='black')
         else:
             self.LED.itemconfig(self.LED_inner, fill='black')
 
 # these two methods can be put in the simulator Tkinter event queue to perform register writes on
-# the register abstraction layer (in turn causing the state of the simulator to change)
+# the register access layer (in turn causing the state of the simulator to change)
 
 def turn_LED_on(chip: mychip_cls, sim_kt_root):
 
     # write a '1' to the LED state field
     chip.GPIO.GPIO_state.PIN_0.write(1)
     # set up another event to happen
     sim_kt_root.after(2000, turn_LED_off, chip, sim_kt_root)
@@ -110,15 +110,15 @@
     # set up another event to happen
     sim_kt_root.after(2000, turn_LED_on, chip, sim_kt_root)
 
 
 if __name__ == '__main__':
 
     # make an instance of the chip simulator and then locally defined the callbacks that will be
-    # used to by the register abstraction model
+    # used to by the register access model
     chip_simulator = ChipSim()
 
     def read_call_back(addr: int, width: int, accesswidth: int):
         return chip_simulator.read_addr_space(addr=addr,
                                               width=width,
                                               accesswidth=accesswidth)
     def write_call_back(addr: int, width: int, accesswidth: int, data: int):
```

### Comparing `peakrdl-python-0.7.3/example/tranversing_address_map/dumping_register_state_to_json_file.py` & `peakrdl-python-0.7.4/example/tranversing_address_map/dumping_register_state_to_json_file.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.3/example/tranversing_address_map/reg_dump.json` & `peakrdl-python-0.7.4/example/tranversing_address_map/reg_dump.json`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.3/example/tranversing_address_map/reseting_registers.py` & `peakrdl-python-0.7.4/example/tranversing_address_map/reseting_registers.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.3/example/tranversing_address_map/writing_register_state_from_json_file.py` & `peakrdl-python-0.7.4/example/tranversing_address_map/writing_register_state_from_json_file.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.3/generate_testcases.py` & `peakrdl-python-0.7.4/generate_testcases.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,29 @@
 #!/usr/bin/env python3
 
+"""
+peakrdl-python is a tool to generate Python Register Access Layer (RAL) from SystemRDL
+Copyright (C) 2021 - 2023
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+script to generate all the test cases from the test set
+"""
+
 import sys
 import os
 
 from glob import glob
 from typing import Optional, List
 
 from systemrdl import RDLCompiler # type: ignore
```

### Comparing `peakrdl-python-0.7.3/pyproject.toml` & `peakrdl-python-0.7.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -5,25 +5,26 @@
 [project]
 name = "peakrdl-python"
 dynamic = ["version"]
 requires-python = ">=3.7"
 dependencies = [
     "systemrdl-compiler>=1.24.0",
     "jinja2",
-    "asynctest;python_version<'3.8'"
+    "asynctest;python_version<'3.8'",
+    "typing-extensions;python_version<'3.11'"
 ]
 
 authors = [
     {name="Keith Brady"},
 ]
-description = "Generate python wrapper for a register model compiled SystemRDL input"
+description = "Generate Python Register Access Layer (RAL) from SystemRDL"
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = [
-    "SystmRDL", "PeakRDL", "CSR", "compiler", "tool", "registers", "generator",
+    "SystemRDL", "PeakRDL", "CSR", "compiler", "tool", "registers", "generator",
     "Python"
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
```

### Comparing `peakrdl-python-0.7.3/src/peakrdl_python/.coveragerc` & `peakrdl-python-0.7.4/src/peakrdl_python/.coveragerc`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.3/src/peakrdl_python/_node_walkers.py` & `peakrdl-python-0.7.4/src/peakrdl_python/_node_walkers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,35 @@
 """
+peakrdl-python is a tool to generate Python Register Access Layer (RAL) from SystemRDL
+Copyright (C) 2021 - 2023
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
 Node walkers to be used in the generated of the output code
 """
 from typing import Optional, List, Union, Iterator
 
 from systemrdl import RDLListener, WalkerAction # type: ignore
 from systemrdl.node import RegNode, MemNode, FieldNode, AddrmapNode, RegfileNode # type: ignore
 
 
 class AddressMaps(RDLListener):
     """
-    class intended to be used as part of the walker/listener protocol to find all the desendent
+    class intended to be used as part of the walker/listener protocol to find all the descendant
     address maps
     """
     def __init__(self) -> None:
         super().__init__()
         self.__address_maps: List[AddrmapNode] = []
 
     def enter_Addrmap(self, node: AddrmapNode) -> Optional[WalkerAction]:
@@ -82,24 +98,7 @@
         - registers
         - memories
 
         Returns: list of nodes
 
         """
         return self.addr_maps + self.reg_files + self.memories + self.registers
-
-    @property
-    def n_dimesional_array_nodes(self) -> List[Union[RegNode, MemNode, AddrmapNode, RegfileNode]]:
-        """
-        All the nodes owned by the address map which are arrays with more than 1 dimension,
-        including:
-        - address maps
-        - register files
-        - registers
-        - memories
-
-        Returns: list of nodes
-        """
-        def n_dimensional_node(node: Union[RegNode, MemNode, AddrmapNode, RegfileNode]) -> bool:
-            return node.is_array and (len(node.array_dimensions) > 1)
-
-        return list(filter(n_dimensional_node, self.addressable_nodes))
```

### Comparing `peakrdl-python-0.7.3/src/peakrdl_python/exporter.py` & `peakrdl-python-0.7.4/src/peakrdl_python/exporter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,25 @@
 """
-Main Classes for the PeakRDL Python
+peakrdl-python is a tool to generate Python Register Access Layer (RAL) from SystemRDL
+Copyright (C) 2021 - 2023
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Main Classes for the peakrdl-python
 """
 import os
 from pathlib import Path
 from shutil import copy
 from typing import List, NoReturn, Iterable, Tuple
 
 import jinja2 as jj
@@ -231,14 +247,16 @@
 
         # If it is the root node, skip to top addrmap
         if isinstance(node, RootNode):
             top_block = node.top
         else:
             top_block = node
 
+        if not isinstance(path, str):
+            raise TypeError(f'path should be a str but got {type(path)}')
         package = _Package(path=path,
                            package_name=node.inst_name,
                            include_tests=not skip_test_case_generation)
         package.create_empty_package(cleanup=delete_existing_package_content)
 
         self._build_node_type_table(top_block)
 
@@ -319,22 +337,36 @@
 
             for block in blocks:
                 owned_elements = OwnedbyAddressMap()
                 # running the walker populated the blocks with all the address maps in within the
                 # top block, including the top_block itself
                 RDLWalker(unroll=True).walk(block, owned_elements, skip_top=True)
 
+                # The code that generates the tests for the register array context managers needs
+                # the arrays rolled up but parents within the address map e.g. a regfile unrolled
+                # I have not found a way to do this with the Walker as the unroll seems to be a
+                # global setting, the following code works but it is not elegant
+                rolled_owned_reg: List[RegNode] = list(block.registers(unroll=False))
+                for regfile in owned_elements.reg_files:
+                    rolled_owned_reg += list(regfile.registers(unroll=False))
+                for memory in owned_elements.memories:
+                    rolled_owned_reg += list(memory.registers(unroll=False))
+                def is_reg_array(item: RegNode) -> bool:
+                    return item.is_array
+                rolled_owned_reg_array = filter(is_reg_array, rolled_owned_reg)
+
                 fq_block_name = '_'.join(block.get_path_segments(array_suffix = '_{index:d}_'))
                 module_tb_path = package.tests.child_module_path('test_' + fq_block_name + '.py')
 
                 context = {
                     'top_node': top_block,
                     'block' : block,
                     'fq_block_name' : fq_block_name,
                     'owned_elements': owned_elements,
+                    'rolled_owned_reg_array' : rolled_owned_reg_array,
                     'systemrdlFieldNode': FieldNode,
                     'systemrdlSignalNode': SignalNode,
                     'systemrdlRegNode': RegNode,
                     'systemrdlMemNode': MemNode,
                     'systemrdlRegfileNode': RegfileNode,
                     'systemrdlAddrmapNode': AddrmapNode,
                     'isinstance': isinstance,
```

### Comparing `peakrdl-python-0.7.3/src/peakrdl_python/lib/callbacks.py` & `peakrdl-python-0.7.4/src/peakrdl_python/lib/callbacks.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,26 @@
 """
-This module is intended to distributed as part of automatically generated code by the PeakRDL
-Python tool. It provides a set of types used by the autogenerated code to callbacks
+peakrdl-python is a tool to generate Python Register Access Layer (RAL) from SystemRDL
+Copyright (C) 2021 - 2023
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+This module is intended to distributed as part of automatically generated code by the
+peakrdl-python tool.  It provides a set of types used by the autogenerated code to callbacks
 """
 import sys
 
 from array import array as Array
 
 from typing import Optional, Union
```

### Comparing `peakrdl-python-0.7.3/src/peakrdl_python/lib/fields.py` & `peakrdl-python-0.7.4/src/peakrdl_python/lib/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,45 @@
 """
-This module is intended to distributed as part of automatically generated code by the PeakRDL
-Python tool. It provides a set of classes used by the autogenerated code to represent register
-fields
+peakrdl-python is a tool to generate Python Register Access Layer (RAL) from SystemRDL
+Copyright (C) 2021 - 2023
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+This module is intended to distributed as part of automatically generated code by the
+peakrdl-python tool. It provides a set of classes used by the autogenerated code to represent
+register fields
 """
 from enum import EnumMeta
 from typing import List, cast, Optional
 from abc import ABC, abstractmethod
 
 from .base import Base
-from .base import swap_msb_lsb_ordering
-from .register import Reg
-from .register import RegReadOnly, RegAsyncReadOnly
-from .register import RegReadWrite, RegAsyncReadWrite
-from .register import RegWriteOnly, RegAsyncWriteOnly
-from .register import ReadableRegister, ReadableAsyncRegister
-from .register import WritableRegister, WritableAsyncRegister
+from .utility_functions import swap_msb_lsb_ordering
+from .register import BaseReg
+from .register import RegReadOnly
+from .async_register import RegAsyncReadOnly
+from .register import RegReadWrite
+from .async_register import RegAsyncReadWrite
+from .register import RegWriteOnly
+from .async_register import RegAsyncWriteOnly
+from .register import ReadableRegister
+from .async_register import ReadableAsyncRegister
+from .register import WritableRegister
+from .async_register import WritableAsyncRegister
 
 
 class FieldSizeProps:
     """
     class to hold the key attributes of a field
     """
     __slots__ = ['__msb', '__lsb', '__width', '__high', '__low']
@@ -143,15 +164,16 @@
         It is not expected that this class will be instantiated under normal
         circumstances however, it is useful for type checking
     """
 
     __slots__ = ['__size_props', '__misc_props',
                  '__bitmask', '__msb0', '__lsb0']
 
-    def __init__(self, parent_register: Reg, size_props: FieldSizeProps, misc_props: FieldMiscProps,
+    def __init__(self, *,
+                 parent_register: BaseReg, size_props: FieldSizeProps, misc_props: FieldMiscProps,
                  logger_handle: str, inst_name: str):
 
         super().__init__(logger_handle=logger_handle,
                          inst_name=inst_name, parent=parent_register)
 
         if not isinstance(size_props, FieldSizeProps):
             raise TypeError(f'size_props must be of {type(FieldSizeProps)} '
@@ -159,16 +181,16 @@
         self.__size_props = size_props
 
         if not isinstance(misc_props, FieldMiscProps):
             raise TypeError(f'misc_props must be of {type(FieldMiscProps)} '
                             f'but got {type(misc_props)}')
         self.__misc_props = misc_props
 
-        if not isinstance(parent_register, Reg):
-            raise TypeError(f'parent_register must be of {type(Reg)} '
+        if not isinstance(parent_register, BaseReg):
+            raise TypeError(f'parent_register must be of {type(BaseReg)} '
                             f'but got {type(parent_register)}')
 
         if self.width > self.register_data_width:
             raise ValueError('width can not be greater than parent width')
 
         if self.high > self.register_data_width:
             raise ValueError(f'field high bit position {self.high:d} must be less than the '
@@ -322,20 +344,20 @@
     def is_volatile(self) -> bool:
         """
         The HW volatility of the field
         """
         return self.__misc_props.is_volatile
 
     @property
-    def __parent_register(self) -> Reg:
+    def __parent_register(self) -> BaseReg:
         """
         parent register the field is placed in
         """
         # this cast is OK because an explict typing check was done in the __init__
-        return cast(Reg, self.parent)
+        return cast(BaseReg, self.parent)
 
 class _FieldReadOnlyFramework(Field, ABC):
     """
     base class for a async or normal read only register field
 
     Args:
         parent_register: register within which the field resides
@@ -373,35 +395,35 @@
         else:
             return_value = swap_msb_lsb_ordering(value=(value & self.bitmask) >> self.low,
                                                  width=self.width)
 
         return return_value
 
     @property
-    def __parent_register(self) -> Reg:
+    def __parent_register(self) -> BaseReg:
         """
         parent register the field is placed in
         """
         # this cast is OK because an explict typing check was done in the __init__
-        return cast(Reg, self.parent)
+        return cast(BaseReg, self.parent)
 
 class FieldReadOnly(_FieldReadOnlyFramework, ABC):
     """
     class for a read only register field
 
     Args:
         parent_register: register within which the field resides
         size_props: object defining the msb, lsb, high bit, low bit and width
         logger_handle: name to be used logging messages associate with this
             object
 
     """
     __slots__ : List[str] = []
 
-    def __init__(self,
+    def __init__(self, *,
                  parent_register: ReadableRegister,
                  size_props: FieldSizeProps,
                  misc_props: FieldMiscProps,
                  logger_handle: str,
                  inst_name: str):
 
         if not isinstance(parent_register, (RegReadWrite, RegReadOnly)):
@@ -488,15 +510,15 @@
         size_props: object defining the msb, lsb, high bit, low bit and width
         logger_handle: name to be used logging messages associate with this
             object
 
     """
     __slots__ : List[str] = []
 
-    def __init__(self,
+    def __init__(self, *,
                  parent_register: WritableRegister,
                  size_props: FieldSizeProps,
                  misc_props: FieldMiscProps,
                  logger_handle: str,
                  inst_name: str):
 
         if not isinstance(parent_register, (RegReadWrite, RegWriteOnly)):
@@ -575,17 +597,18 @@
     Args:
         parent_register: register within which the field resides
         size_props: object defining the msb, lsb, high bit, low bit and width
         logger_handle: name to be used logging messages associate with this
             object
 
     """
-    __slots__ : List[str]  = []
+    __slots__ : List[str] = []
 
-    def __init__(self, parent_register: RegReadWrite,
+    def __init__(self, *,
+                 parent_register: RegReadWrite,
                  size_props: FieldSizeProps,
                  misc_props: FieldMiscProps,
                  logger_handle: str,
                  inst_name: str):
 
         if not isinstance(parent_register, RegReadWrite):
             raise TypeError(f'size_props must be of {type(RegReadWrite)} '
@@ -615,15 +638,15 @@
         size_props: object defining the msb, lsb, high bit, low bit and width
         logger_handle: name to be used logging messages associate with this
             object
 
     """
     __slots__ : List[str] = []
 
-    def __init__(self,
+    def __init__(self, *,
                  parent_register: ReadableAsyncRegister,
                  size_props: FieldSizeProps,
                  misc_props: FieldMiscProps,
                  logger_handle: str,
                  inst_name: str):
 
         if not isinstance(parent_register, (RegAsyncReadWrite, RegAsyncReadOnly)):
@@ -666,15 +689,15 @@
         size_props: object defining the msb, lsb, high bit, low bit and width
         logger_handle: name to be used logging messages associate with this
             object
 
     """
     __slots__ : List[str] = []
 
-    def __init__(self,
+    def __init__(self, *,
                  parent_register: WritableAsyncRegister,
                  size_props: FieldSizeProps,
                  misc_props: FieldMiscProps,
                  logger_handle: str,
                  inst_name: str):
 
         if not isinstance(parent_register, (RegAsyncReadWrite, RegAsyncWriteOnly)):
@@ -753,15 +776,16 @@
         size_props: object defining the msb, lsb, high bit, low bit and width
         logger_handle: name to be used logging messages associate with this
             object
 
     """
     __slots__ : List[str] = []
 
-    def __init__(self, parent_register: RegAsyncReadWrite,
+    def __init__(self, *,
+                 parent_register: RegAsyncReadWrite,
                  size_props: FieldSizeProps,
                  misc_props: FieldMiscProps,
                  logger_handle: str,
                  inst_name: str):
 
         if not isinstance(parent_register, RegAsyncReadWrite):
             raise TypeError(f'size_props must be of {type(RegAsyncReadWrite)} '
```

### Comparing `peakrdl-python-0.7.3/src/peakrdl_python/lib/register.py` & `peakrdl-python-0.7.4/src/peakrdl_python/lib/async_register.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,423 +1,97 @@
 """
-This module is intended to distributed as part of automatically generated code by the PeakRDL
-Python tool. It provides a set of classes used by the autogenerated code to represent register
+peakrdl-python is a tool to generate Python Register Access Layer (RAL) from SystemRDL
+Copyright (C) 2021 - 2023
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+This module is intended to distributed as part of automatically generated code by the
+peakrdl-python tool. It provides a set of classes used by the autogenerated code to represent
+registers
 """
 from enum import Enum
-from typing import List, Union, Iterator, TYPE_CHECKING, Tuple, cast, Optional, Dict
-from typing import AsyncGenerator, Generator
+from typing import List, Union, Iterator, TYPE_CHECKING, Tuple, cast, Optional, Dict, TypeVar
+from typing import AsyncGenerator
 from abc import ABC, abstractmethod
-from contextlib import asynccontextmanager, contextmanager
+from contextlib import asynccontextmanager
 from array import array as Array
+import sys
 
-from .base import Node, AddressMap, RegFile, NodeArray, get_array_typecode
-from .memory import Memory
-from .callbacks import CallbackSet, NormalCallbackSet, AsyncCallbackSet
+from .utility_functions import get_array_typecode
+from .base import AsyncAddressMap, AsyncRegFile
+from .register import BaseReg, BaseRegArray, RegisterWriteVerifyError
+from .memory import  MemoryAsyncReadOnly, MemoryAsyncWriteOnly, MemoryAsyncReadWrite, \
+    AsyncMemory, ReadableAsyncMemory, WritableAsyncMemory
+from .callbacks import AsyncCallbackSet
+
+# pylint: disable=duplicate-code
+if sys.version_info >= (3, 11):
+    from typing import Self
+else:
+    from typing_extensions import Self
+# pylint: enable=duplicate-code
 
 if TYPE_CHECKING:
-    from .fields import FieldReadOnly, FieldWriteOnly, FieldReadWrite
-    from .fields import FieldAsyncReadOnly, FieldAsyncWriteOnly, FieldAsyncReadWrite
-
-# pylint: disable=redefined-slots-in-subclass
-
-
-class RegisterWriteVerifyError(Exception):
-    """
-    Exception that occurs when the read after a write does not match the expected value
-    """
-
-
-class Reg(Node, ABC):
-    """
-    base class of register wrappers
-
-    Note:
-        It is not expected that this class will be instantiated under normal
-        circumstances however, it is useful for type checking
-    """
-
-    __slots__: List[str] = ['__width', '__accesswidth']
-
-    # pylint: disable=too-many-arguments,duplicate-code
-    def __init__(self,
-                 callbacks: CallbackSet,
-                 address: int,
-                 width: int,
-                 accesswidth: int,
-                 logger_handle: str,
-                 inst_name: str,
-                 parent: Union[AddressMap, RegFile, Memory]):
-
-        super().__init__(callbacks=callbacks,
-                         address=address,
-                         logger_handle=logger_handle,
-                         inst_name=inst_name,
-                         parent=parent)
-
-        self.__width = width
-        self.__accesswidth = accesswidth
-    # pylint: enable=too-many-arguments,duplicate-code
-
-    @property
-    def max_value(self) -> int:
-        """maximum unsigned integer value that can be stored in the register
 
-        For example:
-
-        * 8-bit register returns 0xFF (255)
-        * 16-bit register returns 0xFFFF (65535)
-        * 32-bit register returns 0xFFFF_FFFF (4294967295)
-
-        """
-        return (2 ** self.width) - 1
-
-    @property
-    def width(self) -> int:
-        """
-        The width of the register in bits, this uses the `regwidth` systemRDL property
-
-        Returns: register width
-
-        """
-        return self.__width
-
-    @property
-    def accesswidth(self) -> int:
-        """
-        The access width of the register in bits, this uses the `accesswidth` systemRDL property
-
-        Returns: register access width
-        """
-        return self.__accesswidth
-
-
-class RegReadOnly(Reg, ABC):
-    """
-    class for a read only register
+    from .fields import FieldAsyncReadOnly, FieldAsyncWriteOnly, FieldAsyncReadWrite
 
-    Args:
-        callbacks: set of callback to be used for accessing the hardware or simulator
-        address: address of the register
-        width: width of the register in bits
-        accesswidth: minimum access width of the register in bits
-        logger_handle: name to be used logging messages associate with this
-            object
+# pylint: disable=redefined-slots-in-subclass,too-many-lines
 
+class AsyncReg(BaseReg, ABC):
     """
+        base class of async register wrappers
 
-    __slots__: List[str] = ['__in_context_manager', '__register_state']
-
-    # pylint: disable=too-many-arguments, duplicate-code
-    def __init__(self,
-                 callbacks: NormalCallbackSet,
-                 address: int,
-                 width: int,
-                 accesswidth: int,
-                 logger_handle: str,
-                 inst_name: str,
-                 parent: Union[AddressMap, RegFile, Memory]):
-
-        if not isinstance(callbacks, NormalCallbackSet):
-            raise TypeError(f'callback set type is wrong, got {type(callbacks)}')
-
-        super().__init__(callbacks=callbacks,
-                         address=address,
-                         logger_handle=logger_handle,
-                         inst_name=inst_name,
-                         parent=parent, width=width, accesswidth=accesswidth)
-
-        self.__in_context_manager: bool = False
-        self.__register_state: int = 0
-
-    # pylint: enable=too-many-arguments, duplicate-code
-
-    @property
-    def _callbacks(self) -> NormalCallbackSet:
-        # This cast is OK because the type was checked in the __init__
-        return cast(NormalCallbackSet, super()._callbacks)
-
-    @contextmanager
-    def single_read(self) -> Generator['RegReadOnly', None, None]:
-        """
-        Context manager to allow multiple field accesses to be performed with a single
-        read of the register
-
-        Returns:
-
-        """
-        self.__register_state = self.read()
-        self.__in_context_manager = True
-        yield self
-        self.__in_context_manager = False
-
-    def read(self) -> int:
-        """Read value from the register
-
-        Returns:
-            The value from register
-
-        """
-        if self.__in_context_manager:
-            return self.__register_state
-
-        read_block_callback = self._callbacks.read_block_callback
-        read_callback = self._callbacks.read_callback
-
-        if read_callback is not None:
-            # python 3.7 doesn't have the callback defined as protocol so mypy doesn't recognise
-            # the arguments in the call back functions
-            return read_callback(addr=self.address,  # type: ignore[call-arg]
-                                 width=self.width,  # type: ignore[call-arg]
-                                 accesswidth=self.accesswidth)  # type: ignore[call-arg]
-
-        if read_block_callback is not None:
-            # python 3.7 doesn't have the callback defined as protocol so mypy doesn't recognise
-            # the arguments in the call back functions
-            return read_block_callback(addr=self.address,  # type: ignore[call-arg]
-                                       width=self.width,  # type: ignore[call-arg]
-                                       accesswidth=self.accesswidth,  # type: ignore[call-arg]
-                                       length=1)[0]  # type: ignore[call-arg]
-
-        raise RuntimeError('This function does not have a useable callback')
-
-    @property
-    @abstractmethod
-    def readable_fields(self) -> Iterator[Union['FieldReadOnly', 'FieldReadWrite']]:
-        """
-        generator that produces has all the readable fields within the register
-        """
-
-    def read_fields(self) -> Dict['str', Union[bool, Enum, int]]:
+        Note:
+            It is not expected that this class will be instantiated under normal
+            circumstances however, it is useful for type checking
         """
-        read the register and return a dictionary of the field values
-        """
-        return_dict: Dict['str', Union[bool, Enum, int]] = {}
-        with self.single_read() as reg:
-            for field in reg.readable_fields:
-                return_dict[field.inst_name] = field.read()
-
-        return return_dict
-
-
-class RegWriteOnly(Reg, ABC):
-    """
-    class for a write only register
-    """
 
     __slots__: List[str] = []
 
-    # pylint: disable=too-many-arguments, duplicate-code
-    def __init__(self,
-                 callbacks: NormalCallbackSet,
+    # pylint: disable=too-many-arguments,duplicate-code
+    def __init__(self, *,
                  address: int,
                  width: int,
                  accesswidth: int,
                  logger_handle: str,
                  inst_name: str,
-                 parent: Union[AddressMap, RegFile, Memory]):
+                 parent: Union[AsyncAddressMap, AsyncRegFile, AsyncMemory, 'AsyncRegArray']):
 
-        if not isinstance(callbacks, NormalCallbackSet):
-            raise TypeError(f'callback set type is wrong, got {type(callbacks)}')
+        if not isinstance(parent, (AsyncAddressMap, AsyncRegFile,
+                                   MemoryAsyncReadOnly, MemoryAsyncWriteOnly,
+                                   MemoryAsyncReadWrite, AsyncRegArray)):
+            raise TypeError(f'bad parent type got: {type(parent)}')
 
-        super().__init__(callbacks=callbacks,
-                         address=address,
-                         logger_handle=logger_handle,
-                         inst_name=inst_name,
-                         parent=parent, width=width, accesswidth=accesswidth)
+        if not isinstance(parent._callbacks, AsyncCallbackSet):
+            raise TypeError(f'callback set type is wrong, got {type(parent._callbacks)}')
 
-    # pylint: enable=too-many-arguments, duplicate-code
+        super().__init__(address=address, width=width, accesswidth=accesswidth,
+                         logger_handle=logger_handle, inst_name=inst_name, parent=parent)
 
     @property
-    def _callbacks(self) -> NormalCallbackSet:
+    def _callbacks(self) -> AsyncCallbackSet:
+        if self.parent is None:
+            raise RuntimeError('Parent must be set')
         # This cast is OK because the type was checked in the __init__
-        return cast(NormalCallbackSet, super()._callbacks)
-
-    def write(self, data: int) -> None:
-        """Writes a value to the register
-
-        Args:
-            data: data to be written
-
-        Raises:
-            ValueError: if the value provided is outside the range of the
-                permissible values for the register
-            TypeError: if the type of data is wrong
-        """
-        if not isinstance(data, int):
-            raise TypeError(f'data should be an int got {type(data)}')
-
-        if data > self.max_value:
-            raise ValueError('data out of range')
-
-        if data < 0:
-            raise ValueError('data out of range')
-
-        self._logger.info('Writing data:%X to %X', data, self.address)
-
-        block_callback = self._callbacks.write_block_callback
-        single_callback = self._callbacks.write_callback
-
-        if single_callback is not None:
-            # python 3.7 doesn't have the callback defined as protocol so mypy doesn't recognise
-            # the arguments in the call back functions
-            single_callback(addr=self.address,  # type: ignore[call-arg]
-                            width=self.width,  # type: ignore[call-arg]
-                            accesswidth=self.accesswidth,  # type: ignore[call-arg]
-                            data=data)  # type: ignore[call-arg]
-
-        elif block_callback is not None:
-            # python 3.7 doesn't have the callback defined as protocol so mypy doesn't recognise
-            # the arguments in the call back functions
-            data_as_array = Array(get_array_typecode(self.width), [data])
-            block_callback(addr=self.address,  # type: ignore[call-arg]
-                           width=self.width,  # type: ignore[call-arg]
-                           accesswidth=self.accesswidth,  # type: ignore[call-arg]
-                           data=data_as_array)  # type: ignore[call-arg]
-
-        else:
-            raise RuntimeError('This function does not have a useable callback')
-
-    @property
-    @abstractmethod
-    def writable_fields(self) -> Iterator[Union['FieldWriteOnly', 'FieldReadWrite']]:
-        """
-        generator that produces has all the readable fields within the register
-        """
-
-    @abstractmethod
-    def write_fields(self, **kwargs) -> None:  # type: ignore[no-untyped-def]
-        """
-        Do a write to the register, updating any field included in
-        the arguments
-        """
-
-
-class RegReadWrite(RegReadOnly, RegWriteOnly, ABC):
-    """
-    class for a read and write only register
-
-    """
-    __slots__: List[str] = ['__in_context_manager', '__register_state']
-
-    # pylint: disable=too-many-arguments, duplicate-code
-    def __init__(self,
-                 callbacks: NormalCallbackSet,
-                 address: int,
-                 width: int,
-                 accesswidth: int,
-                 logger_handle: str,
-                 inst_name: str,
-                 parent: Union[AddressMap, RegFile, Memory]):
-
-        super().__init__(callbacks=callbacks,
-                         address=address,
-                         logger_handle=logger_handle,
-                         inst_name=inst_name,
-                         parent=parent, width=width, accesswidth=accesswidth)
-
-        self.__in_context_manager: bool = False
-        self.__register_state: Optional[int] = None
-
-    # pylint: enable=too-many-arguments, duplicate-code
-
-    @contextmanager
-    def single_read_modify_write(self, verify: bool = False, skip_write: bool = False) -> \
-            Generator['RegReadWrite', None, None]:
-        """
-        Context manager to allow multiple field reads/write to be done with a single set of
-        field operations
-
-        Args:
-            verify (bool): very the write with a read afterwards
-            skip_write (bool): skip the write back at the end
-
-        Returns:
-
-        """
-        self.__register_state = self.read()
-        self.__in_context_manager = True
-        yield self
-        self.__in_context_manager = False
-        if not skip_write:
-            self.write(self.__register_state, verify)
-
-        # clear the register states at the end of the context manager
-        self.__register_state = None
-
-    def write(self, data: int, verify: bool = False) -> None:  # pylint: disable=arguments-differ
-        """
-        Writes a value to the register
-
-        Args:
-            data: data to be written
-            verify: set to True to read back the register to verify the read has occurred correctly
-
-        Raises:
-            ValueError: if the value provided is outside the range of the
-                        permissible values for the register
-            TypeError: if the type of data is wrong
-            RegisterWriteVerifyError: the read back data after the write does not match the
-                                      expected value
-        """
-        if self.__in_context_manager:
-            if self.__register_state is None:
-                raise RuntimeError('The internal register state should never be None in the '
-                                   'context manager')
-            self.__register_state = data
-        else:
-            super().write(data)
-            if verify:
-                read_back = self.read()
-                if read_back != data:
-                    raise RegisterWriteVerifyError(f'Readback {read_back:X} '
-                                                   f'after writing {data:X}')
-
-    def read(self) -> int:
-        """Read value from the register
-
-        Returns:
-            The value from register
-        """
-        if self.__in_context_manager:
-            if self.__register_state is None:
-                raise RuntimeError('The internal register state should never be None in the '
-                                   'context manager')
-            return self.__register_state
-
-        return super().read()
+        # pylint: disable-next=protected-access
+        return cast(AsyncCallbackSet, self.parent._callbacks)
 
-    def write_fields(self, **kwargs) -> None:  # type: ignore[no-untyped-def]
-        """
-        Do a read-modify-write to the register, updating any field included in
-        the arguments
-        """
-        if len(kwargs) == 0:
-            raise ValueError('no command args')
 
-        with self.single_read_modify_write() as reg:
-            for field_name, field_value in kwargs.items():
-                if field_name not in reg.systemrdl_python_child_name_map.values():
-                    raise ValueError(f'{field_name} is not a member of the register')
-
-                field = getattr(reg, field_name)
-                field.write(field_value)
-
-    def read_fields(self) -> Dict['str', Union[bool, Enum, int]]:
-        """
-        read the register and return a dictionary of the field values
-        """
-        return_dict: Dict['str', Union[bool, Enum, int]] = {}
-        with self.single_read_modify_write(skip_write=True) as reg:
-            for field in reg.readable_fields:
-                return_dict[field.inst_name] = field.read()
-
-        return return_dict
-
-
-class RegAsyncReadOnly(Reg, ABC):
+class RegAsyncReadOnly(AsyncReg, ABC):
     """
     class for an async read only register
 
     Args:
         callbacks: set of callback to be used for accessing the hardware or simulator
         address: address of the register
         width: width of the register in bits
@@ -426,44 +100,34 @@
             object
 
     """
 
     __slots__: List[str] = ['__in_context_manager', '__register_state']
 
     # pylint: disable=too-many-arguments, duplicate-code
-    def __init__(self,
-                 callbacks: AsyncCallbackSet,
+    def __init__(self, *,
                  address: int,
                  width: int,
                  accesswidth: int,
                  logger_handle: str,
                  inst_name: str,
-                 parent: Union[AddressMap, RegFile, Memory]):
+                 parent: Union[AsyncAddressMap, AsyncRegFile, ReadableAsyncMemory]):
 
-        if not isinstance(callbacks, AsyncCallbackSet):
-            raise TypeError(f'callback set type is wrong, got {type(callbacks)}')
 
-        super().__init__(callbacks=callbacks,
-                         address=address,
+        super().__init__(address=address,
                          logger_handle=logger_handle,
                          inst_name=inst_name,
                          parent=parent, width=width, accesswidth=accesswidth)
 
         self.__in_context_manager: bool = False
         self.__register_state: int = 0
-
-    @property
-    def _callbacks(self) -> AsyncCallbackSet:
-        # This cast is OK because the type was checked in the __init__
-        return cast(AsyncCallbackSet, super()._callbacks)
-
     # pylint: enable=too-many-arguments, duplicate-code
 
     @asynccontextmanager
-    async def single_read(self) -> AsyncGenerator['RegAsyncReadOnly', None]:
+    async def single_read(self) -> AsyncGenerator[Self, None]:
         """
         Context manager to allow multiple field accesses to be performed with a single
         read of the register
 
         Returns:
 
         """
@@ -475,19 +139,21 @@
     async def read(self) -> int:
         """Asynchronously read value from the register
 
         Returns:
             The value from register
 
         """
+        # pylint: disable=duplicate-code
         if self.__in_context_manager:
             return self.__register_state
 
         read_block_callback = self._callbacks.read_block_callback
         read_callback = self._callbacks.read_callback
+        # pylint: enable=duplicate-code
 
         if read_callback is not None:
             # python 3.7 doesn't have the callback defined as protocol so mypy doesn't recognise
             # the arguments in the call back functions
             return await read_callback(addr=self.address,  # type: ignore[call-arg]
                                        width=self.width,  # type: ignore[call-arg]
                                        accesswidth=self.accesswidth)  # type: ignore[call-arg]
@@ -518,91 +184,88 @@
         return_dict: Dict['str', Union[bool, Enum, int]] = {}
         async with self.single_read() as reg:
             for field in reg.readable_fields:
                 return_dict[field.inst_name] = await field.read()
 
         return return_dict
 
+    @property
+    def _is_readable(self) -> bool:
+        return True
+
+    @property
+    def _is_writeable(self) -> bool:
+        return False
+
 
-class RegAsyncWriteOnly(Reg, ABC):
+class RegAsyncWriteOnly(AsyncReg, ABC):
     """
     class for an asynchronous write only register
     """
 
     __slots__: List[str] = []
 
-    # pylint: disable=too-many-arguments, duplicate-code
-    def __init__(self,
-                 callbacks: AsyncCallbackSet,
+    # pylint: disable=too-many-arguments, duplicate-code, useless-parent-delegation
+    def __init__(self, *,
                  address: int,
                  width: int,
                  accesswidth: int,
                  logger_handle: str,
                  inst_name: str,
-                 parent: Union[AddressMap, RegFile, Memory]):
+                 parent: Union[AsyncAddressMap, AsyncRegFile, WritableAsyncMemory]):
 
-        if not isinstance(callbacks, AsyncCallbackSet):
-            raise TypeError(f'callback set type is wrong, got {type(callbacks)}')
 
-        super().__init__(callbacks=callbacks,
-                         address=address,
+        super().__init__(address=address,
                          logger_handle=logger_handle,
                          inst_name=inst_name,
                          parent=parent, width=width, accesswidth=accesswidth)
-
-    @property
-    def _callbacks(self) -> AsyncCallbackSet:
-        # This cast is OK because the type was checked in the __init__
-        return cast(AsyncCallbackSet, super()._callbacks)
-
     # pylint: enable=too-many-arguments, duplicate-code
 
     async def write(self, data: int) -> None:
         """Asynchronously writes a value to the register
 
         Args:
             data: data to be written
 
         Raises:
             ValueError: if the value provided is outside the range of the
                 permissible values for the register
             TypeError: if the type of data is wrong
         """
-        if not isinstance(data, int):
-            raise TypeError(f'data should be an int got {type(data)}')
 
-        if data > self.max_value:
-            raise ValueError('data out of range')
-
-        if data < 0:
-            raise ValueError('data out of range')
+        # this method check the types and range checks the data
+        self._validate_data(data=data)
 
+        # pylint: disable=duplicate-code
         self._logger.info('Writing data:%X to %X', data, self.address)
 
         block_callback = self._callbacks.write_block_callback
         single_callback = self._callbacks.write_callback
+        # pylint: enable=duplicate-code
 
         if single_callback is not None:
             # python 3.7 doesn't have the callback defined as protocol so mypy doesn't recognise
             # the arguments in the call back functions
             await single_callback(addr=self.address,  # type: ignore[call-arg]
                                   width=self.width,  # type: ignore[call-arg]
                                   accesswidth=self.accesswidth,  # type: ignore[call-arg]
                                   data=data)  # type: ignore[call-arg]
 
         elif block_callback is not None:
             # python 3.7 doesn't have the callback defined as protocol so mypy doesn't recognise
             # the arguments in the call back functions
+            # pylint: disable-next=duplicate-code
             data_as_array = Array(get_array_typecode(self.width), [data])
             await block_callback(addr=self.address,  # type: ignore[call-arg]
                                  width=self.width,  # type: ignore[call-arg]
                                  accesswidth=self.accesswidth,  # type: ignore[call-arg]
                                  data=data_as_array)  # type: ignore[call-arg]
 
         else:
+            # pylint: disable-next=duplicate-code
             raise RuntimeError('This function does not have a useable callback')
 
     @property
     @abstractmethod
     def writable_fields(self) -> Iterator[Union['FieldAsyncWriteOnly', 'FieldAsyncReadWrite']]:
         """
         generator that produces has all the writable fields within the register
@@ -611,46 +274,52 @@
     @abstractmethod
     async def write_fields(self, **kwargs) -> None:  # type: ignore[no-untyped-def]
         """
         Do an async write to the register, updating any field included in
         the arguments
         """
 
+    @property
+    def _is_readable(self) -> bool:
+        return False
+
+    @property
+    def _is_writeable(self) -> bool:
+        return True
+
 
 class RegAsyncReadWrite(RegAsyncReadOnly, RegAsyncWriteOnly, ABC):
     """
     class for an async read and write only register
 
     """
     __slots__: List[str] = ['__in_context_manager', '__register_state']
 
     # pylint: disable=too-many-arguments, duplicate-code
-    def __init__(self,
-                 callbacks: AsyncCallbackSet,
+    def __init__(self, *,
                  address: int,
                  width: int,
                  accesswidth: int,
                  logger_handle: str,
                  inst_name: str,
-                 parent: Union[AddressMap, RegFile, Memory]):
+                 parent: Union[AsyncAddressMap, AsyncRegFile, MemoryAsyncReadWrite]):
 
-        super().__init__(callbacks=callbacks,
-                         address=address,
+        super().__init__(address=address,
                          logger_handle=logger_handle,
                          inst_name=inst_name,
                          parent=parent, width=width, accesswidth=accesswidth)
 
         self.__in_context_manager: bool = False
         self.__register_state: Optional[int] = None
 
     # pylint: enable=too-many-arguments, duplicate-code
 
     @asynccontextmanager
     async def single_read_modify_write(self, verify: bool = False, skip_write: bool = False) -> \
-        AsyncGenerator['RegAsyncReadWrite', None]:
+        AsyncGenerator[Self, None]:
         """
         Context manager to allow multiple field reads/write to be done with a single set of
         field operations
 
         Args:
             verify (bool): very the write with a read afterwards
             skip_write (bool): skip the write back at the end
@@ -680,14 +349,15 @@
             ValueError: if the value provided is outside the range of the
                         permissible values for the register
             TypeError: if the type of data is wrong
             RegisterWriteVerifyError: the read back data after the write does not match the
                                       expected value
         """
         if self.__in_context_manager:
+            # pylint: disable=duplicate-code
             if self.__register_state is None:
                 raise RuntimeError('The internal register state should never be None in the '
                                    'context manager')
             self.__register_state = data
         else:
             await super().write(data)
             if verify:
@@ -699,14 +369,15 @@
     async def read(self) -> int:
         """Asynchronously read value from the register
 
         Returns:
             The value from register
         """
         if self.__in_context_manager:
+            # pylint: disable=duplicate-code
             if self.__register_state is None:
                 raise RuntimeError('The internal register state should never be None in the '
                                    'context manager')
             return self.__register_state
 
         return await super().read()
 
@@ -733,144 +404,432 @@
             for field_name, field_value in kwargs.items():
                 if field_name not in reg.systemrdl_python_child_name_map.values():
                     raise ValueError(f'{field_name} is not a member of the register')
 
                 field = getattr(reg, field_name)
                 await field.write(field_value)
 
+    @property
+    def _is_readable(self) -> bool:
+        return True
+
+    @property
+    def _is_writeable(self) -> bool:
+        return True
+
 
-ReadableRegister = Union[RegReadOnly, RegReadWrite]
-WritableRegister = Union[RegWriteOnly, RegReadWrite]
 ReadableAsyncRegister = Union[RegAsyncReadOnly, RegAsyncReadWrite]
 WritableAsyncRegister = Union[RegAsyncWriteOnly, RegAsyncReadWrite]
 
 
-class RegReadOnlyArray(NodeArray, ABC):
-    """
-    base class for a array of read only registers
+# pylint: disable-next=invalid-name
+AsyncRegArrayElementType= TypeVar('AsyncRegArrayElementType', bound=AsyncReg)
+
+
+class AsyncRegArray(BaseRegArray, ABC):
     """
-    __slots__: List[str] = []
+    base class of register array wrappers
 
+    Note:
+        It is not expected that this class will be instantiated under normal
+        circumstances however, it is useful for type checking
+    """
     # pylint: disable=too-many-arguments,duplicate-code
-    def __init__(self, logger_handle: str, inst_name: str,
-                 parent: Union[RegFile, AddressMap, Memory],
-                 callbacks: NormalCallbackSet,
+
+    __slots__: List[str] = ['__in_context_manager', '__register_array_cache',
+                            '__register_address_array']
+
+    def __init__(self, *,
+                 logger_handle: str, inst_name: str,
+                 parent: Union[AsyncAddressMap, AsyncRegFile, AsyncMemory],
+                 width: int,
+                 accesswidth: int,
                  address: int,
                  stride: int,
                  dimensions: Tuple[int, ...],
-                 elements: Optional[Dict[Tuple[int, ...], RegReadOnly]] = None):
+                 elements: Optional[Dict[Tuple[int, ...], AsyncRegArrayElementType]] = None):
+
+        self.__in_context_manager: bool = False
+        self.__register_array_cache: Optional[Array] = None
+        self.__register_address_array: Optional[List[int]] = None
+
+        if not isinstance(parent._callbacks, AsyncCallbackSet):
+            raise TypeError(f'callback set type is wrong, got {type(parent._callbacks)}')
 
         super().__init__(logger_handle=logger_handle, inst_name=inst_name,
-                         parent=parent, callbacks=callbacks, address=address,
+                         parent=parent, address=address, width=width, accesswidth=accesswidth,
                          stride=stride, dimensions=dimensions, elements=elements)
-    # pylint: enable=too-many-arguments,duplicate-code
 
+    @property
+    def __empty_array_cache(self) -> Array:
+        empty_array = [0 for _ in range(self.__number_cache_entries)]
+        return Array(get_array_typecode(self.width), empty_array)
 
-class RegWriteOnlyArray(NodeArray, ABC):
-    """
-    base class for a array of write only registers
-    """
-    __slots__: List[str] = []
+    async def __block_read(self) -> Array:
+        """
+        Read all the contents of the array in the most optimal way, ideally with a block operation
+        """
+        read_block_callback = self._callbacks.read_block_callback
+        read_callback = self._callbacks.read_callback
 
-    # pylint: disable=too-many-arguments,duplicate-code
-    def __init__(self, logger_handle: str, inst_name: str,
-                 parent: Union[RegFile, AddressMap, Memory],
-                 callbacks: NormalCallbackSet,
-                 address: int,
-                 stride: int,
-                 dimensions: Tuple[int, ...],
-                 elements: Optional[Dict[Tuple[int, ...], RegWriteOnly]] = None):
+        if read_block_callback is not None:
+            # python 3.7 doesn't have the callback defined as protocol so mypy doesn't recognise
+            # the arguments in the call back functions
+            data_read = \
+                await read_block_callback(  # type: ignore[call-arg]
+                    addr=self.address,  # type: ignore[call-arg]
+                    width=self.width,  # type: ignore[call-arg]
+                    accesswidth=self.accesswidth,  # type: ignore[call-arg]
+                    length=self.__number_cache_entries)  # type: ignore[call-arg]
 
-        super().__init__(logger_handle=logger_handle, inst_name=inst_name,
-                         parent=parent, callbacks=callbacks, address=address,
-                         stride=stride, dimensions=dimensions, elements=elements)
-    # pylint: enable=too-many-arguments,duplicate-code
+            if not isinstance(data_read, Array):
+                raise TypeError('The read block callback is expected to return an array')
 
+            return data_read
 
-class RegReadWriteArray(NodeArray, ABC):
-    """
-    base class for a array of read and write registers
-    """
-    __slots__: List[str] = []
+        if read_callback is not None:
+            # there is not read_block_callback defined so we must used individual read
+            data_array = self.__empty_array_cache
 
-    # pylint: disable=too-many-arguments,duplicate-code
-    def __init__(self, logger_handle: str, inst_name: str,
-                 parent: Union[RegFile, AddressMap, Memory],
-                 callbacks: NormalCallbackSet,
-                 address: int,
-                 stride: int,
-                 dimensions: Tuple[int, ...],
-                 elements: Optional[Dict[Tuple[int, ...], RegReadWrite]] = None):
+            if self.__register_address_array is None:
+                raise RuntimeError('This address array has not be initialised')
 
-        super().__init__(logger_handle=logger_handle, inst_name=inst_name,
-                         parent=parent, callbacks=callbacks, address=address,
-                         stride=stride, dimensions=dimensions, elements=elements)
-    # pylint: enable=too-many-arguments,duplicate-code
+            for entry, address in enumerate(self.__register_address_array):
+                # python 3.7 doesn't have the callback defined as protocol so mypy doesn't
+                # recognise the arguments in the call back functions
+                data_entry = await read_callback(  # type: ignore[call-arg]
+                    addr=address,  # type: ignore[call-arg]
+                    width=self.width,  # type: ignore[call-arg]
+                    accesswidth=self.accesswidth)  # type: ignore[call-arg]
+
+                data_array[entry] = data_entry
+
+            return data_array
+
+        raise RuntimeError('There is no usable callback')
+
+    async def __block_write(self, data: Array, verify: bool) -> None:
+        """
+        Write all the contents of the array in the most optimal way, ideally with a block operation
+        """
+        write_block_callback = self._callbacks.write_block_callback
+        write_callback = self._callbacks.write_callback
+
+        if write_block_callback is not None:
+            # python 3.7 doesn't have the callback defined as protocol so mypy doesn't recognise
+            # the arguments in the call back functions
+            await write_block_callback(addr=self.address,  # type: ignore[call-arg]
+                                       width=self.width,  # type: ignore[call-arg]
+                                       accesswidth=self.width,  # type: ignore[call-arg]
+                                       data=data)  # type: ignore[call-arg]
 
+        elif write_callback is not None:
+            # there is not write_block_callback defined so we must used individual write
 
-class RegAsyncReadOnlyArray(NodeArray, ABC):
+            if self.__register_address_array is None:
+                raise RuntimeError('This address array has not be initialised')
+
+            for entry_index, entry_data in enumerate(data):
+                entry_address = self.__register_address_array[entry_index]
+                # python 3.7 doesn't have the callback defined as protocol so mypy doesn't
+                # recognise the arguments in the call back functions
+                await write_callback(addr=entry_address,  # type: ignore[call-arg]
+                                     width=self.width,  # type: ignore[call-arg]
+                                     accesswidth=self.accesswidth,  # type: ignore[call-arg]
+                                     data=entry_data)  # type: ignore[call-arg]
+
+        else:
+            raise RuntimeError('No suitable callback')
+
+        if verify:
+            read_back_verify_data = self.__block_read()
+            if read_back_verify_data != data:
+                raise RegisterWriteVerifyError('Read back block miss-match')
+
+    def __cache_entry(self, addr: int, width: int, accesswidth: int) -> int:
+        """
+        Validate the data provided and determine the cache entry
+
+        Args:
+            addr: Address to write to
+            width: Width of the register in bits
+            accesswidth: Minimum access width of the register in bits
+
+        Returns: cache entry
+
+        """
+        if not isinstance(width, int):
+            raise TypeError(f'Width should be an int byt got {type(width)}')
+        if width != self.width:
+            raise ValueError('Requested Read width does not match the expected value')
+        if not isinstance(accesswidth, int):
+            raise TypeError(f'accesswidth should be an int byt got {type(accesswidth)}')
+        if accesswidth != self.accesswidth:
+            raise ValueError('Requested Read accesswidth does not match the expected value')
+        if not isinstance(addr, int):
+            raise TypeError(f'addr should be an int byt got {type(addr)}')
+        if not self.address <= addr < (self.address + self.size):
+            raise ValueError(f'Requested address 0x{addr:X} is out of range 0x{self.address:X} to '
+                             f'0x{self.address + self.size - (self.width >> 3):X}')
+        cache_entry = (addr - self.address) // (self.width >> 3)
+        if self.__register_address_array is None:
+            raise RuntimeError('The address table should always be populated here')
+        if self.__register_address_array[cache_entry] != addr:
+            raise RuntimeError(f'The calculated cache entry for address 0x{addr:X}')
+        return cache_entry
+
+    async def __cache_read(self, addr: int, width: int, accesswidth: int) -> int:
+        """
+        Used to replace the normal callbacks with those that access the cache
+
+        Args:
+            addr: Address to write to
+            width: Width of the register in bits
+            accesswidth: Minimum access width of the register in bits
+
+        Returns:
+            value inputted by the used
+        """
+        if self.__register_array_cache is None:
+            raise RuntimeError('The cache array should be initialised')
+        return self.__register_array_cache[self.__cache_entry(addr=addr,
+                                                              width=width,
+                                                              accesswidth=accesswidth)]
+
+    async def __cache_write(self, addr: int, width: int, accesswidth: int, data: int) -> None:
+        """
+        Used to replace the normal callbacks with those that access the cache
+
+        Args:
+            addr: Address to write to
+            width: Width of the register in bits
+            accesswidth: Minimum access width of the register in bits
+            data: value to be written to the register
+
+        Returns:
+            None
+        """
+        if not isinstance(data, int):
+            raise TypeError(f'Data should be an int byt got {type(data)}')
+        if self.__register_array_cache is None:
+            raise RuntimeError('The cache array should be initialised')
+        self.__register_array_cache[self.__cache_entry(addr=addr,
+                                                       width=width,
+                                                       accesswidth=accesswidth)] = data
+
+    @property
+    def __cache_callbacks(self) -> AsyncCallbackSet:
+        return AsyncCallbackSet(read_callback=self.__cache_read,
+                                 write_callback=self.__cache_write)
+
+    @property
+    def __number_cache_entries(self) -> int:
+        return self.size // (self.width >> 3)
+
+    @asynccontextmanager
+    async def _cached_access(self, verify: bool = False, skip_write: bool = False,
+                             skip_initial_read: bool = False) -> \
+            AsyncGenerator[Self, None]:
+        """
+        Context manager to allow multiple field reads/write to be done with a single set of
+        field operations
+
+        Args:
+            verify (bool): very the write with a read afterwards
+            skip_write (bool): skip the write back at the end
+
+        Returns:
+
+        """
+        self.__register_address_array = \
+            [self.address + (i * (self.width >> 3)) for i in range(self.__number_cache_entries)]
+        if skip_initial_read:
+            self.__register_array_cache = self.__empty_array_cache
+        else:
+            self.__register_array_cache = await self.__block_read()
+        self.__in_context_manager = True
+        yield self
+        self.__in_context_manager = False
+        if not skip_write:
+            await self.__block_write(self.__register_array_cache, verify)
+
+        # clear the register states at the end of the context manager
+        self.__register_address_array = None
+        self.__register_array_cache = None
+
+    @property
+    def _callbacks(self) -> AsyncCallbackSet:
+
+        if self.__in_context_manager:
+            return self.__cache_callbacks
+
+        if self.parent is None:
+            raise RuntimeError('Parent must be set')
+        # This cast is OK because the type was checked in the __init__
+        # pylint: disable-next=protected-access
+        return cast(AsyncCallbackSet, self.parent._callbacks)
+
+
+class RegAsyncReadOnlyArray(AsyncRegArray, ABC):
     """
     base class for a array of async read only registers
     """
     __slots__: List[str] = []
 
     # pylint: disable=too-many-arguments,duplicate-code
-    def __init__(self, logger_handle: str, inst_name: str,
-                 parent: Union[RegFile, AddressMap, Memory],
-                 callbacks: AsyncCallbackSet,
+    def __init__(self, *,
+                 logger_handle: str, inst_name: str,
+                 parent: Union[AsyncRegFile, AsyncAddressMap, ReadableAsyncMemory],
                  address: int,
+                 width: int,
+                 accesswidth: int,
                  stride: int,
                  dimensions: Tuple[int, ...],
                  elements: Optional[Dict[Tuple[int, ...], RegAsyncReadOnly]] = None):
 
+        if not isinstance(parent, (AsyncRegFile, AsyncAddressMap,
+                                   MemoryAsyncReadOnly, MemoryAsyncReadWrite)):
+            raise TypeError('parent should be either AsyncRegFile, AsyncAddressMap, '
+                            'MemoryAsyncReadOnly, MemoryAsyncReadWrite '
+                            f'got {type(parent)}')
+
         super().__init__(logger_handle=logger_handle, inst_name=inst_name,
-                         parent=parent, callbacks=callbacks, address=address,
+                         parent=parent, address=address, width=width, accesswidth=accesswidth,
                          stride=stride, dimensions=dimensions, elements=elements)
     # pylint: enable=too-many-arguments,duplicate-code
 
+    @asynccontextmanager
+    async def single_read(self) -> \
+            AsyncGenerator[Self, None]:
+        """
+        Context manager to allow multiple field reads/write to be done with a single set of
+        field operations
+
+        Args:
+
+
+        Returns:
+
+        """
+        async with self._cached_access(verify=False, skip_write=True,
+                                 skip_initial_read=False) as reg_array:
+            yield reg_array
+
+    @property
+    def _is_readable(self) -> bool:
+        return True
+
+    @property
+    def _is_writeable(self) -> bool:
+        return False
 
-class RegAsyncWriteOnlyArray(NodeArray, ABC):
+
+class RegAsyncWriteOnlyArray(AsyncRegArray, ABC):
     """
     base class for a array of async write only registers
     """
     __slots__: List[str] = []
 
     # pylint: disable=too-many-arguments,duplicate-code
-    def __init__(self, logger_handle: str, inst_name: str,
-                 parent: Union[RegFile, AddressMap, Memory],
-                 callbacks: AsyncCallbackSet,
+    def __init__(self, *,
+                 logger_handle: str, inst_name: str,
+                 parent: Union[AsyncRegFile, AsyncAddressMap, WritableAsyncMemory],
                  address: int,
+                 width: int,
+                 accesswidth: int,
                  stride: int,
                  dimensions: Tuple[int, ...],
-                 elements: Optional[Dict[Tuple[int, ...], RegAsyncReadOnly]] = None):
+                 elements: Optional[Dict[Tuple[int, ...], RegAsyncWriteOnly]] = None):
+
+        if not isinstance(parent, (AsyncRegFile, AsyncAddressMap,
+                                   MemoryAsyncWriteOnly, MemoryAsyncReadWrite)):
+            raise TypeError('parent should be either AsyncRegFile, AsyncAddressMap, '
+                            'MemoryAsyncWriteOnly, MemoryAsyncReadWrite '
+                            f'got {type(parent)}')
 
         super().__init__(logger_handle=logger_handle, inst_name=inst_name,
-                         parent=parent, callbacks=callbacks, address=address,
+                         parent=parent, address=address, width=width, accesswidth=accesswidth,
                          stride=stride, dimensions=dimensions, elements=elements)
     # pylint: enable=too-many-arguments,duplicate-code
 
+    @asynccontextmanager
+    async def single_write(self) -> \
+            AsyncGenerator[Self, None]:
+        """
+        Context manager to allow multiple field reads/write to be done with a single set of
+        field operations
+
+        Args:
+
+
+        Returns:
+
+        """
+        async with self._cached_access(verify=False, skip_write=False,
+                                 skip_initial_read=True) as reg_array:
+            yield reg_array
+
+    @property
+    def _is_readable(self) -> bool:
+        return False
+
+    @property
+    def _is_writeable(self) -> bool:
+        return True
+
 
-class RegAsyncReadWriteArray(NodeArray, ABC):
+class RegAsyncReadWriteArray(AsyncRegArray, ABC):
     """
     base class for a array of read and write registers
     """
     __slots__: List[str] = []
 
     # pylint: disable=too-many-arguments,duplicate-code
-    def __init__(self, logger_handle: str, inst_name: str,
-                 parent: Union[RegFile, AddressMap, Memory],
-                 callbacks: AsyncCallbackSet,
+    def __init__(self, *,
+                 logger_handle: str, inst_name: str,
+                 parent: Union[AsyncRegFile, AsyncAddressMap, MemoryAsyncReadWrite],
                  address: int,
+                 width: int,
+                 accesswidth: int,
                  stride: int,
                  dimensions: Tuple[int, ...],
-                 elements: Optional[Dict[Tuple[int, ...], RegAsyncReadOnly]] = None):
+                 elements: Optional[Dict[Tuple[int, ...], RegAsyncReadWrite]] = None):
+
+        if not isinstance(parent, (AsyncRegFile, AsyncAddressMap, MemoryAsyncReadWrite)):
+            raise TypeError('parent should be either AsyncRegFile, AsyncAddressMap, '
+                            'MemoryAsyncReadWrite '
+                            f'got {type(parent)}')
 
         super().__init__(logger_handle=logger_handle, inst_name=inst_name,
-                         parent=parent, callbacks=callbacks, address=address,
+                         parent=parent, address=address, width=width, accesswidth=accesswidth,
                          stride=stride, dimensions=dimensions, elements=elements)
     # pylint: enable=too-many-arguments,duplicate-code
 
+    @asynccontextmanager
+    async def single_read_modify_write(self, verify: bool = False, skip_write: bool = False) -> \
+            AsyncGenerator[Self, None]:
+        """
+        Context manager to allow multiple field reads/write to be done with a single set of
+        field operations
+
+        Args:
+            verify (bool): very the write with a read afterwards
+            skip_write (bool): skip the write back at the end
+
+        Returns:
+
+        """
+        async with self._cached_access(verify=verify, skip_write=skip_write,
+                                  skip_initial_read=False) as reg_array:
+            yield reg_array
+
+    @property
+    def _is_readable(self) -> bool:
+        return True
+
+    @property
+    def _is_writeable(self) -> bool:
+        return True
+
 
-ReadableRegisterArray = Union[RegReadOnlyArray, RegReadWriteArray]
-WritableRegisterArray = Union[RegWriteOnlyArray, RegReadWriteArray]
 ReadableAsyncRegisterArray = Union[RegAsyncReadOnlyArray, RegAsyncReadWriteArray]
-WritableAsyncRegisterArray = Union[RegAsyncWriteOnlyArray, RegAsyncReadWriteArray]
+WriteableAsyncRegisterArray = Union[RegAsyncWriteOnlyArray, RegAsyncReadWriteArray]
```

### Comparing `peakrdl-python-0.7.3/src/peakrdl_python/safe_name_utility.py` & `peakrdl-python-0.7.4/src/peakrdl_python/safe_name_utility.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,24 @@
 """
+peakrdl-python is a tool to generate Python Register Access Layer (RAL) from SystemRDL
+Copyright (C) 2021 - 2023
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
 utility functions for turning potentially unsafe names from the system RDL and making them safe
 """
 import keyword
 from typing import List, Union, Type, Callable, Dict
 from dataclasses import dataclass
 
 from systemrdl.node import RegNode  # type: ignore
```

### Comparing `peakrdl-python-0.7.3/src/peakrdl_python/systemrdl_node_utility_functions.py` & `peakrdl-python-0.7.4/src/peakrdl_python/systemrdl_node_utility_functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,24 @@
 """
+peakrdl-python is a tool to generate Python Register Access Layer (RAL) from SystemRDL
+Copyright (C) 2021 - 2023
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
 A set of utility functions that perform supplementary processing on a node in a compiled
 system RDL dataset.
 """
 from typing import Iterable, Optional, List
 
 import textwrap
```

### Comparing `peakrdl-python-0.7.3/src/peakrdl_python/templates/addrmap.py.jinja` & `peakrdl-python-0.7.4/src/peakrdl_python/templates/addrmap.py.jinja`

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,79 @@
+{#
+peakrdl-python is a tool to generate Python Register Access Layer (RAL) from SystemRDL
+Copyright (C) 2021 - 2023
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <https://www.gnu.org/licenses/>.
+#}
+
 {% include "header.py.jinja" with context %}
 {% if uses_enum %}from enum import EnumMeta, IntEnum, unique{% endif %}
 from typing import Tuple
 from typing import Iterator
 from typing import List
 from typing import Optional
 from typing import Union
-from typing import cast
 from typing import Dict
 from typing import Type
 {% if asyncoutput -%}
 from typing import AsyncGenerator
 {% else %}
 from typing import Generator
 {% endif %}
 import warnings
 
 
 from contextlib import {% if asyncoutput %}async{% endif %}contextmanager
 
 from ..lib import Node
-from ..lib import AddressMap, RegFile, Memory
+
 from ..lib  import AddressMapArray, RegFileArray
 {% if asyncoutput -%}
-    {% if uses_memory %}
+from ..lib import AsyncMemory, AsyncMemoryArray
+from ..lib import AsyncAddressMap
+from ..lib import AsyncRegFile
+from ..lib  import AsyncAddressMapArray
+from ..lib  import AsyncRegFileArray
 from ..lib import MemoryAsyncReadOnly, MemoryAsyncWriteOnly, MemoryAsyncReadWrite
 from ..lib import MemoryAsyncReadOnlyArray, MemoryAsyncWriteOnlyArray, MemoryAsyncReadWriteArray
-    {% endif %}
+from ..lib import AsyncReg, AsyncRegArray
 from ..lib import RegAsyncReadOnly, RegAsyncWriteOnly, RegAsyncReadWrite
 from ..lib import RegAsyncReadOnlyArray, RegAsyncWriteOnlyArray, RegAsyncReadWriteArray
 from ..lib import FieldAsyncReadOnly, FieldAsyncWriteOnly, FieldAsyncReadWrite, Field
 {% if uses_enum %}from ..lib import FieldEnumAsyncReadOnly, FieldEnumAsyncWriteOnly, FieldEnumAsyncReadWrite{% endif %}
 from ..lib import ReadableAsyncRegister, WritableAsyncRegister
-from ..lib import ReadableAsyncRegisterArray, WritableAsyncRegisterArray
+from ..lib import ReadableAsyncMemory, WritableAsyncMemory
+from ..lib import ReadableAsyncRegisterArray, WriteableAsyncRegisterArray
 {%- else -%}
-    {% if uses_memory %}
+from ..lib import Memory, MemoryArray
+from ..lib import AddressMap
+from ..lib import RegFile
+from ..lib  import AddressMapArray
+from ..lib  import RegFileArray
 from ..lib import MemoryReadOnly, MemoryWriteOnly, MemoryReadWrite
 from ..lib import MemoryReadOnlyArray, MemoryWriteOnlyArray, MemoryReadWriteArray
-    {% endif %}
+from ..lib import Reg, RegArray
 from ..lib import RegReadOnly, RegWriteOnly, RegReadWrite
 from ..lib import RegReadOnlyArray, RegWriteOnlyArray, RegReadWriteArray
 from ..lib import FieldReadOnly, FieldWriteOnly, FieldReadWrite, Field
 {% if uses_enum %}from ..lib import FieldEnumReadOnly, FieldEnumWriteOnly, FieldEnumReadWrite{% endif %}
 from ..lib import ReadableRegister, WritableRegister
-from ..lib import ReadableRegisterArray, WritableRegisterArray
+from ..lib import ReadableMemory, WritableMemory
+from ..lib import ReadableRegisterArray, WriteableRegisterArray
 {%- endif %}
 from ..lib import FieldSizeProps, FieldMiscProps
 
 {% if asyncoutput %}
 from ..lib import AsyncCallbackSet
 {% else %}
 from ..lib import NormalCallbackSet
@@ -64,81 +91,82 @@
         {{ register_class_attributes(node) }}
     {%- elif isinstance(node, systemrdlMemNode) %}
         {%- if node.is_array %}
     self.__{{node.inst_name}}:{{get_fully_qualified_type_name(node)}}_array_cls = {{get_fully_qualified_type_name(node)}}_array_cls(address=self.address+{{node.raw_address_offset}},
                                                                                   stride={{node.array_stride}},
                                                                                   dimensions=tuple({{node.array_dimensions}}),
                                                                                   logger_handle=logger_handle+'.{{node.inst_name}}',
-                                                                                  inst_name='{{node.inst_name}}', parent=self,
-                                                                                  callbacks=callbacks)
+                                                                                  inst_name='{{node.inst_name}}', parent=self)
         {%- else %}
             {%- if node.is_sw_readable and node.is_sw_writable %}
-    self.__{{node.inst_name}}:{{get_fully_qualified_type_name(node)}}_cls = {{get_fully_qualified_type_name(node)}}_cls(callbacks=callbacks,
+    self.__{{node.inst_name}}:{{get_fully_qualified_type_name(node)}}_cls = {{get_fully_qualified_type_name(node)}}_cls(
                                                                  address=self.address+{{node.address_offset}},
                                                                  logger_handle=logger_handle+'.{{node.inst_name}}',
                                                                                    inst_name='{{node.inst_name}}', parent=self)
             {%- elif node.is_sw_readable and not node.is_sw_writable %}
-    self.__{{node.inst_name}}:{{get_fully_qualified_type_name(node)}}_cls = {{get_fully_qualified_type_name(node)}}_cls(callbacks=callbacks,
+    self.__{{node.inst_name}}:{{get_fully_qualified_type_name(node)}}_cls = {{get_fully_qualified_type_name(node)}}_cls(
                                                                  address=self.address+{{node.address_offset}},
                                                                  logger_handle=logger_handle+'.{{node.inst_name}}',
                                                                                    inst_name='{{node.inst_name}}', parent=self)
             {%- elif not node.is_sw_readable and node.is_sw_writable %}
-    self.__{{node.inst_name}}:{{get_fully_qualified_type_name(node)}}_cls = {{get_fully_qualified_type_name(node)}}_cls(callbacks=callbacks,
+    self.__{{node.inst_name}}:{{get_fully_qualified_type_name(node)}}_cls = {{get_fully_qualified_type_name(node)}}_cls(
                                                                              address=self.address+{{node.address_offset}},
                                                                              logger_handle=logger_handle+'.{{node.inst_name}}',
                                                                              inst_name='{{node.inst_name}}', parent=self)
             {%- endif %}
         {%- endif %}
     {%- elif isinstance(node, systemrdlRegfileNode) or isinstance(node, systemrdlAddrmapNode) %}
         {%- if node.is_array %}
     self.__{{node.inst_name}}:{{get_fully_qualified_type_name(node)}}_array_cls = {{get_fully_qualified_type_name(node)}}_array_cls(address=self.address+{{node.raw_address_offset}},
                                                                                   stride={{node.array_stride}},
                                                                                   dimensions=tuple({{node.array_dimensions}}),
                                                                                   logger_handle=logger_handle+'.{{node.inst_name}}',
-                                                                                  inst_name='{{node.inst_name}}', parent=self,
-                                                                                  callbacks=callbacks)
+                                                                                  inst_name='{{node.inst_name}}', parent=self)
         {%- else -%}
-    self.__{{node.inst_name}}:{{get_fully_qualified_type_name(node)}}_cls = {{get_fully_qualified_type_name(node)}}_cls(callbacks=callbacks,
+    self.__{{node.inst_name}}:{{get_fully_qualified_type_name(node)}}_cls = {{get_fully_qualified_type_name(node)}}_cls(
                                                                             address=self.address+{{node.address_offset}},
                                                                             logger_handle=logger_handle+'.{{node.inst_name}}',
-                                                                            inst_name='{{node.inst_name}}', parent=self)
+                                                                            inst_name='{{node.inst_name}}',
+                                                                            parent=self)
         {%- endif %}
     {%- endif %}
 {%- endmacro %}
 
 {%- macro regfile_class(node) %}
-class {{get_fully_qualified_type_name(node)}}_cls(RegFile):
+class {{get_fully_qualified_type_name(node)}}_cls({% if asyncoutput %}Async{% endif %}RegFile):
     """
     Class to represent a register file in the register model
 
     {{get_table_block(node) | indent}}
     """
 
     __slots__ : List[str] = [{%- for child_node in node.children(unroll=False) -%}'__{{child_node.inst_name}}'{% if not loop.last %}, {% endif %}{%- endfor %}]
 
     {% if asyncoutput %}AsyncCallbackSet{% else %}NormalCallbackSet{% endif %}
 
     def __init__(self,
-                 callbacks: {% if asyncoutput %}AsyncCallbackSet{% else %}NormalCallbackSet{% endif %},
                  address: int,
                  logger_handle:str,
                  inst_name:str,
-                 parent:Union[AddressMap,RegFile]):
+                 parent:Union[{% if asyncoutput %}Async{% endif %}AddressMap,{% if asyncoutput %}Async{% endif %}RegFile]):
 
-        super().__init__(callbacks=callbacks,
-                         address=address,
+        super().__init__(address=address,
                          logger_handle=logger_handle,
                          inst_name=inst_name,
                          parent=parent)
 
         # instance of objects within the class
         {% for child_node in node.children(unroll=False) -%}
             {{ regfile_or_addr_instance(child_node) | indent }}
         {% endfor %}
 
+    @property
+    def size(self) -> int:
+        return {{node.size}}
+
     # properties for Register and RegisterFiles
     {%- for child_node in node.children(unroll=False) %}
         {%- if isinstance(child_node, systemrdlRegNode) or isinstance(child_node, systemrdlRegfileNode) %}
     @property
     {%- if isinstance(child_node, systemrdlRegNode) -%}
     {%- set property_name = safe_node_name(child_node) -%}
     {%- elif isinstance(child_node, systemrdlRegfileNode) -%}
@@ -176,67 +204,75 @@
             {% else %}
             {{ raise_template_error('unexpected type') }}
             {%- endif %}
             {%- endfor %}
             }
 
     {{ child_register_getter(node) }}
-    {{ child_getter(node, "get_sections",  "RegFile", systemrdlRegfileNode) }}
+
+        {% if asyncoutput %}
+    {{ child_getter(node, "get_sections", "AsyncRegFile, AsyncRegFileArray", systemrdlRegfileNode) }}
+    {% else %}
+    {{ child_getter(node, "get_sections", "RegFile, RegFileArray", systemrdlRegfileNode) }}
+    {% endif %}
 
      {%- if node.is_array %}
-class {{get_fully_qualified_type_name(node)}}_array_cls(RegFileArray):
+class {{get_fully_qualified_type_name(node)}}_array_cls({% if asyncoutput %}Async{% endif %}RegFileArray):
     """
     Class to represent a regfile array in the register model
     """
     __slots__: List[str] = []
 
     def __init__(self, logger_handle: str, inst_name: str,
-                 parent: Union[AddressMap, RegFile],
-                 callbacks: {% if asyncoutput %}AsyncCallbackSet{% else %}NormalCallbackSet{% endif %},
+                 parent: Union[{% if asyncoutput %}Async{% endif %}AddressMap, {% if asyncoutput %}Async{% endif %}RegFile],
                  address: int,
                  stride: int,
                  dimensions: Tuple[int, ...]):
 
         super().__init__(logger_handle=logger_handle, inst_name=inst_name,
-                         parent=parent, callbacks=callbacks, address=address,
+                         parent=parent, address=address,
                          stride=stride, dimensions=dimensions)
 
     @property
     def _element_datatype(self) -> Type[Node]:
         return {{get_fully_qualified_type_name(node)}}_cls
     {%- endif %}
 {%- endmacro %}
 
 {%- macro addrmap_class(node) %}
-class {{get_fully_qualified_type_name(node)}}_cls(AddressMap):
+class {{get_fully_qualified_type_name(node)}}_cls({% if asyncoutput %}Async{% endif %}AddressMap):
     """
     Class to represent a address map in the register model
 
     {{get_table_block(node) | indent}}
     """
 
     __slots__ : List[str] = [{%- for child_node in node.children(unroll=False) -%}{%- if isinstance(child_node, systemrdlRegNode) or isinstance(child_node, systemrdlRegfileNode) or isinstance(child_node, systemrdlAddrmapNode) or isinstance(child_node, systemrdlMemNode) -%}'__{{child_node.inst_name}}'{% if not loop.last %}, {% endif %}{% endif %}{%- endfor %}]
 
-    def __init__(self,
-                 callbacks: {% if asyncoutput %}AsyncCallbackSet{% else %}NormalCallbackSet{% endif %},
+    def __init__(self, *,
                  address:int {%- if node == top_node -%}={{top_node.absolute_address}}{%- endif -%},
                  logger_handle:str {%- if node == top_node -%}='reg_model.{{top_node.get_path()}}'{%- endif -%},
                  inst_name:str{%- if node == top_node -%}='{{node.inst_name}}'{%- endif -%},
-                 parent:Optional[AddressMap]=None):
+                 callbacks: Optional[{% if asyncoutput %}AsyncCallbackSet{% else %}NormalCallbackSet{% endif %}]=None,
+                 parent:Optional[{% if asyncoutput %}Async{% endif %}AddressMap]=None):
 
         super().__init__(callbacks=callbacks,
                          address=address,
                          logger_handle=logger_handle,
                          inst_name=inst_name,
                          parent=parent)
 
         {% for child_node in node.children(unroll=False) -%}
             {{ regfile_or_addr_instance(child_node) | indent }}
         {% endfor %}
 
+    @property
+    def size(self) -> int:
+        return {{node.size}}
+
         {%- for child_node in node.children(unroll=False) -%}
             {%- if isinstance(child_node, systemrdlRegNode) or isinstance(child_node, systemrdlRegfileNode) or isinstance(child_node, systemrdlAddrmapNode) or isinstance(child_node, systemrdlMemNode) %}
     @property
     {%- if isinstance(child_node, systemrdlRegNode) -%}
     {%- set property_name = safe_node_name(child_node) -%}
     {%- elif isinstance(child_node, systemrdlRegfileNode) -%}
     {%- set property_name = safe_node_name(child_node) -%}
@@ -281,43 +317,48 @@
             {% else %}
             {{ raise_template_error('unexpected type') }}
             {%- endif %}
             {%- endfor %}
             }
 
     {{ child_register_getter(node) }}
-    {{ child_getter(node, "get_memories",    "Memory",     systemrdlMemNode) }}
-    {{ child_getter(node, "get_sections", "Union[AddressMap, RegFile]", (systemrdlAddrmapNode, systemrdlRegfileNode)) }}
+    {% if asyncoutput %}
+    {{ child_getter(node, "get_sections", "AsyncAddressMap, AsyncRegFile, AsyncAddressMapArray, AsyncRegFileArray", (systemrdlAddrmapNode, systemrdlRegfileNode)) }}
+    {{ child_getter(node, "get_memories",    "AsyncMemory, AsyncMemoryArray",     systemrdlMemNode) }}
+    {% else %}
+    {{ child_getter(node, "get_sections", "AddressMap, RegFile, AddressMapArray, RegFileArray", (systemrdlAddrmapNode, systemrdlRegfileNode)) }}
+    {{ child_getter(node, "get_memories",    "Memory, MemoryArray",     systemrdlMemNode) }}
+
+    {% endif %}
 
     {%- if node.is_array %}
-class {{get_fully_qualified_type_name(node)}}_array_cls(AddressMapArray):
+class {{get_fully_qualified_type_name(node)}}_array_cls({% if asyncoutput %}Async{% endif %}AddressMapArray):
     """
     Class to represent a addrmap array in the register model
     """
     __slots__: List[str] = []
 
     def __init__(self, logger_handle: str, inst_name: str,
-                 parent: AddressMap,
-                 callbacks: {% if asyncoutput %}AsyncCallbackSet{% else %}NormalCallbackSet{% endif %},
+                 parent: {% if asyncoutput %}Async{% endif %}AddressMap,
                  address: int,
                  stride: int,
                  dimensions: Tuple[int, ...]):
 
         super().__init__(logger_handle=logger_handle, inst_name=inst_name,
-                         parent=parent, callbacks=callbacks, address=address,
+                         parent=parent, address=address,
                          stride=stride, dimensions=dimensions)
 
     @property
     def _element_datatype(self) -> Type[Node]:
         return {{get_fully_qualified_type_name(node)}}_cls
     {%- endif %}
 {%- endmacro %}
 
 {%- macro child_getter(node, getter_name, child_type, child_rdltype) %}
-    def {{getter_name}}(self, unroll:bool=False) -> Iterator[Union[{{child_type}},Tuple[{{child_type}},...]]]:
+    def {{getter_name}}(self, unroll:bool=False) -> Iterator[Union[{{child_type}}]]:
         """
         generator that produces all the {{child_type}} children of this node
         """
         {% for child_node in node.children(unroll=False) -%}
             {%- if isinstance(child_node, child_rdltype) %}
 
                 {%- if isinstance(child_node, systemrdlRegNode) -%}
@@ -332,19 +373,19 @@
                 {{ raise_template_error('unexpected type') }}
                 {%- endif %}
 
 
                 {% if child_node.is_array %}
         if unroll:
             for child in self.{{property_name}}:
-                yield cast({{child_type}}, child)
+                yield child
         else:
-            yield cast(Tuple[{{child_type}},...], self.{{property_name}})
+            yield self.{{property_name}}
                  {% else %}
-        yield cast({{child_type}}, self.{{property_name}})
+        yield self.{{property_name}}
                 {%- endif %}
             {%- endif -%}
         {% endfor %}
 
         # Empty generator in case there are no children of this type
         if False: yield
 {%- endmacro %}
```

### Comparing `peakrdl-python-0.7.3/src/peakrdl_python/templates/addrmap_register.py.jinja` & `peakrdl-python-0.7.4/src/peakrdl_python/templates/addrmap_register.py.jinja`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+{#
+peakrdl-python is a tool to generate Python Register Access Layer (RAL) from SystemRDL
+Copyright (C) 2021 - 2023
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <https://www.gnu.org/licenses/>.
+#}
 
 {%- macro register_class(node) %}
     {%- if node.has_sw_readable and node.has_sw_writable %}
 class {{get_fully_qualified_type_name(node)}}_cls(Reg{% if asyncoutput %}Async{% endif %}ReadWrite):
     {%- elif node.has_sw_readable and not node.has_sw_writable %}
 class {{get_fully_qualified_type_name(node)}}_cls(Reg{% if asyncoutput %}Async{% endif %}ReadOnly):
     {%- elif not node.has_sw_readable and node.has_sw_writable %}
@@ -12,24 +29,32 @@
 
     {{get_table_block(node) | indent}}
     """
 
     __slots__ : List[str] = [{%- for child_node in node.children(unroll=False) -%}'__{{child_node.inst_name}}'{% if not loop.last %}, {% endif %}{%- endfor %}]
 
     def __init__(self,
-                 callbacks: {% if asyncoutput %}AsyncCallbackSet{% else %}NormalCallbackSet{% endif %},
                  address: int,
+                 width: int,
+                 accesswidth: int,
                  logger_handle: str,
                  inst_name: str,
-                 parent: Union[AddressMap,RegFile,Memory]):
-
-        super().__init__(callbacks=callbacks,
-                         address=address,
-                         {% if 'accesswidth' in node.list_properties() -%}accesswidth={{node.get_property('accesswidth')}}{%- else -%}accesswidth={{node.size*8}}{%- endif -%},
-                         width={{node.size*8}},
+                 parent: Union[{% if asyncoutput -%}Async{%- endif -%}AddressMap,{%- if asyncoutput -%}Async{%- endif -%}RegFile,
+                 {%- if node.has_sw_readable and node.has_sw_writable -%}
+                    Memory{% if asyncoutput %}Async{% endif -%}ReadWrite
+                 {%- elif node.has_sw_readable and not node.has_sw_writable -%}
+                    Readable{% if asyncoutput %}Async{% endif -%}Memory
+                 {%- elif not node.has_sw_readable and node.has_sw_writable -%}
+                    Writable{% if asyncoutput %}Async{% endif -%}Memory
+                 {%- endif -%}
+                 ]):
+
+        super().__init__(address=address,
+                         width=width,
+                         accesswidth=accesswidth,
                          logger_handle=logger_handle,
                          inst_name=inst_name,
                          parent=parent)
 
         # build the field attributes
         {%- for child_node in node.fields() %}
             {%- if isinstance(child_node, systemrdlFieldNode) %}
@@ -54,35 +79,14 @@
     def readable_fields(self) -> Iterator[Union[Field{% if asyncoutput %}Async{% endif %}ReadOnly, Field{% if asyncoutput %}Async{% endif %}ReadWrite]]:
         """
         generator that produces has all the readable fields within the register
         """
         {% for child_node in get_reg_readable_fields(node) -%}
         yield self.{{safe_node_name(child_node)}}
         {% endfor %}
-
-    {# context manager #}
-    @{% if asyncoutput %}async{% endif %}contextmanager
-    {% if asyncoutput %}async {% endif %}def single_read(self) -> {% if asyncoutput %}AsyncGenerator['{{get_fully_qualified_type_name(node)}}_cls', None]{% else %}Generator['{{get_fully_qualified_type_name(node)}}_cls', None, None]{% endif %}:
-        """
-        Context Manager to do multiple accesses using a single read operation
-        """
-        {% if asyncoutput %}async {% endif %}with super().single_read() as reg:
-           yield cast('{{get_fully_qualified_type_name(node)}}_cls',reg)
-
-    {% if node.has_sw_writable %}
-    @{% if asyncoutput %}async{% endif %}contextmanager
-    {% if asyncoutput %}async {% endif %}def single_read_modify_write(self, verify:bool = False, skip_write: bool = False) -> {% if asyncoutput %}AsyncGenerator['{{get_fully_qualified_type_name(node)}}_cls', None]{% else %}Generator['{{get_fully_qualified_type_name(node)}}_cls', None, None]{% endif %}:
-        """
-        Context Manager to do multiple accesses using a single read/modify write operation
-        """
-        {% if asyncoutput %}async {% endif %}with super().single_read_modify_write(verify=verify, skip_write=skip_write) as reg:
-           yield cast('{{get_fully_qualified_type_name(node)}}_cls',reg)
-    {% endif %}
-
-
     {% endif %}
 
     {% if node.has_sw_writable %}
     @property
     def writable_fields(self) -> Iterator[Union[Field{% if asyncoutput %}Async{% endif %}WriteOnly, Field{% if asyncoutput %}Async{% endif %}ReadWrite]]:
         """
         generator that produces has all the writable fields within the register
```

### Comparing `peakrdl-python-0.7.3/src/peakrdl_python/templates/addrmap_tb.py.jinja` & `peakrdl-python-0.7.4/src/peakrdl_python/templates/addrmap_tb.py.jinja`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+{#
+peakrdl-python is a tool to generate Python Register Access Layer (RAL) from SystemRDL
+Copyright (C) 2021 - 2023
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <https://www.gnu.org/licenses/>.
+#}
+
 {% include "header_tb.py.jinja" with context %}
 from typing import List, Union, Dict
 from array import array as Array
 {% if asyncoutput %}
 import sys
 import asyncio
 if sys.version_info < (3, 8):
@@ -20,23 +38,35 @@
 from enum import IntEnum
 
 from ..lib import RegisterWriteVerifyError
 
 from ..reg_model.{{top_node.type_name}} import {{top_node.type_name}}_cls
 {% if asyncoutput %}
 from ..lib import FieldAsyncReadOnly, FieldAsyncWriteOnly, FieldAsyncReadWrite
-from ..lib import WritableAsyncRegister, ReadableAsyncRegister, RegAsyncReadWrite, RegAsyncReadOnly, RegAsyncWriteOnly
+from ..lib import WritableAsyncRegister, ReadableAsyncRegister
+from ..lib import RegAsyncReadWrite, RegAsyncReadOnly, RegAsyncWriteOnly
+from ..lib import RegAsyncReadWriteArray, RegAsyncReadOnlyArray, RegAsyncWriteOnlyArray
 from ..lib import MemoryAsyncReadOnly, MemoryAsyncWriteOnly, MemoryAsyncReadWrite
+from ..lib import MemoryAsyncReadOnlyArray, MemoryAsyncWriteOnlyArray, MemoryAsyncReadWriteArray
+from ..lib import AsyncAddressMap, AsyncRegFile
+from ..lib import AsyncAddressMapArray, AsyncRegFileArray
+from ..lib import AsyncMemory
 {% else %}
 from ..lib import FieldReadOnly, FieldWriteOnly, FieldReadWrite
-from ..lib import WritableRegister, ReadableRegister, RegReadWrite, RegReadOnly, RegWriteOnly
+from ..lib import WritableRegister, ReadableRegister
+from ..lib import RegReadWrite, RegReadOnly, RegWriteOnly
+from ..lib import RegReadWriteArray, RegReadOnlyArray, RegWriteOnlyArray
 from ..lib import MemoryReadOnly, MemoryWriteOnly, MemoryReadWrite
-{% endif %}
+from ..lib import MemoryReadOnlyArray, MemoryWriteOnlyArray, MemoryReadWriteArray
 from ..lib import AddressMap, RegFile
+from ..lib import AddressMapArray, RegFileArray
 from ..lib import Memory
+{% endif %}
+
+
 from ..lib import Field
 from ..lib import Reg
 
 from ._{{top_node.inst_name}}_test_base import {{top_node.type_name}}_TestCase, {{top_node.type_name}}_TestCase_BlockAccess
 from ._{{top_node.inst_name}}_test_base import __name__ as base_name
 
 class {{fq_block_name}}_single_access({{top_node.type_name}}_TestCase): # type: ignore[valid-type,misc]
@@ -47,36 +77,57 @@
         """
         {% for node in owned_elements.nodes -%}
         with self.subTest(msg='node: {{'.'.join(node.get_path_segments())}}'):
             self.assertEqual(self.dut.{{'.'.join(get_python_path_segments(node))}}.inst_name, '{{node.get_path_segments()[-1]}}') # type: ignore[union-attr]
             self.assertEqual(self.dut.{{'.'.join(get_python_path_segments(node))}}.full_inst_name, '{{'.'.join(node.get_path_segments())}}')  # type: ignore[union-attr]
         {% endfor %}
 
+    def test_sizes(self) -> None:
+        """
+        Check that the sizes all match
+        """
+        {% for node in owned_elements.addressable_nodes -%}
+        with self.subTest(msg='node: {{'.'.join(node.get_path_segments())}}'):
+            self.assertEqual(self.dut.{{'.'.join(get_python_path_segments(node))}}.size, {{node.size}}) # type: ignore[union-attr]
+        {% endfor %}
+
+        # check the size of the address map itself
+        {% if block == top_node %}
+        with self.subTest(msg='node: {{'.'.join(block.get_path_segments())}}'):
+            self.assertEqual(self.dut.size, {{block.size}}) # type: ignore[union-attr]
+        {% else %}
+        with self.subTest(msg='node: {{'.'.join(block.get_path_segments())}}'):
+            self.assertEqual(self.dut.{{'.'.join(get_python_path_segments(block))}}.size, {{block.size}}) # type: ignore[union-attr]
+        {% endif %}
+
+
     def test_register_properties(self)  -> None:
         """
         Walk the address map and check the address, size and accesswidth of every register is
         correct
         """
         {% for node in owned_elements.registers -%}
         with self.subTest(msg='register: {{'.'.join(node.get_path_segments())}}'):
             self.assertEqual(self.dut.{{'.'.join(get_python_path_segments(node))}}.address, {{node.absolute_address}}) # type: ignore[union-attr]
             self.assertEqual(self.dut.{{'.'.join(get_python_path_segments(node))}}.width, {{node.size * 8}}) # type: ignore[union-attr]
+            self.assertEqual(self.dut.{{'.'.join(get_python_path_segments(node))}}.size, {{node.size}}) # type: ignore[union-attr]
             {% if 'accesswidth' in node.list_properties() -%}self.assertEqual(self.dut.{{'.'.join(get_python_path_segments(node))}}.accesswidth, {{node.get_property('accesswidth')}}){%- else -%} self.assertEqual(self.dut.{{'.'.join(get_python_path_segments(node))}}.accesswidth, self.dut.{{'.'.join(get_python_path_segments(node))}}.accesswidth){%- endif %} # type: ignore[union-attr]
         {% endfor %}
 
     def test_memory_properties(self)  -> None:
         """
         Walk the address map and check the address, size and accesswidth of every memory is
         correct
         """
-        mut: Memory
+        mut: {% if asyncoutput %}Async{% endif %}Memory
         {% for node in owned_elements.memories -%}
         with self.subTest(msg='memory: {{'.'.join(node.get_path_segments())}}'):
             mut = self.dut.{{'.'.join(get_python_path_segments(node))}} # type: ignore[union-attr,assignment]
-            self.assertIsInstance(mut, Memory)
+
+            self.assertIsInstance(mut, (Memory{% if asyncoutput %}Async{% endif %}ReadOnly, Memory{% if asyncoutput %}Async{% endif %}WriteOnly, Memory{% if asyncoutput %}Async{% endif %}ReadWrite))
             self.assertEqual(mut.address, {{node.absolute_address}})
             self.assertEqual(mut.width, {{node.get_property('memwidth')}})
             self.assertEqual(mut.entries, {{node.get_property('mementries')}})
             {% if 'accesswidth' in node.list_properties() -%}self.assertEqual(mut.accesswidth, {{node.get_property('accesswidth')}}){%- else -%}self.assertEqual(mut.accesswidth, mut.accesswidth){%- endif %}
         {% endfor %}
 
     def test_field_properties(self)  -> None:
@@ -886,15 +937,15 @@
         expected_memories:List[Union[MemoryAsyncReadOnly, MemoryAsyncWriteOnly, MemoryAsyncReadWrite]]
 
         {% else %}
         expected_writable_regs: List[WritableRegister]
         expected_readable_regs: List[ReadableRegister]
         expected_memories:List[Union[MemoryReadOnly, MemoryWriteOnly, MemoryReadWrite]]
         {% endif %}
-        expected_sections : List[Union[AddressMap, RegFile]]
+        expected_sections : List[Union[{% if asyncoutput %}Async{% endif %}AddressMap, {% if asyncoutput %}Async{% endif %}RegFile]]
 
         # check the readable registers
         expected_readable_regs = [ {%- for child_node in top_node.children(unroll=True) %}
                                     {%- if isinstance(child_node, systemrdlRegNode) %}{% if child_node.has_sw_readable %}self.dut.{{'.'.join(get_python_path_segments(child_node))}}, # type: ignore[union-attr,list-item] {% endif %}{% endif %}
                                     {% endfor %} ]
         readable_regs = []
         for readable_reg in self.dut.get_readable_registers(unroll=True):  # type: ignore[union-attr]
@@ -930,15 +981,15 @@
 
         # check the sections
         expected_sections = [ {%- for child_node in top_node.children(unroll=True) %}
                               {%- if isinstance(child_node, (systemrdlAddrmapNode, systemrdlRegfileNode)) %}self.dut.{{'.'.join(get_python_path_segments(child_node))}}, # type: ignore[union-attr,list-item] {% endif %}
                               {% endfor %} ]
         sections = []
         for section in self.dut.get_sections(unroll=True):  # type: ignore[union-attr]
-            self.assertIsInstance(section, (AddressMap, RegFile))
+            self.assertIsInstance(section, ({% if asyncoutput %}Async{% endif %}AddressMap, {% if asyncoutput %}Async{% endif %}RegFile))
             sections.append(section)
         self.assertCountEqual(expected_sections, sections)
         {# check the rolled case second #}
         expected_sections = [ {%- for child_node in top_node.children(unroll=False) %}
                               {%- if isinstance(child_node, (systemrdlAddrmapNode, systemrdlRegfileNode)) %}self.dut.{{'.'.join(get_python_path_segments(child_node))}},  # type: ignore[union-attr,list-item] {% endif %}
                               {% endfor %} ]
         sections = []
@@ -948,23 +999,24 @@
 
         # check the memories
         expected_memories = [ {%- for child_node in top_node.children(unroll=True) %}
                               {%- if isinstance(child_node, systemrdlMemNode) %}self.dut.{{'.'.join(get_python_path_segments(child_node))}}, # type: ignore[union-attr,list-item] {% endif %}
                               {% endfor %} ]
         memories = []
         for memory in self.dut.get_memories(unroll=True):  # type: ignore[union-attr]
-            self.assertIsInstance(memory, Memory)
+            self.assertIsInstance(memory, (Memory{% if asyncoutput %}Async{% endif %}ReadOnly, Memory{% if asyncoutput %}Async{% endif %}WriteOnly, Memory{% if asyncoutput %}Async{% endif %}ReadWrite))
             memories.append(memory)
         self.assertCountEqual(expected_memories, memories)
         {# check the rolled case second #}
         expected_memories = [ {%- for child_node in top_node.children(unroll=False) %}
                               {%- if isinstance(child_node, systemrdlMemNode) %}self.dut.{{'.'.join(get_python_path_segments(child_node))}}, # type: ignore[union-attr,list-item] {% endif %}
                               {% endfor %} ]
         memories = []
         for memory in self.dut.get_memories(unroll=False):  # type: ignore[union-attr]
+            self.assertIsInstance(memory, (Memory{% if asyncoutput %}Async{% endif %}ReadOnly, Memory{% if asyncoutput %}Async{% endif %}WriteOnly, Memory{% if asyncoutput %}Async{% endif %}ReadWrite, Memory{% if asyncoutput %}Async{% endif %}ReadOnlyArray, Memory{% if asyncoutput %}Async{% endif %}WriteOnlyArray, Memory{% if asyncoutput %}Async{% endif %}ReadWriteArray))
             memories.append(memory)
         self.assertCountEqual(expected_memories, memories)
 
     {% endif %}{# if block == top_block #}
 
     {% macro check_readable_register_iterators(node) %}
         {# check the unrolled case first #}
@@ -978,14 +1030,15 @@
         self.assertCountEqual(expected_readable_regs, readable_regs)
         {# check the rolled case second #}
         expected_readable_regs = [ {%- for child_node in node.children(unroll=False) %}
                                    {%- if isinstance(child_node, systemrdlRegNode) %}{% if child_node.has_sw_readable %}self.dut.{{'.'.join(get_python_path_segments(child_node))}}, # type: ignore[union-attr,list-item] {% endif %}{% endif %}
                                    {% endfor %} ]
         readable_regs = []
         for readable_reg in self.dut.{{'.'.join(get_python_path_segments(node))}}.get_readable_registers(unroll=False):  # type: ignore[union-attr]
+            self.assertIsInstance(readable_reg, (Reg{% if asyncoutput %}Async{% endif %}ReadWrite, Reg{% if asyncoutput %}Async{% endif %}ReadOnly, Reg{% if asyncoutput %}Async{% endif %}ReadWriteArray, Reg{% if asyncoutput %}Async{% endif %}ReadOnlyArray))
             readable_regs.append(readable_reg)
         self.assertCountEqual(expected_readable_regs, readable_regs)
     {% endmacro %}
 
     {% macro check_writable_register_iterators(node) %}
         {# check the unrolled case first #}
         expected_writable_regs = [ {%- for child_node in node.children(unroll=True) %}
@@ -998,54 +1051,57 @@
         self.assertCountEqual(expected_writable_regs, writable_regs)
         {# check the rolled case second #}
         expected_writable_regs = [ {%- for child_node in node.children(unroll=False) %}
                                    {%- if isinstance(child_node, systemrdlRegNode) %}{% if child_node.has_sw_writable %}self.dut.{{'.'.join(get_python_path_segments(child_node))}}, # type: ignore[union-attr,list-item] {% endif %}{% endif %}
                                    {% endfor %} ]
         writable_regs = []
         for writable_reg in self.dut.{{'.'.join(get_python_path_segments(node))}}.get_writable_registers(unroll=False):  # type: ignore[union-attr]
+            self.assertIsInstance(writable_reg, (Reg{% if asyncoutput %}Async{% endif %}ReadWrite, Reg{% if asyncoutput %}Async{% endif %}WriteOnly, Reg{% if asyncoutput %}Async{% endif %}ReadWriteArray, Reg{% if asyncoutput %}Async{% endif %}WriteOnlyArray))
             writable_regs.append(writable_reg)
         self.assertCountEqual(expected_writable_regs, writable_regs)
     {% endmacro %}
 
     {% macro check_section_iterators(node) %}
         {# check the unrolled case first #}
         expected_sections = [ {%- for child_node in node.children(unroll=True) %}
                               {%- if isinstance(child_node, (systemrdlAddrmapNode, systemrdlRegfileNode)) %}self.dut.{{'.'.join(get_python_path_segments(child_node))}}, # type: ignore[union-attr,list-item] {% endif %}
                               {% endfor %} ]
         sections = []
         for section in self.dut.{{'.'.join(get_python_path_segments(node))}}.get_sections(unroll=True):  # type: ignore[union-attr]
-            self.assertIsInstance(section, (AddressMap, RegFile))
+            self.assertIsInstance(section, ({% if asyncoutput %}Async{% endif %}AddressMap, {% if asyncoutput %}Async{% endif %}RegFile))
             sections.append(section)
         self.assertCountEqual(expected_sections, sections)
         {# check the rolled case second #}
         expected_sections = [ {%- for child_node in node.children(unroll=False) %}
                               {%- if isinstance(child_node, (systemrdlAddrmapNode, systemrdlRegfileNode)) %}self.dut.{{'.'.join(get_python_path_segments(child_node))}},  # type: ignore[union-attr,list-item] {% endif %}
                               {% endfor %} ]
         sections = []
         for section in self.dut.{{'.'.join(get_python_path_segments(node))}}.get_sections(unroll=False):  # type: ignore[union-attr]
+            self.assertIsInstance(section, ({% if asyncoutput %}Async{% endif %}AddressMap, {% if asyncoutput %}Async{% endif %}RegFile, {% if asyncoutput %}Async{% endif %}AddressMapArray, {% if asyncoutput %}Async{% endif %}RegFileArray))
             sections.append(section)
         self.assertCountEqual(expected_sections, sections)
     {% endmacro %}
 
     {% macro check_memory_iterators(node) %}
         {# check the unrolled case first #}
         expected_memories = [ {%- for child_node in node.children(unroll=True) %}
                               {%- if isinstance(child_node, systemrdlMemNode) %}self.dut.{{'.'.join(get_python_path_segments(child_node))}}, # type: ignore[union-attr,list-item] {% endif %}
                               {% endfor %} ]
         memories = []
         for memory in self.dut.{{'.'.join(get_python_path_segments(node))}}.get_memories(unroll=True):  # type: ignore[union-attr]
-            self.assertIsInstance(memory, Memory)
+            self.assertIsInstance(memory, (Memory{% if asyncoutput %}Async{% endif %}ReadOnly, Memory{% if asyncoutput %}Async{% endif %}WriteOnly, Memory{% if asyncoutput %}Async{% endif %}ReadWrite))
             memories.append(memory)
         self.assertCountEqual(expected_memories, memories)
         {# check the rolled case second #}
         expected_memories = [ {%- for child_node in node.children(unroll=False) %}
                               {%- if isinstance(child_node, systemrdlMemNode) %}self.dut.{{'.'.join(get_python_path_segments(child_node))}}, # type: ignore[union-attr,list-item] {% endif %}
                               {% endfor %} ]
         memories = []
         for memory in self.dut.{{'.'.join(get_python_path_segments(node))}}.get_memories(unroll=False):  # type: ignore[union-attr]
+            self.assertIsInstance(memory, (Memory{% if asyncoutput %}Async{% endif %}ReadOnly, Memory{% if asyncoutput %}Async{% endif %}WriteOnly, Memory{% if asyncoutput %}Async{% endif %}ReadWrite, Memory{% if asyncoutput %}Async{% endif %}ReadOnlyArray, Memory{% if asyncoutput %}Async{% endif %}WriteOnlyArray, Memory{% if asyncoutput %}Async{% endif %}ReadWriteArray))
             memories.append(memory)
         self.assertCountEqual(expected_memories, memories)
     {% endmacro %}
 
     def test_traversal_iterators(self) -> None:
         """
         Walk the address map and check that the iterators for each node as as expected
@@ -1060,15 +1116,15 @@
         {% else %}
         expected_writable_fields: List[Union[FieldWriteOnly, FieldReadWrite]]
         expected_readable_fields: List[Union[FieldReadOnly, FieldReadWrite]]
         expected_writable_regs: List[WritableRegister]
         expected_readable_regs: List[ReadableRegister]
         expected_memories:List[Union[MemoryReadOnly, MemoryWriteOnly, MemoryReadWrite]]
         {% endif %}
-        expected_sections : List[Union[AddressMap, RegFile]]
+        expected_sections : List[Union[{% if asyncoutput %}Async{% endif %}AddressMap, {% if asyncoutput %}Async{% endif %}RegFile]]
 
         # test all the registers
         {% for node in owned_elements.registers -%}
         with self.subTest(msg='register: {{'.'.join(node.get_path_segments())}}'):
                 {# a register can only have fields beneath it #}
                 {% if node.has_sw_writable %}
             expected_writable_fields = [ {%- for child_node in node.children(unroll=True) -%}
@@ -1233,14 +1289,48 @@
             write_block_callback_mock.reset_mock()
 
             {%- endif %}
 
         {%- endfor %}
     {%- endif %}
 
+    {% if asyncoutput %}async {% endif %}def test_register_array_context_manager(self) -> None:
+        """
+        Walk the register map and check that register map context managers work correctly
+        """
+        {% for node in rolled_owned_reg_array %}
+        # test context manager to register:
+        # {{'.'.join(node.get_path_segments())}}
+        # size {{node.size}}
+        # total_size {{node.total_size}}
+        empty_read = [0 for i in range({{node.total_size}} // {{node.size}})]
+        follow_along = [0 for i in range({{node.total_size}} // {{node.size}})]
+        with self.subTest(msg='register: {{'.'.join(node.get_path_segments())}}'):
+            with patch(base_name + '.write_addr_space') as write_callback_mock,\
+                                patch(base_name + '.read_addr_space', return_value=0) as read_callback_mock, \
+                                patch(base_name + '.read_block_addr_space',
+                                      return_value=Array('{{get_array_typecode(node.size * 8)}}', empty_read)) as read_block_callback_mock , \
+                                patch(base_name + '.write_block_addr_space') as write_block_callback_mock:
+                {% if node.has_sw_readable and node.has_sw_writable -%}
+                {% if asyncoutput %}async {% endif %}with self.dut.{{'.'.join(get_python_path_segments(node))}}.single_read_modify_write() as dut:
+                    pass
+                {% elif not node.has_sw_readable and node.has_sw_writable-%}
+                {% if asyncoutput %}async {% endif %}with self.dut.{{'.'.join(get_python_path_segments(node))}}.single_write() as dut:
+                    pass
+                read_block_callback_mock.assert_not_called()
+                {% elif node.has_sw_readable and not node.has_sw_writable-%}
+                {% if asyncoutput %}async {% endif %}with self.dut.{{'.'.join(get_python_path_segments(node))}}.single_read() as dut:
+                    pass
+                write_block_callback_mock.assert_not_called()
+                {% endif %}
+                read_callback_mock.assert_not_called()
+                write_callback_mock.assert_not_called()
+
+        {%- endfor %}
+
 
 if __name__ == '__main__':
 {% if asyncoutput %}
     if sys.version_info < (3, 8):
         asynctest.main()
     else:
         unittest.main()
```

### Comparing `peakrdl-python-0.7.3/src/peakrdl_python/templates/baseclass_tb.py.jinja` & `peakrdl-python-0.7.4/src/peakrdl_python/templates/baseclass_tb.py.jinja`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+{#
+peakrdl-python is a tool to generate Python Register Access Layer (RAL) from SystemRDL
+Copyright (C) 2021 - 2023
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <https://www.gnu.org/licenses/>.
+#}
+
 {% include "header_tb.py.jinja" with context %}
 from array import array as Array
 {% if asyncoutput %}
 import sys
 import asyncio
 if sys.version_info < (3, 8):
     import asynctest  # type: ignore[import]
@@ -86,15 +104,15 @@
 {% else %}
 TestCaseBase = unittest.TestCase
 {% endif %}
 
 class {{top_node.type_name}}_TestCase(TestCaseBase): # type: ignore[valid-type,misc]
 
     def setUp(self) -> None:
-        self.dut = {{top_node.type_name}}_cls({% if asyncoutput %}AsyncCallbackSet{% else %}NormalCallbackSet{% endif %}(read_callback=read_callback,
+        self.dut = {{top_node.type_name}}_cls(callbacks={% if asyncoutput %}AsyncCallbackSet{% else %}NormalCallbackSet{% endif %}(read_callback=read_callback,
                                                           write_callback=write_callback))
 
     @staticmethod
     def _reverse_bits(value: int, number_bits: int) -> int:
         """
 
         Args:
@@ -109,15 +127,15 @@
             if (value >> i) & 1:
                 result |= 1 << (number_bits - 1 - i)
         return result
 
 class {{top_node.type_name}}_TestCase_BlockAccess(TestCaseBase): # type: ignore[valid-type,misc]
 
     def setUp(self) -> None:
-        self.dut = {{top_node.type_name}}_cls({% if asyncoutput %}AsyncCallbackSet{% else %}NormalCallbackSet{% endif %}(read_callback=read_callback,
+        self.dut = {{top_node.type_name}}_cls(callbacks={% if asyncoutput %}AsyncCallbackSet{% else %}NormalCallbackSet{% endif %}(read_callback=read_callback,
                                                           write_callback=write_callback,
                                                           read_block_callback=read_block_callback,
                                                           write_block_callback=write_block_callback))
```

### Comparing `peakrdl-python-0.7.3/src/peakrdl_python.egg-info/PKG-INFO` & `peakrdl-python-0.7.4/src/peakrdl_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: peakrdl-python
-Version: 0.7.3
-Summary: Generate python wrapper for a register model compiled SystemRDL input
+Version: 0.7.4
+Summary: Generate Python Register Access Layer (RAL) from SystemRDL
 Author: Keith Brady
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -678,15 +678,15 @@
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Source, https://github.com/krcb197/PeakRDL-python
 Project-URL: Tracker, https://github.com/krcb197/PeakRDL-python/issues
 Project-URL: Documentation, https://peakrdl-python.readthedocs.io/
 Project-URL: Changelog, https://github.com/krcb197/PeakRDL-python/releases
-Keywords: SystmRDL,PeakRDL,CSR,compiler,tool,registers,generator,Python
+Keywords: SystemRDL,PeakRDL,CSR,compiler,tool,registers,generator,Python
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -699,20 +699,21 @@
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: systemrdl-compiler>=1.24.0
 Requires-Dist: jinja2
 Requires-Dist: asynctest; python_version < "3.8"
+Requires-Dist: typing-extensions; python_version < "3.11"
 
 ![CI](https://github.com/krcb197/PeakRDL-python/actions/workflows/action.yaml/badge.svg)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/peakrdl-python.svg)](https://pypi.org/project/peakrdl-python)
 [![Documentation Status](https://readthedocs.org/projects/peakrdl-python/badge/?version=latest)](https://peakrdl-python.readthedocs.io/en/latest/?badge=latest)
 [![Downloads](https://static.pepy.tech/badge/peakrdl-python)](https://pepy.tech/project/peakrdl-python)
 
-# PeakRDL-python
-Generate Python wrapper for a register model compiled SystemRDL input
+# peakrdl-python
+Generate Python Register Access Layer (RAL) from SystemRDL
 
 ## Documentation
-See the [PeakRDL Python Documentation](https://peakrdl-python.readthedocs.io/) for more details
+See the [peakrdl-python Documentation](https://peakrdl-python.readthedocs.io/) for more details
```

### Comparing `peakrdl-python-0.7.3/src/peakrdl_python.egg-info/SOURCES.txt` & `peakrdl-python-0.7.4/src/peakrdl_python.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,51 @@
 .gitignore
 .readthedocs.yaml
 LICENSE
 MANIFEST.in
 README.md
+generate_and_test.py
 generate_testcases.py
 pyproject.toml
 .github/workflows/action.yaml
 docs/api.rst
 docs/api_components.rst
 docs/command_line.rst
 docs/conf.py
 docs/customisation.rst
+docs/design_decisions.rst
+docs/design_tools.rst
 docs/generated_package.rst
 docs/genindex.rst
 docs/index.rst
+docs/installation.rst
 docs/requirements.txt
 example/array_access/array_access.rdl
 example/array_access/demo_array_access.py
+example/enumerated_fields/demo_enumerated_fields.py
+example/enumerated_fields/enumerated_fields.rdl
 example/optimised_access/demo_optimised_access.py
+example/optimised_access/demo_optimised_array_access.py
 example/optimised_access/optimised_access.rdl
+example/optimised_access/optimised_array_access.rdl
 example/overridden_names/over_ridden_names.py
 example/overridden_names/overridden_names.rdl
 example/simulating_callbacks/chip_with_a_GPIO.rdl
 example/simulating_callbacks/flashing_the_LED.py
 example/tranversing_address_map/chip_with_registers.rdl
 example/tranversing_address_map/dumping_register_state_to_json_file.py
 example/tranversing_address_map/reg_dump.json
 example/tranversing_address_map/reseting_registers.py
 example/tranversing_address_map/writing_register_state_from_json_file.py
+example/why_ral/__init__.py
+example/why_ral/gpio.rdl
+example/why_ral/hardware_sim.py
+example/why_ral/with_hal.py
+example/why_ral/with_ral.py
+example/why_ral/without_ral.py
 src/peakrdl_python/.coveragerc
 src/peakrdl_python/__about__.py
 src/peakrdl_python/__init__.py
 src/peakrdl_python/__peakrdl__.py
 src/peakrdl_python/_node_walkers.py
 src/peakrdl_python/exporter.py
 src/peakrdl_python/safe_name_utility.py
@@ -39,19 +53,21 @@
 src/peakrdl_python.egg-info/PKG-INFO
 src/peakrdl_python.egg-info/SOURCES.txt
 src/peakrdl_python.egg-info/dependency_links.txt
 src/peakrdl_python.egg-info/entry_points.txt
 src/peakrdl_python.egg-info/requires.txt
 src/peakrdl_python.egg-info/top_level.txt
 src/peakrdl_python/lib/__init__.py
+src/peakrdl_python/lib/async_register.py
 src/peakrdl_python/lib/base.py
 src/peakrdl_python/lib/callbacks.py
 src/peakrdl_python/lib/fields.py
 src/peakrdl_python/lib/memory.py
 src/peakrdl_python/lib/register.py
+src/peakrdl_python/lib/utility_functions.py
 src/peakrdl_python/templates/__init__.py
 src/peakrdl_python/templates/addrmap.py.jinja
 src/peakrdl_python/templates/addrmap_field.py.jinja
 src/peakrdl_python/templates/addrmap_memory.py.jinja
 src/peakrdl_python/templates/addrmap_register.py.jinja
 src/peakrdl_python/templates/addrmap_simulation.py.jinja
 src/peakrdl_python/templates/addrmap_simulation_tb.jinja
@@ -88,10 +104,14 @@
 tests/testcases/parametrised_readonly_and_readwrite.rdl
 tests/testcases/regfile_and_arrays.rdl
 tests/testcases/same_but_different_enum.rdl
 tests/testcases/signals_definitions_at_various_levels.rdl
 tests/testcases/simple.rdl
 tests/testcases/simple.xml
 tests/testcases/sizes_registers.rdl
+tests/testcases/sizes_registers_array.rdl
 tests/testcases/write_only_enum_with_undefined_reset.rdl
 tests/unit_tests/__init__.py
-tests/unit_tests/test_array_indexing.py
+tests/unit_tests/simple_components.py
+tests/unit_tests/test_array_indexing.py
+tests/unit_tests/test_optimised_reg_array.py
+tests/unit_tests/test_reg.py
```

### Comparing `peakrdl-python-0.7.3/tests/pylint.rc` & `peakrdl-python-0.7.4/tests/pylint.rc`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.3/tests/testcases/addr_map.rdl` & `peakrdl-python-0.7.4/tests/testcases/addr_map.rdl`

 * *Files 16% similar despite different names*

```diff
@@ -29,8 +29,10 @@
 };
 
 addrmap addr_map {
     regtype_a top_reg;
     child_addr_map_type_a child_a;
     child_addr_map_type_b child_b[2];
     child_addr_map_type_c child_c;
+    child_addr_map_type_b child_b_offset[2] += 48;
+
 };
```

### Comparing `peakrdl-python-0.7.3/tests/testcases/basic.rdl` & `peakrdl-python-0.7.4/tests/testcases/basic.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.3/tests/testcases/block_a.xml` & `peakrdl-python-0.7.4/tests/testcases/block_a.xml`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.3/tests/testcases/block_b.xml` & `peakrdl-python-0.7.4/tests/testcases/block_b.xml`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.3/tests/testcases/different_array_types.rdl` & `peakrdl-python-0.7.4/tests/testcases/different_array_types.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.3/tests/testcases/enum_example.rdl` & `peakrdl-python-0.7.4/tests/testcases/enum_example.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.3/tests/testcases/example_issue_106.rdl` & `peakrdl-python-0.7.4/tests/testcases/example_issue_106.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.3/tests/testcases/field_with_overridden_reset.rdl` & `peakrdl-python-0.7.4/tests/testcases/field_with_overridden_reset.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.3/tests/testcases/fields_with_reset_values.rdl` & `peakrdl-python-0.7.4/tests/testcases/fields_with_reset_values.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.3/tests/testcases/memories.rdl` & `peakrdl-python-0.7.4/tests/testcases/memories.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.3/tests/testcases/msb0_and_lsb0.rdl` & `peakrdl-python-0.7.4/tests/testcases/msb0_and_lsb0.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.3/tests/testcases/name_clash.rdl` & `peakrdl-python-0.7.4/tests/testcases/name_clash.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.3/tests/testcases/overridden_python_name.rdl` & `peakrdl-python-0.7.4/tests/testcases/overridden_python_name.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.3/tests/testcases/regfile_and_arrays.rdl` & `peakrdl-python-0.7.4/tests/testcases/regfile_and_arrays.rdl`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         field {} basicfield_a[31:0];
     };
 
     regfile {
         basic_reg_Type basic_reg_a;
     } layer1_regfile_a[2];
 
-    basic_reg_Type layer0_reg_a;
+    basic_reg_Type layer0_reg_a[2];
     regfile {
         regfile {
 			desc = "some description of the regfile";
             reg basic_reg_Type2 {
                 default sw = r;
                 default hw = r;
                 field {} basicfield_a[31:0];
```

### Comparing `peakrdl-python-0.7.3/tests/testcases/same_but_different_enum.rdl` & `peakrdl-python-0.7.4/tests/testcases/same_but_different_enum.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.3/tests/testcases/signals_definitions_at_various_levels.rdl` & `peakrdl-python-0.7.4/tests/testcases/signals_definitions_at_various_levels.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.3/tests/testcases/simple.xml` & `peakrdl-python-0.7.4/tests/testcases/simple.xml`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.3/tests/testcases/sizes_registers.rdl` & `peakrdl-python-0.7.4/tests/testcases/sizes_registers.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.3/tests/unit_tests/test_array_indexing.py` & `peakrdl-python-0.7.4/tests/unit_tests/test_array_indexing.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,162 +1,166 @@
+"""
+Tests for the array indexing in the base library
+"""
+
 import unittest
-from typing import List, Generator, Iterator, Dict, Type, Tuple
+from typing import Tuple, Optional, Iterator, Union, Dict
 from abc import ABC, abstractmethod
-from contextlib import contextmanager
 from itertools import product
 
-from peakrdl_python.lib import RegReadOnlyArray, FieldReadOnly, RegReadOnly, \
-    NormalCallbackSet, AddressMap, FieldMiscProps, FieldSizeProps, Node
+# pylint: disable-next=unused-wildcard-import, wildcard-import
+from peakrdl_python.lib import *
 
-class FieldToTest(FieldReadOnly):
-    """
-    Class to represent a register field in the register model
-    """
-    __slots__: List[str] = []
+from .simple_components import ReadOnlyRegisterArrayToTest, CallBackTestWrapper
 
+# pylint: disable=logging-not-lazy,logging-fstring-interpolation
 
-class RegisterToTest(RegReadOnly):
+class ArrayBase(CallBackTestWrapper, ABC):
     """
-    Class to represent a register in the register model
+    Base of the Array indexing tests
     """
-    __slots__: List[str] = ['__field']
-
-    def __init__(self,
-                 callbacks: NormalCallbackSet,
-                 address: int,
-                 logger_handle: str,
-                 inst_name: str,
-                 parent: AddressMap):
-        super().__init__(callbacks=callbacks,
-                         address=address,
-                         accesswidth=32,
-                         width=32,
-                         logger_handle=logger_handle,
-                         inst_name=inst_name,
-                         parent=parent)
-
-        # build the field attributes
-        self.__field: FieldToTest = FieldToTest(
-            parent_register=self,
-            size_props=FieldSizeProps(
-                width=1,
-                lsb=0,
-                msb=0,
-                low=0,
-                high=0),
-            misc_props=FieldMiscProps(
-                default=None,
-                is_volatile=False),
-            logger_handle=logger_handle + '.field',
-            inst_name='field')
 
     @property
-    def readable_fields(self) -> Iterator[FieldReadOnly]:
+    @abstractmethod
+    def dimensions(self) -> Tuple[int, ...]:
         """
-        generator that produces has all the readable fields within the register
+        Array dimensions
         """
-        yield self.field
 
-    @contextmanager
-    def single_read(self) -> Generator['RegisterToTest', None, None]:
+    @property
+    @abstractmethod
+    def base_address(self) -> int:
         """
-        Context Manager to do multiple accesses using a single read operation
+        Array address
         """
-        with super().single_read() as reg:
-            yield cast('basic_basicreg_c_cls', reg)
 
-    # build the properties for the fields
     @property
-    def field_(self) -> FieldToTest:
+    @abstractmethod
+    def stride(self) -> int:
         """
-        Property to access field of the register
+        Array address stride
         """
-        return self.__field
 
     @property
-    def systemrdl_python_child_name_map(self) -> Dict[str, str]:
+    def dut(self) -> ReadOnlyRegisterArrayToTest:
         """
-        In some cases systemRDL names need to be converted make them python safe, this dictionary
-        is used to map the original systemRDL names to the names of the python attributes of this
-        class
-
-        Returns: dictionary whose key is the systemRDL names and value it the property name
+        Register Array under test
         """
-        return {
-            'field': 'field',
-        }
-
-class RegisterArrayToTest(RegReadOnlyArray):
-    """
-    Class to represent a register array in the register model
-    """
-    __slots__: List[str] = []
-
-    @property
-    def _element_datatype(self) -> Type[Node]:
-        return RegisterToTest
-
-
-class ArrayBase(unittest.TestCase, ABC):
-
-    @property
-    @abstractmethod
-    def dimensions(self) -> int:
-        pass
-
-    @property
-    @abstractmethod
-    def base_address(self) -> int:
-        pass
-
-    @property
-    @abstractmethod
-    def stride(self) -> int:
-        pass
-
-    @property
-    def dut(self) -> RegisterArrayToTest:
-        return self.__dut
+        return self.__dut_warpper.dut
 
     @abstractmethod
     def calculate_address(self, indices: Tuple[int, ...]) -> int:
-        ...
+        """
+        address based on array index
+        """
+
 
     def setUp(self) -> None:
-        self.__dut = RegisterArrayToTest(logger_handle='dut',
-                                       inst_name='dut',
-                                       parent=None,
-                                       callbacks=NormalCallbackSet(),
-                                       address=self.base_address,
-                                       stride=self.stride,
-                                       dimensions=self.dimensions)
+
+        class DUTWrapper(AddressMap):
+            """
+            Address map to to wrap the register array being tested
+            """
+
+            # pylint: disable=too-many-arguments,duplicate-code
+            def __init__(self,
+                         callbacks: Optional[CallbackSet],
+                         address: int,
+                         logger_handle: str,
+                         inst_name: str,
+                         dut_stride : int,
+                         dut_dimensions : Tuple[int, ...]):
+
+
+                super().__init__(callbacks=callbacks, address=address, logger_handle=logger_handle,
+                                 inst_name=inst_name, parent=None )
+
+                self.__dut = ReadOnlyRegisterArrayToTest(logger_handle='dut',
+                                                         inst_name='dut',
+                                                         parent=self,
+                                                         address=address,
+                                                         width=32,
+                                                         accesswidth=32,
+                                                         stride=dut_stride,
+                                                         dimensions=dut_dimensions)
+
+            def get_memories(self, unroll: bool = False) -> \
+                    Iterator[Union[Memory, Tuple[Memory, ...]]]:
+                raise NotImplementedError('Not implemented in the testing')
+
+            def get_sections(self, unroll: bool = False) -> \
+                    Iterator[Union[Union[AddressMap, RegFile],
+                                   Tuple[Union[AddressMap, RegFile], ...]]]:
+                raise NotImplementedError('Not implemented in the testing')
+
+            def get_registers(self, unroll: bool = False) -> \
+                    Iterator[Union[Reg, RegArray]]:
+                """
+                generator that produces all the registers of this node
+                """
+                raise NotImplementedError('Not implemented in the testing')
+
+            @property
+            def systemrdl_python_child_name_map(self) -> Dict[str, str]:
+
+                return {
+                    'dut': 'dut'
+                }
+
+            # pylint: enable=duplicate-code
+
+            @property
+            def dut(self) -> ReadOnlyRegisterArrayToTest:
+                """
+                Register Array under Test
+                """
+                return self.__dut
+
+            @property
+            def size(self) -> int:
+                return self.dut.size
+
+        super().setUp()
+        self.__dut_warpper = DUTWrapper(callbacks=self.callbacks, address=self.base_address,
+                                        logger_handle='dut_wrapper', inst_name='dut_wrapper',
+                                        dut_stride=self.stride, dut_dimensions=self.dimensions)
 
 
 class Test1DArray(ArrayBase):
+    """
+    Test for 1D arrays
+    """
+
 
     @property
-    def dimensions(self) -> int:
+    def dimensions(self) -> Tuple[int, ...]:
         return (10,)
 
     @property
     def stride(self) -> int:
         return 4
 
     @property
     def base_address(self) -> int:
         return 0
 
     def calculate_address(self, indices: Tuple[int, ...]) -> int:
         return (indices[0] * self.stride) + self.base_address
 
-    def test_individual_access(self):
+    def test_individual_access(self) -> None:
+        """
+        Test accessing individual array elements
+        """
         for index in range(self.dimensions[0]):
             self.assertEqual(self.dut[index].address, self.calculate_address((index,)))
 
-    def test_slice(self):
+    def test_slice(self) -> None:
+        """
+        Test accessing slices of the array
+        """
 
         full_slice = self.dut[:]
 
         for index in range(self.dimensions[0]):
             self.assertEqual(full_slice[index].address, self.calculate_address((index,)))
 
         even_slice = self.dut[::2]
@@ -180,32 +184,38 @@
             if index in range(2,self.dimensions[0]-2):
                 self.assertEqual(subset_slice[index].address, self.calculate_address((index,)))
             else:
                 with self.assertRaises(IndexError):
                     _ = subset_slice[index]
 
 class Test2DArray(ArrayBase):
+    """
+    Test for 2D arrays
+    """
 
     @property
-    def dimensions(self) -> int:
+    def dimensions(self) -> Tuple[int, ...]:
         return (10, 12,)
 
     @property
     def stride(self) -> int:
         return 4
 
     @property
     def base_address(self) -> int:
         return 0
 
     def calculate_address(self, indices: Tuple[int, ...]) -> int:
         return (indices[0] * self.dimensions[1] * self.stride) + \
                (indices[1] * self.stride) + self.base_address
 
-    def test_individual_access(self):
+    def test_individual_access(self) -> None:
+        """
+        Test accessing individual array elements
+        """
 
         # do some spot checks
         self.assertEqual(self.dut[0, 0].address, self.calculate_address((0, 0)))
         self.assertEqual(self.dut[1, 1].address, self.calculate_address((1, 1)))
         self.assertEqual(self.dut[1, 2].address, self.calculate_address((1, 2)))
 
         with self.assertRaises(IndexError):
@@ -214,29 +224,38 @@
         with self.assertRaises(IndexError):
             _ = self.dut[1]
 
         # sweep every item
         for index in product(*[range(dim) for dim in self.dimensions]):
             self.assertEqual(self.dut[index].address, self.calculate_address(index))
 
-    def test_inner_slice_access(self):
+    def test_inner_slice_access(self) -> None:
+        """
+        Test accessing an inner slice of the array elements
+        """
 
         inner_chunk = self.dut[0, :]
         for index, entry in enumerate(inner_chunk):
             self.assertEqual(entry.address, self.calculate_address((0, index)))
 
         _ = self.dut[0, 12:]
 
-    def test_outer_slice_access(self):
+    def test_outer_slice_access(self) -> None:
+        """
+        Test accessing an outer slice of the array elements
+        """
 
         outer_chunk = self.dut[:, 0]
         for index, entry in enumerate(outer_chunk):
             self.assertEqual(entry.address, self.calculate_address((index, 0)))
 
-    def test_inner_section(self):
+    def test_inner_section(self) -> None:
+        """
+        Test accessing an sub-section of the array
+        """
 
         chunk = self.dut[2:-2, 3:-3]
         for index, entry in zip(product(range(2,8), range(3,9)), chunk):
             self.assertEqual(entry.address, self.calculate_address(index))
 
 if __name__ == '__main__':
     unittest.main()
```

