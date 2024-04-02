# Comparing `tmp/excitingtools-1.7.0.tar.gz` & `tmp/excitingtools-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/builds/sol/exciting/tools/exciting_tools/dist/.tmp-6u83se2y/excitingtools-1.7.0.tar", last modified: Mon Mar 25 14:29:25 2024, max compression
+gzip compressed data, was "excitingtools-1.7.1.tar", last modified: Tue Apr  2 20:46:36 2024, max compression
```

## Comparing `excitingtools-1.7.0.tar` & `excitingtools-1.7.1.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 14:29:25.000000 excitingtools-1.7.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 14:29:25.000000 excitingtools-1.7.0/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 14:29:25.000000 excitingtools-1.7.0/.github/workflows/
--rw-rw-rw-   0 root         (0) root         (0)      602 2024-03-25 14:28:51.000000 excitingtools-1.7.0/.github/workflows/actions.yml
--rw-rw-rw-   0 root         (0) root         (0)      647 2024-03-25 14:28:51.000000 excitingtools-1.7.0/.github/workflows/joss.yml
--rw-rw-rw-   0 root         (0) root         (0)    21948 2024-03-25 14:28:51.000000 excitingtools-1.7.0/.pylintrc
--rw-rw-rw-   0 root         (0) root         (0)     8901 2024-03-25 14:28:51.000000 excitingtools-1.7.0/.style.yapf
--rw-rw-rw-   0 root         (0) root         (0)     1916 2024-03-25 14:28:51.000000 excitingtools-1.7.0/CITATION.cff
--rw-rw-rw-   0 root         (0) root         (0)     5375 2024-03-25 14:28:51.000000 excitingtools-1.7.0/CONTRIBUTING.md
--rw-rw-rw-   0 root         (0) root         (0)     7650 2024-03-25 14:28:51.000000 excitingtools-1.7.0/COPYING.LESSER
--rw-rw-rw-   0 root         (0) root         (0)    34915 2024-03-25 14:28:51.000000 excitingtools-1.7.0/COPYING.md
--rw-r--r--   0 root         (0) root         (0)    15017 2024-03-25 14:29:25.000000 excitingtools-1.7.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    14448 2024-03-25 14:28:51.000000 excitingtools-1.7.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 14:29:25.000000 excitingtools-1.7.0/excitingtools/
--rw-rw-rw-   0 root         (0) root         (0)      792 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 14:29:25.000000 excitingtools-1.7.0/excitingtools/constants/
--rw-rw-rw-   0 root         (0) root         (0)     1727 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/constants/units.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 14:29:25.000000 excitingtools-1.7.0/excitingtools/dataclasses/
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/dataclasses/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5366 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/dataclasses/band_structure.py
--rw-rw-rw-   0 root         (0) root         (0)      807 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/dataclasses/data_structs.py
--rw-rw-rw-   0 root         (0) root         (0)      145 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/dataclasses/density_of_states.py
--rw-rw-rw-   0 root         (0) root         (0)     6662 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/dataclasses/eigenvalues.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 14:29:25.000000 excitingtools-1.7.0/excitingtools/eigenstates/
--rw-rw-rw-   0 root         (0) root         (0)     1111 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/eigenstates/eigenstates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 14:29:25.000000 excitingtools-1.7.0/excitingtools/exciting_dict_parsers/
--rw-rw-rw-   0 root         (0) root         (0)     5906 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/exciting_dict_parsers/RT_TDDFT_parser.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-25 14:28:52.000000 excitingtools-1.7.0/excitingtools/exciting_dict_parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5722 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/exciting_dict_parsers/bse_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    16078 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/exciting_dict_parsers/groundstate_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     6829 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/exciting_dict_parsers/gw_eigenvalues_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     3880 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/exciting_dict_parsers/gw_eps00_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    16723 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/exciting_dict_parsers/gw_info_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     4361 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/exciting_dict_parsers/gw_taskgroup_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     3292 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/exciting_dict_parsers/gw_vxc_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     5802 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/exciting_dict_parsers/input_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     5691 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/exciting_dict_parsers/parser_factory.py
--rw-rw-rw-   0 root         (0) root         (0)    24629 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/exciting_dict_parsers/properties_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     3081 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/exciting_dict_parsers/species_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     8260 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/exciting_dict_parsers/state_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 14:29:25.000000 excitingtools-1.7.0/excitingtools/exciting_obj_parsers/
--rw-rw-rw-   0 root         (0) root         (0)      219 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/exciting_obj_parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1448 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/exciting_obj_parsers/eigenvalue_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     4331 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/exciting_obj_parsers/gw_eigenvalues.py
--rw-rw-rw-   0 root         (0) root         (0)      634 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/exciting_obj_parsers/input_xml.py
--rw-rw-rw-   0 root         (0) root         (0)     1230 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/exciting_obj_parsers/ks_band_structure.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 14:29:25.000000 excitingtools-1.7.0/excitingtools/input/
--rw-rw-rw-   0 root         (0) root         (0)      399 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/input/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2816 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/input/bandstructure.py
--rw-rw-rw-   0 root         (0) root         (0)     9363 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/input/base_class.py
--rw-rw-rw-   0 root         (0) root         (0)     4734 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/input/dynamic_class.py
--rw-rw-rw-   0 root         (0) root         (0)     4255 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/input/input_classes.py
--rw-rw-rw-   0 root         (0) root         (0)     1297 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/input/input_xml.py
--rw-rw-rw-   0 root         (0) root         (0)    12907 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/input/structure.py
--rw-rw-rw-   0 root         (0) root         (0)     4617 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/input/xml_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 14:29:25.000000 excitingtools-1.7.0/excitingtools/math/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-25 14:28:52.000000 excitingtools-1.7.0/excitingtools/math/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      576 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/math/math_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 14:29:25.000000 excitingtools-1.7.0/excitingtools/parser_utils/
--rw-rw-rw-   0 root         (0) root         (0)       78 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/parser_utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       46 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/parser_utils/erroneous_file_error.py
--rw-rw-rw-   0 root         (0) root         (0)      960 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/parser_utils/grep_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     3049 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/parser_utils/parser_decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     2928 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/parser_utils/parser_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2227 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/parser_utils/regex_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     1668 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/parser_utils/simple_parser.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-25 14:28:52.000000 excitingtools-1.7.0/excitingtools/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 14:29:25.000000 excitingtools-1.7.0/excitingtools/runner/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-25 14:28:52.000000 excitingtools-1.7.0/excitingtools/runner/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6139 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/runner/runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 14:29:25.000000 excitingtools-1.7.0/excitingtools/species/
--rw-rw-rw-   0 root         (0) root         (0)    16525 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/species/species_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 14:29:25.000000 excitingtools-1.7.0/excitingtools/structure/
--rw-rw-rw-   0 root         (0) root         (0)      878 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/structure/ase_utilities.py
--rw-rw-rw-   0 root         (0) root         (0)     4137 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/structure/lattice.py
--rw-rw-rw-   0 root         (0) root         (0)     1532 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/structure/pymatgen_utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 14:29:25.000000 excitingtools-1.7.0/excitingtools/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-25 14:28:52.000000 excitingtools-1.7.0/excitingtools/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5347 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/utils/dict_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      500 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/utils/jobflow_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     9842 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/utils/schema_parsing.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/utils/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2583 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/utils/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    20597 2024-03-25 14:28:51.000000 excitingtools-1.7.0/excitingtools/utils/valid_attributes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 14:29:25.000000 excitingtools-1.7.0/excitingtools.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15017 2024-03-25 14:29:23.000000 excitingtools-1.7.0/excitingtools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4944 2024-03-25 14:29:25.000000 excitingtools-1.7.0/excitingtools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-25 14:29:23.000000 excitingtools-1.7.0/excitingtools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       85 2024-03-25 14:29:23.000000 excitingtools-1.7.0/excitingtools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-03-25 14:29:23.000000 excitingtools-1.7.0/excitingtools.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      243 2024-03-25 14:28:51.000000 excitingtools-1.7.0/git-blame-ignore-revs
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 14:29:25.000000 excitingtools-1.7.0/paper/
--rw-rw-rw-   0 root         (0) root         (0)    10387 2024-03-25 14:28:51.000000 excitingtools-1.7.0/paper/joss_latex.template
--rw-rw-rw-   0 root         (0) root         (0)    14039 2024-03-25 14:28:51.000000 excitingtools-1.7.0/paper/latex.template
--rw-rw-rw-   0 root         (0) root         (0)     5301 2024-03-25 14:28:51.000000 excitingtools-1.7.0/paper/paper.bib
--rw-rw-rw-   0 root         (0) root         (0)     8645 2024-03-25 14:28:51.000000 excitingtools-1.7.0/paper/paper.md
--rw-rw-rw-   0 root         (0) root         (0)      866 2024-03-25 14:28:51.000000 excitingtools-1.7.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       81 2024-03-25 14:28:51.000000 excitingtools-1.7.0/pytest.ini
--rw-rw-rw-   0 root         (0) root         (0)       33 2024-03-25 14:28:51.000000 excitingtools-1.7.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-25 14:29:25.000000 excitingtools-1.7.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 14:29:25.000000 excitingtools-1.7.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-25 14:28:52.000000 excitingtools-1.7.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      416 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 14:29:25.000000 excitingtools-1.7.0/tests/dataclasses/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-25 14:28:52.000000 excitingtools-1.7.0/tests/dataclasses/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3774 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/dataclasses/test_band_structure.py
--rw-rw-rw-   0 root         (0) root         (0)     5438 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/dataclasses/test_eigenvalues.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 14:29:25.000000 excitingtools-1.7.0/tests/dict_parsers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-25 14:28:52.000000 excitingtools-1.7.0/tests/dict_parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1652 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/dict_parsers/test_RT_TDDFT_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    17404 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/dict_parsers/test_bse_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    64620 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/dict_parsers/test_groundstate_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 14:29:25.000000 excitingtools-1.7.0/tests/dict_parsers/test_gw/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-25 14:28:52.000000 excitingtools-1.7.0/tests/dict_parsers/test_gw/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17883 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/dict_parsers/test_gw/mock_gw_info_out.py
--rw-rw-rw-   0 root         (0) root         (0)     1874 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/dict_parsers/test_gw/test_gw_dos_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    16110 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/dict_parsers/test_gw/test_gw_eignvalues_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     4445 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/dict_parsers/test_gw/test_gw_eps00_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    14356 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/dict_parsers/test_gw/test_gw_info_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     4642 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/dict_parsers/test_gw/test_gw_taskgroup_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     4471 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/dict_parsers/test_gw/test_gw_vxc_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     6648 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/dict_parsers/test_input_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     8348 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/dict_parsers/test_ks_band_structure.py
--rw-rw-rw-   0 root         (0) root         (0)     1511 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/dict_parsers/test_parser_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1618 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/dict_parsers/test_properties_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    12175 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/dict_parsers/test_species_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     7410 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/dict_parsers/test_state_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 14:29:25.000000 excitingtools-1.7.0/tests/eigenstates/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-25 14:28:52.000000 excitingtools-1.7.0/tests/eigenstates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      954 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/eigenstates/test_eigenstates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 14:29:25.000000 excitingtools-1.7.0/tests/input/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-25 14:28:52.000000 excitingtools-1.7.0/tests/input/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1443 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/input/test_base_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1742 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/input/test_dynamic_class.py
--rw-rw-rw-   0 root         (0) root         (0)     8127 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/input/test_ground_state.py
--rw-rw-rw-   0 root         (0) root         (0)    10863 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/input/test_input_xml.py
--rw-rw-rw-   0 root         (0) root         (0)     7509 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/input/test_properties.py
--rw-rw-rw-   0 root         (0) root         (0)    21034 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/input/test_structure.py
--rw-rw-rw-   0 root         (0) root         (0)     1926 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/input/test_xml_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     7670 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/input/test_xs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 14:29:25.000000 excitingtools-1.7.0/tests/math/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-25 14:28:52.000000 excitingtools-1.7.0/tests/math/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      340 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/math/test_math_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 14:29:25.000000 excitingtools-1.7.0/tests/obj_parsers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-25 14:28:52.000000 excitingtools-1.7.0/tests/obj_parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3508 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/obj_parsers/test_eigenvalue_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     1861 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/obj_parsers/test_gw_dos.py
--rw-rw-rw-   0 root         (0) root         (0)     9190 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/obj_parsers/test_gw_eigenvalues.py
--rw-rw-rw-   0 root         (0) root         (0)     1606 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/obj_parsers/test_input_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 14:29:25.000000 excitingtools-1.7.0/tests/parser_utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-25 14:28:52.000000 excitingtools-1.7.0/tests/parser_utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1529 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/parser_utils/test_parser_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3176 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/parser_utils/test_regex_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2122 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/parser_utils/test_simple_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 14:29:25.000000 excitingtools-1.7.0/tests/runner/
--rw-rw-rw-   0 root         (0) root         (0)     5177 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/runner/test_runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 14:29:25.000000 excitingtools-1.7.0/tests/species/
--rw-rw-rw-   0 root         (0) root         (0)    24053 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/species/test_species_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 14:29:25.000000 excitingtools-1.7.0/tests/structure/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-25 14:28:52.000000 excitingtools-1.7.0/tests/structure/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      430 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/structure/test_ase_utilities.py
--rw-rw-rw-   0 root         (0) root         (0)     2280 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/structure/test_lattice.py
--rw-rw-rw-   0 root         (0) root         (0)     2254 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/structure/test_pymatgen_utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 14:29:25.000000 excitingtools-1.7.0/tests/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-25 14:28:52.000000 excitingtools-1.7.0/tests/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6021 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/utils/test_dict_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1255 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/utils/test_schema_parsing.py
--rw-rw-rw-   0 root         (0) root         (0)     1676 2024-03-25 14:28:51.000000 excitingtools-1.7.0/tests/utils/test_utils.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2024-04-02 20:46:36.975882 excitingtools-1.7.1/
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2024-04-02 20:46:36.941052 excitingtools-1.7.1/.github/
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2024-04-02 20:46:36.947331 excitingtools-1.7.1/.github/workflows/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      602 2024-03-26 20:55:58.000000 excitingtools-1.7.1/.github/workflows/actions.yml
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      647 2023-03-24 11:27:51.000000 excitingtools-1.7.1/.github/workflows/joss.yml
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    21948 2023-03-24 09:19:21.000000 excitingtools-1.7.1/.pylintrc
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     8901 2023-02-27 14:38:47.000000 excitingtools-1.7.1/.style.yapf
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1916 2023-02-27 14:38:47.000000 excitingtools-1.7.1/CITATION.cff
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     5375 2024-03-26 21:21:27.000000 excitingtools-1.7.1/CONTRIBUTING.md
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     7650 2024-03-26 21:21:27.000000 excitingtools-1.7.1/COPYING.LESSER
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    34915 2024-03-26 21:21:27.000000 excitingtools-1.7.1/COPYING.md
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    15768 2024-04-02 20:46:36.975539 excitingtools-1.7.1/PKG-INFO
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    14969 2024-04-02 14:35:29.000000 excitingtools-1.7.1/README.md
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2024-04-02 20:46:36.947798 excitingtools-1.7.1/excitingtools/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1398 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/__init__.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2024-04-02 20:46:36.948467 excitingtools-1.7.1/excitingtools/constants/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1729 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/constants/units.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2024-04-02 20:46:36.950297 excitingtools-1.7.1/excitingtools/dataclasses/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      163 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/dataclasses/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     5300 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/dataclasses/band_structure.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      801 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/dataclasses/data_structs.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      145 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/dataclasses/density_of_states.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     6618 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/dataclasses/eigenvalues.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2024-04-02 20:46:36.950706 excitingtools-1.7.1/excitingtools/eigenstates/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1111 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/eigenstates/eigenstates.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2024-04-02 20:46:36.954736 excitingtools-1.7.1/excitingtools/exciting_dict_parsers/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     5806 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/exciting_dict_parsers/RT_TDDFT_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-02-27 14:38:47.000000 excitingtools-1.7.1/excitingtools/exciting_dict_parsers/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     5536 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/exciting_dict_parsers/bse_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    14277 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/exciting_dict_parsers/groundstate_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     6642 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/exciting_dict_parsers/gw_eigenvalues_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     3855 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/exciting_dict_parsers/gw_eps00_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    16095 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/exciting_dict_parsers/gw_info_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     4300 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/exciting_dict_parsers/gw_taskgroup_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     3217 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/exciting_dict_parsers/gw_vxc_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     5791 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/exciting_dict_parsers/input_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     5692 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/exciting_dict_parsers/parser_factory.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    24492 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/exciting_dict_parsers/properties_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     2987 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/exciting_dict_parsers/species_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     8231 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/exciting_dict_parsers/state_parser.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2024-04-02 20:46:36.956460 excitingtools-1.7.1/excitingtools/exciting_obj_parsers/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      122 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/exciting_obj_parsers/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1370 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/exciting_obj_parsers/eigenvalue_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     4289 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/exciting_obj_parsers/gw_eigenvalues.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      631 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/exciting_obj_parsers/input_xml.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1196 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/exciting_obj_parsers/ks_band_structure.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2024-04-02 20:46:36.958277 excitingtools-1.7.1/excitingtools/input/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      673 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/input/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     2668 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/input/bandstructure.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     9320 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/input/base_class.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     4744 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/input/dynamic_class.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     4267 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/input/input_classes.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1295 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/input/input_xml.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    12841 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/input/structure.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     4547 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/input/xml_utils.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2024-04-02 20:46:36.958636 excitingtools-1.7.1/excitingtools/math/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-02-27 14:38:47.000000 excitingtools-1.7.1/excitingtools/math/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      572 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/math/math_utils.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2024-04-02 20:46:36.959688 excitingtools-1.7.1/excitingtools/parser_utils/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      113 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/parser_utils/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)       46 2023-02-27 14:38:47.000000 excitingtools-1.7.1/excitingtools/parser_utils/erroneous_file_error.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      971 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/parser_utils/grep_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     3029 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/parser_utils/parser_decorators.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     2860 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/parser_utils/parser_utils.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     2134 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/parser_utils/regex_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1591 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/parser_utils/simple_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2024-02-22 17:54:17.000000 excitingtools-1.7.1/excitingtools/py.typed
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2024-04-02 20:46:36.959905 excitingtools-1.7.1/excitingtools/runner/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-02-27 14:38:47.000000 excitingtools-1.7.1/excitingtools/runner/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     5997 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/runner/runner.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2024-04-02 20:46:36.960132 excitingtools-1.7.1/excitingtools/species/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    16367 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/species/species_file.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2024-04-02 20:46:36.960646 excitingtools-1.7.1/excitingtools/structure/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      861 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/structure/ase_utilities.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     3964 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/structure/lattice.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1528 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/structure/pymatgen_utilities.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2024-04-02 20:46:36.961808 excitingtools-1.7.1/excitingtools/utils/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-02-27 14:38:47.000000 excitingtools-1.7.1/excitingtools/utils/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     5246 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/utils/dict_utils.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      498 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/utils/jobflow_utils.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     9813 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/utils/schema_parsing.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      621 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/utils/test_utils.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     2580 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/utils/utils.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    20597 2024-04-02 14:35:29.000000 excitingtools-1.7.1/excitingtools/utils/valid_attributes.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2024-04-02 20:46:36.974639 excitingtools-1.7.1/excitingtools.egg-info/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    15768 2024-04-02 20:46:36.000000 excitingtools-1.7.1/excitingtools.egg-info/PKG-INFO
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     4944 2024-04-02 20:46:36.000000 excitingtools-1.7.1/excitingtools.egg-info/SOURCES.txt
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)        1 2024-04-02 20:46:36.000000 excitingtools-1.7.1/excitingtools.egg-info/dependency_links.txt
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)       90 2024-04-02 20:46:36.000000 excitingtools-1.7.1/excitingtools.egg-info/requires.txt
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)       14 2024-04-02 20:46:36.000000 excitingtools-1.7.1/excitingtools.egg-info/top_level.txt
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      243 2023-02-27 14:38:47.000000 excitingtools-1.7.1/git-blame-ignore-revs
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2024-04-02 20:46:36.963043 excitingtools-1.7.1/paper/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    10387 2023-03-24 09:19:21.000000 excitingtools-1.7.1/paper/joss_latex.template
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    14039 2024-03-26 20:55:58.000000 excitingtools-1.7.1/paper/latex.template
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     5301 2023-03-24 11:27:51.000000 excitingtools-1.7.1/paper/paper.bib
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     8645 2024-03-26 20:55:58.000000 excitingtools-1.7.1/paper/paper.md
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     2077 2024-04-02 14:35:29.000000 excitingtools-1.7.1/pyproject.toml
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)       81 2024-03-26 21:21:27.000000 excitingtools-1.7.1/pytest.ini
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)       33 2024-03-26 21:21:27.000000 excitingtools-1.7.1/requirements.txt
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)       38 2024-04-02 20:46:36.975931 excitingtools-1.7.1/setup.cfg
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2024-04-02 20:46:36.963470 excitingtools-1.7.1/tests/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-02-27 14:38:47.000000 excitingtools-1.7.1/tests/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      417 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/conftest.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2024-04-02 20:46:36.963994 excitingtools-1.7.1/tests/dataclasses/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-03-24 11:27:51.000000 excitingtools-1.7.1/tests/dataclasses/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     3668 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/dataclasses/test_band_structure.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     5354 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/dataclasses/test_eigenvalues.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2024-04-02 20:46:36.966269 excitingtools-1.7.1/tests/dict_parsers/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-02-27 14:38:47.000000 excitingtools-1.7.1/tests/dict_parsers/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1566 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/dict_parsers/test_RT_TDDFT_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    18022 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/dict_parsers/test_bse_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    62327 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/dict_parsers/test_groundstate_parser.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2024-04-02 20:46:36.968314 excitingtools-1.7.1/tests/dict_parsers/test_gw/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-02-27 14:38:47.000000 excitingtools-1.7.1/tests/dict_parsers/test_gw/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    17399 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/dict_parsers/test_gw/mock_gw_info_out.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     2168 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/dict_parsers/test_gw/test_gw_dos_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    16357 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/dict_parsers/test_gw/test_gw_eignvalues_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     4436 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/dict_parsers/test_gw/test_gw_eps00_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    13903 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/dict_parsers/test_gw/test_gw_info_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     4803 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/dict_parsers/test_gw/test_gw_taskgroup_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     4689 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/dict_parsers/test_gw/test_gw_vxc_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     6440 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/dict_parsers/test_input_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     8134 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/dict_parsers/test_ks_band_structure.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1536 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/dict_parsers/test_parser_factory.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1609 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/dict_parsers/test_properties_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    12740 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/dict_parsers/test_species_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     7395 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/dict_parsers/test_state_parser.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2024-04-02 20:46:36.968719 excitingtools-1.7.1/tests/eigenstates/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-03-24 11:27:51.000000 excitingtools-1.7.1/tests/eigenstates/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      939 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/eigenstates/test_eigenstates.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2024-04-02 20:46:36.970687 excitingtools-1.7.1/tests/input/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-03-25 14:39:41.000000 excitingtools-1.7.1/tests/input/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1449 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/input/test_base_class.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1843 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/input/test_dynamic_class.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     8521 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/input/test_ground_state.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    10796 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/input/test_input_xml.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     7610 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/input/test_properties.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    20903 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/input/test_structure.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1922 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/input/test_xml_utils.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     7690 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/input/test_xs.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2024-04-02 20:46:36.971237 excitingtools-1.7.1/tests/math/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-02-27 14:38:47.000000 excitingtools-1.7.1/tests/math/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      344 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/math/test_math_utils.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2024-04-02 20:46:36.972302 excitingtools-1.7.1/tests/obj_parsers/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-02-27 14:38:47.000000 excitingtools-1.7.1/tests/obj_parsers/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     3804 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/obj_parsers/test_eigenvalue_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     2154 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/obj_parsers/test_gw_dos.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     8945 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/obj_parsers/test_gw_eigenvalues.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1606 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/obj_parsers/test_input_parser.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2024-04-02 20:46:36.972877 excitingtools-1.7.1/tests/parser_utils/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-03-24 11:27:51.000000 excitingtools-1.7.1/tests/parser_utils/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1685 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/parser_utils/test_parser_utils.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     3081 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/parser_utils/test_regex_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     2070 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/parser_utils/test_simple_parser.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2024-04-02 20:46:36.973006 excitingtools-1.7.1/tests/runner/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     4959 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/runner/test_runner.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2024-04-02 20:46:36.973185 excitingtools-1.7.1/tests/species/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    24056 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/species/test_species_file.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2024-04-02 20:46:36.973747 excitingtools-1.7.1/tests/structure/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-02-27 14:38:47.000000 excitingtools-1.7.1/tests/structure/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      429 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/structure/test_ase_utilities.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     2160 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/structure/test_lattice.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     2200 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/structure/test_pymatgen_utilities.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2024-04-02 20:46:36.974286 excitingtools-1.7.1/tests/utils/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-02-27 14:38:47.000000 excitingtools-1.7.1/tests/utils/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     5471 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/utils/test_dict_utils.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1288 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/utils/test_schema_parsing.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1631 2024-04-02 14:35:29.000000 excitingtools-1.7.1/tests/utils/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `excitingtools-1.7.0/.github/workflows/actions.yml` & `excitingtools-1.7.1/.github/workflows/actions.yml`

 * *Files identical despite different names*

### Comparing `excitingtools-1.7.0/.github/workflows/joss.yml` & `excitingtools-1.7.1/.github/workflows/joss.yml`

 * *Files identical despite different names*

### Comparing `excitingtools-1.7.0/.pylintrc` & `excitingtools-1.7.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `excitingtools-1.7.0/.style.yapf` & `excitingtools-1.7.1/.style.yapf`

 * *Files identical despite different names*

### Comparing `excitingtools-1.7.0/CITATION.cff` & `excitingtools-1.7.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `excitingtools-1.7.0/CONTRIBUTING.md` & `excitingtools-1.7.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `excitingtools-1.7.0/COPYING.LESSER` & `excitingtools-1.7.1/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `excitingtools-1.7.0/COPYING.md` & `excitingtools-1.7.1/COPYING.md`

 * *Files identical despite different names*

### Comparing `excitingtools-1.7.0/PKG-INFO` & `excitingtools-1.7.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: excitingtools
-Version: 1.7.0
-Summary: Utilities for aiding in the construction of exciting inputs and the postprocessing exciting outputs.
-Author-email: Alexander Buccheri <alexander.buccheri@mpsd.mpg.de>, Fabian Peschel <peschelf@physik.hu-berlin.de>
-License: GNU GENERAL PUBLIC LICENSE, see 'COPYING.md'
-Project-URL: repository, https://github.com/exciting/excitingtools
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: schemaparsing
-License-File: COPYING.LESSER
-License-File: COPYING.md
-
 # excitingtools
 <span style="font-family:american typewriter; font-size:1em;">**excitingtools**</span> is a collection of 
 modules to facilitate the generation of <span style="font-family:american typewriter; font-size:1em;">**exciting**</span>
 inputs and the post-processing of <span style="font-family:american typewriter; font-size:1em;">**exciting**</span> outputs. 
 
 <span style="font-family:american typewriter; font-size:1em;">**excitingtools**</span> currently provides functionality for:
 
@@ -96,23 +82,34 @@
 """
 import numpy as np
 
 from excitingtools.maths.math_utils import triple_product
 ```
 Exposed modules, forming user API, should be defined in `__init__.py` where ever possible.
 
-## Code Formatting 
-We currently favour [yapf](https://github.com/google/yapf) formatter, which by default applies PEP8 formatting to 
-the code.  
+## Code Checking and Formatting 
+We currently favour the [ruff](https://github.com/astral-sh/ruff) formatter, which by default applies PEP8 formatting to 
+the code. Additional rule selection and configuration can be found in the `pyproject.toml` file.
+
+After installing ruff via pip, if you are in the root directory of excitingtools, you can simply type:
+```bash
+ruff check excitingtools/path/to/file.py
+```
+This will check the selected file for common errors. Without a path the whole project will be checked.
 
-After installing yapf, if you are in the root directory of excitingtools, you can simply type:
+Some problems can be solved automatically with enabling the `--fix` feature:
+```bash
+ruff check --fix excitingtools/path/to/file.py
+```
+Afterward, you can type
 ```bash
-yapf -i excitingtools/path/to/file.py
+ruff format excitingtools/path/to/file.py
 ```
-and it will do the formatting for you. Note: This will automatically use our custom `.style.yapf` style-file.
+and it will do the formatting for you for the selected file, or again for the whole project without an argument.
+Check out the [docs](https://docs.astral.sh/ruff/) for more options.
 
 ## Documentation 
 
 ### Writing Documentation
 All functions and classes should be documented. The favoured docstring is *reStructuredText*:
 
 ```python3
@@ -355,11 +352,12 @@
 ## Contributors
 The following people (in alphabetic order by their family names) have contributed to excitingtools:
 
 * Alexander Buccheri
 * Hannah Kleine
 * Martin Kuban
 * Benedikt Maurer
+* Ronaldo Pela
 * Fabian Peschel
 * Daniel Speckhard
 * Elisa Stephan
 * Mara Voiculescu
```

### Comparing `excitingtools-1.7.0/README.md` & `excitingtools-1.7.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: excitingtools
+Version: 1.7.1
+Summary: Utilities for aiding in the construction of exciting inputs and the postprocessing exciting outputs.
+Author-email: Alexander Buccheri <alexander.buccheri@mpsd.mpg.de>, Fabian Peschel <peschelf@physik.hu-berlin.de>
+License: GNU GENERAL PUBLIC LICENSE, see 'COPYING.md'
+Project-URL: repository, https://github.com/exciting/excitingtools
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: COPYING.LESSER
+License-File: COPYING.md
+Requires-Dist: numpy>=1.14.5
+Requires-Dist: matplotlib>=2.2.0
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: ase>=3.20.0; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+Provides-Extra: schemaparsing
+Requires-Dist: xmlschema; extra == "schemaparsing"
+
 # excitingtools
 <span style="font-family:american typewriter; font-size:1em;">**excitingtools**</span> is a collection of 
 modules to facilitate the generation of <span style="font-family:american typewriter; font-size:1em;">**exciting**</span>
 inputs and the post-processing of <span style="font-family:american typewriter; font-size:1em;">**exciting**</span> outputs. 
 
 <span style="font-family:american typewriter; font-size:1em;">**excitingtools**</span> currently provides functionality for:
 
@@ -82,23 +102,34 @@
 """
 import numpy as np
 
 from excitingtools.maths.math_utils import triple_product
 ```
 Exposed modules, forming user API, should be defined in `__init__.py` where ever possible.
 
-## Code Formatting 
-We currently favour [yapf](https://github.com/google/yapf) formatter, which by default applies PEP8 formatting to 
-the code.  
+## Code Checking and Formatting 
+We currently favour the [ruff](https://github.com/astral-sh/ruff) formatter, which by default applies PEP8 formatting to 
+the code. Additional rule selection and configuration can be found in the `pyproject.toml` file.
+
+After installing ruff via pip, if you are in the root directory of excitingtools, you can simply type:
+```bash
+ruff check excitingtools/path/to/file.py
+```
+This will check the selected file for common errors. Without a path the whole project will be checked.
 
-After installing yapf, if you are in the root directory of excitingtools, you can simply type:
+Some problems can be solved automatically with enabling the `--fix` feature:
+```bash
+ruff check --fix excitingtools/path/to/file.py
+```
+Afterward, you can type
 ```bash
-yapf -i excitingtools/path/to/file.py
+ruff format excitingtools/path/to/file.py
 ```
-and it will do the formatting for you. Note: This will automatically use our custom `.style.yapf` style-file.
+and it will do the formatting for you for the selected file, or again for the whole project without an argument.
+Check out the [docs](https://docs.astral.sh/ruff/) for more options.
 
 ## Documentation 
 
 ### Writing Documentation
 All functions and classes should be documented. The favoured docstring is *reStructuredText*:
 
 ```python3
@@ -341,11 +372,12 @@
 ## Contributors
 The following people (in alphabetic order by their family names) have contributed to excitingtools:
 
 * Alexander Buccheri
 * Hannah Kleine
 * Martin Kuban
 * Benedikt Maurer
+* Ronaldo Pela
 * Fabian Peschel
 * Daniel Speckhard
 * Elisa Stephan
 * Mara Voiculescu
```

### Comparing `excitingtools-1.7.0/excitingtools/constants/units.py` & `excitingtools-1.7.1/excitingtools/constants/units.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-""" Units.
+"""Units.
 
 Physical constants, defined according to [CODATA 2018])(http://physics.nist.gov/constants)
 One could also consider importing them from scipy
 """
+
 import enum
 
 bohr_to_angstrom = 0.529177210903
-angstrom_to_bohr = 1. / bohr_to_angstrom
+angstrom_to_bohr = 1.0 / bohr_to_angstrom
 Hartree_to_eV = 27.211396641308
 
 
 class Unit(enum.Enum):
     """
     Enum class for exciting units. All names are defined with
     as lowercase, for consistency.
 
     This could be replaced with [PINT](https://pint.readthedocs.io/en/stable/), as used by NOMAD, however it's
     currently not required. If/when we wish to do unit manipulation, it should be reconsidered.
     """
+
     hartree = enum.auto()
     inv_hartree = enum.auto()
     ev = enum.auto()
     inv_ev = enum.auto()
     kelvin = enum.auto()
     bohr = enum.auto()
     bohr_pow_3 = enum.auto()
@@ -36,25 +38,25 @@
     force = enum.auto()
     null = enum.auto()
 
 
 # Map Unit enums to strings.
 # Required because JSON cannot dump objects to file.
 enum_to_string = {
-    Unit.hartree: 'Hartree',
-    Unit.inv_hartree: '1/Hartree',
-    Unit.ev: 'eV',
-    Unit.inv_ev: 'eV^-1',
-    Unit.kelvin: 'K',
-    Unit.bohr: 'Bohr',
-    Unit.bohr_pow_3: 'Bohr^3',
-    Unit.inv_bohr: 'Bohr^-1',
-    Unit.inv_bohr_pow_3: 'Bohr^-3',
-    Unit.au: 'a.u.',
-    Unit.degrees: 'degrees',
-    Unit.GK_max: 'GK_max',
-    Unit.electron_rest_mass: 'm_electron',
-    Unit.bohr_velocity_over_bohr_radius: 'v_Bohr/r_Bohr',
-    Unit.bohr_velocity: 'Bohr/t_Bohr',
-    Unit.force: 'Hartree/Bohr', 
-    Unit.null: 'null'
+    Unit.hartree: "Hartree",
+    Unit.inv_hartree: "1/Hartree",
+    Unit.ev: "eV",
+    Unit.inv_ev: "eV^-1",
+    Unit.kelvin: "K",
+    Unit.bohr: "Bohr",
+    Unit.bohr_pow_3: "Bohr^3",
+    Unit.inv_bohr: "Bohr^-1",
+    Unit.inv_bohr_pow_3: "Bohr^-3",
+    Unit.au: "a.u.",
+    Unit.degrees: "degrees",
+    Unit.GK_max: "GK_max",
+    Unit.electron_rest_mass: "m_electron",
+    Unit.bohr_velocity_over_bohr_radius: "v_Bohr/r_Bohr",
+    Unit.bohr_velocity: "Bohr/t_Bohr",
+    Unit.force: "Hartree/Bohr",
+    Unit.null: "null",
 }
```

### Comparing `excitingtools-1.7.0/excitingtools/dataclasses/band_structure.py` & `excitingtools-1.7.1/excitingtools/dataclasses/band_structure.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,29 @@
-""" Band structure class. """
+"""Band structure class."""
+
+from typing import List, Optional, Tuple, Union
 
-from typing import Tuple, List, Optional, Union
-from excitingtools.eigenstates.eigenstates import get_k_point_index
 import numpy as np
 
+from excitingtools.eigenstates.eigenstates import get_k_point_index
+
 
 class BandData:
     ticks_and_labels = Tuple[np.ndarray, List[str]]
-    vertex_keys = ['distance', 'label', 'coord']
+    vertex_keys = ["distance", "label", "coord"]
 
-    def __init__(self,
-                 bands: np.ndarray,
-                 k_points: np.ndarray,
-                 e_fermi: float,
-                 flattened_k_points: Optional[np.ndarray] = None,
-                 vertices: Optional[List[dict]] = None):
-        """ Initialise BandData.
+    def __init__(
+        self,
+        bands: np.ndarray,
+        k_points: np.ndarray,
+        e_fermi: float,
+        flattened_k_points: Optional[np.ndarray] = None,
+        vertices: Optional[List[dict]] = None,
+    ):
+        """Initialise BandData.
 
         :param bands: Band energies with shape (n_k_points, n_bands).
         :param: k_points: k-points at which the band energies have been computed.
         :param: e_fermi: Fermi level.
         :param: flattened_k_points: Flattened k-points along which one can plot a band structure.
         :param: vertices: exciting output containing high-symmetry points and symbols along the
         flattened k-path, as defined in exciting.
@@ -30,56 +34,54 @@
         self.e_fermi = e_fermi
         self.flattened_k_points = flattened_k_points
         self.vertices = vertices
         self.xticks, self.labels = self.band_path()
         self.i_vbm, self.i_cbm = self.get_band_edges()
 
     def band_path(self) -> ticks_and_labels:
-        """ Get an array of points in the k-path that correspond to high symmetry points,
+        """Get an array of points in the k-path that correspond to high symmetry points,
         and a list of their labels.
 
         vertices expected to have the form
         [{'distance': float, 'label': str, 'coord': [float, float, float]}, ...]
         parsed from exciting's bandstructure.xml file.
 
         :return: Tuple of NumPy array containing high symmetry points and list containing their labels.
         If vertices is None, return empty containers.
         """
         if self.vertices is None:
             return np.empty(shape=1), []
 
-        assert list(self.vertices[0].keys()) == self.vertex_keys, \
-            f'Expect a vertex to have the keys {self.vertex_keys}'
+        assert list(self.vertices[0].keys()) == self.vertex_keys, f"Expect a vertex to have the keys {self.vertex_keys}"
 
         vertices = [self.vertices[0]["distance"]]
         labels = [self.vertices[0]["label"]]
 
         for i in range(1, len(self.vertices)):
             vertex = self.vertices[i]["distance"]
             label = self.vertices[i]["label"]
 
             # Handle discontinuities in the band path
             if np.isclose(vertex, vertices[-1]):
                 vertices.pop()
-                label = labels.pop() + ',' + label
+                label = labels.pop() + "," + label
 
             vertices.append(vertex)
             labels.append(label)
 
         # Replace for plotting purposes
-        unicode_gamma = '\u0393'
-        for label in ['Gamma', 'gamma', 'G']:
+        unicode_gamma = "\u0393"
+        for label in ["Gamma", "gamma", "G"]:
             labels = list(map(lambda x: x.replace(label, unicode_gamma), labels))
 
         return np.asarray(vertices), labels
 
     def get_k_point_index(self, k_point: Union[List[float], np.ndarray]) -> int:
-
         if len(k_point) != 3:
-            raise TypeError('Expected type for k-point: list or NumPy array of length 3')
+            raise TypeError("Expected type for k-point: list or NumPy array of length 3")
 
         return get_k_point_index(k_point, self.k_points, verbose=False)
 
     def get_band_edges(self) -> Tuple[int, int]:
         """Get indices of the valence and conduction bands.
 
         :return Tuple of indices for the valence and conduction bands. A ValueError is returned if the Fermi level is
@@ -92,26 +94,24 @@
 
         vbm_energy = np.amax(valence_max_energies)
         ik_vbm = np.argmax(valence_max_energies)
         n_occupied = len(np.where(self.bands[ik_vbm, :] <= vbm_energy)[0])
         i_vbm = n_occupied - 1
 
         if i_vbm + 1 >= self.n_bands:
-            raise ValueError(f'Fermi level {self.e_fermi} larger than highest band energy {np.amax(self.bands)}')
+            raise ValueError(f"Fermi level {self.e_fermi} larger than highest band energy {np.amax(self.bands)}")
 
         return i_vbm, i_vbm + 1
 
     def get_valence_band_maximum(self) -> float:
-        """Get the value of the valence band maximum.
-        """
+        """Get the value of the valence band maximum."""
         return np.amax(self.bands[:, self.i_vbm])
 
     def get_conduction_band_minimum(self) -> float:
-        """Get the value of the conduction band minimum.
-        """
+        """Get the value of the conduction band minimum."""
         return np.amin(self.bands[:, self.i_cbm])
 
     def get_fundamental_band_gap(self) -> float:
         """Get the value of the fundamental band gap.
 
         :return fundamental band gap. The band gap is set to zero if bands cross the Fermi level.
         """
@@ -121,15 +121,15 @@
 
         ik_v = np.argmax(self.bands[:, self.i_vbm])
         ik_c = np.argmin(self.bands[:, self.i_cbm])
 
         return self.bands[ik_c, self.i_cbm] - self.bands[ik_v, self.i_vbm]
 
     def get_band_gap(self, k_valence, k_conduction):
-        """ Get the value of the band gap calculated between two given k-points.
+        """Get the value of the band gap calculated between two given k-points.
 
         :param k_valence: k-point for the valence band.
         :param k_conduction: k-point for the valence band.
         :return band gap.
         """
         ik_v = self.get_k_point_index(k_valence)
         ik_c = self.get_k_point_index(k_conduction)
```

### Comparing `excitingtools-1.7.0/excitingtools/dataclasses/data_structs.py` & `excitingtools-1.7.1/excitingtools/dataclasses/data_structs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,31 @@
-""" Data Structures.
+"""Data Structures.
 
 Data structure is defined as a container for data.
 Many of these classes could be @dataclass, however excitingtools
 retains support for python 3.6.
 """
 
+
 class PointIndex:
-    """ Container for (point, index) pair
-    """
+    """Container for (point, index) pair"""
+
     def __init__(self, point, index: int):
         self.point = point
         self.index = index
 
+
 class BandIndices:
     """Indices of valence band maximum and conduction band minimum"""
+
     def __init__(self, VBM: int, CBm: int):
         self.VBM = VBM
         self.CBm = CBm
 
+
 class NumberOfStates:
-    """Number of states. Useful when indexing does not start at 0/1
-    """
+    """Number of states. Useful when indexing does not start at 0/1"""
+
     def __init__(self, first_state: int, last_state: int):
         self.first_state = first_state
         self.last_state = last_state
         self.n_states = last_state - first_state + 1
```

### Comparing `excitingtools-1.7.0/excitingtools/dataclasses/eigenvalues.py` & `excitingtools-1.7.1/excitingtools/dataclasses/eigenvalues.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,81 +1,84 @@
-""" Eigenvalue class.
-"""
+"""Eigenvalue class."""
+
 import warnings
 from itertools import permutations
-from typing import List, Union, Optional
+from typing import List, Optional, Union
 
 import numpy as np
-from excitingtools.dataclasses.data_structs import PointIndex, BandIndices, NumberOfStates
+
+from excitingtools.dataclasses.data_structs import BandIndices, NumberOfStates, PointIndex
 
 
 class EigenValues:
     point_type = Union[np.ndarray, List[float]]
     index_type = Union[np.ndarray, List[int]]
     # If a k-index is not matched
     NO_MATCH = -1
 
-    def __init__(self,
-                 state_range: NumberOfStates,
-                 k_points: point_type,
-                 k_indices: index_type,
-                 all_eigenvalues: np.ndarray,
-                 weights=None,
-                 occupations: Optional[np.ndarray] = None):
+    def __init__(
+        self,
+        state_range: NumberOfStates,
+        k_points: point_type,
+        k_indices: index_type,
+        all_eigenvalues: np.ndarray,
+        weights=None,
+        occupations: Optional[np.ndarray] = None,
+    ):
         self.state_range = state_range
         self.k_points = k_points
         self.k_indices = k_indices
         self.all_eigenvalues = all_eigenvalues
         self.weights = weights
         self.occupations = occupations
         if all_eigenvalues.shape != (len(self.k_points), self.state_range.n_states):
-            raise ValueError('Shape of all_eigenvalues does not match (n_k, n_states)')
+            raise ValueError("Shape of all_eigenvalues does not match (n_k, n_states)")
 
     def get_array_index(self, i_state: int):
-        """ Given the state index, get the corresponding index in the eigenvalue array.
+        """Given the state index, get the corresponding index in the eigenvalue array.
 
         :param i_state: State index using fortran indexing
         :return array index, using zero-indexing
         """
         assert i_state > 0, "state indexing starts at 1"
         return i_state - self.state_range.first_state
 
     def get_k_point(self, ik: int):
-        """ Get the k-point associated with ik index.
+        """Get the k-point associated with ik index.
 
         :param ik: k-point index.
         :return k-point in fractional coordinates.
         """
         assert ik > 0, "ik indexing starts at 1"
         return self.k_points[ik - 1]
 
     def get_index(self, k_point, verbose=False) -> int:
-        """ Find the corresponding index of a k-point.
+        """Find the corresponding index of a k-point.
 
         If no k-point is found, NO_MATCH is returned.
 
         :param k_point: k-point in fractional coordinates.
         :param verbose: Print warning, if no k-point found.
         :return ik: Corresponding index w.r.t. exciting.
         """
         diff = np.empty(shape=len(self.k_points))
         k_point = np.asarray(k_point)
         for i, point in enumerate(self.k_points):
             diff[i] = np.linalg.norm(np.asarray(point) - k_point)
-        indices = np.argwhere(diff < 1.e-8)
+        indices = np.argwhere(diff < 1.0e-8)
 
         if len(indices) == 0:
             if verbose:
-                warnings.warn(f'{k_point} not present in list of k-points')
+                warnings.warn(f"{k_point} not present in list of k-points")
             return self.NO_MATCH
 
         indices = indices[0]
 
         if len(indices) > 1:
-            raise ValueError(f'Found degenerate k-points at {indices}')
+            raise ValueError(f"Found degenerate k-points at {indices}")
 
         ik = indices[0] + 1
         return ik
 
     def get_k_points(self) -> List[PointIndex]:
         """K-points and their indices
 
@@ -92,42 +95,42 @@
 
         :param ik: k-point index.
         :param k_point: k-point, used to find the k-index if ik is not passed.
         :return eigenvalues at ik k-point.
         """
         if ik is None:
             if k_point is None:
-                raise ValueError('Must provide either k-index or k-point')
+                raise ValueError("Must provide either k-index or k-point")
             ik = self.get_index(k_point)
 
             if ik == self.NO_MATCH:
                 return np.empty(shape=0)
 
         return self.all_eigenvalues[ik - 1, :]
 
     def band_gap(self, band_indices: BandIndices, k_points=None, k_indices=None) -> Union[float, ValueError]:
-        """ Get a band gap for two k-points in the valence band top
+        """Get a band gap for two k-points in the valence band top
         and conduction band bottom, respectively.
 
         TODO(Alex) Consider adding objects to hold k_points and k_indices.
         However, one can retain support for tuples/lists.
 
         :param band_indices: Band indices
         :param k_points: k-points for the valence and conduction bands, in that order.
         :param k_indices: k-indices for the valence and conduction bands, in that order.
         :return Band gap. A ValueError is returned if one or both k-points are not present.
         """
         if k_indices is None:
             if k_points is None:
-                raise ValueError('Must pass either k_points or k_indices to band_gap method')
+                raise ValueError("Must pass either k_points or k_indices to band_gap method")
             k_indices = (self.get_index(k_points[0]), self.get_index(k_points[1]))
 
         if self.NO_MATCH in k_indices:
             indices = np.argwhere(k_indices == self.NO_MATCH)[0]
-            err_msg = f"".join(f'Requested k-point {k_points[i]} not present. \n' for i in indices)
+            err_msg = "".join(f"Requested k-point {k_points[i]} not present. \n" for i in indices)
             return ValueError(err_msg)
 
         i_vbm = self.get_array_index(band_indices.VBM)
         i_cbm = self.get_array_index(band_indices.CBm)
 
         ik_vbm = k_indices[0] - 1
         ik_cbm = k_indices[1] - 1
@@ -145,20 +148,19 @@
         :param conduction_k_point: k-point for conduction band in fractional coordinates.
         :return: Transition energy in Hartree.
         """
         indices_valence = [self.get_index(k_point) for k_point in permutations(valence_k_point)]
         try:
             ik = next(i for i in indices_valence if i != self.NO_MATCH)
         except StopIteration:
-            raise ValueError(f'Requested valence k-point {valence_k_point} not present.')
+            raise ValueError(f"Requested valence k-point {valence_k_point} not present.")
 
         indices_conduction = [self.get_index(k_point) for k_point in permutations(conduction_k_point)]
         try:
             jk = next(i for i in indices_conduction if i != self.NO_MATCH)
         except StopIteration:
-            raise ValueError(f'Requested conduction k-point {conduction_k_point} not present.')
+            raise ValueError(f"Requested conduction k-point {conduction_k_point} not present.")
 
         iVBM = np.where(self.occupations[ik - 1] == 0)[0][0] + self.state_range.first_state - 1
         jCBm = np.where(self.occupations[jk - 1] == 0)[0][0] + self.state_range.first_state
 
         return self.band_gap(BandIndices(iVBM, jCBm), k_indices=[ik, jk])
-
```

### Comparing `excitingtools-1.7.0/excitingtools/eigenstates/eigenstates.py` & `excitingtools-1.7.1/excitingtools/eigenstates/eigenstates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-""" Function for finding the corresponding index of a k-point.
-"""
-import numpy as np
+"""Function for finding the corresponding index of a k-point."""
+
 import warnings
 
+import numpy as np
+
 
 def get_k_point_index(k_point: np.ndarray, k_points_to_search: np.ndarray, verbose=False) -> int:
-    """ Find the corresponding index of a k-point.
+    """Find the corresponding index of a k-point.
 
     If no k-point is found, NO_MATCH is returned.
 
     :param k_point: k-point in fractional coordinates.
     :param k_points_to_search: Array of k-points in which k_point is searched for
     :param verbose: Print warning, if no k-point found.
     :return ik: Corresponding index w.r.t. exciting.
     """
-    NO_MATCH = np.NaN
+    NO_MATCH = np.nan
 
     diff = np.empty(shape=len(k_points_to_search))
     k_point = np.asarray(k_point)
     for i, point in enumerate(k_points_to_search):
         diff[i] = np.linalg.norm(np.asarray(point) - k_point)
-    indices = np.argwhere(diff < 1.e-8)
+    indices = np.argwhere(diff < 1.0e-8)
 
     if len(indices) == 0:
         if verbose:
-            warnings.warn(f'{k_point} not present in list of k-points')
+            warnings.warn(f"{k_point} not present in list of k-points")
         return NO_MATCH
 
     if len(indices) > 1:
-        raise ValueError(f'Found degenerate k-points at {indices}'.replace('\n', ','))
+        raise ValueError(f"Found degenerate k-points at {indices}".replace("\n", ","))
 
     ik = indices[0]
     return ik
```

### Comparing `excitingtools-1.7.0/excitingtools/exciting_dict_parsers/RT_TDDFT_parser.py` & `excitingtools-1.7.1/excitingtools/exciting_dict_parsers/RT_TDDFT_parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,68 @@
 """
 Parsers for real-time TDDFT output files
 """
+
+from typing import List
 from xml.etree.ElementTree import ParseError
+
 import numpy as np
-from typing import List
 
 from excitingtools.parser_utils.grep_parser import grep
 
 
 def parse_nexc(name, skiprows=1):
     """
     Parser for NEXC.OUT
     """
     try:
         data = np.genfromtxt(name, skip_header=skiprows)
-    except:
+    except Exception:
         raise ParseError
     out = {
         "Time": data[:, 0],
         "number_electrons_GroundState": data[:, 1],
         "number_electrons_ExcitedState": data[:, 2],
-        "sum": data[:, 3]
+        "sum": data[:, 3],
     }
 
     return out
 
 
 def parse_jind(name, skiprows=0):
     """
     Parser for JIND.OUT
     """
     try:
         data = np.genfromtxt(name, skip_header=skiprows)
-    except:
+    except Exception:
         raise ParseError
-    out = {
-        "Time": data[:, 0],
-        "Jx": data[:, 1],
-        "Jy": data[:, 2],
-        "Jz": data[:, 3]
-    }
+    out = {"Time": data[:, 0], "Jx": data[:, 1], "Jy": data[:, 2], "Jz": data[:, 3]}
 
     return out
 
 
 def parse_etot(name):
     """
     Parser for ETOT_RTTDDFT.OUT
     """
     try:
         data = np.genfromtxt(name, skip_header=1)
-    except:
+    except Exception:
         raise ParseError
     out = {
         "Time": data[:, 0],
         "ETOT": data[:, 1],
         "Madelung": data[:, 2],
         "Eigenvalues-Core": data[:, 3],
         "Eigenvalues-Valence": data[:, 4],
         "Exchange": data[:, 5],
         "Correlation": data[:, 6],
         "XC-potential": data[:, 7],
-        "Coulomb pot. energy": data[:, 8]
+        "Coulomb pot. energy": data[:, 8],
     }
 
     return out
 
 
 def parse_eigval_screenshots(name: str) -> dict:
     """
@@ -94,136 +91,128 @@
           k_blocks[1]['end']   = line 75  i.e.   38      8.808472531393
 
 
         Default line indexing starts at 0.
         """
 
         # Lines for which a new k-point block starts
-        raw_k_point_lines = grep("ik", name, options={'n': ''}).splitlines()
-        k_point_lines = [int(line.split(':')[0]) for line in raw_k_point_lines]
+        raw_k_point_lines = grep("ik", name, options={"n": ""}).splitlines()
+        k_point_lines = [int(line.split(":")[0]) for line in raw_k_point_lines]
 
         if fortran_index:
             offset = 1
         else:
             # Python indexing
             offset = 0
             k_point_lines = [int(i) - 1 for i in k_point_lines]
 
         n_lines = sum(1 for line in open(name)) + offset
 
         k_blocks = []
         k_start = 0 + offset
         for ik in k_point_lines[1:]:
             k_end = ik - 2
-            k_blocks.append({'start': k_start, 'end': k_end})
+            k_blocks.append({"start": k_start, "end": k_end})
             k_start = k_end + 2
 
         # Account for final k-block
-        k_blocks.append({'start': k_start, 'end': n_lines - 2})
+        k_blocks.append({"start": k_start, "end": n_lines - 2})
 
         return k_blocks
 
     k_blocks = get_k_point_blocks(name)
 
     # Parse file
-    with open(name, 'r') as f:
+    with open(name) as f:
         file = f.readlines()
 
     data = {}
     kpoints = []
     for indices in k_blocks:
         kpoint = {}
-        ik = int(file[indices['start']].split()[-1])
-        eigenvalues = [
-            float(file[i].split()[-1])
-            for i in range(indices['start'] + 1, indices['end'] + 1)
-        ]
-        kpoint['ik'] = ik
-        kpoint['eigenvalues'] = eigenvalues
+        ik = int(file[indices["start"]].split()[-1])
+        eigenvalues = [float(file[i].split()[-1]) for i in range(indices["start"] + 1, indices["end"] + 1)]
+        kpoint["ik"] = ik
+        kpoint["eigenvalues"] = eigenvalues
         kpoints.append(kpoint)
 
-    data['kpoints'] = kpoints
+    data["kpoints"] = kpoints
 
     return data
 
 
 def parse_proj_screenshots(name: str) -> dict:
     """
     Parser for PROJ_*.OUT.
 
     Effectively the same code as parse_eigval_screenshots, but the whitespace
     between blocks differs by 1.
     """
 
-    raw_k_point_lines = grep("ik", name, options={'n': ''}).splitlines()
-    k_point_lines = [int(line.split(':')[0]) - 1 for line in raw_k_point_lines]
+    raw_k_point_lines = grep("ik", name, options={"n": ""}).splitlines()
+    k_point_lines = [int(line.split(":")[0]) - 1 for line in raw_k_point_lines]
     last_line = sum(1 for line in open(name))
 
     k_blocks = []
     k_start = 0
     for ik in k_point_lines[1:]:
         k_end = ik
         k_blocks.append([k_start, k_end])
         k_start = k_end
     k_blocks.append([k_end, last_line])
 
     # Parse file
     with open(name) as f:
         file = f.readlines()
 
-    data = {'ik': [], 'projection': []}
+    data = {"ik": [], "projection": []}
     for i in k_blocks:
         start = i[0]
         end = i[1]
         ik = int(file[start].split()[-1])
-        projection = []
-        for j in range(start + 1, end):
-            projection.append([float(x) for x in file[j].split()])
-        data['ik'].append(ik)
-        data['projection'].append(np.asarray(projection))
+        projection = [[float(x) for x in file[j].split()] for j in range(start + 1, end)]
+        data["ik"].append(ik)
+        data["projection"].append(np.asarray(projection))
     return data
 
+
 def parse_atom_position_velocity_force(name: str) -> dict:
-    """ Parser for ATOM_????.OUT 
+    """Parser for ATOM_????.OUT
     :param str name: name of file to parse
     :return dict out: each dict key corresponds to time, position (3 columns), velocity (3 columns), total force (3 columns).
     The 3 columns refer to the x, y, z components
     """
     try:
         data = np.genfromtxt(name, skip_header=0)
-    except:
+    except Exception:
         raise ParseError
     out = {
         "Time": data[:, 0],
         "x": data[:, 1],
         "y": data[:, 2],
         "z": data[:, 3],
         "vx": data[:, 4],
         "vy": data[:, 5],
         "vz": data[:, 6],
         "Fx": data[:, 7],
         "Fy": data[:, 8],
-        "Fz": data[:, 9]
+        "Fz": data[:, 9],
     }
 
     return out
 
+
 def parse_force(name, skiprows=0):
     """
     Parser for X_????.OUT, where X can be:
     - FCR: core corrections to forces
     - FEXT: external forces (due to e.g. an electric field)
     - FHF: Hellman-Feynman term of forces
     - FVAL: valence corrections to forces
     """
     try:
         data = np.genfromtxt(name, skip_header=skiprows)
-    except:
+    except Exception:
         raise ParseError
-    out = {
-        "Time": data[:, 0],
-        "Fx": data[:, 1],
-        "Fy": data[:, 2],
-        "Fz": data[:, 3]
-    }
+    out = {"Time": data[:, 0], "Fx": data[:, 1], "Fy": data[:, 2], "Fz": data[:, 3]}
 
-    return out
+    return out
```

### Comparing `excitingtools-1.7.0/excitingtools/exciting_dict_parsers/bse_parser.py` & `excitingtools-1.7.1/excitingtools/exciting_dict_parsers/bse_parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-"""Parsers for BSE output files.
-"""
+"""Parsers for BSE output files."""
+
 import re
 from typing import Optional
 
 import numpy as np
 
 
 def numpy_gen_from_txt(name: str, skip_header: Optional[int] = 0) -> np.ndarray:
-    """  Numpy genfromtxt, dressed in try/expect.
+    """Numpy genfromtxt, dressed in try/expect.
 
     Not worth generalising, as would need to support genfromtxt's API.
 
     :param name: File name.
     :param skip_header: Optional number of header lines to skip.
     :return data: Parsed data.
     """
     try:
         data = np.genfromtxt(name, skip_header=skip_header)
     except ValueError:
-        raise ValueError(f'Failed to parse {name}')
+        raise ValueError(f"Failed to parse {name}")
     return data
 
 
 def parse_EPSILON_NAR(name: str) -> dict:
     """
     Parser for:
         EPSILON_NAR_BSE-singlet-TDA-BAR_SCR-full_OC.OUT.xml,
@@ -31,31 +31,27 @@
         LOSS_NAR_FXCMB1_OC_QMT001.OUT.xml
     """
     data = numpy_gen_from_txt(name, skip_header=14)
     out = {
         "frequency": data[:, 0],
         "real_oscillator_strength": data[:, 1],
         "imag_oscillator_strength": data[:, 2],
-        "real_oscillator_strength_kkt": data[:, 3]
+        "real_oscillator_strength_kkt": data[:, 3],
     }
     return out
 
 
 def parse_LOSS_NAR(name):
     """
     Parser for:
      LOSS_NAR_FXCMB1_OC_QMT001.OUT.xml,
      LOSS_NAR_NLF_FXCMB1_OC_QMT001.OUT.xml
     """
     data = numpy_gen_from_txt(name, skip_header=14)
-    out = {
-        "frequency": data[:, 0],
-        "real_oscillator_strength": data[:, 1],
-        "imag_oscillator_strength": data[:, 2]
-    }
+    out = {"frequency": data[:, 0], "real_oscillator_strength": data[:, 1], "imag_oscillator_strength": data[:, 2]}
 
     return out
 
 
 def parse_EXCITON_NAR_BSE(name):
     """
     Parser for EXCITON_NAR_BSE-singlet-TDA-BAR_SCR-full_OC.OUT
@@ -80,79 +76,71 @@
     and
         'EXCITING <version> stopped for task <tasknumber>'
     See example file: exciting/test/test_farm/BSE/PBE_SOL-LiF/ref/INFOXS.OUT
     If a started task is found, it gets stored with name, number and status.
     If the task is found to be finished afterwards, the status finished is set to True.
 
     For success, the last started tasks has to be finished after that (in the file).
-    Last finished task is the last task if calculation was successful, the task before that 
+    Last finished task is the last task if calculation was successful, the task before that
     if it finished, else None.
     :param name: path of the file to parse
     :param parse_timing: parse also timing information for the tasks. By default this is set to
                          False. If the task has not finished None is returned as timing.
     :returns: dictionary containing parsed file
     """
     with open(name) as file:
         lines = file.readlines()
 
     tasks = []
     current_task = -1
 
     lines = "\n".join(lines)
-    all_tasks = re.findall(r'EXCITING .* (started) for task (.*) \( ?(\d+)\)|'
-                           r'EXCITING .* stopped for task .* (\d+)', lines)
+    all_tasks = re.findall(
+        r"EXCITING .* (started) for task (.*) \( ?(\d+)\)|EXCITING .* stopped for task .* (\d+)", lines
+    )
 
     for task in all_tasks:
-        if task[0] == 'started':
-            tasks.append({
-                'name': task[1],
-                'number': int(task[2]),
-                'finished': False
-            })
+        if task[0] == "started":
+            tasks.append({"name": task[1], "number": int(task[2]), "finished": False})
             current_task += 1
         else:
             # asserts shouldn't happen with Exciting:
-            assert tasks != [], 'No tasks started!'
-            assert tasks[current_task]['number'] == int(task[3]), 'Wrong task stopped.'
-            tasks[current_task]['finished'] = True
+            assert tasks, "No tasks started!"
+            assert tasks[current_task]["number"] == int(task[3]), "Wrong task stopped."
+            tasks[current_task]["finished"] = True
 
-    success = tasks[-1]['finished']
+    success = tasks[-1]["finished"]
     last_finished_task = None
     if success:
-        last_finished_task = tasks[-1]['name']
-    elif len(tasks) > 1 and tasks[-2]['finished']:
-        last_finished_task = tasks[-2]['name']
+        last_finished_task = tasks[-1]["name"]
+    elif len(tasks) > 1 and tasks[-2]["finished"]:
+        last_finished_task = tasks[-2]["name"]
 
     if parse_timing:
         times = parse_times(lines)
-        finished_tasks = [task for task in tasks if task['finished']]
-        assert len(times['cpu']) == len(finished_tasks), 'Numbers of finished tasks and parsed times are not the same.'
+        finished_tasks = [task for task in tasks if task["finished"]]
+        assert len(times["cpu"]) == len(finished_tasks), "Numbers of finished tasks and parsed times are not the same."
 
         for index, task in enumerate(finished_tasks):
-            task['cpu_time'] = float(times['cpu'][index])
-            task['wall_time'] = float(times['wall'][index])
-            task['cpu_time_cum'] = float(times['cpu_cum'][index])
-            task['wall_time_cum'] = float(times['wall_cum'][index])
-    
-    return {'tasks': tasks,
-            'success': success,
-            'last_finished_task': last_finished_task}
+            task["cpu_time"] = float(times["cpu"][index])
+            task["wall_time"] = float(times["wall"][index])
+            task["cpu_time_cum"] = float(times["cpu_cum"][index])
+            task["wall_time_cum"] = float(times["wall_cum"][index])
+
+    return {"tasks": tasks, "success": success, "last_finished_task": last_finished_task}
 
 
 def parse_times(infoxs_string: str) -> dict:
     """Parse the run times in INFOXS.OUT for each task.
     :param infoxs_string: String that contains the INFOXS.OUT file.
     :returns: dictionary containing a list of run times for each measurement.
     """
-    cpu_times = re.findall(r'CPU time \s*: ([\d\.\d]+) sec', infoxs_string)
-    wall_times = re.findall(r'wall time \s*: ([\d\.\d]+) sec', infoxs_string)
-    cpu_times_cum = re.findall(r'CPU time \s* \(cumulative\) \s*: ([\d\.\d]+) sec', infoxs_string)
-    wall_times_cum = re.findall(r'wall time \(cumulative\) \s*: ([\d\.\d]+) sec', infoxs_string)
-
-    assert len(cpu_times) == len(wall_times), 'Numbers of parsed timings are not consistent.'
-    assert len(cpu_times) == len(cpu_times_cum), 'Numbers of parsed timings are not consistent.'
-    assert len(cpu_times) == len(wall_times_cum), 'Numbers of parsed timings are not consistent.'
-    
-    return {'cpu': cpu_times, 
-            'wall': wall_times,
-            'cpu_cum': cpu_times_cum,
-            'wall_cum': wall_times_cum}
+    cpu_times = re.findall(r"CPU time \s*: ([\d\.\d]+) sec", infoxs_string)
+    wall_times = re.findall(r"wall time \s*: ([\d\.\d]+) sec", infoxs_string)
+    cpu_times_cum = re.findall(r"CPU time \s* \(cumulative\) \s*: ([\d\.\d]+) sec", infoxs_string)
+    wall_times_cum = re.findall(r"wall time \(cumulative\) \s*: ([\d\.\d]+) sec", infoxs_string)
+
+    assert len(cpu_times) == len(wall_times), "Numbers of parsed timings are not consistent."
+    assert len(cpu_times) == len(cpu_times_cum), "Numbers of parsed timings are not consistent."
+    assert len(cpu_times) == len(wall_times_cum), "Numbers of parsed timings are not consistent."
+
+    return {"cpu": cpu_times, "wall": wall_times, "cpu_cum": cpu_times_cum, "wall_cum": wall_times_cum}
```

### Comparing `excitingtools-1.7.0/excitingtools/exciting_dict_parsers/groundstate_parser.py` & `excitingtools-1.7.1/excitingtools/exciting_dict_parsers/groundstate_parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Ground state file parsers.
 
 All functions in this module could benefit from refactoring.
 """
+
 import re
 import xml.etree.ElementTree as ET
 
 import numpy as np
 
 from excitingtools.parser_utils.erroneous_file_error import ErroneousFileError
-from excitingtools.parser_utils.parser_decorators import xml_root, set_return_values
+from excitingtools.parser_utils.parser_decorators import set_return_values, xml_root
 
 
 @set_return_values
-def parse_info_out(name: str) -> dict:
+def parse_info_out(name: str) -> dict:  # noqa: PLR0912, PLR0915
     """
     Parser exciting INFO.OUT into a dictionary.
     In:
         name     string     path of the file to parse
     Out:
         info     dict       contains the content of the file to parse
     """
@@ -26,120 +27,117 @@
 
     nscl = []
     nini = []
 
     # Get line numbers for SCF iteration blocks
     for i, line in enumerate(lines):
         # stores the number of the first and last line of every iteration into a list
-        if ('SCF iteration number' in line) or ('Hybrids iteration number'in line) \
-           or ('Reached self-consistent loops maximum' in line):
+        if (
+            ("SCF iteration number" in line)
+            or ("Hybrids iteration number" in line)
+            or ("Reached self-consistent loops maximum" in line)
+        ):
             nscl.append(i)
-        if ('Convergency criteria checked for the last'
-            in line) or ('Self-consistent loop stopped' in line):
+        if ("Convergency criteria checked for the last" in line) or ("Self-consistent loop stopped" in line):
             nscl.append(i)
         # stores the number of the first and last line of the initialization into a list
-        if 'Starting initialization' in line:
+        if "Starting initialization" in line:
             nini.append(i + 2)
-        if 'Ending initialization' in line:
+        if "Ending initialization" in line:
             nini.append(i - 2)
 
     calculation_failed = True
     for line in reversed(lines):
         if ("EXCITING" in line) and ("stopped" in line):
             calculation_failed = False
             break
 
     if calculation_failed:
         raise ErroneousFileError()
 
     INFO = {}
-    INFO['initialization'] = {}
+    INFO["initialization"] = {}
     ini = []
     inits = {}
     k = 0
     speci = 0  # variable to detect different species in INFO.OUT
 
     # loops through all lines of the initialization
     for i in range(nini[0], nini[1]):
         # stores the lines, which have the format "variable : value" into a list
-        if (':' in lines[i]):
-            lines[i] = lines[i].split(':')
+        if ":" in lines[i]:
+            lines[i] = lines[i].split(":")
             ini.append(lines[i])
-            if ini[k][0][1] != ' ' and speci != 0:  # if indentation stops, species part is ended
+            if ini[k][0][1] != " " and speci != 0:  # if indentation stops, species part is ended
                 speci = 0
 
             ini[k][0] = ini[k][0].strip()
             ini[k][1] = ini[k][1].strip()
-            if ('Lattice vectors'
-                in ini[k][0]) or ('Reciprocal lattice vectors'
-                                  in ini[k][0]):
+            if ("Lattice vectors" in ini[k][0]) or ("Reciprocal lattice vectors" in ini[k][0]):
                 ini[k][1] = []
-                lines[i + 1] = (lines[i + 1].split())
-                lines[i + 2] = (lines[i + 2].split())
-                lines[i + 3] = (lines[i + 3].split())
+                lines[i + 1] = lines[i + 1].split()
+                lines[i + 2] = lines[i + 2].split()
+                lines[i + 3] = lines[i + 3].split()
                 for j in range(3):
                     ini[k][1].append(lines[i + 1][j])
                     ini[k][1].append(lines[i + 2][j])
                     ini[k][1].append(lines[i + 3][j])
-                if ' ' in ini[k][1]:
+                if " " in ini[k][1]:
                     ini[k][1] = ini[k][1].split()
 
             # initialize species subdict if key Species is found:
-            if ini[k][0] == 'Species':
+            if ini[k][0] == "Species":
                 speci = ini[k][1][0]
                 speci_name = ini[k][1][3:-1]
-                inits.update({'Species ' + speci: {'Species symbol': speci_name}})
+                inits.update({"Species " + speci: {"Species symbol": speci_name}})
 
             # stores variable-value pairs in a dictionary, in species subdict if necessary
             if speci != 0:
-                if ini[k][0][:16] == 'atomic positions':
+                if ini[k][0][:16] == "atomic positions":
                     split_key = ini[k][0].split()
                     unit = split_key[2][1:-1]
-                    inits['Species ' + speci].update({'Atomic positions': {}})
+                    inits["Species " + speci].update({"Atomic positions": {}})
                 else:
                     try:
-                        key_name = 'Atom ' + str(int(ini[k][0]))
-                        inits['Species ' + speci]['Atomic positions'].update({key_name: ini[k][1]})
+                        key_name = "Atom " + str(int(ini[k][0]))
+                        inits["Species " + speci]["Atomic positions"].update({key_name: ini[k][1]})
                     except ValueError:
-                        inits['Species ' + speci].update({ini[k][0]: ini[k][1]})
+                        inits["Species " + speci].update({ini[k][0]: ini[k][1]})
             else:
                 inits.update({ini[k][0]: ini[k][1]})
             k = k + 1
         # type of mixing is stored in the dictionary too
-        if 'mixing' in lines[i]:
+        if "mixing" in lines[i]:
             lines[i] = lines[i].strip()
-            inits.update({'mixing': lines[i]})
-    inits.update({'units': {'positions': unit}})
+            inits.update({"mixing": lines[i]})
+    inits.update({"units": {"positions": unit}})
 
-    INFO['initialization'] = inits
+    INFO["initialization"] = inits
 
-    scl1 = []
-    INFO['scl'] = {}
+    INFO["scl"] = {}
 
     # loops through all scl's
     for j in range(len(nscl) - 1):
         scls = {}
         scl = []
         k = 0
         # loops through all lines of the scl
         for i in range(nscl[j], nscl[j + 1]):
             # stores the lines, which have the format "variable : value" into a list
-            if (':' in lines[i]) and ('+'
-                                      not in lines[i]) and ('(target)'
-                                                            not in lines[i]):
-                lines[i] = lines[i].split(':')
+            if (":" in lines[i]) and ("+" not in lines[i]) and ("(target)" not in lines[i]):
+                lines[i] = lines[i].split(":")
                 scl.append(lines[i])
                 scl[k][0] = scl[k][0].strip()
                 scl[k][1] = scl[k][1].strip()
-                if ' ' in scl[k][1]:
+                if " " in scl[k][1]:
                     scl[k][1] = scl[k][1].split()
                 # stores variable-value pairs in a dictionary
                 scls.update({scl[k][0]: scl[k][1]})
                 k = k + 1
-        INFO['scl'][str(j + 1)] = scls
+        INFO["scl"][str(j + 1)] = scls
 
     return INFO
 
 
 @set_return_values
 def parse_info_xml(name) -> dict:
     """
@@ -150,222 +148,219 @@
         info     dict       contains the content of the file to parse
     """
     try:
         root = ET.parse(name)
     except AttributeError:
         raise ErroneousFileError
 
-    info = root.find('groundstate').attrib
+    info = root.find("groundstate").attrib
 
     excitingRun = []
     i = 0
-    for node in root.find('groundstate').find('scl').iter('iter'):
+    for node in root.find("groundstate").find("scl").iter("iter"):
         excitingRun.append(node.attrib)
-        excitingRun[i]['energies'] = node.find('energies').attrib
-        excitingRun[i]['charges'] = node.find('charges').attrib
-        atom_nr = 0
+        excitingRun[i]["energies"] = node.find("energies").attrib
+        excitingRun[i]["charges"] = node.find("charges").attrib
         atomic_charge = []
         species = []
-        for atoms in node.find('charges').iter('atom'):
-            if atom_nr == 0: species_old = atoms.get('species')
-            atom_nr = atom_nr + 1
-            if atoms.get('species') == species_old:
-                species.append({'muffin-tin': atoms.get('muffin-tin')})
+        for atom_nr, atoms in enumerate(node.find("charges").iter("atom")):
+            if atom_nr == 0:
+                species_old = atoms.get("species")
+            if atoms.get("species") == species_old:
+                species.append({"muffin-tin": atoms.get("muffin-tin")})
             else:
-                species_old = atoms.get('species')
+                species_old = atoms.get("species")
                 atomic_charge.append(species)
-                species = [{'muffin-tin': atoms.get('muffin-tin')}]
+                species = [{"muffin-tin": atoms.get("muffin-tin")}]
                 atomic_charge.append(species)
-                excitingRun[i]['charges']['atomic'] = atomic_charge
-                excitingRun[i]['timing'] = node.find('timing').attrib
-        if node.find('moments') is not None:
-            moments = {}
-            moments['momtot'] = node.find('moments').find('momtot').attrib
-            moments['interstitial'] = node.find('moments').find(
-                'momtot').attrib
-            moments['mommttot'] = node.find('moments').find(
-                'interstitial').attrib
-            excitingRun[i]['moments'] = moments
+                excitingRun[i]["charges"]["atomic"] = atomic_charge
+                excitingRun[i]["timing"] = node.find("timing").attrib
+        if node.find("moments") is not None:
+            moments = {
+                "momtot": node.find("moments").find("momtot").attrib,
+                "interstitial": node.find("moments").find("momtot").attrib,
+                "mommttot": node.find("moments").find("interstitial").attrib,
+            }
+            excitingRun[i]["moments"] = moments
             atom_nr = 0
             atomic_moment = []
             species = []
-            for atoms in node.find('moments').iter('atom'):
-                if atom_nr == 0: species_old = atoms.get('species')
-                atom_nr = atom_nr + 1
-                if atoms.get('species') == species_old:
-                    species.append(atoms.find('mommt').attrib)
+            for atoms in node.find("moments").iter("atom"):
+                if atom_nr == 0:
+                    species_old = atoms.get("species")
+                atom_nr += 1
+                if atoms.get("species") == species_old:
+                    species.append(atoms.find("mommt").attrib)
                 else:
-                    species_old = atoms.get('species')
+                    species_old = atoms.get("species")
                     atomic_moment.append(species)
-                    species = [atoms.find('mommt').attrib]
+                    species = [atoms.find("mommt").attrib]
                     atomic_moment.append(species)
-                    excitingRun[i]['moments']['atomic'] = atomic_moment
+                    excitingRun[i]["moments"]["atomic"] = atomic_moment
         i = i + 1
-    info['scl'] = {}
+    info["scl"] = {}
     for item in excitingRun:  # converts list of scl-iterations into a dictionary
-        name = item['iteration']
-        info['scl'][name] = item
+        name = item["iteration"]
+        info["scl"][name] = item
 
     return info
 
 
 @set_return_values
 def parse_atoms(name) -> dict:
-    """                                                                                                  
-    Parser exciting atoms.xml into a python dictionary.                                                   
-    In:                                                                                                  
-        name     string     path of the file to parse                                                    
-    Out:                                                                                                 
-        info     dict       contains the content of the file to parse                                    
+    """
+    Parser exciting atoms.xml into a python dictionary.
+    In:
+        name     string     path of the file to parse
+    Out:
+        info     dict       contains the content of the file to parse
     """
 
     root = ET.parse(name)
     atoms = {}
-    atoms['Hamiltonian'] = root.find('Hamiltonian').attrib
+    atoms["Hamiltonian"] = root.find("Hamiltonian").attrib
     atom = []
     i = 0
-    for node in root.findall('atom'):
+    for node in root.findall("atom"):
         atom.append(node.attrib)
 
-        spectrum = []
-        states = node.find('spectrum')
-        for state in states.findall('state'):
-            spectrum.append(state.attrib)
+        states = node.find("spectrum")
+        spectrum = [state.attrib for state in states.findall("state")]
 
-        atom[i]['NumericalSetup'] = node.find('NumericalSetup').attrib
-        atom[i]['spectrum'] = {}
+        atom[i]["NumericalSetup"] = node.find("NumericalSetup").attrib
+        atom[i]["spectrum"] = {}
         j = 0
         for item in spectrum:  # converts list of states into a dictionary
             name = str(j)
-            atom[i]['spectrum'][name] = item
+            atom[i]["spectrum"][name] = item
             j = j + 1
         i = i + 1
-    atoms['atom'] = {}
+    atoms["atom"] = {}
     for item in atom:  # converts list of atoms into a dictionary
-        name = item['chemicalSymbol']
-        atoms['atom'][name] = item
+        name = item["chemicalSymbol"]
+        atoms["atom"][name] = item
 
     return atoms
 
 
 @set_return_values
 @xml_root
 def parse_eigval(root) -> dict:
-    """ Parse eigenvalues from eigval.xml file.
+    """Parse eigenvalues from eigval.xml file.
 
     :param root: XML file name, XML string or ElementTree.Element as input.
     :return: dict output: Parsed data.
     """
     eigval = root.attrib
 
     kpts = []
-    for node in root.findall('kpt'):
+    for node in root.findall("kpt"):
         kpt = node.attrib
         state = []
         for subnode in node:
             state.append(subnode.attrib)
-            kpt['state'] = {}  # converts list of states into a dictionary
+            kpt["state"] = {}  # converts list of states into a dictionary
         for item in state:
-            name = item['ist']
-            kpt['state'][name] = item
+            name = item["ist"]
+            kpt["state"][name] = item
             kpts.append(kpt)
-            eigval['kpt'] = {}
+            eigval["kpt"] = {}
     for item in kpts:  # converts list of kpts into a dictionary
-        name = item['ik']
-        eigval['kpt'][name] = item
+        name = item["ik"]
+        eigval["kpt"][name] = item
 
     return eigval
 
 
 @set_return_values
 def parse_evalcore(name) -> dict:
-    """                                                                                                  
-    Parser exciting evalcore.xml into a python dictionary.                                                   
-    In:                                                                                                  
-        name     string     path of the file to parse                                                    
-    Out:                                                                                                 
-        info     dict       contains the content of the file to parse                                    
+    """
+    Parser exciting evalcore.xml into a python dictionary.
+    In:
+        name     string     path of the file to parse
+    Out:
+        info     dict       contains the content of the file to parse
     """
 
     root = ET.parse(name).getroot()
     evalcore = root.attrib
 
     speciess = []
-    for node in root.findall('species'):
+    for node in root.findall("species"):
         species = node.attrib
         atoms = []
         for subnode in node:
             atom = subnode.attrib
             states = []
             for subnode1 in subnode:
                 state = subnode1.attrib
                 states.append(state)
-            atom['state'] = {}
+            atom["state"] = {}
             for item in states:  # converts list of states into a dictionary
-                name = item['ist']
-                atom['state'][name] = item
+                name = item["ist"]
+                atom["state"][name] = item
             atoms.append(atom)
-            species['atom'] = {}
+            species["atom"] = {}
             for item in atoms:  # converts list of atoms into a dictionary
-                name = item['ia']
-                species['atom'][name] = item
+                name = item["ia"]
+                species["atom"][name] = item
         speciess.append(species)
-    evalcore['species'] = {}
+    evalcore["species"] = {}
     for item in speciess:  # converts list of species into a dictionary
-        name = item['chemicalSymbol']
-        evalcore['species'][name] = item
+        name = item["chemicalSymbol"]
+        evalcore["species"][name] = item
 
     return evalcore
 
 
 @set_return_values
 def parse_geometry(name) -> dict:
-    """                                                                                                  
-    Parser exciting geometry.xml into a python dictionary.                                                   
-    In:                                                                                                  
-        name     string     path of the file to parse                                                    
-    Out:                                                                                                 
-        info     dict       contains the content of the file to parse                                    
+    """
+    Parser exciting geometry.xml into a python dictionary.
+    In:
+        name     string     path of the file to parse
+    Out:
+        info     dict       contains the content of the file to parse
     """
 
     root = ET.parse(name).getroot()
-    structure = root.find('structure').attrib
-    crystal = root.find('structure').find('crystal').attrib
-    geometry = {'structure': structure}
-    structure['crystal'] = crystal
+    structure = root.find("structure").attrib
+    crystal = root.find("structure").find("crystal").attrib
+    geometry = {"structure": structure}
+    structure["crystal"] = crystal
     speciess = []
-    for node in root.find('structure').findall('species'):
+    for node in root.find("structure").findall("species"):
         species = node.attrib
         atoms = []
         for subnode in node:
             atom = subnode.attrib
             atoms.append(atom)
-            species['atom'] = {}
+            species["atom"] = {}
         i = 1
         for item in atoms:
             name = str(i)
-            species['atom'][name] = item['coord'].split()
+            species["atom"][name] = item["coord"].split()
             i = i + 1
         speciess.append(species)
-    structure['species'] = {}
+    structure["species"] = {}
     j = 1
     for item in speciess:
         name = str(j)
-        structure['species'][name] = item
+        structure["species"][name] = item
         j = j + 1
 
     basevects = []
-    for node in root.find('structure').find('crystal').findall('basevect'):
+    for node in root.find("structure").find("crystal").findall("basevect"):
         basevect = node.text
         basevects.append(basevect)
-        structure['crystal']['basevect'] = {}
+        structure["crystal"]["basevect"] = {}
         k = 1
     for item in basevects:
         name = str(k)
-        structure['crystal']['basevect'][name] = item
+        structure["crystal"]["basevect"][name] = item
         k = k + 1
     return geometry
 
 
 @set_return_values
 def parse_linengy(name: str) -> dict:
     """
@@ -373,71 +368,64 @@
 
     :param name: path of the file to parse
     :returns: dictionary containing parsed file
     """
 
     linengy = {}
 
-    with open(file=name, mode='r') as fid:
+    with open(file=name) as fid:
         lines = fid.readlines()
 
     apw_line = []
     lo_line = []
 
     for i, line in enumerate(lines):
-        if 'APW functions' in line:
+        if "APW functions" in line:
             apw_line.append(i)
-        if 'local-orbital functions' in line:
+        if "local-orbital functions" in line:
             lo_line.append(i)
 
     apw_line.append(len(lines))
 
-    for i in range(0, len(lo_line)):
+    for i in range(len(lo_line)):
         linengy[str(i)] = {}
-        apw = []
-        lo = []
 
-        for j in range(apw_line[i], lo_line[i]):
-            if "l =" in lines[j]:
-                apw.append(lines[j].split(':')[1].strip())
-        linengy[str(i)]['apw'] = apw
-
-        for j in range(lo_line[i], apw_line[i+1]):
-            if "l =" in lines[j]:
-                lo.append(lines[j].split(':')[1].strip())
-        linengy[str(i)]['lo'] = lo
+        apw = [lines[j].split(":")[1].strip() for j in range(apw_line[i], lo_line[i]) if "l =" in lines[j]]
+        linengy[str(i)]["apw"] = apw
+
+        lo = [lines[j].split(":")[1].strip() for j in range(lo_line[i], apw_line[i + 1]) if "l =" in lines[j]]
+        linengy[str(i)]["lo"] = lo
 
     return linengy
 
 
 @set_return_values
 def parse_lo_recommendation(name: str) -> dict:
     """
     Parser for: LO_RECOMMENDATION.OUT
 
     :param name: path of the file to parse
-    :returns: dictionary containing parsed file                                                                                                  
+    :returns: dictionary containing parsed file
     """
-    with open(file=name, mode='r') as fid:
+    with open(file=name) as fid:
         lines = fid.readlines()
 
-    n_species = int(lines[2].split(':')[1])
-    n_l_channels = int(lines[3].split(':')[1])
-    n_nodes = int(lines[4].split(':')[1])
+    n_species = int(lines[2].split(":")[1])
+    n_l_channels = int(lines[3].split(":")[1])
+    n_nodes = int(lines[4].split(":")[1])
 
-    lo_recommendation = {'n_species': n_species, 'n_l_channels': n_l_channels, 'n_nodes': n_nodes}
+    lo_recommendation = {"n_species": n_species, "n_l_channels": n_l_channels, "n_nodes": n_nodes}
 
-    blocks = lines[6 :]
+    blocks = lines[6:]
     block_size = n_nodes + 3
     n_blocks = n_l_channels * n_species
 
-    for iblock in range(0, n_blocks):
+    for iblock in range(n_blocks):
         offset = iblock * block_size
-        matches = re.findall(r':\s(.*?)(?:,|$)', blocks[offset+0])
+        matches = re.findall(r":\s(.*?)(?:,|$)", blocks[offset + 0])
         species, l = matches[0], int(matches[1])
-        # Package (node, n, energy) as one likes                                                                                        
-        if not species in lo_recommendation:
+        # Package (node, n, energy) as one likes
+        if species not in lo_recommendation:
             lo_recommendation.update({species: {}})
-        lo_recommendation[species].update({l: np.loadtxt(blocks[offset+2:offset+n_nodes+2]).tolist()})
+        lo_recommendation[species].update({l: np.loadtxt(blocks[offset + 2 : offset + n_nodes + 2]).tolist()})
 
     return lo_recommendation
-
```

### Comparing `excitingtools-1.7.0/excitingtools/exciting_dict_parsers/gw_eigenvalues_parser.py` & `excitingtools-1.7.1/excitingtools/exciting_dict_parsers/gw_eigenvalues_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-""" Parse GW's EVALQP.DAT file into dicts.
+"""Parse GW's EVALQP.DAT file into dicts.
 Also seemed like a logical place to add the Fermi-level parser.
 """
+
 import enum
+import os
+import re
 from itertools import count
+
 import numpy as np
-import re
-import os
 
 from excitingtools.dataclasses.data_structs import NumberOfStates
 
-
 # GW eigenvalue file name
-_file_name = 'EVALQP.DAT'
+_file_name = "EVALQP.DAT"
 
 
 def parse_efermi_gw(name: str) -> dict:
-    """ Parser for EFERMI_GW.OUT.
+    """Parser for EFERMI_GW.OUT.
 
     :param name: File name
     :return data: GW Fermi level.
     """
     data = {}
     try:
         data["EFERMI_GW"] = np.genfromtxt(name)
@@ -33,22 +34,19 @@
 
     These *can*  differ from those reported in 'KPOINTS', depending
     on the choice of ngridq in GW
 
     :param file_string: File string.
     :return k_points: k-points and their weights.
     """
-    k_points_raw: list = re.findall(r'\s*k-point .*$', file_string, flags=re.MULTILINE)
+    k_points_raw: list = re.findall(r"\s*k-point .*$", file_string, flags=re.MULTILINE)
     k_points = {}
     for ik, line in enumerate(k_points_raw):
         kx, ky, kz, w = line.split()[-4:]
-        k_points[ik + 1] = {
-            'k_point': [float(k) for k in [kx, ky, kz]],
-            'weight': float(w)
-        }
+        k_points[ik + 1] = {"k_point": [float(k) for k in [kx, ky, kz]], "weight": float(w)}
     return k_points
 
 
 def n_states_from_evalqp(file_string: str) -> NumberOfStates:
     return n_states_from_file(file_string, n_header=2)
 
 
@@ -64,18 +62,16 @@
 
     :param str file_string: Input string.
     :param n_header Number of header lines.
     :return int n_states: Number of states per k-point (occupied plus empty).
     """
     lines = file_string.splitlines()
 
-    # ibgw = first_state
     first_state = int(lines[n_header].split()[0])
 
-    # nbgw = last_state
     last_state = None
     for line in reversed(lines):
         if len(line.strip()) > 0:
             last_state = int(line.split()[0])
             break
 
     assert last_state is not None, "Index of final state to have GW correct applied not found"
@@ -122,17 +118,15 @@
     blank_line = 1
 
     data = {}
     skip_lines = header_size
 
     # Must iterate lowest to highest, else data won't match k-points
     for ik in range(1, len(k_points) + 1):
-        block_data = np.loadtxt(full_file_name,
-                                skiprows=skip_lines,
-                                max_rows=n_states)
+        block_data = np.loadtxt(full_file_name, skiprows=skip_lines, max_rows=n_states)
         # Ignore first column (state index)
         data[ik] = block_data[:, 1:]
         skip_lines += n_states + (header_size + blank_line)
 
     return data
 
 
@@ -164,46 +158,44 @@
     eval_indexing: NumberOfStates = n_states_from_evalqp(file_string)
     k_points = k_points_from_evalqp(file_string)
 
     # Uses np to parse, hence easier to pass file name here
     energies = parse_evalqp_blocks(full_file_name, k_points, eval_indexing.n_states)
     assert len(k_points) == len(energies), "Should be a set of energies for each k-point"
 
-    data = {'state_range': [eval_indexing.first_state, eval_indexing.last_state],
-            'column_labels': parse_column_labels(file_string)}
+    data = {
+        "state_range": [eval_indexing.first_state, eval_indexing.last_state],
+        "column_labels": parse_column_labels(file_string),
+    }
 
     # Repackage energies with their respective k-points
     for ik in range(1, len(k_points) + 1):
-        data[ik] = {
-            'k_point': k_points[ik]['k_point'],
-            'weight': k_points[ik]['weight'],
-            'energies': energies[ik]
-        }
+        data[ik] = {"k_point": k_points[ik]["k_point"], "weight": k_points[ik]["weight"], "energies": energies[ik]}
     return data
 
 
 def parse_column_labels(file_string: str) -> enum.Enum:
-    """ Parse the column labels of EVALQP.DAT, which vary between code versions.
+    """Parse the column labels of EVALQP.DAT, which vary between code versions.
 
     :param str file_string: Input string
     return An enum class with the column labels as attributes, with corresponding
     values starting from 0.
     """
     column_str = file_string.splitlines()[1:2][0]
     column_labels = column_str.split()[1:]
     # zip and count ensure enum indexing starts at 0
-    return enum.Enum(value='EvalQPColumns', names=zip(column_labels, count()))
+    return enum.Enum(value="EvalQPColumns", names=zip(column_labels, count()))
 
 
 def parse_gw_dos(full_file_name: str) -> dict:
     """Parser for GW DOS files.
 
     :param full_file_name: Path + file name
     :return dict data: Parsed energies and DOS from GW DOS files
     """
-    valid_file_names = ['TDOS.OUT', 'TDOS-QP.OUT']
-    path, file_name = os.path.split(full_file_name)
+    valid_file_names = ["TDOS.OUT", "TDOS-QP.OUT"]
+    _, file_name = os.path.split(full_file_name)
     if file_name not in valid_file_names:
-        raise ValueError(f'{file_name} not a valid DOS file name.')
+        raise ValueError(f"{file_name} not a valid DOS file name.")
 
     data = np.genfromtxt(full_file_name)
-    return {'energy': data[:, 0], 'dos': data[:, 1]}
+    return {"energy": data[:, 0], "dos": data[:, 1]}
```

### Comparing `excitingtools-1.7.0/excitingtools/exciting_dict_parsers/gw_eps00_parser.py` & `excitingtools-1.7.1/excitingtools/exciting_dict_parsers/gw_eps00_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-"""Parsers for GW's EPS00_GW.OUT output.
-"""
+"""Parsers for GW's EPS00_GW.OUT output."""
+
 import numpy as np
 
 from excitingtools.parser_utils.parser_decorators import accept_file_name
 from excitingtools.utils.utils import get_new_line_indices
 
 # Output file name
-_file_name = 'EPS00_GW.OUT'
+_file_name = "EPS00_GW.OUT"
 
 
 def parse_eps00_frequencies(file_string: str) -> dict:
     """Parse frequencies from EPS00_GW.OUT.
 
     :param str file_string: Input string
     :return dict frequencies: Dictionary of frequencues {index: frequency}
@@ -21,15 +21,15 @@
     # Start file_lines on first block header
     file_lines = file_string.splitlines()
     file = file_lines[initial_header_size:]
     n_freq = int(len(file) / block_size)
 
     frequencies = {}
     j = 0
-    for i in range(0, n_freq):
+    for i in range(n_freq):
         j = i * block_size
         frequencies[i + 1] = float(file[j].split()[-1])
 
     assert len(frequencies) == n_freq
 
     return frequencies
 
@@ -55,57 +55,55 @@
 
     :param str file_string: Input string
     :param int n_freq: Number of frequency points
     :return dict data: Dict containing real and imaginary parts of the dielectric function,
      eps00, for each frequency point. Frequency indexing (keys) start at 1.
     """
     line = get_new_line_indices(file_string)
-    assert file_string[line[0]:line[1]].isspace(), (
-        "First line of EPS00_GW.OUT must be a whiteline")
+    assert file_string[line[0] : line[1]].isspace(), "First line of EPS00_GW.OUT must be a whiteline"
 
     initial_header = 3
     offset = initial_header - 1
     # Header lines + eps00
     repeat_block_size = 6
 
     data = {}
     file_string = file_string.splitlines()[initial_header:]
 
     def extract_eps_i(line: str) -> tuple:
         eps_i_re = np.array(line.split()[0:3], dtype=float)
         eps_i_img = np.array(line.split()[3:6], dtype=float)
         return eps_i_re, eps_i_img
 
-    for i_freq in range(0, n_freq):
+    for i_freq in range(n_freq):
         i = offset + i_freq * repeat_block_size
 
         eps_x_re, eps_x_img = extract_eps_i(file_string[i])
         eps_y_re, eps_y_img = extract_eps_i(file_string[i + 1])
         eps_z_re, eps_z_img = extract_eps_i(file_string[i + 2])
 
         data[i_freq + 1] = {
-            're': np.array([eps_x_re, eps_y_re, eps_z_re]),
-            'img': np.array([eps_x_img, eps_y_img, eps_z_img])
+            "re": np.array([eps_x_re, eps_y_re, eps_z_re]),
+            "img": np.array([eps_x_img, eps_y_img, eps_z_img]),
         }
 
     return data
 
 
 @accept_file_name
 def parse_eps00_gw(file_string: str) -> dict:
-    """ Parser frequency grid and epsilon00 from EPS00_GW.OUT.
+    """Parser frequency grid and epsilon00 from EPS00_GW.OUT.
 
     :param str file_string: Input string
     :return dict data: Dict containing the frequency, and real and imaginary parts
      of the dielectric function, eps00, for each frequency point.
     """
     frequencies = parse_eps00_frequencies(file_string)
     eps00 = parse_eps00_blocks(file_string, len(frequencies))
-    assert len(frequencies) == len(eps00), \
-        "Expect eps00 to have n frequencies consistent with the frequency grid"
+    assert len(frequencies) == len(eps00), "Expect eps00 to have n frequencies consistent with the frequency grid"
 
     # Repackage frequency points and eps00 together
     data = {}
     for i_freq in range(1, len(frequencies) + 1):
-        data[i_freq] = {'frequency': frequencies[i_freq], 'eps00': eps00[i_freq]}
+        data[i_freq] = {"frequency": frequencies[i_freq], "eps00": eps00[i_freq]}
 
     return data
```

### Comparing `excitingtools-1.7.0/excitingtools/exciting_dict_parsers/gw_info_parser.py` & `excitingtools-1.7.1/excitingtools/exciting_dict_parsers/gw_info_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-""" GW_INFO.OUT Parser, and all sub-block parses that comprise it.
+"""GW_INFO.OUT Parser, and all sub-block parses that comprise it.
 
 NOTE. This could be trivialised to one line if GW_INFO.OUT was refactored
 to write to YAML.
 """
-import numpy as np
-from typing import List, Union
-import sys
+
 import copy
 import re
+import sys
+import warnings
+from typing import List, Union
+
+import numpy as np
 
 from excitingtools.parser_utils.parser_decorators import accept_file_name
 from excitingtools.parser_utils.regex_parser import parse_value_regex, parse_values_regex
-from excitingtools.parser_utils.simple_parser import match_current_return_line_n, match_current_extract_from_line_n
+from excitingtools.parser_utils.simple_parser import match_current_extract_from_line_n, match_current_return_line_n
 from excitingtools.utils.utils import can_be_float
 
 # Info file name for GW
 _file_name = "GW_INFO.OUT"
 
 
 def parse_correlation_self_energy_params(file_string: str) -> dict:
@@ -25,64 +28,63 @@
     specified extraction behaviour given by `keys_extractions`.
 
     Also extract the analytic continuation and singularity schemes, plus their references.
 
     :param str file_string: Input string
     :return dict data: Matched data
     """
-    keys_extractions = {'Solution of the QP equation': lambda x: int(x.split()[0]),
-                        'Energy alignment': lambda x: int(x.split()[0]),
-                        'Analytic continuation method': lambda x: x.strip(),
-                        'Scheme to treat singularities': lambda x: x.strip()
-                        }
+    keys_extractions = {
+        "Solution of the QP equation": lambda x: int(x.split()[0]),
+        "Energy alignment": lambda x: int(x.split()[0]),
+        "Analytic continuation method": lambda x: x.strip(),
+        "Scheme to treat singularities": lambda x: x.strip(),
+    }
 
     data = match_current_extract_from_line_n(file_string, keys_extractions)
 
     # Also extract citations
     def ref_after_citation(x: str) -> str:
         """
         Expected format is
         Citation: Paper reference
         """
         try:
             i = x.index(":")
-            return x[i + 1:].strip()
+            return x[i + 1 :].strip()
         except ValueError:
-            return 'Not found'
+            return "Not found"
 
     # Extraction of citations after
-    for key in ['Analytic continuation method', 'Scheme to treat singularities']:
+    for key in ["Analytic continuation method", "Scheme to treat singularities"]:
         citation_extraction = {key: ref_after_citation}
         matched_dictionary = match_current_extract_from_line_n(file_string, citation_extraction, n_line=2)
-        data[key + ' citation'] = matched_dictionary[key]
+        data[key + " citation"] = matched_dictionary[key]
 
     return data
 
 
 def parse_mixed_product_params(file_string: str) -> dict:
     """Parse mixed product basis parameters.
 
     :param str file_string: Input string
     :return dict data: Matched data
     """
     search_keys = [
-        'Angular momentum cutoff:', 'Linear dependence tolerance factor:',
-        'Plane wave cutoff \\(in units of Gkmax\\):'
+        "Angular momentum cutoff:",
+        "Linear dependence tolerance factor:",
+        "Plane wave cutoff \\(in units of Gkmax\\):",
     ]
 
     data = parse_values_regex(file_string, search_keys)
 
     # Rename keys to give better context
     modified_data = {
-        'MT Angular momentum cutoff':
-        data['Angular momentum cutoff'],
-        'MT Linear dependence tolerance factor':
-        data['Linear dependence tolerance factor'],
-        'Plane wave cutoff (in units of Gkmax)':
-        data['Plane wave cutoff (in units of Gkmax)']
+        "MT Angular momentum cutoff": data["Angular momentum cutoff"],
+        "MT Linear dependence tolerance factor": data["Linear dependence tolerance factor"],
+        "Plane wave cutoff (in units of Gkmax)": data["Plane wave cutoff (in units of Gkmax)"],
     }
 
     return modified_data
 
 
 def parse_bare_coulomb_potential_params(file_string: str) -> dict:
     """Extract bare Coulomb parameter data of the form:
@@ -100,75 +102,76 @@
       'MB tolerance factor': 0.1
     }
 
     :param str file_string: Input string
     :return dict data: Matched data
     """
 
-    pw_cutoff_matching_str = 'Plane wave cutoff \\(in units of Gkmax\\*input%gw%MixBasis%gmb\\):'
+    pw_cutoff_matching_str = "Plane wave cutoff \\(in units of Gkmax\\*input%gw%MixBasis%gmb\\):"
     pw_cutoff = list(parse_value_regex(file_string, pw_cutoff_matching_str).values())
     assert len(pw_cutoff) == 1, "Matched plane wave cutoff is ambiguous - more than one match"
 
     # Defined with less-verbose key
-    data = {'Plane wave cutoff (in units of Gkmax*gmb)': float(pw_cutoff[0])}
+    data = {"Plane wave cutoff (in units of Gkmax*gmb)": float(pw_cutoff[0])}
 
-    data2 = parse_value_regex(file_string, 'Error tolerance for structure constants:')
+    data2 = parse_value_regex(file_string, "Error tolerance for structure constants:")
 
-    data3 = parse_value_regex(file_string, 'the eigenvectors of the bare Coulomb potential:')
+    data3 = parse_value_regex(file_string, "the eigenvectors of the bare Coulomb potential:")
 
     # Defined with less-verbose key (see docs above for full key, over 2 lines)
-    modified_data3 = {'MB tolerance factor': data3.pop('the eigenvectors of the bare Coulomb potential')}
+    modified_data3 = {"MB tolerance factor": data3.pop("the eigenvectors of the bare Coulomb potential")}
 
     return {**data, **data2, **modified_data3}
 
 
 def parse_mixed_product_wf_info(file_string: str) -> dict:
     """Parse mixed product wave function information.
 
     :param str file_string: Input string
     :return dict data: Matched data
     """
     wf_info_keys = [
-        'Maximal number of MT wavefunctions per atom:',
-        'Total number of MT wavefunctions:',
-        'Maximal number of PW wavefunctions:',
-        'Total number of mixed-product wavefunctions:'
+        "Maximal number of MT wavefunctions per atom:",
+        "Total number of MT wavefunctions:",
+        "Maximal number of PW wavefunctions:",
+        "Total number of mixed-product wavefunctions:",
     ]
 
     return parse_values_regex(file_string, wf_info_keys)
 
 
 def parse_frequency_grid_info(file_string: str) -> dict:
     """Parse frequency grid information.
 
     :param str file_string: Input string
     :return dict data: Matched data
     """
-    fgrid_keys = ['Type: < fgrid >',
-                  'Frequency axis: < fconv >',
-                  'Number of frequencies: < nomeg >',
-                  'Cutoff frequency: < freqmax >'
-                  ]
+    fgrid_keys = [
+        "Type: < fgrid >",
+        "Frequency axis: < fconv >",
+        "Number of frequencies: < nomeg >",
+        "Cutoff frequency: < freqmax >",
+    ]
 
     return parse_values_regex(file_string, fgrid_keys)
 
 
 def parse_frequency_grid(file_string: str, n_points: int) -> np.ndarray:
     """Parse the frequency grid and weights used with GW
 
     :param str file_string: Input string
     :param int n_points: Number of frequency grid points
     :return np.ndarray grid_and_weights: Frequency grid and weights in grid[0, :] and grid[1, :],
     respectively
     """
-    index = file_string.find('frequency list: < #    freqs    weight >')
-    frequency_lines = file_string[index:].split('\n')
+    index = file_string.find("frequency list: < #    freqs    weight >")
+    frequency_lines = file_string[index:].split("\n")
 
     grid_and_weights = np.empty(shape=(2, n_points))
-    for i in range(0, n_points):
+    for i in range(n_points):
         index, frequency, weight = frequency_lines[i + 1].split()
         grid_and_weights[0:2, i] = np.array([float(frequency), float(weight)])
 
     return grid_and_weights
 
 
 def parse_ks_eigenstates(file_string: str) -> dict:
@@ -176,51 +179,48 @@
     Note, final keys will have the trailing whitespace stripped.
 
     :param str file_string: Input string
     :return dict data: Matched data
     """
 
     # Trailing whitespace in some instances required for match
-    ks_eigenstates_keys = ['Maximum number of LAPW states:',
-                           'Minimal number of LAPW states:',
-                           '- total KS',
-                           '- occupied',
-                           '- unoccupied ',
-                           '- dielectric function',
-                           '- self energy',
-                           'Energy of the highest unoccupied state: ',
-                           'Number of valence electrons:',
-                           'Number of valence electrons treated in GW: '
-                           ]
+    ks_eigenstates_keys = [
+        "Maximum number of LAPW states:",
+        "Minimal number of LAPW states:",
+        "- total KS",
+        "- occupied",
+        "- unoccupied ",
+        "- dielectric function",
+        "- self energy",
+        "Energy of the highest unoccupied state: ",
+        "Number of valence electrons:",
+        "Number of valence electrons treated in GW: ",
+    ]
 
     data = parse_values_regex(file_string, ks_eigenstates_keys)
 
     # Prepend keys that lack context, such as '- total KS'
     modified_data = {}
     prepend_str = "Number of states used in GW"
 
     for key, value in data.items():
-        if key[0] == '-':
-            new_key = prepend_str + " " + key.rstrip().rstrip(':')
-        else:
-            new_key = key.rstrip().rstrip(':')
+        new_key = prepend_str + " " + key.rstrip().rstrip(":") if key[0] == "-" else key.rstrip().rstrip(":")
         modified_data[new_key] = value
 
     return modified_data
 
 
 def parse_n_q_point_cycles(file_string: str) -> int:
     """Get the maximum number of q iterations performed.
 
     :param str file_string: Input string
     :return int n_q_cycles:  maximum nunber of q iterations performed
     """
-    matches = re.findall('\\(task_gw\\): q-point cycle, iq =' + '(.+?)\n',
-                         file_string)
-    n_q_cycles = max([int(string.strip()) for string in matches])
+    matches = re.findall("\\(task_gw\\): q-point cycle, iq =" + "(.+?)\n", file_string)
+    n_q_cycles = max(int(string.strip()) for string in matches)
     return n_q_cycles
 
 
 def extract_kpoint(file_string: str) -> dict:
     """Parse the substring of the form:
 
      at k =    0.000   0.500   0.500 ik =     3
@@ -235,27 +235,26 @@
     :return dict k_data: Matched data, of the form documented
     """
 
     def parse_k_match(file_string: str, key: str) -> dict:
         data = {}
 
         try:
-            match = re.search(key + '(.+?)\n', file_string)
+            match = re.search(key + "(.+?)\n", file_string)
             k_point_and_index = match.group(1).split()
-            data = {'k_point': [float(k) for k in k_point_and_index[:3]],
-                    'ik': int(k_point_and_index[-1])}
+            data = {"k_point": [float(k) for k in k_point_and_index[:3]], "ik": int(k_point_and_index[-1])}
 
         except AttributeError:
             raise AttributeError("extract_kpoint. Did not find the key", match)
 
         return data
 
-    k_data = parse_k_match(file_string, 'at k      =    ')
+    k_data = parse_k_match(file_string, "at k      =    ")
 
-    return {'VBM': k_data, 'CBm': k_data}
+    return {"VBM": k_data, "CBm": k_data}
 
 
 def extract_kpoints(file_string: str) -> dict:
     """Parse the substring of the form:
 
      at k(VBM) =    0.000   0.500   0.500 ik =     3
         k(CBm) =    0.000   0.000   0.000 ik =     1
@@ -269,35 +268,31 @@
     :param str file_string: Input string
     :return dict k_data: Matched data, of the form documented
     """
 
     def parse_k_match(file_string: str, key: str) -> dict:
         data = {}
 
-        match_key_to_parser_key = {
-            'at k\\(VBM\\) = ': 'VBM',
-            'k\\(CBm\\) = ': 'CBm'
-        }
+        match_key_to_parser_key = {"at k\\(VBM\\) = ": "VBM", "k\\(CBm\\) = ": "CBm"}
 
+        match = re.search(key + "(.+?)\n", file_string)
         try:
-            match = re.search(key + '(.+?)\n', file_string)
-            parser_key = match_key_to_parser_key[key].replace('\\', "")
+            parser_key = match_key_to_parser_key[key].replace("\\", "")
             k_point_and_index = match.group(1).split()
-            data[parser_key] = {'k_point': [float(k) for k in k_point_and_index[:3]],
-                                'ik': int(k_point_and_index[-1])}
+            data[parser_key] = {"k_point": [float(k) for k in k_point_and_index[:3]], "ik": int(k_point_and_index[-1])}
 
         except AttributeError:
-            print("extract_kpoints. Did not find the key", match)
+            warnings.warn(f"extract_kpoints. Did not find the key {match}")
 
         return data
 
-    k_data = parse_k_match(file_string, 'at k\\(VBM\\) = ')
-    k_data2 = parse_k_match(file_string, 'k\\(CBm\\) = ')
+    k_data = parse_k_match(file_string, "at k\\(VBM\\) = ")
+    k_data2 = parse_k_match(file_string, "k\\(CBm\\) = ")
 
-    return {** k_data, **k_data2}
+    return {**k_data, **k_data2}
 
 
 def parse_band_structure_info(file_string: str, bs_type: str) -> dict:
     """Parse KS or GW band structure information.
 
     This routine assumes that the KS band structure info will ALWAYS appear
     before the GW band structure info.
@@ -317,52 +312,44 @@
       Direct BandGap (eV):                      2.3903
       at k      =    0.000   0.000   0.000 ik =     1
 
     :param str bs_type: Band structure type to parse. Either 'ks' or 'gw'
     :param str file_string: Input string
     :return dict k_data: Matched data
     """
-    if bs_type == 'ks':
+    if bs_type == "ks":
         # Parse first instance of each key, exploiting that Kohn-Sham band structure
         # comes before G0W0 band structure. This ASSUMES fixed structure to the file
         pass
 
-    elif bs_type == 'gw':
+    elif bs_type == "gw":
         # Find G0W0 band structure in the file, then start parsing from there
-        gw_header = ' G0W0 band structure '
-        index = file_string.find('G0W0 band structure ')
+        gw_header = "G0W0 band structure "
+        index = file_string.find(gw_header)
         file_string = file_string[index:]
 
     else:
         sys.exit("bs_type must be 'ks' or 'gw'")
 
     # Indirect BandGap may not be present
-    band_structure_keys = ['Fermi energy:',
-                           'Energy range:',
-                           'Band index of VBM:',
-                           'Band index of CBm:']
+    band_structure_keys = ["Fermi energy:", "Energy range:", "Band index of VBM:", "Band index of CBm:"]
 
     data = parse_values_regex(file_string, band_structure_keys)
 
     # Only present if there's an indirect gap
-    indirect_gap = parse_value_regex(file_string,
-                                     'Indirect BandGap \\(eV\\):',
-                                     silent_key_error=True)
+    indirect_gap = parse_value_regex(file_string, "Indirect BandGap \\(eV\\):", silent_key_error=True)
 
     if indirect_gap:
-        direct_gap_keys = [
-            'Direct Bandgap at k\\(VBM\\) \\(eV\\):',
-            'Direct Bandgap at k\\(CBm\\) \\(eV\\):'
-        ]
+        direct_gap_keys = ["Direct Bandgap at k\\(VBM\\) \\(eV\\):", "Direct Bandgap at k\\(CBm\\) \\(eV\\):"]
         data.update(indirect_gap)
         data.update(parse_values_regex(file_string, direct_gap_keys))
         k_point_data = extract_kpoints(file_string)
 
     else:
-        data.update(parse_value_regex(file_string, 'Direct BandGap \\(eV\\):'))
+        data.update(parse_value_regex(file_string, "Direct BandGap \\(eV\\):"))
         k_point_data = extract_kpoint(file_string)
 
     return {**data, **k_point_data}
 
 
 @accept_file_name
 def parse_gw_info(file_string: str) -> dict:
@@ -370,46 +357,47 @@
 
     Timings are not parsed because it's more convenient for regression-testing.
 
     :param str file_string: Parsed file string.
     :return: dict data: dictionary of parsed data.
     """
     data = {}
-    data['correlation_self_energy_parameters'] = parse_correlation_self_energy_params(file_string)
-    data['mixed_product_basis_parameters'] = parse_mixed_product_params(file_string)
-    data['bare_coulomb_potential_parameters'] = parse_bare_coulomb_potential_params(file_string)
-    data['screened_coulomb_potential'] =  match_current_return_line_n(file_string, 'Screened Coulomb potential:').strip()
-    data['core_electrons_treatment'] = match_current_return_line_n(file_string, 'Core electrons treatment:').strip()
-    data['qp_interval'] = parse_value_regex(file_string, 'Interval of quasiparticle states \\(ibgw, nbgw\\):')\
-        ['Interval of quasiparticle states (ibgw, nbgw)']
-    data['n_empty'] = parse_value_regex(file_string, 'Number of empty states \\(GW\\):')['Number of empty states (GW)']
-    data['q_grid'] = parse_value_regex(file_string, 'k/q-points grid:')['k/q-points grid']
-    data['mixed_product_wf_info'] = parse_mixed_product_wf_info(file_string)
-    data['frequency_grid'] = parse_frequency_grid_info(file_string)
-    n_freq_points = data['frequency_grid']['Number of frequencies: < nomeg >']
-    data['frequency_grid']['frequencies_weights'] = parse_frequency_grid(file_string, n_freq_points)
-    data['ks_eigenstates_summary'] = parse_ks_eigenstates(file_string)
-    data['ks_band_structure_summary'] = parse_band_structure_info(file_string, 'ks')
-    data['n_q_cycles'] = parse_n_q_point_cycles(file_string)
-    data['g0w0_band_structure_summary'] = parse_band_structure_info(file_string, 'gw')
+    data["correlation_self_energy_parameters"] = parse_correlation_self_energy_params(file_string)
+    data["mixed_product_basis_parameters"] = parse_mixed_product_params(file_string)
+    data["bare_coulomb_potential_parameters"] = parse_bare_coulomb_potential_params(file_string)
+    data["screened_coulomb_potential"] = match_current_return_line_n(file_string, "Screened Coulomb potential:").strip()
+    data["core_electrons_treatment"] = match_current_return_line_n(file_string, "Core electrons treatment:").strip()
+    data["qp_interval"] = parse_value_regex(file_string, "Interval of quasiparticle states \\(ibgw, nbgw\\):")[
+        "Interval of quasiparticle states (ibgw, nbgw)"
+    ]
+    data["n_empty"] = parse_value_regex(file_string, "Number of empty states \\(GW\\):")["Number of empty states (GW)"]
+    data["q_grid"] = parse_value_regex(file_string, "k/q-points grid:")["k/q-points grid"]
+    data["mixed_product_wf_info"] = parse_mixed_product_wf_info(file_string)
+    data["frequency_grid"] = parse_frequency_grid_info(file_string)
+    n_freq_points = data["frequency_grid"]["Number of frequencies: < nomeg >"]
+    data["frequency_grid"]["frequencies_weights"] = parse_frequency_grid(file_string, n_freq_points)
+    data["ks_eigenstates_summary"] = parse_ks_eigenstates(file_string)
+    data["ks_band_structure_summary"] = parse_band_structure_info(file_string, "ks")
+    data["n_q_cycles"] = parse_n_q_point_cycles(file_string)
+    data["g0w0_band_structure_summary"] = parse_band_structure_info(file_string, "gw")
     return data
 
 
 def extract_gw_timings_as_list(file_string: str) -> Union[List[str], None]:
     """Extract GW timing string block as a list.
 
     Utilises the fact that timings are returned at the end of GW_INFO.OUT
 
     :param str file_string: Parsed file string
     :param list timings: GW timings, with each element storing a
     line of timings as a string.
     """
-    file_list = file_string.split('\n')
+    file_list = file_string.split("\n")
     for i, line in enumerate(reversed(file_list)):
-        if 'GW timing info (seconds)' in line:
+        if "GW timing info (seconds)" in line:
             index = i - 2
             return file_list[-index:]
 
     return None
 
 
 def parse_gw_timings(file_string: str) -> dict:
@@ -438,33 +426,32 @@
     :return: dict data: dictionary of parsed timings
     """
     timings = extract_gw_timings_as_list(file_string)
 
     # Parse and store nested timings
     data = {}
     component_time = {}
-    root_key = 'Initialization'
+    root_key = "Initialization"
     initial_key = root_key
 
     for line in timings:
-
-        key = line.strip().split(':')[0].rstrip()
-        if len(key) == 0: continue
-        is_root_key = key[0] != '-'
+        key = line.strip().split(":")[0].rstrip()
+        if len(key) == 0:
+            continue
+        is_root_key = key[0] != "-"
 
         if is_root_key and (key != initial_key):
             data[root_key] = copy.deepcopy(component_time)
             component_time.clear()
             root_key = key
 
-        time_str = line.strip().split(':')[-1]
-        component_time[key.strip('-').strip()] = float(
-            time_str) if can_be_float(time_str) else None
+        time_str = line.strip().split(":")[-1]
+        component_time[key.strip("-").strip()] = float(time_str) if can_be_float(time_str) else None
 
     # Store last value, Total
     data[root_key] = {root_key: float(time_str)}
 
     # Remove superfluous key from table formatting
-    arb_str = '_________________________________________________________'
+    arb_str = "_________________________________________________________"
     del data[arb_str]
 
     return data
```

### Comparing `excitingtools-1.7.0/excitingtools/exciting_dict_parsers/gw_taskgroup_parser.py` & `excitingtools-1.7.1/excitingtools/exciting_dict_parsers/gw_taskgroup_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,25 +14,24 @@
      1st line: 2 (rank=2)
      2nd line: fours integers i,j,m,n with the ranges: matrix[i:m,j:n]
      next lines: matrix elements (complex numbers)
 
     :param file_name: name of the file
     :return: matrix read from file
     """
-    with open(file_name, 'r') as file:
+    with open(file_name) as file:
         dim = int(file.readline().split()[0])
-        m_ini, n_ini, m_end, n_end = [int(x) for x in file.readline().split()]
+        m_ini, n_ini, m_end, n_end = (int(x) for x in file.readline().split())
         assert dim == 2 and m_ini == 1 and n_ini == 1, "file should contain a full matrix"
         matrix = np.zeros((m_end, n_end), dtype=complex)
 
         counter = 0
         for line in file:
             for data in line.split():
-                matrix[np.unravel_index(counter, (m_end, n_end), order='F')] = \
-                    complex(*literal_eval(data))
+                matrix[np.unravel_index(counter, (m_end, n_end), order="F")] = complex(*literal_eval(data))
                 counter += 1
     return matrix
 
 
 def __parse_file_with_array_of_rank_3(file_name: str) -> NDArray[np.complex128]:
     """Parser for files containing arrays of rank 3.
 
@@ -40,25 +39,24 @@
      1st line: 3 (rank=3)
      2nd line: six integers i,j,k,m,n,p with the ranges: matrix[i:m,j:n,k:p]
      next lines: array elements (complex numbers)
 
     :param file_name: name of the file
     :return: array read from file
     """
-    with open(file_name, 'r') as file:
+    with open(file_name) as file:
         dim = int(file.readline().split()[0])
-        m_ini, n_ini, p_ini, m_end, n_end, p_end = [int(x) for x in file.readline().split()]
+        m_ini, n_ini, p_ini, m_end, n_end, p_end = (int(x) for x in file.readline().split())
         assert dim == 3 and m_ini == 1 and n_ini == 1 and p_ini == 1, "file should contain a full array"
         array = np.zeros((m_end, n_end, p_end), dtype=complex)
 
         counter = 0
         for line in file:
             for data in line.split():
-                array[np.unravel_index(counter, (m_end, n_end, p_end), order='F')] = \
-                    complex(*literal_eval(data))
+                array[np.unravel_index(counter, (m_end, n_end, p_end), order="F")] = complex(*literal_eval(data))
                 counter += 1
     return array
 
 
 def __square_matrix(a: NDArray) -> NDArray:
     """Square a matrix.
 
@@ -67,55 +65,57 @@
     """
     return np.matmul(a.T.conj(), a)
 
 
 def parse_barc(file_name: str) -> Dict[str, NDArray[np.complex128]]:
     """Parser for BARC_*.OUT, where * is an integer.
 
-    The file contains the product: M*(v^1/2), where M is a matrix with 
+    The file contains the product: M*(v^1/2), where M is a matrix with
     eigenvectors, and v is a diagonal matrix with the eigenvalues.
-    Since the definition of M is not unique, we must return A^H*A, 
+    Since the definition of M is not unique, we must return A^H*A,
     where A is the matrix read.
 
     :param file_name: name of the file
     :return: parsed data as dictionary
     """
     return {"CoulombMatrix": __square_matrix(__parse_file_with_matrix(file_name))}
 
+
 def parse_sgi(file_name: str) -> Dict[str, NDArray[np.complex128]]:
     """Parser for SGI_*.OUT, where * is an integer.
 
-    This file contains the vectors $\tilde{S_{Gi}}$, defined in Eq. (41) of 
+    This file contains the vectors $\tilde{S_{Gi}}$, defined in Eq. (41) of
     Computer Phys. Comm. 184, 348 (2013).
     By reading the matrix A as stored, and performing A^H*A, one gets the overlap
     matrix between basis elements defined for the interstitial region.
 
     :param file_name: name of the file
     :return: parsed data as dictionary
     """
     return {"OverlapMatrix": __square_matrix(__parse_file_with_matrix(file_name))}
 
 
 def parse_epsilon(file_name: str) -> Dict[str, NDArray[np.complex128]]:
     """Parser for the gw-epsilon files, which contain the dielectric function, its head or wings.:
       - EPSH.OUT,
       - EPSW1.OUT,
-      - EPSW2.OUT, 
+      - EPSW2.OUT,
       - EPSILON-GW_*.OUT, where * is an integer
-    
+
     :param file_name: name of the file
     :return: parsed data as dictionary
     """
     return {"epsilon_tensor": __parse_file_with_array_of_rank_3(file_name)}
 
+
 def parse_inverse_epsilon(file_name: str) -> Dict[str, NDArray[np.complex128]]:
     """Parser for the gw-inverse-epsilon files, which contain the inverse of the
     dielectric function, its head or wings:
       - INVERSE-EPS-H.OUT,
       - INVERSE-EPS-W1.OUT,
-      - INVERSE-EPS-W2.OUT, 
+      - INVERSE-EPS-W2.OUT,
       - INVERSE-EPSILON-_*.OUT, where * is an integer
 
     :param file_name: name of the file
     :return: parsed data as dictionary
     """
     return {"inverse_epsilon_tensor": __parse_file_with_array_of_rank_3(file_name)}
```

### Comparing `excitingtools-1.7.0/excitingtools/exciting_dict_parsers/gw_vxc_parser.py` & `excitingtools-1.7.1/excitingtools/exciting_dict_parsers/gw_vxc_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-""" VXCNN.DAT Parser.
-"""
-import numpy as np
+"""VXCNN.DAT Parser."""
+
+import pathlib
 import re
 from typing import Union
-import pathlib
+
+import numpy as np
 
 from excitingtools.dataclasses.data_structs import NumberOfStates
 from excitingtools.exciting_dict_parsers.gw_eigenvalues_parser import n_states_from_file
 
 
 def vkl_from_vxc(file_string: str) -> dict:
     """Extract vkl (k-points in fractional coordinates) from VXCNN.DAT.
@@ -17,15 +18,15 @@
 
     k-indices are not extracted as they are always contiguous,
     with indexing starting at 1.
 
     :param str file_string: File string.
     :return dict vkl: k-points in fractional coordinates.
     """
-    raw_data: list = re.findall(r'\s*ik= .*$', file_string, flags=re.MULTILINE)
+    raw_data: list = re.findall(r"\s*ik= .*$", file_string, flags=re.MULTILINE)
     vkl = {}
     for ik, line in enumerate(raw_data):
         vkl[ik + 1] = [float(k) for k in line.split()[-3:]]
     return vkl
 
 
 def parse_vxnn_vectors(full_file_name: Union[str, pathlib.Path], vkl: dict, n_states: int) -> dict:
@@ -59,17 +60,15 @@
     blank_line = 1
 
     data = {}
     skip_lines = header_size
 
     # Must iterate lowest to highest, else data won't match k-points
     for ik in range(1, len(vkl) + 1):
-        vxc_vector = np.loadtxt(full_file_name,
-                                skiprows=skip_lines,
-                                max_rows=n_states)
+        vxc_vector = np.loadtxt(full_file_name, skiprows=skip_lines, max_rows=n_states)
         # Ignore first column (state index)
         data[ik] = vxc_vector[:, 1:]
         skip_lines += n_states + (header_size + blank_line)
 
     return data
 
 
@@ -89,16 +88,15 @@
             file_string = f.read()
     except FileNotFoundError:
         raise FileNotFoundError(f"{full_file_name} does not exist")
 
     states = n_states_from_vxcnn(file_string)
     vkl = vkl_from_vxc(file_string)
     v_xc = parse_vxnn_vectors(full_file_name, vkl, states.n_states)
-    assert len(vkl) == len(v_xc), (
-        "Should be a vector of Vxc_NN for each k-point")
+    assert len(vkl) == len(v_xc), "Should be a vector of Vxc_NN for each k-point"
 
     # Repackage Vxc vectors with their respective k-points
     data = {}
     for ik in range(1, len(vkl) + 1):
-        data[ik] = {'vkl': vkl[ik], 'v_xc_nn': v_xc[ik]}
+        data[ik] = {"vkl": vkl[ik], "v_xc_nn": v_xc[ik]}
 
     return data
```

### Comparing `excitingtools-1.7.0/excitingtools/exciting_dict_parsers/input_parser.py` & `excitingtools-1.7.1/excitingtools/exciting_dict_parsers/input_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-""" Parsers for input.xml. """
+"""Parsers for input.xml."""
 
 import copy
-from typing import Tuple
+from typing import Optional, Tuple
 from xml.etree import ElementTree
 
 from excitingtools.parser_utils.parser_decorators import xml_root
-from excitingtools.parser_utils.parser_utils import find_element, convert_string_dict
+from excitingtools.parser_utils.parser_utils import convert_string_dict, find_element
 from excitingtools.utils import valid_attributes as all_valid_attributes
 from excitingtools.utils.valid_attributes import input_valid_attributes
 
 
 @xml_root
 def parse_input_xml(root):
-    """ Parse an input.xml file into dictionary. """
+    """Parse an input.xml file into dictionary."""
     assert root.tag == "input"
     return parse_element_xml(root)
 
 
-def get_root_from_tag(root: ElementTree.Element, tag: str = None) -> Tuple[ElementTree.Element, str]:
-    """ Get the root from a tag.
+def get_root_from_tag(root: ElementTree.Element, tag: Optional[str] = None) -> Tuple[ElementTree.Element, str]:
+    """Get the root from a tag.
 
     :param tag: tag of interest
     :param root: xml root containing the tag (or having the specified tag as tag)
     :returns: the tag and the found root, if tag was None returns the tag of the given root
     """
     if tag is None:
         return root, root.tag
@@ -31,16 +31,16 @@
     if root is None:
         raise ValueError(f"Your specified input has no tag {tag}.")
 
     return root, root.tag
 
 
 @xml_root
-def parse_element_xml(root, tag: str = None) -> dict:
-    """ Parse a xml element into dictionary. Can be input.xml root or a subelement of it.
+def parse_element_xml(root, tag: Optional[str] = None) -> dict:
+    """Parse a xml element into dictionary. Can be input.xml root or a subelement of it.
     Put the attributes simply in dict and add recursively the subtrees and nested dicts.
 
     :param tag: the tag to parse
     :param root: the xml root containing the tag
     :returns: the parsed dictionary, data converted to actual data types
     """
     root, tag = get_root_from_tag(root, tag)
@@ -48,29 +48,29 @@
     if tag in special_tags_to_parse_map:
         return special_tags_to_parse_map[tag](root)
 
     element_dict = convert_string_dict(copy.deepcopy(root.attrib))
 
     multiple_children = set(getattr(all_valid_attributes, f"{tag}_multiple_children", set()))
     subelements = list(root)
-    multiple_tags = set([subelement.tag for subelement in subelements]) & multiple_children
+    multiple_tags = {subelement.tag for subelement in subelements} & multiple_children
     element_dict.update({tag: [] for tag in multiple_tags})
 
     # for loop over all subelements to retain the order
     for subelement in subelements:
         if subelement.tag in multiple_children:
             element_dict[subelement.tag].append(parse_element_xml(subelement))
         else:
             element_dict[subelement.tag] = parse_element_xml(subelement)
 
     return element_dict
 
 
 def _parse_input_tag(root) -> dict:
-    """ Parse special input tag. Necessary because exciting/xml allows arbitrary attributes at this level.
+    """Parse special input tag. Necessary because exciting/xml allows arbitrary attributes at this level.
     Only parses the explicitly named attributes in the schema.
 
     :param root: the xml root containing the input tag
     :returns: the parsed dictionary, data converted to actual data types
     """
     valid_attribs = {key: value for key, value in root.attrib.items() if key in input_valid_attributes}
     element_dict = convert_string_dict(valid_attribs)
@@ -80,68 +80,66 @@
         element_dict[subelement.tag] = parse_element_xml(subelement)
 
     return element_dict
 
 
 @xml_root
 def parse_structure(root) -> dict:
-    """ Parse exciting input.xml structure element into python dictionary.
+    """Parse exciting input.xml structure element into python dictionary.
 
     :param root: Input for the parser.
     :returns: Dictionary containing the structure input element attributes and subelements. Looks like:
         {'atoms': List of atoms with atom positions in fractional coordinates,
          'lattice': List of 3 lattice vectors, 'species_path': species_path as string,
          'crystal_properties': dictionary with the crystal_properties,
          'species_properties': dictionary with the species_properties,
          all additional keys are structure attributes}
     """
-    structure = find_element(root, 'structure')
+    structure = find_element(root, "structure")
     structure_properties = convert_string_dict(copy.deepcopy(structure.attrib))
-    species_path = structure_properties.pop('speciespath')
+    species_path = structure_properties.pop("speciespath")
 
-    crystal = structure.find('crystal')
+    crystal = structure.find("crystal")
     crystal_properties = convert_string_dict(copy.deepcopy(crystal.attrib))
-    lattice = []
-    for base_vect in crystal:
-        lattice.append([float(x) for x in base_vect.text.split()])
+    lattice = [[float(x) for x in base_vect.text.split()] for base_vect in crystal]
 
     atoms = []
     species_properties = {}
-    for species in structure.findall('species'):
+    for species in structure.findall("species"):
         species_attributes = convert_string_dict(copy.deepcopy(species.attrib))
-        species_file = species_attributes.pop('speciesfile')
+        species_file = species_attributes.pop("speciesfile")
         species_symbol = species_file[:-4]
 
         species_subelements = list(species)
         atom_xml_trees = [x for x in species_subelements if x.tag == "atom"]
         for atom in atom_xml_trees:
             atom_attributes = convert_string_dict(copy.deepcopy(atom.attrib))
-            atom_dict = {'species': species_symbol, 'position': atom_attributes.pop('coord')}
+            atom_dict = {"species": species_symbol, "position": atom_attributes.pop("coord")}
             atom_dict.update(atom_attributes)
             atoms.append(atom_dict)
 
         other_xml_trees = set(species_subelements) - set(atom_xml_trees)
         for tree in other_xml_trees:
             species_attributes[tree.tag] = parse_element_xml(tree)
         species_properties[species_symbol] = species_attributes
 
     return {
-        'atoms': atoms,
-        'lattice': lattice,
-        'species_path': species_path,
-        'crystal_properties': crystal_properties,
-        'species_properties': species_properties,
-        **structure_properties
+        "atoms": atoms,
+        "lattice": lattice,
+        "species_path": species_path,
+        "crystal_properties": crystal_properties,
+        "species_properties": species_properties,
+        **structure_properties,
     }
 
 
 # special tag to parse function map or lambda if one-liner
 # necessary for tags which doesn't contain simply xml attributes and subtrees
 special_tags_to_parse_map = {
     "input": _parse_input_tag,
     "title": lambda root: root.text,
     "keywords": lambda root: root.text,
     "structure": parse_structure,
     "qpointset": lambda root: [[float(x) for x in qpoint.text.split()] for qpoint in root],
-    "plan": lambda root: [doonly.attrib['task'] for doonly in root],
-    "kstlist": lambda root: [[int(x) for x in pointstatepair.text.split()] for pointstatepair in root]
+    "plan": lambda root: [doonly.attrib["task"] for doonly in root],
+    "kstlist": lambda root: [[int(x) for x in pointstatepair.text.split()] for pointstatepair in root],
 }
```

### Comparing `excitingtools-1.7.0/excitingtools/exciting_dict_parsers/parser_factory.py` & `excitingtools-1.7.1/excitingtools/exciting_dict_parsers/parser_factory.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,81 +26,81 @@
     species_parser,
     state_parser,
 )
 
 # Map file name to parser function
 # Note: more specific names should be higher, as the search will go through this map top-down
 _file_to_parser = {
-    'INFO.OUT': groundstate_parser.parse_info_out,
-    'info.xml': groundstate_parser.parse_info_xml,
-    'input.xml': input_parser.parse_input_xml,
-    'species.xml': species_parser.parse_species_xml,
-    'atoms.xml': groundstate_parser.parse_atoms,
-    'evalcore.xml': groundstate_parser.parse_evalcore,
-    'eigval.xml': groundstate_parser.parse_eigval,
-    'geometry.xml': groundstate_parser.parse_geometry,
-    'LINENGY.OUT': groundstate_parser.parse_linengy,
-    'LO_RECOMMENDATION.OUT': groundstate_parser.parse_lo_recommendation,
-    '*3D.xml': properties_parser.parse_plot_3d,
-    'LSJ.xml': properties_parser.parse_lsj,
-    'EFG.xml': properties_parser.parse_efg,
-    'mossbauer.xml': properties_parser.parse_mossbauer,
-    'expiqr.xml': properties_parser.parse_expiqr,
-    'effmass.xml': properties_parser.parse_effmass,
-    'bandstructure.xml': properties_parser.parse_bandstructure_depreciated,
-    'dos.xml': properties_parser.parse_dos,
-    'KERR.OUT': properties_parser.parse_kerr,
-    'EPSILON_??.OUT': properties_parser.parse_epsilon,
-    'CHI_111.OUT': properties_parser.parse_chi,
-    'ELNES.OUT': properties_parser.parse_elnes,
-    'SEEBECK_11.OUT': properties_parser.parse_seebeck,
-    'ELECTCOND_11.OUT': properties_parser.parse_seebeck,
-    'THERMALCOND_11.OUT': properties_parser.parse_seebeck,
-    'Z_11.OUT': properties_parser.parse_seebeck,
-    'ldos.out': properties_parser.parse_ldos,
-    'band_edges.out': properties_parser.parse_band_edges,
-    'spintext.xml': properties_parser.parse_spintext,
-    'POLARIZATION.OUT': properties_parser.parse_polarization,
-    'TDOS_WANNIER.OUT': properties_parser.parse_tdos_wannier,
-    'WANNIER_INFO.OUT': properties_parser.parse_wannier_info,
-    'coreoverlap.xml': properties_parser.parse_core_overlap,
-    'wf1d-*.dat': properties_parser.parse_wf1d,
-    'wf2d-*.xsf': properties_parser.parse_wf2d,
-    'wf3d-*.xsf': properties_parser.parse_wf3d,
-    'wf3d-*.cube': properties_parser.parse_cube,
-    'INFOXS.OUT': bse_parser.parse_infoxs_out,
-    'EPSILON_BSE*.OUT': bse_parser.parse_EPSILON_NAR,
-    'EPSILON_NAR*.OUT': bse_parser.parse_EPSILON_NAR,
-    'DICHROIC_*.OUT': bse_parser.parse_EPSILON_NAR,
-    'OSCI_*.OUT': bse_parser.parse_EXCITON_NAR_BSE,
-    'EXCITON_*.OUT': bse_parser.parse_EXCITON_NAR_BSE,
-    'LOSS_*.OUT': bse_parser.parse_LOSS_NAR,
-    'GW_INFO.OUT': gw_info_parser.parse_gw_info,
-    'EFERMI_GW.OUT': gw_eigenvalues_parser.parse_efermi_gw,
-    'EVALQP.DAT': gw_eigenvalues_parser.parse_evalqp,
-    'VXCNN.DAT': gw_vxc_parser.parse_vxcnn,
-    'EPS00_GW.OUT': gw_eps00_parser.parse_eps00_gw,
-    'BARC_*': gw_taskgroup_parser.parse_barc,
-    'SGI_*': gw_taskgroup_parser.parse_sgi,
-    'EPSILON-GW_*': gw_taskgroup_parser.parse_epsilon,
-    'EPSH.OUT': gw_taskgroup_parser.parse_epsilon,
-    'EPSW1.OUT': gw_taskgroup_parser.parse_epsilon,
-    'EPSW2.OUT': gw_taskgroup_parser.parse_epsilon,
-    'INVERSE-EPS*': gw_taskgroup_parser.parse_inverse_epsilon,
-    'JIND.OUT': RT_TDDFT_parser.parse_jind,
-    'NEXC.OUT': RT_TDDFT_parser.parse_nexc,
-    'ETOT_RTTDDFT.OUT': RT_TDDFT_parser.parse_etot,
-    'EIGVAL_*': RT_TDDFT_parser.parse_eigval_screenshots,
-    'PROJ_*': RT_TDDFT_parser.parse_proj_screenshots,
-    'ATOM_*': RT_TDDFT_parser.parse_atom_position_velocity_force,
-    'FCR_*': RT_TDDFT_parser.parse_force,
-    'FEXT_*': RT_TDDFT_parser.parse_force,
-    'FHF_*': RT_TDDFT_parser.parse_force,
-    'FVAL_*': RT_TDDFT_parser.parse_force,
-    'STATE.OUT': state_parser.parse_state_out,
+    "INFO.OUT": groundstate_parser.parse_info_out,
+    "info.xml": groundstate_parser.parse_info_xml,
+    "input.xml": input_parser.parse_input_xml,
+    "species.xml": species_parser.parse_species_xml,
+    "atoms.xml": groundstate_parser.parse_atoms,
+    "evalcore.xml": groundstate_parser.parse_evalcore,
+    "eigval.xml": groundstate_parser.parse_eigval,
+    "geometry.xml": groundstate_parser.parse_geometry,
+    "LINENGY.OUT": groundstate_parser.parse_linengy,
+    "LO_RECOMMENDATION.OUT": groundstate_parser.parse_lo_recommendation,
+    "*3D.xml": properties_parser.parse_plot_3d,
+    "LSJ.xml": properties_parser.parse_lsj,
+    "EFG.xml": properties_parser.parse_efg,
+    "mossbauer.xml": properties_parser.parse_mossbauer,
+    "expiqr.xml": properties_parser.parse_expiqr,
+    "effmass.xml": properties_parser.parse_effmass,
+    "bandstructure.xml": properties_parser.parse_bandstructure_depreciated,
+    "dos.xml": properties_parser.parse_dos,
+    "KERR.OUT": properties_parser.parse_kerr,
+    "EPSILON_??.OUT": properties_parser.parse_epsilon,
+    "CHI_111.OUT": properties_parser.parse_chi,
+    "ELNES.OUT": properties_parser.parse_elnes,
+    "SEEBECK_11.OUT": properties_parser.parse_seebeck,
+    "ELECTCOND_11.OUT": properties_parser.parse_seebeck,
+    "THERMALCOND_11.OUT": properties_parser.parse_seebeck,
+    "Z_11.OUT": properties_parser.parse_seebeck,
+    "ldos.out": properties_parser.parse_ldos,
+    "band_edges.out": properties_parser.parse_band_edges,
+    "spintext.xml": properties_parser.parse_spintext,
+    "POLARIZATION.OUT": properties_parser.parse_polarization,
+    "TDOS_WANNIER.OUT": properties_parser.parse_tdos_wannier,
+    "WANNIER_INFO.OUT": properties_parser.parse_wannier_info,
+    "coreoverlap.xml": properties_parser.parse_core_overlap,
+    "wf1d-*.dat": properties_parser.parse_wf1d,
+    "wf2d-*.xsf": properties_parser.parse_wf2d,
+    "wf3d-*.xsf": properties_parser.parse_wf3d,
+    "wf3d-*.cube": properties_parser.parse_cube,
+    "INFOXS.OUT": bse_parser.parse_infoxs_out,
+    "EPSILON_BSE*.OUT": bse_parser.parse_EPSILON_NAR,
+    "EPSILON_NAR*.OUT": bse_parser.parse_EPSILON_NAR,
+    "DICHROIC_*.OUT": bse_parser.parse_EPSILON_NAR,
+    "OSCI_*.OUT": bse_parser.parse_EXCITON_NAR_BSE,
+    "EXCITON_*.OUT": bse_parser.parse_EXCITON_NAR_BSE,
+    "LOSS_*.OUT": bse_parser.parse_LOSS_NAR,
+    "GW_INFO.OUT": gw_info_parser.parse_gw_info,
+    "EFERMI_GW.OUT": gw_eigenvalues_parser.parse_efermi_gw,
+    "EVALQP.DAT": gw_eigenvalues_parser.parse_evalqp,
+    "VXCNN.DAT": gw_vxc_parser.parse_vxcnn,
+    "EPS00_GW.OUT": gw_eps00_parser.parse_eps00_gw,
+    "BARC_*": gw_taskgroup_parser.parse_barc,
+    "SGI_*": gw_taskgroup_parser.parse_sgi,
+    "EPSILON-GW_*": gw_taskgroup_parser.parse_epsilon,
+    "EPSH.OUT": gw_taskgroup_parser.parse_epsilon,
+    "EPSW1.OUT": gw_taskgroup_parser.parse_epsilon,
+    "EPSW2.OUT": gw_taskgroup_parser.parse_epsilon,
+    "INVERSE-EPS*": gw_taskgroup_parser.parse_inverse_epsilon,
+    "JIND.OUT": RT_TDDFT_parser.parse_jind,
+    "NEXC.OUT": RT_TDDFT_parser.parse_nexc,
+    "ETOT_RTTDDFT.OUT": RT_TDDFT_parser.parse_etot,
+    "EIGVAL_*": RT_TDDFT_parser.parse_eigval_screenshots,
+    "PROJ_*": RT_TDDFT_parser.parse_proj_screenshots,
+    "ATOM_*": RT_TDDFT_parser.parse_atom_position_velocity_force,
+    "FCR_*": RT_TDDFT_parser.parse_force,
+    "FEXT_*": RT_TDDFT_parser.parse_force,
+    "FHF_*": RT_TDDFT_parser.parse_force,
+    "FVAL_*": RT_TDDFT_parser.parse_force,
+    "STATE.OUT": state_parser.parse_state_out,
 }
 
 
 def parse(full_file_name: str) -> dict:
     """Selects parser according to the name of the input file then returns the result of the parser.
 
     REQUIREMENTS. Parser function must:
@@ -109,15 +109,15 @@
 
     :param full_file_name: file name prepended by full path
     :return: parsed data
     """
 
     full_file_path = Path(full_file_name.rstrip())
     if not full_file_path.exists():
-        raise FileNotFoundError(f'File not found: {full_file_path}')
+        raise FileNotFoundError(f"File not found: {full_file_path}")
 
     file_name = full_file_path.name
 
     parser: Union[Callable[[str], dict], None] = None
     for pattern in _file_to_parser:
         if fnmatch(file_name, pattern):
             parser = _file_to_parser[pattern]
@@ -135,10 +135,10 @@
     :param full_file_name: file name prepended by full path
     :return: parsed data
     """
     warnings.warn(
         "Deprecated API. Use 'excitingtools.parse' instead. "
         "Support for this API will be removed in excitingtools 1.8.0",
         DeprecationWarning,
-        stacklevel=2
+        stacklevel=2,
     )
     return parse(full_file_name)
```

### Comparing `excitingtools-1.7.0/excitingtools/exciting_dict_parsers/properties_parser.py` & `excitingtools-1.7.1/excitingtools/exciting_dict_parsers/properties_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,31 @@
-"""Parsers for exciting properties.
-"""
+"""Parsers for exciting properties."""
+
 import os
-import xml.etree.cElementTree as ET
+import xml.etree.ElementTree as ET
 from typing import Dict
 from xml.etree.ElementTree import ParseError
 
 import numpy as np
 
-from excitingtools.parser_utils.parser_decorators import xml_root, set_return_values
+from excitingtools.parser_utils.parser_decorators import set_return_values, xml_root
 
 
 @set_return_values
 def parse_plot_3d(name: str) -> dict:
     """
     Parser for RHO3D.xml, VCL3D.xml, VXC3D.xml, WF3D.xml, ELF3D.xml, EF3D.xmlit
 
     :param str name: File name
     :return dict output: Parsed data
     """
     root = ET.parse(name)
     plot_3d = {"title": root.find("title").text}
     grid = root.find("grid").attrib
-    axis = []
-    for ax in root.find("grid").findall("axis"):
-        axis.append(ax.attrib)
+    axis = [ax.attrib for ax in root.find("grid").findall("axis")]
     grid["axis"] = {}
     for item in axis:
         name = item["name"]
         grid["axis"][name] = item
     grid["value"] = root.find("grid").find("value").attrib
     plot_3d["grid"] = grid
 
@@ -78,16 +76,16 @@
         spec["atom"] = {}
         for item in atom:
             name = item["n"]
             spec["atom"][name] = item
         species.append(spec)
     LSJ["species"] = {}
     for item in species:
-        name = item['n']
-        LSJ['species'][name] = item
+        name = item["n"]
+        LSJ["species"][name] = item
 
     return LSJ
 
 
 def parse_efg(name: str) -> dict:
     """
     Parser for EFG.xml
@@ -105,37 +103,31 @@
 
     :param str name: File name
     :return dict output: Parsed data
     """
     root = ET.parse(name).getroot()
     data = {}
 
-    for species in root.findall('species'):
-        species_key = species.tag + str(species.attrib['n'])
-        data[species_key] = {
-            'chemicalSymbol': species.attrib['chemicalSymbol']
-        }
+    for species in root.findall("species"):
+        species_key = species.tag + str(species.attrib["n"])
+        data[species_key] = {"chemicalSymbol": species.attrib["chemicalSymbol"]}
 
-        for atom in species.findall('atom'):
-            atom_key = atom.tag + atom.attrib['n']
+        for atom in species.findall("atom"):
+            atom_key = atom.tag + atom.attrib["n"]
 
             for efg_tensor in atom.findall("EFG-tensor"):
                 efg = np.empty(shape=(3, 3))
 
                 for i, line in enumerate(efg_tensor.findall("line")):
                     efg[i, :] = [float(x) for x in line.text.split()]
 
                 for eigenvalues in efg_tensor.findall("eigenvalues"):
                     eig = [float(e) for e in eigenvalues.text.split()]
 
-            data[species_key][atom_key] = {
-                'trace': float(efg_tensor.attrib['trace']),
-                'efg': efg,
-                'eigenvalues': eig
-            }
+            data[species_key][atom_key] = {"trace": float(efg_tensor.attrib["trace"]), "efg": efg, "eigenvalues": eig}
     return data
 
 
 @set_return_values
 def parse_mossbauer(name: str) -> dict:
     """
     Parser for mossbauer.xml
@@ -144,17 +136,15 @@
     :return dict output: Parsed data
     """
     root = ET.parse(name).getroot()
     mossbauer = {}
     species = []
     for node in root.findall("species"):
         spec = node.attrib
-        atom = []
-        for nod in node:
-            atom.append(nod.attrib)
+        atom = [nod.attrib for nod in node]
         spec["atom"] = {}
         for item in atom:
             name = item["n"]
             spec["atom"][name] = item
         species.append(spec)
     mossbauer["species"] = {}
     for item in species:
@@ -210,23 +200,19 @@
     effmass = {}
     effmass["k-point"] = root.find("k-point").attrib
     state = []
     for node in root.findall("state"):
         st = node.attrib
 
         evdk = node.find("evdk").attrib
-        matrix1 = []
-        for line in node.find("evdk").findall("line"):
-            matrix1.append(line.text.split())
+        matrix1 = [line.text.split() for line in node.find("evdk").findall("line")]
         evdk["evdk_matrix"] = matrix1
 
         emt = node.find("emt").attrib
-        matrix2 = []
-        for line in node.find("emt").findall("line"):
-            matrix2.append(line.text.split())
+        matrix2 = [line.text.split() for line in node.find("emt").findall("line")]
         emt["emt_matrix"] = matrix2
 
         st["evdk"] = evdk
         st["emt"] = emt
         state.append(st)
 
     effmass["state"] = {}
@@ -273,50 +259,59 @@
         bandstructure["band"][name] = item
         j = j + 1
     return bandstructure
 
 
 @xml_root
 def parse_band_structure_xml(root) -> dict:
-    """ Parse KS band structure from bandstructure.xml.
+    """Parse KS band structure from bandstructure.xml.
 
     :param root: Band structure XML file name, XML string or ElementTree.Element as input.
     :return: Band data
     """
     # Split band structure file contents: title, bands and vertices
-    bs_xml: Dict[str, list] = {'title': [], 'band': [], 'vertex': []}
+    bs_xml: Dict[str, list] = {"title": [], "band": [], "vertex": []}
 
-    for item in list(root):
-        try:
+    item = root[0]
+    try:
+        for item in list(root):
             bs_xml[item.tag].append(item)
-        except KeyError:
-            raise KeyError(f'Element tag {item.tag} requires implementing in band structure parser')
+    except KeyError:
+        raise KeyError(f"Element tag {item.tag} requires implementing in band structure parser")
 
-    n_bands = len(bs_xml['band'])
-    first_band = bs_xml['band'][0]
+    n_bands = len(bs_xml["band"])
+    first_band = bs_xml["band"][0]
     n_kpts = len(list(first_band))
 
     # Same set of flattened k-points, per band - so parse once
-    k_points_along_band = np.array([point.get('distance') for point in list(first_band)], dtype=float)
+    k_points_along_band = np.array([point.get("distance") for point in list(first_band)], dtype=float)
 
     # Read E(k), per band
     band_energies = np.empty(shape=(n_kpts, n_bands))
-    for ib, band in enumerate(bs_xml['band']):
+    for ib, band in enumerate(bs_xml["band"]):
         for ik, point in enumerate(list(band)):
-            band_energies[ik, ib] = point.get('eval')
+            band_energies[ik, ib] = point.get("eval")
 
-    vertices = []
-    for element in bs_xml['vertex']:
-        vertices.append({'distance': float(element.get('distance')),
-                         'label': element.get('label'),
-                         'coord':  [float(x) for x in element.get('coord').split()]})
-
-    return {'title': bs_xml['title'], 'n_kpts': n_kpts, 'n_bands': n_bands,
-            'k_points_along_band': k_points_along_band,
-            'band_energies': band_energies, 'vertices': vertices}
+    vertices = [
+        {
+            "distance": float(element.get("distance")),
+            "label": element.get("label"),
+            "coord": [float(x) for x in element.get("coord").split()],
+        }
+        for element in bs_xml["vertex"]
+    ]
+
+    return {
+        "title": bs_xml["title"],
+        "n_kpts": n_kpts,
+        "n_bands": n_bands,
+        "k_points_along_band": k_points_along_band,
+        "band_energies": band_energies,
+        "vertices": vertices,
+    }
 
 
 def parse_band_structure_dat(name: str) -> dict:
     """Parser for bandstructure.dat
 
     :param str name: File name
     :return dict output: Parsed data
@@ -328,26 +323,26 @@
     n_kpts = int(header.split()[3])
     n_bands = int(header.split()[2])
     dimensions = 3
 
     k_points = np.empty(shape=(n_kpts, dimensions))
     flattened_k_points = np.empty(n_kpts)
     for i in range(n_kpts):
-        k_points[i] = np.array([k for k in bs_dat[i, 2:5]])
+        k_points[i] = np.array(list(bs_dat[i, 2:5]))
         flattened_k_points[i] = bs_dat[i, 5]
 
-    band_energies = np.reshape(bs_dat[:, 6], (n_kpts, n_bands), order='F')
+    band_energies = np.reshape(bs_dat[:, 6], (n_kpts, n_bands), order="F")
 
     return {
-            'n_kpts': n_kpts,
-            'n_bands': n_bands,
-            'k_points': k_points,
-            'flattened_k_points': flattened_k_points,
-            'band_energies': band_energies
-        }
+        "n_kpts": n_kpts,
+        "n_bands": n_bands,
+        "k_points": k_points,
+        "flattened_k_points": flattened_k_points,
+        "band_energies": band_energies,
+    }
 
 
 @set_return_values
 def parse_dos(name: str) -> dict:
     """
     Parser for dos.xml
 
@@ -372,128 +367,118 @@
         dos["totaldos"]["diagram"]["point"][name] = item
         i = i + 1
     return dos
 
 
 @xml_root
 def parse_charge_density(root) -> np.ndarray:
-    """ Parse charge density from RHO1D.xml file.
+    """Parse charge density from RHO1D.xml file.
 
     `axis` and `vertex` sub-trees ignored in the parsing.
 
     :param root: XML file name, XML string or ElementTree.Element as input.
     :return: Numpy array containing rho[:, 1] = distance and rho[:, 2] = density.
     """
-    function_points = root.find('grid').find('function')
+    function_points = root.find("grid").find("function")
     rho = np.empty(shape=(len(function_points), 2))
     for i, point in enumerate(function_points):
-        rho[i, :] = [point.attrib['distance'], float(point.attrib['value'])]
+        rho[i, :] = [point.attrib["distance"], float(point.attrib["value"])]
     return rho
 
 
 def parse_kerr(name: str) -> dict:
     """
     Parser for KERR.OUT
 
     :param str name: File name
     :return dict output: Parsed data
     """
     try:
         data = np.genfromtxt(name, skip_header=1)
-    except:
+    except Exception:
         raise ParseError
 
-    out = {'energy': data[:, 0], 're': data[:, 1], 'im': data[:, 2]}
+    out = {"energy": data[:, 0], "re": data[:, 1], "im": data[:, 2]}
 
     return out
 
 
 def parse_epsilon(name: str) -> dict:
     """
     Parser for EPSILON_ij.OUT
 
     :param str name: File name
     :return dict output: Parsed data
     """
     try:
         data = np.genfromtxt(name, skip_header=1)
-    except:
+    except Exception:
         raise ParseError
-    out = {'energy': data[:, 0], 're': data[:, 1], 'im': data[:, 2]}
+    out = {"energy": data[:, 0], "re": data[:, 1], "im": data[:, 2]}
     return out
 
 
 def parse_chi(name: str) -> dict:
     """
     Parser for CHI_111.OUT
 
     :param str name: File name
     :return dict output: Parsed data
     """
     try:
         data = np.genfromtxt(name, skip_header=1)
-    except:
+    except Exception:
         raise ParseError
-    out = {
-        'energy': data[:, 0],
-        're': data[:, 1],
-        'im': data[:, 2],
-        'modulus': data[:, 3]
-    }
+    out = {"energy": data[:, 0], "re": data[:, 1], "im": data[:, 2], "modulus": data[:, 3]}
     return out
 
 
 def parse_elnes(name: str) -> dict:
     """
     Parser for ELNES.OUT
 
     :param str name: File name
     :return dict output: Parsed data
     """
     try:
         data = np.genfromtxt(name)
-    except:
+    except Exception:
         raise ParseError
-    out = {'energy': data[:, 0], 'elnes': data[:, 1]}
+    out = {"energy": data[:, 0], "elnes": data[:, 1]}
     return out
 
 
 def parse_seebeck(name: str) -> dict:
     """
     Parser for SEEBECK_11.OUT
 
     :param str name: File name
     :return dict output: Parsed data
     """
     try:
         data = np.genfromtxt(name)
-    except:
+    except Exception:
         raise ParseError
-    out = {
-        'temperature': data[:, 0],
-        'mu': data[:, 1],
-        're': data[:, 2],
-        'im': data[:, 3]
-    }
+    out = {"temperature": data[:, 0], "mu": data[:, 1], "re": data[:, 2], "im": data[:, 3]}
 
     return out
 
 
 def parse_ldos(name: str) -> dict:
     """
     Parser for ldos.out
 
     :param str name: File name
     :return dict output: Parsed data
     """
     try:
         data = np.genfromtxt(name)
-    except:
+    except Exception:
         raise ParseError
-    out = {'energy': data[:, 0], 'ldos': data[:, 1]}
+    out = {"energy": data[:, 0], "ldos": data[:, 1]}
 
     return out
 
 
 def parse_band_edges(name: str) -> dict:
     """
     Parser for band_edges.out
@@ -505,17 +490,17 @@
     * CBm = Conduction band minimum
 
     :param str name: File name
     :return dict output: Parsed data
     """
     try:
         data = np.genfromtxt(name)
-    except:
+    except Exception:
         raise ParseError
-    out = {'c_axis': data[:, 0], 'VBM': data[:, 1], 'CBm': data[:, 2]}
+    out = {"c_axis": data[:, 0], "VBM": data[:, 1], "CBm": data[:, 2]}
 
     return out
 
 
 def parse_spintext(name: str) -> dict:
     """
     Parse spintext.xml
@@ -525,78 +510,67 @@
     Each element of the list contains a dict with keys:
      ['ist', 'k-point', 'spin', 'energy']
 
     :param str name: Path to the spintext.xml that will be parsed
     :return dict spintext: List that holds the parsed spintexture.xml
     """
     # parse file
-    file_name = 'spintext.xml'
-    if name.split('/')[-1] != file_name:
+    file_name = "spintext.xml"
+    if name.split("/")[-1] != file_name:
         name = os.path.join(name, file_name)
 
     tree_spin = ET.parse(name)
     root_spin = tree_spin.getroot()
 
     spintext = {}
-    i = 0
-    for band in root_spin.findall("band"):
+    for i, band in enumerate(root_spin.findall("band")):
         k_point = []
         spin = []
         energy = []
 
         for val in band.findall("k-point"):
             k_point.append([float(k) for k in val.attrib["vec"].split()])
             spin.append([float(s) for s in val.attrib["spin"].split()])
             energy.append(float(val.attrib["energy"]))
 
-        spintext[str(i)] = {
-            "ist": int(band.attrib["ist"]),
-            "k-point": k_point,
-            "spin": spin,
-            "energy": energy
-        }
-        i += 1
+        spintext[str(i)] = {"ist": int(band.attrib["ist"]), "k-point": k_point, "spin": spin, "energy": energy}
 
     return spintext
 
 
 @set_return_values
 def parse_polarization(name: str) -> dict:
     """
     Parser for POLARIZATION.OUT
 
     :param str name: File name
     :return dict output: Parsed data
     """
     file = open(name)
     lines = []
-    for i in range(len(open(name).readlines())):
+    for _ in range(len(open(name).readlines())):
         line = next(file)
-        if '#' not in line:
+        if "#" not in line:
             lines.append(line.split())
-    polarization = {
-        'total': lines[0],
-        'electronic': lines[1],
-        'ionic': lines[2]
-    }
+    polarization = {"total": lines[0], "electronic": lines[1], "ionic": lines[2]}
     return polarization
 
 
 def parse_tdos_wannier(name: str) -> dict:
     """
     Parser for TDOS_WANNIER.OUT
 
     :param str name: File name
     :return dict output: Parsed data
     """
     try:
         data = np.genfromtxt(name)
-    except:
+    except Exception:
         raise ParseError
-    out = {'energy': data[:, 0], 'dos': data[:, 1]}
+    out = {"energy": data[:, 0], "dos": data[:, 1]}
 
     return out
 
 
 def parse_wannier_info(name: str) -> dict:
     """
     Parser for WANNIER_INFO.OUT
@@ -612,53 +586,43 @@
     total = []
     start = False
     for i, line in enumerate(file.readlines()):
         if "* Wannier functions" in line:
             start = True
         if start:
             lines.append(line)
-    for i in range(len(lines)):
-        if lines[i].strip().startswith('1'):
-            for j in range(4):
-                data.append(lines[i + j].split())
-        if lines[i].strip().startswith('5'):
-            for j in range(4):
-                data.append(lines[i + j].split())
-        if lines[i].strip().startswith('total'):
-            total.append(lines[i].split())
+    for i, line in enumerate(lines):
+        if line.strip().startswith("1") or line.strip().startswith("5"):
+            data.extend(lines[i + j].split() for j in range(4))
+        elif line.strip().startswith("total"):
+            total.append(line.split())
     file.close()
 
     # Package data into dictionary
     n_wannier = len(data)
     localisation_center = np.empty(shape=(n_wannier, 3))
-    wannier = {
-        'n_wannier': n_wannier,
-        'Omega': [],
-        'Omega_I': [],
-        'Omega_D': [],
-        'Omega_OD': []
-    }
+    wannier = {"n_wannier": n_wannier, "Omega": [], "Omega_I": [], "Omega_D": [], "Omega_OD": []}
 
     for i, item in enumerate(data):
         localisation_center[i, :] = [float(x) for x in item[1:4]]
-        wannier['Omega'].append(float(item[4]))
-        wannier['Omega_I'].append(float(item[5]))
-        wannier['Omega_D'].append(float(item[6]))
-        wannier['Omega_OD'].append(float(item[7]))
+        wannier["Omega"].append(float(item[4]))
+        wannier["Omega_I"].append(float(item[5]))
+        wannier["Omega_D"].append(float(item[6]))
+        wannier["Omega_OD"].append(float(item[7]))
 
-    wannier['localisation_center'] = localisation_center
+    wannier["localisation_center"] = localisation_center
 
-    totals = {'Omega': [], 'Omega_I': [], 'Omega_D': [], 'Omega_OD': []}
+    totals = {"Omega": [], "Omega_I": [], "Omega_D": [], "Omega_OD": []}
     for j, item in enumerate(total):
-        totals['Omega'].append(float(item[1]))
-        totals['Omega_I'].append(float(item[2]))
-        totals['Omega_D'].append(float(item[3]))
-        totals['Omega_OD'].append(float(item[4]))
+        totals["Omega"].append(float(item[1]))
+        totals["Omega_I"].append(float(item[2]))
+        totals["Omega_D"].append(float(item[3]))
+        totals["Omega_OD"].append(float(item[4]))
 
-    wannier['total'] = totals
+    wannier["total"] = totals
 
     return wannier
 
 
 def parse_core_overlap(name: str) -> dict:
     """
     Parser for coreoverlap.xml
@@ -680,35 +644,34 @@
        n_pairs]
 
     :param str name: File name
     :return dict output: Parsed data
     """
     try:
         tree = ET.parse(name)
-    except:
+    except Exception:
         raise ParseError
 
     root = tree.getroot()
     core_overlap = {
-        'nkpt': int(root.attrib['nkpt']),
-        'nstfv': int(root.attrib['nstfv']),
-        'ncg': int(root.attrib['ncg'])
+        "nkpt": int(root.attrib["nkpt"]),
+        "nstfv": int(root.attrib["nstfv"]),
+        "ncg": int(root.attrib["ncg"]),
     }
 
     k_points = []
     for k_point in root:
-        kpt = {"index": int(k_point.attrib['index'])}
+        kpt = {"index": int(k_point.attrib["index"])}
         pairs = []
         for pair_xml in k_point:
             pair = pair_xml.attrib
-            pair['ist1'] = int(pair['ist1'])
-            pair['ist2'] = int(pair['ist2'])
+            pair["ist1"] = int(pair["ist1"])
+            pair["ist2"] = int(pair["ist2"])
             pair["de"] = float(pair["de"])
-            pair["overlap"] = float(pair["overlap"].split()[0]) ** 2 + float(
-                pair["overlap"].split()[1]) ** 2
+            pair["overlap"] = float(pair["overlap"].split()[0]) ** 2 + float(pair["overlap"].split()[1]) ** 2
             pairs.append(pair)
         kpt["pairs"] = pairs
         k_points.append(kpt)
     core_overlap["kpoints"] = k_points
 
     return core_overlap
 
@@ -718,191 +681,191 @@
     Parses files containing loss function
     e.g. LOSS_FXCRPA_OC11_QMT001.OUT
 
     :param str fname: name of the file
     """
     xdata = []
     ydata = []
-    file = open(fname, 'r')
+    file = open(fname)
     for lines in file:
-        if 'Frequency' in lines:
+        if "Frequency" in lines:
             break
     for lines in file:
         data = lines.split()
         xdata.append(float(data[0]))
         ydata.append(float(data[1]))
     file.close()
     return xdata, ydata
 
 
 def parse_wf1d(fname: str) -> dict:
-  """
-  Parses files containing one dimensional wave function plot as saved in
-  the files, _e.g._, wf1d-0001-0001.dat, where the first 0001 indicates the k-point
-  and the second the state index.
-  
-  :param str fname: name of the file
-  """
-
-  data = np.genfromtxt(fname)
-
-  output = {}
-  output["path"] = data[:, 0]
-  output["|psi|^2"] = data[:, 1]
-  output["Re(psi)"] = data[:, 2]
-  output["Im(psi)"] = data[:, 3]
+    """
+    Parses files containing one dimensional wave function plot as saved in
+    the files, _e.g._, wf1d-0001-0001.dat, where the first 0001 indicates the k-point
+    and the second the state index.
 
-  return output 
+    :param str fname: name of the file
+    """
+
+    data = np.genfromtxt(fname)
+
+    output = {}
+    output["path"] = data[:, 0]
+    output["|psi|^2"] = data[:, 1]
+    output["Re(psi)"] = data[:, 2]
+    output["Im(psi)"] = data[:, 3]
+
+    return output
 
 
 def parse_wf2d(fname: str) -> dict:
-  """
-  Parses files containing the two dimensional wave function plot as saved in the files,
-  _e.g._, wf2d-0001-0001.xsf, where the first 0001 indicates the k-point
-  and the second the state index.
-
-  Does not parse PRIMVEC and PRIMCOORD. These can be parsed with ase.io.read(fname).
-
-  :param str fname: name of the file
-  """
-
-  file = open(fname, 'r')
-  lines = file.readlines()
-  output = {}
-  
-  i = 0
-  while i < len(lines):
-    if 'BEGIN_BLOCK_DATAGRID_2D' in lines[i]:
-      i = i + 1
-      data_name = lines[i].replace('\n', '').lstrip()
-      
-      i = i + 2
-      grid = np.fromstring(lines[i], dtype=int, sep=' ')
-
-      i = i + 1
-      origin = np.fromstring(lines[i], dtype=np.double, sep = ' ')
-      
-      i = i + 1
-      point1 = np.fromstring(lines[i], dtype=np.double, sep = ' ')
-      
-      i = i + 1
-      point2 = np.fromstring(lines[i], dtype=np.double, sep = ' ')
-
-      i = i + 1
-      data = np.fromstring(lines[i], dtype=np.double, sep=' ')
-      while 'END_DATAGRID_2D' not in lines[i]:
-        i = i + 1
-        new_data = np.fromstring(lines[i], dtype=np.double, sep=' ')
-        data = np.concatenate((data, new_data), axis=None)
-    
-      output['grid'] = grid
-      output['origin'] = origin
-      output['point1'] = point1
-      output['point2'] = point2
-      output[data_name] = data # data_name: "module squared", "real", "imaginary"
+    """
+    Parses files containing the two dimensional wave function plot as saved in the files,
+    _e.g._, wf2d-0001-0001.xsf, where the first 0001 indicates the k-point
+    and the second the state index.
+
+    Does not parse PRIMVEC and PRIMCOORD. These can be parsed with ase.io.read(fname).
+
+    :param str fname: name of the file
+    """
+
+    file = open(fname)
+    lines = file.readlines()
+    output = {}
+
+    i = 0
+    while i < len(lines):
+        if "BEGIN_BLOCK_DATAGRID_2D" in lines[i]:
+            i = i + 1
+            data_name = lines[i].replace("\n", "").lstrip()
+
+            i = i + 2
+            grid = np.fromstring(lines[i], dtype=int, sep=" ")
+
+            i = i + 1
+            origin = np.fromstring(lines[i], dtype=np.double, sep=" ")
+
+            i = i + 1
+            point1 = np.fromstring(lines[i], dtype=np.double, sep=" ")
 
-    i = i + 1
+            i = i + 1
+            point2 = np.fromstring(lines[i], dtype=np.double, sep=" ")
+
+            i = i + 1
+            data = np.fromstring(lines[i], dtype=np.double, sep=" ")
+            while "END_DATAGRID_2D" not in lines[i]:
+                i = i + 1
+                new_data = np.fromstring(lines[i], dtype=np.double, sep=" ")
+                data = np.concatenate((data, new_data), axis=None)
+
+            output["grid"] = grid
+            output["origin"] = origin
+            output["point1"] = point1
+            output["point2"] = point2
+            output[data_name] = data  # data_name: "module squared", "real", "imaginary"
+
+        i = i + 1
 
-  return output
+    return output
 
 
 def parse_wf3d(fname: str) -> dict:
-  """
-  Parses files containing the two dimensional wave function plot as saved in the files,
-  _e.g._, wf3d-0001-0001.xsf, where the first 0001 indicates the k-point
-  and the second the state index.
-
-  Does not parse PRIMVEC and PRIMCOORD. These can be parsed with ase.io.read(fname).
-
-  :param str fname: name of the file
-  """
-
-  file = open(fname, 'r')
-  lines = file.readlines()
-  output = {}
-  
-  i = 0
-  while i < len(lines):
-    if 'BEGIN_BLOCK_DATAGRID_3D' in lines[i]:
-      i = i + 1
-      data_name = lines[i].replace('\n', '').lstrip()
-      
-      i = i + 2
-      grid = np.fromstring(lines[i], dtype=int, sep=' ')
-
-      i = i + 1
-      origin = np.fromstring(lines[i], dtype=np.double, sep = ' ')
-      
-      i = i + 1
-      point1 = np.fromstring(lines[i], dtype=np.double, sep = ' ')
-      
-      i = i + 1
-      point2 = np.fromstring(lines[i], dtype=np.double, sep = ' ')
-
-      i = i + 1
-      point3 = np.fromstring(lines[i], dtype=np.double, sep = ' ')
-
-      i = i + 1
-      data = np.fromstring(lines[i], dtype=np.double, sep=' ')
-      while 'END_DATAGRID_3D' not in lines[i]:
+    """
+    Parses files containing the two dimensional wave function plot as saved in the files,
+    _e.g._, wf3d-0001-0001.xsf, where the first 0001 indicates the k-point
+    and the second the state index.
+
+    Does not parse PRIMVEC and PRIMCOORD. These can be parsed with ase.io.read(fname).
+
+    :param str fname: name of the file
+    """
+
+    file = open(fname)
+    lines = file.readlines()
+    output = {}
+
+    i = 0
+    while i < len(lines):
+        if "BEGIN_BLOCK_DATAGRID_3D" in lines[i]:
+            i = i + 1
+            data_name = lines[i].replace("\n", "").lstrip()
+
+            i = i + 2
+            grid = np.fromstring(lines[i], dtype=int, sep=" ")
+
+            i = i + 1
+            origin = np.fromstring(lines[i], dtype=np.double, sep=" ")
+
+            i = i + 1
+            point1 = np.fromstring(lines[i], dtype=np.double, sep=" ")
+
+            i = i + 1
+            point2 = np.fromstring(lines[i], dtype=np.double, sep=" ")
+
+            i = i + 1
+            point3 = np.fromstring(lines[i], dtype=np.double, sep=" ")
+
+            i = i + 1
+            data = np.fromstring(lines[i], dtype=np.double, sep=" ")
+            while "END_DATAGRID_3D" not in lines[i]:
+                i = i + 1
+                new_data = np.fromstring(lines[i], dtype=np.double, sep=" ")
+                data = np.concatenate((data, new_data), axis=None)
+
+            output["grid"] = grid
+            output["origin"] = origin
+            output["point1"] = point1
+            output["point2"] = point2
+            output["point3"] = point3
+            output[data_name] = data  # data_name: "module squared", "real", "imaginary"
+
         i = i + 1
-        new_data = np.fromstring(lines[i], dtype=np.double, sep=' ')
-        data = np.concatenate((data, new_data), axis=None)
-    
-      output['grid'] = grid
-      output['origin'] = origin
-      output['point1'] = point1
-      output['point2'] = point2
-      output['point3'] = point3
-      output[data_name] = data # data_name: "module squared", "real", "imaginary"
 
-    i = i + 1
+    return output
 
-  return output  
 
 def parse_cube(fname: str) -> dict:
-  """
-  Parses .cube files. These files contain data calculated on a regular grid in a box.
-  All vectors are given in cartesian coordinates. `output['cube_data']` contains the data. 
-  It is described by `output['description']`.
-
-  :param str fname: name of the file
-  """
-
-  file = open(fname, 'r')
-  lines = file.readlines()
-  output = {}
-
-  output['title'] = str(lines[0])
-  output['description'] = str(lines[1])
-
-  n_atoms = int(lines[2].split()[0])
-  output['n_atoms'] = n_atoms
-  output['origin'] = np.array(lines[2].split()[1:], dtype=np.double)
-
-  output['n_1'] = int(lines[3].split()[0])
-  output['v_increment_1'] = np.array(lines[3].split()[1:], dtype=np.double)
-
-  output['n_2'] = int(lines[4].split()[0])
-  output['v_increment_2'] = np.array(lines[4].split()[1:], dtype=np.double)
-
-  output['n_3'] = int(lines[5].split()[0])
-  output['v_increment_3'] = np.array(lines[5].split()[1:], dtype=np.double)
-
-  line_offset = 6
-  output['atoms'] = []
-  for line in lines[line_offset : line_offset + n_atoms]:
-      atom_number = int(line.split()[0])
-      charge = np.double(line.split()[1])
-      coordinate = np.array(line.split()[2:], dtype=np.double)
-      output['atoms'].append(dict(atom_number=atom_number, charge=charge, coordinate=coordinate))
-
-  line_offset = line_offset + n_atoms
-
-  cube_data = []
-  for line in lines[line_offset:]:
-      cube_data = cube_data + line.split()
-  
-  output['cube_data'] = np.array(cube_data, dtype=np.double)
+    """
+    Parses .cube files. These files contain data calculated on a regular grid in a box.
+    All vectors are given in cartesian coordinates. `output['cube_data']` contains the data.
+    It is described by `output['description']`.
+
+    :param str fname: name of the file
+    """
+
+    file = open(fname)
+    lines = file.readlines()
+    output = {}
+
+    output["title"] = str(lines[0])
+    output["description"] = str(lines[1])
+
+    n_atoms = int(lines[2].split()[0])
+    output["n_atoms"] = n_atoms
+    output["origin"] = np.array(lines[2].split()[1:], dtype=np.double)
+
+    output["n_1"] = int(lines[3].split()[0])
+    output["v_increment_1"] = np.array(lines[3].split()[1:], dtype=np.double)
+
+    output["n_2"] = int(lines[4].split()[0])
+    output["v_increment_2"] = np.array(lines[4].split()[1:], dtype=np.double)
+
+    output["n_3"] = int(lines[5].split()[0])
+    output["v_increment_3"] = np.array(lines[5].split()[1:], dtype=np.double)
+
+    line_offset = 6
+    output["atoms"] = []
+    for line in lines[line_offset : line_offset + n_atoms]:
+        atom_number = int(line.split()[0])
+        charge = np.double(line.split()[1])
+        coordinate = np.array(line.split()[2:], dtype=np.double)
+        output["atoms"].append(dict(atom_number=atom_number, charge=charge, coordinate=coordinate))
+
+    line_offset = line_offset + n_atoms
+
+    cube_data = []
+    for line in lines[line_offset:]:
+        cube_data = cube_data + line.split()
+
+    output["cube_data"] = np.array(cube_data, dtype=np.double)
 
-  return output
-  
+    return output
```

### Comparing `excitingtools-1.7.0/excitingtools/exciting_dict_parsers/species_parser.py` & `excitingtools-1.7.1/excitingtools/exciting_dict_parsers/species_parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-""" Parse exciting species files into dictionary.
-"""
+"""Parse exciting species files into dictionary."""
+
 from typing import Dict
 
 from excitingtools.parser_utils.parser_decorators import xml_root
 from excitingtools.parser_utils.parser_utils import convert_string_dict
 
 
 @xml_root
 def parse_species_xml(root) -> dict:
-    """ Parses exciting species files as a dict.
+    """Parses exciting species files as a dict.
 
     TODO(Alex) Issue 124. See how easy it is to replace with a generic XML
     parser, with keys defined according to the associated schema.
 
     Return a dictionary with elements:
 
       species = {'chemicalSymbol': chemicalSymbol, 'name': name, 'z': z, 'mass': mass}
@@ -36,40 +36,31 @@
                     ...]
 
     :param root: XML file, XML string, or an ET.Element.
     :return : Dictionary of species file data (described above).
     """
     species_tree = root[0]
     species = convert_string_dict(species_tree.attrib)
-    
-    children: Dict[str, list] = {'atomicState': [], 'basis': [], 'muffinTin': []}
+
+    children: Dict[str, list] = {"atomicState": [], "basis": [], "muffinTin": []}
     for child in list(species_tree):
         children[child.tag].append(child)
 
-    assert len(children['muffinTin']) == 1, "More than one muffinTin sub-tree in the species file"
-    assert len(children['basis']) == 1, "More than one basis sub-tree in the species file"
+    assert len(children["muffinTin"]) == 1, "More than one muffinTin sub-tree in the species file"
+    assert len(children["basis"]) == 1, "More than one basis sub-tree in the species file"
 
-    muffin_tin = convert_string_dict(children['muffinTin'][0].attrib)
+    muffin_tin = convert_string_dict(children["muffinTin"][0].attrib)
 
-    atomic_states = []
-    for atomic_state_tree in children['atomicState']:
-        atomic_states.append(convert_string_dict(atomic_state_tree.attrib))
+    atomic_states = [convert_string_dict(atomic_state_tree.attrib) for atomic_state_tree in children["atomicState"]]
 
-    basis_tree = children['basis'][0]
-    basis: Dict[str, list] = {'default': [], 'custom': [], 'lo': []}
+    basis_tree = children["basis"][0]
+    basis: Dict[str, list] = {"default": [], "custom": [], "lo": []}
 
     for func in basis_tree:
         parsed_attributes = convert_string_dict(func.attrib)
 
-        if func.tag == 'lo':
+        if func.tag == "lo":
             parsed_attributes["wf"] = [convert_string_dict(wf.attrib) for wf in func]
-        
-        basis[func.tag].append(parsed_attributes)
-
-    return {
-        'species': species,
-        'muffin_tin': muffin_tin,
-        'atomic_states': atomic_states,
-        'basis': basis
-        }
 
+        basis[func.tag].append(parsed_attributes)
 
+    return {"species": species, "muffin_tin": muffin_tin, "atomic_states": atomic_states, "basis": basis}
```

### Comparing `excitingtools-1.7.0/excitingtools/exciting_dict_parsers/state_parser.py` & `excitingtools-1.7.1/excitingtools/exciting_dict_parsers/state_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,88 +1,86 @@
-""" Parser for STATE.OUT binary file.
-"""
-import numpy as np
+"""Parser for STATE.OUT binary file."""
+
 import struct
 import sys
 
+import numpy as np
+
 
 def get_byteorder_format_char(byteorder) -> str:
-    """ Converts the byteorder string to formatting symbol for struct.unpack function
+    """Converts the byteorder string to formatting symbol for struct.unpack function
 
     :param byteorder: endianness of the byteorder ("little" or "big")
     :return: the character representing the endianness ('<' or '>')
     """
-    chars = {
-        "little": '<',
-        "big": '>',
-    }
+    chars = {"little": "<", "big": ">"}
     return chars[byteorder]
 
 
 def read_array(file, shape, byteorder) -> np.ndarray:
-    """ Read in a sequence of double values and reshape them into the wanted shape.
+    """Read in a sequence of double values and reshape them into the wanted shape.
 
     :param file: binary file object, which contains the number sequence
     :param shape: the desired shape of the number sequence (with column-major order)
     :param byteorder: the endianness of the bytes representation
     :return: a numpy array of double values with the desired shape
     """
     # get the correct format character for the byteorder
     byteorder = get_byteorder_format_char(byteorder)
     # get the number of bytes for the array
     num_bytes = np.prod(shape) * 8
     # get all the double numbers
     values = struct.unpack(f"{byteorder}{np.prod(shape)}d", file.read(num_bytes))
     # return the values as correctly shaped numpy array
-    return np.reshape(values, shape, order='F')
+    return np.reshape(values, shape, order="F")
 
 
 def read_complex_array(file, shape, byteorder) -> np.ndarray:
-    """ Read in a sequence of complex values and reshape them into the wanted shape.
+    """Read in a sequence of complex values and reshape them into the wanted shape.
 
     :param file: binary file object, which contains the number sequence
     :param shape: the desired shape of the number sequence (with column-major order)
     :param byteorder: the endianness of the bytes representation
     :return: a numpy array of complex values with the desired shape
     """
     byteorder = get_byteorder_format_char(byteorder)
     array = np.reshape(
-        [complex(*struct.unpack(f"{byteorder}2d", file.read(16))) for _ in range(np.prod(shape))], shape, order='F'
+        [complex(*struct.unpack(f"{byteorder}2d", file.read(16))) for _ in range(np.prod(shape))], shape, order="F"
     )
     return array
 
 
 def read_int(file, byteorder, num_bytes=4, signed=False) -> int:
-    """ Read in a single integer.
+    """Read in a single integer.
 
     :param file: binary file object, which contains the number
     :param byteorder: the endianness of the bytes representation
     :param num_bytes: the number of bytes, which constitute the integer
     :param signed: weather the bytes should be interpreted as a signed or unsigned integer
     :return: the read in integer
     """
     return int.from_bytes(file.read(num_bytes), byteorder, signed=signed)
 
 
 def read_integers(file, integers, dest, byteorder):
-    """ Read in a sequence of named integers and store them in a dictionary.
+    """Read in a sequence of named integers and store them in a dictionary.
 
     :param file: binary file object, which contains the integers
     :param integers: the keys of the integers for the dictionary
     :param dest: the dictionary, which stores the integers and gets modified
     :param byteorder: the endianness of the bytes representation
     """
     for integer in integers:
         num_bytes = read_int(file, byteorder)
         dest[integer] = read_int(file, byteorder, num_bytes)
         assert num_bytes == read_int(file, byteorder)
 
 
 def parse_state_out(path, byteorder=sys.byteorder) -> dict:
-    """ Parser for: STATE.OUT
+    """Parser for: STATE.OUT
 
     STATE.OUT is a binary file. For every 'Write' (in Fortran) there are 4 leading bytes, which are an integer
     equal to the number of bytes of the Fortran objects written. After this the leading 4 bytes are
     repeated.
     This file contains information about the version of exciting, which was used and all the information about
     the density and potentials.
     The functions for the muffin-tin region are stored as an expansion of real spherical harmonics.
```

### Comparing `excitingtools-1.7.0/excitingtools/exciting_obj_parsers/eigenvalue_parser.py` & `excitingtools-1.7.1/excitingtools/exciting_obj_parsers/eigenvalue_parser.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-""" Eigenvalue parser, processing dict values and returning to an object.
-"""
+"""Eigenvalue parser, processing dict values and returning to an object."""
 
 import numpy as np
-from excitingtools.exciting_dict_parsers.groundstate_parser import parse_eigval
-from excitingtools.dataclasses.eigenvalues import EigenValues
+
 from excitingtools.dataclasses.data_structs import NumberOfStates
+from excitingtools.dataclasses.eigenvalues import EigenValues
+from excitingtools.exciting_dict_parsers.groundstate_parser import parse_eigval
 
 
 def parse_eigenvalues(root) -> EigenValues:
-    """ High-level parser for eigenvalues. Calls dictionary parser to parse information from the "eigval.xml" file.
+    """High-level parser for eigenvalues. Calls dictionary parser to parse information from the "eigval.xml" file.
 
     :param root: XML file name, XML string or ElementTree.Element as input.
     :return: EigenValues object.
     """
 
     eigval_dict = parse_eigval(root)
-    data = eigval_dict['kpt']
+    data = eigval_dict["kpt"]
 
-    k_points = []
-    for point in data.values():
-        k_points.append([float(x) for x in point['vkl'].split()])
+    k_points = [[float(x) for x in point["vkl"].split()] for point in data.values()]
 
     k_indices = list(map(int, data.keys()))
 
     n_k = len(k_points)
-    n_e = len(data['1']['state'])
+    n_e = len(data["1"]["state"])
     eigenvalues = np.empty((n_k, n_e))
     occupations = np.empty((n_k, n_e))
 
     for ik in range(n_k):
         for ie in range(n_e):
-            eigenvalues[ik, ie] = data[str(ik + 1)]['state'][str(ie + 1)]['eigenvalue']
-            occupations[ik, ie] = data[str(ik + 1)]['state'][str(ie + 1)]['occupancy']
+            eigenvalues[ik, ie] = data[str(ik + 1)]["state"][str(ie + 1)]["eigenvalue"]
+            occupations[ik, ie] = data[str(ik + 1)]["state"][str(ie + 1)]["occupancy"]
 
-    return EigenValues(state_range=NumberOfStates(1, occupations.shape[1]),
-                       k_points=k_points,
-                       k_indices=k_indices,
-                       all_eigenvalues=eigenvalues,
-                       occupations=occupations)
+    return EigenValues(
+        state_range=NumberOfStates(1, occupations.shape[1]),
+        k_points=k_points,
+        k_indices=k_indices,
+        all_eigenvalues=eigenvalues,
+        occupations=occupations,
+    )
```

### Comparing `excitingtools-1.7.0/excitingtools/exciting_obj_parsers/gw_eigenvalues.py` & `excitingtools-1.7.1/excitingtools/exciting_obj_parsers/gw_eigenvalues.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-""" GW eigenvalue parser, processing dict values and returning to an object.
-"""
-import os
-from typing import Optional, List, Union, Dict
+"""GW eigenvalue parser, processing dict values and returning to an object."""
+
 import enum
+import os
+from typing import Dict, List, Optional, Union
+
 import numpy as np
 
-from excitingtools.exciting_dict_parsers.gw_eigenvalues_parser import parse_evalqp, _file_name, parse_gw_dos
 from excitingtools.dataclasses.data_structs import NumberOfStates
-from excitingtools.dataclasses.eigenvalues import EigenValues
 from excitingtools.dataclasses.density_of_states import DOS
+from excitingtools.dataclasses.eigenvalues import EigenValues
+from excitingtools.exciting_dict_parsers.gw_eigenvalues_parser import _file_name, parse_evalqp, parse_gw_dos
 
 
 class NitrogenEvalQPColumns(enum.Enum):
     E_KS = 0
     E_HF = 1
     E_GW = 2
     Sx = 3
@@ -22,14 +23,15 @@
     DE_GW = 7
     Znk = 8
 
 
 class OxygenEvalQPColumns(enum.Enum):
     """Columns of `_file_name`, for exciting oxygen
     excluding the state index."""
+
     E_KS = 0
     E_HF = 1
     E_GW = 2
     Sx = 3
     Re_Sc = 4
     Im_Sc = 5
     Vxc = 6
@@ -42,67 +44,67 @@
 columns_type = Union[enum.Enum, List[enum.Enum]]
 
 # Return an instance of EigenValues, or a dicts of EigenValues if the user asks for
 # multiple data columns.
 return_type = Union[EigenValues, Dict[enum.Enum, EigenValues]]
 
 
-def gw_eigenvalue_parser(input_file_path: str, columns: Optional[columns_type] = OxygenEvalQPColumns.E_GW) -> \
-        return_type:
-    """ High-level Parser for GW eigenvalues file.
+def gw_eigenvalue_parser(
+    input_file_path: str, columns: Optional[columns_type] = OxygenEvalQPColumns.E_GW
+) -> return_type:
+    """High-level Parser for GW eigenvalues file.
 
     Unpacks the result of dict into a sensible form and returns the data to return_type.
 
     :param input_file_path: File path (can include or exclude file name).
     :param columns: Optional choice for which data column of energies to return. Default is to return
     GW eigenvalues, assuming exciting oxygen (most recent release).
     :return An instance of EigenValues, or a dict of (key, value) = [EvalQPColumns, EigenValues].
     """
     path, file_name = os.path.split(input_file_path)
-    if file_name == _file_name:
-        file_path = path
-    else:
-        file_path = input_file_path
+    file_path = path if file_name == _file_name else input_file_path
     abs_file_name = os.path.join(file_path, _file_name)
 
     if not isinstance(columns, list):
         columns = [columns]
 
     # Parse data
     data: dict = parse_evalqp(abs_file_name)
-    state_range_list: List[int] = data.pop('state_range')
-    column_enums = data.pop('column_labels')
+    state_range_list: List[int] = data.pop("state_range")
+    column_enums = data.pop("column_labels")
 
     n_k = len(data.keys())
     state_range = NumberOfStates(state_range_list[0], state_range_list[1])
 
     # Check for inconsistency between requested column and columns available (i.e. data produced with
     # different code versions)
     # Because the parsed column data class is dynamically-generated, one has to do it with lengths
     parsed_column_names = {enum.value for enum in column_enums}
     requested_column_names = {enum.value for enum in type(columns[0])}
 
     if (requested_column_names - parsed_column_names) != set():
         enum_class_name = type(columns[0]).__name__
-        raise ValueError(f'The requested data column is indexed according to exciting version {enum_class_name},'
-                         f'which is not consistent with the columns of the parsed data.'
-                         f' Check that your data was produced with the same code version.')
+        raise ValueError(
+            f"The requested data column is indexed according to exciting version {enum_class_name},"
+            f"which is not consistent with the columns of the parsed data."
+            f" Check that your data was produced with the same code version."
+        )
 
     # Repackage data
     k_indices = []
     k_points = []
     weights = []
     n_columns = len(type(columns[0]))
     all_eigenvalues = np.empty(shape=(n_k, state_range.n_states, n_columns))
 
     for ik, k_block in data.items():
         k_indices.append(ik)
-        k_points.append(k_block['k_point'])
-        weights.append(k_block['weight'])
-        all_eigenvalues[ik - 1, :, :] = k_block['energies'][:, :]
+        k_points.append(k_block["k_point"])
+        weights.append(k_block["weight"])
+        all_eigenvalues[ik - 1, :, :] = k_block["energies"][:, :]
 
     # Return data
     if len(columns) == 1:
         return EigenValues(state_range, k_points, k_indices, all_eigenvalues[:, :, columns[0].value], weights)
 
     eigen_values = {}
     for column in columns:
@@ -117,8 +119,8 @@
 def parse_obj_gw_dos(full_file_name: str) -> DOS:
     """High-level parser for GW DOS files.
 
     :param full_file_name: Path + file name
     :return: DOS object
     """
     gw_dos_data = parse_gw_dos(full_file_name)
-    return DOS(gw_dos_data['energy'], gw_dos_data['dos'])
+    return DOS(gw_dos_data["energy"], gw_dos_data["dos"])
```

### Comparing `excitingtools-1.7.0/excitingtools/exciting_obj_parsers/input_xml.py` & `excitingtools-1.7.1/excitingtools/exciting_obj_parsers/input_xml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-""" Parse input XML data directly into corresponding python classes.
-"""
+"""Parse input XML data directly into corresponding python classes."""
 
 from excitingtools.exciting_dict_parsers.input_parser import parse_input_xml as parse_input_xml_to_dict
 from excitingtools.input.input_xml import ExcitingInputXML
 from excitingtools.parser_utils.parser_decorators import xml_root
 
 
 @xml_root
 def parse_input_xml(root) -> ExcitingInputXML:
-    """ Parse exciting input.xml into the corresponding python ExcitingInput Objects.
+    """Parse exciting input.xml into the corresponding python ExcitingInput Objects.
     :param root: Input for the parser.
     :returns: the exciting input object
     """
     element_dict: dict = parse_input_xml_to_dict(root)
     return ExcitingInputXML(**element_dict)
```

### Comparing `excitingtools-1.7.0/excitingtools/exciting_obj_parsers/ks_band_structure.py` & `excitingtools-1.7.1/excitingtools/exciting_obj_parsers/ks_band_structure.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,32 @@
-""" KS (ground state) Band structure Parser, returning to an object.
-"""
+"""KS (ground state) Band structure Parser, returning to an object."""
 
 import os
+from pathlib import Path
+
 import numpy as np
+
 from excitingtools.dataclasses.band_structure import BandData
-from excitingtools.exciting_dict_parsers.properties_parser import parse_band_structure_xml, parse_band_structure_dat
-from pathlib import Path
+from excitingtools.exciting_dict_parsers.properties_parser import parse_band_structure_dat, parse_band_structure_xml
 
 
 def parse_band_structure(file_name: str) -> BandData:
-    """ High-level parser for KS band structure. Calls dictionary parsers to parse information from both
+    """High-level parser for KS band structure. Calls dictionary parsers to parse information from both
     "bandstructure.xml" and "bandstructure.dat" files.
 
     :param str file_name: File name for band structure such as "bandstructure.dat", "bandstructure.xml" or
                           "bandstructure"
     :return: BandData object.
     """
     name = os.path.splitext(file_name)[0]
-    data_from_xml = parse_band_structure_xml(name + '.xml')
-    data_from_dat = parse_band_structure_dat(name + '.dat')
+    data_from_xml = parse_band_structure_xml(name + ".xml")
+    data_from_dat = parse_band_structure_dat(name + ".dat")
 
     e_fermi = float(np.loadtxt(Path(file_name).parent / "EFERMI.OUT"))
 
-    return BandData(bands=data_from_xml['band_energies'],
-                    k_points=data_from_dat['k_points'],
-                    e_fermi=e_fermi,
-                    flattened_k_points=data_from_xml['k_points_along_band'],
-                    vertices=data_from_xml['vertices'])
+    return BandData(
+        bands=data_from_xml["band_energies"],
+        k_points=data_from_dat["k_points"],
+        e_fermi=e_fermi,
+        flattened_k_points=data_from_xml["k_points_along_band"],
+        vertices=data_from_xml["vertices"],
+    )
```

### Comparing `excitingtools-1.7.0/excitingtools/input/bandstructure.py` & `excitingtools-1.7.1/excitingtools/input/bandstructure.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-""" Generate bandstructure input from atoms. """
+"""Generate bandstructure input from atoms."""
+
 from __future__ import annotations
 
 import re
 from typing import List
 
 import ase.dft
 import numpy as np
@@ -12,60 +13,62 @@
 from excitingtools import ExcitingStructure
 from excitingtools.input.input_classes import ExcitingBandStructureInput
 
 _default_steps = 100
 
 
 def band_structure_input_from_cell_or_bandpath(
-        cell_or_bandpath: Cell | ase.dft.kpoints.BandPath,
-        steps: int = _default_steps) -> ExcitingBandStructureInput:
+    cell_or_bandpath: Cell | ase.dft.kpoints.BandPath, steps: int = _default_steps
+) -> ExcitingBandStructureInput:
     """Get band path from ASE lattice cell or ASE bandpath object.
 
     :param cell_or_bandpath: ase.cell.Cell object or ase.dft.kpoints.BandPath
     :param steps: number of steps for bandstructure calculation
     :return: the exciting band structure input
     """
     bandpath = cell_or_bandpath.bandpath() if isinstance(cell_or_bandpath, Cell) else cell_or_bandpath
     points = []
-    pattern = r'[A-Z,][a-z]*[0-9]*'
+    pattern = r"[A-Z,][a-z]*[0-9]*"
     for point in re.findall(pattern, bandpath.path):
         if point == ",":
             points[-1]["breakafter"] = True
         else:
-            points.append(
-                {"coord": list(bandpath.special_points[point]), "label": point})
+            points.append({"coord": list(bandpath.special_points[point]), "label": point})
 
     return ExcitingBandStructureInput(plot1d={"path": {"steps": steps, "point": points}})
 
 
-def band_structure_input_from_lattice(lattice_vectors: List[List[float]] | np.ndarray,
-                                      steps: int = _default_steps) -> ExcitingBandStructureInput:
-    """ Get band path from lattice vectors as array or list of lists using ASE. Lattice vectors
+def band_structure_input_from_lattice(
+    lattice_vectors: List[List[float]] | np.ndarray, steps: int = _default_steps
+) -> ExcitingBandStructureInput:
+    """Get band path from lattice vectors as array or list of lists using ASE. Lattice vectors
     in array needs to be stored row-wise.
 
     :param lattice_vectors: lattice
     :param steps: number of steps for bandstructure calculation
     :return: the exciting band structure input
     """
     return band_structure_input_from_cell_or_bandpath(Cell(lattice_vectors), steps=steps)
 
 
-def band_structure_input_from_ase_atoms_obj(atoms_obj: Atoms,
-                                            steps: int = _default_steps) -> ExcitingBandStructureInput:
-    """ Get band path from ase object.
+def band_structure_input_from_ase_atoms_obj(
+    atoms_obj: Atoms, steps: int = _default_steps
+) -> ExcitingBandStructureInput:
+    """Get band path from ase object.
 
     :param atoms_obj: ase atoms object
     :param steps: number of steps for bandstructure calculation
     :return: the exciting band structure input
     """
     return band_structure_input_from_cell_or_bandpath(atoms_obj.cell, steps)
 
 
-def get_bandstructure_input_from_exciting_structure(structure: ExcitingStructure,
-                                                    steps: int = _default_steps) -> ExcitingBandStructureInput:
-    """ Use ase bandpath to get bandstructure input for exciting using ASE.
+def get_bandstructure_input_from_exciting_structure(
+    structure: ExcitingStructure, steps: int = _default_steps
+) -> ExcitingBandStructureInput:
+    """Use ase bandpath to get bandstructure input for exciting using ASE.
 
     :param structure: exciting structure input object
     :param steps: number of steps for bandstructure calculation
     :return: bandstructure input for exciting
     """
     return band_structure_input_from_lattice(structure.get_lattice(), steps=steps)
```

### Comparing `excitingtools-1.7.0/excitingtools/input/base_class.py` & `excitingtools-1.7.1/excitingtools/input/base_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Base class for exciting input classes."""
 
 import importlib
 import re
 import warnings
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import Union, List, Type, Iterator
+from typing import Iterator, List, Type, Union
 from xml.etree import ElementTree
 
 import numpy as np
 
 from excitingtools.exciting_dict_parsers.input_parser import parse_element_xml
 from excitingtools.utils import valid_attributes as all_valid_attributes
 from excitingtools.utils.dict_utils import check_valid_keys
@@ -24,49 +24,48 @@
 
     name: Used as tag for the xml subelement
     """
 
     name: str = "ABSTRACT"  # not directly used, need a value here because of the dynamic class list
 
     @abstractmethod
-    def __init__(self, **kwargs):
-        ...
+    def __init__(self, **kwargs): ...
 
     @abstractmethod
     def to_xml(self) -> ElementTree:
-        """ Convert class attributes to XML ElementTree."""
+        """Convert class attributes to XML ElementTree."""
 
     def to_xml_str(self) -> str:
-        """ Convert attributes to XML tree string. """
-        return ElementTree.tostring(self.to_xml(), encoding='unicode', method='xml')
+        """Convert attributes to XML tree string."""
+        return ElementTree.tostring(self.to_xml(), encoding="unicode", method="xml")
 
     def as_dict(self) -> dict:
-        """ Convert attributes to dictionary. """
+        """Convert attributes to dictionary."""
         serialise_attrs = special_serialization_attrs(self)
         return {**serialise_attrs, "xml_string": self.to_xml_str()}
 
     @classmethod
     def from_xml(cls, xml_string: path_type):
-        """ Initialise class instance from XML-formatted string.
+        """Initialise class instance from XML-formatted string.
 
         Example Usage
         --------------
         xs_input = ExcitingXSInput.from_xml(xml_string)
         """
         return cls(**parse_element_xml(xml_string, tag=cls.name))
 
     @classmethod
     def from_dict(cls, d):
-        """ Recreates class instance from dictionary. """
+        """Recreates class instance from dictionary."""
         return cls.from_xml(d["xml_string"])
 
 
 class ExcitingXMLInput(AbstractExcitingInput, ABC):
     """Base class for exciting inputs, with exceptions being title, plan, qpointset and kstlist,
-     because they are not passed as a dictionary. """
+    because they are not passed as a dictionary."""
 
     # Convert python data to string, formatted specifically for exciting
     _attributes_to_input_str = {
         int: lambda x: str(x),
         np.int64: lambda x: str(x),
         np.float64: lambda x: str(x),
         float: lambda x: str(x),
@@ -99,22 +98,23 @@
         subtree_class_map = {cls.name: cls for cls in class_list}
         subtrees = set(kwargs.keys()) - valid_attributes
         single_subtrees = subtrees - multiple_children
         multiple_subtrees = subtrees - single_subtrees
         for subtree in single_subtrees:
             kwargs[subtree] = self._initialise_subelement_attribute(subtree_class_map[subtree], kwargs[subtree])
         for subtree in multiple_subtrees:
-            kwargs[subtree] = [self._initialise_subelement_attribute(subtree_class_map[subtree], x) for
-                               x in kwargs[subtree]]
+            kwargs[subtree] = [
+                self._initialise_subelement_attribute(subtree_class_map[subtree], x) for x in kwargs[subtree]
+            ]
 
         # Set attributes from kwargs
         self.__dict__.update(kwargs)
 
     def __setattr__(self, name: str, value):
-        """ Overload the attribute setting in python with instance.attr = value to check for validity in the schema.
+        """Overload the attribute setting in python with instance.attr = value to check for validity in the schema.
 
         :param name: name of the attribute
         :param value: new value, can be anything
         """
         valid_attributes, valid_subtrees, _, _ = self.get_valid_attributes()
         check_valid_keys({name}, valid_attributes | set(valid_subtrees), self.name)
         super().__setattr__(name, value)
@@ -123,15 +123,15 @@
         mandatory_keys = list(self.get_valid_attributes())[2]
         if name in mandatory_keys:
             warnings.warn(f"Attempt to delete mandatory attribute '{name}' was prevented.")
         else:
             super().__delattr__(name)
 
     def get_valid_attributes(self) -> Iterator:
-        """ Extract the valid attributes, valid subtrees, mandatory attributes and multiple children
+        """Extract the valid attributes, valid subtrees, mandatory attributes and multiple children
         from the parsed schema.
 
         :return: valid attributes, valid subtrees, mandatory attributes and multiple children
         """
         yield set(getattr(all_valid_attributes, f"{self.name}_valid_attributes", set()))
         yield getattr(all_valid_attributes, f"{self.name}_valid_subtrees", [])
         yield set(getattr(all_valid_attributes, f"{self.name}_mandatory_attributes", set()))
@@ -143,51 +143,53 @@
         excitingtools_namespace_content = importlib.import_module("excitingtools").__dict__
         input_class_namespace_content = importlib.import_module("excitingtools.input.input_classes").__dict__
         all_contents = {**excitingtools_namespace_content, **input_class_namespace_content}.values()
         return [cls for cls in all_contents if isinstance(cls, type) and issubclass(cls, AbstractExcitingInput)]
 
     @staticmethod
     def _initialise_subelement_attribute(xml_class, element):
-        """ Initialize given elements to the ExcitingXSInput constructor. If element is already ExcitingXMLInput class
+        """Initialize given elements to the ExcitingXSInput constructor. If element is already ExcitingXMLInput class
         object, nothing happens. Else the class constructor of the given XMLClass is called. For a passed
         dictionary the dictionary is passed as kwargs.
         """
         if isinstance(element, xml_class):
             return element
-        elif isinstance(element, dict):
+        if isinstance(element, dict):
             # assume kwargs
             return xml_class(**element)
-        else:
-            # Assume the element type is valid for the class constructor
-            return xml_class(element)
+        # Assume the element type is valid for the class constructor
+        return xml_class(element)
 
     def to_xml(self) -> ElementTree:
         """Put class attributes into an XML tree, with the element given by self.name.
 
         Example ground state XML subtree:
            <groundstate vkloff="0.5  0.5  0.5" ngridk="2 2 2" mixer="msec" </groundstate>
 
         Note, kwargs preserve the order of the arguments, however the order does not appear to be
         preserved when passed to (or perhaps converted to string) with xml.etree.ElementTree.tostring.
 
         :return ElementTree.Element sub_tree: sub_tree element tree, with class attributes inserted.
         """
-        valid_attributes, valid_subtrees, _, multiple_children = self.get_valid_attributes()
+        valid_attributes, valid_subtrees, _, _ = self.get_valid_attributes()
 
-        attributes = {key: self._attributes_to_input_str[type(value)](value) for key, value
-                      in vars(self).items() if key in valid_attributes}
+        attributes = {
+            key: self._attributes_to_input_str[type(value)](value)
+            for key, value in vars(self).items()
+            if key in valid_attributes
+        }
         xml_tree = ElementTree.Element(self.name, **attributes)
 
         subtrees = {key: self.__dict__[key] for key in set(vars(self).keys()) - set(attributes.keys())}
         ordered_subtrees = flatten_list([subtrees[x] for x in valid_subtrees if x in subtrees])
         for subtree in ordered_subtrees:
             xml_tree.append(subtree.to_xml())
 
         # Seems to want this operation on a separate line
-        xml_tree.text = ' '
+        xml_tree.text = " "
 
         return xml_tree
 
 
 def query_exciting_version(exciting_root: path_type) -> dict:
     """Query the exciting version.
 
@@ -201,22 +203,22 @@
 
     Also checks the src/mod_misc.F90 file for the major exciting version.
 
     :param exciting_root: exciting root directory.
     :return version: Build and version details
     """
     exciting_root = Path(exciting_root)
-    version_inc = exciting_root / 'src/version.inc'
-    assert version_inc.exists(), f'{version_inc} cannot be found. This file generated when the code is built'
+    version_inc = exciting_root / "src/version.inc"
+    assert version_inc.exists(), f"{version_inc} cannot be found. This file generated when the code is built"
 
-    with open(version_inc, 'r') as fid:
+    with open(version_inc) as fid:
         all_lines = fid.readlines()
 
     git_hash_part1 = all_lines[0].split()[-1][1:-1]
     git_hash_part2 = all_lines[1].split()[-1][1:-1]
     compiler_parts = all_lines[2].split()[2:]
     compiler = " ".join(s for s in compiler_parts).strip()
 
     mod_misc = exciting_root / "src/mod_misc.F90"
     major_version = re.search(r"character\(40\) :: versionname = '(NEON)'", mod_misc.read_text())[1]
 
-    return {'compiler': compiler[1:-1], 'git_hash': git_hash_part1 + git_hash_part2, "major": major_version}
+    return {"compiler": compiler[1:-1], "git_hash": git_hash_part1 + git_hash_part2, "major": major_version}
```

### Comparing `excitingtools-1.7.0/excitingtools/input/dynamic_class.py` & `excitingtools-1.7.1/excitingtools/input/dynamic_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,24 @@
  * 'class name' defines the name of the class, when calling in Python.
  *  'bases' define any parent classes for "class name" to inherit from, given in a tuple.
  *  'attributes' defines any attributes (data or methods) to include in "class name".
 
 ALL data should be defined as a string, as it will get rendered as a Python-valid string,
 which subsequently gets interpreted at run-time.
 """
-from typing import Dict, Union, List, Optional, Iterator
+
+from typing import Dict, Iterator, List, Optional, Union
 
 from excitingtools.exciting_dict_parsers.input_parser import special_tags_to_parse_map
 from excitingtools.utils import valid_attributes
 from excitingtools.utils.valid_attributes import input_valid_subtrees
 
 
 def class_constructor_string(class_definitions: Dict[str, Union[dict, str]]) -> str:
-    """ Given a dictionary, return a Python-interpretable string of one or more
+    """Given a dictionary, return a Python-interpretable string of one or more
     class definitions.
 
         Example function argument:
         class_definitions = {'class name':
                                   {'bases': '(ParentClass1, ParentClass2)',
                                    'attributes':
                                             {'attribute1', 'attribute1',
@@ -40,70 +41,75 @@
 
     :param class_definitions: A dict containing the class name, attributes and parent classes,
     all in string form.
     :return: class_definition_str: A Python-interpretable string of class definitions using
     the type() constructor.
     """
     # first import the base class
-    class_definition_str = 'from excitingtools.input.base_class import ExcitingXMLInput \n'
+    class_definition_str = "from excitingtools.input.base_class import ExcitingXMLInput \n"
     for class_name, bases_and_attributes in class_definitions.items():
         # Parent class (or classes)
-        bases = bases_and_attributes['bases']
+        bases = bases_and_attributes["bases"]
 
         # Attributes and methods (including private attributes)
-        attributes = bases_and_attributes['attributes']
+        attributes = bases_and_attributes["attributes"]
 
-        class_definition_str += \
+        class_definition_str += (
             f"Exciting{class_name}Input = type('Exciting{class_name}Input', {bases}, {attributes}) \n"
+        )
 
     return class_definition_str
 
 
 def give_class_dictionary(name: str) -> dict:
-    """ Gives class dictionary with inheritance and further properties.
+    """Gives class dictionary with inheritance and further properties.
 
     :param name: name of class
     :return: dict with definition
     """
-    return {"bases": '(ExcitingXMLInput, )',
-            "attributes": {"__doc__": f"Class for exciting {name} input.",
-                           "__module__": "excitingtools.input.input_classes",
-                           'name': name}}
+    return {
+        "bases": "(ExcitingXMLInput, )",
+        "attributes": {
+            "__doc__": f"Class for exciting {name} input.",
+            "__module__": "excitingtools.input.input_classes",
+            "name": name,
+        },
+    }
 
 
 def class_name_uppercase(name: str) -> str:
-    """ Converts the name in a string which better fits as class name, capitalizing the first letter and
+    """Converts the name in a string which better fits as class name, capitalizing the first letter and
     leaving the rest unchanged.
     Exceptions are groundstate -> GroundState, xs -> XS, gw -> GW, bandstructure -> BandStructure, eph -> EPH
 
     :param name: name of the class/tag in original notation
     :return: name usually capitilized, see exceptions
     """
     exceptions = {"groundstate": "GroundState", "xs": "XS", "gw": "GW", "bandstructure": "BandStructure", "eph": "EPH"}
     if name in exceptions:
         return exceptions[name]
     return name[0].upper() + name[1:]
 
 
 def get_all_valid_subtrees(valid_xml_tags: Optional[List[str]]) -> Optional[Iterator[str]]:
-    """ Get recursively all valid xml (sub-)trees (tags) from exciting.
+    """Get recursively all valid xml (sub-)trees (tags) from exciting.
 
     :param valid_xml_tags: valid xml tags
     :return: list of all valid xml tags of all trees and subtrees
     """
     if not valid_xml_tags:
         return
     for valid_tag in valid_xml_tags:
         yield valid_tag
         tag_valid_subtrees = valid_attributes.__dict__.get(f"{valid_tag}_valid_subtrees")
         yield from get_all_valid_subtrees(tag_valid_subtrees)
 
 
 def generate_classes_str() -> str:
-    """ Generate string to execute by python. For all standard input classes.
+    """Generate string to execute by python. For all standard input classes.
 
     :return: python string
     """
     non_standard_input_classes = set(special_tags_to_parse_map)
     all_valid_subtrees = set(get_all_valid_subtrees(input_valid_subtrees))
     standard_input_classes = all_valid_subtrees - non_standard_input_classes
```

### Comparing `excitingtools-1.7.0/excitingtools/input/input_classes.py` & `excitingtools-1.7.1/excitingtools/input/input_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-""" Automatic generation of all standard input classes plus definiton of exceptions. """
-from typing import List, Union, Any
+"""Automatic generation of all standard input classes plus definiton of exceptions."""
+
+from typing import Any, List, Union
 from xml.etree import ElementTree
 
 import numpy as np
 
 from excitingtools.input.base_class import AbstractExcitingInput
 from excitingtools.input.dynamic_class import generate_classes_str
 from excitingtools.utils.dict_utils import check_valid_keys
@@ -13,117 +14,123 @@
 # define names of classes which are meant to be available for a user or used directly elsewhere in excitingtools
 # type hint as Any to not conflict with static type checkers as the input classes are generated dynamically
 ExcitingCrystalInput: Any
 ExcitingSpeciesInput: Any
 ExcitingAtomInput: Any
 ExcitingGroundStateInput: Any
 ExcitingXSInput: Any
+ExcitingBSEInput: Any
 ExcitingPropertiesInput: Any
 ExcitingPointInput: Any
 ExcitingBandStructureInput: Any
 ExcitingRelaxInput: Any
 ExcitingPhononsInput: Any
 ExcitingGWInput: Any
 ExcitingMDInput: Any
 ExcitingEPHInput: Any
 
 # execute dynamically generated string with all standard class defintions
 exec(generate_classes_str())
 
 
 class ExcitingTitleInput(AbstractExcitingInput):
-    """ Holds only the title but for consistency reasons as class. """
+    """Holds only the title but for consistency reasons as class."""
+
     name = "title"
 
     def __init__(self, title: str):
         self.title = title
 
     def to_xml(self) -> ElementTree:
-        """ Puts title to xml, only the text is title. """
+        """Puts title to xml, only the text is title."""
         title_tree = ElementTree.Element(self.name)
         title_tree.text = self.title
         return title_tree
 
 
 class ExcitingKeywordsInput(AbstractExcitingInput):
-    """ Input class for keywords. Can set any info via a text string, it's not used by exciting. """
+    """Input class for keywords. Can set any info via a text string, it's not used by exciting."""
+
     name = "keywords"
 
     def __init__(self, info: str):
         self.info = info
 
     def to_xml(self) -> ElementTree:
-        """ Puts keywords to xml. """
+        """Puts keywords to xml."""
         keywords_tree = ElementTree.Element(self.name)
         keywords_tree.text = self.info
         return keywords_tree
 
 
 class ExcitingQpointsetInput(AbstractExcitingInput):
     """
     Class for exciting Qpointset Input
     """
+
     name = "qpointset"
 
     def __init__(self, qpointset: Union[np.ndarray, List[List[float]]] = np.array([0.0, 0.0, 0.0])):
         """
         Qpointset should be passed either as numpy array or as a list of lists, so either
         np.array([[0., 0., 0.], [0.0, 0.0, 0.01], ...])
         or
         [[0., 0., 0.], [0.0, 0.0, 0.01], ...]
         """
         self.qpointset = qpointset
 
     def to_xml(self) -> ElementTree.Element:
-        """ Special implementation of to_xml for the qpointset element. """
+        """Special implementation of to_xml for the qpointset element."""
         qpointset = ElementTree.Element(self.name)
         for qpoint in self.qpointset:
-            ElementTree.SubElement(qpointset, 'qpoint').text = list_to_str(qpoint)
+            ElementTree.SubElement(qpointset, "qpoint").text = list_to_str(qpoint)
 
         return qpointset
 
 
 class ExcitingPlanInput(AbstractExcitingInput):
     """
     Class for exciting Plan Input
     """
+
     name = "plan"
 
     def __init__(self, plan: List[str]):
         """
         Plan doonly elements are passed as a List of strings in the order exciting shall execute them:
             ['bse', 'xseigval', ...]
         """
         check_valid_keys(plan, valid_plan_entries, self.name)
         self.plan = plan
 
     def to_xml(self) -> ElementTree.Element:
-        """ Special implementation of to_xml for the plan element. """
+        """Special implementation of to_xml for the plan element."""
         plan = ElementTree.Element(self.name)
         for task in self.plan:
-            ElementTree.SubElement(plan, 'doonly', task=task)
+            ElementTree.SubElement(plan, "doonly", task=task)
 
         return plan
 
 
 class ExcitingKstlistInput(AbstractExcitingInput):
     """
     Class for exciting Kstlist Input
     """
+
     name = "kstlist"
 
     def __init__(self, kstlist: Union[np.ndarray, List[List[int]]]):
         """
         Kstlist should be passed either as numpy array or as a list of lists, so either
         np.array([[1, 2], [3, 4], ...])
         or
         [[1, 2], [3, 4], ...]
         """
         self.kstlist = kstlist
 
     def to_xml(self) -> ElementTree.Element:
-        """ Special implementation of to_xml for the kstlist element. """
+        """Special implementation of to_xml for the kstlist element."""
         kstlist = ElementTree.Element(self.name)
         for pointstatepair in self.kstlist:
-            ElementTree.SubElement(kstlist, 'pointstatepair').text = list_to_str(pointstatepair)
+            ElementTree.SubElement(kstlist, "pointstatepair").text = list_to_str(pointstatepair)
 
         return kstlist
```

### Comparing `excitingtools-1.7.0/excitingtools/input/input_xml.py` & `excitingtools-1.7.1/excitingtools/input/input_xml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-""" Input xml class. """
+"""Input xml class."""
+
 from pathlib import Path
 from typing import Union
 
 from excitingtools.input.base_class import ExcitingXMLInput
 from excitingtools.input.input_classes import ExcitingGroundStateInput, ExcitingTitleInput
 from excitingtools.input.structure import ExcitingStructure
 from excitingtools.input.xml_utils import prettify_tag_attributes, xml_tree_to_pretty_str
 
 
 class ExcitingInputXML(ExcitingXMLInput):
     """
     Container for a complete input xml file.
     """
+
     name = "input"
     _default_filename = "input.xml"
     structure: ExcitingStructure
     groundstate: ExcitingGroundStateInput
     title: ExcitingTitleInput
 
     def set_title(self, title: str):
-        """ Set a new title. """
+        """Set a new title."""
         self.__dict__["title"].title = title
 
     def to_xml_str(self) -> str:
         """Compose XML ElementTrees from exciting input classes to create an input xml string.
 
         :return: Input XML tree as a string, with pretty formatting.
         """
```

### Comparing `excitingtools-1.7.0/excitingtools/input/structure.py` & `excitingtools-1.7.1/excitingtools/input/structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,47 +3,50 @@
 See https://exciting.wikidot.com/ref:structure
 """
 
 from __future__ import annotations
 
 import copy
 from pathlib import Path
-from typing import Optional, Union, List, Dict, Iterator, Tuple
+from typing import Dict, Iterator, List, Optional, Tuple, Union
 from xml.etree import ElementTree
 
 import numpy as np
 from numpy.typing import NDArray
 
 from excitingtools.constants.units import angstrom_to_bohr, bohr_to_angstrom
-from excitingtools.input.base_class import ExcitingXMLInput, AbstractExcitingInput
-from excitingtools.input.input_classes import ExcitingCrystalInput, ExcitingSpeciesInput, ExcitingAtomInput
+from excitingtools.input.base_class import AbstractExcitingInput, ExcitingXMLInput
+from excitingtools.input.input_classes import ExcitingAtomInput, ExcitingCrystalInput, ExcitingSpeciesInput
 from excitingtools.structure.lattice import check_lattice, check_lattice_vector_norms
 from excitingtools.utils import valid_attributes
 from excitingtools.utils.dict_utils import check_valid_keys
 from excitingtools.utils.utils import list_to_str
 
 
 class ExcitingStructure(ExcitingXMLInput):
     """Class allowing exciting XML structure to be written from python data."""
+
     name = "structure"
 
     # Path type
     path_type = Union[str, Path]
 
     # Mandatory attribute "coord" taken out because it's specified inside the atoms
     _valid_atom_attributes = set(valid_attributes.atom_valid_attributes) - {"coord"}
 
-    def __init__(self,
-                 atoms,
-                 lattice: Optional[list | np.ndarray] = None,
-                 species_path: path_type = './',
-                 crystal_properties: Optional[dict | ExcitingCrystalInput] = None,
-                 species_properties: Optional[Dict[str, Union[dict, ExcitingSpeciesInput]]] = None,
-                 **kwargs):
-        """ Initialise instance of ExcitingStructure.
+    def __init__(
+        self,
+        atoms,
+        lattice: Optional[list | np.ndarray] = None,
+        species_path: path_type = "./",
+        crystal_properties: Optional[dict | ExcitingCrystalInput] = None,
+        species_properties: Optional[Dict[str, Union[dict, ExcitingSpeciesInput]]] = None,
+        **kwargs,
+    ):
+        """Initialise instance of ExcitingStructure.
 
         TODO(Alex) Issue 117. Create our own class with a subset of methods common to ASE' Atom()
           Then we can have a single API for this init. If ASE is used, xAtom() is just a wrapper of
           Atom(), else we have some light methods.
 
         All valid attributes can be found in the module valid_attributes.py
 
@@ -76,42 +79,40 @@
             raise ValueError("If atoms is a list, lattice must be passed as a separate argument.")
 
         # Simple container for atoms, as documented in __init__.
         if isinstance(atoms, list):
             check_lattice(lattice)
             check_lattice_vector_norms(lattice)
             self.lattice = np.asarray(lattice, dtype=np.float64)
-            self.species = [atom['species'].capitalize() for atom in atoms]
-            self.positions = [atom['position'] for atom in atoms]
+            self.species = [atom["species"].capitalize() for atom in atoms]
+            self.positions = [atom["position"] for atom in atoms]
             self.atom_properties = list(self._init_atom_properties(atoms))
         else:
             self.lattice, self.species, self.positions = self._init_lattice_species_positions_from_ase_atoms(atoms)
             self.atom_properties = [{}] * len(self.species)
 
         self.unique_species = sorted(set(self.species))
 
         # Optional properties
-        self.crystal_properties = self._initialise_subelement_attribute(
-            ExcitingCrystalInput, crystal_properties or {}
-        )
+        self.crystal_properties = self._initialise_subelement_attribute(ExcitingCrystalInput, crystal_properties or {})
         self.species_properties = dict(self._init_species_properties(species_properties))
 
     def __setattr__(self, name: str, value):
-        """ Overload the attribute setting from the base class, since here we use different attribute names than
+        """Overload the attribute setting from the base class, since here we use different attribute names than
         defined in the schema.
 
         :param name: name of the attribute
         :param value: new value, can be anything
         """
         AbstractExcitingInput.__setattr__(self, name, value)
 
     def _init_lattice_species_positions_from_ase_atoms(
-            self, atoms
+        self, atoms
     ) -> Tuple[NDArray[float], List[str], List[NDArray[float]]]:
-        """ Initialise lattice, species and positions from an ASE Atoms Object.
+        """Initialise lattice, species and positions from an ASE Atoms Object.
 
         Duck typing for atoms, such that ASE is not a hard dependency.
 
         :param atoms: ASE Atoms object.
         :return  Lattice, species, positions: Lattice, species and positions
         """
         try:
@@ -121,20 +122,22 @@
             species = [x.capitalize() for x in atoms.get_chemical_symbols()]
             if self.structure_attributes.get("cartesian"):
                 positions = angstrom_to_bohr * atoms.get_positions()
             else:
                 positions = atoms.get_scaled_positions()
             return lattice, species, list(positions)
         except AttributeError:
-            message = "atoms must either be an ase.atoms.Atoms object or List[dict], of the form" \
-                      "[{'species': 'X', 'position': [x, y, z]}, ...]."
+            message = (
+                "atoms must either be an ase.atoms.Atoms object or List[dict], of the form"
+                "[{'species': 'X', 'position': [x, y, z]}, ...]."
+            )
             raise AttributeError(message)
 
     def _init_atom_properties(self, atoms: List[dict]) -> Iterator[dict]:
-        """ Initialise atom_properties.
+        """Initialise atom_properties.
 
         For atoms that contain optional atomic properties, store them as
         dicts in a list of len(n_atoms). Atoms with none of these properties
         will be defined as empty dicts.
 
         For each element of atoms, one must have  {'species': 'X', 'position': [x, y, z]}  and
         may have the additional attributes: {'bfcmt': [bx, by, bz], 'lockxyz': [lx, ly, lz], 'mommtfix': [mx, my, mz]}.
@@ -146,31 +149,31 @@
         """
         for atom in atoms:
             atom_properties = {key: value for key, value in atom.items() if key not in {"species", "position"}}
             check_valid_keys(atom_properties.keys(), self._valid_atom_attributes, "Atom properties")
             yield atom_properties
 
     def _init_species_properties(self, species_properties: Union[dict, None]) -> Iterator[Tuple[str, ExcitingXMLInput]]:
-        """ Initialise species_properties.
+        """Initialise species_properties.
 
         For species without properties, return empty_properties: {'S': {}, 'Al': {}}.
 
         :param species_properties: Species properties
         :return Dict of ExitingXMLInput-species_properties.
         """
         if species_properties is None:
             species_properties = {}
 
         for species in self.unique_species:
             props = species_properties.get(species) or {}
-            props["speciesfile"] = species + '.xml'
+            props["speciesfile"] = species + ".xml"
             yield species, ExcitingSpeciesInput(**props)
 
     def get_lattice(self, convert_to_angstrom: bool = False) -> np.ndarray:
-        """ Get the full lattice, meaning after the application of scale and stretch values to the stored
+        """Get the full lattice, meaning after the application of scale and stretch values to the stored
         lattice vectors.
 
         :param convert_to_angstrom: if True returns lattice in angstrom, else in bohr
         :return: full lattice vectors, stored row-wise in a matrix
         """
         lattice = copy.deepcopy(self.lattice)
         unit_conversion = bohr_to_angstrom if convert_to_angstrom else 1
@@ -178,19 +181,19 @@
         lattice *= scale * unit_conversion
 
         stretch = np.array(getattr(self.crystal_properties, "stretch", [1, 1, 1]))
         lattice *= stretch[:, None]
         return lattice
 
     def add_atom(
-            self,
-            species: str,
-            position: Union[List[float], NDArray[float]],
-            properties: Union[dict, None] = None,
-            species_properties: Union[dict | None] = None
+        self,
+        species: str,
+        position: Union[List[float], NDArray[float]],
+        properties: Union[dict, None] = None,
+        species_properties: Union[dict | None] = None,
     ):
         """Add a new atom to the structure.
 
         :param species: of the new atom
         :param position: of the new atom
         :param properties: optional atom properties
         :param species_properties: if it is a new species, optional species properties, else not used
@@ -233,15 +236,15 @@
         """
         indices = {}
         for x in self.unique_species:
             indices[x] = [i for i, element in enumerate(self.species) if element == x]
         return indices
 
     def _xml_atomic_subtree(self, species: str, species_tree: ElementTree.Element, atomic_indices: dict):
-        """ Add the required atomic positions and any optional attributes, per species.
+        """Add the required atomic positions and any optional attributes, per species.
 
         :param species: Species
         :param species_tree: Empty SubElement for species x, which gets filled
         """
         for index in atomic_indices[species]:
             species_tree.append(ExcitingAtomInput(coord=self.positions[index], **self.atom_properties[index]).to_xml())
 
@@ -266,15 +269,15 @@
 
         :return ET structure: Element tree containing structure attributes.
         """
         structure_attributes = {
             key: self._attributes_to_input_str[type(value)](value) for key, value in self.structure_attributes.items()
         }
         structure = ElementTree.Element(self.name, **structure_attributes)
-        structure.text = ' '
+        structure.text = " "
 
         # Lattice vectors
         crystal = self.crystal_properties.to_xml()
         structure.append(crystal)
         for vector in self.lattice:
             ElementTree.SubElement(crystal, "basevect").text = list_to_str(vector)
```

### Comparing `excitingtools-1.7.0/excitingtools/input/xml_utils.py` & `excitingtools-1.7.1/excitingtools/input/xml_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""Utilities to aid in writing and formatting XML
-"""
+"""Utilities to aid in writing and formatting XML"""
+
 import re
 from xml.dom import minidom
 from xml.etree import ElementTree
 
 
 def xml_tree_to_pretty_str(elem: ElementTree.Element) -> str:
     """Convert an XML element to a pretty string.
 
     :param ElementTree.Element elem: Element/ element tree
     :return str : XML tree string, with pretty formatting.
     """
-    rough_string = ElementTree.tostring(elem, 'utf-8')
+    rough_string = ElementTree.tostring(elem, "utf-8")
     reparsed = minidom.parseString(rough_string)
     return reparsed.toprettyxml(indent="\t")
 
 
 def line_reformatter(input_str: str) -> str:
     """Identify attributes of an XML string element, and reformat them such that they are on new lines.
 
@@ -48,44 +48,42 @@
     :param str input_str: Input string, opened and closed with an XML element.
     :return str reformatted_str: Reformatted form of input_str
     """
     full_tag = input_str.split(" ")[0]
     tag = full_tag.strip()
     number_of_tag_indents = len(full_tag) - len(tag)
 
-    tag_indent = '\t' * number_of_tag_indents
-    attr_indent = tag_indent + ' ' * 3
+    tag_indent = "\t" * number_of_tag_indents
+    attr_indent = tag_indent + " " * 3
 
     # Get rid of format characters, like \n, \t etc
     input_str = input_str.strip()
 
     # Isolate attributes according to position of quotation marks in string
     # (cannot use whitespaces to split)
-    quote_indices = [x.start() for x in re.finditer('\"', input_str)]
+    quote_indices = [x.start() for x in re.finditer('"', input_str)]
     closing_quote_indices = quote_indices[1::2]
-    attribute_start_indices = [len(tag) + 1] + [i + 1 for i in
-                                                closing_quote_indices[:-1]]
+    attribute_start_indices = [len(tag) + 1] + [i + 1 for i in closing_quote_indices[:-1]]
 
-    reformatted_str = tag_indent + tag + '\n'
+    reformatted_str = tag_indent + tag + "\n"
 
-    for i in range(0, len(attribute_start_indices)):
-        i1 = attribute_start_indices[i]
+    for i, start_index in enumerate(attribute_start_indices):
         i2 = closing_quote_indices[i]
-        attribute_str = input_str[i1:i2 + 1].strip()
-        reformatted_str += attr_indent + attribute_str + '\n'
+        attribute_str = input_str[start_index : i2 + 1].strip()
+        reformatted_str += attr_indent + attribute_str + "\n"
 
     # short ending option:
-    if input_str[-2:] == '/>':
-        return reformatted_str[:-1] + '/>'
-    reformatted_str = reformatted_str[:-1] + '>'
+    if input_str[-2:] == "/>":
+        return reformatted_str[:-1] + "/>"
+    reformatted_str = reformatted_str[:-1] + ">"
     # no ending option:
-    if not input_str[-(len(tag) + 2):-len(tag)] == '</':
+    if input_str[-(len(tag) + 2) : -len(tag)] != "</":
         return reformatted_str
     # long ending option:
-    reformatted_str += "\n" + tag_indent + input_str[-(len(tag) + 2):] + ''
+    reformatted_str += "\n" + tag_indent + input_str[-(len(tag) + 2) :] + ""
     return reformatted_str
 
 
 def prettify_tag_attributes(xml_string: str) -> str:
     """Prettify XML string formatting of attributes.
 
     The routine finds the lines containing an XML element, applies
@@ -108,16 +106,16 @@
         </groundstate>
     ```
 
     :param str xml_string: Already-prettified XML string (assumes tags are on their own lines)
     :return str reformatted_xml_string: xml_string, with the tag substrings reformatted according to the example
      - Line break per attribute.
     """
-    xml_list = xml_string.split('\n')
+    xml_list = xml_string.split("\n")
     min_number_attributes_for_split = 3
 
     for i, line in enumerate(xml_list):
         if line.count("=") >= min_number_attributes_for_split:
             xml_list[i] = line_reformatter(line)
 
     xml_list_without_blank_lines = filter(lambda x: x.strip(), xml_list)
-    return "".join(x + '\n' for x in xml_list_without_blank_lines)
+    return "".join(x + "\n" for x in xml_list_without_blank_lines)
```

### Comparing `excitingtools-1.7.0/excitingtools/parser_utils/grep_parser.py` & `excitingtools-1.7.1/excitingtools/parser_utils/grep_parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-"""Wrapper for command-line grep.
-"""
+"""Wrapper for command-line grep."""
+
 import subprocess
+import warnings
 from typing import Optional, Union
 
 
 def grep(string: str, fname: str, options: Optional[dict] = None) -> Union[str, None]:
     """
     Wrapper for command-line grep.
 
     Can pass any grep options like: options = {'A': value}
 
     :param str string: Search string
     :param str fname: File name to search
     :param Optional[dict] options: Grep options.
     :return output: String if matched, None if failed.
     """
-    opts = ''
+    opts = ""
     if options is not None:
         for key, value in options.items():
-            opts += '-' + key + ' ' + str(value) + ' '
+            opts += "-" + key + " " + str(value) + " "
 
     grep_str = "grep " + opts + " '" + string + "' " + fname
 
     try:
         output = subprocess.check_output(grep_str, shell=True).decode("utf-8")
     except subprocess.CalledProcessError as grepexc:
-        print("subprocess error:", grepexc.returncode, "grep found:",
-              grepexc.output)
+        warnings.warn(f"subprocess error: {grepexc.returncode}, grep found: {grepexc.output}")
         output = None
 
     return output
```

### Comparing `excitingtools-1.7.0/excitingtools/parser_utils/parser_decorators.py` & `excitingtools-1.7.1/excitingtools/parser_utils/parser_decorators.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-"""Decorators and wrappers for parser functions.
-"""
+"""Decorators and wrappers for parser functions."""
+
 import pathlib
 import xml.etree.ElementTree as ET
-from typing import Callable, Union
+from typing import Callable, Optional, Union
 
 from excitingtools.utils.dict_utils import __container_converter
 
 
 def return_file_string(file_name: Union[str, pathlib.Path]) -> str:
-    """ Given a file name, return the file contents as a string.
+    """Given a file name, return the file contents as a string.
 
     :param file_name: File name.
     :return file_string: File contents string.
     """
     file_name_ = file_name
 
     if isinstance(file_name_, str):
         file_name_ = pathlib.Path(file_name_)
 
     if not file_name_.exists():
-        raise FileNotFoundError(f'{file_name_} not found')
+        raise FileNotFoundError(f"{file_name_} not found")
 
     return file_name_.read_text()
 
 
 def file_handler(file_name: Union[str, pathlib.Path], parser_func: Callable[[str], dict]) -> dict:
     """Provide a wrapper for file IO.
 
@@ -33,47 +33,50 @@
     :return: dict data: Dictionary of parsed data, with values converted from strings.
     """
     file_string = return_file_string(file_name)
     return parser_func(file_string)
 
 
 def accept_file_name(parser: Callable):
-    """ Decorate parsers that accept string contents, such that they take file names instead.
-    """
+    """Decorate parsers that accept string contents, such that they take file names instead."""
+
     def modified_func(file_name: Union[str, pathlib.Path]):
-        """ Wrapper.
+        """Wrapper.
         param: file_name: File name.
         """
         file_string = return_file_string(file_name)
         return parser(file_string)
+
     return modified_func
 
 
 def set_return_values(parser: Callable[[str], dict]) -> Callable[[str], dict]:
-    """ Mutate the values of a parsed dictionary to return
+    """Mutate the values of a parsed dictionary to return
     appropriate types, rather than strings.
     """
+
     def modified_exciting_parser(full_file_name: str) -> dict:
-        """ Wrapper.
+        """Wrapper.
         :param full_file_name: File name.
         :return: converted data
         """
         data = parser(full_file_name)
         return __container_converter(data)
+
     return modified_exciting_parser
 
 
 def xml_root(func: Callable):
-    """ Decorate XML parsers, enabling the developer to pass
+    """Decorate XML parsers, enabling the developer to pass
     an XML file name, XML string or ElementTree.Element as input
     and return the XML root.
     """
-    function_selection = {type(None): lambda x, y: func(x), str: lambda x, y: func(x, y)}
+    function_selection = {type(None): lambda x, _: func(x), str: lambda x, y: func(x, y)}
 
-    def modified_func(input: str, tag: str = None):
+    def modified_func(input: str, tag: Optional[str] = None):
         # Element
         if isinstance(input, ET.Element):
             return function_selection[type(tag)](input, tag)
 
         # File name
         try:
             tree = ET.parse(input)
@@ -83,11 +86,10 @@
             pass
 
         # XML string
         try:
             root = ET.fromstring(input)
             return function_selection[type(tag)](root, tag)
         except (ET.ParseError, TypeError):
-            raise ValueError(f'Input string neither an XML file, '
-                             f'nor valid XML: {input}')
+            raise ValueError(f"Input string neither an XML file, nor valid XML: {input}")
 
     return modified_func
```

### Comparing `excitingtools-1.7.0/excitingtools/parser_utils/parser_utils.py` & `excitingtools-1.7.1/excitingtools/parser_utils/parser_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,58 +1,55 @@
-"""General parser utility functions.
-"""
+"""General parser utility functions."""
+
 import re
-from typing import Dict, Any
-from xml.etree import ElementTree
 from json import JSONDecodeError, loads
+from typing import Any, Dict
+from xml.etree import ElementTree
 
 
 def find_element(root: ElementTree.Element, tag: str) -> ElementTree.Element:
-    """ Finds a given tag in an Element, either return the full ElementTree
+    """Finds a given tag in an Element, either return the full ElementTree
     if the tag is correct or find the tag in that ElementTree.
     :param root: Element to find the tag in
     :param tag: tag to search for
     :return: the (sub)element with the correct tag
     """
     if root.tag == tag:
         return root
     return root.find(tag)
 
 
 def convert_string_dict(inputs: dict) -> Dict[str, Any]:
-    """ Parses and converts a dictionary with string values to their actual data types.
+    """Parses and converts a dictionary with string values to their actual data types.
 
     :param inputs: input dictionary
     :return: the converted dictionary
     """
     for key, value in inputs.items():
         inputs[key] = convert_single_entry(value)
     return inputs
 
 
 def convert_single_entry(input_str: str):
-    """ Converts a single string. Accepts also lists separated by whitespaces.
+    """Converts a single string. Accepts also lists separated by whitespaces.
 
     :param input_str: input string
     :return: the converted data
     """
-    split_string = input_str.split()
-    result = []
-    for i in split_string:
-        result.append(json_convert(standardise_fortran_exponent(i)))
+    result = [json_convert(standardise_fortran_exponent(i)) for i in input_str.split()]
 
     if len(result) == 1:
         return result[0]
-    if len(list((filter(lambda x: isinstance(x, str), result)))) == len(result):
+    if len(list(filter(lambda x: isinstance(x, str), result))) == len(result):
         return " ".join(result)
     return result
 
 
 def json_convert(input_str: str):
-    """ Tries to convert a single string with no whitespaces to its actual data type
+    """Tries to convert a single string with no whitespaces to its actual data type
     using the json decoder (detects int, float and bool). Else returns the string as string.
     :param input_str: input string
     :return: the converted value
     """
     try:
         return loads(input_str)
     except JSONDecodeError:
@@ -63,25 +60,25 @@
     try:
         return float(input_str)
     except ValueError:
         return input_str
 
 
 def standardise_fortran_exponent(input_str: str, return_as_str: bool = True):
-    """ Tries to convert a single string representing a float value in scientific notation
+    """Tries to convert a single string representing a float value in scientific notation
     to the actual number.
     d(D) and q(Q) correspond to higher floating point precision than e(E). Replace
     them since they cannot be parsed by JSON
 
     :param input_str: input string
     :param return_as_str: return the number as a string in python format with e as exponential
     :return: If string can be converted to a float return it, else
     return the input string.
     """
-    subbed_str = re.sub('[dDqQ]', 'E', input_str, count=1)
+    subbed_str = re.sub("[dDqQ]", "E", input_str, count=1)
     if subbed_str == input_str:
         return input_str
 
     try:
         number = float(subbed_str)
     except ValueError:
         return input_str
```

### Comparing `excitingtools-1.7.0/excitingtools/parser_utils/regex_parser.py` & `excitingtools-1.7.1/excitingtools/parser_utils/regex_parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-"""Wrappers for parsing with regex
-"""
+"""Wrappers for parsing with regex"""
+
 import re
 from typing import List, Union
 
 from excitingtools.utils.utils import convert_to_literal
 
 
-def parse_value_regex(file_string: str,
-                      key: str,
-                      no_colon=True,
-                      silent_key_error=False) -> dict:
+def parse_value_regex(file_string: str, key: str, no_colon=True, silent_key_error=False) -> dict:
     """
     Match the first instance of a string (key) if present in file_string,
     and return the result in a dictionary.
 
     :param str file_string: Input string
     :param str key: String to match, also used as a key in the returned dictionary
     :param optional bool no_colon: Remove trailing colons from parsed data keys
@@ -23,46 +20,43 @@
     """
     data = {}
 
     def process_value(x: str) -> Union[int, float, str]:
         numerical_value = convert_to_literal(x)
         if numerical_value is None:
             return x.strip()
-        else:
-            return numerical_value
+        return numerical_value
 
     try:
-        match = re.search(key + '(.+)\n', file_string)
+        match = re.search(key + "(.+)\n", file_string)
         values = match.group(1).split()
         # Remove escape characters
-        parser_key = key.replace('\\', "")
+        parser_key = key.replace("\\", "")
         processed_values = [process_value(raw_value) for raw_value in values]
-        data[parser_key] = processed_values[0] if len(
-            processed_values) == 1 else processed_values
+        data[parser_key] = processed_values[0] if len(processed_values) == 1 else processed_values
 
     except AttributeError:
         if not silent_key_error:
-            print("parse_value_regex. Did not find the key:", key)
+            print("parse_value_regex. Did not find the key:", key)  # noqa: T201
         return {}
 
     if no_colon:
-        return {key.rstrip(':'): value for key, value in data.items()}
-    else:
-        return data
+        return {key.rstrip(":"): value for key, value in data.items()}
+    return data
 
 
 def parse_values_regex(file_string: str, keys: List[str]) -> dict:
     """
     For a list of strings, match the first instance of each string
     (contained in keys) if present in file_string, and return the
     result in a dictionary.
 
     :param str file_string: Input string
     :param List[str] keys: Keys to match in lines of file_string
 
     :return dict parsed_data: Matched data
     """
-    assert type(keys) == list, "2nd argument of parse_values_regex must be List[str]"
+    assert isinstance(keys, list), "2nd argument of parse_values_regex must be List[str]"
     matches_dict = {}
     for key in keys:
         matches_dict.update(**parse_value_regex(file_string, key))
     return matches_dict
```

### Comparing `excitingtools-1.7.0/excitingtools/parser_utils/simple_parser.py` & `excitingtools-1.7.1/excitingtools/parser_utils/simple_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-""" Simple text parsers.
-"""
+"""Simple text parsers."""
+
 from typing import Union
 
 
 def match_current_return_line_n(file_string: str, match: str, n_line=1) -> Union[str, None]:
     """
     Match a string on the ith line and return a substring from the i+n_line line.
 
     :param str file_string: Input string
     :param str match: String to match
     :param int n_line: The index of the line to return, following the matched line
 
     :return Union[str, None] matched line string, or None
     """
-    file = file_string.split('\n')
+    file = file_string.split("\n")
     for i, line in enumerate(file):
         if match in line:
             return file[i + n_line]
     return None
 
 
-def match_current_extract_from_line_n(input_string: str,
-                                      keys_extractions: dict,
-                                      n_line=1) -> dict:
+def match_current_extract_from_line_n(input_string: str, keys_extractions: dict, n_line=1) -> dict:
     """
     Given an input_string, match a substring (defined by the key of keys_extractions),
     return the a substring from the i+n_line line below the match, and extract a value
     from that line using the value of the key, defined by keys_extractions[key]
 
     :param str file_string: Input string
     :param dict keys_extractions: keys = strings to match
```

### Comparing `excitingtools-1.7.0/excitingtools/runner/runner.py` & `excitingtools-1.7.1/excitingtools/runner/runner.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-""" Binary runner and results classes.
-"""
+"""Binary runner and results classes."""
+
 from __future__ import annotations
 
 import copy
 import enum
 import os
 import shutil
 import subprocess
@@ -12,49 +12,51 @@
 from pathlib import Path
 from typing import List, Optional, Union
 
 from excitingtools.utils.jobflow_utils import special_serialization_attrs
 
 
 class RunnerCode(enum.Enum):
-    """ Runner codes.
-     By default, the initial value starts at 1.
+    """Runner codes.
+    By default, the initial value starts at 1.
     """
+
     time_out = enum.auto()
 
 
 @dataclass
 class SubprocessRunResults:
-    """ Results returned from subprocess.run()
-    """
+    """Results returned from subprocess.run()"""
 
     stdout: str
     stderr: str
     return_code: int | RunnerCode
     process_time: Optional[float] = None
 
     @property
     def success(self) -> bool:
         """Determine the run success by evaluating the return code."""
         return self.return_code == 0
 
 
 class BinaryRunner:
-    """ Class to execute a subprocess.
-    """
+    """Class to execute a subprocess."""
+
     path_type = Union[str, Path]
 
-    def __init__(self,
-                 binary: path_type,
-                 run_cmd: List[str] | str = "",
-                 omp_num_threads: int = 1,
-                 time_out: int = 60,
-                 directory: path_type = './',
-                 args: Optional[List[str]] = None):
-        """ Initialise class.
+    def __init__(
+        self,
+        binary: path_type,
+        run_cmd: List[str] | str = "",
+        omp_num_threads: int = 1,
+        time_out: int = 60,
+        directory: path_type = "./",
+        args: Optional[List[str]] = None,
+    ):
+        """Initialise class.
 
         :param str binary: Binary name prepended by full path, or just binary name (if present in $PATH).
          No check for existence here as it could live on a remote worker (see run() doc)
         :param Union[List[str], str] run_cmd: Run commands sequentially as a list. For example:
           * For serial: []
           * For MPI:   ['mpirun', '-np', '2']
         or as a string. For example"
@@ -70,17 +72,15 @@
         self.omp_num_threads = omp_num_threads
         self.time_out = time_out
         self.args = args or []
 
         if isinstance(run_cmd, str):
             self.run_cmd = run_cmd.split()
         elif not isinstance(run_cmd, list):
-            raise ValueError(
-                "Run commands expected in a str or list. For example ['mpirun', '-np', '2']"
-            )
+            raise ValueError("Run commands expected in a str or list. For example ['mpirun', '-np', '2']")
 
         self._check_mpi_processes()
 
         if omp_num_threads <= 0:
             raise ValueError("Number of OMP threads must be > 0")
 
         if time_out <= 0:
@@ -100,19 +100,18 @@
         # call function on class to get only the keys (values not needed)
         serialise_keys = special_serialization_attrs(cls)
         for key in serialise_keys:
             my_dict.pop(key, None)
         return cls(**my_dict)
 
     def _check_mpi_processes(self):
-        """ Check whether mpi is specified and if yes that the number of MPI processes specified is valid.
-        """
+        """Check whether mpi is specified and if yes that the number of MPI processes specified is valid."""
         # Search if MPI is specified:
         try:
-            i = self.run_cmd.index('-np')
+            i = self.run_cmd.index("-np")
         except ValueError:
             # .index will return ValueError if 'np' not found. This corresponds to serial and omp calculations.
             return
         try:
             mpi_processes = int(self.run_cmd[i + 1])
         except IndexError:
             raise ValueError("Number of MPI processes must be specified after the '-np'")
@@ -132,17 +131,15 @@
 
         :return: the run results with output and error message, runner code and run time
         """
         binary = Path(self.binary)
         if not binary.is_file():
             binary = shutil.which(self.binary)
             if not binary:
-                raise FileNotFoundError(
-                    f"{self.binary} binary is not present in the current directory nor in $PATH"
-                )
+                raise FileNotFoundError(f"{self.binary} binary is not present in the current directory nor in $PATH")
 
         if not Path(self.directory).is_dir():
             raise OSError(f"Run directory does not exist: {self.directory}")
 
         execution_list = self.run_cmd + [Path(binary).as_posix()] + self.args
         my_env = {**os.environ, "OMP_NUM_THREADS": str(self.omp_num_threads)}
 
@@ -151,18 +148,18 @@
             result = subprocess.run(
                 execution_list,
                 cwd=self.directory,
                 env=my_env,
                 capture_output=True,
                 encoding="utf-8",
                 timeout=self.time_out,
+                check=False,
             )
             total_time = time.time() - time_start
-            return SubprocessRunResults(result.stdout, result.stderr,
-                                        result.returncode, total_time)
+            return SubprocessRunResults(result.stdout, result.stderr, result.returncode, total_time)
 
         except subprocess.TimeoutExpired as timed_out:
             output = timed_out.output.decode("utf-8") if timed_out.output else ""
-            error = 'BinaryRunner: Job timed out. \n\n'
+            error = "BinaryRunner: Job timed out. \n\n"
             if timed_out.stderr:
                 error += timed_out.stderr.decode("utf-8")
             return SubprocessRunResults(output, error, RunnerCode.time_out, self.time_out)
```

### Comparing `excitingtools-1.7.0/excitingtools/species/species_file.py` & `excitingtools-1.7.1/excitingtools/species/species_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 """SpeciesFile class.
-Provides functionality to read in a species file, add high energy local orbitals (HELOs), and 
+Provides functionality to read in a species file, add high energy local orbitals (HELOs), and
 write the updated XML structures back to file.
 """
+
 import copy
 import warnings
+from collections import defaultdict
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Dict, Union, Tuple, Set, Callable
+from typing import Callable, Dict, Set, Tuple, Union
 from xml.etree import ElementTree
-from collections import defaultdict 
 
 from excitingtools.exciting_dict_parsers.species_parser import parse_species_xml
 from excitingtools.input.xml_utils import xml_tree_to_pretty_str
 from excitingtools.utils.jobflow_utils import special_serialization_attrs
 
 
 @dataclass
 class SpeciesFile:
-    """ Holds a species file. """
+    """Holds a species file."""
+
     species: dict
     muffin_tin: dict
     atomic_states: list
-    basis: dict 
+    basis: dict
 
     def __post_init__(self):
-        """Ensures that the 'basis' dictionary includes 'custom' and 'lo' keys. 
-        If these keys are absent, they are initialized as empty lists. 
+        """Ensures that the 'basis' dictionary includes 'custom' and 'lo' keys.
+        If these keys are absent, they are initialized as empty lists.
         """
-        self.basis.setdefault('custom', [])
-        self.basis.setdefault('lo', [])
+        self.basis.setdefault("custom", [])
+        self.basis.setdefault("lo", [])
 
     @classmethod
     def from_file(cls, file: Union[str, Path]):
-        """ Reads in an exciting species XML file, parses the file as a dict and
+        """Reads in an exciting species XML file, parses the file as a dict and
         initializes an instance of the class with the parsed data.
-        
+
         :param file: XML species file.
         :return: An instance of the class initialized with the data from the species file.
         """
         return cls(**parse_species_xml(file))
-    
+
     def as_dict(self) -> dict:
         """Returns a dictionary representing the current object for later recreation.
         The serialise attributes are required for recognition by monty and jobflow.
         """
         serialise_attrs = special_serialization_attrs(self)
         return {**serialise_attrs, **self.__dict__}
 
@@ -55,62 +57,62 @@
         serialise_keys = special_serialization_attrs(cls)
         for key in serialise_keys:
             my_dict.pop(key, None)
         return cls(**my_dict)
 
     def get_first_helo_n(self, l: int) -> int:
         """Returns the first principle quantum number 'n' for which additional High Energy Local
-        Orbitals (HELOs) can be added, for a given angular momentum quantum number 'l'. 
+        Orbitals (HELOs) can be added, for a given angular momentum quantum number 'l'.
         The 'n' value determination is based on:
 
         1. For a specific 'l' channel the highest 'n' specified in the atomic states is 'max_n'.
-        2. If there exist local orbitals with a 'n' greater than the maximum found in atomic states for 
+        2. If there exist local orbitals with a 'n' greater than the maximum found in atomic states for
            the same 'l', 'max_n' is set to this 'n'.
         3. The first added HELO then starts at 'max_n + 1'.
-        4. For an 'l' channel not represented in atomic states or as a local orbital, the first added HELO 
+        4. For an 'l' channel not represented in atomic states or as a local orbital, the first added HELO
             has principle quantum number 'n = l + 1' .
 
-        :param l: angular momentum quantum number 'l' 
-        :return: first possible principle quantum number 'n' for a HELO for the given 'l'-channel 
+        :param l: angular momentum quantum number 'l'
+        :return: first possible principle quantum number 'n' for a HELO for the given 'l'-channel
         """
         atomicstate_ns_per_l, lo_ns_per_l = self.get_atomicstates_ns_per_l(), self.get_lo_ns_per_l()
         max_n_for_specified_l = max(atomicstate_ns_per_l.get(l, {l}) | lo_ns_per_l.get(l, {l}))
 
         # If matchingOrder > 1 for the same l and highest n, skip n+1 HELO.
         ns_per_l_with_mO_over_1 = self.check_matching_orders()
         if ns_per_l_with_mO_over_1.get(l) and max_n_for_specified_l in ns_per_l_with_mO_over_1[l]:
             warnings.warn(f"HELO skipped for l: {l} and n: {max_n_for_specified_l + 1}")
             return max_n_for_specified_l + 2
 
         return max_n_for_specified_l + 1
-    
+
     def get_atomicstates_ns_per_l(self, cond: Callable[[dict], bool] = lambda _: True) -> Dict[int, set]:
-        """Generates a dictionary mapping each 'l' channel present in the atomic states their corresponding 'n' values. 
+        """Generates a dictionary mapping each 'l' channel present in the atomic states their corresponding 'n' values.
 
         :param cond: condition for choosing specific atomic states
         :return: Dictionary with 'l' channels as keys and sets of 'n' values from the atomic states.
         """
         atomicstate_ns_per_l = defaultdict(set)
         cond_atomic_states = filter(cond, self.atomic_states)
         for state in cond_atomic_states:
             atomicstate_ns_per_l[state["l"]].add(state["n"])
 
         return atomicstate_ns_per_l
-    
+
     def get_valence_and_semicore_atomicstate_ns_per_l(self) -> Dict[int, Dict[str, Set[int]]]:
         """
-        Classifies and returns all non-core states into valence and semicore states for each 'l' channel and 
+        Classifies and returns all non-core states into valence and semicore states for each 'l' channel and
         corresponding 'n' value.
 
         This function classifies all states that do not belong to the core based on the maximum 'n' value for each 'l':
             - States with the maximum 'n' value for their 'l' channel are classified as valence states.
             - All other non-core states are classified as semicore states.
 
-        :return: A dictionary mapping each 'l' channel to another dictionary containing two keys: 'semicore' and 
-                'valence'. Each of these keys maps to a set of 'n' values corresponding to the classified atomic states. 
+        :return: A dictionary mapping each 'l' channel to another dictionary containing two keys: 'semicore' and
+                'valence'. Each of these keys maps to a set of 'n' values corresponding to the classified atomic states.
 
         Example:
             {
                 0: {'semicore': {1, 2}, 'valence': {3}},
                 1: {'semicore': {2}, 'valence': {3, 4}},
                 ...
             }
@@ -122,115 +124,115 @@
             max_n = max(ns)
             ns.remove(max_n)
             valence_and_semicore_states[l] = {"semicore": ns, "valence": {max_n}}
 
         return valence_and_semicore_states
 
     def get_lo_ns_per_l(self) -> Dict[int, set]:
-        """Generates a dictionary mapping each 'l' channel present in the local orbitals to their corresponding 'n' 
-        values. Only includes local orbitals with a defined 'n' value. Local orbitals only defined through the 
+        """Generates a dictionary mapping each 'l' channel present in the local orbitals to their corresponding 'n'
+        values. Only includes local orbitals with a defined 'n' value. Local orbitals only defined through the
         attribute 'trialEnergy' are ignored.
 
         :return: Dictionary with 'l' channels as keys and corresponding sets of 'n' values from local orbitals.
         """
         lo_ns_per_l = defaultdict(set)
         for lo in self.basis["lo"]:
             for wf in lo["wf"]:
                 if "n" in wf:
                     lo_ns_per_l[lo["l"]].add(wf["n"])
 
         return lo_ns_per_l
-    
+
     def get_helos_from_species(self) -> Dict[int, set]:
         """Generates a dictionary mapping each 'l' channel to a list of principle quantum numbers 'n' unique to high
         energy/local orbitals (HELOs). This is achieved by comparing 'n' values in local orbitals against those
         in atomic states for each 'l' channel, extracting those exclusive to HELOs.
 
         :return: Dictionary with 'l' channels as keys and exclusive HELO 'n' values as sets.
         """
         atomicstate_ns_per_l, lo_ns_per_l = self.get_atomicstates_ns_per_l(), self.get_lo_ns_per_l()
-        
+
         helo_ns_per_l = {}
         for l, ns in lo_ns_per_l.items():
             unique_helos = ns - atomicstate_ns_per_l.get(l, set())
             helo_ns_per_l[l] = unique_helos
 
         return helo_ns_per_l
 
     def check_matching_orders(self) -> Dict[int, list]:
-        """Creates a dictionary that lists principle quantum numbers 'n' for each angular momentum quantum number 'l', 
+        """Creates a dictionary that lists principle quantum numbers 'n' for each angular momentum quantum number 'l',
         where the 'n' values are associated with a matchingOrder greater than 1 in the local orbitals.
 
         :return: Dictionary with 'l' channels as keys and lists of 'n' values that have matchingOrder > 1 as values.
         """
         ns_per_l_with_mO_over_1 = defaultdict(list)
         for lo in self.basis["lo"]:
             for wf in lo["wf"]:
                 if wf.get("n") and wf["matchingOrder"] > 1:
                     ns_per_l_with_mO_over_1[lo["l"]].append(wf["n"])
 
         return ns_per_l_with_mO_over_1
 
     def add_number_los_for_all_valence_semicore_states(self, number_lo: int):
-        """Adds a certain number `number_lo` of local orbitals with increasing matching order for every valence and 
-        semicore state to the basis `self.basis[lo]`. Here the local orbital always consists of 2 wave function 
+        """Adds a certain number `number_lo` of local orbitals with increasing matching order for every valence and
+        semicore state to the basis `self.basis[lo]`. Here the local orbital always consists of 2 wave function
         elements.
 
-        :param number_lo: number of local orbitals added for every valence and semicore state 
-        """ 
+        :param number_lo: number of local orbitals added for every valence and semicore state
+        """
         valence_semicore_states = self.get_atomicstates_ns_per_l(lambda x: not x["core"])
 
         for l, ns in valence_semicore_states.items():
             for n in ns:
                 for _ in range(number_lo):
                     self.add_lo_higher_matching_order(l, n)
 
     def add_basic_lo_all_semicore_states(self):
         """Adds one local orbital for every semicore state present in the atomic states.
 
-        Moving a state from core to valence requires the addition of at least one local orbital to accurately 
+        Moving a state from core to valence requires the addition of at least one local orbital to accurately
         describe the semicore state.
         The local orbital consists of two radial functions at matchingOrder 0:
             - one at the same principal quantum number 'n' of the (L)APW  for the given angular momentum ('l') channel.
             - the other at the principal quantum number 'n' of the semi core state.
         """
         valence_and_semicore_states = self.get_valence_and_semicore_atomicstate_ns_per_l()
-        semicore_states = {l: data['semicore'] for l, data in valence_and_semicore_states.items()}
+        semicore_states = {l: data["semicore"] for l, data in valence_and_semicore_states.items()}
 
         for l, ns in semicore_states.items():
             for n in ns:
-                self.add_lo(l, (n+1, n), (0, 0))
+                self.add_lo(l, (n + 1, n), (0, 0))
 
     def add_custom_for_all_valence_states(self, custom_type: str):
         """Adds a custom element to the basis for every valence state present in the atomic states.
-        
+
         :param custom_type: Type of the custom basis function. It can be either `apw`, `lapw`, or `apw+lo`.
         """
         valence_and_semicore_states = self.get_valence_and_semicore_atomicstate_ns_per_l()
-        valence_states = {l: data['valence'] for l, data in valence_and_semicore_states.items()}
+        valence_states = {l: data["valence"] for l, data in valence_and_semicore_states.items()}
 
         for l, ns in valence_states.items():
-            for n in ns: 
-                self.basis["custom"].append({'l': l, 'type': custom_type, 'n': n, 'searchE': False})
+            for n in ns:
+                self.basis["custom"].append({"l": l, "type": custom_type, "n": n, "searchE": False})
 
     def add_helos(self, l: int, number: int):
-        """Adds a specific 'number' of High Energy Local Orbitals (HELOs) to the basis 
+        """Adds a specific 'number' of High Energy Local Orbitals (HELOs) to the basis
         for a given angular momentum channel 'l'.
 
         :param l: angular momentum number l
         :param number: the number of HELOs to be added to the l-channel
         """
         first_helo_n_for_l = self.get_first_helo_n(l)
 
         for nr_lo in range(number):
-            self.add_lo(l, (first_helo_n_for_l + nr_lo, ) * 2, [0, 1])
+            self.add_lo(l, (first_helo_n_for_l + nr_lo,) * 2, [0, 1])
 
     def find_highest_matching_order_for_state(self, l: int, n: int) -> int:
-        """Returns the highest matching order for a specific state, defined by principal quantum numner 'n' and 
-        anguar momentum 'l', for which a local orbital exists in the species file.  
+        """Returns the highest matching order for a specific state, defined by principal quantum numner 'n' and
+        anguar momentum 'l', for which a local orbital exists in the species file.
 
         :param l: angular momentum number l
         :param n: principal quantum number n
         :return: highest matchingOrder mO
         """
 
         l_los = filter(lambda x: x["l"] == l, self.basis["lo"])
@@ -238,107 +240,104 @@
 
         return max(mOs, default=0)
 
     def add_lo_higher_matching_order(self, l: int, n: int):
         """Adds a Local Orbital with the next highest matching order for a state defined by angular momentum 'l'
         and principal quantum number 'n'.
 
-        :param l: angular momentum number 
-        :param n: principal quantum number 
+        :param l: angular momentum number
+        :param n: principal quantum number
         """
         mO = self.find_highest_matching_order_for_state(l, n)
         self.add_lo(l, (n, n), (mO, mO + 1))
 
     def add_lo(self, l: int, ns: Tuple[int, int], matching_orders: Tuple[int, int]):
-        """Adds a single local orbital to the basis for a given angular momentum channel 'l', 
+        """Adds a single local orbital to the basis for a given angular momentum channel 'l',
         with tuples of principal quantum number 'n' and corresponding 'matching_orders'.
 
         :param l: angular momentum number l
         :param ns: tuple of principal quantum number n
         :param matching_orders: tuple of matching orders
         """
-        assert len(ns) == len(matching_orders), \
-            "Number of principal quantum numbers n must equal the number of given matching orders."
+        assert len(ns) == len(
+            matching_orders
+        ), "Number of principal quantum numbers n must equal the number of given matching orders."
 
         if matching_orders[0] >= 3:
             warnings.warn("Maximum matchingOrder reached; cannot add new local orbital.")
-            return 
+            return
+
+        wf = [{"matchingOrder": mO, "searchE": False, "n": n} for mO, n in zip(matching_orders, ns)]
+        self.basis["lo"].append({"l": l, "wf": wf})
 
-        wf = [{'matchingOrder': mO, 'searchE': False, 'n': n} for mO, n in zip(matching_orders, ns)]
-        self.basis['lo'].append({'l': l, 'wf': wf})
-    
     def remove_lo(self, l: int, ns: Tuple[int, int], matching_orders: Tuple[int, int]) -> bool:
         """Removes a single local orbital from the basis for a given angular momentum channel 'l',
         based on a list of tuples, each containing a principal quantum number 'n' and its corresponding matching order.
         If a local orbital with the specified 'n' and matching orders is present in the basis, it is removed.
 
         :param l: Angular momentum number l.
         :param ns: tuple of principal quantum number n
         :param matching_orders: tuple of matching orders
         :return removed: Boolean indicating if the local orbital was present and removed.
         """
 
-        removed = False 
-        
+        removed = False
+
         for lo in self.basis["lo"]:
             ns_mOs_lo = sorted([(wf["n"], wf["matchingOrder"]) for wf in lo["wf"] if wf.get("n")])
             if lo["l"] == l and sorted(zip(ns, matching_orders)) == ns_mOs_lo:
                 removed = True
                 self.basis["lo"].remove(lo)
-                break 
+                break
 
         return removed
 
     def remove_lo_highest_matching_order(self, l: int, n: int) -> bool:
         """Removes the Local Orbital from the basis for a given angular momentum channel 'l' and
-         principal quantum number 'n' that contains the wave function with the highest matching order. 
-         If the local orbital to be removed is present in the basis, the returned boolean is set to True. 
+         principal quantum number 'n' that contains the wave function with the highest matching order.
+         If the local orbital to be removed is present in the basis, the returned boolean is set to True.
 
         :param l: angular momentum number l
         :param n: principal quantum number n
         :return removed: states if the given local orbital was present in the basis
         """
         mO = self.find_highest_matching_order_for_state(l, n)
 
-        return self.remove_lo(l, (n, n), (mO-1, mO))
+        return self.remove_lo(l, (n, n), (mO - 1, mO))
 
     def add_default(self, trial_energy: float, default_type: str):
         """Adds the default element with a given trial energy and type to the basis.
-        
+
         :param trial_energy: trial energy used in the default element
         :param default_type: type of the default basis functions. Can be either `apw`, `lapw`, or `apw+lo`.
         """
-        self.basis["default"].append({'type': default_type, 'trialEnergy': trial_energy, 'searchE': False})
+        self.basis["default"].append({"type": default_type, "trialEnergy": trial_energy, "searchE": False})
 
     def to_xml(self) -> ElementTree.Element:
         """Converts the class attributes into an XML structure using ElementTree.
 
         :return: An ElementTree.Element representing the root of the XML structure.
         """
         spdb = ElementTree.Element("spdb")
         sp = ElementTree.SubElement(spdb, "sp", {k: str(v) for k, v in self.species.items()})
         ElementTree.SubElement(sp, "muffinTin", {k: str(v) for k, v in self.muffin_tin.items()})
         for state in self.atomic_states:
-            ElementTree.SubElement(
-                sp, "atomicState", {k: str(v).lower() for k, v in state.items()}) 
+            ElementTree.SubElement(sp, "atomicState", {k: str(v).lower() for k, v in state.items()})
 
         basis = ElementTree.SubElement(sp, "basis")
         for default in self.basis["default"]:
-            ElementTree.SubElement(
-                basis, "default", {k: str(v).lower() for k, v in default.items()})
+            ElementTree.SubElement(basis, "default", {k: str(v).lower() for k, v in default.items()})
 
         for custom in self.basis["custom"]:
-            ElementTree.SubElement(
-                basis, "custom", {k: str(v).lower() for k, v in custom.items()})
+            ElementTree.SubElement(basis, "custom", {k: str(v).lower() for k, v in custom.items()})
 
         for lo in self.basis["lo"]:
             lo_element = ElementTree.SubElement(basis, "lo", l=str(lo["l"]))
-            for wf in lo['wf']:
-                ElementTree.SubElement(
-                    lo_element, "wf", {k: str(v).lower() for k, v in wf.items()})
+            for wf in lo["wf"]:
+                ElementTree.SubElement(lo_element, "wf", {k: str(v).lower() for k, v in wf.items()})
 
         return spdb
 
     def to_xml_str(self) -> str:
         """Compose XML ElementTrees from exciting input classes to create an input xml string.
 
         :return: Input XML tree as a string, with pretty formatting.
```

### Comparing `excitingtools-1.7.0/excitingtools/structure/ase_utilities.py` & `excitingtools-1.7.1/excitingtools/structure/ase_utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-""" Utilities for interaction with the ASE library. """
+"""Utilities for interaction with the ASE library."""
 
 from ase import Atoms
 
 from excitingtools import ExcitingStructure
 from excitingtools.constants.units import bohr_to_angstrom
 
 
 def exciting_structure_to_ase(structure: ExcitingStructure) -> Atoms:
-    """ Function to extract the physical structure from an exciting structure object
+    """Function to extract the physical structure from an exciting structure object
     and transforms it into an ase.atoms.Atoms object.
 
     :param structure: input exciting structure object
     :returns: ASE Atoms object
     """
     lattice = structure.get_lattice(convert_to_angstrom=True)
     if structure.structure_attributes.get("cartesian"):
         positions = structure.positions * bohr_to_angstrom
         return Atoms(symbols=structure.species, positions=positions, cell=lattice, pbc=True)
-    else:
-        return Atoms(symbols=structure.species, scaled_positions=structure.positions, cell=lattice, pbc=True)
+    return Atoms(symbols=structure.species, scaled_positions=structure.positions, cell=lattice, pbc=True)
```

### Comparing `excitingtools-1.7.0/excitingtools/structure/lattice.py` & `excitingtools-1.7.1/excitingtools/structure/lattice.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,62 +1,57 @@
-"""Functions that operate on a crystal lattice.
-"""
+"""Functions that operate on a crystal lattice."""
+
 import numpy as np
 
 from excitingtools.math.math_utils import triple_product
 
 
 def check_lattice(lattice: list):
     """Check lattice vector consistency.
 
     Checks that the user supplies three different lattice vectors.
     One could also check the lattice vector angles.
 
     :param list lattice: Lattice vectors
     """
     if len(lattice) != 3:
-        raise ValueError('lattice argument expected to have 3 elements')
+        raise ValueError("lattice argument expected to have 3 elements")
 
-    for i in range(0, 3):
+    for i in range(3):
         if len(lattice[i]) != 3:
-            raise ValueError(
-                f'lattice vector {i} expected to have 3 components. Instead has {len(lattice[i])}'
-            )
+            raise ValueError(f"lattice vector {i} expected to have 3 components. Instead has {len(lattice[i])}")
 
     for i, j in [(0, 1), (1, 2), (0, 2)]:
-        if np.allclose(lattice[i], lattice[j], atol=1.e-6):
-            raise ValueError(
-                f'lattice vectors {i} and {j} are numerically equivalent')
+        if np.allclose(lattice[i], lattice[j], atol=1.0e-6):
+            raise ValueError(f"lattice vectors {i} and {j} are numerically equivalent")
 
 
-def check_lattice_vector_norms(lattice: list, tol=1.e-6):
-    """ Check the norm of each lattice vector.
+def check_lattice_vector_norms(lattice: list, tol=1.0e-6):
+    """Check the norm of each lattice vector.
 
     :param list lattice: Lattice vectors
     :param tol: Optional tolerance for what is considered numerically zero.
     """
     norms = np.empty(shape=3)
 
-    for i in range(0, 3):
+    for i in range(3):
         norms[i] = np.linalg.norm(lattice[i])
 
     zero_norms = np.where(norms < tol)[0]
     for i in zero_norms:
-        raise ValueError(f'lattice vector {i} has a norm of zero')
+        raise ValueError(f"lattice vector {i} has a norm of zero")
 
 
 def parallelepiped_volume(lattice_vectors: np.ndarray) -> float:
     """Volume of a parallelepiped cell.
 
     :param np.ndarray lattice_vectors: Lattice vectors, stored column-wise
     :return: float: Cell volume
     """
-    return np.abs(
-        triple_product(lattice_vectors[:, 0], lattice_vectors[:, 1],
-                       lattice_vectors[:, 2]))
+    return np.abs(triple_product(lattice_vectors[:, 0], lattice_vectors[:, 1], lattice_vectors[:, 2]))
 
 
 def reciprocal_lattice_vectors(a: np.ndarray) -> np.ndarray:
     r"""
     Get the reciprocal lattice vectors of real-space lattice vectors \{\mathbf{a}\}:
 
       \mathbf{b}_0 = 2 \pi \frac{\mathbf{a}_1 \wedge \mathbf{a}_2} {\mathbf{a}_0 \cdot (\mathbf{a}_1 \wedge \mathbf{a}_2)}
@@ -71,31 +66,32 @@
     b[:, 0] = 2 * np.pi * np.cross(a[:, 1], a[:, 2]) / volume
     b[:, 1] = 2 * np.pi * np.cross(a[:, 2], a[:, 0]) / volume
     b[:, 2] = 2 * np.pi * np.cross(a[:, 0], a[:, 1]) / volume
     return b
 
 
 # TODO(Bene) This needs cleaning up. Missing any documenting maths. Not at all clear what's happening
-def plane_transformation(rec_lat_vec: np.array,
-                         plot_vec: np.array) -> np.array:
+def plane_transformation(rec_lat_vec: np.array, plot_vec: np.array) -> np.array:
     """
     Take reciprocal lattice vectors and ONS of a plane in rec. lat. coordinates where the first two vectors span the plane and the third is normal to them
     and calculate a matrix that transforms points in the plane to the xy plane in cartesian coordinates.
     input:
     :param rec_lat_vec:            reciprocal lattice vectors
     :param plot_vec:               ONS of the plotting plane
     :return transformation_matrix: matrix that transforms k and spin vectors to the plot plane
     """
     norm = np.linalg.norm
     # transform plot vec in cartesian coordinates
     plot_vec = (rec_lat_vec.dot(plot_vec)).transpose()
     # extend plot vec to an orthogonal system
-    plot_vec = np.array([(plot_vec[1] - plot_vec[0]) / norm(plot_vec[1] - plot_vec[0]),
-                         (plot_vec[2] - plot_vec[0]) / norm(plot_vec[2] - plot_vec[0]),
-                         np.cross(plot_vec[1] - plot_vec[0], plot_vec[2] - plot_vec[0]) \
-                         / norm(np.cross(plot_vec[1] - plot_vec[0], plot_vec[2] - plot_vec[0]))])
+    plot_vec = np.array(
+        [
+            (plot_vec[1] - plot_vec[0]) / norm(plot_vec[1] - plot_vec[0]),
+            (plot_vec[2] - plot_vec[0]) / norm(plot_vec[2] - plot_vec[0]),
+            np.cross(plot_vec[1] - plot_vec[0], plot_vec[2] - plot_vec[0])
+            / norm(np.cross(plot_vec[1] - plot_vec[0], plot_vec[2] - plot_vec[0])),
+        ]
+    )
     transformation_matrix = np.linalg.inv(plot_vec)
-    for v in transformation_matrix:
-        v = v / norm(v)
     transformation_matrix = np.transpose(transformation_matrix)
 
     return transformation_matrix
```

### Comparing `excitingtools-1.7.0/excitingtools/structure/pymatgen_utilities.py` & `excitingtools-1.7.1/excitingtools/structure/pymatgen_utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-""" Utilities to interact with the pymatgen library. """
+"""Utilities to interact with the pymatgen library."""
 
 from pymatgen.core import Structure
 
 from excitingtools import ExcitingStructure
 from excitingtools.constants.units import angstrom_to_bohr, bohr_to_angstrom
 
 
 def exciting_structure_to_pymatgen(structure: ExcitingStructure) -> Structure:
-    """ Function to extract the physical structure from an exciting structure object
+    """Function to extract the physical structure from an exciting structure object
     and transforms it into a pymatgen.core.structure.Structure object.
 
     :param structure: input exciting structure object
     :returns: pymatgen Structure object
     """
     lattice = structure.get_lattice(convert_to_angstrom=True)
     cartesian = structure.structure_attributes.get("cartesian", False)
     positions = structure.positions * bohr_to_angstrom if cartesian else structure.positions
     return Structure(lattice=lattice, species=structure.species, coords=positions, coords_are_cartesian=cartesian)
 
 
 def pymatgen_to_exciting_structure(structure: Structure) -> ExcitingStructure:
-    """ Initialise lattice, species and positions from a pymatgen Structure Object.
+    """Initialise lattice, species and positions from a pymatgen Structure Object.
     Note: pymatgen works in Angstrom, whereas exciting expects atomic units
 
     :param structure: pymatgen Structure object.
     :return exciting structure object
     """
     lattice = structure.lattice.matrix * angstrom_to_bohr
     species = [x.symbol.capitalize() for x in structure.species]
```

### Comparing `excitingtools-1.7.0/excitingtools/utils/dict_utils.py` & `excitingtools-1.7.1/excitingtools/utils/dict_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-""" Dictionary Utilities.
-"""
+"""Dictionary Utilities."""
+
+import contextlib
 import copy
 import json
 import sys
-from collections.abc import Mapping, Hashable, KeysView
+from collections.abc import Hashable, KeysView, Mapping
 from typing import Iterator, Union
 
 import numpy as np
 
 
 def common_iterable(obj: Union[dict, list]):
     """
@@ -16,43 +17,39 @@
 
         for index in common_iterable(d):
             print('index = key or integer index:', index)
             print('d[index] = dictionary value or list element:', d[index])
     """
     if isinstance(obj, dict):
         return obj
-    else:
-        return (index for index, value in enumerate(obj))
+    return (index for index, value in enumerate(obj))
 
 
 def __container_converter(data: Union[list, dict]) -> dict:
     """
     Converts string versions of numerical data from input dict into numerical data.
 
     :param dict data: Dictionary with string values.
     :return:dict data: Input dictionary with all string literal values converted to numerical values.
     """
     np_convert = {np.float64: float, np.int32: int}
 
     for element in common_iterable(data):
-        if isinstance(data[element], dict) or isinstance(data[element], list):
+        if isinstance(data[element], (dict, list)):
             data[element] = __container_converter(data[element])
         elif isinstance(data[element], np.ndarray):
             data[element] = data[element].tolist()
         elif isinstance(data[element], (np.float64, np.int32)):
             value = data[element]
             data[element] = np_convert[type(value)](value)
         elif isinstance(data[element], Hashable):
-            try:
+            with contextlib.suppress(Exception):
                 data[element] = json.loads(data[element])
-            except:
-                pass
         else:
-            message = 'Type not converted by dict converter: ' + str(
-                type(data[element]))
+            message = "Type not converted by dict converter: " + str(type(data[element]))
             sys.exit(message)
 
     return data
 
 
 def container_converter(data: dict) -> dict:
     """
@@ -87,15 +84,15 @@
 
     for index in common_iterable(d):
         # Can't iterate over a set with an index, and tuple cannot be mutated
         if isinstance(d[index], (set, tuple)):
             d[index] = list(d[index])
 
         # Class instances with the __dict__ attribute
-        if '__dict__' in dir(d[index]):
+        if "__dict__" in dir(d[index]):
             d[index] = vars(d[index])
 
         # Recursively apply routine to other containers
         elif not isinstance(d[index], Hashable):
             d[index] = serialise_dict_values(d[index])
 
         # pass over hashable values and np arrays
@@ -134,23 +131,22 @@
 
     :param dict dictionary: dictionary, mutated by function.
     :param list key_chain: List of keys leading to the item to be deleted.
     """
     if len(key_chain) == 1:
         del dictionary[key_chain[0]]
         return
-    else:
-        delete_nested_key(dictionary[key_chain[0]], key_chain[1:])
+    delete_nested_key(dictionary[key_chain[0]], key_chain[1:])
 
 
-def check_valid_keys(input_keys: Union[list, set, tuple, KeysView],
-                     valid_keys: Union[list, set, tuple, KeysView],
-                     name: str = ''):
-    """ Check that a given set of input keys are valid.
+def check_valid_keys(
+    input_keys: Union[list, set, tuple, KeysView], valid_keys: Union[list, set, tuple, KeysView], name: str = ""
+):
+    """Check that a given set of input keys are valid.
 
     :param input_keys: Input keys
     :param valid_keys: Valid keys
     :param name: Optional name for error message
     """
     erroneous_inputs = set(input_keys) - set(valid_keys)
     if erroneous_inputs:
-        raise ValueError(f'{name} keys are not valid: {erroneous_inputs}')
+        raise ValueError(f"{name} keys are not valid: {erroneous_inputs}")
```

### Comparing `excitingtools-1.7.0/excitingtools/utils/schema_parsing.py` & `excitingtools-1.7.1/excitingtools/utils/schema_parsing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-""" Parse the schema and generate a python file which can be read by the input classes.
+"""Parse the schema and generate a python file which can be read by the input classes.
 Should only be run if changes to the schema are made.
 """
+
 import re
 from pathlib import Path
 from typing import List
 
 import xmlschema
 from xmlschema.validators import XsdAnyElement
 
 from excitingtools.utils.utils import get_excitingtools_root
 
 
 def copy_schema_files_for_parsing(schema_files: List[str]) -> List[Path]:
-    """ Copies the schema files to the current directory.
+    """Copies the schema files to the current directory.
 
     Also generates a file (input.xsd) with schema extensions, with modified include paths.
     This is a work-around because the exciting documentation fails to compile
     when a schema with the modified include is used.
 
     :param schema_files: the name of the schema files and tags of the xml element
     :return file_list: A list of all generated or copied files.
@@ -53,72 +54,77 @@
         <xs:enumeration value="lattice coordinates"></xs:enumeration>
       </xs:restriction>
     </xs:simpleType>
   </xs:attribute>
   
 </xs:schema>"""
 
-    inputschemaextentions_path = Path(f'{inputschemaextentions_name}.xsd')
+    inputschemaextentions_path = Path(f"{inputschemaextentions_name}.xsd")
     inputschemaextentions_path.write_text(inputschemaextentions)
     root = get_excitingtools_root()
 
     # handling of the input.xsd file
-    inputschema_file = root / '../../xml/schema/input.xsd'
+    inputschema_file = root / "../../xml/schema/input.xsd"
     content = inputschema_file.read_text().split("\n")
-    content[1] = ('<xs:schema xmlns:ex="inputschemaextentions.xsd" '
-                  'xmlns:xs="http://www.w3.org/2001/XMLSchema" '
-                  'xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" '
-                  'xsi:schemaLocation="inputschemaextentions.xsd inputschemaextentions.xsd">')
+    content[1] = (
+        '<xs:schema xmlns:ex="inputschemaextentions.xsd" '
+        'xmlns:xs="http://www.w3.org/2001/XMLSchema" '
+        'xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" '
+        'xsi:schemaLocation="inputschemaextentions.xsd inputschemaextentions.xsd">'
+    )
     new_inputschema_file = Path("input.xsd")
     new_inputschema_file.write_text("\n".join(content))
 
     file_list = [inputschemaextentions_path, new_inputschema_file]
 
     # handling of all other included schema files
     for schema_name in schema_files:
-        schema_root = root / '../../xml/schema'
-        schema_reference = schema_root / f'{schema_name}.xsd'
+        schema_root = root / "../../xml/schema"
+        schema_reference = schema_root / f"{schema_name}.xsd"
         content = schema_reference.read_text().split("\n")
 
         content[1] = f'  xmlns:ex="{inputschemaextentions_name}.xsd"'
         content[3] = f'  xsi:schemaLocation="{inputschemaextentions_name}.xsd {inputschemaextentions_name}.xsd">'
         content = "\n".join(content)
 
         new_schema_file = Path(f"{schema_name}.xsd")
         new_schema_file.write_text(content)
         file_list.append(new_schema_file)
 
     return file_list
 
 
 def read_schema_to_dict(name: str) -> dict:
-    """ Read schema and transform to sensible dictionary.
+    """Read schema and transform to sensible dictionary.
 
     Note: This could be done with an external library, such as `xmltodict` or `xmljson`
     but as this module should be run infrequently, a custom implementation reduces
     dependencies.
 
     :param name: name of the schema file and tag of the xml element
     :return: a dictionary with the need information about children/parents and valid attributes.
     """
-    schema = xmlschema.XMLSchema(f'{name}.xsd')
+    schema = xmlschema.XMLSchema(f"{name}.xsd")
 
     tag_info = {}
     xsd_elements = filter(lambda x: isinstance(x, xmlschema.XsdElement) and x.ref is None, schema.iter_components())
 
     for xsd_element in xsd_elements:
         attributes = xsd_element.attributes
         mandatory_attributes = set([k for k, v in attributes.items() if v.use == "required"])
         children = [x.name for x in xsd_element.iterchildren() if not isinstance(x, XsdAnyElement)]
         mandatory_children = set([x.name for x in xsd_element.iterchildren() if x.min_occurs > 0])
         multiple_childs = set([x.name for x in xsd_element.iterchildren() if x.max_occurs is None or x.max_occurs > 1])
 
-        tag_info[xsd_element.name] = {"attribs": filter(lambda x: x is not None, attributes), "children": children,
-                                      "mandatory_attribs": mandatory_attributes | mandatory_children,
-                                      "multiple_children": multiple_childs}
+        tag_info[xsd_element.name] = {
+            "attribs": filter(lambda x: x is not None, attributes),
+            "children": children,
+            "mandatory_attribs": mandatory_attributes | mandatory_children,
+            "multiple_children": multiple_childs,
+        }
 
         # special handling for the plan
         if xsd_element.name == "doonly":
             tag_info["doonly"]["plan"] = attributes["task"].type.validators[0].enumeration
 
     # exclude special structure attributes (already explicitly specified in the __init__ of ExcitingStructure class)
     if name == "structure":
@@ -126,26 +132,26 @@
         tag_info["crystal"]["mandatory_attribs"].remove("basevect")
         tag_info["species"]["mandatory_attribs"].remove("atom")
 
     return tag_info
 
 
 def write_schema_info(super_tag: str, schema_dict: dict) -> str:
-    """ Converts dict representation of the schema to string.
+    """Converts dict representation of the schema to string.
 
     :param super_tag: name of the top-level element
     :param schema_dict: contains all the information read from the schema
     :return info_string: string of python-formatted code
     """
     info_string = f"\n# {super_tag} information \n"
     for tag in schema_dict:
         valid_attributes = sorted(schema_dict[tag]["attribs"])
-        valid_subtrees = schema_dict[tag]['children']
-        mandatory_attributes = sorted(schema_dict[tag]['mandatory_attribs'])
-        multiple_childs = sorted(schema_dict[tag]['multiple_children'])
+        valid_subtrees = schema_dict[tag]["children"]
+        mandatory_attributes = sorted(schema_dict[tag]["mandatory_attribs"])
+        multiple_childs = sorted(schema_dict[tag]["multiple_children"])
 
         if not (valid_attributes or valid_subtrees or mandatory_attributes):
             continue
 
         if valid_attributes:
             info_string += list_string_line_limit(f"{tag}_valid_attributes", valid_attributes) + " \n"
         if valid_subtrees:
@@ -155,70 +161,72 @@
         if multiple_childs:
             info_string += list_string_line_limit(f"{tag}_multiple_children", multiple_childs) + " \n"
         info_string += "\n"
     return info_string
 
 
 def list_string_line_limit(name: str, content: list, max_length: int = 120) -> str:
-    """ Given a list of unique items, produces a python formatted string containing the definition of the list
+    """Given a list of unique items, produces a python formatted string containing the definition of the list
     given by the name:
         name = ['entry1', 'entry2', ...]
     Inserts a line break every time the string gets longer then the limit.
 
     :param name: the name of the set in the final string representing the definition
     :param content: the list to write to string as a set (list because of consistent ordering)
     :param max_length: the maximum line length
     :return: the formatted string with fixed line length
     """
-    formatted_string = ''
-    current_line_string = name + ' = ['
+    formatted_string = ""
+    current_line_string = name + " = ["
     start_len = len(current_line_string)
-    entry_break_string = "', "
+    entry_break_string = '", '
 
     for entry in content:
         if len(str(entry) + current_line_string + entry_break_string) > max_length:
-            formatted_string += current_line_string + '\n'
-            current_line_string = start_len * ' '
-        current_line_string += f"'{entry}{entry_break_string}"
+            formatted_string += current_line_string + "\n"
+            current_line_string = start_len * " "
+        current_line_string += f'"{entry}{entry_break_string}'
 
     formatted_string += current_line_string[:-2] + "]"
     return formatted_string
 
 
 def get_all_include_files() -> list:
-    """ Gets a list of all included files in the input.xsd file.
-    """
-    input_schema_file = (get_excitingtools_root() / '../../xml/schema/input.xsd').resolve()
+    """Gets a list of all included files in the input.xsd file."""
+    input_schema_file = (get_excitingtools_root() / "../../xml/schema/input.xsd").resolve()
     if not input_schema_file.exists():
-        raise ValueError("Couldn't find exciting schema. Most likely you are using excitingtools outside of exciting."
-                         "To fix this, try installing excitingtools from source in editable (-e) mode.")
+        raise ValueError(
+            "Couldn't find exciting schema. Most likely you are using excitingtools outside of exciting."
+            "To fix this, try installing excitingtools from source in editable (-e) mode."
+        )
     return re.findall(r'<xs:include id=".*" schemaLocation="(.*)\.xsd"/>', input_schema_file.read_text())
 
 
 def main():
-    """ Main function to read the schema and write it to python readable file.
-    """
+    """Main function to read the schema and write it to python readable file."""
     filename = Path(__file__).parent / "valid_attributes.py"
-    info = '""" Automatically generated file with the valid attributes from the schema. \n' \
-           'Do not manually change. Instead, run "utils/schema_parsing.py" to regenerate. """ \n'
+    info = (
+        '""" Automatically generated file with the valid attributes from the schema. \n'
+        'Do not manually change. Instead, run "utils/schema_parsing.py" to regenerate. """ \n'
+    )
 
     schemas = get_all_include_files()
     tmp_files = copy_schema_files_for_parsing(schemas)
 
     input_schema_dict = {"input": read_schema_to_dict("input")["input"]}
     info += write_schema_info("input", input_schema_dict)
 
     for schema in schemas:
         schema_dict = read_schema_to_dict(schema)
         info += write_schema_info(schema, schema_dict)
 
     # Handle special case for 'xs' to handle the valid plan entries
     xs_schema_dict = read_schema_to_dict("xs")
     info += "\n# valid entries for the xs subtree 'plan'\n"
-    info += list_string_line_limit("valid_plan_entries", sorted(xs_schema_dict['doonly']['plan'])) + " \n"
+    info += list_string_line_limit("valid_plan_entries", sorted(xs_schema_dict["doonly"]["plan"])) + " \n"
 
     with open(filename, "w") as fid:
         fid.write(info)
 
     for file in tmp_files:
         file.unlink()
```

### Comparing `excitingtools-1.7.0/excitingtools/utils/test_utils.py` & `excitingtools-1.7.1/excitingtools/utils/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-""" Classes and functions to aid unit testing.
-"""
+"""Classes and functions to aid unit testing."""
+
 import pathlib
 
 
 class MockFile:
-    """ Single class for testing parsers that require either:
+    """Single class for testing parsers that require either:
        * File.
        * String contents of file.
 
     Usage:
     @pytest.fixture
     def file_mock(tmp_path):
        file = tmp_path / _file_name
        file.write_text(string_contents)
        return MockFile(file, string_contents)
     """
+
     def __init__(self, file: pathlib.Path, string: str):
         # File object
         self.file = file
         # File contents
         self.string = string
         # Name prepended by path
         self.full_path = self.file.as_posix()
```

### Comparing `excitingtools-1.7.0/excitingtools/utils/utils.py` & `excitingtools-1.7.1/excitingtools/utils/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-"""General utility functions. Typically, conversion/type-checking.
-"""
+"""General utility functions. Typically, conversion/type-checking."""
+
 import pathlib
 import re
-from typing import Union, List, Optional, Callable, Iterator, Iterable, Any
+from typing import Any, Callable, Iterable, Iterator, List, Optional, Union
 
 
 def get_excitingtools_root() -> pathlib.Path:
-    """ Get the root directory of excitingtools. """
+    """Get the root directory of excitingtools."""
     return pathlib.Path(__file__).parents[2]
 
 
 def can_be_float(value) -> bool:
     """
     Check if a value can be interpreted as a float
 
@@ -60,15 +60,15 @@
      string[line[5]: line[6]]
 
     :param str string: Input string
     :return List[int] indices: List of indices corresponding to
      new lines in string.
     """
     indices = [0]
-    indices += [m.start() + 1 for m in re.finditer('\n', string)]
+    indices += [m.start() + 1 for m in re.finditer("\n", string)]
     return indices
 
 
 def list_to_str(mylist: Iterable[Any], modifier: Optional[Callable] = None) -> str:
     """Convert a list or iterable to a lower-case string.
 
     :param mylist: the input iterable
@@ -77,15 +77,15 @@
     """
     if modifier is None:
         return " ".join([str(x).lower() for x in mylist])
     return " ".join([modifier(str(x).lower()) for x in mylist])
 
 
 def flatten_list(input_list: list) -> Iterator:
-    """ Flatten a list of lists and other elements.
+    """Flatten a list of lists and other elements.
 
     :param input_list: input list
     :return: an iterator for the flattened list
     """
     for x in input_list:
         if isinstance(x, list):
             yield from flatten_list(x)
```

### Comparing `excitingtools-1.7.0/excitingtools.egg-info/PKG-INFO` & `excitingtools-1.7.1/excitingtools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 Metadata-Version: 2.1
 Name: excitingtools
-Version: 1.7.0
+Version: 1.7.1
 Summary: Utilities for aiding in the construction of exciting inputs and the postprocessing exciting outputs.
 Author-email: Alexander Buccheri <alexander.buccheri@mpsd.mpg.de>, Fabian Peschel <peschelf@physik.hu-berlin.de>
 License: GNU GENERAL PUBLIC LICENSE, see 'COPYING.md'
 Project-URL: repository, https://github.com/exciting/excitingtools
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: schemaparsing
 License-File: COPYING.LESSER
 License-File: COPYING.md
+Requires-Dist: numpy>=1.14.5
+Requires-Dist: matplotlib>=2.2.0
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: ase>=3.20.0; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+Provides-Extra: schemaparsing
+Requires-Dist: xmlschema; extra == "schemaparsing"
 
 # excitingtools
 <span style="font-family:american typewriter; font-size:1em;">**excitingtools**</span> is a collection of 
 modules to facilitate the generation of <span style="font-family:american typewriter; font-size:1em;">**exciting**</span>
 inputs and the post-processing of <span style="font-family:american typewriter; font-size:1em;">**exciting**</span> outputs. 
 
 <span style="font-family:american typewriter; font-size:1em;">**excitingtools**</span> currently provides functionality for:
@@ -96,23 +102,34 @@
 """
 import numpy as np
 
 from excitingtools.maths.math_utils import triple_product
 ```
 Exposed modules, forming user API, should be defined in `__init__.py` where ever possible.
 
-## Code Formatting 
-We currently favour [yapf](https://github.com/google/yapf) formatter, which by default applies PEP8 formatting to 
-the code.  
+## Code Checking and Formatting 
+We currently favour the [ruff](https://github.com/astral-sh/ruff) formatter, which by default applies PEP8 formatting to 
+the code. Additional rule selection and configuration can be found in the `pyproject.toml` file.
 
-After installing yapf, if you are in the root directory of excitingtools, you can simply type:
+After installing ruff via pip, if you are in the root directory of excitingtools, you can simply type:
+```bash
+ruff check excitingtools/path/to/file.py
+```
+This will check the selected file for common errors. Without a path the whole project will be checked.
+
+Some problems can be solved automatically with enabling the `--fix` feature:
+```bash
+ruff check --fix excitingtools/path/to/file.py
+```
+Afterward, you can type
 ```bash
-yapf -i excitingtools/path/to/file.py
+ruff format excitingtools/path/to/file.py
 ```
-and it will do the formatting for you. Note: This will automatically use our custom `.style.yapf` style-file.
+and it will do the formatting for you for the selected file, or again for the whole project without an argument.
+Check out the [docs](https://docs.astral.sh/ruff/) for more options.
 
 ## Documentation 
 
 ### Writing Documentation
 All functions and classes should be documented. The favoured docstring is *reStructuredText*:
 
 ```python3
@@ -355,11 +372,12 @@
 ## Contributors
 The following people (in alphabetic order by their family names) have contributed to excitingtools:
 
 * Alexander Buccheri
 * Hannah Kleine
 * Martin Kuban
 * Benedikt Maurer
+* Ronaldo Pela
 * Fabian Peschel
 * Daniel Speckhard
 * Elisa Stephan
 * Mara Voiculescu
```

### Comparing `excitingtools-1.7.0/excitingtools.egg-info/SOURCES.txt` & `excitingtools-1.7.1/excitingtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `excitingtools-1.7.0/paper/joss_latex.template` & `excitingtools-1.7.1/paper/joss_latex.template`

 * *Files identical despite different names*

### Comparing `excitingtools-1.7.0/paper/latex.template` & `excitingtools-1.7.1/paper/latex.template`

 * *Files identical despite different names*

### Comparing `excitingtools-1.7.0/paper/paper.bib` & `excitingtools-1.7.1/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `excitingtools-1.7.0/paper/paper.md` & `excitingtools-1.7.1/paper/paper.md`

 * *Files identical despite different names*

### Comparing `excitingtools-1.7.0/tests/dataclasses/test_band_structure.py` & `excitingtools-1.7.1/tests/dataclasses/test_band_structure.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,59 +1,71 @@
-from excitingtools.dataclasses.band_structure import BandData
-import pytest
 import numpy as np
+import pytest
+
+from excitingtools.dataclasses.band_structure import BandData
 
 
 @pytest.fixture
 def band_data():
-    """ Initialise an instance of BandData, and check attributes are set correctly.
+    """Initialise an instance of BandData, and check attributes are set correctly.
     Reference data taken from 'bandstructure.xml' and 'bandstructure.dat' files for silver, containing only two bands
     and only 6 k-sampling points per band.
     """
 
-    ref_bands = np.array([[-3.37071333, 0.59519479],
-                          [-3.37071074, 0.59537998],
-                          [-3.37070519, 0.59575556],
-                          [-3.3706986, 0.59616303],
-                          [-3.3706822, 0.59664939],
-                          [-3.37066123, 0.59639211]])
-
-    ref_k_points = np.array([[1.000000, 0.000000, 0.000000],
-                             [0.988281, 0.011719, 0.000000],
-                             [0.976562, 0.023438, 0.000000],
-                             [0.964844, 0.035156, 0.000000],
-                             [0.953125, 0.046875, 0.000000],
-                             [0.941406, 0.058594, 0.000000]])
+    ref_bands = np.array(
+        [
+            [-3.37071333, 0.59519479],
+            [-3.37071074, 0.59537998],
+            [-3.37070519, 0.59575556],
+            [-3.3706986, 0.59616303],
+            [-3.3706822, 0.59664939],
+            [-3.37066123, 0.59639211],
+        ]
+    )
+
+    ref_k_points = np.array(
+        [
+            [1.000000, 0.000000, 0.000000],
+            [0.988281, 0.011719, 0.000000],
+            [0.976562, 0.023438, 0.000000],
+            [0.964844, 0.035156, 0.000000],
+            [0.953125, 0.046875, 0.000000],
+            [0.941406, 0.058594, 0.000000],
+        ]
+    )
 
     ref_e_fermi = 0.0
 
-    ref_flattened_k_points = np.array([0., 0.02697635, 0.05395270, 0.08092905, 0.10790540, 0.13488176])
+    ref_flattened_k_points = np.array([0.0, 0.02697635, 0.05395270, 0.08092905, 0.10790540, 0.13488176])
 
-    ref_vertices = [{'distance': 0.0, 'label': 'Gamma', 'coord': [0.0, 0.0, 0.0]},
-                    {'distance': 0.8632432750, 'label': 'K', 'coord': [0.625, 0.375, 0.0]},
-                    {'distance': 1.150991033, 'label': 'X', 'coord': [0.5, 0.5, 0.0]},
-                    {'distance': 1.964864598, 'label': 'G', 'coord': [0.0, 0.0, 0.0]},
-                    {'distance': 2.669699781, 'label': 'L', 'coord': [0.5, 0.0, 0.0]}]
+    ref_vertices = [
+        {"distance": 0.0, "label": "Gamma", "coord": [0.0, 0.0, 0.0]},
+        {"distance": 0.8632432750, "label": "K", "coord": [0.625, 0.375, 0.0]},
+        {"distance": 1.150991033, "label": "X", "coord": [0.5, 0.5, 0.0]},
+        {"distance": 1.964864598, "label": "G", "coord": [0.0, 0.0, 0.0]},
+        {"distance": 2.669699781, "label": "L", "coord": [0.5, 0.0, 0.0]},
+    ]
 
     band_data = BandData(ref_bands, ref_k_points, ref_e_fermi, ref_flattened_k_points, ref_vertices)
 
-    assert band_data.n_k_points == band_data.bands.shape[0], (
-        "First dim of bands array equals the number of k-sampling points in the band structure")
+    assert (
+        band_data.n_k_points == band_data.bands.shape[0]
+    ), "First dim of bands array equals the number of k-sampling points in the band structure"
     assert band_data.n_k_points == 6, "sampling points per band"
     assert band_data.n_bands == 2, "band_structure_xml contains two bands"
-    assert np.allclose(band_data.k_points, ref_k_points, atol=1.e-8)
-    assert np.allclose(band_data.bands, ref_bands, atol=1.e-8)
+    assert np.allclose(band_data.k_points, ref_k_points, atol=1.0e-8)
+    assert np.allclose(band_data.bands, ref_bands, atol=1.0e-8)
     assert band_data.vertices == ref_vertices
 
     return band_data
 
 
 def test_xticks_and_labels(band_data):
     flattened_high_sym_points_ref = [0.000000000, 0.86324327, 1.15099103, 1.9648646, 2.66969978]
-    unicode_gamma = '\u0393'
+    unicode_gamma = "\u0393"
     labels_ref = [unicode_gamma, "K", "X", unicode_gamma, "L"]
 
     flattened_high_sym_points, labels = band_data.band_path()
 
     assert np.allclose(flattened_high_sym_points, flattened_high_sym_points_ref)
     assert labels == labels_ref
```

### Comparing `excitingtools-1.7.0/tests/dataclasses/test_eigenvalues.py` & `excitingtools-1.7.1/tests/dataclasses/test_eigenvalues.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,51 @@
+from typing import List
+
 import numpy as np
 import pytest
-from typing import List
 
-from excitingtools.dataclasses.data_structs import NumberOfStates, PointIndex, BandIndices
+from excitingtools.dataclasses.data_structs import BandIndices, NumberOfStates, PointIndex
 from excitingtools.dataclasses.eigenvalues import EigenValues
 
 
 @pytest.fixture
 def eigenvalues_instance():
-    """ Initialise an instance of EigenValues, and check attributes are set correctly.
+    """Initialise an instance of EigenValues, and check attributes are set correctly.
     Reference data taken from `evalqp_oxygen` in test_gw_eigenvalues.py
 
     G0W0 band structure
 
     Band index of VBM:  21
     Band index of CBm:  22
 
     Indirect BandGap (eV):                    5.3790
     at k(VBM) =    0.000   0.500   0.500 ik =     3
        k(CBm) =    0.000   0.000   0.000 ik =     1
     Direct Bandgap at k(VBM) (eV):            5.5451
     Direct Bandgap at k(CBm) (eV):            5.9468
     """
-    ref_gw_eigenvalues = np.array([[-0.12905, -0.12891, -0.12896,  0.08958,  0.08957,  0.18396],
-                                   [-0.19801, -0.17047, -0.17035,  0.11429,  0.11430,  0.19514],
-                                   [-0.15828, -0.15818, -0.10809,  0.09569,  0.14613,  0.18404]])
-
-    ref_k_points = np.array([[0.000000, 0.000000, 0.000000],
-                             [0.000000, 0.000000, 0.500000],
-                             [0.000000, 0.500000, 0.500000]])
+    ref_gw_eigenvalues = np.array(
+        [
+            [-0.12905, -0.12891, -0.12896, 0.08958, 0.08957, 0.18396],
+            [-0.19801, -0.17047, -0.17035, 0.11429, 0.11430, 0.19514],
+            [-0.15828, -0.15818, -0.10809, 0.09569, 0.14613, 0.18404],
+        ]
+    )
+
+    ref_k_points = np.array(
+        [[0.000000, 0.000000, 0.000000], [0.000000, 0.000000, 0.500000], [0.000000, 0.500000, 0.500000]]
+    )
 
     ref_weights = [0.125, 0.5, 0.375000]
 
     ref_occupations = np.array([[2, 2, 2, 0, 0, 0], [2, 2, 2, 0, 0, 0], [2, 2, 2, 0, 0, 0]])
 
-    eigen_values = EigenValues(NumberOfStates(19, 24), ref_k_points, [1, 2, 3], ref_gw_eigenvalues, ref_weights,
-                               ref_occupations)
+    eigen_values = EigenValues(
+        NumberOfStates(19, 24), ref_k_points, [1, 2, 3], ref_gw_eigenvalues, ref_weights, ref_occupations
+    )
 
     assert ref_gw_eigenvalues.shape == (len(eigen_values.k_points), eigen_values.state_range.n_states)
     assert eigen_values.state_range.first_state == 19
     assert eigen_values.state_range.last_state == 24
     assert np.allclose(eigen_values.k_points, ref_k_points)
     assert eigen_values.k_indices == [1, 2, 3]
     assert np.allclose(eigen_values.all_eigenvalues, ref_gw_eigenvalues), "GW column eigenvalues, for all k-points"
@@ -75,38 +81,38 @@
     assert k_points_and_indices[0].index == 1
     assert k_points_and_indices[1].index == 2
     assert k_points_and_indices[2].index == 3
 
 
 def test_class_eigenvalues_get_eigenvalues(eigenvalues_instance):
     eigenvalues = eigenvalues_instance.get_eigenvalues(k_point=[0.0, 0.5, 0.5])
-    assert np.allclose(eigenvalues,
-                       [-0.15828, -0.15818, -0.10809, 0.09569, 0.14613, 0.18404])
+    assert np.allclose(eigenvalues, [-0.15828, -0.15818, -0.10809, 0.09569, 0.14613, 0.18404])
 
-    assert eigenvalues_instance.get_eigenvalues(k_point=[0.5, 0.5, 0.5]).size == 0, \
-        "No k-point, hence eigenvalues"
+    assert eigenvalues_instance.get_eigenvalues(k_point=[0.5, 0.5, 0.5]).size == 0, "No k-point, hence eigenvalues"
 
 
 def test_class_eigenvalues_band_gap(eigenvalues_instance):
     k_valence = [0.000, 0.500, 0.500]
     k_conduction = [0.000, 0.000, 0.000]
 
     indirect_band_gap = eigenvalues_instance.band_gap(BandIndices(21, 22), k_points=[k_valence, k_conduction])
     direct_band_gap_at_Gamma = eigenvalues_instance.band_gap(BandIndices(21, 22), k_points=[k_conduction, k_conduction])
 
-    assert np.isclose(indirect_band_gap, 0.19767), 'Indirect band gap in Ha'
-    assert np.isclose(direct_band_gap_at_Gamma, 0.218540887), 'Direct band gap at Gamma, in Ha'
+    assert np.isclose(indirect_band_gap, 0.19767), "Indirect band gap in Ha"
+    assert np.isclose(direct_band_gap_at_Gamma, 0.218540887), "Direct band gap at Gamma, in Ha"
 
 
 def test_class_eigenvalues_get_transition_energy(eigenvalues_instance):
     k_valence = [0.000, 0.500, 0.500]
     k_conduction = [0.000, 0.000, 0.000]
 
     indirect_gap = eigenvalues_instance.get_transition_energy(k_valence, k_conduction)
-    direct_gap_at_Gamma =eigenvalues_instance.get_transition_energy(k_conduction, k_conduction)
+    direct_gap_at_Gamma = eigenvalues_instance.get_transition_energy(k_conduction, k_conduction)
 
-    assert np.isclose(indirect_gap, 0.19767), 'Transition energy for X→Γ, in Ha'
-    assert np.isclose(direct_gap_at_Gamma, 0.21854), 'Transition energy for Γ→Γ, in Ha'
+    assert np.isclose(indirect_gap, 0.19767), "Transition energy for X→Γ, in Ha"
+    assert np.isclose(direct_gap_at_Gamma, 0.21854), "Transition energy for Γ→Γ, in Ha"
 
     with pytest.raises(ValueError, match="Requested conduction k-point \\[1, 1, 1\\] not present."):
-        eigenvalues_instance.get_transition_energy(k_valence, [1, 1, 1]), \
-        "ValueError is returned if k-point is not matched."
+        (
+            eigenvalues_instance.get_transition_energy(k_valence, [1, 1, 1]),
+            "ValueError is returned if k-point is not matched.",
+        )
```

### Comparing `excitingtools-1.7.0/tests/dict_parsers/test_RT_TDDFT_parser.py` & `excitingtools-1.7.1/tests/dict_parsers/test_RT_TDDFT_parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 """
 Test for the RT_TDDFT_parser
 """
 
-import pytest
 import numpy as np
+import pytest
 
 from excitingtools.exciting_dict_parsers.RT_TDDFT_parser import parse_proj_screenshots
 
 proj_file_str_square_matrices = """ ik:          1
    1.00000   0.00000
    0.00000   1.00000
  ik:          2
    1.00000   0.00000
    0.00000   1.00000
 """
 
 reference_parsed_proj_square_matrices = {
-    'ik': [1, 2],
-    'projection': [ np.array([[1., 0.], [0., 1.]]), 
-                    np.array([[1., 0.], [0., 1.]])]
-    }
+    "ik": [1, 2],
+    "projection": [np.array([[1.0, 0.0], [0.0, 1.0]]), np.array([[1.0, 0.0], [0.0, 1.0]])],
+}
 
 proj_file_str_rectangular_matrices = """ ik:          1
    1.00000   0.00000   0.00000
    0.00000   1.00000   0.00000
  ik:          2
    0.60000   0.80000   0.00000
    0.00000   0.00000   1.00000
 """
 
 reference_parsed_proj_rectangular_matrices = {
-    'ik': [1, 2],
-    'projection': [ np.array([[1., 0., 0.], [0., 1., 0.]]), 
-                    np.array([[0.6, 0.8, 0.], [0., 0., 1.]])]
-    }
-
-@pytest.mark.parametrize(["proj_file_str", "reference_parsed_dict"],
-                         [(proj_file_str_square_matrices, reference_parsed_proj_square_matrices),
-                          (proj_file_str_rectangular_matrices, reference_parsed_proj_rectangular_matrices)])
+    "ik": [1, 2],
+    "projection": [np.array([[1.0, 0.0, 0.0], [0.0, 1.0, 0.0]]), np.array([[0.6, 0.8, 0.0], [0.0, 0.0, 1.0]])],
+}
+
+
+@pytest.mark.parametrize(
+    ["proj_file_str", "reference_parsed_dict"],
+    [
+        (proj_file_str_square_matrices, reference_parsed_proj_square_matrices),
+        (proj_file_str_rectangular_matrices, reference_parsed_proj_rectangular_matrices),
+    ],
+)
 def test_parse_proj_screenshots(proj_file_str, reference_parsed_dict, tmp_path):
     proj_file_path = tmp_path / "PROJ_0.OUT"
     proj_file_path.write_text(proj_file_str)
     proj_out = parse_proj_screenshots(proj_file_path.as_posix())
-    is_equal = ( proj_out['ik'] == reference_parsed_dict['ik'] )
-    key = 'projection'
-    is_equal = is_equal and all( [np.allclose(x, y) for (x,y) in 
-                                  zip(proj_out[key],reference_parsed_dict[key])] )
-    assert is_equal
+    is_equal = proj_out["ik"] == reference_parsed_dict["ik"]
+    key = "projection"
+    is_equal = is_equal and all([np.allclose(x, y) for (x, y) in zip(proj_out[key], reference_parsed_dict[key])])
+    assert is_equal
```

### Comparing `excitingtools-1.7.0/tests/dict_parsers/test_bse_parser.py` & `excitingtools-1.7.1/tests/dict_parsers/test_bse_parser.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Test bse parsers.
 The infoxs reference is boiled down to the necessary parts for a test.
 Execute tests from exciting_tools directory:
 pytest --capture=tee-sys
 """
+
 import pytest
 
 from excitingtools.exciting_dict_parsers.bse_parser import parse_infoxs_out
 
 infoxs_file_str_success = """================================================================================
 | EXCITING NITROGEN-14 started for task xsgeneigvec (301)                      =
 | version hash id: 1775bff4453c84689fb848894a9224f155377cfc                    =
@@ -247,77 +248,156 @@
 | EXCITING NITROGEN-14 started for task scrwritepmat (420)                     =
 | Date (DD-MM-YYYY) : 10-12-2020                                               =
 ================================================================================
 """
 
 
 reference_parsed_infoxs_file_success = {
-    'tasks': [{'name': 'xsgeneigvec', 'number': 301, 'finished': True}, 
-              {'name': 'writepmatxs', 'number': 320, 'finished': True},
-              {'name': 'scrgeneigvec', 'number': 401, 'finished': True}, 
-              {'name': 'scrwritepmat', 'number': 420, 'finished': True},
-              {'name': 'bse', 'number': 445, 'finished': True}],
-    'success': True,
-    'last_finished_task': 'bse'
-    }
+    "tasks": [
+        {"name": "xsgeneigvec", "number": 301, "finished": True},
+        {"name": "writepmatxs", "number": 320, "finished": True},
+        {"name": "scrgeneigvec", "number": 401, "finished": True},
+        {"name": "scrwritepmat", "number": 420, "finished": True},
+        {"name": "bse", "number": 445, "finished": True},
+    ],
+    "success": True,
+    "last_finished_task": "bse",
+}
 
 reference_parsed_infoxs_file_fail = {
-    'tasks': [{'name': 'xsgeneigvec', 'number': 301, 'finished': True}, 
-              {'name': 'writepmatxs', 'number': 320, 'finished': False},
-              {'name': 'xsgeneigvec', 'number': 301, 'finished': True}, 
-              {'name': 'writepmatxs', 'number': 320, 'finished': True},
-              {'name': 'scrgeneigvec', 'number': 401, 'finished': True}, 
-              {'name': 'scrwritepmat', 'number': 420, 'finished': False}],
-    'success': False,
-    'last_finished_task': 'scrgeneigvec'
-    }
-
-
-@pytest.mark.parametrize(["infoxs_file_str", "reference_parsed_dict"],
-                         [(infoxs_file_str_success, reference_parsed_infoxs_file_success),
-                          (infoxs_file_str_fail, reference_parsed_infoxs_file_fail)])
+    "tasks": [
+        {"name": "xsgeneigvec", "number": 301, "finished": True},
+        {"name": "writepmatxs", "number": 320, "finished": False},
+        {"name": "xsgeneigvec", "number": 301, "finished": True},
+        {"name": "writepmatxs", "number": 320, "finished": True},
+        {"name": "scrgeneigvec", "number": 401, "finished": True},
+        {"name": "scrwritepmat", "number": 420, "finished": False},
+    ],
+    "success": False,
+    "last_finished_task": "scrgeneigvec",
+}
+
+
+@pytest.mark.parametrize(
+    ["infoxs_file_str", "reference_parsed_dict"],
+    [
+        (infoxs_file_str_success, reference_parsed_infoxs_file_success),
+        (infoxs_file_str_fail, reference_parsed_infoxs_file_fail),
+    ],
+)
 def test_parse_info_xs_out(infoxs_file_str, reference_parsed_dict, tmp_path):
     infoxs_file_path = tmp_path / "INFOXS.OUT"
     infoxs_file_path.write_text(infoxs_file_str)
     info_xs_out = parse_infoxs_out(infoxs_file_path.as_posix())
     assert info_xs_out == reference_parsed_dict
 
 
 reference_parsed_infoxs_file_times_success = {
-    'tasks': [{'name': 'xsgeneigvec', 'number': 301, 'finished': True,
-               'cpu_time': 14.57, 'wall_time': 2.13, 'cpu_time_cum': 111.58, 'wall_time_cum': 2.13}, 
-              {'name': 'writepmatxs', 'number': 320, 'finished': True,
-               'cpu_time': 14.57, 'wall_time': 2.13, 'cpu_time_cum': 111.58, 'wall_time_cum': 2.13},
-              {'name': 'scrgeneigvec', 'number': 401, 'finished': True,
-               'cpu_time': 14.57, 'wall_time': 2.13, 'cpu_time_cum': 111.58, 'wall_time_cum': 2.13}, 
-              {'name': 'scrwritepmat', 'number': 420, 'finished': True,
-              'cpu_time': 14.57, 'wall_time': 2.13, 'cpu_time_cum': 111.58, 'wall_time_cum': 2.13},
-              {'name': 'bse', 'number': 445, 'finished': True,
-               'cpu_time': 14.57, 'wall_time': 2.13, 'cpu_time_cum': 111.58, 'wall_time_cum': 2.13}],
-    'success': True,
-    'last_finished_task': 'bse'
-    }
+    "tasks": [
+        {
+            "name": "xsgeneigvec",
+            "number": 301,
+            "finished": True,
+            "cpu_time": 14.57,
+            "wall_time": 2.13,
+            "cpu_time_cum": 111.58,
+            "wall_time_cum": 2.13,
+        },
+        {
+            "name": "writepmatxs",
+            "number": 320,
+            "finished": True,
+            "cpu_time": 14.57,
+            "wall_time": 2.13,
+            "cpu_time_cum": 111.58,
+            "wall_time_cum": 2.13,
+        },
+        {
+            "name": "scrgeneigvec",
+            "number": 401,
+            "finished": True,
+            "cpu_time": 14.57,
+            "wall_time": 2.13,
+            "cpu_time_cum": 111.58,
+            "wall_time_cum": 2.13,
+        },
+        {
+            "name": "scrwritepmat",
+            "number": 420,
+            "finished": True,
+            "cpu_time": 14.57,
+            "wall_time": 2.13,
+            "cpu_time_cum": 111.58,
+            "wall_time_cum": 2.13,
+        },
+        {
+            "name": "bse",
+            "number": 445,
+            "finished": True,
+            "cpu_time": 14.57,
+            "wall_time": 2.13,
+            "cpu_time_cum": 111.58,
+            "wall_time_cum": 2.13,
+        },
+    ],
+    "success": True,
+    "last_finished_task": "bse",
+}
 
 reference_parsed_infoxs_file_times_fail = {
-    'tasks': [{'name': 'xsgeneigvec', 'number': 301, 'finished': True,
-               'cpu_time': 14.57, 'wall_time': 2.13, 'cpu_time_cum': 111.58, 'wall_time_cum': 2.13}, 
-              {'name': 'writepmatxs', 'number': 320, 'finished': False},
-              {'name': 'xsgeneigvec', 'number': 301, 'finished': True,
-               'cpu_time': 14.57, 'wall_time': 2.13, 'cpu_time_cum': 111.58, 'wall_time_cum': 2.13}, 
-              {'name': 'writepmatxs', 'number': 320, 'finished': True,
-               'cpu_time': 14.57, 'wall_time': 2.13, 'cpu_time_cum': 111.58, 'wall_time_cum': 2.13},
-              {'name': 'scrgeneigvec', 'number': 401, 'finished': True,
-               'cpu_time': 14.57, 'wall_time': 2.13, 'cpu_time_cum': 111.58, 'wall_time_cum': 2.13}, 
-              {'name': 'scrwritepmat', 'number': 420, 'finished': False}],
-    'success': False,
-    'last_finished_task': 'scrgeneigvec'
-    }
-
-
-@pytest.mark.parametrize(["infoxs_file_str", "reference_parsed_dict"],
-                         [(infoxs_file_str_success, reference_parsed_infoxs_file_times_success),
-                          (infoxs_file_str_fail, reference_parsed_infoxs_file_times_fail)])
+    "tasks": [
+        {
+            "name": "xsgeneigvec",
+            "number": 301,
+            "finished": True,
+            "cpu_time": 14.57,
+            "wall_time": 2.13,
+            "cpu_time_cum": 111.58,
+            "wall_time_cum": 2.13,
+        },
+        {"name": "writepmatxs", "number": 320, "finished": False},
+        {
+            "name": "xsgeneigvec",
+            "number": 301,
+            "finished": True,
+            "cpu_time": 14.57,
+            "wall_time": 2.13,
+            "cpu_time_cum": 111.58,
+            "wall_time_cum": 2.13,
+        },
+        {
+            "name": "writepmatxs",
+            "number": 320,
+            "finished": True,
+            "cpu_time": 14.57,
+            "wall_time": 2.13,
+            "cpu_time_cum": 111.58,
+            "wall_time_cum": 2.13,
+        },
+        {
+            "name": "scrgeneigvec",
+            "number": 401,
+            "finished": True,
+            "cpu_time": 14.57,
+            "wall_time": 2.13,
+            "cpu_time_cum": 111.58,
+            "wall_time_cum": 2.13,
+        },
+        {"name": "scrwritepmat", "number": 420, "finished": False},
+    ],
+    "success": False,
+    "last_finished_task": "scrgeneigvec",
+}
+
+
+@pytest.mark.parametrize(
+    ["infoxs_file_str", "reference_parsed_dict"],
+    [
+        (infoxs_file_str_success, reference_parsed_infoxs_file_times_success),
+        (infoxs_file_str_fail, reference_parsed_infoxs_file_times_fail),
+    ],
+)
 def test_parse_info_xs_out_timing(infoxs_file_str, reference_parsed_dict, tmp_path):
     infoxs_file_path = tmp_path / "INFOXS.OUT"
     infoxs_file_path.write_text(infoxs_file_str)
     info_xs_out = parse_infoxs_out(infoxs_file_path.as_posix(), parse_timing=True)
     assert info_xs_out == reference_parsed_dict
```

### Comparing `excitingtools-1.7.0/tests/dict_parsers/test_groundstate_parser.py` & `excitingtools-1.7.1/tests/dict_parsers/test_groundstate_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """
 Test ground state parsers
 Execute tests from exciting_tools directory:
 pytest --capture=tee-sys
 """
-from excitingtools.exciting_dict_parsers.groundstate_parser import parse_info_out
-from excitingtools.exciting_dict_parsers.groundstate_parser import parse_linengy
-from excitingtools.exciting_dict_parsers.groundstate_parser import parse_lo_recommendation
+
+from excitingtools.exciting_dict_parsers.groundstate_parser import (
+    parse_info_out,
+    parse_linengy,
+    parse_lo_recommendation,
+)
 
 
 def test_parse_info_out(tmp_path):
     """
     Note, this test will break if:
       * the parser keys change
       * the structure of the output changes
@@ -21,25 +24,15 @@
     info_ref = {
         "initialization": {
             "APW functions": 8,
             "Brillouin zone volume": 0.0734963595,
             "Effective Wigner radius, r_s": 3.55062021,
             "Exchange-correlation type": 100,
             "G-vector grid sizes": "36    36    36",
-            "Lattice vectors (cartesian)": [
-                15.0,
-                0.0,
-                0.0,
-                0.0,
-                15.0,
-                0.0,
-                0.0,
-                0.0,
-                15.0,
-            ],
+            "Lattice vectors (cartesian)": [15.0, 0.0, 0.0, 0.0, 15.0, 0.0, 0.0, 0.0, 15.0],
             "Maximum Hamiltonian size": 263,
             "Maximum number of plane-waves": 251,
             "Maximum |G+k| for APW functions": 1.66666667,
             "Maximum |G| for potential and density": 7.5,
             "Number of Bravais lattice symmetries": 48,
             "Number of crystal symmetries": 48,
             "Number of empty states": 5,
@@ -56,17 +49,15 @@
                 0.0,
                 0.4188790205,
             ],
             "Smearing scheme": "Gaussian",
             "Smearing width": 0.001,
             "Species 1": {
                 "# of radial points in muffin-tin": 1000,
-                "Atomic positions": {
-                    "Atom 1": "0.00000000  0.00000000  0.00000000"
-                },
+                "Atomic positions": {"Atom 1": "0.00000000  0.00000000  0.00000000"},
                 "Species": "1 (Ar)",
                 "Species symbol": "Ar",
                 "atomic mass": 72820.7492,
                 "electronic charge": 18.0,
                 "muffin-tin radius": 6.0,
                 "name": "argon",
                 "nuclear charge": -18.0,
@@ -145,28 +136,28 @@
                 "core": 10.0,
                 "core leakage": 0.0,
                 "interstitial": 0.00184037,
                 "total charge": 18.0,
                 "total charge in muffin-tins": 17.99815963,
                 "valence": 8.0,
                 "xc potential energy": -38.82693481,
-            }
-        }
+            },
+        },
     }
 
-    file = tmp_path / 'INFO.OUT'
+    file = tmp_path / "INFO.OUT"
     file.write_text(LDA_VWN_Ar_INFO_OUT)
     assert file.exists(), "INFO.OUT not written to tmp_path"
 
     info_out = parse_info_out(file.as_posix())
 
-    assert info_out['initialization'] == info_ref['initialization'], "Initialization data consistent"
+    assert info_out["initialization"] == info_ref["initialization"], "Initialization data consistent"
     assert len(info_out["scl"]) == 12, "expected 12 SCF steps"
-    assert info_out['scl']['1'] == info_ref['scl']['1'], "SCF first iteration data consistent"
-    assert info_out['scl']['12'] == info_ref['scl']['12'], "SCF last iteration data consistent"
+    assert info_out["scl"]["1"] == info_ref["scl"]["1"], "SCF first iteration data consistent"
+    assert info_out["scl"]["12"] == info_ref["scl"]["12"], "SCF last iteration data consistent"
 
 
 LDA_VWN_Ar_INFO_OUT = """================================================================================
 | EXCITING NITROGEN-14 started                                                 =
 | version hash id: 1775bff4453c84689fb848894a9224f155377cfc                    =
 |                                                                              =
 |                                                                              =
@@ -807,63 +798,30 @@
     """
 
     # Reference of the dictionary parsed with parse_linengy
     # Generated with print(json.dumps(info_out, sort_keys=True, indent=4))
 
     linengy_ref = {
         "0": {
-            "apw": [
-                -2.1,
-                -1.1,
-                0.15,
-                0.15,
-                0.15,
-                0.15,
-                0.15,
-                0.15,
-                0.15,
-                0.15,
-                0.15,
-                0.15,
-                0.15,
-                0.15,
-                0.15,
-                0.15,
-            ],
+            "apw": [-2.1, -1.1, 0.15, 0.15, 0.15, 0.15, 0.15, 0.15, 0.15, 0.15, 0.15, 0.15, 0.15, 0.15, 0.15, 0.15],
             "lo": [
                 1.839014478,
                 1.839014478,
                 -0.7435250385,
                 -0.7435250385,
                 1.839014478,
                 1.839014478,
                 1.839014478,
                 -1.775228393,
                 -0.7435250385,
                 -0.7435250385,
-            ]
+            ],
         },
         "1": {
-            "apw": [
-                -0.3,
-                0.15,
-                0.15,
-                0.15,
-                0.15,
-                0.15,
-                0.15,
-                0.15,
-                0.15,
-                0.15,
-                0.15,
-                0.15,
-                0.15,
-                0.15,
-                0.15,
-            ],
+            "apw": [-0.3, 0.15, 0.15, 0.15, 0.15, 0.15, 0.15, 0.15, 0.15, 0.15, 0.15, 0.15, 0.15, 0.15, 0.15],
             "lo": [
                 0.7475318132,
                 0.7475318132,
                 1.385527458,
                 1.385527458,
                 1.974765418,
                 1.974765418,
@@ -881,28 +839,28 @@
                 -6.768218591,
                 -6.768218591,
                 -6.768218591,
                 -6.768218591,
                 -6.768218591,
                 1.974765418,
                 1.974765418,
-            ]
-        }
+            ],
+        },
     }
 
-    file = tmp_path / 'LINENGY.OUT'
+    file = tmp_path / "LINENGY.OUT"
     file.write_text(GGA_PBE_SOL_automatic_trial_energies_NaCl_LINENGY_OUT)
     assert file.exists(), "LINENGY.OUT not written to tmp_path"
 
     linengy = parse_linengy(file.as_posix())
 
-    assert linengy['0']['apw'] == linengy_ref['0']['apw'], "First species apw data consistent"
-    assert linengy['0']['lo'] == linengy_ref['0']['lo'], "First species lo data consistent"
-    assert linengy['1']['apw'] == linengy_ref['1']['apw'], "Second species apw data consistent"
-    assert linengy['1']['lo'] == linengy_ref['1']['lo'], "Second species lo data consistent"
+    assert linengy["0"]["apw"] == linengy_ref["0"]["apw"], "First species apw data consistent"
+    assert linengy["0"]["lo"] == linengy_ref["0"]["lo"], "First species lo data consistent"
+    assert linengy["1"]["apw"] == linengy_ref["1"]["apw"], "Second species apw data consistent"
+    assert linengy["1"]["lo"] == linengy_ref["1"]["lo"], "Second species lo data consistent"
 
 
 GGA_PBE_SOL_automatic_trial_energies_NaCl_LINENGY_OUT = """Species :    1 (Na), atom :    1
  APW functions :
   l =  0, order =  1 :   -2.100000000    
   l =  1, order =  1 :   -1.100000000    
   l =  2, order =  1 :   0.1500000000    
@@ -981,136 +939,216 @@
       * the parser keys change
       * the structure of the output changes
     """
 
     # Reference of the dictionary parsed with parse_lo_recommendation
     # Generated with print(json.dumps(info_out, sort_keys=True, indent=4))
 
-    lo_recommendation_ref = {'n_species': 2, 'n_l_channels': 4, 'n_nodes': 21,
-                             'Na': {0: [[0.0, 1.0, -37.65990706181], [1.0, 2.0, -1.796282469826],
-                                        [2.0, 3.0, 1.821425619362],
-                                        [3.0, 4.0, 7.892575399809], [4.0, 5.0, 16.986165613637],
-                                        [5.0, 6.0, 28.846080585981],
-                                        [6.0, 7.0, 43.369227333017], [7.0, 8.0, 60.495491296112],
-                                        [8.0, 9.0, 80.187724549122],
-                                        [9.0, 10.0, 102.422176950914], [10.0, 11.0, 127.182990712735],
-                                        [11.0, 12.0, 154.458866712915],
-                                        [12.0, 13.0, 184.241158329361], [13.0, 14.0, 216.522955263927],
-                                        [14.0, 15.0, 251.298756937161],
-                                        [15.0, 16.0, 288.564346156074], [16.0, 17.0, 328.316602395923],
-                                        [17.0, 18.0, 370.553203330272],
-                                        [18.0, 19.0, 415.272297641907], [19.0, 20.0, 462.472263422762],
-                                        [20.0, 21.0, 512.15160534914]],
-                                    1: [[0.0, 2.0, -0.764380938525], [1.0, 3.0, 2.150459202106],
-                                        [2.0, 4.0, 7.68064315441],
-                                        [3.0, 5.0, 15.944823175319], [4.0, 6.0, 26.826688781275],
-                                        [5.0, 7.0, 40.283086869083],
-                                        [6.0, 8.0, 56.289616891011], [7.0, 9.0, 74.830023777453],
-                                        [8.0, 10.0, 95.891983053944],
-                                        [9.0, 11.0, 119.465424264199], [10.0, 12.0, 145.542112894232],
-                                        [11.0, 13.0, 174.115704751485],
-                                        [12.0, 14.0, 205.181692970898], [13.0, 15.0, 238.737011824859],
-                                        [14.0, 16.0, 274.779422707574],
-                                        [15.0, 17.0, 313.306969990248], [16.0, 18.0, 354.317721540693],
-                                        [17.0, 19.0, 397.809787603557],
-                                        [18.0, 20.0, 443.781471675578], [19.0, 21.0, 492.231385973938],
-                                        [20.0, 22.0, 543.158450851233]],
-                                    2: [[0.0, 3.0, 2.044659668292], [1.0, 4.0, 6.427853785834],
-                                        [2.0, 5.0, 13.431600603035],
-                                        [3.0, 6.0, 23.065707720667], [4.0, 7.0, 35.286723443086],
-                                        [5.0, 8.0, 50.060639647089],
-                                        [6.0, 9.0, 67.365856793742], [7.0, 10.0, 87.18903211822],
-                                        [8.0, 11.0, 109.521849753452],
-                                        [9.0, 12.0, 134.358761651081], [10.0, 13.0, 161.695405680071],
-                                        [11.0, 14.0, 191.52770328581],
-                                        [12.0, 15.0, 223.85164087452], [13.0, 16.0, 258.663517453378],
-                                        [14.0, 17.0, 295.960290921283],
-                                        [15.0, 18.0, 335.73972677672], [16.0, 19.0, 378.000263814603],
-                                        [17.0, 20.0, 422.740724390955],
-                                        [18.0, 21.0, 469.960046963641], [19.0, 22.0, 519.657164852307],
-                                        [20.0, 23.0, 571.831020081621]],
-                                    3: [[0.0, 4.0, 3.879401688185], [1.0, 5.0, 9.964477889618],
-                                        [2.0, 6.0, 18.47378344193],
-                                        [3.0, 7.0, 29.505302500625], [4.0, 8.0, 43.071695950394],
-                                        [5.0, 9.0, 59.165686791534],
-                                        [6.0, 10.0, 77.776580159806], [7.0, 11.0, 98.89485358398],
-                                        [8.0, 12.0, 122.513132271493],
-                                        [9.0, 13.0, 148.626189112094], [10.0, 14.0, 177.230592656783],
-                                        [11.0, 15.0, 208.324116670413],
-                                        [12.0, 16.0, 241.905061644769], [13.0, 17.0, 277.971722458938],
-                                        [14.0, 18.0, 316.522185899964],
-                                        [15.0, 19.0, 357.554436071786], [16.0, 20.0, 401.066608041866],
-                                        [17.0, 21.0, 447.057187991954],
-                                        [18.0, 22.0, 495.525055433203], [19.0, 23.0, 546.469383913223],
-                                        [20.0, 24.0, 599.889489594382]]},
-                             'Cl': {0: [[0.0, 1.0, -100.974592263771], [1.0, 2.0, -8.943406336517],
-                                        [2.0, 3.0, 0.803820215121],
-                                        [3.0, 4.0, 11.265670674793], [4.0, 5.0, 27.995235804499],
-                                        [5.0, 6.0, 50.139499480779],
-                                        [6.0, 7.0, 77.425670325936], [7.0, 8.0, 109.722811813338],
-                                        [8.0, 9.0, 146.943417860813],
-                                        [9.0, 10.0, 189.030459361669], [10.0, 11.0, 235.945624307269],
-                                        [11.0, 12.0, 287.660637659017],
-                                        [12.0, 13.0, 344.155876726629], [13.0, 14.0, 405.415989381911],
-                                        [14.0, 15.0, 471.42935525429],
-                                        [15.0, 16.0, 542.186581729314], [16.0, 17.0, 617.680068606306],
-                                        [17.0, 18.0, 697.90359882698],
-                                        [18.0, 19.0, 782.852080659573], [19.0, 20.0, 872.521357718829],
-                                        [20.0, 21.0, 966.908013775037]],
-                                    1: [[0.0, 2.0, -6.707821362791], [1.0, 3.0, 1.442002863349],
-                                        [2.0, 4.0, 11.086329356142],
-                                        [3.0, 5.0, 26.446761118127], [4.0, 6.0, 46.908960145565],
-                                        [5.0, 7.0, 72.31449630133],
-                                        [6.0, 8.0, 102.593748915541], [7.0, 9.0, 137.708872214526],
-                                        [8.0, 10.0, 177.628868217528],
-                                        [9.0, 11.0, 222.335815545055], [10.0, 12.0, 271.812774967963],
-                                        [11.0, 13.0, 326.047911895729],
-                                        [12.0, 14.0, 385.030908226461], [13.0, 15.0, 448.753672165588],
-                                        [14.0, 16.0, 517.209705744261],
-                                        [15.0, 17.0, 590.393819776316], [16.0, 18.0, 668.301879780751],
-                                        [17.0, 19.0, 750.930453348811],
-                                        [18.0, 20.0, 838.276595190814], [19.0, 21.0, 930.337672332757],
-                                        [20.0, 22.0, 1027.111295649087]],
-                                    2: [[0.0, 3.0, 2.030626399034], [1.0, 4.0, 9.540398069814],
-                                        [2.0, 5.0, 22.521806870793],
-                                        [3.0, 6.0, 40.580505794574], [4.0, 7.0, 63.608967480673],
-                                        [5.0, 8.0, 91.521851721479],
-                                        [6.0, 9.0, 124.28110055295], [7.0, 10.0, 161.847878698612],
-                                        [8.0, 11.0, 204.202486065259],
-                                        [9.0, 12.0, 251.327905737439], [10.0, 13.0, 303.212514505293],
-                                        [11.0, 14.0, 359.847427715492],
-                                        [12.0, 15.0, 421.225227525549], [13.0, 16.0, 487.339835071361],
-                                        [14.0, 17.0, 558.185801503932],
-                                        [15.0, 18.0, 633.758349847869], [16.0, 19.0, 714.053292909356],
-                                        [17.0, 20.0, 799.067051302979],
-                                        [18.0, 21.0, 888.796639877965], [19.0, 22.0, 983.239587157865],
-                                        [20.0, 23.0, 1082.393826570133]],
-                                    3: [[0.0, 4.0, 5.877668530234], [1.0, 5.0, 16.734445897029],
-                                        [2.0, 6.0, 32.521343858776],
-                                        [3.0, 7.0, 53.248636736501], [4.0, 8.0, 78.839760672149],
-                                        [5.0, 9.0, 109.265751512702],
-                                        [6.0, 10.0, 144.502223464379], [7.0, 11.0, 184.526132806013],
-                                        [8.0, 12.0, 229.322756357998],
-                                        [9.0, 13.0, 278.877755682806], [10.0, 14.0, 333.181582371119],
-                                        [11.0, 15.0, 392.226089160902],
-                                        [12.0, 16.0, 456.00524371215], [13.0, 17.0, 524.514261786364],
-                                        [14.0, 18.0, 597.749258861014],
-                                        [15.0, 19.0, 675.706956131225], [16.0, 20.0, 758.384407267418],
-                                        [17.0, 21.0, 845.778892453188],
-                                        [18.0, 22.0, 937.887883257667], [19.0, 23.0, 1034.709065214155],
-                                        [20.0, 24.0, 1136.240377687629]]}}
+    lo_recommendation_ref = {
+        "n_species": 2,
+        "n_l_channels": 4,
+        "n_nodes": 21,
+        "Na": {
+            0: [
+                [0.0, 1.0, -37.65990706181],
+                [1.0, 2.0, -1.796282469826],
+                [2.0, 3.0, 1.821425619362],
+                [3.0, 4.0, 7.892575399809],
+                [4.0, 5.0, 16.986165613637],
+                [5.0, 6.0, 28.846080585981],
+                [6.0, 7.0, 43.369227333017],
+                [7.0, 8.0, 60.495491296112],
+                [8.0, 9.0, 80.187724549122],
+                [9.0, 10.0, 102.422176950914],
+                [10.0, 11.0, 127.182990712735],
+                [11.0, 12.0, 154.458866712915],
+                [12.0, 13.0, 184.241158329361],
+                [13.0, 14.0, 216.522955263927],
+                [14.0, 15.0, 251.298756937161],
+                [15.0, 16.0, 288.564346156074],
+                [16.0, 17.0, 328.316602395923],
+                [17.0, 18.0, 370.553203330272],
+                [18.0, 19.0, 415.272297641907],
+                [19.0, 20.0, 462.472263422762],
+                [20.0, 21.0, 512.15160534914],
+            ],
+            1: [
+                [0.0, 2.0, -0.764380938525],
+                [1.0, 3.0, 2.150459202106],
+                [2.0, 4.0, 7.68064315441],
+                [3.0, 5.0, 15.944823175319],
+                [4.0, 6.0, 26.826688781275],
+                [5.0, 7.0, 40.283086869083],
+                [6.0, 8.0, 56.289616891011],
+                [7.0, 9.0, 74.830023777453],
+                [8.0, 10.0, 95.891983053944],
+                [9.0, 11.0, 119.465424264199],
+                [10.0, 12.0, 145.542112894232],
+                [11.0, 13.0, 174.115704751485],
+                [12.0, 14.0, 205.181692970898],
+                [13.0, 15.0, 238.737011824859],
+                [14.0, 16.0, 274.779422707574],
+                [15.0, 17.0, 313.306969990248],
+                [16.0, 18.0, 354.317721540693],
+                [17.0, 19.0, 397.809787603557],
+                [18.0, 20.0, 443.781471675578],
+                [19.0, 21.0, 492.231385973938],
+                [20.0, 22.0, 543.158450851233],
+            ],
+            2: [
+                [0.0, 3.0, 2.044659668292],
+                [1.0, 4.0, 6.427853785834],
+                [2.0, 5.0, 13.431600603035],
+                [3.0, 6.0, 23.065707720667],
+                [4.0, 7.0, 35.286723443086],
+                [5.0, 8.0, 50.060639647089],
+                [6.0, 9.0, 67.365856793742],
+                [7.0, 10.0, 87.18903211822],
+                [8.0, 11.0, 109.521849753452],
+                [9.0, 12.0, 134.358761651081],
+                [10.0, 13.0, 161.695405680071],
+                [11.0, 14.0, 191.52770328581],
+                [12.0, 15.0, 223.85164087452],
+                [13.0, 16.0, 258.663517453378],
+                [14.0, 17.0, 295.960290921283],
+                [15.0, 18.0, 335.73972677672],
+                [16.0, 19.0, 378.000263814603],
+                [17.0, 20.0, 422.740724390955],
+                [18.0, 21.0, 469.960046963641],
+                [19.0, 22.0, 519.657164852307],
+                [20.0, 23.0, 571.831020081621],
+            ],
+            3: [
+                [0.0, 4.0, 3.879401688185],
+                [1.0, 5.0, 9.964477889618],
+                [2.0, 6.0, 18.47378344193],
+                [3.0, 7.0, 29.505302500625],
+                [4.0, 8.0, 43.071695950394],
+                [5.0, 9.0, 59.165686791534],
+                [6.0, 10.0, 77.776580159806],
+                [7.0, 11.0, 98.89485358398],
+                [8.0, 12.0, 122.513132271493],
+                [9.0, 13.0, 148.626189112094],
+                [10.0, 14.0, 177.230592656783],
+                [11.0, 15.0, 208.324116670413],
+                [12.0, 16.0, 241.905061644769],
+                [13.0, 17.0, 277.971722458938],
+                [14.0, 18.0, 316.522185899964],
+                [15.0, 19.0, 357.554436071786],
+                [16.0, 20.0, 401.066608041866],
+                [17.0, 21.0, 447.057187991954],
+                [18.0, 22.0, 495.525055433203],
+                [19.0, 23.0, 546.469383913223],
+                [20.0, 24.0, 599.889489594382],
+            ],
+        },
+        "Cl": {
+            0: [
+                [0.0, 1.0, -100.974592263771],
+                [1.0, 2.0, -8.943406336517],
+                [2.0, 3.0, 0.803820215121],
+                [3.0, 4.0, 11.265670674793],
+                [4.0, 5.0, 27.995235804499],
+                [5.0, 6.0, 50.139499480779],
+                [6.0, 7.0, 77.425670325936],
+                [7.0, 8.0, 109.722811813338],
+                [8.0, 9.0, 146.943417860813],
+                [9.0, 10.0, 189.030459361669],
+                [10.0, 11.0, 235.945624307269],
+                [11.0, 12.0, 287.660637659017],
+                [12.0, 13.0, 344.155876726629],
+                [13.0, 14.0, 405.415989381911],
+                [14.0, 15.0, 471.42935525429],
+                [15.0, 16.0, 542.186581729314],
+                [16.0, 17.0, 617.680068606306],
+                [17.0, 18.0, 697.90359882698],
+                [18.0, 19.0, 782.852080659573],
+                [19.0, 20.0, 872.521357718829],
+                [20.0, 21.0, 966.908013775037],
+            ],
+            1: [
+                [0.0, 2.0, -6.707821362791],
+                [1.0, 3.0, 1.442002863349],
+                [2.0, 4.0, 11.086329356142],
+                [3.0, 5.0, 26.446761118127],
+                [4.0, 6.0, 46.908960145565],
+                [5.0, 7.0, 72.31449630133],
+                [6.0, 8.0, 102.593748915541],
+                [7.0, 9.0, 137.708872214526],
+                [8.0, 10.0, 177.628868217528],
+                [9.0, 11.0, 222.335815545055],
+                [10.0, 12.0, 271.812774967963],
+                [11.0, 13.0, 326.047911895729],
+                [12.0, 14.0, 385.030908226461],
+                [13.0, 15.0, 448.753672165588],
+                [14.0, 16.0, 517.209705744261],
+                [15.0, 17.0, 590.393819776316],
+                [16.0, 18.0, 668.301879780751],
+                [17.0, 19.0, 750.930453348811],
+                [18.0, 20.0, 838.276595190814],
+                [19.0, 21.0, 930.337672332757],
+                [20.0, 22.0, 1027.111295649087],
+            ],
+            2: [
+                [0.0, 3.0, 2.030626399034],
+                [1.0, 4.0, 9.540398069814],
+                [2.0, 5.0, 22.521806870793],
+                [3.0, 6.0, 40.580505794574],
+                [4.0, 7.0, 63.608967480673],
+                [5.0, 8.0, 91.521851721479],
+                [6.0, 9.0, 124.28110055295],
+                [7.0, 10.0, 161.847878698612],
+                [8.0, 11.0, 204.202486065259],
+                [9.0, 12.0, 251.327905737439],
+                [10.0, 13.0, 303.212514505293],
+                [11.0, 14.0, 359.847427715492],
+                [12.0, 15.0, 421.225227525549],
+                [13.0, 16.0, 487.339835071361],
+                [14.0, 17.0, 558.185801503932],
+                [15.0, 18.0, 633.758349847869],
+                [16.0, 19.0, 714.053292909356],
+                [17.0, 20.0, 799.067051302979],
+                [18.0, 21.0, 888.796639877965],
+                [19.0, 22.0, 983.239587157865],
+                [20.0, 23.0, 1082.393826570133],
+            ],
+            3: [
+                [0.0, 4.0, 5.877668530234],
+                [1.0, 5.0, 16.734445897029],
+                [2.0, 6.0, 32.521343858776],
+                [3.0, 7.0, 53.248636736501],
+                [4.0, 8.0, 78.839760672149],
+                [5.0, 9.0, 109.265751512702],
+                [6.0, 10.0, 144.502223464379],
+                [7.0, 11.0, 184.526132806013],
+                [8.0, 12.0, 229.322756357998],
+                [9.0, 13.0, 278.877755682806],
+                [10.0, 14.0, 333.181582371119],
+                [11.0, 15.0, 392.226089160902],
+                [12.0, 16.0, 456.00524371215],
+                [13.0, 17.0, 524.514261786364],
+                [14.0, 18.0, 597.749258861014],
+                [15.0, 19.0, 675.706956131225],
+                [16.0, 20.0, 758.384407267418],
+                [17.0, 21.0, 845.778892453188],
+                [18.0, 22.0, 937.887883257667],
+                [19.0, 23.0, 1034.709065214155],
+                [20.0, 24.0, 1136.240377687629],
+            ],
+        },
+    }
 
-    file = tmp_path / 'LO_RECOMMENDATION.OUT'
+    file = tmp_path / "LO_RECOMMENDATION.OUT"
     file.write_text(GGA_PBE_SOL_automatic_trial_energies_NaCl_LO_RECOMMENDATION_OUT)
     assert file.exists(), "LO_RECOMMENDATION.OUT not written to tmp_path"
 
     lo_recommendation = parse_lo_recommendation(file.as_posix())
 
-    assert lo_recommendation['Na'] == lo_recommendation_ref['Na'], "First species data consistent"
-    assert lo_recommendation['Cl'] == lo_recommendation_ref['Cl'], "Second species data consistent"
+    assert lo_recommendation["Na"] == lo_recommendation_ref["Na"], "First species data consistent"
+    assert lo_recommendation["Cl"] == lo_recommendation_ref["Cl"], "Second species data consistent"
 
 
 GGA_PBE_SOL_automatic_trial_energies_NaCl_LO_RECOMMENDATION_OUT = """# Recommended linearization energies computet with Wigner-Seitz rules.
  --------------------------------------------------------------------
  #  n_species:  2
  # n_l-channels:  4
  # n_nodes: 21
```

### Comparing `excitingtools-1.7.0/tests/dict_parsers/test_gw/mock_gw_info_out.py` & `excitingtools-1.7.1/tests/dict_parsers/test_gw/mock_gw_info_out.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,8 @@
-"""Outputs from GW_INFO.OUT
-"""
-import pytest
-from excitingtools.utils.test_utils import MockFile
-
-from excitingtools.exciting_dict_parsers.gw_info_parser import _file_name
-
-
-@pytest.fixture
-def zro2_gw_info_out_mock(tmp_path):
-    file = tmp_path / _file_name
-    file.write_text(zro2_gw_info_out)
-    return MockFile(file, zro2_gw_info_out)
-
-
-@pytest.fixture
-def si_2_gw_info_out_mock(tmp_path):
-    file = tmp_path / _file_name
-    file.write_text(si_2_gw_info_out)
-    return MockFile(file, si_2_gw_info_out)
-
+"""Outputs from GW_INFO.OUT"""
 
 # GW output for ZrO2. This reports an indirect gap, as well as its direct gap
 zro2_gw_info_out = """
 ================================================================================
 =                            GW input parameters                               =
 ================================================================================
 
@@ -414,8 +394,7 @@
      - calcselfx                            :         0.04
      - calcselfc                            :         2.00
      - calcvxcnn                            :         0.11
      - input/output                         :         0.00
  _________________________________________________________
  Total                                      :         4.25
 """
-
```

### Comparing `excitingtools-1.7.0/tests/dict_parsers/test_gw/test_gw_dos_parser.py` & `excitingtools-1.7.1/tests/obj_parsers/test_gw_dos.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """
-Test gw DOS parser.
+Test gw DOS parser, returning to an object.
 Execute tests from exciting_tools directory:
 pytest --capture=tee-sys
 """
 
+import numpy as np
 import pytest
+
+from excitingtools.exciting_obj_parsers.gw_eigenvalues import parse_obj_gw_dos
 from excitingtools.utils.test_utils import MockFile
-from excitingtools.exciting_dict_parsers.gw_eigenvalues_parser import parse_gw_dos
-import numpy as np
+
 
 @pytest.fixture
 def gw_dos_mock(tmp_path) -> MockFile:
-    """ Mock TDOS.OUT data for 15 energy and DOS value pairs
-    """
+    """Mock TDOS.OUT data for 15 energy and DOS value pairs"""
     dos_str = """-0.5000000000  0.000000000
     -0.4949748744  0.000000000
     -0.4899497487  0.000000000
     -0.4849246231  0.000000000
     -0.4798994975  0.000000000
     -0.4748743719  0.000000000
     -0.4698492462  0.000000000
@@ -30,22 +31,52 @@
     -0.4296482412  1.164919267
     """
     dos_file = tmp_path / "TDOS.OUT"
     dos_file.write_text(dos_str)
     return MockFile(dos_file, dos_str)
 
 
-def test_parse_gw_dos(gw_dos_mock):
-    """ Test parsing of energy and DOS values from TDOS.OUT
-    """
-    data = parse_gw_dos(gw_dos_mock.file)
+def test_parse_obj_gw_dos(gw_dos_mock):
+    """Test that the parser correctly returns to the DOS object."""
+    data = parse_obj_gw_dos(gw_dos_mock.file)
+
+    ref_energies = np.array(
+        [
+            -0.5000000000,
+            -0.4949748744,
+            -0.4899497487,
+            -0.4849246231,
+            -0.4798994975,
+            -0.4748743719,
+            -0.4698492462,
+            -0.4648241206,
+            -0.4597989950,
+            -0.4547738693,
+            -0.4497487437,
+            -0.4447236181,
+            -0.4396984925,
+            -0.4346733668,
+            -0.4296482412,
+        ]
+    )
+    ref_dos = np.array(
+        [
+            0.000000000,
+            0.000000000,
+            0.000000000,
+            0.000000000,
+            0.000000000,
+            0.000000000,
+            0.000000000,
+            0.000000000,
+            0.000000000,
+            0.000000000,
+            0.1025457101e-01,
+            0.1050068072,
+            0.3502961458,
+            0.6899275378,
+            1.164919267,
+        ]
+    )
 
-    ref_energies = np.array([-0.5000000000, -0.4949748744, -0.4899497487, -0.4849246231, -0.4798994975, -0.4748743719,
-                             -0.4698492462, -0.4648241206, -0.4597989950, -0.4547738693, -0.4497487437, -0.4447236181,
-                             -0.4396984925, -0.4346733668, -0.4296482412])
-    ref_dos = np.array([0.000000000, 0.000000000, 0.000000000, 0.000000000, 0.000000000, 0.000000000,
-                        0.000000000, 0.000000000, 0.000000000, 0.000000000, 0.1025457101E-01, 0.1050068072, 0.3502961458,
-                        0.6899275378, 1.164919267])
-
-    assert set(data) == {'energy', 'dos'}
-    assert np.allclose(data['energy'], ref_energies)
-    assert np.allclose(data['dos'], ref_dos)
+    assert np.allclose(data.energy, ref_energies)
+    assert np.allclose(data.dos, ref_dos)
```

### Comparing `excitingtools-1.7.0/tests/dict_parsers/test_gw/test_gw_eignvalues_parser.py` & `excitingtools-1.7.1/tests/dict_parsers/test_gw/test_gw_eignvalues_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-import pytest
 import numpy as np
-
-from excitingtools.utils.test_utils import MockFile
+import pytest
 
 from excitingtools.dataclasses.data_structs import NumberOfStates
-from excitingtools.exciting_dict_parsers.gw_eigenvalues_parser import k_points_from_evalqp, n_states_from_evalqp, \
-    parse_column_labels, parse_evalqp
+from excitingtools.exciting_dict_parsers.gw_eigenvalues_parser import (
+    k_points_from_evalqp,
+    n_states_from_evalqp,
+    parse_column_labels,
+    parse_evalqp,
+)
+from excitingtools.utils.test_utils import MockFile
 
 
 @pytest.fixture
 def evalqp_mock(tmp_path):
-    """ Mock EVALQP.OUT data with energies for 3 k-points, and corrections starting from the first state
-    """
+    """Mock EVALQP.OUT data with energies for 3 k-points, and corrections starting from the first state"""
     evalqp_str = """k-point #     1:    0.000000    0.000000    0.000000    0.125000
 state   E_KS       E_HF       E_GW       Sx         Re(Sc)     Im(Sc)     Vxc        DE_HF      DE_GW      Znk
   1   -14.68627  -16.50308  -16.31014   -4.72516    0.17351    0.00002   -2.90835   -1.81681   -1.62387    0.98817
   2   -11.48914  -12.99338  -12.79204   -4.36834    0.18150    0.00003   -2.86410   -1.50424   -1.30290    0.98500
   3   -11.48914  -12.99338  -12.79204   -4.36834    0.18150    0.00003   -2.86410   -1.50424   -1.30290    0.98500
   4   -11.48914  -12.99338  -12.79203   -4.36834    0.18151    0.00003   -2.86410   -1.50424   -1.30289    0.98500
   5    -6.24399   -7.20716   -7.01655   -3.72742    0.17144    0.00000   -2.76425   -0.96317   -0.77257    0.97579
@@ -58,15 +60,15 @@
     evalqp_file = tmp_path / "EVALQP.DAT"
     evalqp_file.write_text(evalqp_str)
     return MockFile(evalqp_file, evalqp_str)
 
 
 @pytest.fixture
 def evalqp_mock_partial_corrections(tmp_path):
-    """ Mock EVALQP.OUT data with energies for 3 k-points, BUT corrections starting from NOT the
+    """Mock EVALQP.OUT data with energies for 3 k-points, BUT corrections starting from NOT the
     first state.
     """
     evalqp_str = """k-point #     1:    0.000000    0.000000    0.000000    0.015625
  state    E_KS      E_HF       E_GW       Sx         Sc         Vxc         DE_HF        DE_GW       Znk
    5    -3.10465   -3.86125   -3.66015   -2.47956    0.35377   -1.72297   -0.75660   -0.55550    0.87583
    6    -3.10403   -3.86057   -3.64943   -2.48053    0.36134   -1.72399   -0.75654   -0.54540    0.86720
    7    -3.10403   -3.86057   -3.65031   -2.48053    0.36104   -1.72399   -0.75654   -0.54628    0.86875
@@ -88,29 +90,27 @@
     """
     evalqp_file = tmp_path / "EVALQP.DAT"
     evalqp_file.write_text(evalqp_str)
     return MockFile(evalqp_file, evalqp_str)
 
 
 def test_k_points_from_evalqp(evalqp_mock):
-    """ Test parsing of EVALQP.DAT
-    """
+    """Test parsing of EVALQP.DAT"""
     ref = {
-        1: {'k_point': [0.000000, 0.000000, 0.000000], 'weight': 0.125000},
-        2: {'k_point': [0.000000, 0.000000, 0.500000], 'weight': 0.500000},
-        3: {'k_point': [0.000000, 0.500000, 0.500000], 'weight': 0.375000}
+        1: {"k_point": [0.000000, 0.000000, 0.000000], "weight": 0.125000},
+        2: {"k_point": [0.000000, 0.000000, 0.500000], "weight": 0.500000},
+        3: {"k_point": [0.000000, 0.500000, 0.500000], "weight": 0.375000},
     }
 
     k_points_and_weights = k_points_from_evalqp(evalqp_mock.string)
     assert k_points_and_weights == ref, "k_points_and_weights should match reference"
 
 
-def test_n_states_from_evalqp_one_kpoint(evalqp_mock):
-    """ Test parsing of EVALQP.DAT
-    """
+def test_n_states_from_evalqp_one_kpoint():
+    """Test parsing of EVALQP.DAT"""
     evalqp_str_with_one_kpoint = """k-point #     1:    0.000000    0.000000    0.000000    0.125000
  state   E_KS       E_HF       E_GW       Sx         Re(Sc)     Im(Sc)     Vxc        DE_HF      DE_GW      Znk
    1   -14.68627  -16.50308  -16.31014   -4.72516    0.17351    0.00002   -2.90835   -1.81681   -1.62387    0.98817
    2   -11.48914  -12.99338  -12.79204   -4.36834    0.18150    0.00003   -2.86410   -1.50424   -1.30290    0.98500
    3   -11.48914  -12.99338  -12.79204   -4.36834    0.18150    0.00003   -2.86410   -1.50424   -1.30290    0.98500
    4   -11.48914  -12.99338  -12.79203   -4.36834    0.18151    0.00003   -2.86410   -1.50424   -1.30289    0.98500
    5    -6.24399   -7.20716   -7.01655   -3.72742    0.17144    0.00000   -2.76425   -0.96317   -0.77257    0.97579
@@ -138,96 +138,126 @@
     assert gw.first_state == 5, "GW corrections should start at state 5"
     assert gw.last_state == 8, "GW corrections should start at state 8"
     assert gw.n_states == 4, "Each k-point should have 4 states"
 
 
 def test_parse_column_labels_for_oxygen(evalqp_mock):
     column_labels = parse_column_labels(evalqp_mock.string)
-    assert column_labels._member_names_ == ['E_KS', 'E_HF', 'E_GW', 'Sx',
-                                            'Re(Sc)', 'Im(Sc)', 'Vxc', 'DE_HF', 'DE_GW', 'Znk']
+    assert column_labels._member_names_ == [
+        "E_KS",
+        "E_HF",
+        "E_GW",
+        "Sx",
+        "Re(Sc)",
+        "Im(Sc)",
+        "Vxc",
+        "DE_HF",
+        "DE_GW",
+        "Znk",
+    ]
     assert column_labels.E_KS.value == 0, "Expect first label value to start at 0"
 
 
 def test_parse_column_labels_for_nitrogen(evalqp_mock):
     column_labels = parse_column_labels(evalqp_mock.string)
-    assert column_labels._member_names_ == ['E_KS', 'E_HF', 'E_GW', 'Sx',
-                                            'Re(Sc)', 'Im(Sc)', 'Vxc', 'DE_HF', 'DE_GW', 'Znk']
+    assert column_labels._member_names_ == [
+        "E_KS",
+        "E_HF",
+        "E_GW",
+        "Sx",
+        "Re(Sc)",
+        "Im(Sc)",
+        "Vxc",
+        "DE_HF",
+        "DE_GW",
+        "Znk",
+    ]
     assert column_labels.E_KS.value == 0, "Expect first label value to start at 0"
 
 
 def test_parse_evalqp(evalqp_mock):
-    """ Test parsing eigenvalues and weights from EVALQP.DAT.
-    """
+    """Test parsing eigenvalues and weights from EVALQP.DAT."""
 
     # Energies for all states, per k-point
     energies_1 = np.array(
-        [[-14.68627, -16.50308, -16.31014, -4.72516, 0.17351, 0.00002, -2.90835, -1.81681, -1.62387, 0.98817],
-         [-11.48914, -12.99338, -12.79204, -4.36834, 0.18150, 0.00003, -2.86410, -1.50424, -1.30290, 0.98500],
-         [-11.48914, -12.99338, -12.79204, -4.36834, 0.18150, 0.00003, -2.86410, -1.50424, -1.30290, 0.98500],
-         [-11.48914, -12.99338, -12.79203, -4.36834, 0.18151, 0.00003, -2.86410, -1.50424, -1.30289, 0.98500],
-         [-6.24399, -7.20716, -7.01655, -3.72742, 0.17144, 0.00000, -2.76425, -0.96317, -0.77257, 0.97579],
-         [-6.24399, -7.20716, -7.01652, -3.72742, 0.17144, -0.00001, -2.76425, -0.96317, -0.77253, 0.97575],
-         [-6.24340, -7.20928, -7.01752, -3.73069, 0.17268, 0.00003, -2.76481, -0.96588, -0.77412, 0.97594],
-         [-6.24340, -7.20928, -7.01752, -3.73069, 0.17268, 0.00003, -2.76481, -0.96588, -0.77412, 0.97594],
-         [-6.24340, -7.20928, -7.01752, -3.73069, 0.17268, 0.00003, -2.76481, -0.96588, -0.77412, 0.97594],
-         [-1.82156, -2.31023, -2.07248, -1.52298, 0.20180, 0.00623, -1.03431, -0.48867, -0.25092, 0.87468],
-         [-1.00771, -1.29282, -1.07701, -1.21488, 0.19790, 0.02221, -0.92977, -0.28511, -0.06930, 0.79459]]
-        )
+        [
+            [-14.68627, -16.50308, -16.31014, -4.72516, 0.17351, 0.00002, -2.90835, -1.81681, -1.62387, 0.98817],
+            [-11.48914, -12.99338, -12.79204, -4.36834, 0.18150, 0.00003, -2.86410, -1.50424, -1.30290, 0.98500],
+            [-11.48914, -12.99338, -12.79204, -4.36834, 0.18150, 0.00003, -2.86410, -1.50424, -1.30290, 0.98500],
+            [-11.48914, -12.99338, -12.79203, -4.36834, 0.18151, 0.00003, -2.86410, -1.50424, -1.30289, 0.98500],
+            [-6.24399, -7.20716, -7.01655, -3.72742, 0.17144, 0.00000, -2.76425, -0.96317, -0.77257, 0.97579],
+            [-6.24399, -7.20716, -7.01652, -3.72742, 0.17144, -0.00001, -2.76425, -0.96317, -0.77253, 0.97575],
+            [-6.24340, -7.20928, -7.01752, -3.73069, 0.17268, 0.00003, -2.76481, -0.96588, -0.77412, 0.97594],
+            [-6.24340, -7.20928, -7.01752, -3.73069, 0.17268, 0.00003, -2.76481, -0.96588, -0.77412, 0.97594],
+            [-6.24340, -7.20928, -7.01752, -3.73069, 0.17268, 0.00003, -2.76481, -0.96588, -0.77412, 0.97594],
+            [-1.82156, -2.31023, -2.07248, -1.52298, 0.20180, 0.00623, -1.03431, -0.48867, -0.25092, 0.87468],
+            [-1.00771, -1.29282, -1.07701, -1.21488, 0.19790, 0.02221, -0.92977, -0.28511, -0.06930, 0.79459],
+        ]
+    )
 
     energies_2 = np.array(
-        [[-14.68627, -16.50308, -16.31014, -4.72516, 0.17351, 0.00002, -2.90835, -1.81681, -1.62387, 0.98817],
-         [-11.48915, -12.99338, -12.79204, -4.36834, 0.18150, 0.00003, -2.86410, -1.50424, -1.30289, 0.98500],
-         [-11.48915, -12.99338, -12.79204, -4.36834, 0.18151, 0.00003, -2.86410, -1.50424, -1.30289, 0.98500],
-         [-11.48914, -12.99338, -12.79204, -4.36834, 0.18150, 0.00003, -2.86410, -1.50424, -1.30290, 0.98500],
-         [-6.24401, -7.20719, -7.01653, -3.72740, 0.17145, -0.00001, -2.76423, -0.96318, -0.77252, 0.97574],
-         [-6.24401, -7.20719, -7.01650, -3.72740, 0.17145, -0.00001, -2.76423, -0.96318, -0.77249, 0.97570],
-         [-6.24345, -7.20933, -7.01756, -3.73065, 0.17268, 0.00003, -2.76477, -0.96588, -0.77411, 0.97593],
-         [-6.24344, -7.20932, -7.01754, -3.73066, 0.17268, 0.00003, -2.76478, -0.96588, -0.77410, 0.97593],
-         [-6.24344, -7.20932, -7.01755, -3.73066, 0.17268, 0.00003, -2.76478, -0.96588, -0.77411, 0.97593],
-         [-1.81969, -2.30723, -2.07258, -1.52476, 0.20051, 0.00867, -1.03723, -0.48754, -0.25289, 0.88104],
-         [-1.03473, -1.34882, -1.09998, -1.20344, 0.22865, 0.02686, -0.88936, -0.31408, -0.06525, 0.76380]]
+        [
+            [-14.68627, -16.50308, -16.31014, -4.72516, 0.17351, 0.00002, -2.90835, -1.81681, -1.62387, 0.98817],
+            [-11.48915, -12.99338, -12.79204, -4.36834, 0.18150, 0.00003, -2.86410, -1.50424, -1.30289, 0.98500],
+            [-11.48915, -12.99338, -12.79204, -4.36834, 0.18151, 0.00003, -2.86410, -1.50424, -1.30289, 0.98500],
+            [-11.48914, -12.99338, -12.79204, -4.36834, 0.18150, 0.00003, -2.86410, -1.50424, -1.30290, 0.98500],
+            [-6.24401, -7.20719, -7.01653, -3.72740, 0.17145, -0.00001, -2.76423, -0.96318, -0.77252, 0.97574],
+            [-6.24401, -7.20719, -7.01650, -3.72740, 0.17145, -0.00001, -2.76423, -0.96318, -0.77249, 0.97570],
+            [-6.24345, -7.20933, -7.01756, -3.73065, 0.17268, 0.00003, -2.76477, -0.96588, -0.77411, 0.97593],
+            [-6.24344, -7.20932, -7.01754, -3.73066, 0.17268, 0.00003, -2.76478, -0.96588, -0.77410, 0.97593],
+            [-6.24344, -7.20932, -7.01755, -3.73066, 0.17268, 0.00003, -2.76478, -0.96588, -0.77411, 0.97593],
+            [-1.81969, -2.30723, -2.07258, -1.52476, 0.20051, 0.00867, -1.03723, -0.48754, -0.25289, 0.88104],
+            [-1.03473, -1.34882, -1.09998, -1.20344, 0.22865, 0.02686, -0.88936, -0.31408, -0.06525, 0.76380],
+        ]
     )
 
     energies_3 = np.array(
-        [[-14.68627, -16.50308, -16.31014, -4.72516, 0.17351, 0.00002, -2.90835, -1.81681, -1.62387, 0.98818],
-         [-11.48915, -12.99338, -12.79204, -4.36834, 0.18150, 0.00003, -2.86410, -1.50424, -1.30290, 0.98500],
-         [-11.48915, -12.99338, -12.79204, -4.36834, 0.18150, 0.00003, -2.86410, -1.50424, -1.30289, 0.98500],
-         [-11.48915, -12.99338, -12.79204, -4.36834, 0.18151, 0.00003, -2.86410, -1.50424, -1.30289, 0.98500],
-         [-6.24405, -7.20722, -7.01657, -3.72737, 0.17144, -0.00001, -2.76420, -0.96317, -0.77252, 0.97574],
-         [-6.24403, -7.20721, -7.01657, -3.72738, 0.17144, -0.00000, -2.76421, -0.96317, -0.77253, 0.97575],
-         [-6.24346, -7.20934, -7.01757, -3.73064, 0.17268, 0.00004, -2.76476, -0.96588, -0.77411, 0.97593],
-         [-6.24344, -7.20932, -7.01755, -3.73066, 0.17268, 0.00003, -2.76478, -0.96588, -0.77412, 0.97594],
-         [-6.24344, -7.20932, -7.01755, -3.73066, 0.17268, 0.00003, -2.76478, -0.96588, -0.77411, 0.97593],
-         [-1.81908, -2.30620, -2.07323, -1.52531, 0.19899, 0.00760, -1.03818, -0.48712, -0.25415, 0.88205],
-         [-1.03685, -1.35370, -1.10126, -1.20433, 0.23184, 0.02427, -0.88748, -0.31684, -0.06441, 0.75775]]
+        [
+            [-14.68627, -16.50308, -16.31014, -4.72516, 0.17351, 0.00002, -2.90835, -1.81681, -1.62387, 0.98818],
+            [-11.48915, -12.99338, -12.79204, -4.36834, 0.18150, 0.00003, -2.86410, -1.50424, -1.30290, 0.98500],
+            [-11.48915, -12.99338, -12.79204, -4.36834, 0.18150, 0.00003, -2.86410, -1.50424, -1.30289, 0.98500],
+            [-11.48915, -12.99338, -12.79204, -4.36834, 0.18151, 0.00003, -2.86410, -1.50424, -1.30289, 0.98500],
+            [-6.24405, -7.20722, -7.01657, -3.72737, 0.17144, -0.00001, -2.76420, -0.96317, -0.77252, 0.97574],
+            [-6.24403, -7.20721, -7.01657, -3.72738, 0.17144, -0.00000, -2.76421, -0.96317, -0.77253, 0.97575],
+            [-6.24346, -7.20934, -7.01757, -3.73064, 0.17268, 0.00004, -2.76476, -0.96588, -0.77411, 0.97593],
+            [-6.24344, -7.20932, -7.01755, -3.73066, 0.17268, 0.00003, -2.76478, -0.96588, -0.77412, 0.97594],
+            [-6.24344, -7.20932, -7.01755, -3.73066, 0.17268, 0.00003, -2.76478, -0.96588, -0.77411, 0.97593],
+            [-1.81908, -2.30620, -2.07323, -1.52531, 0.19899, 0.00760, -1.03818, -0.48712, -0.25415, 0.88205],
+            [-1.03685, -1.35370, -1.10126, -1.20433, 0.23184, 0.02427, -0.88748, -0.31684, -0.06441, 0.75775],
+        ]
     )
 
     ref = {
-        1: {'k_point': [0.000000, 0.000000, 0.000000], 'weight': 0.125000},
-        2: {'k_point': [0.000000, 0.000000, 0.500000], 'weight': 0.500000},
-        3: {'k_point': [0.000000, 0.500000, 0.500000], 'weight': 0.375000}
-        }
+        1: {"k_point": [0.000000, 0.000000, 0.000000], "weight": 0.125000},
+        2: {"k_point": [0.000000, 0.000000, 0.500000], "weight": 0.500000},
+        3: {"k_point": [0.000000, 0.500000, 0.500000], "weight": 0.375000},
+    }
 
     output = parse_evalqp(evalqp_mock.full_path)
-    assert set(output.keys()) == {'state_range', 'column_labels', 1, 2, 3}, \
-        'Key include state range, columns and k-indices'
+    assert set(output.keys()) == {
+        "state_range",
+        "column_labels",
+        1,
+        2,
+        3,
+    }, "Key include state range, columns and k-indices"
 
-    del output['state_range']
-    del output['column_labels']
+    del output["state_range"]
+    del output["column_labels"]
 
     # k-points
     assert len(output) == 3, "Expect 3 k-points"
-    assert min([ik for ik in output.keys()]) == 1, 'k-point indexing starts at 1'
-    assert output[1]['k_point'] == ref[1]['k_point'], "Compare k-point 1 to reference"
-    assert output[2]['k_point'] == ref[2]['k_point'], "Compare k-point 2 to reference"
-    assert output[3]['k_point'] == ref[3]['k_point'], "Compare k-point 3 to reference"
+    assert min([ik for ik in output]) == 1, "k-point indexing starts at 1"
+    assert output[1]["k_point"] == ref[1]["k_point"], "Compare k-point 1 to reference"
+    assert output[2]["k_point"] == ref[2]["k_point"], "Compare k-point 2 to reference"
+    assert output[3]["k_point"] == ref[3]["k_point"], "Compare k-point 3 to reference"
 
     # Weights
-    assert output[1]['weight'] == ref[1]['weight'], "Compare weight 1 to reference"
-    assert output[2]['weight'] == ref[2]['weight'], "Compare weight 2 to reference"
-    assert output[3]['weight'] == ref[3]['weight'], "Compare weight 3 to reference"
+    assert output[1]["weight"] == ref[1]["weight"], "Compare weight 1 to reference"
+    assert output[2]["weight"] == ref[2]["weight"], "Compare weight 2 to reference"
+    assert output[3]["weight"] == ref[3]["weight"], "Compare weight 3 to reference"
 
     # Energies
-    assert output[1]['energies'].shape == (11, 10), 'rows = 11 states and cols = 10 energies'
-    assert np.allclose(output[1]['energies'], energies_1), "Compare energies 1 to reference"
-    assert np.allclose(output[2]['energies'], energies_2), "Compare energies 2 to reference"
-    assert np.allclose(output[3]['energies'], energies_3), "Compare energies 3 to reference"
+    assert output[1]["energies"].shape == (11, 10), "rows = 11 states and cols = 10 energies"
+    assert np.allclose(output[1]["energies"], energies_1), "Compare energies 1 to reference"
+    assert np.allclose(output[2]["energies"], energies_2), "Compare energies 2 to reference"
+    assert np.allclose(output[3]["energies"], energies_3), "Compare energies 3 to reference"
```

### Comparing `excitingtools-1.7.0/tests/dict_parsers/test_gw/test_gw_eps00_parser.py` & `excitingtools-1.7.1/tests/dict_parsers/test_gw/test_gw_eps00_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-""" Test all GW output file parsers, except GW_INFO.OUT
-"""
-import pytest
+"""Test all GW output file parsers, except GW_INFO.OUT"""
+
 import numpy as np
+import pytest
 
+from excitingtools.exciting_dict_parsers.gw_eps00_parser import _file_name, parse_eps00_frequencies, parse_eps00_gw
 from excitingtools.utils.test_utils import MockFile
 from excitingtools.utils.utils import get_new_line_indices
 
-from excitingtools.exciting_dict_parsers.gw_eps00_parser import parse_eps00_frequencies, parse_eps00_gw, \
-    _file_name
-
 
 @pytest.fixture
 def eps00_mock(tmp_path):
     # EPS00_GW.OUT segment. Note that first line of file must be blank.
     eps_string = """
 (dielectric tensor, random phase approximation)
 
@@ -37,66 +35,64 @@
 """
     eps00_file = tmp_path / _file_name
     eps00_file.write_text(eps_string)
     return MockFile(eps00_file, eps_string)
 
 
 def test_parse_eps00_frequencies(eps00_mock):
-    """ Test parsing frequencies from EPS00_GW.OUT
-    """
+    """Test parsing frequencies from EPS00_GW.OUT"""
     line = get_new_line_indices(eps00_mock.string)
 
     ref = {1: 0.00529953, 2: 0.02771249, 3: 0.06718440}
 
-    assert eps00_mock.string[line[0]:line[1]].isspace(), "First line of eps_string must be a whiteline"
+    assert eps00_mock.string[line[0] : line[1]].isspace(), "First line of eps_string must be a whiteline"
     assert parse_eps00_frequencies(eps00_mock.string) == ref, "Frequency grid for eps00"
 
 
 def test_parse_eps00_gw(eps00_mock):
-    """ Test parsing EPS00_GW.OUT
-    """
+    """Test parsing EPS00_GW.OUT"""
     line = get_new_line_indices(eps00_mock.string)
-    assert eps00_mock.string[line[0]:line[1]].isspace(), "First line of eps_string must be a whiteline"
+    assert eps00_mock.string[line[0] : line[1]].isspace(), "First line of eps_string must be a whiteline"
 
     ref = {
         1: {
-            'frequency': 0.00529953,
-            'eps00': {
-                're': np.array([[8.31881773, 0., 0.], [0., 8.31881773, 0.], [0., 0., 8.31881773]]),
-                'img': np.array([[0., 0., 0.], [0., 0., 0.], [0., 0., 0.]])
-                }
+            "frequency": 0.00529953,
+            "eps00": {
+                "re": np.array([[8.31881773, 0.0, 0.0], [0.0, 8.31881773, 0.0], [0.0, 0.0, 8.31881773]]),
+                "img": np.array([[0.0, 0.0, 0.0], [0.0, 0.0, 0.0], [0.0, 0.0, 0.0]]),
             },
+        },
         2: {
-            'frequency': 0.02771249,
-            'eps00': {
-                're': np.array([[8.22189228, 0., 0.], [0., 8.22189228, 0.], [0., 0., 8.22189228]]),
-                'img': np.array([[-0., 0., 0.], [0., -0., 0.], [0., 0., -0.]])
-                }
+            "frequency": 0.02771249,
+            "eps00": {
+                "re": np.array([[8.22189228, 0.0, 0.0], [0.0, 8.22189228, 0.0], [0.0, 0.0, 8.22189228]]),
+                "img": np.array([[-0.0, 0.0, 0.0], [0.0, -0.0, 0.0], [0.0, 0.0, -0.0]]),
             },
+        },
         3: {
-            'frequency': 0.06718440,
-            'eps00': {
-                're': np.array([[7.78004308, 0.0, 0.0], [0., 7.78004308, 0.], [0., 0., 7.78004308]]),
-                'img': np.array([[0., 0., 0.], [0., 0., 0.], [0., 0., 0.]])
-                }
-            }
-        }
+            "frequency": 0.06718440,
+            "eps00": {
+                "re": np.array([[7.78004308, 0.0, 0.0], [0.0, 7.78004308, 0.0], [0.0, 0.0, 7.78004308]]),
+                "img": np.array([[0.0, 0.0, 0.0], [0.0, 0.0, 0.0], [0.0, 0.0, 0.0]]),
+            },
+        },
+    }
 
     output = parse_eps00_gw(eps00_mock.file)
 
     assert len(output) == 3, "3 frequency points"
-    assert [k for k in output[1].keys()] == ['frequency', 'eps00'], "Frequency point 1 keys "
-    assert [k for k in output[2].keys()] == ['frequency', 'eps00'], "Frequency point 2 keys "
-    assert [k for k in output[3].keys()] == ['frequency', 'eps00'], "Frequency point 3 keys "
-
-    assert output[1]['frequency'] == 0.00529953, "Frequency point 1 value"
-    assert output[2]['frequency'] == 0.02771249, "Frequency point 2 value"
-    assert output[3]['frequency'] == 0.06718440, "Frequency point 3 value"
+    assert [k for k in output[1]] == ["frequency", "eps00"], "Frequency point 1 keys "
+    assert [k for k in output[2]] == ["frequency", "eps00"], "Frequency point 2 keys "
+    assert [k for k in output[3]] == ["frequency", "eps00"], "Frequency point 3 keys "
+
+    assert output[1]["frequency"] == 0.00529953, "Frequency point 1 value"
+    assert output[2]["frequency"] == 0.02771249, "Frequency point 2 value"
+    assert output[3]["frequency"] == 0.06718440, "Frequency point 3 value"
 
-    assert np.allclose(output[1]['eps00']['re'], ref[1]['eps00']['re']),"Re{eps00} at frequency point 1"
-    assert np.allclose(output[1]['eps00']['img'], ref[1]['eps00']['img']),"Im{eps00} at frequency point 1"
+    assert np.allclose(output[1]["eps00"]["re"], ref[1]["eps00"]["re"]), "Re{eps00} at frequency point 1"
+    assert np.allclose(output[1]["eps00"]["img"], ref[1]["eps00"]["img"]), "Im{eps00} at frequency point 1"
 
-    assert np.allclose(output[2]['eps00']['re'], ref[2]['eps00']['re']),"Re{eps00} at frequency point 2"
-    assert np.allclose(output[2]['eps00']['img'], ref[2]['eps00']['img']),"Im{eps00} at frequency point 2"
+    assert np.allclose(output[2]["eps00"]["re"], ref[2]["eps00"]["re"]), "Re{eps00} at frequency point 2"
+    assert np.allclose(output[2]["eps00"]["img"], ref[2]["eps00"]["img"]), "Im{eps00} at frequency point 2"
 
-    assert np.allclose(output[3]['eps00']['re'], ref[3]['eps00']['re']),"Re{eps00} at frequency point 3"
-    assert np.allclose(output[3]['eps00']['img'], ref[3]['eps00']['img']),"Im{eps00} at frequency point 3"
+    assert np.allclose(output[3]["eps00"]["re"], ref[3]["eps00"]["re"]), "Re{eps00} at frequency point 3"
+    assert np.allclose(output[3]["eps00"]["img"], ref[3]["eps00"]["img"]), "Im{eps00} at frequency point 3"
```

### Comparing `excitingtools-1.7.0/tests/dict_parsers/test_gw/test_gw_info_parser.py` & `excitingtools-1.7.1/tests/dict_parsers/test_gw/test_gw_info_parser.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,291 +2,375 @@
 
 One notes that GW_INFO.OUT is plain text, and so any change to the formatting
 or text which is used in the parser pattern-matching, will break the parser.
 A much better format for this file would be YAML.
 """
 
 import numpy as np
+import pytest
 
-from excitingtools.exciting_dict_parsers.gw_info_parser import parse_gw_info, parse_frequency_grid, \
-    parse_correlation_self_energy_params, extract_kpoints, parse_ks_eigenstates, \
-    parse_n_q_point_cycles, parse_band_structure_info, parse_mixed_product_params, \
-    parse_bare_coulomb_potential_params, parse_gw_timings
+from excitingtools.exciting_dict_parsers.gw_info_parser import (
+    _file_name,
+    extract_kpoints,
+    parse_band_structure_info,
+    parse_bare_coulomb_potential_params,
+    parse_correlation_self_energy_params,
+    parse_frequency_grid,
+    parse_gw_info,
+    parse_gw_timings,
+    parse_ks_eigenstates,
+    parse_mixed_product_params,
+    parse_n_q_point_cycles,
+)
+from excitingtools.utils.test_utils import MockFile
+
+from .mock_gw_info_out import si_2_gw_info_out, zro2_gw_info_out
 
 # Text files are large, it's easier to store externally.
-# Note, these fixtures are used, even if greyed out by the IDE
-from . mock_gw_info_out import zro2_gw_info_out_mock, si_2_gw_info_out_mock
+
+
+@pytest.fixture
+def zro2_gw_info_out_mock(tmp_path):
+    file = tmp_path / _file_name
+    file.write_text(zro2_gw_info_out)
+    return MockFile(file, zro2_gw_info_out)
+
+
+@pytest.fixture
+def si_2_gw_info_out_mock(tmp_path):
+    file = tmp_path / _file_name
+    file.write_text(si_2_gw_info_out)
+    return MockFile(file, si_2_gw_info_out)
 
 
 def test_parse_correlation_self_energy_params(zro2_gw_info_out_mock):
-    """ Test `Correlation self-energy parameters` block of GW_INFO.OUT.
-    """
-    reference = {'Solution of the QP equation': 0,
-                 'Energy alignment': 0,
-                 'Analytic continuation method': "PADE - Thiele's reciprocal difference method",
-                 'Analytic continuation method citation': "H. J. Vidberg and J. W. Serence, J. Low Temp. Phys. 29, 179 (1977)",
-                 'Scheme to treat singularities': 'Auxiliary function method "mpb"',
-                 'Scheme to treat singularities citation': 'S. Massidda, M. Posternak, and A. Baldereschi, PRB 48, 5058 (1993)'
-                 }
+    """Test `Correlation self-energy parameters` block of GW_INFO.OUT."""
+    reference = {
+        "Solution of the QP equation": 0,
+        "Energy alignment": 0,
+        "Analytic continuation method": "PADE - Thiele's reciprocal difference method",
+        "Analytic continuation method citation": "H. J. Vidberg and J. W. Serence, J. Low Temp. Phys. 29, 179 (1977)",
+        "Scheme to treat singularities": 'Auxiliary function method "mpb"',
+        "Scheme to treat singularities citation": "S. Massidda, M. Posternak, and A. Baldereschi, PRB 48, 5058 (1993)",
+    }
 
     output = parse_correlation_self_energy_params(zro2_gw_info_out_mock.string)
     assert reference == output, "parse_correlation_self_energy_params dictionary not consistent with reference"
 
 
 def test_parse_mixed_product_params(zro2_gw_info_out_mock):
-    """ Test `Mixed product basis parameters` block of GW_INFO.OUT.
-    """
+    """Test `Mixed product basis parameters` block of GW_INFO.OUT."""
     ref = {
-        'MT Angular momentum cutoff': 4,
-        'MT Linear dependence tolerance factor': 0.001,
-        'Plane wave cutoff (in units of Gkmax)': 1.0
+        "MT Angular momentum cutoff": 4,
+        "MT Linear dependence tolerance factor": 0.001,
+        "Plane wave cutoff (in units of Gkmax)": 1.0,
     }
 
     output = parse_mixed_product_params(zro2_gw_info_out_mock.string)
 
     assert output == ref, "Expect parsed mixed product basis parameters to equal the reference"
 
 
 def test_parse_bare_coulomb_potential_params(zro2_gw_info_out_mock):
-    """ Test `Bare Coulomb potential parameters` block of GW_INFO.OUT.
-    """
+    """Test `Bare Coulomb potential parameters` block of GW_INFO.OUT."""
     ref = {
-        'Plane wave cutoff (in units of Gkmax*gmb)': 2.0,
-        'Error tolerance for structure constants': 1e-16,
-        'MB tolerance factor': 0.1
+        "Plane wave cutoff (in units of Gkmax*gmb)": 2.0,
+        "Error tolerance for structure constants": 1e-16,
+        "MB tolerance factor": 0.1,
     }
 
     output = parse_bare_coulomb_potential_params(zro2_gw_info_out_mock.string)
 
     assert output == ref, "Expect parsed bare Coulomb parameters to match the reference"
 
 
 def test_parse_frequency_grid(zro2_gw_info_out_mock):
-    """ Test parsing `frequency grid` block of GW_INFO.OUT.
-    """
+    """Test parsing `frequency grid` block of GW_INFO.OUT."""
     n_points = 32
     f_grid = parse_frequency_grid(zro2_gw_info_out_mock.string, n_points)
 
-    ref_frequencies = np.array([5.2995325042E-03, 2.7712488463E-02, 6.7184398806E-02, 0.1222977958, 0.1910618778,
-                                0.2709916112, 0.3591982246, 0.4524937451, 0.5475062549, 0.6408017754,
-                                0.7290083888, 0.8089381222, 0.8777022042, 0.9328156012, 0.9722875115,
-                                0.9947004675, 1.005327767, 1.028502360, 1.072023237, 1.139338599,
-                                1.236188495, 1.371726328, 1.560544990, 1.826463152, 2.209975300,
-                                2.783978125, 3.690151129, 5.233906478, 8.176762249, 14.88440795,
-                                36.08481430, 188.6958895])
-
-    ref_weights = np.array([1.3576229706E-02, 3.1126761969E-02, 4.7579255841E-02, 6.2314485628E-02, 7.4797994408E-02,
-                            8.4578259698E-02, 9.1301707522E-02, 9.4725305228E-02, 9.4725305228E-02, 9.1301707522E-02,
-                            8.4578259698E-02, 7.4797994408E-02, 6.2314485628E-02, 4.7579255841E-02, 3.1126761969E-02,
-                            1.3576229706E-02, 1.3721277051E-02, 3.2926421206E-02, 5.4679689940E-02, 8.0889962951E-02,
-                            0.1143034524, 0.1591452545, 0.2223471090, 0.3160005534, 0.4626375217,
-                            0.7076370069, 1.151720377, 2.048999581, 4.166311667, 10.54097479,
-                            40.53058703, 483.3971183])
+    ref_frequencies = np.array(
+        [
+            5.2995325042e-03,
+            2.7712488463e-02,
+            6.7184398806e-02,
+            0.1222977958,
+            0.1910618778,
+            0.2709916112,
+            0.3591982246,
+            0.4524937451,
+            0.5475062549,
+            0.6408017754,
+            0.7290083888,
+            0.8089381222,
+            0.8777022042,
+            0.9328156012,
+            0.9722875115,
+            0.9947004675,
+            1.005327767,
+            1.028502360,
+            1.072023237,
+            1.139338599,
+            1.236188495,
+            1.371726328,
+            1.560544990,
+            1.826463152,
+            2.209975300,
+            2.783978125,
+            3.690151129,
+            5.233906478,
+            8.176762249,
+            14.88440795,
+            36.08481430,
+            188.6958895,
+        ]
+    )
+
+    ref_weights = np.array(
+        [
+            1.3576229706e-02,
+            3.1126761969e-02,
+            4.7579255841e-02,
+            6.2314485628e-02,
+            7.4797994408e-02,
+            8.4578259698e-02,
+            9.1301707522e-02,
+            9.4725305228e-02,
+            9.4725305228e-02,
+            9.1301707522e-02,
+            8.4578259698e-02,
+            7.4797994408e-02,
+            6.2314485628e-02,
+            4.7579255841e-02,
+            3.1126761969e-02,
+            1.3576229706e-02,
+            1.3721277051e-02,
+            3.2926421206e-02,
+            5.4679689940e-02,
+            8.0889962951e-02,
+            0.1143034524,
+            0.1591452545,
+            0.2223471090,
+            0.3160005534,
+            0.4626375217,
+            0.7076370069,
+            1.151720377,
+            2.048999581,
+            4.166311667,
+            10.54097479,
+            40.53058703,
+            483.3971183,
+        ]
+    )
 
     assert len(ref_frequencies) == 32, "Require 32 reference frequency points"
     assert len(ref_weights) == 32, "Require 32 reference weights"
 
-    assert np.allclose(f_grid[0, :],
-                       ref_frequencies), "Frequency points parsed from gw_info_out disagree with reference"
+    assert np.allclose(
+        f_grid[0, :], ref_frequencies
+    ), "Frequency points parsed from gw_info_out disagree with reference"
     assert np.allclose(f_grid[1, :], ref_weights), "Weights parsed from gw_info_out disagree with reference"
 
 
 def test_parse_ks_eigenstates(zro2_gw_info_out_mock):
-    """ Test parsing ` Kohn-Sham eigenstates summary` block from GW_INFO.OUT.
-    """
+    """Test parsing ` Kohn-Sham eigenstates summary` block from GW_INFO.OUT."""
     ref = {
-        'Maximum number of LAPW states': 847,
-        'Minimal number of LAPW states': 838,
-        'Number of states used in GW - total KS': 838,
-        'Number of states used in GW - occupied': 21,
-        'Number of states used in GW - unoccupied': 2000,
-        'Number of states used in GW - dielectric function': 838,
-        'Number of states used in GW - self energy': 838,
-        'Energy of the highest unoccupied state': 1030.791933,
-        'Number of valence electrons': 42,
-        'Number of valence electrons treated in GW': 42
+        "Maximum number of LAPW states": 847,
+        "Minimal number of LAPW states": 838,
+        "Number of states used in GW - total KS": 838,
+        "Number of states used in GW - occupied": 21,
+        "Number of states used in GW - unoccupied": 2000,
+        "Number of states used in GW - dielectric function": 838,
+        "Number of states used in GW - self energy": 838,
+        "Energy of the highest unoccupied state": 1030.791933,
+        "Number of valence electrons": 42,
+        "Number of valence electrons treated in GW": 42,
     }
 
     output = parse_ks_eigenstates(zro2_gw_info_out_mock.string)
 
     assert output == ref, "Parsed KS eigenstates settings not consistent with reference"
 
 
 def test_parse_n_q_point_cycles(zro2_gw_info_out_mock):
     max_q = parse_n_q_point_cycles(zro2_gw_info_out_mock.string)
     assert max_q == 2, "Two q cycles expected from the reference data"
 
 
 def test_extract_kpoint(zro2_gw_info_out_mock):
-    ref = {'VBM': {'k_point': [0.0, 0.5, 0.5], 'ik': 3},
-           'CBm': {'k_point': [0.0, 0.0, 0.0], 'ik': 1}
-           }
+    ref = {"VBM": {"k_point": [0.0, 0.5, 0.5], "ik": 3}, "CBm": {"k_point": [0.0, 0.0, 0.0], "ik": 1}}
 
     output = extract_kpoints(zro2_gw_info_out_mock.string)
 
     assert output == ref, "Expect extracted VBM and CBm k-points to match reference"
 
 
 def test_parse_band_structure_info(zro2_gw_info_out_mock):
-    """ Test parsing the `Kohn-Sham band structure` block of GW_INFO.OUT
-    """
+    """Test parsing the `Kohn-Sham band structure` block of GW_INFO.OUT"""
     ks_ref = {
-        'Fermi energy': 0.0,
-        'Energy range': [-14.6863, 1030.7919],
-        'Band index of VBM': 21,
-        'Band index of CBm': 22,
-        'Indirect BandGap (eV)': 3.3206,
-        'Direct Bandgap at k(VBM) (eV)': 3.7482,
-        'Direct Bandgap at k(CBm) (eV)': 3.8653,
-        'VBM': {'k_point': [0.0, 0.5, 0.5], 'ik': 3},
-        'CBm': {'k_point': [0.0, 0.0, 0.0], 'ik': 1}
+        "Fermi energy": 0.0,
+        "Energy range": [-14.6863, 1030.7919],
+        "Band index of VBM": 21,
+        "Band index of CBm": 22,
+        "Indirect BandGap (eV)": 3.3206,
+        "Direct Bandgap at k(VBM) (eV)": 3.7482,
+        "Direct Bandgap at k(CBm) (eV)": 3.8653,
+        "VBM": {"k_point": [0.0, 0.5, 0.5], "ik": 3},
+        "CBm": {"k_point": [0.0, 0.0, 0.0], "ik": 1},
     }
-    ks_output = parse_band_structure_info(zro2_gw_info_out_mock.string, 'ks')
+    ks_output = parse_band_structure_info(zro2_gw_info_out_mock.string, "ks")
     assert ks_output == ks_ref, "Expect parsed KS band structure info to match the reference"
 
 
 def test_parse_g0w0_band_structure_info(si_2_gw_info_out_mock, zro2_gw_info_out_mock):
-    """ Test parsing the `G0W0 band structure` block of GW_INFO.OUT
-    """
+    """Test parsing the `G0W0 band structure` block of GW_INFO.OUT"""
     # Direct gap
     g0w0_ref = {
-        'Fermi energy': 0.0176,
-        'Energy range': [-0.4799, 0.5045],
-        'Band index of VBM': 4,
-        'Band index of CBm': 5,
-        'Direct BandGap (eV)': 3.2457,
-        'VBM': {'k_point': [0.0, 0.0, 0.0], 'ik': 1},
-        'CBm': {'k_point': [0.0, 0.0, 0.0], 'ik': 1}
+        "Fermi energy": 0.0176,
+        "Energy range": [-0.4799, 0.5045],
+        "Band index of VBM": 4,
+        "Band index of CBm": 5,
+        "Direct BandGap (eV)": 3.2457,
+        "VBM": {"k_point": [0.0, 0.0, 0.0], "ik": 1},
+        "CBm": {"k_point": [0.0, 0.0, 0.0], "ik": 1},
     }
-    gw_output = parse_band_structure_info(si_2_gw_info_out_mock.string, 'gw')
-    assert gw_output == g0w0_ref, \
-        "Expect parsed G0W0 band structure info to match the reference for direct gap "
-
+    gw_output = parse_band_structure_info(si_2_gw_info_out_mock.string, "gw")
+    assert gw_output == g0w0_ref, "Expect parsed G0W0 band structure info to match the reference for direct gap "
 
     # Indirect gap
     g0w0_ref = {
-        'Fermi energy': -0.0054,
-        'Energy range': [-16.2632, 1031.409],
-        'Band index of VBM': 21,
-        'Band index of CBm': 22,
-        'Indirect BandGap (eV)': 5.392,
-        'Direct Bandgap at k(VBM) (eV)': 5.5472,
-        'Direct Bandgap at k(CBm) (eV)': 5.9646,
-        'VBM': {'k_point': [0.0, 0.5, 0.5], 'ik': 3},
-        'CBm': {'k_point': [0.0, 0.0, 0.0], 'ik': 1}
+        "Fermi energy": -0.0054,
+        "Energy range": [-16.2632, 1031.409],
+        "Band index of VBM": 21,
+        "Band index of CBm": 22,
+        "Indirect BandGap (eV)": 5.392,
+        "Direct Bandgap at k(VBM) (eV)": 5.5472,
+        "Direct Bandgap at k(CBm) (eV)": 5.9646,
+        "VBM": {"k_point": [0.0, 0.5, 0.5], "ik": 3},
+        "CBm": {"k_point": [0.0, 0.0, 0.0], "ik": 1},
     }
-    gw_output = parse_band_structure_info(zro2_gw_info_out_mock.string, 'gw')
-    assert gw_output == g0w0_ref, \
-        "Expect parsed G0W0 band structure info to match the reference for indirect gap"
+    gw_output = parse_band_structure_info(zro2_gw_info_out_mock.string, "gw")
+    assert gw_output == g0w0_ref, "Expect parsed G0W0 band structure info to match the reference for indirect gap"
 
 
 def test_parse_gw_info(zro2_gw_info_out_mock):
-    """ Test parsing of the whole GW_INFO.OUT
-    """
+    """Test parsing of the whole GW_INFO.OUT"""
 
     # Reference, without frequencies_weights
-    ref = {'correlation_self_energy_parameters': {'Solution of the QP equation': 0,
-                                                  'Energy alignment': 0,
-                                                  'Analytic continuation method': "PADE - Thiele's reciprocal difference method",
-                                                  'Analytic continuation method citation':
-                                                      'H. J. Vidberg and J. W. Serence, J. Low Temp. Phys. 29, 179 (1977)',
-                                                  'Scheme to treat singularities': 'Auxiliary function method "mpb"',
-                                                  'Scheme to treat singularities citation':
-                                                      'S. Massidda, M. Posternak, and A. Baldereschi, PRB 48, 5058 (1993)'},
-           'mixed_product_basis_parameters': {'MT Angular momentum cutoff': 4,
-                                              'MT Linear dependence tolerance factor': 0.001,
-                                              'Plane wave cutoff (in units of Gkmax)': 1.0},
-           'bare_coulomb_potential_parameters': {'Plane wave cutoff (in units of Gkmax*gmb)': 2.0,
-                                                 'Error tolerance for structure constants': 1e-16,
-                                                 'MB tolerance factor': 0.1},
-           'screened_coulomb_potential': 'Full-frequency Random-Phase Approximation',
-           'core_electrons_treatment': 'all - Core states are included in all calculations',
-           'qp_interval': [1, 2000],
-           'n_empty': 2000,
-           'q_grid': [2, 2, 2],
-           'mixed_product_wf_info': {'Maximal number of MT wavefunctions per atom': 1069,
-                                     'Total number of MT wavefunctions': 2733,
-                                     'Maximal number of PW wavefunctions': 468,
-                                     'Total number of mixed-product wavefunctions': 3201},
-           'frequency_grid': {'Type: < fgrid >': 'gauleg2',
-                              'Frequency axis: < fconv >': 'imfreq',
-                              'Number of frequencies: < nomeg >': 32,
-                              'Cutoff frequency: < freqmax >': 1.0},
-           'ks_eigenstates_summary': {'Maximum number of LAPW states': 847,
-                                      'Minimal number of LAPW states': 838,
-                                      'Number of states used in GW - total KS': 838,
-                                      'Number of states used in GW - occupied': 21,
-                                      'Number of states used in GW - unoccupied': 2000,
-                                      'Number of states used in GW - dielectric function': 838,
-                                      'Number of states used in GW - self energy': 838,
-                                      'Energy of the highest unoccupied state': 1030.791933,
-                                      'Number of valence electrons': 42,
-                                      'Number of valence electrons treated in GW': 42},
-           'ks_band_structure_summary': {'Fermi energy': 0.0,
-                                         'Energy range': [-14.6863, 1030.7919],
-                                         'Band index of VBM': 21, 'Band index of CBm': 22,
-                                         'Indirect BandGap (eV)': 3.3206,
-                                         'Direct Bandgap at k(VBM) (eV)': 3.7482,
-                                         'Direct Bandgap at k(CBm) (eV)': 3.8653,
-                                         'VBM': {'k_point': [0.0, 0.5, 0.5], 'ik': 3},
-                                         'CBm': {'k_point': [0.0, 0.0, 0.0], 'ik': 1}},
-           'n_q_cycles': 2,
-           'g0w0_band_structure_summary': {'Fermi energy': -0.0054,
-                                           'Energy range': [-16.2632, 1031.409],
-                                           'Band index of VBM': 21,
-                                           'Band index of CBm': 22,
-                                           'Indirect BandGap (eV)': 5.392,
-                                           'Direct Bandgap at k(VBM) (eV)': 5.5472,
-                                           'Direct Bandgap at k(CBm) (eV)': 5.9646,
-                                           'VBM': {'k_point': [0.0, 0.5, 0.5], 'ik': 3},
-                                           'CBm': {'k_point': [0.0, 0.0, 0.0], 'ik': 1}}
-           }
+    ref = {
+        "correlation_self_energy_parameters": {
+            "Solution of the QP equation": 0,
+            "Energy alignment": 0,
+            "Analytic continuation method": "PADE - Thiele's reciprocal difference method",
+            "Analytic continuation method citation": "H. J. Vidberg and J. W. Serence, J. Low Temp. Phys. 29, 179 (1977)",
+            "Scheme to treat singularities": 'Auxiliary function method "mpb"',
+            "Scheme to treat singularities citation": "S. Massidda, M. Posternak, and A. Baldereschi, PRB 48, 5058 (1993)",
+        },
+        "mixed_product_basis_parameters": {
+            "MT Angular momentum cutoff": 4,
+            "MT Linear dependence tolerance factor": 0.001,
+            "Plane wave cutoff (in units of Gkmax)": 1.0,
+        },
+        "bare_coulomb_potential_parameters": {
+            "Plane wave cutoff (in units of Gkmax*gmb)": 2.0,
+            "Error tolerance for structure constants": 1e-16,
+            "MB tolerance factor": 0.1,
+        },
+        "screened_coulomb_potential": "Full-frequency Random-Phase Approximation",
+        "core_electrons_treatment": "all - Core states are included in all calculations",
+        "qp_interval": [1, 2000],
+        "n_empty": 2000,
+        "q_grid": [2, 2, 2],
+        "mixed_product_wf_info": {
+            "Maximal number of MT wavefunctions per atom": 1069,
+            "Total number of MT wavefunctions": 2733,
+            "Maximal number of PW wavefunctions": 468,
+            "Total number of mixed-product wavefunctions": 3201,
+        },
+        "frequency_grid": {
+            "Type: < fgrid >": "gauleg2",
+            "Frequency axis: < fconv >": "imfreq",
+            "Number of frequencies: < nomeg >": 32,
+            "Cutoff frequency: < freqmax >": 1.0,
+        },
+        "ks_eigenstates_summary": {
+            "Maximum number of LAPW states": 847,
+            "Minimal number of LAPW states": 838,
+            "Number of states used in GW - total KS": 838,
+            "Number of states used in GW - occupied": 21,
+            "Number of states used in GW - unoccupied": 2000,
+            "Number of states used in GW - dielectric function": 838,
+            "Number of states used in GW - self energy": 838,
+            "Energy of the highest unoccupied state": 1030.791933,
+            "Number of valence electrons": 42,
+            "Number of valence electrons treated in GW": 42,
+        },
+        "ks_band_structure_summary": {
+            "Fermi energy": 0.0,
+            "Energy range": [-14.6863, 1030.7919],
+            "Band index of VBM": 21,
+            "Band index of CBm": 22,
+            "Indirect BandGap (eV)": 3.3206,
+            "Direct Bandgap at k(VBM) (eV)": 3.7482,
+            "Direct Bandgap at k(CBm) (eV)": 3.8653,
+            "VBM": {"k_point": [0.0, 0.5, 0.5], "ik": 3},
+            "CBm": {"k_point": [0.0, 0.0, 0.0], "ik": 1},
+        },
+        "n_q_cycles": 2,
+        "g0w0_band_structure_summary": {
+            "Fermi energy": -0.0054,
+            "Energy range": [-16.2632, 1031.409],
+            "Band index of VBM": 21,
+            "Band index of CBm": 22,
+            "Indirect BandGap (eV)": 5.392,
+            "Direct Bandgap at k(VBM) (eV)": 5.5472,
+            "Direct Bandgap at k(CBm) (eV)": 5.9646,
+            "VBM": {"k_point": [0.0, 0.5, 0.5], "ik": 3},
+            "CBm": {"k_point": [0.0, 0.0, 0.0], "ik": 1},
+        },
+    }
 
     output = parse_gw_info(zro2_gw_info_out_mock.file)
 
     # frequencies and weights tested in separate unit test
-    f_w = output['frequency_grid'].pop('frequencies_weights')
+    output["frequency_grid"].pop("frequencies_weights")
 
     assert output == ref, "Output from parse_gw_info does not agree with reference dictionary"
 
 
 def test_parse_gw_timings(zro2_gw_info_out_mock):
-    """ Test parsing `GW timing info` block in GW_INFO.OUT
-    """
+    """Test parsing `GW timing info` block in GW_INFO.OUT"""
 
     ref = {
-        'Initialization': {
-            'Initialization': 15.46,
-            'init_scf': 8.38,
-            'init_kpt': 0.04,
-            'init_eval': 0.02,
-            'init_freq': 0.0,
-            'init_mb': 6.76
-        },
-        'Subroutines': {
-            'Subroutines': None,
-            'calcpmat': 5.12,
-            'calcbarcmb': 5.65,
-            'BZ integration weights': 18.35
-        },
-        'Dielectric function': {
-            'Dielectric function': 422.09,
-            'head': 0.3,
-            'wings': 70.14,
-            'body (not timed)': 0.0,
-            'inversion': 1.72
-        },
-        'WF products expansion': {
-            'WF products expansion': 2525.59,
-            'diagsgi': 0.24,
-            'calcmpwipw': 0.04,
-            'calcmicm': 2.63,
-            'calcminc': 2.1,
-            'calcminm': 2520.58
-        },
-        'Self-energy': {'Self-energy': 7069.46, 'calcselfx': 43.33, 'calcselfc': 7026.14},
-        'calcvxcnn': {'calcvxcnn': 27.52},
-        'input/output': {'input/output': 0.0},
-        'Total': {'Total': 7555.78}
+        "Initialization": {
+            "Initialization": 15.46,
+            "init_scf": 8.38,
+            "init_kpt": 0.04,
+            "init_eval": 0.02,
+            "init_freq": 0.0,
+            "init_mb": 6.76,
+        },
+        "Subroutines": {"Subroutines": None, "calcpmat": 5.12, "calcbarcmb": 5.65, "BZ integration weights": 18.35},
+        "Dielectric function": {
+            "Dielectric function": 422.09,
+            "head": 0.3,
+            "wings": 70.14,
+            "body (not timed)": 0.0,
+            "inversion": 1.72,
+        },
+        "WF products expansion": {
+            "WF products expansion": 2525.59,
+            "diagsgi": 0.24,
+            "calcmpwipw": 0.04,
+            "calcmicm": 2.63,
+            "calcminc": 2.1,
+            "calcminm": 2520.58,
+        },
+        "Self-energy": {"Self-energy": 7069.46, "calcselfx": 43.33, "calcselfc": 7026.14},
+        "calcvxcnn": {"calcvxcnn": 27.52},
+        "input/output": {"input/output": 0.0},
+        "Total": {"Total": 7555.78},
     }
 
-    assert parse_gw_timings(zro2_gw_info_out_mock.string) == ref, "Parsed timings do not agree with reference dictionary"
+    assert (
+        parse_gw_timings(zro2_gw_info_out_mock.string) == ref
+    ), "Parsed timings do not agree with reference dictionary"
```

### Comparing `excitingtools-1.7.0/tests/dict_parsers/test_gw/test_gw_taskgroup_parser.py` & `excitingtools-1.7.1/tests/dict_parsers/test_gw/test_gw_taskgroup_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,117 +1,145 @@
 """
 Tests for the gw_taskgroup_parser
 """
 
-import pytest
 import numpy as np
+import pytest
 
-from excitingtools.exciting_dict_parsers.gw_taskgroup_parser import parse_barc, \
-  parse_sgi, parse_epsilon, parse_inverse_epsilon
+from excitingtools.exciting_dict_parsers.gw_taskgroup_parser import (
+    parse_barc,
+    parse_epsilon,
+    parse_inverse_epsilon,
+    parse_sgi,
+)
 
 rectangular_matrix = """ 2
 1 1 2 3
 (1.01E-4,-5.5E-8)
 (0.25,0.77)
 (0.25,0.77)
 (0.000000000000000E+000,0.000000000000000E+000)
 (5.4E+005,-1.1)
 (-5.4E+005,1.1)
 """
 
 reference_rectangular_matrix = {
-    "matrix": np.array([
-        [complex(1.01e-4, -5.5e-8), complex(0.25, 0.77), complex(5.4e5, -1.1)],
-        [complex(0.25, 0.77), complex(0., 0.), complex(-5.4e5, 1.1)]
-    ])
+    "matrix": np.array(
+        [
+            [complex(1.01e-4, -5.5e-8), complex(0.25, 0.77), complex(5.4e5, -1.1)],
+            [complex(0.25, 0.77), complex(0.0, 0.0), complex(-5.4e5, 1.1)],
+        ]
+    )
 }
 
 square_matrix = """ 2
 1 1 2 2
 (1.01E-4,-5.5E-8) (0.000000000000000E+000,0.000000000000000E+000)
 (5.4E+005,-1.1)
 (-5.4E+005,1.1)
 """
 
 reference_square_matrix = {
-    "matrix": np.array([
-        [complex(1.01e-4, -5.5e-8), complex(5.4e5, -1.1)],
-        [complex(0., 0.), complex(-5.4e5, 1.1)]
-    ])
+    "matrix": np.array([[complex(1.01e-4, -5.5e-8), complex(5.4e5, -1.1)], [complex(0.0, 0.0), complex(-5.4e5, 1.1)]])
 }
 
 
-@pytest.mark.parametrize(["barc_file_str", "reference_barc"],
-                         [(rectangular_matrix, reference_rectangular_matrix),
-                          (square_matrix, reference_square_matrix)])
+@pytest.mark.parametrize(
+    ["barc_file_str", "reference_barc"],
+    [(rectangular_matrix, reference_rectangular_matrix), (square_matrix, reference_square_matrix)],
+)
 def test_parse_barc(barc_file_str, reference_barc, tmp_path):
     barc_file_path = tmp_path / "BARC_1.OUT"
     barc_file_path.write_text(barc_file_str)
     barc = parse_barc(barc_file_path.as_posix())
     A = reference_barc["matrix"]
     ref = {"CoulombMatrix": np.matmul(A.T.conj(), A)}
     np.testing.assert_allclose(barc["CoulombMatrix"], ref["CoulombMatrix"])
 
-@pytest.mark.parametrize(["sgi_file_str", "reference_sgi"],
-                         [(rectangular_matrix, reference_rectangular_matrix),
-                          (square_matrix, reference_square_matrix)])
+
+@pytest.mark.parametrize(
+    ["sgi_file_str", "reference_sgi"],
+    [(rectangular_matrix, reference_rectangular_matrix), (square_matrix, reference_square_matrix)],
+)
 def test_parse_sgi(sgi_file_str, reference_sgi, tmp_path):
     sgi_file_path = tmp_path / "SGI_1.OUT"
     sgi_file_path.write_text(sgi_file_str)
     sgi = parse_sgi(sgi_file_path.as_posix())
     A = reference_sgi["matrix"]
     ref = {"OverlapMatrix": np.matmul(A.T.conj(), A)}
     np.testing.assert_allclose(sgi["OverlapMatrix"], ref["OverlapMatrix"])
 
+
 array_of_rank_3_example_1 = """ 3
 1 1 1 2 2 1
 (1.01E-4,-5.5E-8) (0.25,0.77)
 (0.35,0.88) (0.000000000000000E+000,0.000000000000000E+000)
 """
 
-reference_array_of_rank_3_example_1 = { 
-    "array": np.array([
-        [[complex(1.01e-4, -5.5e-8)], [complex(0.35,0.88)]],
-        [[complex(0.25, 0.77)], [complex(0., 0.0)]]
-    ])
+reference_array_of_rank_3_example_1 = {
+    "array": np.array(
+        [[[complex(1.01e-4, -5.5e-8)], [complex(0.35, 0.88)]], [[complex(0.25, 0.77)], [complex(0.0, 0.0)]]]
+    )
 }
 
 array_of_rank_3_example_2 = """ 3
 1 1 1 3 4 2
 (1.01E-4,-5.5E-8) (0.25,0.77)
 (0.35,0.88) (0.000000000000000E+000,0.000000000000000E+000)
 (-1.01E+004,-5.4E-8) (0.19,0.21) (1.5E-3,-9E6)
 (0.07,0.00) (0.08,0.09) (1.1,2.2) (-4.5,-2.1) (-6.0E+000,8.0E-006)
 (0.1,0.2) (1.5,2.5) (3.5,7.8) (7.0,8.7) (5.0,6.5) (8.0,9.1)
 (0.01,0.00) (0.00,0.01) (0.02,0.00) (0.00,0.02) (0.3,0.0) (0.0,0.3)
 """
 
-reference_array_of_rank_3_example_2 = { 
-    "array": np.array([
-        [[complex(1.01e-4,-5.5e-8), complex(0.1,0.2)], [complex(0.,0.), complex(7.0,8.7)], 
-         [complex(1.5e-3,-9e6), complex(0.01,0.00)], [complex(1.1,2.2), complex(0.00,0.02)]],
-        [[complex(0.25,0.77), complex(1.5,2.5)], [complex(-1.01e4,-5.4e-8), complex(5.0,6.5)], 
-         [complex(0.07,0.00), complex(0.00,0.01)], [complex(-4.5,-2.1), complex(0.3,0.0)]],
-        [[complex(0.35,0.88), complex(3.5,7.8)], [complex(0.19,0.21), complex(8.0,9.1)], 
-         [complex(0.08,0.09), complex(0.02,0.00)], [complex(-6,8e-6), complex(0.0,0.3)]]
-    ])
+reference_array_of_rank_3_example_2 = {
+    "array": np.array(
+        [
+            [
+                [complex(1.01e-4, -5.5e-8), complex(0.1, 0.2)],
+                [complex(0.0, 0.0), complex(7.0, 8.7)],
+                [complex(1.5e-3, -9e6), complex(0.01, 0.00)],
+                [complex(1.1, 2.2), complex(0.00, 0.02)],
+            ],
+            [
+                [complex(0.25, 0.77), complex(1.5, 2.5)],
+                [complex(-1.01e4, -5.4e-8), complex(5.0, 6.5)],
+                [complex(0.07, 0.00), complex(0.00, 0.01)],
+                [complex(-4.5, -2.1), complex(0.3, 0.0)],
+            ],
+            [
+                [complex(0.35, 0.88), complex(3.5, 7.8)],
+                [complex(0.19, 0.21), complex(8.0, 9.1)],
+                [complex(0.08, 0.09), complex(0.02, 0.00)],
+                [complex(-6, 8e-6), complex(0.0, 0.3)],
+            ],
+        ]
+    )
 }
 
-@pytest.mark.parametrize(["file_epsilon_str", "reference_epsilon"],
-                         [(array_of_rank_3_example_1,reference_array_of_rank_3_example_1),
-                          (array_of_rank_3_example_2,reference_array_of_rank_3_example_2)])
+
+@pytest.mark.parametrize(
+    ["file_epsilon_str", "reference_epsilon"],
+    [
+        (array_of_rank_3_example_1, reference_array_of_rank_3_example_1),
+        (array_of_rank_3_example_2, reference_array_of_rank_3_example_2),
+    ],
+)
 def test_parse_epsilon(file_epsilon_str, reference_epsilon, tmp_path):
     epsilon_file_path = tmp_path / "EPSILON-GW_1.OUT"
     epsilon_file_path.write_text(file_epsilon_str)
     epsilon = parse_epsilon(epsilon_file_path.as_posix())
     np.testing.assert_allclose(epsilon["epsilon_tensor"], reference_epsilon["array"])
 
-@pytest.mark.parametrize(["file_inverse_epsilon_str", "reference_inverse_epsilon"],
-                         [(array_of_rank_3_example_1,reference_array_of_rank_3_example_1),
-                          (array_of_rank_3_example_2,reference_array_of_rank_3_example_2)])
+
+@pytest.mark.parametrize(
+    ["file_inverse_epsilon_str", "reference_inverse_epsilon"],
+    [
+        (array_of_rank_3_example_1, reference_array_of_rank_3_example_1),
+        (array_of_rank_3_example_2, reference_array_of_rank_3_example_2),
+    ],
+)
 def test_parse_inverse_epsilon(file_inverse_epsilon_str, reference_inverse_epsilon, tmp_path):
     inverse_epsilon_file_path = tmp_path / "INVERSE-EPSILON_1.OUT"
     inverse_epsilon_file_path.write_text(file_inverse_epsilon_str)
     inverse_epsilon = parse_inverse_epsilon(inverse_epsilon_file_path.as_posix())
-    np.testing.assert_allclose( 
-        inverse_epsilon["inverse_epsilon_tensor"], reference_inverse_epsilon["array"]
-    )
+    np.testing.assert_allclose(inverse_epsilon["inverse_epsilon_tensor"], reference_inverse_epsilon["array"])
```

### Comparing `excitingtools-1.7.0/tests/dict_parsers/test_gw/test_gw_vxc_parser.py` & `excitingtools-1.7.1/tests/dict_parsers/test_gw/test_gw_vxc_parser.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-import pytest
 import numpy as np
+import pytest
 
-from excitingtools.utils.test_utils import MockFile
 from excitingtools.exciting_dict_parsers.gw_vxc_parser import parse_vxcnn, vkl_from_vxc
+from excitingtools.utils.test_utils import MockFile
 
 
 @pytest.fixture
 def vxc_mock(tmp_path):
-    """ Mock VXCNN.DAT data with energies for 3 k-points
-    """
+    """Mock VXCNN.DAT data with energies for 3 k-points"""
     vxc_string = """ik=   1    vkl=  0.0000  0.0000  0.0000
        1       -2.908349       -0.000000
        2       -2.864103        0.000000
        3       -2.864103       -0.000000
        4       -2.864103       -0.000000
        5       -2.764246       -0.000000
        6       -2.764246        0.000000
@@ -51,50 +50,80 @@
     file = tmp_path / "VXCNN.DAT"
     file.write_text(vxc_string)
     return MockFile(file, vxc_string)
 
 
 def test_vkl_from_vxc(vxc_mock):
     # k-points in units of the lattice vectors
-    vkl_ref = {
-        1: [0.0000, 0.0000, 0.0000], 2: [0.0000, 0.0000, 0.5000], 3: [0.0000, 0.5000, 0.5000]
-        }
+    vkl_ref = {1: [0.0000, 0.0000, 0.0000], 2: [0.0000, 0.0000, 0.5000], 3: [0.0000, 0.5000, 0.5000]}
     output = vkl_from_vxc(vxc_mock.string)
     assert len(output) == 3, "Expect 3 k-points"
     assert output == vkl_ref, "vkl values equal to vkl_ref"
 
 
 def test_parse_vxcnn(vxc_mock):
-
     # Reference V_xc extracted from vxc_string, defined above
-    v_xc_1 = np.array([[-2.908349, -0.000000], [-2.864103, 0.000000], [-2.864103, -0.000000],
-                       [-2.864103, -0.000000], [-2.764246, -0.000000], [-2.764246, 0.000000],
-                       [-2.764809, -0.000000], [-2.764809, -0.000000], [-2.764809, -0.000000],
-                       [-1.034312, -0.000000], [-0.929773, -0.000000]])
-
-    v_xc_2 = np.array([[-2.908349, 0.000000], [-2.864100, -0.000000], [-2.864100, 0.000000],
-                       [-2.864101, -0.000000], [-2.764227, -0.000000], [-2.764227, 0.000000],
-                       [-2.764770, 0.000000], [-2.764777, 0.000000], [-2.764777, 0.000000],
-                       [-1.037228, -0.000000], [-0.889360, 0.000000]])
-
-    v_xc_3 = np.array([[-2.908349, -0.000000], [-2.864099, -0.000000], [-2.864099, -0.000000],
-                       [-2.864099, 0.000000], [-2.764195, 0.000000], [-2.764208, 0.000000],
-                       [-2.764760, -0.000000], [-2.764780, -0.000000], [-2.764780, -0.000000],
-                       [-1.038185, 0.000000], [-0.887485, -0.000000]])
+    v_xc_1 = np.array(
+        [
+            [-2.908349, -0.000000],
+            [-2.864103, 0.000000],
+            [-2.864103, -0.000000],
+            [-2.864103, -0.000000],
+            [-2.764246, -0.000000],
+            [-2.764246, 0.000000],
+            [-2.764809, -0.000000],
+            [-2.764809, -0.000000],
+            [-2.764809, -0.000000],
+            [-1.034312, -0.000000],
+            [-0.929773, -0.000000],
+        ]
+    )
+
+    v_xc_2 = np.array(
+        [
+            [-2.908349, 0.000000],
+            [-2.864100, -0.000000],
+            [-2.864100, 0.000000],
+            [-2.864101, -0.000000],
+            [-2.764227, -0.000000],
+            [-2.764227, 0.000000],
+            [-2.764770, 0.000000],
+            [-2.764777, 0.000000],
+            [-2.764777, 0.000000],
+            [-1.037228, -0.000000],
+            [-0.889360, 0.000000],
+        ]
+    )
+
+    v_xc_3 = np.array(
+        [
+            [-2.908349, -0.000000],
+            [-2.864099, -0.000000],
+            [-2.864099, -0.000000],
+            [-2.864099, 0.000000],
+            [-2.764195, 0.000000],
+            [-2.764208, 0.000000],
+            [-2.764760, -0.000000],
+            [-2.764780, -0.000000],
+            [-2.764780, -0.000000],
+            [-1.038185, 0.000000],
+            [-0.887485, -0.000000],
+        ]
+    )
 
     output = parse_vxcnn(vxc_mock.file)
 
-    assert [key for key in output[1].keys()] == ['vkl', 'v_xc_nn'], "Key consistency for ik=1 of parsed vxcnn"
-    assert [key for key in output[2].keys()] == ['vkl', 'v_xc_nn'], "Key consistency for ik=2 of parsed vxcnn"
-    assert [key for key in output[3].keys()] == ['vkl', 'v_xc_nn'], "Key consistency for ik=3 of parsed vxcnn"
-
-    assert output[1]['vkl'] == [0.0000, 0.0000, 0.0000], "vkl (ik=1)"
-    assert output[2]['vkl'] == [0.0000, 0.0000, 0.5000], "vkl (ik=2)"
-    assert output[3]['vkl'] == [0.0000, 0.5000, 0.5000], "vkl (ik=3)"
-
-    assert output[1]['v_xc_nn'].shape == (11, 2), "Expect V_xc to have 2 cols for 11 states"
-    assert output[2]['v_xc_nn'].shape == (11, 2), "Expect V_xc to have 2 cols for 11 states"
-    assert output[3]['v_xc_nn'].shape == (11, 2), "Expect V_xc to have 2 cols for 11 states"
-
-    assert np.allclose(output[1]['v_xc_nn'], v_xc_1), "v_xc_nn for ik=1"
-    assert np.allclose(output[2]['v_xc_nn'], v_xc_2), "v_xc_nn for ik=2"
-    assert np.allclose(output[3]['v_xc_nn'], v_xc_3), "v_xc_nn for ik=3"
+    assert [key for key in output[1]] == ["vkl", "v_xc_nn"], "Key consistency for ik=1 of parsed vxcnn"
+    assert [key for key in output[2]] == ["vkl", "v_xc_nn"], "Key consistency for ik=2 of parsed vxcnn"
+    assert [key for key in output[3]] == ["vkl", "v_xc_nn"], "Key consistency for ik=3 of parsed vxcnn"
+
+    assert output[1]["vkl"] == [0.0000, 0.0000, 0.0000], "vkl (ik=1)"
+    assert output[2]["vkl"] == [0.0000, 0.0000, 0.5000], "vkl (ik=2)"
+    assert output[3]["vkl"] == [0.0000, 0.5000, 0.5000], "vkl (ik=3)"
+
+    assert output[1]["v_xc_nn"].shape == (11, 2), "Expect V_xc to have 2 cols for 11 states"
+    assert output[2]["v_xc_nn"].shape == (11, 2), "Expect V_xc to have 2 cols for 11 states"
+    assert output[3]["v_xc_nn"].shape == (11, 2), "Expect V_xc to have 2 cols for 11 states"
+
+    assert np.allclose(output[1]["v_xc_nn"], v_xc_1), "v_xc_nn for ik=1"
+    assert np.allclose(output[2]["v_xc_nn"], v_xc_2), "v_xc_nn for ik=2"
+    assert np.allclose(output[3]["v_xc_nn"], v_xc_3), "v_xc_nn for ik=3"
```

### Comparing `excitingtools-1.7.0/tests/dict_parsers/test_input_parser.py` & `excitingtools-1.7.1/tests/dict_parsers/test_input_parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Test for the input.xml file parser
 """
+
 import pytest
 
-from excitingtools.exciting_dict_parsers.input_parser import parse_element_xml, parse_structure, parse_input_xml
+from excitingtools.exciting_dict_parsers.input_parser import parse_element_xml, parse_input_xml, parse_structure
 
 reference_input_str = """<?xml version="1.0" encoding="UTF-8"?>
 <input sharedfs="true" 
   xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
   xsi:noNamespaceSchemaLocation="https://xml.exciting-code.org/excitinginput.xsd">
   
   <title>Lithium Fluoride BSE</title>
@@ -98,81 +99,79 @@
 def test_parse_keywords():
     assert parse_element_xml(reference_input_str, tag="keywords") == "keyword1 keyword2"
 
 
 def test_parse_groundstate():
     ground_state = parse_element_xml(reference_input_str, tag="groundstate")
     assert ground_state == {
-        'xctype': 'GGA_PBE', 'ngridk': [4, 4, 4],
-        'epsengy': 1e-7, 'outputlevel': 'high',
-        'spin': {'bfieldc': [0, 0, 0], 'fixspin': 'total FSM'},
-        'OEP': {'maxitoep': 100}
+        "xctype": "GGA_PBE",
+        "ngridk": [4, 4, 4],
+        "epsengy": 1e-7,
+        "outputlevel": "high",
+        "spin": {"bfieldc": [0, 0, 0], "fixspin": "total FSM"},
+        "OEP": {"maxitoep": 100},
     }
 
 
 def test_parse_groundstate_from_gs_root():
-    ground_state = parse_element_xml('<groundstate xctype="GGA_PBE" ngridk="4 4 4" epsengy="1d-7" outputlevel="high"/>',
-                                     tag="groundstate")
-    assert ground_state == {
-        'xctype': 'GGA_PBE', 'ngridk': [4, 4, 4],
-        'epsengy': 1e-7, 'outputlevel': 'high'
-    }
+    ground_state = parse_element_xml(
+        '<groundstate xctype="GGA_PBE" ngridk="4 4 4" epsengy="1d-7" outputlevel="high"/>', tag="groundstate"
+    )
+    assert ground_state == {"xctype": "GGA_PBE", "ngridk": [4, 4, 4], "epsengy": 1e-7, "outputlevel": "high"}
 
 
 def test_parse_structure():
     structure = parse_structure(reference_input_str)
     structure_ref = {
-        'atoms': [{'species': 'Li', 'position': [0.0, 0.0, 0.0],
-                   'bfcmt': [0.0, 0.0, 0.0]},
-                  {'species': 'F', 'position': [0.5, 0.5, 0.5],
-                   'lockxyz': [False, True, False]}],
-        'lattice': [[3.80402, 3.80402, 0.0],
-                    [3.80402, 0.0, 3.80402],
-                    [0.0, 3.80402, 3.80402]],
-        'species_path': '.',
-        'crystal_properties': {'scale': 1.0, 'stretch': [1.0, 1.0, 1.0]},
-        'species_properties': {'F': {'LDAplusU': {'J': 2.3, 'U': 0.5, 'l': 3}},
-                               'Li': {'dfthalfparam': {'ampl': 1,
-                                                       'cut': 3.9,
-                                                       'exponent': 8,
-                                                       'shell': [{'ionization': 0.25,
-                                                                 'number': 0}]},
-                                      'rmt': 1.5}},
-        'autormt': False,
-        'epslat': 1.0e-6,
+        "atoms": [
+            {"species": "Li", "position": [0.0, 0.0, 0.0], "bfcmt": [0.0, 0.0, 0.0]},
+            {"species": "F", "position": [0.5, 0.5, 0.5], "lockxyz": [False, True, False]},
+        ],
+        "lattice": [[3.80402, 3.80402, 0.0], [3.80402, 0.0, 3.80402], [0.0, 3.80402, 3.80402]],
+        "species_path": ".",
+        "crystal_properties": {"scale": 1.0, "stretch": [1.0, 1.0, 1.0]},
+        "species_properties": {
+            "F": {"LDAplusU": {"J": 2.3, "U": 0.5, "l": 3}},
+            "Li": {
+                "dfthalfparam": {"ampl": 1, "cut": 3.9, "exponent": 8, "shell": [{"ionization": 0.25, "number": 0}]},
+                "rmt": 1.5,
+            },
+        },
+        "autormt": False,
+        "epslat": 1.0e-6,
     }
     assert structure_ref == structure
 
 
 def test_parse_xs():
     xs = parse_element_xml(reference_input_str, tag="xs")
     xs_ref = {
-        'xstype': 'BSE',
-        'ngridq': [3, 3, 3],
-        'vkloff': [0.05, 0.15, 0.25],
-        'nempty': 1,
-        'broad': 0.0073499,
-        'nosym': True,
-        'energywindow': {'intv': [0.0, 1.0], 'points': 50},
-        'screening': {'screentype': 'full', 'nempty': 115},
-        'BSE': {'bsetype': 'singlet', 'nstlbse': [1, 5, 1, 2], 'aresbse': False},
-        'qpointset': [[0.0, 0.0, 0.0]],
-        'plan': ['screen', 'bse']
+        "xstype": "BSE",
+        "ngridq": [3, 3, 3],
+        "vkloff": [0.05, 0.15, 0.25],
+        "nempty": 1,
+        "broad": 0.0073499,
+        "nosym": True,
+        "energywindow": {"intv": [0.0, 1.0], "points": 50},
+        "screening": {"screentype": "full", "nempty": 115},
+        "BSE": {"bsetype": "singlet", "nstlbse": [1, 5, 1, 2], "aresbse": False},
+        "qpointset": [[0.0, 0.0, 0.0]],
+        "plan": ["screen", "bse"],
     }
     assert xs_ref == xs
     assert isinstance(xs["ngridq"][0], int)
 
 
-input_ref_parsed_keys = {'title', 'groundstate', 'structure', 'xs', 'sharedfs', "properties", "keywords"}
+input_ref_parsed_keys = {"title", "groundstate", "structure", "xs", "sharedfs", "properties", "keywords"}
 
 
 def test_parse_input_xml():
     parsed_data = parse_element_xml(reference_input_str)
     assert set(parsed_data.keys()) == input_ref_parsed_keys
-    assert parsed_data['sharedfs']
+    assert parsed_data["sharedfs"]
 
 
 def test_parse_input_xml_directly():
     parsed_data = parse_input_xml(reference_input_str)
     assert set(parsed_data.keys()) == input_ref_parsed_keys
 
 
@@ -185,20 +184,24 @@
     parsed_data = parse_element_xml(reference_input_str, tag="input")
     assert set(parsed_data.keys()) == input_ref_parsed_keys
 
 
 def test_parse_properties():
     properties = parse_element_xml(reference_input_str, tag="properties")
     properties_ref = {
-        'dos': {"nsmdos": 2, "ngrdos": 300, "nwdos": 1000, "winddos": [-0.3, 0.3]},
-        'bandstructure': {"plot1d": {"path": {
-            "steps": 100,
-            "point":
-                [
-                    {"coord": [1, 0, 0], "label": "Gamma"},
-                    {"coord": [0.625, 0.375, 0], "label": "K"},
-                    {"coord": [0.5, 0.5, 0], "label": "X", "breakafter": True},
-                    {"coord": [0, 0, 0], "label": "Gamma"},
-                    {"coord": [0.5, 0, 0], "label": "L"}
-                ]}}}
+        "dos": {"nsmdos": 2, "ngrdos": 300, "nwdos": 1000, "winddos": [-0.3, 0.3]},
+        "bandstructure": {
+            "plot1d": {
+                "path": {
+                    "steps": 100,
+                    "point": [
+                        {"coord": [1, 0, 0], "label": "Gamma"},
+                        {"coord": [0.625, 0.375, 0], "label": "K"},
+                        {"coord": [0.5, 0.5, 0], "label": "X", "breakafter": True},
+                        {"coord": [0, 0, 0], "label": "Gamma"},
+                        {"coord": [0.5, 0, 0], "label": "L"},
+                    ],
+                }
+            }
+        },
     }
     assert properties_ref == properties
```

### Comparing `excitingtools-1.7.0/tests/dict_parsers/test_parser_factory.py` & `excitingtools-1.7.1/tests/dict_parsers/test_parser_factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,18 @@
     assert_allclose(parsed_data["im"], [0.0, 0.0])
     assert_allclose(parsed_data["re"], [1.0, 0.0])
 
     file = tmp_path / "EPSILON_BSE-NAR_TDA-BAR_OC11.OUT"
     file.write_text("a\n" * 14 + "0 0 0 1\n0 0 0 2")
     parsed_data = parse(file.as_posix())
     assert set(parsed_data) == {
-        "frequency", "imag_oscillator_strength", "real_oscillator_strength", "real_oscillator_strength_kkt"
+        "frequency",
+        "imag_oscillator_strength",
+        "real_oscillator_strength",
+        "real_oscillator_strength_kkt",
     }
     assert_allclose(parsed_data["frequency"], [0.0, 0.0])
     assert_allclose(parsed_data["imag_oscillator_strength"], [0.0, 0.0])
     assert_allclose(parsed_data["real_oscillator_strength"], [0.0, 0.0])
     assert_allclose(parsed_data["real_oscillator_strength_kkt"], [1.0, 2.0])
 
     file = tmp_path / "Z_11.OUT"
```

### Comparing `excitingtools-1.7.0/tests/dict_parsers/test_properties_parser.py` & `excitingtools-1.7.1/tests/dict_parsers/test_properties_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import numpy as np
 
 from excitingtools.exciting_dict_parsers.properties_parser import parse_charge_density
 
-
 # Most of the values have been removed to shorten the test
 RHO1_xml = """<?xml version="1.0" encoding="UTF-8"?>
 <plot1d>
   <title>silicon-primitive-PBEsol</title>
   <grid>
     <axis label=" Distance" latexunit=" a_0" graceunit=" graceunit"/>
     <axis label=" Density" latexunit=" ???" graceunit=" graceunit"/>
@@ -20,16 +19,21 @@
     </function>
     <vertex distance="0.000000000" upperboundary="1985.188367" lowerboundary="0.8456287531E-01" label="" coord="0.000000000       0.000000000       0.000000000"/>
     <vertex distance="4.443235504" upperboundary="1985.188367" lowerboundary="0.8456287531E-01" label="" coord="0.2500000000      0.2500000000      0.2500000000"/>
   </grid>
 </plot1d>
 """
 
+
 def test_parse_charge_density():
     rho1 = parse_charge_density(RHO1_xml)
-    ref = np.array([[0.00000000e+00, 1.98518837e+03],
-                    [4.48811667e-02, 5.08882988e+02],
-                    [8.97623334e-02, 1.51827164e+02],
-                    [1.34643500e-01, 5.22636138e+01],
-                    [1.79524667e-01, 2.43321622e+01],
-                    [2.24405834e-01, 1.59499145e+01]])
-    assert np.allclose(rho1, ref, atol=1.e-8)
+    ref = np.array(
+        [
+            [0.00000000e00, 1.98518837e03],
+            [4.48811667e-02, 5.08882988e02],
+            [8.97623334e-02, 1.51827164e02],
+            [1.34643500e-01, 5.22636138e01],
+            [1.79524667e-01, 2.43321622e01],
+            [2.24405834e-01, 1.59499145e01],
+        ]
+    )
+    assert np.allclose(rho1, ref, atol=1.0e-8)
```

### Comparing `excitingtools-1.7.0/tests/dict_parsers/test_species_parser.py` & `excitingtools-1.7.1/tests/dict_parsers/test_species_parser.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,117 +1,193 @@
 from excitingtools.exciting_dict_parsers.species_parser import parse_species_xml
 
 
 def test_parse_species_xml():
-    """ Test parsing of species.xml files.
-    """
-    assert isinstance(species_str, str), (
-        "Expect species parser to handle strings of XML data, "
-        "due to use of decorator"
-    )
+    """Test parsing of species.xml files."""
+    assert isinstance(species_str, str), "Expect species parser to handle strings of XML data, due to use of decorator"
 
     species_dict = parse_species_xml(species_str)
 
-    assert set(species_dict) == {'species', 'muffin_tin', 'atomic_states', 'basis'}, 'Top level species file keys'
-    assert species_dict['species'] == {
-        'chemicalSymbol': 'Zn', 'name': 'zinc', 'z': -30.0, 'mass': 119198.678
-    }
-    assert species_dict['muffin_tin'] == {
-        'rmin': 1e-06, 'radius': 2.0, 'rinf': 21.8982, 'radialmeshPoints': 600.0
-    }
-
-    assert isinstance(species_dict['atomic_states'], list), 'Atomic states stored as a list'
-    atomic_states = [{'n': 1, 'l': 0, 'kappa': 1, 'occ': 2.00000,
-                      'core': True}, {'n': 2, 'l': 0, 'kappa': 1, 'occ': 2.00000, 'core': True},
-                     {'n': 2, 'l': 1, 'kappa': 1, 'occ': 2.00000,
-                      'core': True}, {'n': 2, 'l': 1, 'kappa': 2, 'occ': 4.00000, 'core': True},
-                     {'n': 3, 'l': 0, 'kappa': 1, 'occ': 2.00000,
-                      'core': False}, {'n': 3, 'l': 1, 'kappa': 1, 'occ': 2.00000, 'core': False},
-                     {'n': 3, 'l': 1, 'kappa': 2, 'occ': 4.00000,
-                      'core': False}, {'n': 3, 'l': 2, 'kappa': 2, 'occ': 4.00000, 'core': False},
-                     {'n': 3, 'l': 2, 'kappa': 3, 'occ': 6.00000,
-                      'core': False}, {'n': 4, 'l': 0, 'kappa': 1, 'occ': 2.00000, 'core': False}]
-    assert species_dict['atomic_states'] == atomic_states
+    assert set(species_dict) == {"species", "muffin_tin", "atomic_states", "basis"}, "Top level species file keys"
+    assert species_dict["species"] == {"chemicalSymbol": "Zn", "name": "zinc", "z": -30.0, "mass": 119198.678}
+    assert species_dict["muffin_tin"] == {"rmin": 1e-06, "radius": 2.0, "rinf": 21.8982, "radialmeshPoints": 600.0}
+
+    assert isinstance(species_dict["atomic_states"], list), "Atomic states stored as a list"
+    atomic_states = [
+        {"n": 1, "l": 0, "kappa": 1, "occ": 2.00000, "core": True},
+        {"n": 2, "l": 0, "kappa": 1, "occ": 2.00000, "core": True},
+        {"n": 2, "l": 1, "kappa": 1, "occ": 2.00000, "core": True},
+        {"n": 2, "l": 1, "kappa": 2, "occ": 4.00000, "core": True},
+        {"n": 3, "l": 0, "kappa": 1, "occ": 2.00000, "core": False},
+        {"n": 3, "l": 1, "kappa": 1, "occ": 2.00000, "core": False},
+        {"n": 3, "l": 1, "kappa": 2, "occ": 4.00000, "core": False},
+        {"n": 3, "l": 2, "kappa": 2, "occ": 4.00000, "core": False},
+        {"n": 3, "l": 2, "kappa": 3, "occ": 6.00000, "core": False},
+        {"n": 4, "l": 0, "kappa": 1, "occ": 2.00000, "core": False},
+    ]
+    assert species_dict["atomic_states"] == atomic_states
 
-    basis = species_dict['basis']
-    assert set(basis) == {'default', 'custom', 'lo'}, 'Keys for basis'
+    basis = species_dict["basis"]
+    assert set(basis) == {"default", "custom", "lo"}, "Keys for basis"
 
-    assert basis['default'] == [{'type': 'lapw', 'trialEnergy': 0.1500, 'searchE': True}]
+    assert basis["default"] == [{"type": "lapw", "trialEnergy": 0.1500, "searchE": True}]
 
     # Custom apw, lapw or apw+lo
-    assert basis['custom'] == [
-        {'l': 0, 'type': 'lapw', 'trialEnergy': 1.35670550183736, 'searchE': False},
-        {'l': 1, 'type': 'lapw', 'trialEnergy': -2.69952312512447,
-         'searchE': False}, {'l': 2, 'type': 'lapw', 'trialEnergy': 0.00, 'searchE': False},
-        {'l': 3, 'type': 'lapw', 'trialEnergy': 1.000,
-         'searchE': False}, {'l': 4, 'type': 'lapw', 'trialEnergy': 1.000, 'searchE': False},
-        {'l': 5, 'type': 'lapw', 'trialEnergy': 1.000, 'searchE': False}
+    assert basis["custom"] == [
+        {"l": 0, "type": "lapw", "trialEnergy": 1.35670550183736, "searchE": False},
+        {"l": 1, "type": "lapw", "trialEnergy": -2.69952312512447, "searchE": False},
+        {"l": 2, "type": "lapw", "trialEnergy": 0.00, "searchE": False},
+        {"l": 3, "type": "lapw", "trialEnergy": 1.000, "searchE": False},
+        {"l": 4, "type": "lapw", "trialEnergy": 1.000, "searchE": False},
+        {"l": 5, "type": "lapw", "trialEnergy": 1.000, "searchE": False},
     ]
 
     # All explicitly specified LOs
-    los = [{'l': 0, 'wf': [{'matchingOrder': 0, 'searchE': False, 'trialEnergy': -4.37848525995355},
-                           {'matchingOrder': 1, 'searchE': False, 'trialEnergy': -4.37848525995355}]},
-           {'l': 0, 'wf': [{'matchingOrder': 0, 'searchE': False, 'trialEnergy': 1.35670550183736},
-                           {'matchingOrder': 1, 'searchE': False, 'trialEnergy': 1.35670550183736}]},
-           {'l': 0, 'wf': [{'matchingOrder': 0, 'searchE': False, 'trialEnergy': 1.35670550183736},
-                           {'matchingOrder': 0, 'searchE': False, 'trialEnergy': -4.37848525995355}]},
-           {'l': 0, 'wf': [{'matchingOrder': 1, 'searchE': False, 'trialEnergy': 1.35670550183736},
-                           {'matchingOrder': 2, 'searchE': False, 'trialEnergy': 1.35670550183736}]},
-           {'l': 1, 'wf': [{'matchingOrder': 0, 'searchE': False, 'trialEnergy': -2.69952312512447},
-                           {'matchingOrder': 1, 'searchE': False, 'trialEnergy': -2.69952312512447}]},
-           {'l': 1, 'wf': [{'matchingOrder': 1, 'searchE': False, 'trialEnergy': -2.69952312512447},
-                           {'matchingOrder': 2, 'searchE': False, 'trialEnergy': -2.69952312512447}]},
-           {'l': 2, 'wf': [{'matchingOrder': 0, 'searchE': False, 'trialEnergy': 0.0},
-                           {'matchingOrder': 1, 'searchE': False, 'trialEnergy': 0.0}]},
-           {'l': 2, 'wf': [{'matchingOrder': 1, 'searchE': False, 'trialEnergy': 0.0},
-                           {'matchingOrder': 2, 'searchE': False, 'trialEnergy': 0.0}]},
-           {'l': 3, 'wf': [{'matchingOrder': 0, 'searchE': False, 'trialEnergy': 1.0},
-                           {'matchingOrder': 1, 'searchE': False, 'trialEnergy': 1.0}]},
-           {'l': 3, 'wf': [{'matchingOrder': 1, 'searchE': False, 'trialEnergy': 1.0},
-                           {'matchingOrder': 2, 'searchE': False, 'trialEnergy': 1.0}]},
-           {'l': 4, 'wf': [{'matchingOrder': 0, 'searchE': False, 'trialEnergy': 1.0},
-                           {'matchingOrder': 1, 'searchE': False, 'trialEnergy': 1.0}]},
-           {'l': 4, 'wf': [{'matchingOrder': 1, 'searchE': False, 'trialEnergy': 1.0},
-                           {'matchingOrder': 2, 'searchE': False, 'trialEnergy': 1.0}]},
-           {'l': 5, 'wf': [{'matchingOrder': 0, 'searchE': False, 'trialEnergy': 1.0},
-                           {'matchingOrder': 1, 'searchE': False, 'n': 5}]},
-           {'l': 5, 'wf': [{'matchingOrder': 1, 'n': 5, 'searchE': False},
-                           {'matchingOrder': 2, 'n': 6, 'searchE': False}]}]
-    
-    assert len(basis['lo']) == 14, "Number of explicitly-defined local orbitals"
-    assert set(basis['lo'][0]) == {'l', 'wf'}, "Attributes defining a local orbital"
-    assert basis['lo'] == los
+    los = [
+        {
+            "l": 0,
+            "wf": [
+                {"matchingOrder": 0, "searchE": False, "trialEnergy": -4.37848525995355},
+                {"matchingOrder": 1, "searchE": False, "trialEnergy": -4.37848525995355},
+            ],
+        },
+        {
+            "l": 0,
+            "wf": [
+                {"matchingOrder": 0, "searchE": False, "trialEnergy": 1.35670550183736},
+                {"matchingOrder": 1, "searchE": False, "trialEnergy": 1.35670550183736},
+            ],
+        },
+        {
+            "l": 0,
+            "wf": [
+                {"matchingOrder": 0, "searchE": False, "trialEnergy": 1.35670550183736},
+                {"matchingOrder": 0, "searchE": False, "trialEnergy": -4.37848525995355},
+            ],
+        },
+        {
+            "l": 0,
+            "wf": [
+                {"matchingOrder": 1, "searchE": False, "trialEnergy": 1.35670550183736},
+                {"matchingOrder": 2, "searchE": False, "trialEnergy": 1.35670550183736},
+            ],
+        },
+        {
+            "l": 1,
+            "wf": [
+                {"matchingOrder": 0, "searchE": False, "trialEnergy": -2.69952312512447},
+                {"matchingOrder": 1, "searchE": False, "trialEnergy": -2.69952312512447},
+            ],
+        },
+        {
+            "l": 1,
+            "wf": [
+                {"matchingOrder": 1, "searchE": False, "trialEnergy": -2.69952312512447},
+                {"matchingOrder": 2, "searchE": False, "trialEnergy": -2.69952312512447},
+            ],
+        },
+        {
+            "l": 2,
+            "wf": [
+                {"matchingOrder": 0, "searchE": False, "trialEnergy": 0.0},
+                {"matchingOrder": 1, "searchE": False, "trialEnergy": 0.0},
+            ],
+        },
+        {
+            "l": 2,
+            "wf": [
+                {"matchingOrder": 1, "searchE": False, "trialEnergy": 0.0},
+                {"matchingOrder": 2, "searchE": False, "trialEnergy": 0.0},
+            ],
+        },
+        {
+            "l": 3,
+            "wf": [
+                {"matchingOrder": 0, "searchE": False, "trialEnergy": 1.0},
+                {"matchingOrder": 1, "searchE": False, "trialEnergy": 1.0},
+            ],
+        },
+        {
+            "l": 3,
+            "wf": [
+                {"matchingOrder": 1, "searchE": False, "trialEnergy": 1.0},
+                {"matchingOrder": 2, "searchE": False, "trialEnergy": 1.0},
+            ],
+        },
+        {
+            "l": 4,
+            "wf": [
+                {"matchingOrder": 0, "searchE": False, "trialEnergy": 1.0},
+                {"matchingOrder": 1, "searchE": False, "trialEnergy": 1.0},
+            ],
+        },
+        {
+            "l": 4,
+            "wf": [
+                {"matchingOrder": 1, "searchE": False, "trialEnergy": 1.0},
+                {"matchingOrder": 2, "searchE": False, "trialEnergy": 1.0},
+            ],
+        },
+        {
+            "l": 5,
+            "wf": [
+                {"matchingOrder": 0, "searchE": False, "trialEnergy": 1.0},
+                {"matchingOrder": 1, "searchE": False, "n": 5},
+            ],
+        },
+        {
+            "l": 5,
+            "wf": [{"matchingOrder": 1, "n": 5, "searchE": False}, {"matchingOrder": 2, "n": 6, "searchE": False}],
+        },
+    ]
+
+    assert len(basis["lo"]) == 14, "Number of explicitly-defined local orbitals"
+    assert set(basis["lo"][0]) == {"l", "wf"}, "Attributes defining a local orbital"
+    assert basis["lo"] == los
 
 
 def test_parse_species_xml_different_ordering():
     species_dict = parse_species_xml(species_str_diff_order)
 
-    assert set(species_dict) == {'species', 'muffin_tin', 'atomic_states', 'basis'}, 'Top level species file keys'
+    assert set(species_dict) == {"species", "muffin_tin", "atomic_states", "basis"}, "Top level species file keys"
 
     # References
-    ref_species = {'chemicalSymbol': 'C', 'name': 'carbon', 'z': -6.0, 'mass': 21894.16673}
-    ref_muffin_tin = {'rmin': 1e-05, 'radius': 1.45, 'rinf': 21.0932, 'radialmeshPoints': 250.0}
-    ref_atomic_states = [{'n': 1, 'l': 0, 'kappa': 1, 'occ': 2.0, 'core': False},
-                         {'n': 2, 'l': 0, 'kappa': 1, 'occ': 2.0, 'core': False},
-                         {'n': 2, 'l': 1, 'kappa': 1, 'occ': 1.0, 'core': False},
-                         {'n': 2, 'l': 1, 'kappa': 2, 'occ': 1.0, 'core': False}]
-    ref_basis = {'default': [{'type': 'lapw', 'trialEnergy': 0.15, 'searchE': False}],
-                 'custom': [{'l': 0, 'type': 'apw+lo', 'trialEnergy': 0.15, 'searchE': True},
-                            {'l': 1, 'type': 'apw+lo', 'trialEnergy': 0.15, 'searchE': True}],
-                 'lo': [{'l': 0, 'wfproj': False,
-                         'wf': [{'matchingOrder': 0, 'trialEnergy': 0.15, 'searchE': True},
-                                {'matchingOrder': 1, 'trialEnergy': 0.15, 'searchE': True},
-                                {'matchingOrder': 0, 'trialEnergy': -9.8, 'searchE': False}]}]}
-    
-    assert species_dict['species'] == ref_species, "species data disagrees"
-    assert species_dict['muffin_tin'] == ref_muffin_tin, "muffin tin data disagrees"
-    assert species_dict['atomic_states'] == ref_atomic_states, "atomic state data disagrees"
-    assert species_dict['basis']['default'] == ref_basis['default'], "basis default data disagrees"
-    assert species_dict['basis']['custom'] == ref_basis['custom'], "basis custom data disagrees"
-    assert species_dict['basis']['lo'] == ref_basis['lo'], "basis lo data disagrees"
+    ref_species = {"chemicalSymbol": "C", "name": "carbon", "z": -6.0, "mass": 21894.16673}
+    ref_muffin_tin = {"rmin": 1e-05, "radius": 1.45, "rinf": 21.0932, "radialmeshPoints": 250.0}
+    ref_atomic_states = [
+        {"n": 1, "l": 0, "kappa": 1, "occ": 2.0, "core": False},
+        {"n": 2, "l": 0, "kappa": 1, "occ": 2.0, "core": False},
+        {"n": 2, "l": 1, "kappa": 1, "occ": 1.0, "core": False},
+        {"n": 2, "l": 1, "kappa": 2, "occ": 1.0, "core": False},
+    ]
+    ref_basis = {
+        "default": [{"type": "lapw", "trialEnergy": 0.15, "searchE": False}],
+        "custom": [
+            {"l": 0, "type": "apw+lo", "trialEnergy": 0.15, "searchE": True},
+            {"l": 1, "type": "apw+lo", "trialEnergy": 0.15, "searchE": True},
+        ],
+        "lo": [
+            {
+                "l": 0,
+                "wfproj": False,
+                "wf": [
+                    {"matchingOrder": 0, "trialEnergy": 0.15, "searchE": True},
+                    {"matchingOrder": 1, "trialEnergy": 0.15, "searchE": True},
+                    {"matchingOrder": 0, "trialEnergy": -9.8, "searchE": False},
+                ],
+            }
+        ],
+    }
+
+    assert species_dict["species"] == ref_species, "species data disagrees"
+    assert species_dict["muffin_tin"] == ref_muffin_tin, "muffin tin data disagrees"
+    assert species_dict["atomic_states"] == ref_atomic_states, "atomic state data disagrees"
+    assert species_dict["basis"]["default"] == ref_basis["default"], "basis default data disagrees"
+    assert species_dict["basis"]["custom"] == ref_basis["custom"], "basis custom data disagrees"
+    assert species_dict["basis"]["lo"] == ref_basis["lo"], "basis lo data disagrees"
 
 
 species_str = """<?xml version="1.0" encoding="utf-8"?>
 <spdb xsi:noNamespaceSchemaLocation="../../xml/species.xsd" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
   <sp chemicalSymbol="Zn" name="zinc" z="-30.0000" mass="119198.6780">
     <muffinTin rmin="0.100000E-05" radius="2.0000" rinf="21.8982" radialmeshPoints="600"/>
     <atomicState n="1" l="0" kappa="1" occ="2.00000" core="true"/>
```

### Comparing `excitingtools-1.7.0/tests/dict_parsers/test_state_parser.py` & `excitingtools-1.7.1/tests/dict_parsers/test_state_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,52 +1,54 @@
-from excitingtools.exciting_dict_parsers.state_parser import parse_state_out
+import sys
 from pathlib import Path
+
 import numpy as np
-import sys
+
+from excitingtools.exciting_dict_parsers.state_parser import parse_state_out
 
 
 def write_int(file, i: int, byteorder):
-    """ Writes an integer as bytes to the file.
+    """Writes an integer as bytes to the file.
 
     :param file: file object to write the int
     :param i: integer, which bytes should be written
     :param byteorder: endianness of the byteorder ("little" or "big")
     """
     file.write(int.to_bytes(4, 4, byteorder))
     file.write(i.to_bytes(4, byteorder))
     file.write(int.to_bytes(4, 4, byteorder))
 
 
 def write_array(file, a: np.ndarray, byteorder):
-    """ Writes a numpy array to the file as bytes.
+    """Writes a numpy array to the file as bytes.
 
     :param file: file object to write the int
     :param a: numpy array, which bytes should be written
     :param byteorder: endianness of the byteorder ("little" or "big")
     """
     num_bytes = a.size * 8
     file.write(num_bytes.to_bytes(4, byteorder))
-    file.write(a.tobytes(order='F'))
+    file.write(a.tobytes(order="F"))
     file.write(num_bytes.to_bytes(4, byteorder))
 
 
 def write_state(path, state: dict):
-    """ Creates a file at the specified path and writes the dictionary in the same structure as STATE.OUT
+    """Creates a file at the specified path and writes the dictionary in the same structure as STATE.OUT
 
     :param path: path to the file to which should be written to
     :param state: state dictionary, which should be converted to a binary STATE file
     """
     byteorder = sys.byteorder
     with open(path, "wb+") as file:
         # write version information
         file.write(int.to_bytes(52, 4, byteorder))
         for i in state["version"]:
             i: int
             file.write(i.to_bytes(4, byteorder))
-        file.write("YomNFS0t4s8uhGxs4FCNGsAOp5DapSm7HAQ58aVd".encode("utf-8"))
+        file.write(b"YomNFS0t4s8uhGxs4FCNGsAOp5DapSm7HAQ58aVd")
         file.write(int.to_bytes(52, 4, byteorder))
         # write other general information
         for key in ("spinpol", "nspecies", "lmmaxvr", "nrmtmax"):
             write_int(file, state[key], byteorder)
         # next write the species specific information
         for i in range(state["nspecies"]):
             write_int(file, state["number of atoms"][i], byteorder)
@@ -63,36 +65,39 @@
         # next write the array pairs
         arrays = (
             ("muffintin density", "interstitial density"),
             ("muffintin coulomb potential", "interstitial coulomb potential"),
             ("muffintin exchange-correlation potential", "interstitial exchange-correlation potential"),
         )
         for muffintin_array, interstitial_array in arrays:
-            muffintin_array: np.ndarray = state[muffintin_array]
-            interstitial_array: np.ndarray = state[interstitial_array]
-            num_bytes = (muffintin_array.size + interstitial_array.size) * 8
+            muffintin_array_state: np.ndarray = state[muffintin_array]
+            interstitial_array_state: np.ndarray = state[interstitial_array]
+            num_bytes = (muffintin_array_state.size + interstitial_array_state.size) * 8
             file.write(num_bytes.to_bytes(4, byteorder))
-            file.write(muffintin_array.tobytes(order='F'))
-            file.write(interstitial_array.tobytes(order='F'))
+            file.write(muffintin_array_state.tobytes(order="F"))
+            file.write(interstitial_array_state.tobytes(order="F"))
             file.write(num_bytes.to_bytes(4, byteorder))
         # Lastly write the potential arrays
-        num_bytes = 8 * (state["muffintin effective potential"].size + state["interstitial effective potential"].size +
-                         2 * state["reciprocal interstitial effective potential"].size)
+        num_bytes = 8 * (
+            state["muffintin effective potential"].size
+            + state["interstitial effective potential"].size
+            + 2 * state["reciprocal interstitial effective potential"].size
+        )
         file.write(num_bytes.to_bytes(4, byteorder))
-        file.write(state["muffintin effective potential"].tobytes(order='F'))
-        file.write(state["interstitial effective potential"].tobytes(order='F'))
-        file.write(state["reciprocal interstitial effective potential"].tobytes(order='F'))
+        file.write(state["muffintin effective potential"].tobytes(order="F"))
+        file.write(state["interstitial effective potential"].tobytes(order="F"))
+        file.write(state["reciprocal interstitial effective potential"].tobytes(order="F"))
         file.write(num_bytes.to_bytes(4, byteorder))
 
 
 def test_parse_state_out(tmp_path: Path):
     directory = tmp_path
 
     # setting seed to avoid randomness in tests
-    np.random.seed(0)
+    rng = np.random.default_rng(0)
 
     state_ref = {
         "version": (1, 2, 3),
         "versionhash": "YomNFS0t4s8uhGxs4FCNGsAOp5DapSm7HAQ58aVd",
         "spinpol": False,
         "nspecies": 2,
         "lmmaxvr": 3,
@@ -101,23 +106,23 @@
         "muffintin radial meshes": [np.array([1.0, 2.0]), np.array([0.5, 0.75, 1.5])],
         "g vector grid": (2, 2, 2),
         "ngvec": 5,
         "ndmag": 0,
         "nspinor": 1,
         "ldapu": 0,
         "lmmaxlu": 16,
-        "muffintin density": np.random.random((3, 3, 2)),
-        "interstitial density": np.random.random(8),
-        "muffintin coulomb potential": np.random.random((3, 3, 2)),
-        "interstitial coulomb potential": np.random.random(8),
-        "muffintin exchange-correlation potential": np.random.random((3, 3, 2)),
-        "interstitial exchange-correlation potential": np.random.random(8),
-        "muffintin effective potential": np.random.random((3, 3, 2)),
-        "interstitial effective potential": np.random.random(8),
-        "reciprocal interstitial effective potential": np.random.random(5) + 1j * np.random.random(5),
+        "muffintin density": rng.random((3, 3, 2)),
+        "interstitial density": rng.random(8),
+        "muffintin coulomb potential": rng.random((3, 3, 2)),
+        "interstitial coulomb potential": rng.random(8),
+        "muffintin exchange-correlation potential": rng.random((3, 3, 2)),
+        "interstitial exchange-correlation potential": rng.random(8),
+        "muffintin effective potential": rng.random((3, 3, 2)),
+        "interstitial effective potential": rng.random(8),
+        "reciprocal interstitial effective potential": rng.random(5) + 1j * rng.random(5),
     }
     write_state(directory / "STATE.OUT", state_ref)
     state_out = parse_state_out(directory / "STATE.OUT")
 
     assert state_out["version"] == state_ref["version"]
     assert state_out["versionhash"] == state_ref["versionhash"]
     assert state_out["spinpol"] == state_ref["spinpol"]
@@ -133,15 +138,20 @@
     assert state_out["nspinor"] == state_ref["nspinor"]
     assert state_out["ldapu"] == state_ref["ldapu"]
     assert state_out["lmmaxlu"] == state_ref["lmmaxlu"]
     assert np.allclose(state_out["muffintin density"], state_ref["muffintin density"])
     assert np.allclose(state_out["interstitial density"], state_ref["interstitial density"])
     assert np.allclose(state_out["muffintin coulomb potential"], state_ref["muffintin coulomb potential"])
     assert np.allclose(state_out["interstitial coulomb potential"], state_ref["interstitial coulomb potential"])
-    assert np.allclose(state_out["muffintin exchange-correlation potential"],
-                       state_ref["muffintin exchange-correlation potential"])
-    assert np.allclose(state_out["interstitial exchange-correlation potential"],
-                       state_ref["interstitial exchange-correlation potential"])
+    assert np.allclose(
+        state_out["muffintin exchange-correlation potential"], state_ref["muffintin exchange-correlation potential"]
+    )
+    assert np.allclose(
+        state_out["interstitial exchange-correlation potential"],
+        state_ref["interstitial exchange-correlation potential"],
+    )
     assert np.allclose(state_out["muffintin effective potential"], state_ref["muffintin effective potential"])
     assert np.allclose(state_out["interstitial effective potential"], state_ref["interstitial effective potential"])
-    assert np.allclose(state_out["reciprocal interstitial effective potential"],
-                       state_ref["reciprocal interstitial effective potential"])
+    assert np.allclose(
+        state_out["reciprocal interstitial effective potential"],
+        state_ref["reciprocal interstitial effective potential"],
+    )
```

### Comparing `excitingtools-1.7.0/tests/eigenstates/test_eigenstates.py` & `excitingtools-1.7.1/tests/eigenstates/test_eigenstates.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,26 @@
-""" Test for get_index function in eigenstates.py
-"""
+"""Test for get_index function in eigenstates.py"""
 
-from excitingtools.eigenstates.eigenstates import get_k_point_index
-import pytest
-import numpy as np
 import re
 
+import numpy as np
+import pytest
+
+from excitingtools.eigenstates.eigenstates import get_k_point_index
+
 
 def test_get_k_point_index():
-    k_points = np.array([[1.000000, 0.000000, 0.000000],
-                         [0.988281, 0.011719, 0.000000],
-                         [0.988281, 0.011719, 0.000000],
-                         [0.976562, 0.023438, 0.000000],
-                         [0.953125, 0.046875, 0.000000]])
+    k_points = np.array(
+        [
+            [1.000000, 0.000000, 0.000000],
+            [0.988281, 0.011719, 0.000000],
+            [0.988281, 0.011719, 0.000000],
+            [0.976562, 0.023438, 0.000000],
+            [0.953125, 0.046875, 0.000000],
+        ]
+    )
 
     assert get_k_point_index([1.000000, 0.000000, 0.000000], k_points) == 0
     assert get_k_point_index([0.953125, 0.046875, 0.000000], k_points) == 4
     assert np.isnan(get_k_point_index([0.000000, 0.500000, 0.500000], k_points)), "No k-point matched"
     with pytest.raises(ValueError, match=re.escape("Found degenerate k-points at [[1], [2]]")):
         get_k_point_index([0.988281, 0.011719, 0.000000], k_points), "ValueError is returned for degenerate k-points"
```

### Comparing `excitingtools-1.7.0/tests/input/test_input_xml.py` & `excitingtools-1.7.1/tests/input/test_input_xml.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,154 +6,165 @@
 
 NOTE:
 All attribute tests should assert on the XML tree content's as the attribute
 order is not preserved by the ElementTree.tostring method. Elements appear to
 be fine.
 """
 
-import pytest
 import numpy as np
+import pytest
 
-from excitingtools.input.input_classes import ExcitingGroundStateInput, ExcitingXSInput, ExcitingKeywordsInput
+from excitingtools.input.input_classes import ExcitingGroundStateInput, ExcitingKeywordsInput, ExcitingXSInput
 from excitingtools.input.input_xml import ExcitingInputXML
 from excitingtools.input.structure import ExcitingStructure
 
 
 @pytest.fixture
 def exciting_structure() -> ExcitingStructure:
-    """ Initialise an exciting structure. """
+    """Initialise an exciting structure."""
     cubic_lattice = [[1.0, 0.0, 0.0], [0.0, 1.0, 0.0], [0.0, 0.0, 1.0]]
-    arbitrary_atoms = [{'species': 'Li', 'position': [0.0, 0.0, 0.0]},
-                       {'species': 'Li', 'position': [1.0, 0.0, 0.0]},
-                       {'species': 'F', 'position': [2.0, 0.0, 0.0]}]
+    arbitrary_atoms = [
+        {"species": "Li", "position": [0.0, 0.0, 0.0]},
+        {"species": "Li", "position": [1.0, 0.0, 0.0]},
+        {"species": "F", "position": [2.0, 0.0, 0.0]},
+    ]
 
-    return ExcitingStructure(arbitrary_atoms, cubic_lattice, '.')
+    return ExcitingStructure(arbitrary_atoms, cubic_lattice, ".")
 
 
 @pytest.fixture
 def exciting_input_xml(exciting_structure: ExcitingStructure) -> ExcitingInputXML:
-    """ Initialises a complete input file. """
+    """Initialises a complete input file."""
     ground_state = ExcitingGroundStateInput(
         rgkmax=8.0,
         do="fromscratch",
         ngridk=[6, 6, 6],
         xctype="GGA_PBE_SOL",
         vkloff=[0, 0, 0],
         tforce=True,
-        nosource=False
+        nosource=False,
     )
 
-    bse_attributes = {'bsetype': 'singlet', 'xas': True}
-    energywindow_attributes = {'intv': [5.8, 8.3], 'points': 5000}
-    screening_attributes = {'screentype': 'full', 'nempty': 15}
-    plan_input = ['screen', 'bse']
+    bse_attributes = {"bsetype": "singlet", "xas": True}
+    energywindow_attributes = {"intv": [5.8, 8.3], "points": 5000}
+    screening_attributes = {"screentype": "full", "nempty": 15}
+    plan_input = ["screen", "bse"]
     qpointset_input = [[0, 0, 0], [0.5, 0.5, 0.5]]
-    xs = ExcitingXSInput(xstype="BSE", broad=0.32, ngridk=[8, 8, 8],
-                         BSE=bse_attributes,
-                         energywindow=energywindow_attributes,
-                         screening=screening_attributes,
-                         qpointset=qpointset_input,
-                         plan=plan_input)
+    xs = ExcitingXSInput(
+        xstype="BSE",
+        broad=0.32,
+        ngridk=[8, 8, 8],
+        BSE=bse_attributes,
+        energywindow=energywindow_attributes,
+        screening=screening_attributes,
+        qpointset=qpointset_input,
+        plan=plan_input,
+    )
     keywords = ExcitingKeywordsInput("keyword1 keyword2 keyword3")
 
-    return ExcitingInputXML(sharedfs=True, structure=exciting_structure, title='Test Case', groundstate=ground_state,
-                            xs=xs, keywords=keywords)
+    return ExcitingInputXML(
+        sharedfs=True,
+        structure=exciting_structure,
+        title="Test Case",
+        groundstate=ground_state,
+        xs=xs,
+        keywords=keywords,
+    )
 
 
-def test_exciting_input_xml_structure_and_gs_and_xs(exciting_input_xml: ExcitingInputXML):
+def test_exciting_input_xml_structure_and_gs_and_xs(exciting_input_xml: ExcitingInputXML):  # noqa: PLR0915
     """Test the XML created for a ground state input is valid.
     Test SubTree composition using only mandatory attributes for each XML subtree.
     """
     input_xml_tree = exciting_input_xml.to_xml()
 
-    assert input_xml_tree.tag == 'input'
-    assert input_xml_tree.keys() == ['sharedfs']
+    assert input_xml_tree.tag == "input"
+    assert input_xml_tree.keys() == ["sharedfs"]
 
     subelements = list(input_xml_tree)
     assert len(subelements) == 5
 
     title_xml = subelements[0]
-    assert title_xml.tag == 'title'
+    assert title_xml.tag == "title"
     assert title_xml.keys() == []
-    assert title_xml.text == 'Test Case'
+    assert title_xml.text == "Test Case"
 
     structure_xml = subelements[1]
-    assert structure_xml.tag == 'structure'
-    assert structure_xml.keys() == ['speciespath']
+    assert structure_xml.tag == "structure"
+    assert structure_xml.keys() == ["speciespath"]
     assert len(list(structure_xml)) == 3
 
     groundstate_xml = subelements[2]
-    assert groundstate_xml.tag == 'groundstate'
-    assert groundstate_xml.text == ' '
-    assert groundstate_xml.keys() == \
-           ['rgkmax', 'do', 'ngridk', 'xctype', 'vkloff', 'tforce', 'nosource']
-    assert groundstate_xml.get('rgkmax') == "8.0"
-    assert groundstate_xml.get('do') == "fromscratch"
-    assert groundstate_xml.get('ngridk') == "6 6 6"
-    assert groundstate_xml.get('xctype') == "GGA_PBE_SOL"
-    assert groundstate_xml.get('vkloff') == "0 0 0"
-    assert groundstate_xml.get('tforce') == "true"
-    assert groundstate_xml.get('nosource') == "false"
+    assert groundstate_xml.tag == "groundstate"
+    assert groundstate_xml.text == " "
+    assert groundstate_xml.keys() == ["rgkmax", "do", "ngridk", "xctype", "vkloff", "tforce", "nosource"]
+    assert groundstate_xml.get("rgkmax") == "8.0"
+    assert groundstate_xml.get("do") == "fromscratch"
+    assert groundstate_xml.get("ngridk") == "6 6 6"
+    assert groundstate_xml.get("xctype") == "GGA_PBE_SOL"
+    assert groundstate_xml.get("vkloff") == "0 0 0"
+    assert groundstate_xml.get("tforce") == "true"
+    assert groundstate_xml.get("nosource") == "false"
 
     xs_xml = subelements[3]
-    assert xs_xml.tag == 'xs'
-    assert set(xs_xml.keys()) == {'broad', 'ngridk', 'xstype'}
-    assert xs_xml.get('broad') == '0.32'
-    assert xs_xml.get('ngridk') == '8 8 8'
-    assert xs_xml.get('xstype') == 'BSE'
+    assert xs_xml.tag == "xs"
+    assert set(xs_xml.keys()) == {"broad", "ngridk", "xstype"}
+    assert xs_xml.get("broad") == "0.32"
+    assert xs_xml.get("ngridk") == "8 8 8"
+    assert xs_xml.get("xstype") == "BSE"
 
     xs_subelements = list(xs_xml)
     assert len(xs_subelements) == 5
     valid_tags = {"screening", "BSE", "energywindow", "qpointset", "plan"}
     assert valid_tags == set(xs_subelement.tag for xs_subelement in xs_subelements)
 
     screening_xml = xs_xml.find("screening")
     assert screening_xml.tag == "screening"
-    assert screening_xml.keys() == ['screentype', 'nempty']
-    assert screening_xml.get('screentype') == 'full'
-    assert screening_xml.get('nempty') == '15'
+    assert screening_xml.keys() == ["screentype", "nempty"]
+    assert screening_xml.get("screentype") == "full"
+    assert screening_xml.get("nempty") == "15"
 
     bse_xml = xs_xml.find("BSE")
-    assert bse_xml.tag == 'BSE'
-    assert bse_xml.keys() == ['bsetype', 'xas']
-    assert bse_xml.get('bsetype') == 'singlet'
-    assert bse_xml.get('xas') == 'true'
+    assert bse_xml.tag == "BSE"
+    assert bse_xml.keys() == ["bsetype", "xas"]
+    assert bse_xml.get("bsetype") == "singlet"
+    assert bse_xml.get("xas") == "true"
 
     energywindow_xml = xs_xml.find("energywindow")
     assert energywindow_xml.tag == "energywindow"
-    assert energywindow_xml.keys() == ['intv', 'points']
-    assert energywindow_xml.get('intv') == '5.8 8.3'
-    assert energywindow_xml.get('points') == '5000'
+    assert energywindow_xml.keys() == ["intv", "points"]
+    assert energywindow_xml.get("intv") == "5.8 8.3"
+    assert energywindow_xml.get("points") == "5000"
 
     qpointset_xml = xs_xml.find("qpointset")
     assert qpointset_xml.tag == "qpointset"
     assert qpointset_xml.items() == []
     qpoints = list(qpointset_xml)
     assert len(qpoints) == 2
-    assert qpoints[0].tag == 'qpoint'
+    assert qpoints[0].tag == "qpoint"
     assert qpoints[0].items() == []
-    valid_qpoints = {'0 0 0', '0.5 0.5 0.5'}
+    valid_qpoints = {"0 0 0", "0.5 0.5 0.5"}
     assert qpoints[0].text in valid_qpoints
     valid_qpoints.discard(qpoints[0].text)
     assert qpoints[1].text in valid_qpoints
 
     plan_xml = xs_xml.find("plan")
     assert plan_xml.tag == "plan"
     assert plan_xml.items() == []
     doonlys = list(plan_xml)
     assert len(doonlys) == 2
-    assert doonlys[0].tag == 'doonly'
-    assert doonlys[0].items() == [('task', 'screen')]
-    assert doonlys[1].tag == 'doonly'
-    assert doonlys[1].items() == [('task', 'bse')]
+    assert doonlys[0].tag == "doonly"
+    assert doonlys[0].items() == [("task", "screen")]
+    assert doonlys[1].tag == "doonly"
+    assert doonlys[1].items() == [("task", "bse")]
 
     title_xml = subelements[4]
-    assert title_xml.tag == 'keywords'
+    assert title_xml.tag == "keywords"
     assert title_xml.keys() == []
-    assert title_xml.text == 'keyword1 keyword2 keyword3'
+    assert title_xml.text == "keyword1 keyword2 keyword3"
 
 
 def test_attribute_modification(exciting_input_xml: ExcitingInputXML):
     """Test the XML created for a ground state input is valid.
     Test SubTree composition using only mandatory attributes for each XML subtree.
     """
     exciting_input_xml.set_title("New Test Case")
@@ -162,68 +173,72 @@
     exciting_input_xml.xs.energywindow.points = 4000
     input_xml_tree = exciting_input_xml.to_xml()
 
     subelements = list(input_xml_tree)
     assert len(subelements) == 5
 
     title_xml = subelements[0]
-    assert title_xml.tag == 'title'
-    assert title_xml.text == 'New Test Case'
+    assert title_xml.tag == "title"
+    assert title_xml.text == "New Test Case"
 
     structure_xml = subelements[1]
     assert structure_xml[0].get("scale") == "2.3"
 
     groundstate_xml = subelements[2]
-    assert groundstate_xml.get('rgkmax') == "9.0"
+    assert groundstate_xml.get("rgkmax") == "9.0"
 
     xs_xml = subelements[3]
     xs_subelements = list(xs_xml)
     assert len(xs_subelements) == 5
 
     energywindow_xml = xs_xml.find("energywindow")
-    assert energywindow_xml.get('points') == '4000'
+    assert energywindow_xml.get("points") == "4000"
 
 
-def test_as_dict(exciting_input_xml: ExcitingInputXML, mock_env_jobflow_missing):
+@pytest.mark.usefixtures("mock_env_jobflow_missing")
+def test_as_dict(exciting_input_xml: ExcitingInputXML):
     dict_representation = exciting_input_xml.as_dict()
     assert set(dict_representation.keys()) == {"xml_string"}
     # check only that the xml string starts with the correct first lines:
-    assert dict_representation["xml_string"].startswith('<?xml version="1.0" ?>\n<input sharedfs="true">\n\t'
-                                                        '<title>Test Case</title>\n\t<structure')
+    assert dict_representation["xml_string"].startswith(
+        '<?xml version="1.0" ?>\n<input sharedfs="true">\n\t<title>Test Case</title>\n\t<structure'
+    )
 
 
-def test_as_dict_jobflow(exciting_input_xml: ExcitingInputXML, mock_env_jobflow):
+@pytest.mark.usefixtures("mock_env_jobflow")
+def test_as_dict_jobflow(exciting_input_xml: ExcitingInputXML):
     dict_representation = exciting_input_xml.as_dict()
     xml_string = dict_representation.pop("xml_string")
-    assert dict_representation == {'@class': 'ExcitingInputXML',
-                                   '@module': 'excitingtools.input.input_xml'}
+    assert dict_representation == {"@class": "ExcitingInputXML", "@module": "excitingtools.input.input_xml"}
     # check only that the xml string starts with the correct first lines:
-    assert xml_string.startswith('<?xml version="1.0" ?>\n<input sharedfs="true">\n\t'
-                                 '<title>Test Case</title>\n\t<structure')
+    assert xml_string.startswith(
+        '<?xml version="1.0" ?>\n<input sharedfs="true">\n\t<title>Test Case</title>\n\t<structure'
+    )
 
 
-def test_from_dict(exciting_input_xml: ExcitingInputXML, mock_env_jobflow_missing):
+@pytest.mark.usefixtures("mock_env_jobflow_missing")
+def test_from_dict(exciting_input_xml: ExcitingInputXML):
     new_input_xml = ExcitingInputXML.from_dict(exciting_input_xml.as_dict())
     assert new_input_xml.title.title == "Test Case"  # pylint: disable=no-member
     assert new_input_xml.groundstate.ngridk == [6, 6, 6]  # pylint: disable=no-member
 
 
-def test_from_dict_jobflow(exciting_input_xml: ExcitingInputXML, mock_env_jobflow):
+@pytest.mark.usefixtures("mock_env_jobflow")
+def test_from_dict_jobflow(exciting_input_xml: ExcitingInputXML):
     new_input_xml = ExcitingInputXML.from_dict(exciting_input_xml.as_dict())
     assert new_input_xml.title.title == "Test Case"  # pylint: disable=no-member
 
 
 def test_missing_structure():
     with pytest.raises(ValueError, match="Missing mandatory arguments: {'structure'}"):
         ExcitingInputXML(title="Test Case", groundstate=ExcitingGroundStateInput())
 
 
 def test_from_gs_dict(exciting_structure):
-    input_xml = ExcitingInputXML(structure=exciting_structure, title="Test Case",
-                                 groundstate={"rgkmax": 7.0})
+    input_xml = ExcitingInputXML(structure=exciting_structure, title="Test Case", groundstate={"rgkmax": 7.0})
     assert input_xml.title.title == "Test Case"  # pylint: disable=no-member
     assert input_xml.groundstate.rgkmax == 7.0  # pylint: disable=no-member
     assert input_xml.structure.speciespath == "."  # pylint: disable=no-member
 
 
 def test_from_xml():
     input_str = """<?xml version='1.0' encoding='utf-8'?>
@@ -246,16 +261,16 @@
         </groundstate>
     </input>"""
     input_xml = ExcitingInputXML.from_xml(input_str)
     assert input_xml.title.title == "BN (B3)"
 
     assert input_xml.structure.speciespath == "speciespath"
     assert input_xml.structure.autormt is True
-    assert input_xml.structure.species == ['B', 'N']
-    np.testing.assert_allclose(input_xml.structure.positions, [[0.] * 3, [0.25] * 3])
+    assert input_xml.structure.species == ["B", "N"]
+    np.testing.assert_allclose(input_xml.structure.positions, [[0.0] * 3, [0.25] * 3])
     np.testing.assert_allclose(input_xml.structure.lattice, np.full((3, 3), 0.5) - 0.5 * np.eye(3))
     assert input_xml.structure.crystal_properties.scale == pytest.approx(6.816242132875)
 
     assert input_xml.groundstate.outputlevel == "high"
     assert input_xml.groundstate.ngridk == [10, 10, 10]
     assert input_xml.groundstate.rgkmax == pytest.approx(7.0)
     assert input_xml.groundstate.maxscl == 200
```

### Comparing `excitingtools-1.7.0/tests/input/test_properties.py` & `excitingtools-1.7.1/tests/input/test_properties.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,58 @@
-""" Test properties.
+"""Test properties.
 
 NOTE:
 All attribute tests should assert on the XML tree content's as the attribute
 order is not preserved by the ElementTree.tostring method. Elements appear to
 be fine.
 """
+
 import re
 
 import pytest
 
 from excitingtools.exciting_dict_parsers.input_parser import parse_element_xml
-from excitingtools.input.bandstructure import band_structure_input_from_ase_atoms_obj, \
-    get_bandstructure_input_from_exciting_structure, band_structure_input_from_cell_or_bandpath
-from excitingtools.input.input_classes import ExcitingPropertiesInput, ExcitingGroundStateInput
+from excitingtools.input.bandstructure import (
+    band_structure_input_from_ase_atoms_obj,
+    band_structure_input_from_cell_or_bandpath,
+    get_bandstructure_input_from_exciting_structure,
+)
+from excitingtools.input.input_classes import ExcitingGroundStateInput, ExcitingPropertiesInput
 from excitingtools.input.input_xml import ExcitingInputXML
 from excitingtools.input.structure import ExcitingStructure
 
 
 @pytest.fixture
 def ase_ag():
     """If we cannot import ase we skip tests with this fixture.
 
     :returns: bulk Silver crystal
     """
-    ase_build = pytest.importorskip('ase.build')
-    return ase_build.bulk('Ag')
+    ase_build = pytest.importorskip("ase.build")
+    return ase_build.bulk("Ag")
 
 
 def test_bandstructure_properties_input():
     """Test giving the bandstructure input as a nested dict."""
     properties = {
-        "bandstructure": {"plot1d": {"path": {
-            "steps": 100,
-            "point":
-                [
-                    {"coord": [1, 0, 0], "label": "Gamma"},
-                    {"coord": [0.625, 0.375, 0], "label": "K"},
-                    {"coord": [0.5, 0.5, 0], "label": "X", "breakafter": True},
-                    {"coord": [0, 0, 0], "label": "Gamma"},
-                    {"coord": [0.5, 0, 0], "label": "L"}]}}}}
+        "bandstructure": {
+            "plot1d": {
+                "path": {
+                    "steps": 100,
+                    "point": [
+                        {"coord": [1, 0, 0], "label": "Gamma"},
+                        {"coord": [0.625, 0.375, 0], "label": "K"},
+                        {"coord": [0.5, 0.5, 0], "label": "X", "breakafter": True},
+                        {"coord": [0, 0, 0], "label": "Gamma"},
+                        {"coord": [0.5, 0, 0], "label": "L"},
+                    ],
+                }
+            }
+        }
+    }
 
     properties_input = ExcitingPropertiesInput(**properties)
     xml_string = properties_input.to_xml_str()
 
     assert properties == parse_element_xml(xml_string)
 
 
@@ -54,18 +64,18 @@
     correct.
     """
     ase_ag.set_cell(ase_ag.cell * 3)
     bs = band_structure_input_from_ase_atoms_obj(ase_ag)
     properties_input = ExcitingPropertiesInput(bandstructure=bs)
     bs_xml_string = properties_input.to_xml_str()
     # Get the high symmetry path.
-    all_labels = re.findall(r'label=\"([A-Z])', bs_xml_string)
-    assert all_labels == ['G', 'X', 'W', 'K', 'G', 'L', 'U', 'W', 'L', 'K', 'U', 'X']
+    all_labels = re.findall(r"label=\"([A-Z])", bs_xml_string)
+    assert all_labels == ["G", "X", "W", "K", "G", "L", "U", "W", "L", "K", "U", "X"]
     # Ensure there is only one breakafter statement.
-    assert len(re.findall(r'breakafter', bs_xml_string)) == 1
+    assert len(re.findall(r"breakafter", bs_xml_string)) == 1
 
     bs_xml = properties_input.to_xml()
     points = bs_xml.find("bandstructure").find("plot1d").find("path").findall("point")
     assert len(points) == 12
     assert points[0].get("coord") == "0.0 0.0 0.0"
     assert points[1].get("coord") == "0.5 0.0 0.5"
     assert points[2].get("coord") == "0.5 0.25 0.75"
@@ -84,39 +94,39 @@
 def test_bs_input(ase_ag):
     """Test writing exciting full input xml file with bandstructure property."""
     gs = ExcitingGroundStateInput(rgkmax=5.0)
     struct = ExcitingStructure(ase_ag)
     bs = band_structure_input_from_ase_atoms_obj(ase_ag)
     properties_input = ExcitingPropertiesInput(bandstructure=bs)
     input_xml = ExcitingInputXML(
-        structure=struct, groundstate=gs, title="BS exciting",
-        properties=properties_input).to_xml()
+        structure=struct, groundstate=gs, title="BS exciting", properties=properties_input
+    ).to_xml()
 
-    assert input_xml.tag == 'input'
+    assert input_xml.tag == "input"
     assert input_xml.keys() == []
 
     subelements = list(input_xml)
     assert len(subelements) == 4
     title_xml = subelements[0]
-    assert title_xml.tag == 'title'
+    assert title_xml.tag == "title"
     assert title_xml.keys() == []
-    assert title_xml.text == 'BS exciting'
+    assert title_xml.text == "BS exciting"
 
     properties_xml = subelements[3]
-    assert properties_xml.tag == 'properties'
+    assert properties_xml.tag == "properties"
     assert properties_xml.keys() == []
-    assert properties_xml.text == ' '
-    assert properties_xml[0].tag == 'bandstructure'
-    assert properties_xml[0][0].tag == 'plot1d'
-    assert properties_xml[0][0][0].tag == 'path'
-
-    first_coordinates = properties_xml[0][0][0][0].get('coord')
-    first_label = properties_xml[0][0][0][0].get('label')
-    assert first_coordinates == '0.0 0.0 0.0'
-    assert first_label == 'G'
+    assert properties_xml.text == " "
+    assert properties_xml[0].tag == "bandstructure"
+    assert properties_xml[0][0].tag == "plot1d"
+    assert properties_xml[0][0][0].tag == "path"
+
+    first_coordinates = properties_xml[0][0][0][0].get("coord")
+    first_label = properties_xml[0][0][0][0].get("label")
+    assert first_coordinates == "0.0 0.0 0.0"
+    assert first_label == "G"
 
 
 def test_get_bandstructure_input_from_exciting_structure(ase_ag):
     structure = ExcitingStructure(ase_ag)
     bs_xml = get_bandstructure_input_from_exciting_structure(structure).to_xml()
     points = bs_xml.find("plot1d").find("path").findall("point")
     assert len(points) == 12
@@ -133,22 +143,20 @@
     assert points[0].get("coord") == "0.0 0.0 0.0"
     assert points[1].get("coord") == "0.5 0.0 0.5"
     assert points[2].get("coord") == "0.125 -0.375 0.3125"
 
 
 def test_get_bandstructure_input_from_ase_bandpath(ase_ag):
     """Test creating required bandstructure input from an ASE bandpath.
-    
+
     Someone could create a bandpath that doesn't fall on special points
     e.g., 'Kpt0Kpt1,GMX,XZ'.
     """
-    ase = pytest.importorskip("ase")   
-    bandpath = ase.dft.kpoints.bandpath(
-        cell=ase_ag.cell,
-        path=[(0, 0, 0), (0.1, 0.2, 0.1), (0, 0, 0)])
+    ase = pytest.importorskip("ase")
+    bandpath = ase.dft.kpoints.bandpath(cell=ase_ag.cell, path=[(0, 0, 0), (0.1, 0.2, 0.1), (0, 0, 0)])
     bandstructure = band_structure_input_from_cell_or_bandpath(bandpath)
     bs_xml = bandstructure.to_xml()
     assert bs_xml.tag == "bandstructure", 'Root tag should be "bandstructure"'
     plot1d_xml = bs_xml.find("plot1d")
     assert plot1d_xml is not None, 'Missing "plot1d" subtree'
 
     path_xml = plot1d_xml.find("path")
```

### Comparing `excitingtools-1.7.0/tests/input/test_structure.py` & `excitingtools-1.7.1/tests/input/test_structure.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,303 +27,315 @@
 
 @pytest.fixture
 def xml_structure_H2He():
     """
     structure object initialised with a mock crystal, using mandatory arguments only.
     """
     cubic_lattice = [[1.0, 0.0, 0.0], [0.0, 1.0, 0.0], [0.0, 0.0, 1.0]]
-    arbitrary_atoms = [{'species': 'H', 'position': [0, 0, 0]},
-                       {'species': 'H', 'position': [1, 0, 0]},
-                       {'species': 'He', 'position': [2, 0, 0]}]
-    structure = ExcitingStructure(arbitrary_atoms, cubic_lattice, './')
+    arbitrary_atoms = [
+        {"species": "H", "position": [0, 0, 0]},
+        {"species": "H", "position": [1, 0, 0]},
+        {"species": "He", "position": [2, 0, 0]},
+    ]
+    structure = ExcitingStructure(arbitrary_atoms, cubic_lattice, "./")
     return structure.to_xml()
 
 
 def test_class_exciting_structure_xml(xml_structure_H2He):
     """
     Test input XML attributes from an instance of ExcitingStructure.
     """
-    assert xml_structure_H2He.tag == 'structure', 'XML root should be structure'
-    assert xml_structure_H2He.keys() == ['speciespath'], 'structure defined to have only speciespath '
-    assert xml_structure_H2He.get('speciespath') == './', 'species path set to ./'
+    assert xml_structure_H2He.tag == "structure", "XML root should be structure"
+    assert xml_structure_H2He.keys() == ["speciespath"], "structure defined to have only speciespath "
+    assert xml_structure_H2He.get("speciespath") == "./", "species path set to ./"
 
 
 def test_class_exciting_structure_crystal_xml(xml_structure_H2He):
     """
     crystal subtree of structure.
     """
     elements = list(xml_structure_H2He)
-    assert len(elements) == 3, 'Expect structure tree to have 3 sub-elements'
+    assert len(elements) == 3, "Expect structure tree to have 3 sub-elements"
 
     crystal_xml = elements[0]
-    assert crystal_xml.tag == "crystal", 'First subtree is crystal'
+    assert crystal_xml.tag == "crystal", "First subtree is crystal"
     assert crystal_xml.items() == [], "No required attributes in crystal."
 
     lattice_vectors = list(crystal_xml)
     assert len(lattice_vectors) == 3, "Always expect three lattice vectors"
-    assert lattice_vectors[0].items() == [], 'Lattice vectors have no items'
+    assert lattice_vectors[0].items() == [], "Lattice vectors have no items"
     assert lattice_vectors[0].text == "1.0 0.0 0.0", "Lattice vector `a` differs from input"
     assert lattice_vectors[1].text == "0.0 1.0 0.0", "Lattice vector `b` differs from input"
     assert lattice_vectors[2].text == "0.0 0.0 1.0", "Lattice vector `c` differs from input"
 
 
 def test_class_exciting_structure_species_xml(xml_structure_H2He):
     """
     species subtrees of structure.
     """
     elements = list(xml_structure_H2He)
-    assert len(elements) == 3, 'Expect structure tree to have 3 sub-elements'
+    assert len(elements) == 3, "Expect structure tree to have 3 sub-elements"
 
     species_h_xml = elements[1]
-    assert species_h_xml.tag == "species", 'Second subtree is species'
+    assert species_h_xml.tag == "species", "Second subtree is species"
 
     species_he_xml = elements[2]
-    assert species_he_xml.tag == "species", 'Third subtree is species'
+    assert species_he_xml.tag == "species", "Third subtree is species"
 
-    assert species_h_xml.items() == [('speciesfile', 'H.xml')], 'species is inconsistent'
-    assert species_he_xml.items() == [('speciesfile', 'He.xml')], 'species is inconsistent'
+    assert species_h_xml.items() == [("speciesfile", "H.xml")], "species is inconsistent"
+    assert species_he_xml.items() == [("speciesfile", "He.xml")], "species is inconsistent"
 
     atoms_h = list(species_h_xml)
-    assert len(atoms_h) == 2, 'Number of H atoms is wrong'
-    assert atoms_h[0].items() == [('coord', '0 0 0')], "Coordinate of first H differs to input"
-    assert atoms_h[1].items() == [('coord', '1 0 0')], "Coordinate of second H differs to input"
+    assert len(atoms_h) == 2, "Number of H atoms is wrong"
+    assert atoms_h[0].items() == [("coord", "0 0 0")], "Coordinate of first H differs to input"
+    assert atoms_h[1].items() == [("coord", "1 0 0")], "Coordinate of second H differs to input"
 
     atoms_he = list(species_he_xml)
-    assert len(atoms_he) == 1, 'Number of He atoms is wrong'
-    assert atoms_he[0].items() == [('coord', '2 0 0')], "Coordinate of only He differs to input"
+    assert len(atoms_he) == 1, "Number of He atoms is wrong"
+    assert atoms_he[0].items() == [("coord", "2 0 0")], "Coordinate of only He differs to input"
 
 
 @pytest.fixture
 def xml_structure_CdS():
     """
     structure object initialised with a mock crystal, using all atom properties.
     Optional atom attributes require the generic container, List[dict].
     """
     cubic_lattice = [[1.0, 0.0, 0.0], [0.0, 1.0, 0.0], [0.0, 0.0, 1.0]]
-    arbitrary_atoms = [{
-        'species': 'Cd',
-        'position': [0.0, 0.0, 0.0],
-        'bfcmt': [1.0, 1.0, 1.0],
-        'lockxyz': [False, False, False],
-        'mommtfix': [2.0, 2.0, 2.0]
-    }, {'species': 'S', 'position': [1.0, 0.0, 0.0]}]
-    structure = ExcitingStructure(arbitrary_atoms, cubic_lattice, './')
+    arbitrary_atoms = [
+        {
+            "species": "Cd",
+            "position": [0.0, 0.0, 0.0],
+            "bfcmt": [1.0, 1.0, 1.0],
+            "lockxyz": [False, False, False],
+            "mommtfix": [2.0, 2.0, 2.0],
+        },
+        {"species": "S", "position": [1.0, 0.0, 0.0]},
+    ]
+    structure = ExcitingStructure(arbitrary_atoms, cubic_lattice, "./")
     return structure.to_xml()
 
 
 def test_optional_atom_attributes_xml(xml_structure_CdS):
     """
     Test optional atom attributes are correctly set in XML tree.
     """
-    assert xml_structure_CdS.tag == 'structure'
-    assert xml_structure_CdS.keys() == ['speciespath'], 'structure defined to have only speciespath '
-    assert xml_structure_CdS.get('speciespath') == './', 'speciespath set to be ./'
+    assert xml_structure_CdS.tag == "structure"
+    assert xml_structure_CdS.keys() == ["speciespath"], "structure defined to have only speciespath "
+    assert xml_structure_CdS.get("speciespath") == "./", "speciespath set to be ./"
 
     elements = list(xml_structure_CdS)
-    assert len(elements) == 3, 'Expect structure tree to have 3 sub-elements'
+    assert len(elements) == 3, "Expect structure tree to have 3 sub-elements"
 
     # Crystal
     crystal_xml = elements[0]
-    assert crystal_xml.tag == "crystal", 'First subtree is crystal'
+    assert crystal_xml.tag == "crystal", "First subtree is crystal"
     assert crystal_xml.items() == [], "No required attributes in crystal."
 
     # Species
     species_cd_xml = elements[1]
-    assert species_cd_xml.tag == "species", 'Second subtree is species'
-    assert species_cd_xml.items() == [('speciesfile', 'Cd.xml')]
+    assert species_cd_xml.tag == "species", "Second subtree is species"
+    assert species_cd_xml.items() == [("speciesfile", "Cd.xml")]
 
     species_s_xml = elements[2]
-    assert species_s_xml.tag == "species", 'Third subtree is species'
-    assert species_s_xml.items() == [('speciesfile', 'S.xml')]
+    assert species_s_xml.tag == "species", "Third subtree is species"
+    assert species_s_xml.items() == [("speciesfile", "S.xml")]
 
     # Cd
     atoms_cd = list(species_cd_xml)
-    assert len(atoms_cd) == 1, 'Wrong number of Cd atoms'
-    assert set(atoms_cd[0].keys()) == {'coord', 'bfcmt', 'mommtfix', 'lockxyz'}, \
-        'Cd contains all mandatory and optional atom properties'
-    assert ('coord', '0.0 0.0 0.0') in atoms_cd[0].items()
-    assert ('bfcmt', '1.0 1.0 1.0') in atoms_cd[0].items()
-    assert ('mommtfix', '2.0 2.0 2.0') in atoms_cd[0].items()
-    assert ('lockxyz', 'false false false') in atoms_cd[0].items()
+    assert len(atoms_cd) == 1, "Wrong number of Cd atoms"
+    assert set(atoms_cd[0].keys()) == {
+        "coord",
+        "bfcmt",
+        "mommtfix",
+        "lockxyz",
+    }, "Cd contains all mandatory and optional atom properties"
+    assert ("coord", "0.0 0.0 0.0") in atoms_cd[0].items()
+    assert ("bfcmt", "1.0 1.0 1.0") in atoms_cd[0].items()
+    assert ("mommtfix", "2.0 2.0 2.0") in atoms_cd[0].items()
+    assert ("lockxyz", "false false false") in atoms_cd[0].items()
 
     # S
     atoms_s = list(species_s_xml)
-    assert len(atoms_s) == 1, 'Wrong number of S atoms'
-    assert atoms_s[0].keys() == ['coord'], \
-        'S only contains mandatory atom properties'
-    assert atoms_s[0].items() == [('coord', '1.0 0.0 0.0')]
+    assert len(atoms_s) == 1, "Wrong number of S atoms"
+    assert atoms_s[0].keys() == ["coord"], "S only contains mandatory atom properties"
+    assert atoms_s[0].items() == [("coord", "1.0 0.0 0.0")]
 
 
 @pytest.fixture
 def lattice_and_atoms_CdS():
     """
     structure object initialised with a mock crystal
     """
     cubic_lattice = [[1.0, 0.0, 0.0], [0.0, 1.0, 0.0], [0.0, 0.0, 1.0]]
-    arbitrary_atoms = [{'species': 'Cd', 'position': [0.0, 0.0, 0.0]},
-                       {'species': 'S', 'position': [1.0, 0.0, 0.0]}]
+    arbitrary_atoms = [{"species": "Cd", "position": [0.0, 0.0, 0.0]}, {"species": "S", "position": [1.0, 0.0, 0.0]}]
     return cubic_lattice, arbitrary_atoms
 
 
 def test_optional_structure_attributes_xml(lattice_and_atoms_CdS):
     """
     Test optional structure attributes.
     """
     cubic_lattice, arbitrary_atoms = lattice_and_atoms_CdS
-    structure_attributes = {
-        'autormt': True, 'cartesian': False, 'epslat': 1.e-6, 'primcell': False, 'tshift': True
-    }
-    structure = ExcitingStructure(arbitrary_atoms, cubic_lattice, './', **structure_attributes)
+    structure_attributes = {"autormt": True, "cartesian": False, "epslat": 1.0e-6, "primcell": False, "tshift": True}
+    structure = ExcitingStructure(arbitrary_atoms, cubic_lattice, "./", **structure_attributes)
     xml_structure = structure.to_xml()
 
-    mandatory = {'speciespath'}
+    mandatory = {"speciespath"}
     optional = set(structure_attributes)
 
-    assert xml_structure.tag == 'structure'
-    assert set(xml_structure.keys()) == mandatory | optional, \
-        'Should contain mandatory speciespath plus all optional attributes'
-    assert xml_structure.get('speciespath') == './', 'species path should be ./'
-    assert xml_structure.get('autormt') == 'true'
-    assert xml_structure.get('cartesian') == 'false'
-    assert xml_structure.get('epslat') == '1e-06'
-    assert xml_structure.get('primcell') == 'false'
-    assert xml_structure.get('tshift') == 'true'
+    assert xml_structure.tag == "structure"
+    assert (
+        set(xml_structure.keys()) == mandatory | optional
+    ), "Should contain mandatory speciespath plus all optional attributes"
+    assert xml_structure.get("speciespath") == "./", "species path should be ./"
+    assert xml_structure.get("autormt") == "true"
+    assert xml_structure.get("cartesian") == "false"
+    assert xml_structure.get("epslat") == "1e-06"
+    assert xml_structure.get("primcell") == "false"
+    assert xml_structure.get("tshift") == "true"
 
 
 def test_optional_crystal_attributes_xml(lattice_and_atoms_CdS):
     """
     Test optional crystal attributes.
     """
     cubic_lattice, arbitrary_atoms = lattice_and_atoms_CdS
 
     structure = ExcitingStructure(
-        arbitrary_atoms,
-        cubic_lattice,
-        './',
-        crystal_properties={'scale': 1.00, 'stretch': [1.00, 1.00, 1.00]}
+        arbitrary_atoms, cubic_lattice, "./", crystal_properties={"scale": 1.00, "stretch": [1.00, 1.00, 1.00]}
     )
     xml_structure = structure.to_xml()
 
     elements = list(xml_structure)
-    assert len(elements) == 3, 'Number of sub-elements in structure tree'
+    assert len(elements) == 3, "Number of sub-elements in structure tree"
 
     crystal_xml = elements[0]
-    assert crystal_xml.tag == "crystal", 'First subtree is crystal'
-    assert crystal_xml.keys() == ['scale', 'stretch'], 'Optional crystal properties'
-    assert crystal_xml.get('scale') == '1.0', 'scale value inconsistent with input'
-    assert crystal_xml.get('stretch') == '1.0 1.0 1.0', 'stretch value inconsistent with input'
+    assert crystal_xml.tag == "crystal", "First subtree is crystal"
+    assert crystal_xml.keys() == ["scale", "stretch"], "Optional crystal properties"
+    assert crystal_xml.get("scale") == "1.0", "scale value inconsistent with input"
+    assert crystal_xml.get("stretch") == "1.0 1.0 1.0", "stretch value inconsistent with input"
 
 
 def test_optional_species_attributes_xml(lattice_and_atoms_CdS):
     """
     Test optional species attributes.
     """
     cubic_lattice, arbitrary_atoms = lattice_and_atoms_CdS
-    species_attributes = {'Cd': {'rmt': 3.0, "LDAplusU": {"J": 1.5, "U": 2.4, "l": 2}},
-                          'S': {'rmt': 4.0, "dfthalfparam": {"ampl": 1.2, "cut": 1.9, "exponent": 5,
-                                                             "shell": [{"ionization": 0.8, "number": 1}]}}}
+    species_attributes = {
+        "Cd": {"rmt": 3.0, "LDAplusU": {"J": 1.5, "U": 2.4, "l": 2}},
+        "S": {
+            "rmt": 4.0,
+            "dfthalfparam": {"ampl": 1.2, "cut": 1.9, "exponent": 5, "shell": [{"ionization": 0.8, "number": 1}]},
+        },
+    }
 
-    structure = ExcitingStructure(
-        arbitrary_atoms, cubic_lattice, './', species_properties=species_attributes
-    )
+    structure = ExcitingStructure(arbitrary_atoms, cubic_lattice, "./", species_properties=species_attributes)
     xml_structure = structure.to_xml()
 
     elements = list(xml_structure)
-    assert len(elements) == 3, 'Number of sub-elements in structure tree'
+    assert len(elements) == 3, "Number of sub-elements in structure tree"
 
     species_cd_xml = elements[1]
-    assert species_cd_xml.tag == "species", 'Second subtree is species'
+    assert species_cd_xml.tag == "species", "Second subtree is species"
 
     species_s_xml = elements[2]
-    assert species_s_xml.tag == "species", 'Third subtree is species'
+    assert species_s_xml.tag == "species", "Third subtree is species"
 
-    assert set(species_cd_xml.keys()) == {'speciesfile', 'rmt'}, "species attributes differ from expected"
-    assert species_cd_xml.get('speciesfile') == 'Cd.xml', 'speciesfile differs from expected'
-    assert species_cd_xml.get('rmt') == '3.0', 'Cd muffin tin radius differs from input'
+    assert set(species_cd_xml.keys()) == {"speciesfile", "rmt"}, "species attributes differ from expected"
+    assert species_cd_xml.get("speciesfile") == "Cd.xml", "speciesfile differs from expected"
+    assert species_cd_xml.get("rmt") == "3.0", "Cd muffin tin radius differs from input"
 
     species_cd_elements = list(species_cd_xml)
     assert len(species_cd_elements) == 2
     ldaplusu_xml = species_cd_elements[0]
     assert ldaplusu_xml.tag == "LDAplusU"
 
-    assert set(ldaplusu_xml.keys()) == {'J', 'U', 'l'}
+    assert set(ldaplusu_xml.keys()) == {"J", "U", "l"}
     assert ldaplusu_xml.get("J") == "1.5"
     assert ldaplusu_xml.get("U") == "2.4"
     assert ldaplusu_xml.get("l") == "2"
 
-    assert set(species_s_xml.keys()) == {'speciesfile', 'rmt'}, "species attributes differ from expected"
-    assert species_s_xml.get('speciesfile') == 'S.xml', 'speciesfile differs from expected'
-    assert species_s_xml.get('rmt') == '4.0', 'S muffin tin radius differs from input'
+    assert set(species_s_xml.keys()) == {"speciesfile", "rmt"}, "species attributes differ from expected"
+    assert species_s_xml.get("speciesfile") == "S.xml", "speciesfile differs from expected"
+    assert species_s_xml.get("rmt") == "4.0", "S muffin tin radius differs from input"
 
     species_s_elements = list(species_s_xml)
     assert len(species_s_elements) == 2
     dfthalfparam_xml = species_s_elements[0]
     assert dfthalfparam_xml.tag == "dfthalfparam"
 
-    assert set(dfthalfparam_xml.keys()) == {'ampl', 'cut', 'exponent'}
+    assert set(dfthalfparam_xml.keys()) == {"ampl", "cut", "exponent"}
     assert dfthalfparam_xml.get("ampl") == "1.2"
     assert dfthalfparam_xml.get("cut") == "1.9"
     assert dfthalfparam_xml.get("exponent") == "5"
 
     dfthalfparam_elements = list(dfthalfparam_xml)
     assert len(dfthalfparam_elements) == 1
     shell_xml = dfthalfparam_elements[0]
     assert shell_xml.tag == "shell"
 
-    assert set(shell_xml.keys()) == {'ionization', 'number'}
-    assert shell_xml.get('ionization') == '0.8'
-    assert shell_xml.get('number') == '1'
+    assert set(shell_xml.keys()) == {"ionization", "number"}
+    assert shell_xml.get("ionization") == "0.8"
+    assert shell_xml.get("number") == "1"
 
 
-ref_dict = {'xml_string': '<structure speciespath="./"> <crystal> <basevect>1.0 0.0 0.0</basevect>'
-                          '<basevect>0.0 1.0 0.0</basevect><basevect>0.0 0.0 1.0</basevect></crystal>'
-                          '<species speciesfile="Cd.xml"> <atom coord="0.0 0.0 0.0"> </atom></species>'
-                          '<species speciesfile="S.xml"> <atom coord="1.0 0.0 0.0"> </atom></species></structure>'}
+ref_dict = {
+    "xml_string": '<structure speciespath="./"> <crystal> <basevect>1.0 0.0 0.0</basevect>'
+    "<basevect>0.0 1.0 0.0</basevect><basevect>0.0 0.0 1.0</basevect></crystal>"
+    '<species speciesfile="Cd.xml"> <atom coord="0.0 0.0 0.0"> </atom></species>'
+    '<species speciesfile="S.xml"> <atom coord="1.0 0.0 0.0"> </atom></species></structure>'
+}
 
 
-def test_as_dict(lattice_and_atoms_CdS, mock_env_jobflow_missing):
+@pytest.mark.usefixtures("mock_env_jobflow_missing")
+def test_as_dict(lattice_and_atoms_CdS):
     cubic_lattice, arbitrary_atoms = lattice_and_atoms_CdS
 
-    structure = ExcitingStructure(arbitrary_atoms, cubic_lattice, './')
+    structure = ExcitingStructure(arbitrary_atoms, cubic_lattice, "./")
 
-    assert structure.as_dict() == ref_dict, 'expected different dict representation'
+    assert structure.as_dict() == ref_dict, "expected different dict representation"
 
 
-def test_as_dict_jobflow(lattice_and_atoms_CdS, mock_env_jobflow):
+@pytest.mark.usefixtures("mock_env_jobflow")
+def test_as_dict_jobflow(lattice_and_atoms_CdS):
     cubic_lattice, arbitrary_atoms = lattice_and_atoms_CdS
 
-    structure = ExcitingStructure(arbitrary_atoms, cubic_lattice, './')
+    structure = ExcitingStructure(arbitrary_atoms, cubic_lattice, "./")
 
-    assert structure.as_dict() == {**ref_dict, '@class': 'ExcitingStructure',
-                                   '@module': 'excitingtools.input.structure'}, \
-        'expected different dict representation'
+    assert structure.as_dict() == {
+        **ref_dict,
+        "@class": "ExcitingStructure",
+        "@module": "excitingtools.input.structure",
+    }, "expected different dict representation"
 
 
 def test_from_dict(lattice_and_atoms_CdS):
     cubic_lattice, arbitrary_atoms = lattice_and_atoms_CdS
     structure = ExcitingStructure.from_dict(ref_dict)
 
     assert np.allclose(structure.lattice, np.array(cubic_lattice))
-    assert structure.species == [d['species'] for d in arbitrary_atoms]
-    assert structure.positions == [d['position'] for d in arbitrary_atoms]
-    assert structure.speciespath == './'  # pylint: disable=no-member
+    assert structure.species == [d["species"] for d in arbitrary_atoms]
+    assert structure.positions == [d["position"] for d in arbitrary_atoms]
+    assert structure.speciespath == "./"  # pylint: disable=no-member
 
 
 def test_add_and_remove_atoms(lattice_and_atoms_CdS):
     cubic_lattice, arbitrary_atoms = lattice_and_atoms_CdS
-    structure = ExcitingStructure(arbitrary_atoms, cubic_lattice, './')
+    structure = ExcitingStructure(arbitrary_atoms, cubic_lattice, "./")
 
     assert len(structure.species) == 2, "initially there are 2 atoms in the structure"
     # just confirm that the xml tree can be built, not that it is fully correct
     structure.to_xml()
 
-    structure.add_atom("Cd", [0.25, 0.25, 0.25], {'bfcmt': [1.0, 1.0, 1.0]})
+    structure.add_atom("Cd", [0.25, 0.25, 0.25], {"bfcmt": [1.0, 1.0, 1.0]})
     xml_tree = structure.to_xml()
     assert xml_tree.findall("species")[0].findall("atom")[1].attrib == {
-        "coord": "0.25 0.25 0.25", "bfcmt": "1.0 1.0 1.0"
+        "coord": "0.25 0.25 0.25",
+        "bfcmt": "1.0 1.0 1.0",
     }
 
     structure.add_atom("Mg", [0.75, 0.25, 0.0], species_properties={"rmt": 3})
     xml_tree = structure.to_xml()
     mg_tree = xml_tree.findall("species")[1]
     assert mg_tree.attrib == {"rmt": "3", "speciesfile": "Mg.xml"}
     mg_atom = mg_tree.findall("atom")[0]
@@ -345,117 +357,119 @@
 
 @pytest.fixture
 def lattice_and_atoms_H20():
     """
     H20 molecule in a big box (angstrom)
     """
     cubic_lattice = [[10.0, 0.0, 0.0], [0.0, 10.0, 0.0], [0.0, 0.0, 10.0]]
-    atoms = [{'species': 'H', 'position': [0.00000, 0.75545, -0.47116]},
-             {'species': 'O', 'position': [0.00000, 0.00000, 0.11779]},
-             {'species': 'H', 'position': [0.00000, 0.75545, -0.47116]}]
+    atoms = [
+        {"species": "H", "position": [0.00000, 0.75545, -0.47116]},
+        {"species": "O", "position": [0.00000, 0.00000, 0.11779]},
+        {"species": "H", "position": [0.00000, 0.75545, -0.47116]},
+    ]
     return cubic_lattice, atoms
 
 
 def test_group_atoms_by_species(lattice_and_atoms_H20):
     """
     Test group_atoms_by_species method.
     """
     cubic_lattice, atoms = lattice_and_atoms_H20
-    structure = ExcitingStructure(atoms, cubic_lattice, './')
-    assert structure.species == ['H', 'O', 'H'], 'Species list differs from lattice_and_atoms_H20'
+    structure = ExcitingStructure(atoms, cubic_lattice, "./")
+    assert structure.species == ["H", "O", "H"], "Species list differs from lattice_and_atoms_H20"
 
     indices = dict(structure._group_atoms_by_species())
-    assert set(indices.keys()) == {'H', 'O'}, 'List unique species in structure'
-    assert indices['H'] == [0, 2], "Expect atoms 0 and 2 to be H"
-    assert indices['O'] == [1], "Expect atom 1 to be O"
+    assert set(indices.keys()) == {"H", "O"}, "List unique species in structure"
+    assert indices["H"] == [0, 2], "Expect atoms 0 and 2 to be H"
+    assert indices["O"] == [1], "Expect atom 1 to be O"
 
-    hydrogen = [structure.species[i] for i in indices['H']]
-    oxygen = [structure.species[i] for i in indices['O']]
+    hydrogen = [structure.species[i] for i in indices["H"]]
+    oxygen = [structure.species[i] for i in indices["O"]]
     assert hydrogen == ["H", "H"], "Expect list to only contain H symbols"
     assert oxygen == ["O"], "Expect list to contain only one O symbol"
 
 
 @pytest.fixture
 def ase_atoms_H20(lattice_and_atoms_H20):
     """
     H20 molecule in a big box (angstrom), in ASE Atoms()
     Converts a List[dict] to ase.atoms.Atoms.
     """
     ase = pytest.importorskip("ase")
     lattice, atoms = lattice_and_atoms_H20
-    symbols = [atom['species'] for atom in atoms]
+    symbols = [atom["species"] for atom in atoms]
     cubic_cell = np.asarray(lattice)
-    positions = [atom['position'] for atom in atoms]
+    positions = [atom["position"] for atom in atoms]
     return ase.Atoms(symbols=symbols, positions=positions, cell=cubic_cell, pbc=True)
 
 
 def test_class_exciting_structure_ase(ase_atoms_H20):
     """
     Test the ASE Atoms object gets used correctly by the ExcitingStructure constructor.
     """
     atoms = ase_atoms_H20
-    structure = ExcitingStructure(atoms, species_path='./')
+    structure = ExcitingStructure(atoms, species_path="./")
 
     assert structure.species == ["H", "O", "H"]
-    assert np.allclose(structure.lattice,
-                       [[18.897261246257703, 0.0, 0.0],
-                        [0.0, 18.897261246257703, 0.0],
-                        [0.0, 0.0, 18.897261246257703]]), \
-        'Expect lattice vectors to match input values'
+    assert np.allclose(
+        structure.lattice,
+        [[18.897261246257703, 0.0, 0.0], [0.0, 18.897261246257703, 0.0], [0.0, 0.0, 18.897261246257703]],
+    ), "Expect lattice vectors to match input values"
 
-    assert np.allclose(structure.positions, atoms.get_scaled_positions()), 'Expect positions to match input values.'
+    assert np.allclose(structure.positions, atoms.get_scaled_positions()), "Expect positions to match input values."
 
     # TODO(Alex) Issue 117. Compare xml_structure built with and without ASE - should be consistent
     # This just confirms the XML tree is built, not that it is correct.
     xml_structure = structure.to_xml()
-    assert list(xml_structure.keys()) == ['speciespath'], 'Only expect speciespath in structure xml keys'
+    assert list(xml_structure.keys()) == ["speciespath"], "Only expect speciespath in structure xml keys"
 
 
 def test_using_non_standard_species_symbol():
     cubic_lattice = [[10.0, 0.0, 0.0], [0.0, 10.0, 0.0], [0.0, 0.0, 10.0]]
-    atoms = [{'species': 'C_molecule', 'position': [0.00000, 0.75545, -0.47116]}]
+    atoms = [{"species": "C_molecule", "position": [0.00000, 0.75545, -0.47116]}]
     structure = ExcitingStructure(atoms, cubic_lattice)
 
     structure_xml = structure.to_xml()
-    assert structure_xml.tag == 'structure', 'XML root should be structure'
-    assert structure_xml.keys() == ['speciespath'], 'structure defined to have only speciespath '
-    assert structure_xml.get('speciespath') == './', 'species path set to ./'
+    assert structure_xml.tag == "structure", "XML root should be structure"
+    assert structure_xml.keys() == ["speciespath"], "structure defined to have only speciespath "
+    assert structure_xml.get("speciespath") == "./", "species path set to ./"
 
     elements = list(structure_xml)
-    assert len(elements) == 2, 'Expect structure tree to have 2 sub-elements'
+    assert len(elements) == 2, "Expect structure tree to have 2 sub-elements"
 
     species_c_xml = elements[1]
-    assert species_c_xml.tag == "species", 'Second subtree is species'
+    assert species_c_xml.tag == "species", "Second subtree is species"
 
-    assert species_c_xml.items() == [('speciesfile', 'C_molecule.xml')], 'species is inconsistent'
+    assert species_c_xml.items() == [("speciesfile", "C_molecule.xml")], "species is inconsistent"
 
     atoms_h = list(species_c_xml)
     assert len(atoms_h) == 1
-    assert atoms_h[0].items() == [('coord', '0.0 0.75545 -0.47116')]
+    assert atoms_h[0].items() == [("coord", "0.0 0.75545 -0.47116")]
 
 
 def test_get_full_lattice(lattice_and_atoms_CdS):
     cubic_lattice, arbitrary_atoms = lattice_and_atoms_CdS
-    structure = ExcitingStructure(arbitrary_atoms, cubic_lattice, './',
-                                  crystal_properties={'scale': 1.50, 'stretch': [2.00, 1.00, 3.00]})
+    structure = ExcitingStructure(
+        arbitrary_atoms, cubic_lattice, "./", crystal_properties={"scale": 1.50, "stretch": [2.00, 1.00, 3.00]}
+    )
     ref_lattice = np.array([[3, 0, 0], [0, 1.5, 0], [0, 0, 4.5]])
     assert np.allclose(structure.get_lattice(), ref_lattice)
 
 
-def test_structure_input_with_integers(tmp_path):
+def test_structure_input_with_integers():
     atoms = [{"species": "C", "position": [0, 0, 0]}]
     structure = ExcitingStructure(atoms, [[1, 0, 0], [0, 1, 0], [0, 0, 1]], "./")
-    ref_lattice = np.array([[0.52917721, 0., 0.], [0., 0.52917721, 0.], [0., 0., 0.52917721]])
+    ref_lattice = np.array([[0.52917721, 0.0, 0.0], [0.0, 0.52917721, 0.0], [0.0, 0.0, 0.52917721]])
     assert np.allclose(structure.get_lattice(convert_to_angstrom=True), ref_lattice)
 
 
 def test_get_bandstructure_input_from_exciting_structure(lattice_and_atoms_H20):
     pytest.importorskip("ase")
     cubic_lattice, atoms = lattice_and_atoms_H20
-    structure = ExcitingStructure(atoms, cubic_lattice, './')
+    structure = ExcitingStructure(atoms, cubic_lattice, "./")
     bandstructure = get_bandstructure_input_from_exciting_structure(structure)
     bs_xml = bandstructure.to_xml()
 
     assert bs_xml.tag == "bandstructure", 'Root tag should be "bandstructure"'
 
     plot1d_xml = bs_xml.find("plot1d")
     assert plot1d_xml is not None, 'Missing "plot1d" subtree'
```

### Comparing `excitingtools-1.7.0/tests/input/test_xml_utils.py` & `excitingtools-1.7.1/tests/input/test_xml_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-"""Test XML utilities.
-"""
+"""Test XML utilities."""
 
 from excitingtools.input.xml_utils import line_reformatter
 
 
 def test_line_reformatter_long_ending():
     """Test reformatting of XML as a string works."""
     input_str = (
         '<groundstate do="fromscratch" ngridk="6 6 6" nosource="false" '
         'rgkmax="8.0" tforce="true" vkloff="0 0 0" xctype="GGA_PBE_SOL"> '
-        '</groundstate>'
+        "</groundstate>"
     )
     pretty_input_str = line_reformatter(input_str)
-    # Note, whitespace is important
+    # Note whitespace is important
     reference = """<groundstate
    do="fromscratch"
    ngridk="6 6 6"
    nosource="false"
    rgkmax="8.0"
    tforce="true"
    vkloff="0 0 0"
@@ -29,15 +28,15 @@
     """Test reformatting of XML as a string works for xml strings
     with a different (short) ending."""
     input_str = (
         '<groundstate do="fromscratch" ngridk="6 6 6" nosource="false" '
         'rgkmax="8.0" tforce="true" vkloff="0 0 0" xctype="GGA_PBE_SOL"/> '
     )
     pretty_input_str = line_reformatter(input_str)
-    # Note, whitespace is important
+    # Note whitespace is important
     reference = """<groundstate
    do="fromscratch"
    ngridk="6 6 6"
    nosource="false"
    rgkmax="8.0"
    tforce="true"
    vkloff="0 0 0"
@@ -49,15 +48,15 @@
     """Test reformatting of XML as a string works for xml strings
     with no closing at the end."""
     input_str = (
         '<groundstate do="fromscratch" ngridk="6 6 6" nosource="false" '
         'rgkmax="8.0" tforce="true" vkloff="0 0 0" xctype="GGA_PBE_SOL"> '
     )
     pretty_input_str = line_reformatter(input_str)
-    # Note, whitespace is important
+    # Note whitespace is important
     reference = """<groundstate
    do="fromscratch"
    ngridk="6 6 6"
    nosource="false"
    rgkmax="8.0"
    tforce="true"
    vkloff="0 0 0"
```

### Comparing `excitingtools-1.7.0/tests/input/test_xs.py` & `excitingtools-1.7.1/tests/input/test_xs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,221 +1,225 @@
 """Test ExcitingGroundStateInput class attribute assignment and methods.
 
 NOTE:
 All attribute tests should assert on the XML tree content's as the attribute
 order is not preserved by the ElementTree.tostring method. Elements appear to
 be fine.
 """
+
 import numpy as np
 import pytest
 
-# noinspection PyUnresolvedReferences
 from excitingtools.input.input_classes import ExcitingBSEInput, ExcitingXSInput
 
 
 def test_class_ExcitingXSInput():
     xs_input = ExcitingXSInput(xstype="BSE")
 
     xs_xml = xs_input.to_xml()
-    assert xs_xml.tag == 'xs'
-    assert xs_xml.items() == [('xstype', 'BSE')]
+    assert xs_xml.tag == "xs"
+    assert xs_xml.items() == [("xstype", "BSE")]
 
 
 def test_class_ExcitingXSInput_xstype_missing():
     with pytest.raises(ValueError, match="Missing mandatory arguments: {'xstype'}"):
         ExcitingXSInput(ngridk=[4, 4, 4])
 
 
-def test_ExcitingXSInput_as_dict(mock_env_jobflow_missing):
+@pytest.mark.usefixtures("mock_env_jobflow_missing")
+def test_ExcitingXSInput_as_dict():
     xs_input = ExcitingXSInput(xstype="BSE")
-    ref_dict = {'xml_string': '<xs xstype="BSE"> </xs>'}
-    assert xs_input.as_dict() == ref_dict, 'expected different dict representation'
+    ref_dict = {"xml_string": '<xs xstype="BSE"> </xs>'}
+    assert xs_input.as_dict() == ref_dict, "expected different dict representation"
 
 
-def test_ExcitingXSInput_as_dict_jobflow(mock_env_jobflow):
+@pytest.mark.usefixtures("mock_env_jobflow")
+def test_ExcitingXSInput_as_dict_jobflow():
     xs_input = ExcitingXSInput(xstype="BSE")
-    ref_dict = {'@class': 'ExcitingXSInput',
-                '@module': 'excitingtools.input.input_classes',
-                'xml_string': '<xs xstype="BSE"> </xs>'}
-    assert xs_input.as_dict() == ref_dict, 'expected different dict representation'
+    ref_dict = {
+        "@class": "ExcitingXSInput",
+        "@module": "excitingtools.input.input_classes",
+        "xml_string": '<xs xstype="BSE"> </xs>',
+    }
+    assert xs_input.as_dict() == ref_dict, "expected different dict representation"
 
 
 def test_ExcitingXSInput_from_dict():
-    ref_dict = {'xml_string': '<xs xstype="BSE"> </xs>'}
+    ref_dict = {"xml_string": '<xs xstype="BSE"> </xs>'}
     recreated_xs = ExcitingXSInput.from_dict(ref_dict)
-    assert recreated_xs.to_xml_str() == ref_dict['xml_string']
+    assert recreated_xs.to_xml_str() == ref_dict["xml_string"]
 
 
 def test_class_ExcitingXSInput_xs():
-    xs = {'broad': 0.32, 'ngridk': [8, 8, 8], 'tevout': True, 'nempty': 52, 'pwmat': 'fft', "xstype": "BSE"}
+    xs = {"broad": 0.32, "ngridk": [8, 8, 8], "tevout": True, "nempty": 52, "pwmat": "fft", "xstype": "BSE"}
     xs_input = ExcitingXSInput(**xs)
 
     xs_xml = xs_input.to_xml()
-    assert xs_xml.tag == 'xs'
+    assert xs_xml.tag == "xs"
     assert set(xs_xml.keys()) == set(xs)
-    assert xs_xml.get('xstype') == 'BSE'
-    assert xs_xml.get('broad') == '0.32'
-    assert xs_xml.get('ngridk') == '8 8 8'
-    assert xs_xml.get('tevout') == 'true'
-    assert xs_xml.get('nempty') == '52'
-    assert xs_xml.get('pwmat') == 'fft'
+    assert xs_xml.get("xstype") == "BSE"
+    assert xs_xml.get("broad") == "0.32"
+    assert xs_xml.get("ngridk") == "8 8 8"
+    assert xs_xml.get("tevout") == "true"
+    assert xs_xml.get("nempty") == "52"
+    assert xs_xml.get("pwmat") == "fft"
 
 
 def test_class_ExcitingXsInput_wrong_key():
     with pytest.raises(ValueError, match="xs keys are not valid: {'wrong_key'}"):
         ExcitingXSInput(xstype="BSE", wrong_key=1)
 
 
 def test_class_ExcitingXSInput_BSE_element():
-    bse_attributes = {'bsetype': 'singlet', 'xas': True, 'xasspecies': 1}
+    bse_attributes = {"bsetype": "singlet", "xas": True, "xasspecies": 1}
     bse_keys = list(bse_attributes)
     xs_input = ExcitingXSInput(xstype="BSE", BSE=bse_attributes)
 
     xs_xml = xs_input.to_xml()
-    assert xs_xml.tag == 'xs'
-    assert set(xs_xml.keys()) == {'xstype'}
+    assert xs_xml.tag == "xs"
+    assert set(xs_xml.keys()) == {"xstype"}
 
     elements = list(xs_xml)
     assert len(elements) == 1
 
     bse_xml = elements[0]
     assert bse_xml.tag == "BSE"
-    assert bse_xml.keys() == bse_keys, 'Should contain all bse attributes'
-    assert bse_xml.get('bsetype') == 'singlet'
-    assert bse_xml.get('xas') == 'true'
-    assert bse_xml.get('xasspecies') == '1'
+    assert bse_xml.keys() == bse_keys, "Should contain all bse attributes"
+    assert bse_xml.get("bsetype") == "singlet"
+    assert bse_xml.get("xas") == "true"
+    assert bse_xml.get("xasspecies") == "1"
 
 
 def test_class_ExcitingXSInput_BSE_element_object():
-    bse_object = ExcitingBSEInput(bsetype='singlet', xas=True, xasspecies=1)
-    bse_keys = {'bsetype', 'xas', 'xasspecies'}
+    bse_object = ExcitingBSEInput(bsetype="singlet", xas=True, xasspecies=1)
+    bse_keys = {"bsetype", "xas", "xasspecies"}
     xs_input = ExcitingXSInput(xstype="BSE", BSE=bse_object)
 
     xs_xml = xs_input.to_xml()
-    assert xs_xml.tag == 'xs'
-    assert set(xs_xml.keys()) == {'xstype'}
+    assert xs_xml.tag == "xs"
+    assert set(xs_xml.keys()) == {"xstype"}
 
     elements = list(xs_xml)
     assert len(elements) == 1
 
     bse_xml = elements[0]
     assert bse_xml.tag == "BSE"
-    assert set(bse_xml.keys()) == bse_keys, 'Should contain all bse attributes'
-    assert bse_xml.get('bsetype') == 'singlet'
-    assert bse_xml.get('xas') == 'true'
-    assert bse_xml.get('xasspecies') == '1'
+    assert set(bse_xml.keys()) == bse_keys, "Should contain all bse attributes"
+    assert bse_xml.get("bsetype") == "singlet"
+    assert bse_xml.get("xas") == "true"
+    assert bse_xml.get("xasspecies") == "1"
 
 
 def test_class_ExcitingXSInput_energywindow_element():
-    energywindow_attributes = {'intv': [5.8, 8.3], 'points': 5000}
+    energywindow_attributes = {"intv": [5.8, 8.3], "points": 5000}
     xs_input = ExcitingXSInput(xstype="BSE", energywindow=energywindow_attributes)
 
     xs_xml = xs_input.to_xml()
-    assert xs_xml.tag == 'xs'
+    assert xs_xml.tag == "xs"
 
     elements = list(xs_xml)
     assert len(elements) == 1
 
     energywindow_xml = elements[0]
     assert energywindow_xml.tag == "energywindow"
-    assert set(energywindow_xml.keys()) == set(energywindow_attributes), 'Should contain all bse attributes'
-    assert energywindow_xml.get('intv') == '5.8 8.3'
-    assert energywindow_xml.get('points') == '5000'
+    assert set(energywindow_xml.keys()) == set(energywindow_attributes), "Should contain all bse attributes"
+    assert energywindow_xml.get("intv") == "5.8 8.3"
+    assert energywindow_xml.get("points") == "5000"
 
 
 def test_class_ExcitingXSInput_screening_element():
-    screening_attributes = {'screentype': 'full', 'nempty': 15}
+    screening_attributes = {"screentype": "full", "nempty": 15}
     xs_input = ExcitingXSInput(xstype="BSE", screening=screening_attributes)
 
     xs_xml = xs_input.to_xml()
-    assert xs_xml.tag == 'xs'
+    assert xs_xml.tag == "xs"
 
     elements = list(xs_xml)
     assert len(elements) == 1
 
     screening_xml = elements[0]
     assert screening_xml.tag == "screening"
-    assert set(screening_xml.keys()) == set(screening_attributes), 'Should contain all bse attributes'
-    assert screening_xml.get('screentype') == 'full'
-    assert screening_xml.get('nempty') == '15'
+    assert set(screening_xml.keys()) == set(screening_attributes), "Should contain all bse attributes"
+    assert screening_xml.get("screentype") == "full"
+    assert screening_xml.get("nempty") == "15"
 
 
 def test_class_ExcitingQpointsetInput_numpy():
     qpointset_input = np.array(((0, 0, 0), (0.5, 0.5, 0.5)))
 
     xs_input = ExcitingXSInput(xstype="BSE", qpointset=qpointset_input)
 
     xs_xml = xs_input.to_xml()
-    assert xs_xml.tag == 'xs'
+    assert xs_xml.tag == "xs"
 
     elements = list(xs_xml)
     assert len(elements) == 1
 
     qpointset_xml = elements[0]
     assert qpointset_xml.tag == "qpointset"
     assert qpointset_xml.items() == []
 
     qpoints = list(qpointset_xml)
     assert len(qpoints) == 2
-    assert qpoints[0].tag == 'qpoint'
+    assert qpoints[0].tag == "qpoint"
     assert qpoints[0].items() == []
-    assert qpoints[0].text == '0.0 0.0 0.0'
-    assert qpoints[1].text == '0.5 0.5 0.5'
+    assert qpoints[0].text == "0.0 0.0 0.0"
+    assert qpoints[1].text == "0.5 0.5 0.5"
 
 
 def test_class_ExcitingQpointsetInput_list():
     qpointset_input = [[0, 0, 0], [0.5, 0.5, 0.5]]
 
     xs_input = ExcitingXSInput(xstype="BSE", qpointset=qpointset_input)
 
     xs_xml = xs_input.to_xml()
-    assert xs_xml.tag == 'xs'
+    assert xs_xml.tag == "xs"
 
     elements = list(xs_xml)
     assert len(elements) == 1
 
     qpointset_xml = elements[0]
     assert qpointset_xml.tag == "qpointset"
     assert qpointset_xml.items() == []
 
     qpoints = list(qpointset_xml)
     assert len(qpoints) == 2
-    assert qpoints[0].tag == 'qpoint'
+    assert qpoints[0].tag == "qpoint"
     assert qpoints[0].items() == []
-    assert qpoints[0].text == '0 0 0'
-    assert qpoints[1].text == '0.5 0.5 0.5'
+    assert qpoints[0].text == "0 0 0"
+    assert qpoints[1].text == "0.5 0.5 0.5"
 
 
 def test_class_ExcitingPlanInput():
-    plan_input = ['screen', 'bse', 'bsegenspec']
+    plan_input = ["screen", "bse", "bsegenspec"]
 
     xs_input = ExcitingXSInput(xstype="BSE", plan=plan_input)
 
     xs_xml = xs_input.to_xml()
-    assert xs_xml.tag == 'xs'
+    assert xs_xml.tag == "xs"
 
     elements = list(xs_xml)
     assert len(elements) == 1
 
     plan_xml = elements[0]
     assert plan_xml.tag == "plan"
     assert plan_xml.items() == []
 
     doonlys = list(plan_xml)
     assert len(doonlys) == 3
-    assert doonlys[0].tag == 'doonly'
-    assert doonlys[0].items() == [('task', 'screen')]
-    assert doonlys[1].tag == 'doonly'
-    assert doonlys[1].items() == [('task', 'bse')]
-    assert doonlys[2].tag == 'doonly'
-    assert doonlys[2].items() == [('task', 'bsegenspec')]
+    assert doonlys[0].tag == "doonly"
+    assert doonlys[0].items() == [("task", "screen")]
+    assert doonlys[1].tag == "doonly"
+    assert doonlys[1].items() == [("task", "bse")]
+    assert doonlys[2].tag == "doonly"
+    assert doonlys[2].items() == [("task", "bsegenspec")]
 
 
 def test_class_ExcitingPlanInput_wrong_plan():
-    plan_input = ['screen', 'bse', 'bsegenspec', 'falseplan']
+    plan_input = ["screen", "bse", "bsegenspec", "falseplan"]
 
     with pytest.raises(ValueError) as error:
         ExcitingXSInput(xstype="BSE", plan=plan_input)
     assert error.value.args[0] == "plan keys are not valid: {'falseplan'}"
 
 
 def test_class_ExcitingXSInput_attribute_setting_getting():
```

### Comparing `excitingtools-1.7.0/tests/obj_parsers/test_eigenvalue_parser.py` & `excitingtools-1.7.1/tests/obj_parsers/test_eigenvalue_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import numpy as np
 import pytest
-from excitingtools.utils.test_utils import MockFile
+
 from excitingtools.exciting_obj_parsers.eigenvalue_parser import parse_eigenvalues
+from excitingtools.utils.test_utils import MockFile
 
 
 @pytest.fixture
 def eigval_xml_mock(tmp_path) -> MockFile:
-    """ Mock 'eigval.xml' data, containing only two k-sampling points.
-    """
+    """Mock 'eigval.xml' data, containing only two k-sampling points."""
     eigval_xml_str = """<?xml version="1.0" encoding="UTF-8"?>
     <eigval>
         <kpt ik="1" vkl="0.000000000000e0 0.000000000000e0 0.000000000000e0">
             <state ist="1" eigenvalue="-3.728453763676e-1" occupancy="2.000000000000e0"/>
             <state ist="2" eigenvalue="4.171109202867e-1" occupancy="2.000000000000e0"/>
             <state ist="3" eigenvalue="4.171125401350e-1" occupancy="2.000000000000e0"/>
             <state ist="4" eigenvalue="4.171125401350e-1" occupancy="2.000000000000e0"/>
@@ -42,18 +42,42 @@
 
 
 def test_parse_eigenvalues(eigval_xml_mock):
     eigval_data = parse_eigenvalues(eigval_xml_mock.file)
 
     ref_k_points = np.array([[0.0, 0.0, 0.0], [0.25, 0.0, 0.0]])
 
-    ref_eigenvalues = np.array([[-0.37284538, 0.41711092, 0.41711254, 0.41711254, 0.62407639, 0.62407733, 0.62407733,
-                                 0.90577707, 1.12982943, 1.39260832],
-                                [-0.30988964, 0.17579802, 0.35365277, 0.35365392, 0.70554696, 0.70554812, 0.71764897,
-                                 0.95780094, 1.18348852, 1.24223224]])
+    ref_eigenvalues = np.array(
+        [
+            [
+                -0.37284538,
+                0.41711092,
+                0.41711254,
+                0.41711254,
+                0.62407639,
+                0.62407733,
+                0.62407733,
+                0.90577707,
+                1.12982943,
+                1.39260832,
+            ],
+            [
+                -0.30988964,
+                0.17579802,
+                0.35365277,
+                0.35365392,
+                0.70554696,
+                0.70554812,
+                0.71764897,
+                0.95780094,
+                1.18348852,
+                1.24223224,
+            ],
+        ]
+    )
 
     ref_occupations = np.array([[2, 2, 2, 2, 0, 0, 0, 0, 0, 0], [2, 2, 2, 2, 0, 0, 0, 0, 0, 0]])
 
     assert eigval_data.state_range.first_state == 1
     assert eigval_data.state_range.last_state == 10
     assert np.allclose(eigval_data.k_points, ref_k_points)
     assert eigval_data.k_indices == [1, 2]
```

### Comparing `excitingtools-1.7.0/tests/obj_parsers/test_gw_eigenvalues.py` & `excitingtools-1.7.1/tests/obj_parsers/test_gw_eigenvalues.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-import numpy as np
-import pytest
 from typing import Tuple
 
-from excitingtools.exciting_obj_parsers.gw_eigenvalues import gw_eigenvalue_parser, _file_name, OxygenEvalQPColumns, \
-    NitrogenEvalQPColumns
-from excitingtools.dataclasses.eigenvalues import EigenValues
+import numpy as np
+import pytest
 
 from excitingtools.dataclasses.data_structs import BandIndices
+from excitingtools.dataclasses.eigenvalues import EigenValues
+from excitingtools.exciting_obj_parsers.gw_eigenvalues import (
+    NitrogenEvalQPColumns,
+    OxygenEvalQPColumns,
+    _file_name,
+    gw_eigenvalue_parser,
+)
 from excitingtools.utils.test_utils import MockFile
 
 
 @pytest.fixture
 def evalqp_nitrogen(tmp_path) -> Tuple[MockFile, BandIndices]:
     evalqp_string = """k-point #     1:    0.000000    0.000000    0.000000    0.015625
 state    E_KS      E_HF       E_GW       Sx         Sc         Vxc         DE_HF        DE_GW       Znk
@@ -47,24 +51,24 @@
  state   E_KS       E_HF       E_GW       Sx         Re(Sc)     Im(Sc)     Vxc        DE_HF      DE_GW      Znk
   19    -0.08099   -0.28150   -0.12905   -0.97072    0.13696   -0.00000   -0.77021   -0.20051   -0.04806    0.75633
   20    -0.08099   -0.28150   -0.12891   -0.97072    0.13710   -0.00000   -0.77021   -0.20051   -0.04792    0.75570
   21    -0.08099   -0.28150   -0.12896   -0.97072    0.13704   -0.00000   -0.77021   -0.20051   -0.04797    0.75582
   22     0.06097    0.32400    0.08958   -0.36222   -0.22727   -0.00000   -0.62524    0.26303    0.02861    0.80010
   23     0.06097    0.32400    0.08957   -0.36222   -0.22728   -0.00000   -0.62524    0.26303    0.02860    0.80006
   24     0.17630    0.38074    0.18396   -0.27546   -0.19505    0.00000   -0.47989    0.20443    0.00766    0.81561
- 
+
 k-point #     2:    0.000000    0.000000    0.500000    0.500000
  state   E_KS       E_HF       E_GW       Sx         Re(Sc)     Im(Sc)     Vxc        DE_HF      DE_GW      Znk
   19    -0.15356   -0.36518   -0.19801   -0.93999    0.15132   -0.00008   -0.72837   -0.21162   -0.04445    0.73712
   20    -0.12231   -0.33123   -0.17047   -0.96038    0.14470   -0.00001   -0.75145   -0.20893   -0.04816    0.74983
   21    -0.12231   -0.33123   -0.17035   -0.96038    0.14482   -0.00001   -0.75145   -0.20893   -0.04804    0.74940
   22     0.08561    0.35313    0.11429   -0.38438   -0.23136    0.00001   -0.65190    0.26752    0.02868    0.79318
   23     0.08561    0.35313    0.11430   -0.38438   -0.23135    0.00001   -0.65190    0.26752    0.02869    0.79323
   24     0.16667    0.43794    0.19514   -0.48319   -0.23505    0.00001   -0.75446    0.27128    0.02848    0.78602
- 
+
 k-point #     3:    0.000000    0.500000    0.500000    0.375000
  state   E_KS       E_HF       E_GW       Sx         Re(Sc)     Im(Sc)     Vxc        DE_HF      DE_GW      Znk
   19    -0.11749   -0.30231   -0.15828   -0.93575    0.13070   -0.00001   -0.75094   -0.18481   -0.04078    0.75361
   20    -0.11749   -0.30231   -0.15818   -0.93575    0.13079   -0.00001   -0.75094   -0.18481   -0.04068    0.75304
   21    -0.06097   -0.25700   -0.10809   -0.99057    0.13377    0.00000   -0.79454   -0.19603   -0.04712    0.75686
   22     0.07678    0.30493    0.09569   -0.40229   -0.20437    0.00000   -0.63044    0.22815    0.01891    0.79516
   23     0.11412    0.40512    0.14613   -0.38364   -0.24999    0.00001   -0.67464    0.29100    0.03201    0.78053
@@ -72,76 +76,85 @@
 """
     file = tmp_path / _file_name
     file.write_text(evalqp_string)
     return MockFile(file, string=evalqp_string), BandIndices(21, 22)
 
 
 def test_parse_evalqp_oxygen(evalqp_oxygen):
-    """ Test that the parser correctly returns to the EigenValues object.
-    """
+    """Test that the parser correctly returns to the EigenValues object."""
     file, band_indices = evalqp_oxygen
     eigen_values: EigenValues = gw_eigenvalue_parser(file.full_path)
 
-    ref_gw_eigenvalues = np.array([[-0.12905, -0.12891, -0.12896,  0.08958,  0.08957,  0.18396],
-                                   [-0.19801, -0.17047, -0.17035,  0.11429,  0.11430,  0.19514],
-                                   [-0.15828, -0.15818, -0.10809,  0.09569,  0.14613,  0.18404]])
-
-    ref_k_points = np.array([[0.000000, 0.000000, 0.000000],
-                             [0.000000, 0.000000, 0.500000],
-                             [0.000000, 0.500000, 0.500000]])
+    ref_gw_eigenvalues = np.array(
+        [
+            [-0.12905, -0.12891, -0.12896, 0.08958, 0.08957, 0.18396],
+            [-0.19801, -0.17047, -0.17035, 0.11429, 0.11430, 0.19514],
+            [-0.15828, -0.15818, -0.10809, 0.09569, 0.14613, 0.18404],
+        ]
+    )
+
+    ref_k_points = np.array(
+        [[0.000000, 0.000000, 0.000000], [0.000000, 0.000000, 0.500000], [0.000000, 0.500000, 0.500000]]
+    )
 
     assert eigen_values.state_range.first_state == 19
     assert eigen_values.state_range.last_state == 24
     assert np.allclose(eigen_values.k_points, ref_k_points)
     assert eigen_values.k_indices == [1, 2, 3]
     assert np.allclose(eigen_values.all_eigenvalues, ref_gw_eigenvalues), "GW column eigenvalues, for all k-points"
     assert eigen_values.weights == [0.125, 0.5, 0.375000]
 
 
 def test_parse_evalqp_oxygen_Znk(evalqp_oxygen):
-    """ Test that the parser correctly returns to the EigenValues object.
-    """
+    """Test that the parser correctly returns to the EigenValues object."""
     file, band_indices = evalqp_oxygen
     eigen_values: EigenValues = gw_eigenvalue_parser(file.full_path, columns=OxygenEvalQPColumns.Znk)
 
-    ref_gw_eigenvalues = np.array([[0.75633, 0.75570, 0.75582, 0.80010, 0.80006, 0.81561],
-                                   [0.73712, 0.74983, 0.74940, 0.79318, 0.79323, 0.78602],
-                                   [0.75361, 0.75304, 0.75686, 0.79516, 0.78053, 0.78971]])
+    ref_gw_eigenvalues = np.array(
+        [
+            [0.75633, 0.75570, 0.75582, 0.80010, 0.80006, 0.81561],
+            [0.73712, 0.74983, 0.74940, 0.79318, 0.79323, 0.78602],
+            [0.75361, 0.75304, 0.75686, 0.79516, 0.78053, 0.78971],
+        ]
+    )
 
     assert np.allclose(eigen_values.all_eigenvalues, ref_gw_eigenvalues), "Znk values, for all k-points"
 
 
 def test_parse_evalqp_nitrogen(evalqp_nitrogen):
-    """ Test that the parser correctly returns to the EigenValues object.
-    """
+    """Test that the parser correctly returns to the EigenValues object."""
     file, band_indices = evalqp_nitrogen
     eigen_values: EigenValues = gw_eigenvalue_parser(file.full_path, NitrogenEvalQPColumns.E_GW)
 
-    ref_gw_eigenvalues = np.array([[-0.03139, -0.03144, -0.03143, 0.08701, 0.08704],
-                                   [-0.17533, -0.05906, -0.05905, 0.06505, 0.12124],
-                                   [-0.28494, -0.07605, -0.07607, 0.04622, 0.11503]])
-
-    ref_k_points = np.array([[0.000000, 0.000000, 0.000000],
-                             [0.000000, 0.000000, 0.250000],
-                             [0.000000, 0.000000, 0.500000]])
+    ref_gw_eigenvalues = np.array(
+        [
+            [-0.03139, -0.03144, -0.03143, 0.08701, 0.08704],
+            [-0.17533, -0.05906, -0.05905, 0.06505, 0.12124],
+            [-0.28494, -0.07605, -0.07607, 0.04622, 0.11503],
+        ]
+    )
+
+    ref_k_points = np.array(
+        [[0.000000, 0.000000, 0.000000], [0.000000, 0.000000, 0.250000], [0.000000, 0.000000, 0.500000]]
+    )
 
     assert eigen_values.state_range.first_state == 10
     assert eigen_values.state_range.last_state == 14
     assert np.allclose(eigen_values.k_points, ref_k_points)
     assert eigen_values.k_indices == [1, 2, 3]
     assert np.allclose(eigen_values.all_eigenvalues, ref_gw_eigenvalues), "GW column eigenvalues, for all k-points"
     assert eigen_values.weights == [0.015625, 0.125, 0.0625]
 
 
 def test_parse_evalqp_incompatible(evalqp_nitrogen):
-    """ Test for the exception.
+    """Test for the exception.
     Trying to parse _filename generated with nitrogen, but requesting oxygen column indexing.
     """
     file, band_indices = evalqp_nitrogen
 
     with pytest.raises(ValueError) as error:
-        eigen_values: EigenValues = gw_eigenvalue_parser(file.full_path,
-                                                         OxygenEvalQPColumns.E_GW)
-    assert error.value.args[
-               0] == "The requested data column is indexed according to exciting version OxygenEvalQPColumns," \
-                     "which is not consistent with the columns of the parsed data. " \
-                     "Check that your data was produced with the same code version."
+        gw_eigenvalue_parser(file.full_path, OxygenEvalQPColumns.E_GW)
+    assert (
+        error.value.args[0] == "The requested data column is indexed according to exciting version OxygenEvalQPColumns,"
+        "which is not consistent with the columns of the parsed data. "
+        "Check that your data was produced with the same code version."
+    )
```

### Comparing `excitingtools-1.7.0/tests/obj_parsers/test_input_parser.py` & `excitingtools-1.7.1/tests/obj_parsers/test_input_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,9 +54,9 @@
   
 </input>
 """
 
 
 def test_parse_input_xml_to_object():
     input_xml = parse_input_xml(reference_input_str)
-    assert set(vars(input_xml)) == {'xs', 'groundstate', 'structure', 'title'}
+    assert set(vars(input_xml)) == {"xs", "groundstate", "structure", "title"}
     assert input_xml.to_xml_str().startswith('<?xml version="1.0" ?>\n<input>\n\t<title>Lithium Fluoride BSE')
```

### Comparing `excitingtools-1.7.0/tests/parser_utils/test_parser_utils.py` & `excitingtools-1.7.1/tests/parser_utils/test_parser_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,54 @@
-""" Tests for parser utils. """
+"""Tests for parser utils."""
+
 import pytest
 
-from excitingtools.parser_utils.parser_utils import json_convert, standardise_fortran_exponent, \
-    convert_single_entry, convert_string_dict
+from excitingtools.parser_utils.parser_utils import (
+    convert_single_entry,
+    convert_string_dict,
+    json_convert,
+    standardise_fortran_exponent,
+)
 
 
 @pytest.mark.parametrize(
     "test_input,expected",
-    [("true", True), ("false", False), ("fromscratch", "fromscratch"), ("skip", "skip"), ("3", 3), ("-1", -1),
-     ("2.34", 2.34), ("5.1e3", 5100)]
+    [
+        ("true", True),
+        ("false", False),
+        ("fromscratch", "fromscratch"),
+        ("skip", "skip"),
+        ("3", 3),
+        ("-1", -1),
+        ("2.34", 2.34),
+        ("5.1e3", 5100),
+    ],
 )
 def test_convert_json(test_input, expected):
     assert json_convert(test_input) == expected
 
 
 @pytest.mark.parametrize("test_input,expected", [("23.2D-1", 2.32), ("1q0", 1)])
 def test_convert_fortran_exponent(test_input, expected):
     assert standardise_fortran_exponent(test_input, return_as_str=False) == expected
 
 
 @pytest.mark.parametrize(
     "test_input,expected",
-    [("true", True), ("skip", "skip"), ("3", 3), ("2.34", 2.34), ("true false false", [True, False, False]),
-     ("1.3 2.3e4 3 90", [1.3, 2.3e4, 3, 90]), ("4 4 3", [4, 4, 3]), ("1 2", [1, 2]), ("ab cd", "ab cd")]
+    [
+        ("true", True),
+        ("skip", "skip"),
+        ("3", 3),
+        ("2.34", 2.34),
+        ("true false false", [True, False, False]),
+        ("1.3 2.3e4 3 90", [1.3, 2.3e4, 3, 90]),
+        ("4 4 3", [4, 4, 3]),
+        ("1 2", [1, 2]),
+        ("ab cd", "ab cd"),
+    ],
 )
 def test_convert_single_entry(test_input, expected):
     assert convert_single_entry(test_input) == expected
 
 
 def test_convert_single_entry_to_int():
     converted_int = convert_single_entry("3")
```

### Comparing `excitingtools-1.7.0/tests/parser_utils/test_regex_parser.py` & `excitingtools-1.7.1/tests/parser_utils/test_regex_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,76 +1,80 @@
 """
 Test regex parser wrappers
 """
+
 import pytest
 
 from excitingtools.parser_utils.regex_parser import parse_value_regex
 
 
 def test_parse_value_regex():
-
     test_string = """
     --------------------------------------------------------------------------------
     -                               frequency grid                                 -
     --------------------------------------------------------------------------------
-     
-     Type: < fgrid > gauleg2                                 
-     Frequency axis: < fconv > imfreq                                  
+
+     Type: < fgrid > gauleg2
+     Frequency axis: < fconv > imfreq
      Number of frequencies: < nomeg >           32
-     Cutoff frequency: < freqmax >    1.00000000000000  
-    
+     Cutoff frequency: < freqmax >    1.00000000000000
+
     --------------------------------------------------------------------------------
     -                          Kohn-Sham band structure                            -
     --------------------------------------------------------------------------------
-     
+
      Fermi energy:     0.0000
      Energy range:   -14.6863 1030.7919
      Band index of VBM:  21
      Band index of CBm:  22
-     
+
      Indirect BandGap (eV):                    3.3206
      at k(VBM) =    0.000   0.500   0.500 ik =     3
         k(CBm) =    0.000   0.000   0.000 ik =     1
      Direct Bandgap at k(VBM) (eV):            3.7482
      Direct Bandgap at k(CBm) (eV):            3.8653
-     
+
      --------------------------------------------------------------------------------
      -                            G0W0 band structure                               -
      --------------------------------------------------------------------------------
-      
+
       Fermi energy:    -0.0054
       Energy range:   -16.2632 1031.4090
       Band index of VBM:  21
       Band index of CBm:  22
-      
+
       Indirect BandGap (eV):                    5.3920
       at k(VBM) =    0.000   0.500   0.500 ik =     3
          k(CBm) =    0.000   0.000   0.000 ik =     1
       Direct Bandgap at k(VBM) (eV):            5.5472
       Direct Bandgap at k(CBm) (eV):            5.9646
     """
 
-    assert {'Fermi energy': 0.0} == parse_value_regex(test_string, 'Fermi energy:'), \
-        "Expect to match first string instance and return {key:float}"
-
-    assert {'Indirect BandGap (eV)': 3.3206} == parse_value_regex(test_string, 'Indirect BandGap \\(eV\\):'), \
-       "Expect to match first string instance and return {key:float}"
-
-    assert {'Energy range': [-14.6863, 1030.7919]} == parse_value_regex(test_string, 'Energy range:'), \
-        "Expect to match first string instance and return {key:List[float]}"
-
-    assert {'Type: < fgrid >': 'gauleg2'} == parse_value_regex(test_string, 'Type: < fgrid >'), \
-        "Expect to match first string instance and return {key:str}"
+    assert {"Fermi energy": 0.0} == parse_value_regex(
+        test_string, "Fermi energy:"
+    ), "Expect to match first string instance and return {key:float}"
+
+    assert {"Indirect BandGap (eV)": 3.3206} == parse_value_regex(
+        test_string, "Indirect BandGap \\(eV\\):"
+    ), "Expect to match first string instance and return {key:float}"
+
+    assert {"Energy range": [-14.6863, 1030.7919]} == parse_value_regex(
+        test_string, "Energy range:"
+    ), "Expect to match first string instance and return {key:List[float]}"
+
+    assert {"Type: < fgrid >": "gauleg2"} == parse_value_regex(
+        test_string, "Type: < fgrid >"
+    ), "Expect to match first string instance and return {key:str}"
 
 
 @pytest.mark.xfail
 def test_failures_with_parse_value_regex():
     """
     This fails for timings because matching 'Initialization' returns ':        15.46',
     (for example), and the colon cannot be interpreted by eval()
     """
     test_string = """
      Initialization                             :        15.46
          - init_scf                             :         8.38
     """
 
-    data = parse_value_regex(test_string, 'Initialization')
+    parse_value_regex(test_string, "Initialization")
```

### Comparing `excitingtools-1.7.0/tests/parser_utils/test_simple_parser.py` & `excitingtools-1.7.1/tests/parser_utils/test_simple_parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,51 @@
 """
 Test parsers in simple_parser
 """
 
-from excitingtools.parser_utils.simple_parser import match_current_return_line_n, \
-    match_current_extract_from_line_n
+from excitingtools.parser_utils.simple_parser import match_current_extract_from_line_n, match_current_return_line_n
 
 
 def test_match_current_return_next_n():
-
     input_string = """
        Tolerance factor to reduce the MB size based on
        the eigenvectors of the bare Coulomb potential:   0.100000000000000     
      
     --------------------------------------------------------------------------------
      
      Screened Coulomb potential:
        Full-frequency Random-Phase Approximation
        Some additional data : 5
      """
 
-    string_match = match_current_return_line_n(
-        input_string, 'Screened Coulomb potential:', n_line=1
-        )
-    assert string_match.strip() == "Full-frequency Random-Phase Approximation", \
-        "Expect to return the string one line below the match"
-
-    string_match = match_current_return_line_n(input_string, 'Screened Coulomb potential:')
-    assert string_match.strip() == "Full-frequency Random-Phase Approximation", \
-        "Expect default behaviour to return the string one line below the match"
-
-    string_match = match_current_return_line_n(
-        input_string, 'Screened Coulomb potential:', n_line=2
-        )
-    assert string_match.strip() == "Some additional data : 5", \
-        "Expect to return the string two lines below the match"
+    string_match = match_current_return_line_n(input_string, "Screened Coulomb potential:", n_line=1)
+    assert (
+        string_match.strip() == "Full-frequency Random-Phase Approximation"
+    ), "Expect to return the string one line below the match"
+
+    string_match = match_current_return_line_n(input_string, "Screened Coulomb potential:")
+    assert (
+        string_match.strip() == "Full-frequency Random-Phase Approximation"
+    ), "Expect default behaviour to return the string one line below the match"
 
+    string_match = match_current_return_line_n(input_string, "Screened Coulomb potential:", n_line=2)
+    assert string_match.strip() == "Some additional data : 5", "Expect to return the string two lines below the match"
 
-def test_match_current_extract_from_line_n():
 
+def test_match_current_extract_from_line_n():
     input_string = """
        Tolerance factor to reduce the MB size based on
        the eigenvectors of the bare Coulomb potential:   0.100000000000000     
 
     --------------------------------------------------------------------------------
 
      Screened Coulomb potential:
        Full-frequency Random-Phase Approximation
        Some additional data : 5
      """
 
     # Extract 5 from "Some additional data : 5"
-    key_extraction = {'Screened Coulomb potential:': lambda x: int(x.split(':')[-1])}
+    key_extraction = {"Screened Coulomb potential:": lambda x: int(x.split(":")[-1])}
 
     data = match_current_extract_from_line_n(input_string, key_extraction, n_line=2)
 
-    assert data == {'Screened Coulomb potential:': 5}, \
-        "Expect to return the integer from 2 lines below the match key"
+    assert data == {"Screened Coulomb potential:": 5}, "Expect to return the integer from 2 lines below the match key"
```

### Comparing `excitingtools-1.7.0/tests/runner/test_runner.py` & `excitingtools-1.7.1/tests/runner/test_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 
 mock_binary = "false_exciting_binary"
 
 
 @pytest.mark.xfail(shutil.which(mock_binary) is not None, reason="Binary name exists.")
 def test_no_binary():
     my_runner = BinaryRunner(mock_binary, "./", 1, 1)
-    with pytest.raises(FileNotFoundError,
-                       match=fr"{mock_binary} binary is not present in the current directory nor in \$PATH"):
+    with pytest.raises(
+        FileNotFoundError, match=rf"{mock_binary} binary is not present in the current directory nor in \$PATH"
+    ):
         my_runner.run()
 
 
 @pytest.fixture
 def exciting_smp(tmp_path: Path) -> str:
     binary = tmp_path / "exciting_smp"
     binary.touch()
@@ -68,39 +69,44 @@
 def test_false_timeout(exciting_smp: str):
     with pytest.raises(ValueError, match="time_out must be a positive integer"):
         BinaryRunner(exciting_smp, [""], 1, -1)
 
 
 @pytest.fixture
 def runner(tmp_path: Path, exciting_mpismp: str) -> BinaryRunner:
-    """Produces a runner with binary and run dir mocked up.
-    """
+    """Produces a runner with binary and run dir mocked up."""
     run_dir = tmp_path / "ab/de"
     run_dir.mkdir(parents=True)
     return BinaryRunner(exciting_mpismp, ["mpirun", "-np", "3"], 4, 260, run_dir.as_posix(), [">", "std.out"])
 
 
-def test_as_dict(tmp_path: Path, runner: BinaryRunner, mock_env_jobflow_missing):
-    assert runner.as_dict() == {'args': ['>', 'std.out'],
-                                'binary': (tmp_path / "exciting_mpismp").as_posix(),
-                                'directory': (tmp_path / "ab/de").as_posix(),
-                                'omp_num_threads': 4,
-                                'run_cmd': ['mpirun', '-np', '3'],
-                                'time_out': 260}
-
-
-def test_as_dict_jobflow(tmp_path: Path, runner: BinaryRunner, mock_env_jobflow):
-    assert runner.as_dict() == {'@class': 'BinaryRunner',
-                                '@module': 'excitingtools.runner.runner',
-                                'args': ['>', 'std.out'],
-                                'binary': (tmp_path / "exciting_mpismp").as_posix(),
-                                'directory': (tmp_path / "ab/de").as_posix(),
-                                'omp_num_threads': 4,
-                                'run_cmd': ['mpirun', '-np', '3'],
-                                'time_out': 260}
+@pytest.mark.usefixtures("mock_env_jobflow_missing")
+def test_as_dict(tmp_path: Path, runner: BinaryRunner):
+    assert runner.as_dict() == {
+        "args": [">", "std.out"],
+        "binary": (tmp_path / "exciting_mpismp").as_posix(),
+        "directory": (tmp_path / "ab/de").as_posix(),
+        "omp_num_threads": 4,
+        "run_cmd": ["mpirun", "-np", "3"],
+        "time_out": 260,
+    }
+
+
+@pytest.mark.usefixtures("mock_env_jobflow")
+def test_as_dict_jobflow(tmp_path: Path, runner: BinaryRunner):
+    assert runner.as_dict() == {
+        "@class": "BinaryRunner",
+        "@module": "excitingtools.runner.runner",
+        "args": [">", "std.out"],
+        "binary": (tmp_path / "exciting_mpismp").as_posix(),
+        "directory": (tmp_path / "ab/de").as_posix(),
+        "omp_num_threads": 4,
+        "run_cmd": ["mpirun", "-np", "3"],
+        "time_out": 260,
+    }
 
 
 def test_from_dict(tmp_path: Path, runner):
     new_runner = BinaryRunner.from_dict(runner.as_dict())
     assert new_runner.binary == (tmp_path / "exciting_mpismp").as_posix()
     assert new_runner.time_out == 260
 
@@ -112,27 +118,27 @@
     run_dir = tmp_path / "ab/de"
     run_dir.mkdir(parents=True)
     binary = tmp_path / "hello"
     binary.touch()
     runner = BinaryRunner(binary.as_posix(), ["echo"], 1, 60, run_dir.as_posix())
     run_results = runner.run()
     assert run_results.success
-    assert run_results.stderr == ''
+    assert run_results.stderr == ""
     assert run_results.stdout == binary.as_posix() + "\n"
 
 
 def test_timeout_with_bash_command(tmp_path: Path):
     """Produces a runner with binary and run dir mocked up.
 
     Test a simple sleep command to get a timeout.
     """
     time_out = 1
     binary = tmp_path / "sleep.sh"
     binary.write_text(f"sleep {time_out + 0.1}")
     runner = BinaryRunner(binary.as_posix(), ["sh"], 1, time_out, tmp_path.as_posix())
     run_results = runner.run()
     assert not run_results.success
-    assert run_results.stderr == 'BinaryRunner: Job timed out. \n\n'
+    assert run_results.stderr == "BinaryRunner: Job timed out. \n\n"
     assert run_results.stdout == ""
     assert run_results.process_time == time_out
     assert isinstance(run_results.return_code, RunnerCode)
     assert run_results.return_code == RunnerCode.time_out
```

### Comparing `excitingtools-1.7.0/tests/structure/test_lattice.py` & `excitingtools-1.7.1/tests/structure/test_lattice.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
-Tests for functions in lattice.py 
+Tests for functions in lattice.py
 """
+
 import numpy as np
 
-from excitingtools.structure.lattice import reciprocal_lattice_vectors, parallelepiped_volume, plane_transformation
 from excitingtools.math.math_utils import triple_product
+from excitingtools.structure.lattice import parallelepiped_volume, plane_transformation, reciprocal_lattice_vectors
 
 
 def test_parallelepiped_volume():
-
     # FCC lattice vectors with arbitrary lattice constant
-    a = 3.2 * np.array([[0., 1., 1.], [1., 0., 1.], [1., 1., 0.]])
+    a = 3.2 * np.array([[0.0, 1.0, 1.0], [1.0, 0.0, 1.0], [1.0, 1.0, 0.0]])
 
     triple_product_result = triple_product(a[:, 0], a[:, 1], a[:, 2])
     volume = parallelepiped_volume(np.array([a[:, 0], a[:, 1], a[:, 2]]))
 
     assert np.isclose(triple_product_result, 65.5360)
     assert np.isclose(volume, 65.5360)
 
@@ -29,38 +29,36 @@
     r"""
     Test
         \mathbf{a}_i \cdot \mathbf{b}_j = 2 \pi \delta_{ij}
 
     """
 
     # fcc with arbitrary lattice constant
-    a = 3.2 * np.array([[0., 1., 1.], [1., 0., 1.], [1., 1., 0.]])
+    a = 3.2 * np.array([[0.0, 1.0, 1.0], [1.0, 0.0, 1.0], [1.0, 1.0, 0.0]])
     b = reciprocal_lattice_vectors(a)
 
     assert a.shape == (3, 3)
     assert b.shape == (3, 3)
 
     a_dot_b = np.transpose(a) @ b
     off_diagonal_indices = np.where(~np.eye(a_dot_b.shape[0], dtype=bool))
     off_diagonal_elements = a_dot_b[off_diagonal_indices]
 
     assert np.allclose(a_dot_b.diagonal(), 2 * np.pi)
-    assert np.allclose(off_diagonal_elements, 0.)
+    assert np.allclose(off_diagonal_elements, 0.0)
 
 
 def test_plane_transformation():
     """
     Test plane_transformation function.
     """
-    rec_lat_vec = np.array([[-0.042506, -0.042506,  0.050235],
-                         [-0.042506,  0.050235, -0.042506],
-                         [-0.085013,  0.007728,  0.007728]]
-                       )
-
-    plot_vec = np.array([[-0.5881478,  0.5881478,  0.5881478],
-                            [ 0.5881478, -0.5881478,  0.5881478],
-                            [ 0.5881478,  0.5881478, -0.5881478]]
-                          )
+    rec_lat_vec = np.array(
+        [[-0.042506, -0.042506, 0.050235], [-0.042506, 0.050235, -0.042506], [-0.085013, 0.007728, 0.007728]]
+    )
+
+    plot_vec = np.array(
+        [[-0.5881478, 0.5881478, 0.5881478], [0.5881478, -0.5881478, 0.5881478], [0.5881478, 0.5881478, -0.5881478]]
+    )
     # This is supposed to be 3x3 Identity
     transformation_matrix = plane_transformation(rec_lat_vec, plot_vec)
 
-    assert np.allclose(transformation_matrix.dot(rec_lat_vec)[2,:], 0.0, atol=1e-6)
+    assert np.allclose(transformation_matrix.dot(rec_lat_vec)[2, :], 0.0, atol=1e-6)
```

### Comparing `excitingtools-1.7.0/tests/structure/test_pymatgen_utilities.py` & `excitingtools-1.7.1/tests/structure/test_pymatgen_utilities.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,50 @@
-""" Tests for pymatgen utilities. """
+"""Tests for pymatgen utilities."""
+
 import numpy as np
 import pytest
 
 
 @pytest.fixture
 def pymatgen_atoms_H2O():
     """
     H20 molecule in a big box (angstrom), in pymatgen Structure()
     Converts a List[dict] to pymatgen.core.structure.Structure.
     """
     pymatgen_struct = pytest.importorskip("pymatgen.core.structure")
     cubic_cell = np.array([[10.0, 0.0, 0.0], [0.0, 10.0, 0.0], [0.0, 0.0, 10.0]])
-    atoms = [{'species': 'H', 'position': [0.00000, 0.75545, -0.47116]},
-             {'species': 'O', 'position': [0.00000, 0.00000, 0.11779]},
-             {'species': 'H', 'position': [0.00000, 0.75545, -0.47116]}]
+    atoms = [
+        {"species": "H", "position": [0.00000, 0.75545, -0.47116]},
+        {"species": "O", "position": [0.00000, 0.00000, 0.11779]},
+        {"species": "H", "position": [0.00000, 0.75545, -0.47116]},
+    ]
 
-    symbols = [atom['species'] for atom in atoms]
-    positions = [atom['position'] for atom in atoms]
+    symbols = [atom["species"] for atom in atoms]
+    positions = [atom["position"] for atom in atoms]
     return pymatgen_struct.Structure(lattice=cubic_cell, species=symbols, coords=positions, coords_are_cartesian=True)
 
 
 def test_class_exciting_structure_pymatgen(pymatgen_atoms_H2O):
     """
     Test the pymatgen Structure object gets used correctly by the ExcitingStructure constructor.
     """
     pymatgen_conversion = pytest.importorskip("excitingtools.structure.pymatgen_utilities")
     structure = pymatgen_conversion.pymatgen_to_exciting_structure(pymatgen_atoms_H2O)
 
     assert structure.species == ["H", "O", "H"]
-    assert np.allclose(structure.lattice,
-                       [[18.897261246257703, 0.0, 0.0],
-                        [0.0, 18.897261246257703, 0.0],
-                        [0.0, 0.0, 18.897261246257703]]), \
-        'Expect lattice vectors to match input values'
+    assert np.allclose(
+        structure.lattice,
+        [[18.897261246257703, 0.0, 0.0], [0.0, 18.897261246257703, 0.0], [0.0, 0.0, 18.897261246257703]],
+    ), "Expect lattice vectors to match input values"
 
-    assert np.allclose(structure.positions, pymatgen_atoms_H2O.frac_coords), 'Expect positions to match input values.'
+    assert np.allclose(structure.positions, pymatgen_atoms_H2O.frac_coords), "Expect positions to match input values."
 
     # This just confirms the XML tree is built, not that it is correct.
     xml_structure = structure.to_xml()
-    assert list(xml_structure.keys()) == ['speciespath'], 'Only expect speciespath in structure xml keys'
+    assert list(xml_structure.keys()) == ["speciespath"], "Only expect speciespath in structure xml keys"
 
 
 def test_class_exciting_structure_to_pymatgen(pymatgen_atoms_H2O):
     pymatgen_conversion = pytest.importorskip("excitingtools.structure.pymatgen_utilities")
     structure = pymatgen_conversion.pymatgen_to_exciting_structure(pymatgen_atoms_H2O)
     new_pymatgen_atoms = pymatgen_conversion.exciting_structure_to_pymatgen(structure)
     assert pymatgen_atoms_H2O == new_pymatgen_atoms
```

### Comparing `excitingtools-1.7.0/tests/utils/test_dict_utils.py` & `excitingtools-1.7.1/tests/utils/test_dict_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,204 +1,150 @@
 """
 Tests for functions in dict_utils.py
 """
+
 import numpy as np
 
-from excitingtools.utils.dict_utils import container_converter, serialise_dict_values, delete_nested_key
+from excitingtools.utils.dict_utils import container_converter, delete_nested_key, serialise_dict_values
 
 
 def test_convert_container():
     """Test container_converter function on string values in a dict."""
     input = {
-        'a': '5.0',
-        'b': ['1.0', '10.0'],
-        'c': {
-            'a1': '1.0'
-        },
-        'd': "blu",
-        'e': [['1', '2.3'], '3'],
-        'f': ['1', 'a']
-    }
-    expected = {
-        'a': 5.0,
-        'b': [1.0, 10.0],
-        'c': {
-            'a1': 1.0
-        },
-        'd': "blu",
-        'e': [[1, 2.3], 3],
-        'f': [1, 'a']
+        "a": "5.0",
+        "b": ["1.0", "10.0"],
+        "c": {"a1": "1.0"},
+        "d": "blu",
+        "e": [["1", "2.3"], "3"],
+        "f": ["1", "a"],
     }
+    expected = {"a": 5.0, "b": [1.0, 10.0], "c": {"a1": 1.0}, "d": "blu", "e": [[1, 2.3], 3], "f": [1, "a"]}
 
-    assert container_converter(input) == expected, (
-        'String value/s failed to convert to numerical values')
+    assert container_converter(input) == expected, "String value/s failed to convert to numerical values"
 
 
 def test_convert_container_no_strings():
     """Test container_converter where there are no string values in dict."""
-    input = {
-        'a': 5.0,
-        'b': [1.0, 10.0],
-        'c': {
-            'a1': 1.0
-        },
-        'd': "blu",
-        'e': [[1, 2.3], 3],
-        'f': [1, 11.3]
-    }
+    input = {"a": 5.0, "b": [1.0, 10.0], "c": {"a1": 1.0}, "d": "blu", "e": [[1, 2.3], 3], "f": [1, 11.3]}
 
-    assert container_converter(input) == input, (
-        "Expect the converter to do nothing")
+    assert container_converter(input) == input, "Expect the converter to do nothing"
 
 
 def test_convert_container_data_type():
-    input = {
-        'a': '5.0',
-        'b': ['1.0', '10.0'],
-        'c': {
-            'a1': '1.0'
-        },
-        'd': "blu",
-        'e': [['1', '2.3'], '3']
-    }
-    expected = {
-        'a': 5.0,
-        'b': [1.0, 10.0],
-        'c': {
-            'a1': 1.0
-        },
-        'd': "blu",
-        'e': [[1, 2.3], 3]
-    }
+    input = {"a": "5.0", "b": ["1.0", "10.0"], "c": {"a1": "1.0"}, "d": "blu", "e": [["1", "2.3"], "3"]}
+    expected = {"a": 5.0, "b": [1.0, 10.0], "c": {"a1": 1.0}, "d": "blu", "e": [[1, 2.3], 3]}
 
     output = container_converter(input)
 
     for elem1, elem2 in zip(output.values(), expected.values()):
         assert type(elem1) == type(elem2)
-    for elem, elem2 in zip(output['c'].values(), expected['c'].values()):
+    for elem, elem2 in zip(output["c"].values(), expected["c"].values()):
         assert type(elem) == type(elem2)
-    for elem, elem2 in zip(output['b'], expected['b']):
+    for elem, elem2 in zip(output["b"], expected["b"]):
         assert type(elem) == type(elem2)
-    for elem, elem2 in zip(output['e'], expected['e']):
+    for elem, elem2 in zip(output["e"], expected["e"]):
         assert type(elem) == type(elem2)
-    for elem, elem2 in zip(output['e'][0], expected['e'][0]):
+    for elem, elem2 in zip(output["e"][0], expected["e"][0]):
         assert type(elem) == type(elem2)
 
-    assert output == expected, (
-        "Output is consistent with the expected dictionary")
+    assert output == expected, "Output is consistent with the expected dictionary"
 
 
 class Mock:
-
     def __init__(self, a, b):
         self.a = a
         self.b = b
 
 
 def test_serialise_dict_values():
-
     # Value is an object
-    input = {'mock_key': Mock(1, 2)}
+    input = {"mock_key": Mock(1, 2)}
     output = serialise_dict_values(input)
-    assert output == {
-        'mock_key': {
-            'a': 1,
-            'b': 2
-        }
-    }, "Convert object values to dicts"
+    assert output == {"mock_key": {"a": 1, "b": 2}}, "Convert object values to dicts"
 
     # Object nested in a dictionary
-    input = {'mock_key': {'another-key': Mock(1, 2)}}
+    input = {"mock_key": {"another-key": Mock(1, 2)}}
     output = serialise_dict_values(input)
-    assert output == {
-        'mock_key': {
-            'another-key': {
-                'a': 1,
-                'b': 2
-            }
-        }
-    }, "Convert nested object values into dicts"
+    assert output == {"mock_key": {"another-key": {"a": 1, "b": 2}}}, "Convert nested object values into dicts"
 
     # Object nested in a list, and within a dictionary within a list
-    input = {'a': [1, 2, Mock(3, 4), {'b': Mock(5, 6)}]}
+    input = {"a": [1, 2, Mock(3, 4), {"b": Mock(5, 6)}]}
     output = serialise_dict_values(input)
-    assert output == {'a': [1, 2, {'a': 3, 'b': 4}, {'b': {'a': 5, 'b': 6}}]}, \
-        "Convert nested object values into dicts, where the top-level container value is a list"
+    assert output == {
+        "a": [1, 2, {"a": 3, "b": 4}, {"b": {"a": 5, "b": 6}}]
+    }, "Convert nested object values into dicts, where the top-level container value is a list"
 
 
 def test_serialise_dict_value_is_tuple():
-
     # Object nested in a dictionary, nested within a tuple
-    input = {'mock_key': (1, {'another-key': Mock(1, 2)})}
+    input = {"mock_key": (1, {"another-key": Mock(1, 2)})}
     output = serialise_dict_values(input)
-    assert output == {'mock_key': [1, {'another-key': {'a': 1, 'b': 2}}]}, \
-        "Convert nested object values into dicts, where the top-level container value is a tuple." \
+    assert output == {"mock_key": [1, {"another-key": {"a": 1, "b": 2}}]}, (
+        "Convert nested object values into dicts, where the top-level container value is a tuple."
         "Note, tuple cannot be mutated so it is converted to a list by serialise_dict_values"
+    )
 
 
 def test_serialise_dict_value_is_set():
-
     # Object nested in a dictionary, nested within a set
-    input = {'mock_key': {1, 2, Mock(1, 2)}}
+    input = {"mock_key": {1, 2, Mock(1, 2)}}
     output = serialise_dict_values(input)
 
-    output_keys = [k for k in output.keys()]
-    output_values = [v for v in output.values()]
-
-    assert len(output_keys) == 1
-    assert output_keys[0] == 'mock_key'
-    assert len(output_values) == 1
+    assert len(output) == 1
+    assert next(iter(output)) == "mock_key"
+    assert len(output.values()) == 1
 
     # Mock object -> dictionary, meaning one cannot compare the input and outout with collections.Counter,
     # sets or sorted (neither object nor dictionary is hashable)
     def unordered_lists_the_same(a: list, b: list) -> bool:
         """
         Check contents of two lists are consistent, irregardless of order
         """
-        for element in a:
-            try:
+        try:
+            for element in a:
                 b.remove(element)
-            except ValueError:
-                return False
+        except ValueError:
+            return False
         return not b
 
-    assert unordered_lists_the_same(output_values[0], [1, 2, {'a': 1, 'b': 2}]), \
-        "Convert nested object values into dicts, where the top-level container value is a set. " \
+    assert unordered_lists_the_same(next(iter(output.values())), [1, 2, {"a": 1, "b": 2}]), (
+        "Convert nested object values into dicts, where the top-level container value is a set. "
         "Note, set is not iterable and is converted to a list with some arbitrary order by serialise_dict_values"
+    )
 
 
 def test_serialise_dict_values_null_behaviour():
-    """"
+    """ "
     Test serialize_dict_values on different dict key types.
     """
-    input = {'mock_key': [1, 2]}
+    input = {"mock_key": [1, 2]}
     output = serialise_dict_values(input)
     assert output == input, "Pass over list values"
 
-    input = {'mock_key': (1, 2)}
+    input = {"mock_key": (1, 2)}
     output = serialise_dict_values(input)
     assert output == input, "Pass over tuple values"
 
-    input = {'mock_key': {1, 2}}
+    input = {"mock_key": {1, 2}}
     output = serialise_dict_values(input)
     assert output == input, "Pass over set values"
 
-    input = {'mock_key': np.array([1., 2., 3.])}
+    input = {"mock_key": np.array([1.0, 2.0, 3.0])}
     output = serialise_dict_values(input)
     assert output == input, "Pass over np.array values"
 
 
 def test_delete_nested_key():
     """
     Test delete_nested_key removes a key from dict.
     """
-    input = {'a': {'b': 1, 'c': {'d': 1, 'e': 2}}}
-    key_to_remove = ['a']
+    input = {"a": {"b": 1, "c": {"d": 1, "e": 2}}}
+    key_to_remove = ["a"]
     delete_nested_key(input, key_to_remove)
     output = {}
     assert output == input
 
-    input = {'a': {'b': 1, 'c': {'d': 1, 'e': 2}}}
-    key_to_remove = ['a', 'c', 'd']
+    input = {"a": {"b": 1, "c": {"d": 1, "e": 2}}}
+    key_to_remove = ["a", "c", "d"]
     delete_nested_key(input, key_to_remove)
-    output = {'a': {'b': 1, 'c': {'e': 2}}}
+    output = {"a": {"b": 1, "c": {"e": 2}}}
     assert output == input
```

### Comparing `excitingtools-1.7.0/tests/utils/test_utils.py` & `excitingtools-1.7.1/tests/utils/test_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,40 @@
-""" Tests for utils. """
-from excitingtools.utils.utils import can_be_float, convert_to_literal, get_new_line_indices, flatten_list
+"""Tests for utils."""
+
+from excitingtools.utils.utils import can_be_float, convert_to_literal, flatten_list, get_new_line_indices
 
 
 def test_can_be_float():
     """
     Test can_be_float function on different input types.
     """
-    assert can_be_float('1.0'), (
-        "Expect string of a literal '1.0' can convert to float")
-    assert can_be_float('1'), (
-        "Expect string of a literal '1' can convert to float")
-    assert can_be_float(True), (
-        "Expect True can be converted to a float (would be 1.0)")
-    assert can_be_float('a') is False, (
-        "Expect string of the letter 'a' cannot be converted to a float")
+    assert can_be_float("1.0"), "Expect string of a literal '1.0' can convert to float"
+    assert can_be_float("1"), "Expect string of a literal '1' can convert to float"
+    assert can_be_float(True), "Expect True can be converted to a float (would be 1.0)"
+    assert can_be_float("a") is False, "Expect string of the letter 'a' cannot be converted to a float"
 
 
 def test_convert_to_literal():
     """
     Test convert_to_literal turns string reps of numeric data into numeric data.
     """
-    assert convert_to_literal('1.1') == 1.1, "string of literal '1.1' converts to float"
-    assert convert_to_literal('1.0') == 1.0, "string of literal '1.0' converts to float"
-    assert convert_to_literal('1') == 1, "string of literal '1' converts to int"
+    assert convert_to_literal("1.1") == 1.1, "string of literal '1.1' converts to float"
+    assert convert_to_literal("1.0") == 1.0, "string of literal '1.0' converts to float"
+    assert convert_to_literal("1") == 1, "string of literal '1' converts to int"
 
 
 def test_get_new_line_indices():
     """
     Test getting new line indices function.
     """
-    test_string = 'Test Here\n 2nd Line'
+    test_string = "Test Here\n 2nd Line"
     expected_line_indices = 2
     expected_line_index_list = [0, 10]
     assert len(get_new_line_indices(test_string)) == expected_line_indices
     assert get_new_line_indices(test_string)[0] == expected_line_index_list[0]
     assert get_new_line_indices(test_string)[1] == expected_line_index_list[1]
 
 
 def test_flatten_list():
-    input_list = [[1, 2, 3], 4, 5, [6, [7, 8]], {'9': 9, '10': 10}]
-    ref_list = [1, 2, 3, 4, 5, 6, 7, 8, {'9': 9, '10': 10}]
+    input_list = [[1, 2, 3], 4, 5, [6, [7, 8]], {"9": 9, "10": 10}]
+    ref_list = [1, 2, 3, 4, 5, 6, 7, 8, {"9": 9, "10": 10}]
     assert list(flatten_list(input_list)) == ref_list
```

