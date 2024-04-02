# Comparing `tmp/typedal-3.0.0b3.tar.gz` & `tmp/typedal-3.0.0b4.tar.gz`

## Comparing `typedal-3.0.0b3.tar` & `typedal-3.0.0b4.tar`

### file list

```diff
@@ -1,2158 +1,2158 @@
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.readthedocs.yml
--rw-r--r--   0        0        0    18226 2020-02-02 00:00:00.000000 typedal-3.0.0b3/CHANGELOG.md
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 typedal-3.0.0b3/coverage.svg
--rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 typedal-3.0.0b3/example_new.py
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 typedal-3.0.0b3/example_old.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 typedal-3.0.0b3/mkdocs.yml
--rwxr-xr-x   0        0        0      314 2020-02-02 00:00:00.000000 typedal-3.0.0b3/start_dummy_pg.sh
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.github/workflows/su6.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/@plugins_snapshot.json
--rw-r--r--   0        0        0   177667 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/_ast.data.json
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/_ast.meta.json
--rw-r--r--   0        0        0    52400 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/_codecs.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/_codecs.meta.json
--rw-r--r--   0        0        0    18227 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/_collections_abc.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/_collections_abc.meta.json
--rw-r--r--   0        0        0     2923 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/_ctypes.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/_ctypes.meta.json
--rw-r--r--   0        0        0   170960 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/_decimal.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/_decimal.meta.json
--rw-r--r--   0        0        0    23362 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/abc.data.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/abc.meta.json
--rw-r--r--   0        0        0    60687 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/array.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/array.meta.json
--rw-r--r--   0        0        0  1054992 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/builtins.data.json
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/builtins.meta.json
--rw-r--r--   0        0        0   123328 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/codecs.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/codecs.meta.json
--rw-r--r--   0        0        0   104160 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/contextlib.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/contextlib.meta.json
--rw-r--r--   0        0        0    57612 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/dataclasses.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/dataclasses.meta.json
--rw-r--r--   0        0        0   142044 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/datetime.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/datetime.meta.json
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/decimal.data.json
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/decimal.meta.json
--rw-r--r--   0        0        0    61020 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/enum.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/enum.meta.json
--rw-r--r--   0        0        0    22399 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/genericpath.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/genericpath.meta.json
--rw-r--r--   0        0        0    85348 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/io.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/io.meta.json
--rw-r--r--   0        0        0    28778 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/mmap.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/mmap.meta.json
--rw-r--r--   0        0        0    78982 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/numbers.data.json
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/numbers.meta.json
--rw-r--r--   0        0        0    88278 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/pathlib.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/pathlib.meta.json
--rw-r--r--   0        0        0    45131 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/pickle.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/pickle.meta.json
--rw-r--r--   0        0        0    75208 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/posixpath.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/posixpath.meta.json
--rw-r--r--   0        0        0   167175 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/re.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/re.meta.json
--rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/sre_compile.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/sre_compile.meta.json
--rw-r--r--   0        0        0    28013 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/sre_constants.data.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/sre_constants.meta.json
--rw-r--r--   0        0        0    49442 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/sre_parse.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/sre_parse.meta.json
--rw-r--r--   0        0        0   168498 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/subprocess.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/subprocess.meta.json
--rw-r--r--   0        0        0   146267 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/sys.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/sys.meta.json
--rw-r--r--   0        0        0    43605 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/time.data.json
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/time.meta.json
--rw-r--r--   0        0        0   228230 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/types.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/types.meta.json
--rw-r--r--   0        0        0   416965 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/typing.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/typing.meta.json
--rw-r--r--   0        0        0    73907 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/typing_extensions.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/typing_extensions.meta.json
--rw-r--r--   0        0        0    89065 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   407999 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/collections/__init__.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/collections/__init__.meta.json
--rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/collections/abc.data.json
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/collections/abc.meta.json
--rw-r--r--   0        0        0   128994 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/email/__init__.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/email/__init__.meta.json
--rw-r--r--   0        0        0    12200 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/email/charset.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/email/charset.meta.json
--rw-r--r--   0        0        0     7249 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/email/contentmanager.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25073 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/email/errors.data.json
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/email/errors.meta.json
--rw-r--r--   0        0        0     9154 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/email/header.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/email/header.meta.json
--rw-r--r--   0        0        0    79298 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/email/message.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/email/message.meta.json
--rw-r--r--   0        0        0    30857 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/email/policy.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/email/policy.meta.json
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/importlib/__init__.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70175 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/importlib/abc.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/importlib/abc.meta.json
--rw-r--r--   0        0        0    64626 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/importlib/machinery.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/importlib/machinery.meta.json
--rw-r--r--   0        0        0    90277 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11935 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0   350178 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/os/__init__.data.json
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/os/__init__.meta.json
--rw-r--r--   0        0        0     4908 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/os/path.data.json
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/os/path.meta.json
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/src/__init__.data.json
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/src/__init__.meta.json
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/src/typedal/__about__.data.json
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/src/typedal/__about__.meta.json
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/src/typedal/__init__.data.json
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/src/typedal/__init__.meta.json
--rw-r--r--   0        0        0    33347 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/src/typedal/core.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/src/typedal/core.meta.json
--rw-r--r--   0        0        0    29038 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/src/typedal/fields.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/src/typedal/fields.meta.json
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/src/typedal/pydal_objects.data.json
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.10/src/typedal/pydal_objects.meta.json
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0     8152 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/__future__.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/__future__.meta.json
--rw-r--r--   0        0        0   180405 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    72680 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_bisect.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_bisect.meta.json
--rw-r--r--   0        0        0    57020 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    24646 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0    11060 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_compression.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_compression.meta.json
--rw-r--r--   0        0        0    21088 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_csv.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_csv.meta.json
--rw-r--r--   0        0        0   127335 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0   185969 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_decimal.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_decimal.meta.json
--rw-r--r--   0        0        0    23461 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_json.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_json.meta.json
--rw-r--r--   0        0        0    20139 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_locale.data.json
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_locale.meta.json
--rw-r--r--   0        0        0   163664 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_operator.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_operator.meta.json
--rw-r--r--   0        0        0     6555 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_random.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_random.meta.json
--rw-r--r--   0        0        0   141220 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_socket.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_socket.meta.json
--rw-r--r--   0        0        0    20067 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_stat.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_stat.meta.json
--rw-r--r--   0        0        0    25355 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_thread.data.json
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_thread.meta.json
--rw-r--r--   0        0        0     8127 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_tracemalloc.data.json
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_tracemalloc.meta.json
--rw-r--r--   0        0        0    17812 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_warnings.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_warnings.meta.json
--rw-r--r--   0        0        0    43019 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_weakref.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_weakref.meta.json
--rw-r--r--   0        0        0    64281 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_weakrefset.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_weakrefset.meta.json
--rw-r--r--   0        0        0    28042 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0   211034 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/argparse.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/argparse.meta.json
--rw-r--r--   0        0        0    81489 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0   154628 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/ast.data.json
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/ast.meta.json
--rw-r--r--   0        0        0     9651 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/atexit.data.json
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/atexit.meta.json
--rw-r--r--   0        0        0    15948 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/base64.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/base64.meta.json
--rw-r--r--   0        0        0    53666 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/bdb.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/bdb.meta.json
--rw-r--r--   0        0        0    11979 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/binascii.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/binascii.meta.json
--rw-r--r--   0        0        0    13025 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/bisect.data.json
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/bisect.meta.json
--rw-r--r--   0        0        0  1691043 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0    50828 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/bz2.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/bz2.meta.json
--rw-r--r--   0        0        0    61196 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/calendar.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/calendar.meta.json
--rw-r--r--   0        0        0    21019 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cmd.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cmd.meta.json
--rw-r--r--   0        0        0   129633 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0     7712 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/colorsys.data.json
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/colorsys.meta.json
--rw-r--r--   0        0        0   159139 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configparser.data.json
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configparser.meta.json
--rw-r--r--   0        0        0   128222 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0    63702 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/contextvars.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/contextvars.meta.json
--rw-r--r--   0        0        0     6338 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/copy.data.json
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/copy.meta.json
--rw-r--r--   0        0        0    13348 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/copyreg.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/copyreg.meta.json
--rw-r--r--   0        0        0    38114 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/csv.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/csv.meta.json
--rw-r--r--   0        0        0    82220 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/dataclasses.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/dataclasses.meta.json
--rw-r--r--   0        0        0   173432 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/datetime.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/datetime.meta.json
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/decimal.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/decimal.meta.json
--rw-r--r--   0        0        0    74115 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/difflib.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/difflib.meta.json
--rw-r--r--   0        0        0    67645 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/dis.data.json
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/dis.meta.json
--rw-r--r--   0        0        0    77702 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/doctest.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/doctest.meta.json
--rw-r--r--   0        0        0   114800 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0    23733 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/errno.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/errno.meta.json
--rw-r--r--   0        0        0    27481 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/example_new.data.json
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/example_new.meta.json
--rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/fnmatch.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/fnmatch.meta.json
--rw-r--r--   0        0        0   117065 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/fractions.data.json
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/fractions.meta.json
--rw-r--r--   0        0        0   187190 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/functools.data.json
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/functools.meta.json
--rw-r--r--   0        0        0    16492 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/gc.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/gc.meta.json
--rw-r--r--   0        0        0    30432 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/getpass.data.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/getpass.meta.json
--rw-r--r--   0        0        0    58893 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/gettext.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/gettext.meta.json
--rw-r--r--   0        0        0    11236 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/glob.data.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/glob.meta.json
--rw-r--r--   0        0        0    55273 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/gzip.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/gzip.meta.json
--rw-r--r--   0        0        0    32987 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/hashlib.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/hashlib.meta.json
--rw-r--r--   0        0        0    20199 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/hmac.data.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/hmac.meta.json
--rw-r--r--   0        0        0   393898 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/inspect.data.json
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/inspect.meta.json
--rw-r--r--   0        0        0    96360 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0   169807 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/ipaddress.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/ipaddress.meta.json
--rw-r--r--   0        0        0   521458 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/itertools.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/itertools.meta.json
--rw-r--r--   0        0        0     8942 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/linecache.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/linecache.meta.json
--rw-r--r--   0        0        0    21639 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/locale.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/locale.meta.json
--rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/marshal.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/marshal.meta.json
--rw-r--r--   0        0        0    62500 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/math.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/math.meta.json
--rw-r--r--   0        0        0    16551 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/mimetypes.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/mimetypes.meta.json
--rw-r--r--   0        0        0    32933 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/msvcrt.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/msvcrt.meta.json
--rw-r--r--   0        0        0   151900 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/mypy_extensions.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/mypy_extensions.meta.json
--rw-r--r--   0        0        0    84033 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/numbers.data.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/numbers.meta.json
--rw-r--r--   0        0        0     6122 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/opcode.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/opcode.meta.json
--rw-r--r--   0        0        0    55486 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/operator.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/operator.meta.json
--rw-r--r--   0        0        0   102946 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    96201 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pdb.data.json
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pdb.meta.json
--rw-r--r--   0        0        0    48959 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    31491 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pkgutil.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pkgutil.meta.json
--rw-r--r--   0        0        0    37189 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/platform.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/platform.meta.json
--rw-r--r--   0        0        0   124421 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0    12597 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pprint.data.json
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pprint.meta.json
--rw-r--r--   0        0        0     7678 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pty.data.json
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pty.meta.json
--rw-r--r--   0        0        0   111565 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pydoc.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pydoc.meta.json
--rw-r--r--   0        0        0    37466 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/queue.data.json
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/queue.meta.json
--rw-r--r--   0        0        0    43645 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/random.data.json
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/random.meta.json
--rw-r--r--   0        0        0   243154 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    17416 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/reprlib.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/reprlib.meta.json
--rw-r--r--   0        0        0     6994 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/secrets.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/secrets.meta.json
--rw-r--r--   0        0        0    22630 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/select.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/select.meta.json
--rw-r--r--   0        0        0    66210 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/selectors.data.json
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/selectors.meta.json
--rw-r--r--   0        0        0    17284 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/shlex.data.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/shlex.meta.json
--rw-r--r--   0        0        0    90180 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/shutil.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/shutil.meta.json
--rw-r--r--   0        0        0    51409 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/signal.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/signal.meta.json
--rw-r--r--   0        0        0   126342 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/socket.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/socket.meta.json
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/src.data.json
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/src.meta.json
--rw-r--r--   0        0        0    14457 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    28914 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    51841 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0   212877 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/ssl.data.json
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/ssl.meta.json
--rw-r--r--   0        0        0     6530 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/stat.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/stat.meta.json
--rw-r--r--   0        0        0    32136 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/string.data.json
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/string.meta.json
--rw-r--r--   0        0        0    15829 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/struct.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/struct.meta.json
--rw-r--r--   0        0        0   238269 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   155328 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0    16019 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/sysconfig.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/sysconfig.meta.json
--rw-r--r--   0        0        0   145159 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tarfile.data.json
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tarfile.meta.json
--rw-r--r--   0        0        0   216804 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tempfile.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tempfile.meta.json
--rw-r--r--   0        0        0    50218 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/termios.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/termios.meta.json
--rw-r--r--   0        0        0    20222 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/textwrap.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/textwrap.meta.json
--rw-r--r--   0        0        0    70414 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/threading.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/threading.meta.json
--rw-r--r--   0        0        0    45633 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/time.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/time.meta.json
--rw-r--r--   0        0        0    14997 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/token.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/token.meta.json
--rw-r--r--   0        0        0    52648 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tokenize.data.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tokenize.meta.json
--rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomllib.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomllib.meta.json
--rw-r--r--   0        0        0    68653 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/traceback.data.json
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/traceback.meta.json
--rw-r--r--   0        0        0    48898 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tracemalloc.data.json
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tracemalloc.meta.json
--rw-r--r--   0        0        0     5355 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tty.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tty.meta.json
--rw-r--r--   0        0        0   306063 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   593708 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0   118925 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0    60291 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/unicodedata.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/unicodedata.meta.json
--rw-r--r--   0        0        0    35665 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/uuid.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/uuid.meta.json
--rw-r--r--   0        0        0    28607 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/warnings.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/warnings.meta.json
--rw-r--r--   0        0        0   253459 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/weakref.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/weakref.meta.json
--rw-r--r--   0        0        0    96907 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/zipfile.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/zipfile.meta.json
--rw-r--r--   0        0        0    17771 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/zlib.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/zlib.meta.json
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/__init__.data.json
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/__init__.meta.json
--rw-r--r--   0        0        0     6371 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_argcomplete.data.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_argcomplete.meta.json
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_version.data.json
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_version.meta.json
--rw-r--r--   0        0        0    48646 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/cacheprovider.data.json
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/cacheprovider.meta.json
--rw-r--r--   0        0        0   184495 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/capture.data.json
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/capture.meta.json
--rw-r--r--   0        0        0    28325 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/compat.data.json
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/compat.meta.json
--rw-r--r--   0        0        0    33667 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/debugging.data.json
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/debugging.meta.json
--rw-r--r--   0        0        0     7912 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/deprecated.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/deprecated.meta.json
--rw-r--r--   0        0        0    43717 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/doctest.data.json
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/doctest.meta.json
--rw-r--r--   0        0        0   181399 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/fixtures.data.json
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/fixtures.meta.json
--rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/freeze_support.data.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/freeze_support.meta.json
--rw-r--r--   0        0        0    10089 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/helpconfig.data.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/helpconfig.meta.json
--rw-r--r--   0        0        0    67739 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/hookspec.data.json
--rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/hookspec.meta.json
--rw-r--r--   0        0        0    67338 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/legacypath.data.json
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/legacypath.meta.json
--rw-r--r--   0        0        0    87227 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/logging.data.json
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/logging.meta.json
--rw-r--r--   0        0        0    52638 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/main.data.json
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/main.meta.json
--rw-r--r--   0        0        0    29094 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/monkeypatch.data.json
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/monkeypatch.meta.json
--rw-r--r--   0        0        0    62209 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/nodes.data.json
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/nodes.meta.json
--rw-r--r--   0        0        0    34335 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/outcomes.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/outcomes.meta.json
--rw-r--r--   0        0        0    38506 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/pathlib.data.json
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/pathlib.meta.json
--rw-r--r--   0        0        0   143660 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/pytester.data.json
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/pytester.meta.json
--rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/pytester_assertions.data.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/pytester_assertions.meta.json
--rw-r--r--   0        0        0   125125 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/python.data.json
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/python.meta.json
--rw-r--r--   0        0        0    61369 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/python_api.data.json
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/python_api.meta.json
--rw-r--r--   0        0        0    37939 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/recwarn.data.json
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/recwarn.meta.json
--rw-r--r--   0        0        0    53903 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/reports.data.json
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/reports.meta.json
--rw-r--r--   0        0        0    45874 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/runner.data.json
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/runner.meta.json
--rw-r--r--   0        0        0    11808 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/scope.data.json
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/scope.meta.json
--rw-r--r--   0        0        0    17100 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/stash.data.json
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/stash.meta.json
--rw-r--r--   0        0        0   129351 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/terminal.data.json
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/terminal.meta.json
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/timing.data.json
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/timing.meta.json
--rw-r--r--   0        0        0    26426 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/tmpdir.data.json
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/tmpdir.meta.json
--rw-r--r--   0        0        0    34310 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/warning_types.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/warning_types.meta.json
--rw-r--r--   0        0        0    14515 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/warnings.data.json
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/warnings.meta.json
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_code/__init__.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_code/__init__.meta.json
--rw-r--r--   0        0        0   208544 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_code/code.data.json
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_code/code.meta.json
--rw-r--r--   0        0        0    20396 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_code/source.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_code/source.meta.json
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_io/__init__.data.json
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_io/__init__.meta.json
--rw-r--r--   0        0        0    13200 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_io/saferepr.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_io/saferepr.meta.json
--rw-r--r--   0        0        0    16853 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_io/terminalwriter.data.json
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_io/terminalwriter.meta.json
--rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_io/wcwidth.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_io/wcwidth.meta.json
--rw-r--r--   0        0        0    13753 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/assertion/__init__.data.json
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/assertion/__init__.meta.json
--rw-r--r--   0        0        0    64441 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/assertion/rewrite.data.json
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/assertion/rewrite.meta.json
--rw-r--r--   0        0        0     6078 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/assertion/truncate.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/assertion/truncate.meta.json
--rw-r--r--   0        0        0    23734 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/assertion/util.data.json
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/assertion/util.meta.json
--rw-r--r--   0        0        0   107743 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/config/__init__.data.json
--rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/config/__init__.meta.json
--rw-r--r--   0        0        0    42346 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/config/argparsing.data.json
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/config/argparsing.meta.json
--rw-r--r--   0        0        0     5077 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/config/compat.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/config/compat.meta.json
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/config/exceptions.data.json
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/config/exceptions.meta.json
--rw-r--r--   0        0        0    10343 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/config/findpaths.data.json
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/config/findpaths.meta.json
--rw-r--r--   0        0        0    27773 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/mark/__init__.data.json
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/mark/__init__.meta.json
--rw-r--r--   0        0        0    34035 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/mark/expression.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/mark/expression.meta.json
--rw-r--r--   0        0        0   133374 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/mark/structures.data.json
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_pytest/mark/structures.meta.json
--rw-r--r--   0        0        0   112991 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_typeshed/xml.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/_typeshed/xml.meta.json
--rw-r--r--   0        0        0    23372 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/async_timeout/__init__.data.json
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/async_timeout/__init__.meta.json
--rw-r--r--   0        0        0    15027 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/__init__.data.json
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/__init__.meta.json
--rw-r--r--   0        0        0   116469 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/base_events.data.json
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/base_events.meta.json
--rw-r--r--   0        0        0    36018 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/coroutines.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/coroutines.meta.json
--rw-r--r--   0        0        0   222121 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/events.data.json
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/events.meta.json
--rw-r--r--   0        0        0    11879 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/exceptions.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/exceptions.meta.json
--rw-r--r--   0        0        0    43204 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/futures.data.json
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/futures.meta.json
--rw-r--r--   0        0        0    41996 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/locks.data.json
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/locks.meta.json
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/mixins.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/mixins.meta.json
--rw-r--r--   0        0        0    18996 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/protocols.data.json
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/protocols.meta.json
--rw-r--r--   0        0        0    28441 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/queues.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/queues.meta.json
--rw-r--r--   0        0        0    11969 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/runners.data.json
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/runners.meta.json
--rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/selector_events.data.json
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/selector_events.meta.json
--rw-r--r--   0        0        0    39572 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/streams.data.json
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/streams.meta.json
--rw-r--r--   0        0        0    25143 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/subprocess.data.json
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/subprocess.meta.json
--rw-r--r--   0        0        0    10201 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/taskgroups.data.json
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/taskgroups.meta.json
--rw-r--r--   0        0        0   210760 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/tasks.data.json
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/tasks.meta.json
--rw-r--r--   0        0        0     6673 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/threads.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/threads.meta.json
--rw-r--r--   0        0        0    10036 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/timeouts.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/timeouts.meta.json
--rw-r--r--   0        0        0    30202 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/transports.data.json
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/transports.meta.json
--rw-r--r--   0        0        0    62212 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/unix_events.data.json
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/asyncio/unix_events.meta.json
--rw-r--r--   0        0        0    51606 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/__init__.data.json
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/__init__.meta.json
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/_width_table.data.json
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/_width_table.meta.json
--rw-r--r--   0        0        0    34730 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/brackets.data.json
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/brackets.meta.json
--rw-r--r--   0        0        0    34153 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/cache.data.json
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/cache.meta.json
--rw-r--r--   0        0        0    24821 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/comments.data.json
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/comments.meta.json
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/const.data.json
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/const.meta.json
--rw-r--r--   0        0        0    20396 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/files.data.json
--rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/files.meta.json
--rw-r--r--   0        0        0    37122 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/handle_ipynb_magics.data.json
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/handle_ipynb_magics.meta.json
--rw-r--r--   0        0        0    69328 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/linegen.data.json
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/linegen.meta.json
--rw-r--r--   0        0        0    85067 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/lines.data.json
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/lines.meta.json
--rw-r--r--   0        0        0    35409 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/mode.data.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/mode.meta.json
--rw-r--r--   0        0        0    56411 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/nodes.data.json
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/nodes.meta.json
--rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/numerics.data.json
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/numerics.meta.json
--rw-r--r--   0        0        0    11971 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/output.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/output.meta.json
--rw-r--r--   0        0        0    12323 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/parsing.data.json
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/parsing.meta.json
--rw-r--r--   0        0        0    26344 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/ranges.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/ranges.meta.json
--rw-r--r--   0        0        0    17026 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/report.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/report.meta.json
--rw-r--r--   0        0        0    11815 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/rusty.data.json
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/rusty.meta.json
--rw-r--r--   0        0        0    13426 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/strings.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/strings.meta.json
--rw-r--r--   0        0        0    85345 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/trans.data.json
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/black/trans.meta.json
--rw-r--r--   0        0        0     7752 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/click/__init__.data.json
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/click/__init__.meta.json
--rw-r--r--   0        0        0    49747 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/click/_compat.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/click/_compat.meta.json
--rw-r--r--   0        0        0    52435 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/click/_termui_impl.data.json
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/click/_termui_impl.meta.json
--rw-r--r--   0        0        0   213135 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/click/core.data.json
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/click/core.meta.json
--rw-r--r--   0        0        0    73391 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/click/decorators.data.json
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/click/decorators.meta.json
--rw-r--r--   0        0        0    31405 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/click/exceptions.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/click/exceptions.meta.json
--rw-r--r--   0        0        0    18490 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/click/formatting.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/click/formatting.meta.json
--rw-r--r--   0        0        0     8330 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/click/globals.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/click/globals.meta.json
--rw-r--r--   0        0        0    31096 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/click/parser.data.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/click/parser.meta.json
--rw-r--r--   0        0        0    38460 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/click/shell_completion.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/click/shell_completion.meta.json
--rw-r--r--   0        0        0    25411 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/click/termui.data.json
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/click/termui.meta.json
--rw-r--r--   0        0        0    89634 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/click/types.data.json
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/click/types.meta.json
--rw-r--r--   0        0        0    37412 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/click/utils.data.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/click/utils.meta.json
--rw-r--r--   0        0        0   788818 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/concurrent/__init__.data.json
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/concurrent/__init__.meta.json
--rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/concurrent/futures/__init__.data.json
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/concurrent/futures/__init__.meta.json
--rw-r--r--   0        0        0    86898 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/concurrent/futures/_base.data.json
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/concurrent/futures/_base.meta.json
--rw-r--r--   0        0        0    66256 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/concurrent/futures/process.data.json
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/concurrent/futures/process.meta.json
--rw-r--r--   0        0        0    24284 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/concurrent/futures/thread.data.json
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/concurrent/futures/thread.meta.json
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configurablejson/__init__.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configurablejson/__init__.meta.json
--rw-r--r--   0        0        0    19403 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configurablejson/_internals.data.json
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configurablejson/_internals.meta.json
--rw-r--r--   0        0        0    17411 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configurablejson/encode.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configurablejson/encode.meta.json
--rw-r--r--   0        0        0     4837 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/__init__.data.json
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/__init__.meta.json
--rw-r--r--   0        0        0    13895 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/abs.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/abs.meta.json
--rw-r--r--   0        0        0    10489 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/alias.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/alias.meta.json
--rw-r--r--   0        0        0    15569 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/beautify.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/beautify.meta.json
--rw-r--r--   0        0        0    34248 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/binary_config.data.json
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/binary_config.meta.json
--rw-r--r--   0        0        0    48466 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/cls.data.json
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/cls.meta.json
--rw-r--r--   0        0        0    37519 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/core.data.json
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/core.meta.json
--rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/dump.data.json
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/dump.meta.json
--rw-r--r--   0        0        0    47435 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/errors.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/errors.meta.json
--rw-r--r--   0        0        0    16366 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/helpers.data.json
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/helpers.meta.json
--rw-r--r--   0        0        0     5735 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/postpone.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/postpone.meta.json
--rw-r--r--   0        0        0     6506 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/singleton.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/singleton.meta.json
--rw-r--r--   0        0        0     7818 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/type_converters.data.json
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/type_converters.meta.json
--rw-r--r--   0        0        0    10079 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/loaders/__init__.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/loaders/__init__.meta.json
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/loaders/_types.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/loaders/_types.meta.json
--rw-r--r--   0        0        0    11833 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/loaders/loaders_shared.data.json
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/loaders/loaders_shared.meta.json
--rw-r--r--   0        0        0    31947 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/loaders/register.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/loaders/register.meta.json
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/__about__.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/__about__.meta.json
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/__init__.data.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/__init__.meta.json
--rw-r--r--   0        0        0    13119 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/exceptions.data.json
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/exceptions.meta.json
--rw-r--r--   0        0        0    20535 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/utils.data.json
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/utils.meta.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/__init__.data.json
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/__init__.meta.json
--rw-r--r--   0        0        0    48126 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/_oid.data.json
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/_oid.meta.json
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/__init__.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/__init__.meta.json
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/__init__.data.json
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/__init__.meta.json
--rw-r--r--   0        0        0    14600 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/aead.data.json
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/aead.meta.json
--rw-r--r--   0        0        0    91123 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/backend.data.json
--rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/backend.meta.json
--rw-r--r--   0        0        0    13430 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/ciphers.data.json
--rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/ciphers.meta.json
--rw-r--r--   0        0        0     9234 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/cmac.data.json
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/cmac.meta.json
--rw-r--r--   0        0        0    30942 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/ec.data.json
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/ec.meta.json
--rw-r--r--   0        0        0    35743 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/rsa.data.json
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/rsa.meta.json
--rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/utils.data.json
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/utils.meta.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/__init__.data.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/__init__.meta.json
--rw-r--r--   0        0        0     8138 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/__init__.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/__init__.meta.json
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/_openssl.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/_openssl.meta.json
--rw-r--r--   0        0        0     6808 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/asn1.data.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/asn1.meta.json
--rw-r--r--   0        0        0     6527 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/exceptions.data.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/exceptions.meta.json
--rw-r--r--   0        0        0     5960 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/ocsp.data.json
--rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/ocsp.meta.json
--rw-r--r--   0        0        0    34855 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/x509.data.json
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/x509.meta.json
--rw-r--r--   0        0        0    12942 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/__init__.data.json
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/__init__.meta.json
--rw-r--r--   0        0        0    21687 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/aead.data.json
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/aead.meta.json
--rw-r--r--   0        0        0     6737 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/cmac.data.json
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/cmac.meta.json
--rw-r--r--   0        0        0    27431 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/dh.data.json
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/dh.meta.json
--rw-r--r--   0        0        0    25255 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/dsa.data.json
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/dsa.meta.json
--rw-r--r--   0        0        0    23775 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/ec.data.json
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/ec.meta.json
--rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/ed25519.data.json
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/ed25519.meta.json
--rw-r--r--   0        0        0     6177 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/ed448.data.json
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/ed448.meta.json
--rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/hashes.data.json
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/hashes.meta.json
--rw-r--r--   0        0        0     8319 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/hmac.data.json
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/hmac.meta.json
--rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/kdf.data.json
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/kdf.meta.json
--rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/keys.data.json
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/keys.meta.json
--rw-r--r--   0        0        0     8574 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/poly1305.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/poly1305.meta.json
--rw-r--r--   0        0        0    23980 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/rsa.data.json
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/rsa.meta.json
--rw-r--r--   0        0        0     6221 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/x25519.data.json
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/x25519.meta.json
--rw-r--r--   0        0        0     6133 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/x448.data.json
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/x448.meta.json
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/openssl/__init__.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/openssl/__init__.meta.json
--rw-r--r--   0        0        0    21364 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/openssl/_conditional.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/openssl/_conditional.meta.json
--rw-r--r--   0        0        0    15055 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/openssl/binding.data.json
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/openssl/binding.meta.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/__init__.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/__init__.meta.json
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/_asymmetric.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/_asymmetric.meta.json
--rw-r--r--   0        0        0    10701 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/_cipheralgorithm.data.json
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/_cipheralgorithm.meta.json
--rw-r--r--   0        0        0    34260 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/_serialization.data.json
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/_serialization.meta.json
--rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/constant_time.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/constant_time.meta.json
--rw-r--r--   0        0        0    58762 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/hashes.data.json
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/hashes.meta.json
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/__init__.data.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/__init__.meta.json
--rw-r--r--   0        0        0    30857 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/dh.data.json
--rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/dh.meta.json
--rw-r--r--   0        0        0    32764 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/dsa.data.json
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/dsa.meta.json
--rw-r--r--   0        0        0    87270 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/ec.data.json
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/ec.meta.json
--rw-r--r--   0        0        0    23234 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/ed25519.data.json
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/ed25519.meta.json
--rw-r--r--   0        0        0    22916 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/ed448.data.json
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/ed448.meta.json
--rw-r--r--   0        0        0    23642 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/padding.data.json
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/padding.meta.json
--rw-r--r--   0        0        0    34585 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/rsa.data.json
--rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/rsa.meta.json
--rw-r--r--   0        0        0     8764 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/types.data.json
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/types.meta.json
--rw-r--r--   0        0        0     7346 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/utils.data.json
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/utils.meta.json
--rw-r--r--   0        0        0    21642 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/x25519.data.json
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/x25519.meta.json
--rw-r--r--   0        0        0    21336 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/x448.data.json
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/x448.meta.json
--rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/__init__.data.json
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/__init__.meta.json
--rw-r--r--   0        0        0    18107 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/aead.data.json
--rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/aead.meta.json
--rw-r--r--   0        0        0    55273 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/algorithms.data.json
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/algorithms.meta.json
--rw-r--r--   0        0        0    51375 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/base.data.json
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/base.meta.json
--rw-r--r--   0        0        0    60153 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/modes.data.json
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/modes.meta.json
--rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/serialization/__init__.data.json
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/serialization/__init__.meta.json
--rw-r--r--   0        0        0     7038 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/serialization/base.data.json
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/serialization/base.meta.json
--rw-r--r--   0        0        0    28300 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/serialization/pkcs12.data.json
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/serialization/pkcs12.meta.json
--rw-r--r--   0        0        0   121932 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/serialization/ssh.data.json
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/serialization/ssh.meta.json
--rw-r--r--   0        0        0    31282 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/__init__.data.json
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/__init__.meta.json
--rw-r--r--   0        0        0   177864 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/base.data.json
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/base.meta.json
--rw-r--r--   0        0        0    22913 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/certificate_transparency.data.json
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/certificate_transparency.meta.json
--rw-r--r--   0        0        0   400114 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/extensions.data.json
--rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/extensions.meta.json
--rw-r--r--   0        0        0    52975 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/general_name.data.json
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/general_name.meta.json
--rw-r--r--   0        0        0    56606 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/name.data.json
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/name.meta.json
--rw-r--r--   0        0        0    97342 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/ocsp.data.json
--rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/ocsp.meta.json
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/oid.data.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/oid.meta.json
--rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/verification.data.json
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/verification.meta.json
--rw-r--r--   0        0        0    66125 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0    63522 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/ctypes/wintypes.data.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/ctypes/wintypes.meta.json
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/distutils/__init__.data.json
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/distutils/__init__.meta.json
--rw-r--r--   0        0        0    16325 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/distutils/util.data.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/distutils/util.meta.json
--rw-r--r--   0        0        0     4515 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/dotenv/__init__.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/dotenv/__init__.meta.json
--rw-r--r--   0        0        0    24352 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/dotenv/main.data.json
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/dotenv/main.meta.json
--rw-r--r--   0        0        0    56881 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/dotenv/parser.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/dotenv/parser.meta.json
--rw-r--r--   0        0        0    15883 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/dotenv/variables.data.json
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/dotenv/variables.meta.json
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/edwh_migrate/__init__.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/edwh_migrate/__init__.meta.json
--rw-r--r--   0        0        0    53859 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/edwh_migrate/migrate.data.json
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/edwh_migrate/migrate.meta.json
--rw-r--r--   0        0        0     7662 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    16390 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7417 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25129 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9350 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0   101117 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    33204 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0    26015 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/email/utils.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/email/utils.meta.json
--rw-r--r--   0        0        0     9410 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/__init__.data.json
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/__init__.meta.json
--rw-r--r--   0        0        0   101033 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/cmd.data.json
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/cmd.meta.json
--rw-r--r--   0        0        0    22061 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/compat.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/compat.meta.json
--rw-r--r--   0        0        0    72061 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/config.data.json
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/config.meta.json
--rw-r--r--   0        0        0     8346 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/db.data.json
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/db.meta.json
--rw-r--r--   0        0        0    43517 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/diff.data.json
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/diff.meta.json
--rw-r--r--   0        0        0    31208 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/exc.data.json
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/exc.meta.json
--rw-r--r--   0        0        0    86993 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/remote.data.json
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/remote.meta.json
--rw-r--r--   0        0        0    14236 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/types.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/types.meta.json
--rw-r--r--   0        0        0   120972 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/util.data.json
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/util.meta.json
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/index/__init__.data.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/index/__init__.meta.json
--rw-r--r--   0        0        0    67883 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/index/base.data.json
--rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/index/base.meta.json
--rw-r--r--   0        0        0    19230 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/index/fun.data.json
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/index/fun.meta.json
--rw-r--r--   0        0        0    54512 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/index/typ.data.json
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/index/typ.meta.json
--rw-r--r--   0        0        0    16630 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/index/util.data.json
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/index/util.meta.json
--rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/objects/__init__.data.json
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/objects/__init__.meta.json
--rw-r--r--   0        0        0    28657 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/objects/base.data.json
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/objects/base.meta.json
--rw-r--r--   0        0        0     6290 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/objects/blob.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/objects/blob.meta.json
--rw-r--r--   0        0        0    44705 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/objects/commit.data.json
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/objects/commit.meta.json
--rw-r--r--   0        0        0    13968 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/objects/fun.data.json
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/objects/fun.meta.json
--rw-r--r--   0        0        0     9015 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/objects/tag.data.json
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/objects/tag.meta.json
--rw-r--r--   0        0        0    38948 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/objects/tree.data.json
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/objects/tree.meta.json
--rw-r--r--   0        0        0   112403 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/objects/util.data.json
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/objects/util.meta.json
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/objects/submodule/__init__.data.json
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/objects/submodule/__init__.meta.json
--rw-r--r--   0        0        0    66249 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/objects/submodule/base.data.json
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/objects/submodule/base.meta.json
--rw-r--r--   0        0        0    13416 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/objects/submodule/root.data.json
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/objects/submodule/root.meta.json
--rw-r--r--   0        0        0    12184 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/objects/submodule/util.data.json
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/objects/submodule/util.meta.json
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/refs/__init__.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/refs/__init__.meta.json
--rw-r--r--   0        0        0    18213 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/refs/head.data.json
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/refs/head.meta.json
--rw-r--r--   0        0        0    40948 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/refs/log.data.json
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/refs/log.meta.json
--rw-r--r--   0        0        0    18936 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/refs/reference.data.json
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/refs/reference.meta.json
--rw-r--r--   0        0        0    10509 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/refs/remote.data.json
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/refs/remote.meta.json
--rw-r--r--   0        0        0    64655 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/refs/symbolic.data.json
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/refs/symbolic.meta.json
--rw-r--r--   0        0        0    13266 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/refs/tag.data.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/refs/tag.meta.json
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/repo/__init__.data.json
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/repo/__init__.meta.json
--rw-r--r--   0        0        0   108932 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/repo/base.data.json
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/repo/base.meta.json
--rw-r--r--   0        0        0    12722 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/repo/fun.data.json
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/git/repo/fun.meta.json
--rw-r--r--   0        0        0     4779 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/html/__init__.data.json
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/html/__init__.meta.json
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/html/entities.data.json
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/html/entities.meta.json
--rw-r--r--   0        0        0    24033 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/http/__init__.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/http/__init__.meta.json
--rw-r--r--   0        0        0    74759 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/http/client.data.json
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/http/client.meta.json
--rw-r--r--   0        0        0    63694 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/http/cookiejar.data.json
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/http/cookiejar.meta.json
--rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    61909 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    76878 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    22649 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/importlib/readers.data.json
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/importlib/readers.meta.json
--rw-r--r--   0        0        0    24411 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/importlib/util.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/importlib/util.meta.json
--rw-r--r--   0        0        0   102879 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    18350 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    10734 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/importlib/resources/__init__.data.json
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/importlib/resources/__init__.meta.json
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/importlib/resources/abc.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/importlib/resources/abc.meta.json
--rw-r--r--   0        0        0    67163 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/iniconfig/__init__.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/iniconfig/__init__.meta.json
--rw-r--r--   0        0        0    24550 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/iniconfig/_parse.data.json
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/iniconfig/_parse.meta.json
--rw-r--r--   0        0        0     4983 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/iniconfig/exceptions.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/iniconfig/exceptions.meta.json
--rw-r--r--   0        0        0    15855 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/json/__init__.data.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/json/__init__.meta.json
--rw-r--r--   0        0        0    15446 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/json/decoder.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/json/decoder.meta.json
--rw-r--r--   0        0        0    11337 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/json/encoder.data.json
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/json/encoder.meta.json
--rw-r--r--   0        0        0   161727 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/logging/__init__.data.json
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/logging/__init__.meta.json
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/__init__.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/__init__.meta.json
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/_compat.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/_compat.meta.json
--rw-r--r--   0        0        0     5699 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/_punycode.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/_punycode.meta.json
--rw-r--r--   0        0        0    35792 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/main.data.json
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/main.meta.json
--rw-r--r--   0        0        0     8178 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/parser_block.data.json
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/parser_block.meta.json
--rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/parser_core.data.json
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/parser_core.meta.json
--rw-r--r--   0        0        0     9963 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/parser_inline.data.json
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/parser_inline.meta.json
--rw-r--r--   0        0        0    21363 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/renderer.data.json
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/renderer.meta.json
--rw-r--r--   0        0        0    38344 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/ruler.data.json
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/ruler.meta.json
--rw-r--r--   0        0        0    29705 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/token.data.json
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/token.meta.json
--rw-r--r--   0        0        0    39948 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/utils.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/utils.meta.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/common/__init__.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/common/__init__.meta.json
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/common/entities.data.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/common/entities.meta.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json
--rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/common/html_re.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/common/html_re.meta.json
--rw-r--r--   0        0        0     6147 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json
--rw-r--r--   0        0        0    18415 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/common/utils.data.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/common/utils.meta.json
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json
--rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json
--rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json
--rw-r--r--   0        0        0     4996 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/presets/__init__.data.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/presets/default.data.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/presets/default.meta.json
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/presets/zero.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/presets/zero.meta.json
--rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/code.data.json
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json
--rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json
--rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json
--rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/list.data.json
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json
--rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json
--rw-r--r--   0        0        0    18155 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json
--rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/table.data.json
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json
--rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/block.data.json
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json
--rw-r--r--   0        0        0     6399 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json
--rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json
--rw-r--r--   0        0        0     8420 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json
--rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json
--rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json
--rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/text_join.data.json
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/text_join.meta.json
--rw-r--r--   0        0        0     4052 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json
--rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json
--rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json
--rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/fragments_join.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/fragments_join.meta.json
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json
--rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/linkify.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/linkify.meta.json
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json
--rw-r--r--   0        0        0    41273 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json
--rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/mdurl/__init__.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/mdurl/__init__.meta.json
--rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/mdurl/_decode.data.json
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/mdurl/_decode.meta.json
--rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/mdurl/_encode.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/mdurl/_encode.meta.json
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/mdurl/_format.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/mdurl/_format.meta.json
--rw-r--r--   0        0        0    13015 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/mdurl/_parse.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/mdurl/_parse.meta.json
--rw-r--r--   0        0        0    28308 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/mdurl/_url.data.json
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/mdurl/_url.meta.json
--rw-r--r--   0        0        0    34141 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/__init__.data.json
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/__init__.meta.json
--rw-r--r--   0        0        0    33167 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/connection.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/connection.meta.json
--rw-r--r--   0        0        0   122489 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/context.data.json
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/context.meta.json
--rw-r--r--   0        0        0   218030 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/managers.data.json
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/managers.meta.json
--rw-r--r--   0        0        0    62426 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/pool.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/pool.meta.json
--rw-r--r--   0        0        0     9487 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/popen_fork.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json
--rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json
--rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json
--rw-r--r--   0        0        0    18525 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/process.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/process.meta.json
--rw-r--r--   0        0        0    28704 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/queues.data.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/queues.meta.json
--rw-r--r--   0        0        0    30366 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/reduction.data.json
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/reduction.meta.json
--rw-r--r--   0        0        0    36116 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/shared_memory.data.json
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json
--rw-r--r--   0        0        0    98077 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json
--rw-r--r--   0        0        0    10102 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/spawn.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/spawn.meta.json
--rw-r--r--   0        0        0    28435 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/synchronize.data.json
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/synchronize.meta.json
--rw-r--r--   0        0        0    24570 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/util.data.json
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/util.meta.json
--rw-r--r--   0        0        0   397801 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     4908 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/packaging/__init__.data.json
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/packaging/__init__.meta.json
--rw-r--r--   0        0        0    15520 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/packaging/_elffile.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/packaging/_elffile.meta.json
--rw-r--r--   0        0        0    29325 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/packaging/_manylinux.data.json
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/packaging/_manylinux.meta.json
--rw-r--r--   0        0        0    20376 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/packaging/_musllinux.data.json
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/packaging/_musllinux.meta.json
--rw-r--r--   0        0        0    48580 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/packaging/_parser.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/packaging/_parser.meta.json
--rw-r--r--   0        0        0    14958 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/packaging/_structures.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/packaging/_structures.meta.json
--rw-r--r--   0        0        0    20540 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/packaging/_tokenizer.data.json
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/packaging/_tokenizer.meta.json
--rw-r--r--   0        0        0    19513 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/packaging/markers.data.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/packaging/markers.meta.json
--rw-r--r--   0        0        0    10512 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/packaging/requirements.data.json
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/packaging/requirements.meta.json
--rw-r--r--   0        0        0    60559 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/packaging/specifiers.data.json
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/packaging/specifiers.meta.json
--rw-r--r--   0        0        0    29671 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/packaging/tags.data.json
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/packaging/tags.meta.json
--rw-r--r--   0        0        0    13225 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/packaging/utils.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/packaging/utils.meta.json
--rw-r--r--   0        0        0    80955 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/packaging/version.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/packaging/version.meta.json
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pathspec/__init__.data.json
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pathspec/__init__.meta.json
--rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pathspec/_meta.data.json
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pathspec/_meta.meta.json
--rw-r--r--   0        0        0    29494 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pathspec/gitignore.data.json
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pathspec/gitignore.meta.json
--rw-r--r--   0        0        0    29872 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pathspec/pathspec.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pathspec/pathspec.meta.json
--rw-r--r--   0        0        0    19851 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pathspec/pattern.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pathspec/pattern.meta.json
--rw-r--r--   0        0        0    55592 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pathspec/util.data.json
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pathspec/util.meta.json
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pathspec/patterns/__init__.data.json
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pathspec/patterns/__init__.meta.json
--rw-r--r--   0        0        0    18510 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.meta.json
--rw-r--r--   0        0        0    32503 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/platformdirs/__init__.data.json
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/platformdirs/__init__.meta.json
--rw-r--r--   0        0        0    52590 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/platformdirs/api.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/platformdirs/api.meta.json
--rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/platformdirs/version.data.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/platformdirs/version.meta.json
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pluggy/__init__.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pluggy/__init__.meta.json
--rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pluggy/_callers.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pluggy/_callers.meta.json
--rw-r--r--   0        0        0   102996 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pluggy/_hooks.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pluggy/_hooks.meta.json
--rw-r--r--   0        0        0    39554 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pluggy/_manager.data.json
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pluggy/_manager.meta.json
--rw-r--r--   0        0        0    22344 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pluggy/_result.data.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pluggy/_result.meta.json
--rw-r--r--   0        0        0    13570 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pluggy/_tracing.data.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pluggy/_tracing.meta.json
--rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pluggy/_version.data.json
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pluggy/_version.meta.json
--rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/__init__.data.json
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/__init__.meta.json
--rw-r--r--   0        0        0    26890 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/auto_suggest.data.json
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/auto_suggest.meta.json
--rw-r--r--   0        0        0   115432 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/buffer.data.json
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/buffer.meta.json
--rw-r--r--   0        0        0    25920 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/cache.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/cache.meta.json
--rw-r--r--   0        0        0    20835 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/cursor_shapes.data.json
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/cursor_shapes.meta.json
--rw-r--r--   0        0        0    31349 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/data_structures.data.json
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/data_structures.meta.json
--rw-r--r--   0        0        0    87520 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/document.data.json
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/document.meta.json
--rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/enums.data.json
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/enums.meta.json
--rw-r--r--   0        0        0    28526 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/history.data.json
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/history.meta.json
--rw-r--r--   0        0        0    65848 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/keys.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/keys.meta.json
--rw-r--r--   0        0        0    14425 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/mouse_events.data.json
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/mouse_events.meta.json
--rw-r--r--   0        0        0    23629 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/patch_stdout.data.json
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/patch_stdout.meta.json
--rw-r--r--   0        0        0    42743 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/renderer.data.json
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/renderer.meta.json
--rw-r--r--   0        0        0    13657 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/search.data.json
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/search.meta.json
--rw-r--r--   0        0        0    10289 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/selection.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/selection.meta.json
--rw-r--r--   0        0        0    35717 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/utils.data.json
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/utils.meta.json
--rw-r--r--   0        0        0    30382 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/validation.data.json
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/validation.meta.json
--rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/application/__init__.data.json
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/application/__init__.meta.json
--rw-r--r--   0        0        0   116580 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/application/application.data.json
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/application/application.meta.json
--rw-r--r--   0        0        0    17411 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/application/current.data.json
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/application/current.meta.json
--rw-r--r--   0        0        0     9568 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/application/dummy.data.json
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/application/dummy.meta.json
--rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/application/run_in_terminal.data.json
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/application/run_in_terminal.meta.json
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/clipboard/__init__.data.json
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/clipboard/__init__.meta.json
--rw-r--r--   0        0        0    20695 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/clipboard/base.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/clipboard/base.meta.json
--rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/clipboard/in_memory.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/clipboard/in_memory.meta.json
--rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/completion/__init__.data.json
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/completion/__init__.meta.json
--rw-r--r--   0        0        0    49069 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/completion/base.data.json
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/completion/base.meta.json
--rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/completion/deduplicate.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/completion/deduplicate.meta.json
--rw-r--r--   0        0        0    10866 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/completion/filesystem.data.json
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/completion/filesystem.meta.json
--rw-r--r--   0        0        0    34018 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/completion/fuzzy_completer.data.json
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/completion/fuzzy_completer.meta.json
--rw-r--r--   0        0        0    10210 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/completion/nested.data.json
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/completion/nested.meta.json
--rw-r--r--   0        0        0    10571 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/completion/word_completer.data.json
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/completion/word_completer.meta.json
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/eventloop/__init__.data.json
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/eventloop/__init__.meta.json
--rw-r--r--   0        0        0    15354 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/eventloop/async_context_manager.data.json
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/eventloop/async_context_manager.meta.json
--rw-r--r--   0        0        0    12774 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/eventloop/async_generator.data.json
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/eventloop/async_generator.meta.json
--rw-r--r--   0        0        0    22342 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/eventloop/dummy_contextvars.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/eventloop/dummy_contextvars.meta.json
--rw-r--r--   0        0        0    19676 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/eventloop/inputhook.data.json
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/eventloop/inputhook.meta.json
--rw-r--r--   0        0        0     8541 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/eventloop/utils.data.json
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/eventloop/utils.meta.json
--rw-r--r--   0        0        0     9943 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/filters/__init__.data.json
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/filters/__init__.meta.json
--rw-r--r--   0        0        0    31137 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/filters/app.data.json
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/filters/app.meta.json
--rw-r--r--   0        0        0    35307 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/filters/base.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/filters/base.meta.json
--rw-r--r--   0        0        0    20205 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/filters/cli.data.json
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/filters/cli.meta.json
--rw-r--r--   0        0        0     4798 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/filters/utils.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/filters/utils.meta.json
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/formatted_text/__init__.data.json
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/formatted_text/__init__.meta.json
--rw-r--r--   0        0        0    17680 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/formatted_text/ansi.data.json
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/formatted_text/ansi.meta.json
--rw-r--r--   0        0        0    16203 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/formatted_text/base.data.json
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/formatted_text/base.meta.json
--rw-r--r--   0        0        0    10955 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/formatted_text/html.data.json
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/formatted_text/html.meta.json
--rw-r--r--   0        0        0     6736 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/formatted_text/pygments.data.json
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/formatted_text/pygments.meta.json
--rw-r--r--   0        0        0     6887 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/formatted_text/utils.data.json
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/formatted_text/utils.meta.json
--rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/input/__init__.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/input/__init__.meta.json
--rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/input/ansi_escape_sequences.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/input/ansi_escape_sequences.meta.json
--rw-r--r--   0        0        0    31531 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/input/base.data.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/input/base.meta.json
--rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/input/defaults.data.json
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/input/defaults.meta.json
--rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/input/typeahead.data.json
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/input/typeahead.meta.json
--rw-r--r--   0        0        0    18000 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/input/vt100_parser.data.json
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/input/vt100_parser.meta.json
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/__init__.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/__init__.meta.json
--rw-r--r--   0        0        0     4744 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/defaults.data.json
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/defaults.meta.json
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/digraphs.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/digraphs.meta.json
--rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/emacs_state.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/emacs_state.meta.json
--rw-r--r--   0        0        0    65935 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/key_bindings.data.json
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/key_bindings.meta.json
--rw-r--r--   0        0        0    41736 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/key_processor.data.json
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/key_processor.meta.json
--rw-r--r--   0        0        0    18379 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/vi_state.data.json
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/vi_state.meta.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/__init__.data.json
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/__init__.meta.json
--rw-r--r--   0        0        0     3880 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/auto_suggest.data.json
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/auto_suggest.meta.json
--rw-r--r--   0        0        0     5505 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/basic.data.json
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/basic.meta.json
--rw-r--r--   0        0        0     7918 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/completion.data.json
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/completion.meta.json
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/cpr.data.json
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/cpr.meta.json
--rw-r--r--   0        0        0     8255 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/emacs.data.json
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/emacs.meta.json
--rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/focus.data.json
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/focus.meta.json
--rw-r--r--   0        0        0    12947 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/mouse.data.json
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/mouse.meta.json
--rw-r--r--   0        0        0    77971 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/named_commands.data.json
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/named_commands.meta.json
--rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/open_in_editor.data.json
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/open_in_editor.meta.json
--rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/page_navigation.data.json
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/page_navigation.meta.json
--rw-r--r--   0        0        0     8280 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/scroll.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/scroll.meta.json
--rw-r--r--   0        0        0    32939 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/vi.data.json
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/vi.meta.json
--rw-r--r--   0        0        0     6953 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/__init__.data.json
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/__init__.meta.json
--rw-r--r--   0        0        0   191072 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/containers.data.json
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/containers.meta.json
--rw-r--r--   0        0        0   103397 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/controls.data.json
--rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/controls.meta.json
--rw-r--r--   0        0        0    15289 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/dimension.data.json
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/dimension.meta.json
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/dummy.data.json
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/dummy.meta.json
--rw-r--r--   0        0        0    35473 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/layout.data.json
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/layout.meta.json
--rw-r--r--   0        0        0    29041 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/margins.data.json
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/margins.meta.json
--rw-r--r--   0        0        0    43226 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/menus.data.json
--rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/menus.meta.json
--rw-r--r--   0        0        0     6979 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/mouse_handlers.data.json
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/mouse_handlers.meta.json
--rw-r--r--   0        0        0    85872 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/processors.data.json
--rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/processors.meta.json
--rw-r--r--   0        0        0    27012 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/screen.data.json
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/screen.meta.json
--rw-r--r--   0        0        0    25956 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/scrollable_pane.data.json
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/scrollable_pane.meta.json
--rw-r--r--   0        0        0    45237 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/utils.data.json
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/utils.meta.json
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/lexers/__init__.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/lexers/__init__.meta.json
--rw-r--r--   0        0        0    14816 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/lexers/base.data.json
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/lexers/base.meta.json
--rw-r--r--   0        0        0    25563 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/lexers/pygments.data.json
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/lexers/pygments.meta.json
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/output/__init__.data.json
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/output/__init__.meta.json
--rw-r--r--   0        0        0    78123 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/output/base.data.json
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/output/base.meta.json
--rw-r--r--   0        0        0    10015 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/output/color_depth.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/output/color_depth.meta.json
--rw-r--r--   0        0        0     4215 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/output/defaults.data.json
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/output/defaults.meta.json
--rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/output/flush_stdout.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/output/flush_stdout.meta.json
--rw-r--r--   0        0        0    31685 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/output/plain_text.data.json
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/output/plain_text.meta.json
--rw-r--r--   0        0        0    56262 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/output/vt100.data.json
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/output/vt100.meta.json
--rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/shortcuts/__init__.data.json
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/shortcuts/__init__.meta.json
--rw-r--r--   0        0        0    22835 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/shortcuts/dialogs.data.json
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/shortcuts/dialogs.meta.json
--rw-r--r--   0        0        0   114712 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/shortcuts/prompt.data.json
--rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/shortcuts/prompt.meta.json
--rw-r--r--   0        0        0    11079 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/shortcuts/utils.data.json
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/shortcuts/utils.meta.json
--rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/shortcuts/progress_bar/__init__.data.json
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/shortcuts/progress_bar/__init__.meta.json
--rw-r--r--   0        0        0    57362 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/shortcuts/progress_bar/base.data.json
--rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/shortcuts/progress_bar/base.meta.json
--rw-r--r--   0        0        0    53097 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/shortcuts/progress_bar/formatters.data.json
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/shortcuts/progress_bar/formatters.meta.json
--rw-r--r--   0        0        0     5348 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/styles/__init__.data.json
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/styles/__init__.meta.json
--rw-r--r--   0        0        0    52925 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/styles/base.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/styles/base.meta.json
--rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/styles/defaults.data.json
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/styles/defaults.meta.json
--rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/styles/named_colors.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/styles/named_colors.meta.json
--rw-r--r--   0        0        0     5665 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/styles/pygments.data.json
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/styles/pygments.meta.json
--rw-r--r--   0        0        0    28725 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/styles/style.data.json
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/styles/style.meta.json
--rw-r--r--   0        0        0    45971 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/styles/style_transformation.data.json
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/styles/style_transformation.meta.json
--rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/widgets/__init__.data.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/widgets/__init__.meta.json
--rw-r--r--   0        0        0    97873 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/widgets/base.data.json
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/widgets/base.meta.json
--rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/widgets/dialogs.data.json
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/widgets/dialogs.meta.json
--rw-r--r--   0        0        0    20613 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/widgets/menus.data.json
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/widgets/menus.meta.json
--rw-r--r--   0        0        0    31768 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/widgets/toolbars.data.json
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/widgets/toolbars.meta.json
--rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pydal2sql/__init__.data.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pydal2sql/__init__.meta.json
--rw-r--r--   0        0        0    41445 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pydal2sql/typer_support.data.json
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pydal2sql/typer_support.meta.json
--rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pydal2sql/types.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pydal2sql/types.meta.json
--rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pydal2sql_core/__init__.data.json
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pydal2sql_core/__init__.meta.json
--rw-r--r--   0        0        0    33442 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pydal2sql_core/cli_support.data.json
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pydal2sql_core/cli_support.meta.json
--rw-r--r--   0        0        0    11990 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pydal2sql_core/core.data.json
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pydal2sql_core/core.meta.json
--rw-r--r--   0        0        0    14843 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pydal2sql_core/helpers.data.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pydal2sql_core/helpers.meta.json
--rw-r--r--   0        0        0    17244 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pydal2sql_core/types.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pydal2sql_core/types.meta.json
--rw-r--r--   0        0        0    37406 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pyexpat/__init__.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pyexpat/__init__.meta.json
--rw-r--r--   0        0        0    11760 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pyexpat/errors.data.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pyexpat/errors.meta.json
--rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pyexpat/model.data.json
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pyexpat/model.meta.json
--rw-r--r--   0        0        0    11300 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pytest/__init__.data.json
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/pytest/__init__.meta.json
--rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/__init__.data.json
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/__init__.meta.json
--rw-r--r--   0        0        0     4346 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/constants.data.json
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/constants.meta.json
--rw-r--r--   0        0        0    23428 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/form.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/form.meta.json
--rw-r--r--   0        0        0     8188 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompt.data.json
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompt.meta.json
--rw-r--r--   0        0        0     9442 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/question.data.json
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/question.meta.json
--rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/styles.data.json
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/styles.meta.json
--rw-r--r--   0        0        0    10514 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/utils.data.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/utils.meta.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/version.data.json
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/version.meta.json
--rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/__init__.data.json
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/__init__.meta.json
--rw-r--r--   0        0        0    14644 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/autocomplete.data.json
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/autocomplete.meta.json
--rw-r--r--   0        0        0     7096 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/checkbox.data.json
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/checkbox.meta.json
--rw-r--r--   0        0        0    34906 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/common.data.json
--rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/common.meta.json
--rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/confirm.data.json
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/confirm.meta.json
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/password.data.json
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/password.meta.json
--rw-r--r--   0        0        0    10875 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/path.data.json
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/path.meta.json
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/press_any_key_to_continue.data.json
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/press_any_key_to_continue.meta.json
--rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/rawselect.data.json
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/rawselect.meta.json
--rw-r--r--   0        0        0     5962 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/select.data.json
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/select.meta.json
--rw-r--r--   0        0        0     4730 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/text.data.json
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/text.meta.json
--rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/__init__.data.json
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/__init__.meta.json
--rw-r--r--   0        0        0    16999 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/backoff.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/backoff.meta.json
--rw-r--r--   0        0        0    85848 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/client.data.json
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/client.meta.json
--rw-r--r--   0        0        0    93397 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/cluster.data.json
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/cluster.meta.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/compat.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/compat.meta.json
--rw-r--r--   0        0        0    66520 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/connection.data.json
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/connection.meta.json
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/crc.data.json
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/crc.meta.json
--rw-r--r--   0        0        0     6763 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/credentials.data.json
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/credentials.meta.json
--rw-r--r--   0        0        0    38204 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/exceptions.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/exceptions.meta.json
--rw-r--r--   0        0        0    17826 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/lock.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/lock.meta.json
--rw-r--r--   0        0        0    10756 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/ocsp.data.json
--rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/ocsp.meta.json
--rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/retry.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/retry.meta.json
--rw-r--r--   0        0        0    25650 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/sentinel.data.json
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/sentinel.meta.json
--rw-r--r--   0        0        0    14572 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/typing.data.json
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/typing.meta.json
--rw-r--r--   0        0        0     8733 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/utils.data.json
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/utils.meta.json
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/__init__.data.json
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/__init__.meta.json
--rw-r--r--   0        0        0    25974 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/base.data.json
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/base.meta.json
--rw-r--r--   0        0        0    13625 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/commands.data.json
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/commands.meta.json
--rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/encoders.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/encoders.meta.json
--rw-r--r--   0        0        0    19890 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/helpers.data.json
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/helpers.meta.json
--rw-r--r--   0        0        0    16424 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/hiredis.data.json
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/hiredis.meta.json
--rw-r--r--   0        0        0     7715 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/resp2.data.json
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/resp2.meta.json
--rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/resp3.data.json
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/resp3.meta.json
--rw-r--r--   0        0        0    13926 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/socket.data.json
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/socket.meta.json
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/asyncio/__init__.data.json
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/asyncio/__init__.meta.json
--rw-r--r--   0        0        0   110856 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/asyncio/client.data.json
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/asyncio/client.meta.json
--rw-r--r--   0        0        0   103724 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/asyncio/cluster.data.json
--rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/asyncio/cluster.meta.json
--rw-r--r--   0        0        0    95161 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/asyncio/connection.data.json
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/asyncio/connection.meta.json
--rw-r--r--   0        0        0    18737 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/asyncio/lock.data.json
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/asyncio/lock.meta.json
--rw-r--r--   0        0        0     9741 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/asyncio/retry.data.json
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/asyncio/retry.meta.json
--rw-r--r--   0        0        0    28762 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/asyncio/sentinel.data.json
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/asyncio/sentinel.meta.json
--rw-r--r--   0        0        0     5149 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/asyncio/utils.data.json
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/asyncio/utils.meta.json
--rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/__init__.data.json
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/__init__.meta.json
--rw-r--r--   0        0        0    93587 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/cluster.data.json
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/cluster.meta.json
--rw-r--r--   0        0        0   401564 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/core.data.json
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/core.meta.json
--rw-r--r--   0        0        0     6004 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/helpers.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/helpers.meta.json
--rw-r--r--   0        0        0     6977 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/redismodules.data.json
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/redismodules.meta.json
--rw-r--r--   0        0        0     8799 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/sentinel.data.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/sentinel.meta.json
--rw-r--r--   0        0        0    36127 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/bf/__init__.data.json
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/bf/__init__.meta.json
--rw-r--r--   0        0        0    35430 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/bf/commands.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/bf/commands.meta.json
--rw-r--r--   0        0        0    20186 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/bf/info.data.json
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/bf/info.meta.json
--rw-r--r--   0        0        0    16330 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/graph/__init__.data.json
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/graph/__init__.meta.json
--rw-r--r--   0        0        0    12253 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/graph/commands.data.json
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/graph/commands.meta.json
--rw-r--r--   0        0        0     5581 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/graph/edge.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/graph/edge.meta.json
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/graph/exceptions.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/graph/exceptions.meta.json
--rw-r--r--   0        0        0    12629 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/graph/execution_plan.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/graph/execution_plan.meta.json
--rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/graph/node.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/graph/node.meta.json
--rw-r--r--   0        0        0     8795 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/graph/path.data.json
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/graph/path.meta.json
--rw-r--r--   0        0        0    43138 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/graph/query_result.data.json
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/graph/query_result.meta.json
--rw-r--r--   0        0        0    11069 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/json/__init__.data.json
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/json/__init__.meta.json
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/json/_util.data.json
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/json/_util.meta.json
--rw-r--r--   0        0        0    31474 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/json/commands.data.json
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/json/commands.meta.json
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/json/decoders.data.json
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/json/decoders.meta.json
--rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/json/path.data.json
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/json/path.meta.json
--rw-r--r--   0        0        0    19740 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/search/__init__.data.json
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/search/__init__.meta.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/search/_util.data.json
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/search/_util.meta.json
--rw-r--r--   0        0        0    34189 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/search/aggregation.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/search/aggregation.meta.json
--rw-r--r--   0        0        0    55636 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/search/commands.data.json
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/search/commands.meta.json
--rw-r--r--   0        0        0     3840 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/search/document.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/search/document.meta.json
--rw-r--r--   0        0        0    38931 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/search/query.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/search/query.meta.json
--rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/search/result.data.json
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/search/result.meta.json
--rw-r--r--   0        0        0     8818 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/search/suggestion.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/search/suggestion.meta.json
--rw-r--r--   0        0        0    12615 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/timeseries/__init__.data.json
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/timeseries/__init__.meta.json
--rw-r--r--   0        0        0    68529 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/timeseries/commands.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/timeseries/commands.meta.json
--rw-r--r--   0        0        0     8125 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/timeseries/info.data.json
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/timeseries/info.meta.json
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/timeseries/utils.data.json
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/timeseries/utils.meta.json
--rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/__init__.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/__init__.meta.json
--rw-r--r--   0        0        0     8768 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/__main__.data.json
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/__main__.meta.json
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_cell_widths.data.json
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_cell_widths.meta.json
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_emoji_codes.data.json
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_emoji_codes.meta.json
--rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_emoji_replace.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_emoji_replace.meta.json
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_export_format.data.json
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_export_format.meta.json
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_extension.data.json
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_extension.meta.json
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_fileno.data.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_fileno.meta.json
--rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_log_render.data.json
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_log_render.meta.json
--rw-r--r--   0        0        0     6839 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_loop.data.json
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_loop.meta.json
--rw-r--r--   0        0        0    16444 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_null_file.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_null_file.meta.json
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_palettes.data.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_palettes.meta.json
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_pick.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_pick.meta.json
--rw-r--r--   0        0        0    12590 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_ratio.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_ratio.meta.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_spinners.data.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_spinners.meta.json
--rw-r--r--   0        0        0     7101 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_stack.data.json
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_stack.meta.json
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_timer.data.json
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_timer.meta.json
--rw-r--r--   0        0        0    53433 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_win32_console.data.json
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_win32_console.meta.json
--rw-r--r--   0        0        0     8940 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_windows.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_windows.meta.json
--rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_windows_renderer.data.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_windows_renderer.meta.json
--rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_wrap.data.json
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/_wrap.meta.json
--rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/abc.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/abc.meta.json
--rw-r--r--   0        0        0    24347 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/align.data.json
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/align.meta.json
--rw-r--r--   0        0        0    26848 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/ansi.data.json
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/ansi.meta.json
--rw-r--r--   0        0        0    21129 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/box.data.json
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/box.meta.json
--rw-r--r--   0        0        0     8887 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/cells.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/cells.meta.json
--rw-r--r--   0        0        0    57697 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/color.data.json
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/color.meta.json
--rw-r--r--   0        0        0    21972 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/color_triplet.data.json
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/color_triplet.meta.json
--rw-r--r--   0        0        0    11427 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/columns.data.json
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/columns.meta.json
--rw-r--r--   0        0        0   190779 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/console.data.json
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/console.meta.json
--rw-r--r--   0        0        0     6421 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/constrain.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/constrain.meta.json
--rw-r--r--   0        0        0    22261 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/containers.data.json
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/containers.meta.json
--rw-r--r--   0        0        0    23326 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/control.data.json
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/control.meta.json
--rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/default_styles.data.json
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/default_styles.meta.json
--rw-r--r--   0        0        0    11746 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/emoji.data.json
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/emoji.meta.json
--rw-r--r--   0        0        0    10354 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/errors.data.json
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/errors.meta.json
--rw-r--r--   0        0        0     9209 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/file_proxy.data.json
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/file_proxy.meta.json
--rw-r--r--   0        0        0    16680 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/highlighter.data.json
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/highlighter.meta.json
--rw-r--r--   0        0        0    10622 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/json.data.json
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/json.meta.json
--rw-r--r--   0        0        0    10805 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/jupyter.data.json
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/jupyter.meta.json
--rw-r--r--   0        0        0    30064 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/live.data.json
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/live.meta.json
--rw-r--r--   0        0        0     9936 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/live_render.data.json
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/live_render.meta.json
--rw-r--r--   0        0        0    88816 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/markdown.data.json
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/markdown.meta.json
--rw-r--r--   0        0        0    27404 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/markup.data.json
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/markup.meta.json
--rw-r--r--   0        0        0    25218 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/measure.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/measure.meta.json
--rw-r--r--   0        0        0    13374 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/padding.data.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/padding.meta.json
--rw-r--r--   0        0        0     6681 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/pager.data.json
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/pager.meta.json
--rw-r--r--   0        0        0    10046 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/palette.data.json
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/palette.meta.json
--rw-r--r--   0        0        0    18539 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/panel.data.json
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/panel.meta.json
--rw-r--r--   0        0        0   133658 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/pretty.data.json
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/pretty.meta.json
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/protocol.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/protocol.meta.json
--rw-r--r--   0        0        0    16838 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/region.data.json
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/region.meta.json
--rw-r--r--   0        0        0    29387 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/repr.data.json
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/repr.meta.json
--rw-r--r--   0        0        0     9164 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/rule.data.json
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/rule.meta.json
--rw-r--r--   0        0        0     4759 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/scope.data.json
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/scope.meta.json
--rw-r--r--   0        0        0     6015 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/screen.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/screen.meta.json
--rw-r--r--   0        0        0   100846 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/segment.data.json
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/segment.meta.json
--rw-r--r--   0        0        0    11158 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/spinner.data.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/spinner.meta.json
--rw-r--r--   0        0        0    13247 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/status.data.json
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/status.meta.json
--rw-r--r--   0        0        0    58607 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/style.data.json
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/style.meta.json
--rw-r--r--   0        0        0     6702 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/styled.data.json
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/styled.meta.json
--rw-r--r--   0        0        0    81805 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/syntax.data.json
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/syntax.meta.json
--rw-r--r--   0        0        0    86262 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/table.data.json
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/table.meta.json
--rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/terminal_theme.data.json
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/terminal_theme.meta.json
--rw-r--r--   0        0        0    92014 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/text.data.json
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/text.meta.json
--rw-r--r--   0        0        0    15945 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/theme.data.json
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/theme.meta.json
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/themes.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/themes.meta.json
--rw-r--r--   0        0        0    58612 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/traceback.data.json
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/rich/traceback.meta.json
--rw-r--r--   0        0        0    22875 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/sqlite3/__init__.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/sqlite3/__init__.meta.json
--rw-r--r--   0        0        0   185529 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/sqlite3/dbapi2.data.json
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/sqlite3/dbapi2.meta.json
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/src/__init__.data.json
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/src/__init__.meta.json
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/src/typedal/__about__.data.json
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/src/typedal/__about__.meta.json
--rw-r--r--   0        0        0    13692 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/src/typedal/config.data.json
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/src/typedal/config.meta.json
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/su6/__about__.data.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/su6/__about__.meta.json
--rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/su6/__init__.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/su6/__init__.meta.json
--rw-r--r--   0        0        0    27733 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/su6/cli.data.json
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/su6/cli.meta.json
--rw-r--r--   0        0        0    67427 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/su6/core.data.json
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/su6/core.meta.json
--rw-r--r--   0        0        0    63551 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/su6/plugins.data.json
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/su6/plugins.meta.json
--rw-r--r--   0        0        0   155536 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/sys/__init__.data.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/sys/__init__.meta.json
--rw-r--r--   0        0        0    93809 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tabulate/__init__.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tabulate/__init__.meta.json
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tabulate/version.data.json
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tabulate/version.meta.json
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tests/__init__.data.json
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tests/__init__.meta.json
--rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomli/__init__.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomli/__init__.meta.json
--rw-r--r--   0        0        0    55884 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomli/_parser.data.json
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomli/_parser.meta.json
--rw-r--r--   0        0        0     7143 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomli/_re.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomli/_re.meta.json
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomli/_types.data.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomli/_types.meta.json
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomli_w/__init__.data.json
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomli_w/__init__.meta.json
--rw-r--r--   0        0        0    34224 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomli_w/_writer.data.json
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomli_w/_writer.meta.json
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/__init__.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/__init__.meta.json
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/_compat.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/_compat.meta.json
--rw-r--r--   0        0        0     9960 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/_types.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/_types.meta.json
--rw-r--r--   0        0        0     8336 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/_utils.data.json
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/_utils.meta.json
--rw-r--r--   0        0        0    24999 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/api.data.json
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/api.meta.json
--rw-r--r--   0        0        0    50132 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/container.data.json
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/container.meta.json
--rw-r--r--   0        0        0    38878 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/exceptions.data.json
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/exceptions.meta.json
--rw-r--r--   0        0        0   287553 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/items.data.json
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/items.meta.json
--rw-r--r--   0        0        0    36621 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/parser.data.json
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/parser.meta.json
--rw-r--r--   0        0        0    24225 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/source.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/source.meta.json
--rw-r--r--   0        0        0     8088 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/toml_char.data.json
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/toml_char.meta.json
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/toml_document.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/toml_document.meta.json
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typedal/__about__.data.json
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typedal/__about__.meta.json
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typedal/__init__.data.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typedal/__init__.meta.json
--rw-r--r--   0        0        0    36289 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typedal/caching.data.json
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typedal/caching.meta.json
--rw-r--r--   0        0        0    27838 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typedal/cli.data.json
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typedal/cli.meta.json
--rw-r--r--   0        0        0    22466 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typedal/config.data.json
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typedal/config.meta.json
--rw-r--r--   0        0        0   301190 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typedal/core.data.json
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typedal/core.meta.json
--rw-r--r--   0        0        0    30719 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typedal/fields.data.json
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typedal/fields.meta.json
--rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typedal/for_py4web.data.json
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typedal/for_py4web.meta.json
--rw-r--r--   0        0        0    12836 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typedal/for_web2py.data.json
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typedal/for_web2py.meta.json
--rw-r--r--   0        0        0    28464 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typedal/helpers.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typedal/helpers.meta.json
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typedal/serializers.data.json
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typedal/serializers.meta.json
--rw-r--r--   0        0        0    24209 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typedal/types.data.json
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typedal/types.meta.json
--rw-r--r--   0        0        0     9735 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typedal/web2py_py4web_shared.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typedal/web2py_py4web_shared.meta.json
--rw-r--r--   0        0        0    10626 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typedal/serializers/as_json.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typedal/serializers/as_json.meta.json
--rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typeguard/__init__.data.json
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typeguard/__init__.meta.json
--rw-r--r--   0        0        0    40710 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_checkers.data.json
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_checkers.meta.json
--rw-r--r--   0        0        0    15819 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_config.data.json
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_config.meta.json
--rw-r--r--   0        0        0    35537 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_decorators.data.json
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_decorators.meta.json
--rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_exceptions.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_exceptions.meta.json
--rw-r--r--   0        0        0    23488 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_functions.data.json
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_functions.meta.json
--rw-r--r--   0        0        0    23369 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_importhook.data.json
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_importhook.meta.json
--rw-r--r--   0        0        0     5789 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_memo.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_memo.meta.json
--rw-r--r--   0        0        0    21446 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_suppression.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_suppression.meta.json
--rw-r--r--   0        0        0    85648 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_transformer.data.json
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_transformer.meta.json
--rw-r--r--   0        0        0    11727 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_utils.data.json
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_utils.meta.json
--rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typer/__init__.data.json
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typer/__init__.meta.json
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typer/_compat_utils.data.json
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typer/_compat_utils.meta.json
--rw-r--r--   0        0        0    12325 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typer/_completion_shared.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typer/_completion_shared.meta.json
--rw-r--r--   0        0        0    36460 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typer/_typing.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typer/_typing.meta.json
--rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typer/colors.data.json
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typer/colors.meta.json
--rw-r--r--   0        0        0     9694 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typer/completion.data.json
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typer/completion.meta.json
--rw-r--r--   0        0        0    50878 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typer/core.data.json
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typer/core.meta.json
--rw-r--r--   0        0        0    57396 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typer/main.data.json
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typer/main.meta.json
--rw-r--r--   0        0        0    74258 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typer/models.data.json
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typer/models.meta.json
--rw-r--r--   0        0        0    78838 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typer/params.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typer/params.meta.json
--rw-r--r--   0        0        0    33649 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typer/rich_utils.data.json
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typer/rich_utils.meta.json
--rw-r--r--   0        0        0    19703 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typer/utils.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/typer/utils.meta.json
--rw-r--r--   0        0        0     6249 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/unittest/__init__.data.json
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/unittest/__init__.meta.json
--rw-r--r--   0        0        0    27032 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/unittest/_log.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/unittest/_log.meta.json
--rw-r--r--   0        0        0    11460 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/unittest/async_case.data.json
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/unittest/async_case.meta.json
--rw-r--r--   0        0        0   286451 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/unittest/case.data.json
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/unittest/case.meta.json
--rw-r--r--   0        0        0    15314 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/unittest/loader.data.json
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/unittest/loader.meta.json
--rw-r--r--   0        0        0    12573 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/unittest/main.data.json
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/unittest/main.meta.json
--rw-r--r--   0        0        0   193614 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/unittest/mock.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/unittest/mock.meta.json
--rw-r--r--   0        0        0    22521 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/unittest/result.data.json
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/unittest/result.meta.json
--rw-r--r--   0        0        0    13338 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/unittest/runner.data.json
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/unittest/runner.meta.json
--rw-r--r--   0        0        0    17553 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/unittest/signals.data.json
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/unittest/signals.meta.json
--rw-r--r--   0        0        0    12052 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/unittest/suite.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/unittest/suite.meta.json
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/urllib/__init__.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/urllib/__init__.meta.json
--rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/urllib/error.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/urllib/error.meta.json
--rw-r--r--   0        0        0   235720 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/urllib/parse.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/urllib/parse.meta.json
--rw-r--r--   0        0        0   169451 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/urllib/request.data.json
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/urllib/request.meta.json
--rw-r--r--   0        0        0    30659 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/urllib/response.data.json
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/urllib/response.meta.json
--rw-r--r--   0        0        0    31341 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/witchery/__init__.data.json
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/witchery/__init__.meta.json
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/xml/__init__.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/xml/__init__.meta.json
--rw-r--r--   0        0        0    30071 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/xml/dom/__init__.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/xml/dom/__init__.meta.json
--rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/xml/dom/domreg.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/xml/dom/domreg.meta.json
--rw-r--r--   0        0        0    67176 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/xml/dom/expatbuilder.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/xml/dom/expatbuilder.meta.json
--rw-r--r--   0        0        0    15865 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/xml/dom/minicompat.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/xml/dom/minicompat.meta.json
--rw-r--r--   0        0        0   173371 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/xml/dom/minidom.data.json
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/xml/dom/minidom.meta.json
--rw-r--r--   0        0        0    36037 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/xml/dom/xmlbuilder.data.json
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/xml/dom/xmlbuilder.meta.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/xml/parsers/__init__.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/xml/parsers/__init__.meta.json
--rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/xml/parsers/expat/__init__.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/xml/parsers/expat/__init__.meta.json
--rw-r--r--   0        0        0    20645 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/xml/sax/__init__.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/xml/sax/__init__.meta.json
--rw-r--r--   0        0        0    26771 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/xml/sax/handler.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/xml/sax/handler.meta.json
--rw-r--r--   0        0        0    53739 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/xml/sax/xmlreader.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/xml/sax/xmlreader.meta.json
--rw-r--r--   0        0        0   188224 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/__init__.data.json
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/__init__.meta.json
--rw-r--r--   0        0        0    23798 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/_yaml.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/_yaml.meta.json
--rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/composer.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/composer.meta.json
--rw-r--r--   0        0        0    48721 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/constructor.data.json
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/constructor.meta.json
--rw-r--r--   0        0        0    21570 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/cyaml.data.json
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/cyaml.meta.json
--rw-r--r--   0        0        0    13642 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/dumper.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/dumper.meta.json
--rw-r--r--   0        0        0    63025 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/emitter.data.json
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/emitter.meta.json
--rw-r--r--   0        0        0     9518 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/error.data.json
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/error.meta.json
--rw-r--r--   0        0        0    31137 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/events.data.json
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/events.meta.json
--rw-r--r--   0        0        0    13347 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/loader.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/loader.meta.json
--rw-r--r--   0        0        0    11844 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/nodes.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/nodes.meta.json
--rw-r--r--   0        0        0    15083 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/parser.data.json
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/parser.meta.json
--rw-r--r--   0        0        0    13189 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/reader.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/reader.meta.json
--rw-r--r--   0        0        0    46065 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/representer.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/representer.meta.json
--rw-r--r--   0        0        0    11331 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/resolver.data.json
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/resolver.meta.json
--rw-r--r--   0        0        0    31183 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/scanner.data.json
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/scanner.meta.json
--rw-r--r--   0        0        0    10682 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/serializer.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/serializer.meta.json
--rw-r--r--   0        0        0    40449 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/tokens.data.json
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.mypy_cache/3.11/yaml/tokens.meta.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.pytest_cache/README.md
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     4398 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/0.1.14/15432600919105507093
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/0.1.14/7801493945118068108
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/0.1.6/2759713849472344579
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/0.1.7/14298551053547083375
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/0.1.7/3401287376304810316
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/1215429078721865123
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/121ed75fe9fe5f8e
--rw-r--r--   0        0        0    23412 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/14855161046259211094
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/19309938546e93ab
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/197f3188bc94f91f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/1aa1390b5bde1004
--rw-r--r--   0        0        0     8089 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/1b34455c399f0006
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/1bd1a229a4f4ee7f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/1c46d1f378d28fbb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/1ca71ee291d82018
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/1d6bb777df44b8ec
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/1dc8423cfb79eaa4
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/20585cf790eae81e
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/217892307344966949
--rw-r--r--   0        0        0    12122 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/221af82ae72a7f27
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/2282e801459c52a4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/248c4e1a32c704cb
--rw-r--r--   0        0        0    10858 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/24e1b4aab386ebc8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/28b1d8ac7e2aab6b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/2b7f7d266c8efaad
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/2bb6610cadf18e18
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/2dac345be8527adf
--rw-r--r--   0        0        0    11525 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/2f3396c610fd7095
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/31731f8e74291475
--rw-r--r--   0        0        0    13342 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/322af04e6d059ce5
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/3826106cf4494de8
--rw-r--r--   0        0        0    11210 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/38d5fd55b14a9d6c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/3afc55a04b8f8bb2
--rw-r--r--   0        0        0    12129 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/4022ee8774ccd98a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/42f9a2406e74c24f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/4696b157ff786f22
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/46a88ce266f1ad94
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/4a6edd5010cb9700
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/4d0230e9a81a468
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/52018ba3989fcaf7
--rw-r--r--   0        0        0    13679 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/5491563776466765346
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/54e6ba8c25a22ffc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/566d94db91d23339
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/5a67aed8f6b70cd5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/5b076d769fa5cacd
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/5ceb1580c62ee794
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/6bc90dbb56504f96
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/6c52d14716eee431
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/6f0c8f98e4da1d48
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/74e52af774eebdbd
--rw-r--r--   0        0        0    11023 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/75bd1769f6e29ed7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/815ba2cfea236769
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/876d9a8d302e1c46
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/8891791100357482236
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/88e2927df9448936
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/8c4d3f5ef14b0167
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/8f8ec552e76f3eab
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/95c82d8566c6704c
--rw-r--r--   0        0        0     8349 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/a0739889bf9412e8
--rw-r--r--   0        0        0     5692 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/a225e4df39be9b29
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/a2340fd4c9aa1141
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/a513d558646cd439
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/b121e2b70fd66eb8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/b218ff88bc22b626
--rw-r--r--   0        0        0    10964 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/b419496fa9e72887
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/b886c97e4d4117f0
--rw-r--r--   0        0        0     8238 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/bdcdf5c7bbc1d738
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/c06de16f3c7a64cc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/c635f255374598c5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/c671ae94ff3d3e2e
--rw-r--r--   0        0        0     8042 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/cdfecbca581311ee
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/ce44121ca4091b64
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/ced49ec87d10bcb0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/cfc06a1f13c8ab47
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/d16c5d29763a704e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/d225ad4c14b8ca60
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/d379b35d5e80b789
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/d3a95555c0919160
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/d655bee8ff0a59f2
--rw-r--r--   0        0        0    11315 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/da4811a7730a562a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/dca573767bc8be7e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/e3e29f9eacb7027f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/e46ab4b61bb5d446
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/e5e0cc178d5c9df5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/eb564f7989641958
--rw-r--r--   0        0        0    11467 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/eee2f3c667de6c7a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/f04d0d78a00adfd6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/f2ddc22a4b221f54
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/f879e8c947a6b7a4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/fa45ef3c3166e02d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.ruff_cache/content/faa51a5044a3c279
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 typedal-3.0.0b3/docs/1_getting_started.md
--rw-r--r--   0        0        0     6509 2020-02-02 00:00:00.000000 typedal-3.0.0b3/docs/2_defining_tables.md
--rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 typedal-3.0.0b3/docs/3_building_queries.md
--rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 typedal-3.0.0b3/docs/4_relationships.md
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 typedal-3.0.0b3/docs/5_py4web.md
--rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 typedal-3.0.0b3/docs/6_migrations.md
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 typedal-3.0.0b3/docs/index.md
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 typedal-3.0.0b3/docs/requirements.txt
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 typedal-3.0.0b3/docs/css/code_blocks.css
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 typedal-3.0.0b3/htmlcov/.gitignore
--rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 typedal-3.0.0b3/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     5891 2020-02-02 00:00:00.000000 typedal-3.0.0b3/htmlcov/d_0ccc93afd6526b6c___about___py.html
--rw-r--r--   0        0        0     7907 2020-02-02 00:00:00.000000 typedal-3.0.0b3/htmlcov/d_0ccc93afd6526b6c___init___py.html
--rw-r--r--   0        0        0   119633 2020-02-02 00:00:00.000000 typedal-3.0.0b3/htmlcov/d_0ccc93afd6526b6c_caching_py.html
--rw-r--r--   0        0        0   146640 2020-02-02 00:00:00.000000 typedal-3.0.0b3/htmlcov/d_0ccc93afd6526b6c_cli_py.html
--rw-r--r--   0        0        0   104666 2020-02-02 00:00:00.000000 typedal-3.0.0b3/htmlcov/d_0ccc93afd6526b6c_config_py.html
--rw-r--r--   0        0        0   778432 2020-02-02 00:00:00.000000 typedal-3.0.0b3/htmlcov/d_0ccc93afd6526b6c_core_py.html
--rw-r--r--   0        0        0    61614 2020-02-02 00:00:00.000000 typedal-3.0.0b3/htmlcov/d_0ccc93afd6526b6c_fields_py.html
--rw-r--r--   0        0        0    17238 2020-02-02 00:00:00.000000 typedal-3.0.0b3/htmlcov/d_0ccc93afd6526b6c_for_py4web_py.html
--rw-r--r--   0        0        0    22550 2020-02-02 00:00:00.000000 typedal-3.0.0b3/htmlcov/d_0ccc93afd6526b6c_for_web2py_py.html
--rw-r--r--   0        0        0    69134 2020-02-02 00:00:00.000000 typedal-3.0.0b3/htmlcov/d_0ccc93afd6526b6c_helpers_py.html
--rw-r--r--   0        0        0    42239 2020-02-02 00:00:00.000000 typedal-3.0.0b3/htmlcov/d_0ccc93afd6526b6c_types_py.html
--rw-r--r--   0        0        0    17336 2020-02-02 00:00:00.000000 typedal-3.0.0b3/htmlcov/d_0ccc93afd6526b6c_web2py_py4web_shared_py.html
--rw-r--r--   0        0        0    25828 2020-02-02 00:00:00.000000 typedal-3.0.0b3/htmlcov/d_18c616467159315a_as_json_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 typedal-3.0.0b3/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     7664 2020-02-02 00:00:00.000000 typedal-3.0.0b3/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 typedal-3.0.0b3/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 typedal-3.0.0b3/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 typedal-3.0.0b3/htmlcov/status.json
--rw-r--r--   0        0        0    12406 2020-02-02 00:00:00.000000 typedal-3.0.0b3/htmlcov/style.css
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 typedal-3.0.0b3/src/typedal/__about__.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 typedal-3.0.0b3/src/typedal/__init__.py
--rw-r--r--   0        0        0    11818 2020-02-02 00:00:00.000000 typedal-3.0.0b3/src/typedal/caching.py
--rw-r--r--   0        0        0    18427 2020-02-02 00:00:00.000000 typedal-3.0.0b3/src/typedal/cli.py
--rw-r--r--   0        0        0    11626 2020-02-02 00:00:00.000000 typedal-3.0.0b3/src/typedal/config.py
--rw-r--r--   0        0        0    95038 2020-02-02 00:00:00.000000 typedal-3.0.0b3/src/typedal/core.py
--rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 typedal-3.0.0b3/src/typedal/fields.py
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 typedal-3.0.0b3/src/typedal/for_py4web.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 typedal-3.0.0b3/src/typedal/for_web2py.py
--rw-r--r--   0        0        0     6509 2020-02-02 00:00:00.000000 typedal-3.0.0b3/src/typedal/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typedal-3.0.0b3/src/typedal/py.typed
--rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 typedal-3.0.0b3/src/typedal/types.py
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 typedal-3.0.0b3/src/typedal/web2py_py4web_shared.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 typedal-3.0.0b3/src/typedal/serializers/as_json.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typedal-3.0.0b3/tests/__init__.py
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 typedal-3.0.0b3/tests/test_cli.py
--rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 typedal-3.0.0b3/tests/test_config.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 typedal-3.0.0b3/tests/test_docs_examples.py
--rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 typedal-3.0.0b3/tests/test_helpers.py
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 typedal-3.0.0b3/tests/test_json.py
--rw-r--r--   0        0        0    13197 2020-02-02 00:00:00.000000 typedal-3.0.0b3/tests/test_main.py
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 typedal-3.0.0b3/tests/test_mypy.py
--rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 typedal-3.0.0b3/tests/test_orm.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 typedal-3.0.0b3/tests/test_py4web.py
--rw-r--r--   0        0        0    11355 2020-02-02 00:00:00.000000 typedal-3.0.0b3/tests/test_query_builder.py
--rw-r--r--   0        0        0    15716 2020-02-02 00:00:00.000000 typedal-3.0.0b3/tests/test_relationships.py
--rw-r--r--   0        0        0     7012 2020-02-02 00:00:00.000000 typedal-3.0.0b3/tests/test_row.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 typedal-3.0.0b3/tests/test_stats.py
--rw-r--r--   0        0        0     8365 2020-02-02 00:00:00.000000 typedal-3.0.0b3/tests/test_table.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 typedal-3.0.0b3/tests/test_web2py.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 typedal-3.0.0b3/tests/test_xx_others.py
--rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 typedal-3.0.0b3/tests/timings.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 typedal-3.0.0b3/tests/configs/simple.toml
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 typedal-3.0.0b3/tests/configs/valid.env
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 typedal-3.0.0b3/tests/configs/valid.toml
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 typedal-3.0.0b3/.gitignore
--rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 typedal-3.0.0b3/README.md
--rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 typedal-3.0.0b3/pyproject.toml
--rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 typedal-3.0.0b3/PKG-INFO
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.readthedocs.yml
+-rw-r--r--   0        0        0    18401 2020-02-02 00:00:00.000000 typedal-3.0.0b4/CHANGELOG.md
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 typedal-3.0.0b4/coverage.svg
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 typedal-3.0.0b4/example_new.py
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 typedal-3.0.0b4/example_old.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 typedal-3.0.0b4/mkdocs.yml
+-rwxr-xr-x   0        0        0      314 2020-02-02 00:00:00.000000 typedal-3.0.0b4/start_dummy_pg.sh
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.github/workflows/su6.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/@plugins_snapshot.json
+-rw-r--r--   0        0        0   177667 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/_ast.data.json
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/_ast.meta.json
+-rw-r--r--   0        0        0    52400 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/_codecs.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/_codecs.meta.json
+-rw-r--r--   0        0        0    18227 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/_collections_abc.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/_collections_abc.meta.json
+-rw-r--r--   0        0        0     2923 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/_ctypes.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/_ctypes.meta.json
+-rw-r--r--   0        0        0   170960 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/_decimal.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/_decimal.meta.json
+-rw-r--r--   0        0        0    23362 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/abc.data.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/abc.meta.json
+-rw-r--r--   0        0        0    60687 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/array.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/array.meta.json
+-rw-r--r--   0        0        0  1054992 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/builtins.data.json
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/builtins.meta.json
+-rw-r--r--   0        0        0   123328 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/codecs.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/codecs.meta.json
+-rw-r--r--   0        0        0   104160 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/contextlib.data.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/contextlib.meta.json
+-rw-r--r--   0        0        0    57612 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/dataclasses.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/dataclasses.meta.json
+-rw-r--r--   0        0        0   142044 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/datetime.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/datetime.meta.json
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/decimal.data.json
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/decimal.meta.json
+-rw-r--r--   0        0        0    61020 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/enum.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/enum.meta.json
+-rw-r--r--   0        0        0    22399 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/genericpath.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/genericpath.meta.json
+-rw-r--r--   0        0        0    85348 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/io.data.json
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/io.meta.json
+-rw-r--r--   0        0        0    28778 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/mmap.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/mmap.meta.json
+-rw-r--r--   0        0        0    78982 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/numbers.data.json
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/numbers.meta.json
+-rw-r--r--   0        0        0    88278 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/pathlib.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/pathlib.meta.json
+-rw-r--r--   0        0        0    45131 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/pickle.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/pickle.meta.json
+-rw-r--r--   0        0        0    75208 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/posixpath.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/posixpath.meta.json
+-rw-r--r--   0        0        0   167175 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/re.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/re.meta.json
+-rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/sre_compile.data.json
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/sre_compile.meta.json
+-rw-r--r--   0        0        0    28013 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/sre_constants.data.json
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/sre_constants.meta.json
+-rw-r--r--   0        0        0    49442 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/sre_parse.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/sre_parse.meta.json
+-rw-r--r--   0        0        0   168498 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/subprocess.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/subprocess.meta.json
+-rw-r--r--   0        0        0   146267 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/sys.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/sys.meta.json
+-rw-r--r--   0        0        0    43605 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/time.data.json
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/time.meta.json
+-rw-r--r--   0        0        0   228230 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/types.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/types.meta.json
+-rw-r--r--   0        0        0   416965 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/typing.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/typing.meta.json
+-rw-r--r--   0        0        0    73907 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/typing_extensions.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/typing_extensions.meta.json
+-rw-r--r--   0        0        0    89065 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   407999 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/collections/__init__.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/collections/abc.data.json
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/collections/abc.meta.json
+-rw-r--r--   0        0        0   128994 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/email/__init__.data.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/email/__init__.meta.json
+-rw-r--r--   0        0        0    12200 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/email/charset.data.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/email/charset.meta.json
+-rw-r--r--   0        0        0     7249 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25073 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/email/errors.data.json
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/email/errors.meta.json
+-rw-r--r--   0        0        0     9154 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/email/header.data.json
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/email/header.meta.json
+-rw-r--r--   0        0        0    79298 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/email/message.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/email/message.meta.json
+-rw-r--r--   0        0        0    30857 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/email/policy.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/email/policy.meta.json
+-rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70175 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/importlib/abc.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64626 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    90277 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    11935 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0   350178 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/os/__init__.data.json
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/os/__init__.meta.json
+-rw-r--r--   0        0        0     4908 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/os/path.data.json
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/os/path.meta.json
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/src/__init__.data.json
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/src/__init__.meta.json
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/src/typedal/__about__.data.json
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/src/typedal/__about__.meta.json
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/src/typedal/__init__.data.json
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/src/typedal/__init__.meta.json
+-rw-r--r--   0        0        0    33347 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/src/typedal/core.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/src/typedal/core.meta.json
+-rw-r--r--   0        0        0    29038 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/src/typedal/fields.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/src/typedal/fields.meta.json
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/src/typedal/pydal_objects.data.json
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.10/src/typedal/pydal_objects.meta.json
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0     8152 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/__future__.data.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/__future__.meta.json
+-rw-r--r--   0        0        0   180405 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    72680 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_bisect.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_bisect.meta.json
+-rw-r--r--   0        0        0    57020 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    24646 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0    11060 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_compression.data.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_compression.meta.json
+-rw-r--r--   0        0        0    21088 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_csv.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_csv.meta.json
+-rw-r--r--   0        0        0   127335 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0   185969 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_decimal.data.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_decimal.meta.json
+-rw-r--r--   0        0        0    23461 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_json.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_json.meta.json
+-rw-r--r--   0        0        0    20139 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_locale.data.json
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_locale.meta.json
+-rw-r--r--   0        0        0   163664 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_operator.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_operator.meta.json
+-rw-r--r--   0        0        0     6555 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_random.data.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_random.meta.json
+-rw-r--r--   0        0        0   141220 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_socket.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_socket.meta.json
+-rw-r--r--   0        0        0    20067 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_stat.data.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_stat.meta.json
+-rw-r--r--   0        0        0    25355 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_thread.data.json
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_thread.meta.json
+-rw-r--r--   0        0        0     8127 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_tracemalloc.data.json
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_tracemalloc.meta.json
+-rw-r--r--   0        0        0    17812 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_warnings.data.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_warnings.meta.json
+-rw-r--r--   0        0        0    43019 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_weakref.data.json
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_weakref.meta.json
+-rw-r--r--   0        0        0    64281 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_weakrefset.data.json
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_weakrefset.meta.json
+-rw-r--r--   0        0        0    28042 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0   211034 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/argparse.data.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/argparse.meta.json
+-rw-r--r--   0        0        0    81489 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0   154628 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/ast.data.json
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/ast.meta.json
+-rw-r--r--   0        0        0     9651 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/atexit.data.json
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/atexit.meta.json
+-rw-r--r--   0        0        0    15948 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/base64.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/base64.meta.json
+-rw-r--r--   0        0        0    53666 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/bdb.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/bdb.meta.json
+-rw-r--r--   0        0        0    11979 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/binascii.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/binascii.meta.json
+-rw-r--r--   0        0        0    13025 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/bisect.data.json
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/bisect.meta.json
+-rw-r--r--   0        0        0  1691043 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0    50828 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/bz2.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/bz2.meta.json
+-rw-r--r--   0        0        0    61196 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/calendar.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/calendar.meta.json
+-rw-r--r--   0        0        0    21019 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cmd.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cmd.meta.json
+-rw-r--r--   0        0        0   129633 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0     7712 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/colorsys.data.json
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/colorsys.meta.json
+-rw-r--r--   0        0        0   159139 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configparser.data.json
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configparser.meta.json
+-rw-r--r--   0        0        0   128222 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0    63702 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/contextvars.data.json
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/contextvars.meta.json
+-rw-r--r--   0        0        0     6338 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/copy.data.json
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/copy.meta.json
+-rw-r--r--   0        0        0    13348 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/copyreg.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/copyreg.meta.json
+-rw-r--r--   0        0        0    38114 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/csv.data.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/csv.meta.json
+-rw-r--r--   0        0        0    82220 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/dataclasses.data.json
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/dataclasses.meta.json
+-rw-r--r--   0        0        0   173432 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/datetime.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/datetime.meta.json
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/decimal.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/decimal.meta.json
+-rw-r--r--   0        0        0    74115 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/difflib.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/difflib.meta.json
+-rw-r--r--   0        0        0    67645 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/dis.data.json
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/dis.meta.json
+-rw-r--r--   0        0        0    77702 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/doctest.data.json
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/doctest.meta.json
+-rw-r--r--   0        0        0   114800 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0    23733 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/errno.data.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/errno.meta.json
+-rw-r--r--   0        0        0    27481 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/example_new.data.json
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/example_new.meta.json
+-rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/fnmatch.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/fnmatch.meta.json
+-rw-r--r--   0        0        0   117065 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/fractions.data.json
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/fractions.meta.json
+-rw-r--r--   0        0        0   187190 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/functools.data.json
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/functools.meta.json
+-rw-r--r--   0        0        0    16492 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/gc.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/gc.meta.json
+-rw-r--r--   0        0        0    30432 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/getpass.data.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/getpass.meta.json
+-rw-r--r--   0        0        0    58893 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/gettext.data.json
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/gettext.meta.json
+-rw-r--r--   0        0        0    11236 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/glob.data.json
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/glob.meta.json
+-rw-r--r--   0        0        0    55273 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/gzip.data.json
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/gzip.meta.json
+-rw-r--r--   0        0        0    32987 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/hashlib.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/hashlib.meta.json
+-rw-r--r--   0        0        0    20199 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/hmac.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/hmac.meta.json
+-rw-r--r--   0        0        0   393898 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/inspect.data.json
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/inspect.meta.json
+-rw-r--r--   0        0        0    96360 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0   169807 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/ipaddress.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/ipaddress.meta.json
+-rw-r--r--   0        0        0   521458 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/itertools.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/itertools.meta.json
+-rw-r--r--   0        0        0     8942 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/linecache.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/linecache.meta.json
+-rw-r--r--   0        0        0    21639 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/locale.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/locale.meta.json
+-rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/marshal.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/marshal.meta.json
+-rw-r--r--   0        0        0    62500 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/math.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/math.meta.json
+-rw-r--r--   0        0        0    16551 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/mimetypes.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/mimetypes.meta.json
+-rw-r--r--   0        0        0    32933 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/msvcrt.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/msvcrt.meta.json
+-rw-r--r--   0        0        0   151900 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/mypy_extensions.data.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/mypy_extensions.meta.json
+-rw-r--r--   0        0        0    84033 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/numbers.data.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/numbers.meta.json
+-rw-r--r--   0        0        0     6122 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/opcode.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/opcode.meta.json
+-rw-r--r--   0        0        0    55486 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/operator.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/operator.meta.json
+-rw-r--r--   0        0        0   102946 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    96201 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pdb.data.json
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pdb.meta.json
+-rw-r--r--   0        0        0    48959 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    31491 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pkgutil.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pkgutil.meta.json
+-rw-r--r--   0        0        0    37189 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/platform.data.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/platform.meta.json
+-rw-r--r--   0        0        0   124421 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0    12597 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pprint.data.json
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pprint.meta.json
+-rw-r--r--   0        0        0     7678 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pty.data.json
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pty.meta.json
+-rw-r--r--   0        0        0   111565 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pydoc.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pydoc.meta.json
+-rw-r--r--   0        0        0    37466 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/queue.data.json
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/queue.meta.json
+-rw-r--r--   0        0        0    43645 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/random.data.json
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/random.meta.json
+-rw-r--r--   0        0        0   243154 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0    17416 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/reprlib.data.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/reprlib.meta.json
+-rw-r--r--   0        0        0     6994 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/secrets.data.json
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/secrets.meta.json
+-rw-r--r--   0        0        0    22630 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/select.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/select.meta.json
+-rw-r--r--   0        0        0    66210 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/selectors.data.json
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/selectors.meta.json
+-rw-r--r--   0        0        0    17284 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/shlex.data.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/shlex.meta.json
+-rw-r--r--   0        0        0    90180 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/shutil.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/shutil.meta.json
+-rw-r--r--   0        0        0    51409 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/signal.data.json
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/signal.meta.json
+-rw-r--r--   0        0        0   126342 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/socket.data.json
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/socket.meta.json
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/src.data.json
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/src.meta.json
+-rw-r--r--   0        0        0    14457 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    28914 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    51841 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0   212877 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/ssl.data.json
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/ssl.meta.json
+-rw-r--r--   0        0        0     6530 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/stat.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/stat.meta.json
+-rw-r--r--   0        0        0    32136 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/string.data.json
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/string.meta.json
+-rw-r--r--   0        0        0    15829 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/struct.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/struct.meta.json
+-rw-r--r--   0        0        0   238269 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   155328 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0    16019 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/sysconfig.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/sysconfig.meta.json
+-rw-r--r--   0        0        0   145159 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tarfile.data.json
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tarfile.meta.json
+-rw-r--r--   0        0        0   216804 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tempfile.data.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tempfile.meta.json
+-rw-r--r--   0        0        0    50218 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/termios.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/termios.meta.json
+-rw-r--r--   0        0        0    20222 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/textwrap.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/textwrap.meta.json
+-rw-r--r--   0        0        0    70414 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/threading.data.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/threading.meta.json
+-rw-r--r--   0        0        0    45633 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/time.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/time.meta.json
+-rw-r--r--   0        0        0    14997 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/token.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/token.meta.json
+-rw-r--r--   0        0        0    52648 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tokenize.data.json
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tokenize.meta.json
+-rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomllib.data.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomllib.meta.json
+-rw-r--r--   0        0        0    68653 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/traceback.data.json
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/traceback.meta.json
+-rw-r--r--   0        0        0    48898 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tracemalloc.data.json
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tracemalloc.meta.json
+-rw-r--r--   0        0        0     5355 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tty.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tty.meta.json
+-rw-r--r--   0        0        0   306063 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   593708 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0   118925 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0    60291 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/unicodedata.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/unicodedata.meta.json
+-rw-r--r--   0        0        0    35665 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/uuid.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/uuid.meta.json
+-rw-r--r--   0        0        0    28607 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/warnings.data.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/warnings.meta.json
+-rw-r--r--   0        0        0   253459 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/weakref.data.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/weakref.meta.json
+-rw-r--r--   0        0        0    96907 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/zipfile.data.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/zipfile.meta.json
+-rw-r--r--   0        0        0    17771 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/zlib.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/zlib.meta.json
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/__init__.data.json
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/__init__.meta.json
+-rw-r--r--   0        0        0     6371 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_argcomplete.data.json
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_argcomplete.meta.json
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_version.data.json
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_version.meta.json
+-rw-r--r--   0        0        0    48646 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/cacheprovider.data.json
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/cacheprovider.meta.json
+-rw-r--r--   0        0        0   184495 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/capture.data.json
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/capture.meta.json
+-rw-r--r--   0        0        0    28325 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/compat.data.json
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/compat.meta.json
+-rw-r--r--   0        0        0    33667 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/debugging.data.json
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/debugging.meta.json
+-rw-r--r--   0        0        0     7912 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/deprecated.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/deprecated.meta.json
+-rw-r--r--   0        0        0    43717 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/doctest.data.json
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/doctest.meta.json
+-rw-r--r--   0        0        0   181399 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/fixtures.data.json
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/fixtures.meta.json
+-rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/freeze_support.data.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/freeze_support.meta.json
+-rw-r--r--   0        0        0    10089 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/helpconfig.data.json
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/helpconfig.meta.json
+-rw-r--r--   0        0        0    67739 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/hookspec.data.json
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/hookspec.meta.json
+-rw-r--r--   0        0        0    67338 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/legacypath.data.json
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/legacypath.meta.json
+-rw-r--r--   0        0        0    87227 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/logging.data.json
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/logging.meta.json
+-rw-r--r--   0        0        0    52638 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/main.data.json
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/main.meta.json
+-rw-r--r--   0        0        0    29094 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/monkeypatch.data.json
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/monkeypatch.meta.json
+-rw-r--r--   0        0        0    62209 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/nodes.data.json
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/nodes.meta.json
+-rw-r--r--   0        0        0    34335 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/outcomes.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/outcomes.meta.json
+-rw-r--r--   0        0        0    38506 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/pathlib.data.json
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/pathlib.meta.json
+-rw-r--r--   0        0        0   143660 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/pytester.data.json
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/pytester.meta.json
+-rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/pytester_assertions.data.json
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/pytester_assertions.meta.json
+-rw-r--r--   0        0        0   125125 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/python.data.json
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/python.meta.json
+-rw-r--r--   0        0        0    61369 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/python_api.data.json
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/python_api.meta.json
+-rw-r--r--   0        0        0    37939 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/recwarn.data.json
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/recwarn.meta.json
+-rw-r--r--   0        0        0    53903 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/reports.data.json
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/reports.meta.json
+-rw-r--r--   0        0        0    45874 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/runner.data.json
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/runner.meta.json
+-rw-r--r--   0        0        0    11808 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/scope.data.json
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/scope.meta.json
+-rw-r--r--   0        0        0    17100 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/stash.data.json
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/stash.meta.json
+-rw-r--r--   0        0        0   129351 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/terminal.data.json
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/terminal.meta.json
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/timing.data.json
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/timing.meta.json
+-rw-r--r--   0        0        0    26426 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/tmpdir.data.json
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/tmpdir.meta.json
+-rw-r--r--   0        0        0    34310 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/warning_types.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/warning_types.meta.json
+-rw-r--r--   0        0        0    14515 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/warnings.data.json
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/warnings.meta.json
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_code/__init__.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_code/__init__.meta.json
+-rw-r--r--   0        0        0   208544 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_code/code.data.json
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_code/code.meta.json
+-rw-r--r--   0        0        0    20396 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_code/source.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_code/source.meta.json
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_io/__init__.data.json
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_io/__init__.meta.json
+-rw-r--r--   0        0        0    13200 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_io/saferepr.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_io/saferepr.meta.json
+-rw-r--r--   0        0        0    16853 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_io/terminalwriter.data.json
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_io/terminalwriter.meta.json
+-rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_io/wcwidth.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_io/wcwidth.meta.json
+-rw-r--r--   0        0        0    13753 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/assertion/__init__.data.json
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/assertion/__init__.meta.json
+-rw-r--r--   0        0        0    64441 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/assertion/rewrite.data.json
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/assertion/rewrite.meta.json
+-rw-r--r--   0        0        0     6078 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/assertion/truncate.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/assertion/truncate.meta.json
+-rw-r--r--   0        0        0    23734 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/assertion/util.data.json
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/assertion/util.meta.json
+-rw-r--r--   0        0        0   107743 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/config/__init__.data.json
+-rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/config/__init__.meta.json
+-rw-r--r--   0        0        0    42346 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/config/argparsing.data.json
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/config/argparsing.meta.json
+-rw-r--r--   0        0        0     5077 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/config/compat.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/config/compat.meta.json
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/config/exceptions.data.json
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/config/exceptions.meta.json
+-rw-r--r--   0        0        0    10343 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/config/findpaths.data.json
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/config/findpaths.meta.json
+-rw-r--r--   0        0        0    27773 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/mark/__init__.data.json
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/mark/__init__.meta.json
+-rw-r--r--   0        0        0    34035 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/mark/expression.data.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/mark/expression.meta.json
+-rw-r--r--   0        0        0   133374 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/mark/structures.data.json
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_pytest/mark/structures.meta.json
+-rw-r--r--   0        0        0   112991 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_typeshed/xml.data.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/_typeshed/xml.meta.json
+-rw-r--r--   0        0        0    23372 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/async_timeout/__init__.data.json
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/async_timeout/__init__.meta.json
+-rw-r--r--   0        0        0    15027 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/__init__.data.json
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/__init__.meta.json
+-rw-r--r--   0        0        0   116469 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/base_events.data.json
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/base_events.meta.json
+-rw-r--r--   0        0        0    36018 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/coroutines.data.json
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/coroutines.meta.json
+-rw-r--r--   0        0        0   222121 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/events.data.json
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/events.meta.json
+-rw-r--r--   0        0        0    11879 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/exceptions.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/exceptions.meta.json
+-rw-r--r--   0        0        0    43204 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/futures.data.json
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/futures.meta.json
+-rw-r--r--   0        0        0    41996 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/locks.data.json
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/locks.meta.json
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/mixins.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/mixins.meta.json
+-rw-r--r--   0        0        0    18996 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/protocols.data.json
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/protocols.meta.json
+-rw-r--r--   0        0        0    28441 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/queues.data.json
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/queues.meta.json
+-rw-r--r--   0        0        0    11969 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/runners.data.json
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/runners.meta.json
+-rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/selector_events.data.json
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/selector_events.meta.json
+-rw-r--r--   0        0        0    39572 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/streams.data.json
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/streams.meta.json
+-rw-r--r--   0        0        0    25143 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/subprocess.data.json
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/subprocess.meta.json
+-rw-r--r--   0        0        0    10201 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/taskgroups.data.json
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/taskgroups.meta.json
+-rw-r--r--   0        0        0   210760 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/tasks.data.json
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/tasks.meta.json
+-rw-r--r--   0        0        0     6673 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/threads.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/threads.meta.json
+-rw-r--r--   0        0        0    10036 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/timeouts.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/timeouts.meta.json
+-rw-r--r--   0        0        0    30202 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/transports.data.json
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/transports.meta.json
+-rw-r--r--   0        0        0    62212 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/unix_events.data.json
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/asyncio/unix_events.meta.json
+-rw-r--r--   0        0        0    51606 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/__init__.data.json
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/__init__.meta.json
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/_width_table.data.json
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/_width_table.meta.json
+-rw-r--r--   0        0        0    34730 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/brackets.data.json
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/brackets.meta.json
+-rw-r--r--   0        0        0    34153 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/cache.data.json
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/cache.meta.json
+-rw-r--r--   0        0        0    24821 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/comments.data.json
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/comments.meta.json
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/const.data.json
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/const.meta.json
+-rw-r--r--   0        0        0    20396 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/files.data.json
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/files.meta.json
+-rw-r--r--   0        0        0    37122 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/handle_ipynb_magics.data.json
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/handle_ipynb_magics.meta.json
+-rw-r--r--   0        0        0    69328 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/linegen.data.json
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/linegen.meta.json
+-rw-r--r--   0        0        0    85067 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/lines.data.json
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/lines.meta.json
+-rw-r--r--   0        0        0    35409 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/mode.data.json
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/mode.meta.json
+-rw-r--r--   0        0        0    56411 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/nodes.data.json
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/nodes.meta.json
+-rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/numerics.data.json
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/numerics.meta.json
+-rw-r--r--   0        0        0    11971 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/output.data.json
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/output.meta.json
+-rw-r--r--   0        0        0    12323 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/parsing.data.json
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/parsing.meta.json
+-rw-r--r--   0        0        0    26344 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/ranges.data.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/ranges.meta.json
+-rw-r--r--   0        0        0    17026 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/report.data.json
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/report.meta.json
+-rw-r--r--   0        0        0    11815 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/rusty.data.json
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/rusty.meta.json
+-rw-r--r--   0        0        0    13426 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/strings.data.json
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/strings.meta.json
+-rw-r--r--   0        0        0    85345 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/trans.data.json
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/black/trans.meta.json
+-rw-r--r--   0        0        0     7752 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/click/__init__.data.json
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/click/__init__.meta.json
+-rw-r--r--   0        0        0    49747 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/click/_compat.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/click/_compat.meta.json
+-rw-r--r--   0        0        0    52435 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/click/_termui_impl.data.json
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/click/_termui_impl.meta.json
+-rw-r--r--   0        0        0   213135 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/click/core.data.json
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/click/core.meta.json
+-rw-r--r--   0        0        0    73391 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/click/decorators.data.json
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/click/decorators.meta.json
+-rw-r--r--   0        0        0    31405 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/click/exceptions.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/click/exceptions.meta.json
+-rw-r--r--   0        0        0    18490 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/click/formatting.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/click/formatting.meta.json
+-rw-r--r--   0        0        0     8330 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/click/globals.data.json
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/click/globals.meta.json
+-rw-r--r--   0        0        0    31096 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/click/parser.data.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/click/parser.meta.json
+-rw-r--r--   0        0        0    38460 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/click/shell_completion.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/click/shell_completion.meta.json
+-rw-r--r--   0        0        0    25411 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/click/termui.data.json
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/click/termui.meta.json
+-rw-r--r--   0        0        0    89634 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/click/types.data.json
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/click/types.meta.json
+-rw-r--r--   0        0        0    37412 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/click/utils.data.json
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/click/utils.meta.json
+-rw-r--r--   0        0        0   788818 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/concurrent/__init__.data.json
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/concurrent/__init__.meta.json
+-rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/concurrent/futures/__init__.data.json
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/concurrent/futures/__init__.meta.json
+-rw-r--r--   0        0        0    86898 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/concurrent/futures/_base.data.json
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/concurrent/futures/_base.meta.json
+-rw-r--r--   0        0        0    66256 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/concurrent/futures/process.data.json
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/concurrent/futures/process.meta.json
+-rw-r--r--   0        0        0    24284 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/concurrent/futures/thread.data.json
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/concurrent/futures/thread.meta.json
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configurablejson/__init__.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configurablejson/__init__.meta.json
+-rw-r--r--   0        0        0    19403 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configurablejson/_internals.data.json
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configurablejson/_internals.meta.json
+-rw-r--r--   0        0        0    17411 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configurablejson/encode.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configurablejson/encode.meta.json
+-rw-r--r--   0        0        0     4837 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/__init__.data.json
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/__init__.meta.json
+-rw-r--r--   0        0        0    13895 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/abs.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/abs.meta.json
+-rw-r--r--   0        0        0    10489 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/alias.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/alias.meta.json
+-rw-r--r--   0        0        0    15569 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/beautify.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/beautify.meta.json
+-rw-r--r--   0        0        0    34248 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/binary_config.data.json
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/binary_config.meta.json
+-rw-r--r--   0        0        0    48466 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/cls.data.json
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/cls.meta.json
+-rw-r--r--   0        0        0    37519 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/core.data.json
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/core.meta.json
+-rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/dump.data.json
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/dump.meta.json
+-rw-r--r--   0        0        0    47435 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/errors.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/errors.meta.json
+-rw-r--r--   0        0        0    16366 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/helpers.data.json
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/helpers.meta.json
+-rw-r--r--   0        0        0     5735 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/postpone.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/postpone.meta.json
+-rw-r--r--   0        0        0     6506 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/singleton.data.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/singleton.meta.json
+-rw-r--r--   0        0        0     7818 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/type_converters.data.json
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/type_converters.meta.json
+-rw-r--r--   0        0        0    10079 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/loaders/__init__.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/loaders/__init__.meta.json
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/loaders/_types.data.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/loaders/_types.meta.json
+-rw-r--r--   0        0        0    11833 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/loaders/loaders_shared.data.json
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/loaders/loaders_shared.meta.json
+-rw-r--r--   0        0        0    31947 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/loaders/register.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/loaders/register.meta.json
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/__about__.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/__about__.meta.json
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/__init__.data.json
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/__init__.meta.json
+-rw-r--r--   0        0        0    13119 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/exceptions.data.json
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/exceptions.meta.json
+-rw-r--r--   0        0        0    20535 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/utils.data.json
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/utils.meta.json
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/__init__.data.json
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/__init__.meta.json
+-rw-r--r--   0        0        0    48126 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/_oid.data.json
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/_oid.meta.json
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/__init__.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/__init__.meta.json
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/__init__.data.json
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/__init__.meta.json
+-rw-r--r--   0        0        0    14600 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/aead.data.json
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/aead.meta.json
+-rw-r--r--   0        0        0    91123 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/backend.data.json
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/backend.meta.json
+-rw-r--r--   0        0        0    13430 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/ciphers.data.json
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/ciphers.meta.json
+-rw-r--r--   0        0        0     9234 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/cmac.data.json
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/cmac.meta.json
+-rw-r--r--   0        0        0    30942 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/ec.data.json
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/ec.meta.json
+-rw-r--r--   0        0        0    35743 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/rsa.data.json
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/rsa.meta.json
+-rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/utils.data.json
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/utils.meta.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/__init__.data.json
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/__init__.meta.json
+-rw-r--r--   0        0        0     8138 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/__init__.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/__init__.meta.json
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/_openssl.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/_openssl.meta.json
+-rw-r--r--   0        0        0     6808 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/asn1.data.json
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/asn1.meta.json
+-rw-r--r--   0        0        0     6527 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/exceptions.data.json
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/exceptions.meta.json
+-rw-r--r--   0        0        0     5960 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/ocsp.data.json
+-rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/ocsp.meta.json
+-rw-r--r--   0        0        0    34855 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/x509.data.json
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/x509.meta.json
+-rw-r--r--   0        0        0    12942 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/__init__.data.json
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/__init__.meta.json
+-rw-r--r--   0        0        0    21687 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/aead.data.json
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/aead.meta.json
+-rw-r--r--   0        0        0     6737 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/cmac.data.json
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/cmac.meta.json
+-rw-r--r--   0        0        0    27431 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/dh.data.json
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/dh.meta.json
+-rw-r--r--   0        0        0    25255 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/dsa.data.json
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/dsa.meta.json
+-rw-r--r--   0        0        0    23775 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/ec.data.json
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/ec.meta.json
+-rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/ed25519.data.json
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/ed25519.meta.json
+-rw-r--r--   0        0        0     6177 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/ed448.data.json
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/ed448.meta.json
+-rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/hashes.data.json
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/hashes.meta.json
+-rw-r--r--   0        0        0     8319 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/hmac.data.json
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/hmac.meta.json
+-rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/kdf.data.json
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/kdf.meta.json
+-rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/keys.data.json
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/keys.meta.json
+-rw-r--r--   0        0        0     8574 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/poly1305.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/poly1305.meta.json
+-rw-r--r--   0        0        0    23980 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/rsa.data.json
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/rsa.meta.json
+-rw-r--r--   0        0        0     6221 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/x25519.data.json
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/x25519.meta.json
+-rw-r--r--   0        0        0     6133 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/x448.data.json
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/x448.meta.json
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/openssl/__init__.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/openssl/__init__.meta.json
+-rw-r--r--   0        0        0    21364 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/openssl/_conditional.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/openssl/_conditional.meta.json
+-rw-r--r--   0        0        0    15055 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/openssl/binding.data.json
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/openssl/binding.meta.json
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/__init__.data.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/__init__.meta.json
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/_asymmetric.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/_asymmetric.meta.json
+-rw-r--r--   0        0        0    10701 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/_cipheralgorithm.data.json
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/_cipheralgorithm.meta.json
+-rw-r--r--   0        0        0    34260 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/_serialization.data.json
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/_serialization.meta.json
+-rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/constant_time.data.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/constant_time.meta.json
+-rw-r--r--   0        0        0    58762 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/hashes.data.json
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/hashes.meta.json
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/__init__.data.json
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/__init__.meta.json
+-rw-r--r--   0        0        0    30857 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/dh.data.json
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/dh.meta.json
+-rw-r--r--   0        0        0    32764 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/dsa.data.json
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/dsa.meta.json
+-rw-r--r--   0        0        0    87270 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/ec.data.json
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/ec.meta.json
+-rw-r--r--   0        0        0    23234 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/ed25519.data.json
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/ed25519.meta.json
+-rw-r--r--   0        0        0    22916 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/ed448.data.json
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/ed448.meta.json
+-rw-r--r--   0        0        0    23642 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/padding.data.json
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/padding.meta.json
+-rw-r--r--   0        0        0    34585 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/rsa.data.json
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/rsa.meta.json
+-rw-r--r--   0        0        0     8764 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/types.data.json
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/types.meta.json
+-rw-r--r--   0        0        0     7346 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/utils.data.json
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/utils.meta.json
+-rw-r--r--   0        0        0    21642 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/x25519.data.json
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/x25519.meta.json
+-rw-r--r--   0        0        0    21336 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/x448.data.json
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/x448.meta.json
+-rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/__init__.data.json
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/__init__.meta.json
+-rw-r--r--   0        0        0    18107 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/aead.data.json
+-rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/aead.meta.json
+-rw-r--r--   0        0        0    55273 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/algorithms.data.json
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/algorithms.meta.json
+-rw-r--r--   0        0        0    51375 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/base.data.json
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/base.meta.json
+-rw-r--r--   0        0        0    60153 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/modes.data.json
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/modes.meta.json
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/serialization/__init__.data.json
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/serialization/__init__.meta.json
+-rw-r--r--   0        0        0     7038 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/serialization/base.data.json
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/serialization/base.meta.json
+-rw-r--r--   0        0        0    28300 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/serialization/pkcs12.data.json
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/serialization/pkcs12.meta.json
+-rw-r--r--   0        0        0   121932 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/serialization/ssh.data.json
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/serialization/ssh.meta.json
+-rw-r--r--   0        0        0    31282 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/__init__.data.json
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/__init__.meta.json
+-rw-r--r--   0        0        0   177864 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/base.data.json
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/base.meta.json
+-rw-r--r--   0        0        0    22913 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/certificate_transparency.data.json
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/certificate_transparency.meta.json
+-rw-r--r--   0        0        0   400114 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/extensions.data.json
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/extensions.meta.json
+-rw-r--r--   0        0        0    52975 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/general_name.data.json
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/general_name.meta.json
+-rw-r--r--   0        0        0    56606 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/name.data.json
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/name.meta.json
+-rw-r--r--   0        0        0    97342 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/ocsp.data.json
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/ocsp.meta.json
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/oid.data.json
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/oid.meta.json
+-rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/verification.data.json
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/verification.meta.json
+-rw-r--r--   0        0        0    66125 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0    63522 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/ctypes/wintypes.data.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/ctypes/wintypes.meta.json
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/distutils/__init__.data.json
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/distutils/__init__.meta.json
+-rw-r--r--   0        0        0    16325 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/distutils/util.data.json
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/distutils/util.meta.json
+-rw-r--r--   0        0        0     4515 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/dotenv/__init__.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/dotenv/__init__.meta.json
+-rw-r--r--   0        0        0    24352 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/dotenv/main.data.json
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/dotenv/main.meta.json
+-rw-r--r--   0        0        0    56881 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/dotenv/parser.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/dotenv/parser.meta.json
+-rw-r--r--   0        0        0    15883 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/dotenv/variables.data.json
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/dotenv/variables.meta.json
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/edwh_migrate/__init__.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/edwh_migrate/__init__.meta.json
+-rw-r--r--   0        0        0    53859 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/edwh_migrate/migrate.data.json
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/edwh_migrate/migrate.meta.json
+-rw-r--r--   0        0        0     7662 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    16390 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7417 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25129 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9350 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0   101117 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    33204 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0    26015 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/email/utils.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/email/utils.meta.json
+-rw-r--r--   0        0        0     9410 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/__init__.data.json
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/__init__.meta.json
+-rw-r--r--   0        0        0   101033 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/cmd.data.json
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/cmd.meta.json
+-rw-r--r--   0        0        0    22061 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/compat.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/compat.meta.json
+-rw-r--r--   0        0        0    72061 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/config.data.json
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/config.meta.json
+-rw-r--r--   0        0        0     8346 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/db.data.json
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/db.meta.json
+-rw-r--r--   0        0        0    43517 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/diff.data.json
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/diff.meta.json
+-rw-r--r--   0        0        0    31208 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/exc.data.json
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/exc.meta.json
+-rw-r--r--   0        0        0    86993 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/remote.data.json
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/remote.meta.json
+-rw-r--r--   0        0        0    14236 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/types.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/types.meta.json
+-rw-r--r--   0        0        0   120972 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/util.data.json
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/util.meta.json
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/index/__init__.data.json
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/index/__init__.meta.json
+-rw-r--r--   0        0        0    67883 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/index/base.data.json
+-rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/index/base.meta.json
+-rw-r--r--   0        0        0    19230 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/index/fun.data.json
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/index/fun.meta.json
+-rw-r--r--   0        0        0    54512 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/index/typ.data.json
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/index/typ.meta.json
+-rw-r--r--   0        0        0    16630 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/index/util.data.json
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/index/util.meta.json
+-rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/objects/__init__.data.json
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/objects/__init__.meta.json
+-rw-r--r--   0        0        0    28657 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/objects/base.data.json
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/objects/base.meta.json
+-rw-r--r--   0        0        0     6290 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/objects/blob.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/objects/blob.meta.json
+-rw-r--r--   0        0        0    44705 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/objects/commit.data.json
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/objects/commit.meta.json
+-rw-r--r--   0        0        0    13968 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/objects/fun.data.json
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/objects/fun.meta.json
+-rw-r--r--   0        0        0     9015 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/objects/tag.data.json
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/objects/tag.meta.json
+-rw-r--r--   0        0        0    38948 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/objects/tree.data.json
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/objects/tree.meta.json
+-rw-r--r--   0        0        0   112403 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/objects/util.data.json
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/objects/util.meta.json
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/objects/submodule/__init__.data.json
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/objects/submodule/__init__.meta.json
+-rw-r--r--   0        0        0    66249 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/objects/submodule/base.data.json
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/objects/submodule/base.meta.json
+-rw-r--r--   0        0        0    13416 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/objects/submodule/root.data.json
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/objects/submodule/root.meta.json
+-rw-r--r--   0        0        0    12184 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/objects/submodule/util.data.json
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/objects/submodule/util.meta.json
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/refs/__init__.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/refs/__init__.meta.json
+-rw-r--r--   0        0        0    18213 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/refs/head.data.json
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/refs/head.meta.json
+-rw-r--r--   0        0        0    40948 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/refs/log.data.json
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/refs/log.meta.json
+-rw-r--r--   0        0        0    18936 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/refs/reference.data.json
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/refs/reference.meta.json
+-rw-r--r--   0        0        0    10509 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/refs/remote.data.json
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/refs/remote.meta.json
+-rw-r--r--   0        0        0    64655 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/refs/symbolic.data.json
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/refs/symbolic.meta.json
+-rw-r--r--   0        0        0    13266 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/refs/tag.data.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/refs/tag.meta.json
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/repo/__init__.data.json
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/repo/__init__.meta.json
+-rw-r--r--   0        0        0   108932 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/repo/base.data.json
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/repo/base.meta.json
+-rw-r--r--   0        0        0    12722 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/repo/fun.data.json
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/git/repo/fun.meta.json
+-rw-r--r--   0        0        0     4779 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/html/__init__.data.json
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/html/__init__.meta.json
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/html/entities.data.json
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/html/entities.meta.json
+-rw-r--r--   0        0        0    24033 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/http/__init__.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/http/__init__.meta.json
+-rw-r--r--   0        0        0    74759 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/http/client.data.json
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/http/client.meta.json
+-rw-r--r--   0        0        0    63694 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/http/cookiejar.data.json
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/http/cookiejar.meta.json
+-rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    61909 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    76878 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    22649 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/importlib/readers.data.json
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/importlib/readers.meta.json
+-rw-r--r--   0        0        0    24411 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/importlib/util.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/importlib/util.meta.json
+-rw-r--r--   0        0        0   102879 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    18350 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    10734 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/importlib/resources/__init__.data.json
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/importlib/resources/__init__.meta.json
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/importlib/resources/abc.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/importlib/resources/abc.meta.json
+-rw-r--r--   0        0        0    67163 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/iniconfig/__init__.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/iniconfig/__init__.meta.json
+-rw-r--r--   0        0        0    24550 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/iniconfig/_parse.data.json
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/iniconfig/_parse.meta.json
+-rw-r--r--   0        0        0     4983 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/iniconfig/exceptions.data.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/iniconfig/exceptions.meta.json
+-rw-r--r--   0        0        0    15855 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/json/__init__.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/json/__init__.meta.json
+-rw-r--r--   0        0        0    15446 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/json/decoder.data.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/json/decoder.meta.json
+-rw-r--r--   0        0        0    11337 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/json/encoder.data.json
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/json/encoder.meta.json
+-rw-r--r--   0        0        0   161727 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/logging/__init__.data.json
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/logging/__init__.meta.json
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/__init__.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/__init__.meta.json
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/_compat.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/_compat.meta.json
+-rw-r--r--   0        0        0     5699 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/_punycode.data.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/_punycode.meta.json
+-rw-r--r--   0        0        0    35792 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/main.data.json
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/main.meta.json
+-rw-r--r--   0        0        0     8178 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/parser_block.data.json
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/parser_block.meta.json
+-rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/parser_core.data.json
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/parser_core.meta.json
+-rw-r--r--   0        0        0     9963 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/parser_inline.data.json
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/parser_inline.meta.json
+-rw-r--r--   0        0        0    21363 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/renderer.data.json
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/renderer.meta.json
+-rw-r--r--   0        0        0    38344 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/ruler.data.json
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/ruler.meta.json
+-rw-r--r--   0        0        0    29705 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/token.data.json
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/token.meta.json
+-rw-r--r--   0        0        0    39948 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/utils.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/utils.meta.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/common/__init__.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/common/__init__.meta.json
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/common/entities.data.json
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/common/entities.meta.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json
+-rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/common/html_re.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/common/html_re.meta.json
+-rw-r--r--   0        0        0     6147 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json
+-rw-r--r--   0        0        0    18415 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/common/utils.data.json
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/common/utils.meta.json
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json
+-rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json
+-rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json
+-rw-r--r--   0        0        0     4996 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/presets/__init__.data.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/presets/default.data.json
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/presets/default.meta.json
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/presets/zero.data.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/presets/zero.meta.json
+-rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/code.data.json
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json
+-rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json
+-rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json
+-rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/list.data.json
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json
+-rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json
+-rw-r--r--   0        0        0    18155 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json
+-rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/table.data.json
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json
+-rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/block.data.json
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json
+-rw-r--r--   0        0        0     6399 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json
+-rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json
+-rw-r--r--   0        0        0     8420 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json
+-rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json
+-rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/text_join.data.json
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/text_join.meta.json
+-rw-r--r--   0        0        0     4052 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json
+-rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json
+-rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json
+-rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/fragments_join.data.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/fragments_join.meta.json
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json
+-rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/linkify.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/linkify.meta.json
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json
+-rw-r--r--   0        0        0    41273 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json
+-rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/mdurl/__init__.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/mdurl/__init__.meta.json
+-rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/mdurl/_decode.data.json
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/mdurl/_decode.meta.json
+-rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/mdurl/_encode.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/mdurl/_encode.meta.json
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/mdurl/_format.data.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/mdurl/_format.meta.json
+-rw-r--r--   0        0        0    13015 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/mdurl/_parse.data.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/mdurl/_parse.meta.json
+-rw-r--r--   0        0        0    28308 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/mdurl/_url.data.json
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/mdurl/_url.meta.json
+-rw-r--r--   0        0        0    34141 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/__init__.data.json
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/__init__.meta.json
+-rw-r--r--   0        0        0    33167 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/connection.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/connection.meta.json
+-rw-r--r--   0        0        0   122489 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/context.data.json
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/context.meta.json
+-rw-r--r--   0        0        0   218030 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/managers.data.json
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/managers.meta.json
+-rw-r--r--   0        0        0    62426 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/pool.data.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/pool.meta.json
+-rw-r--r--   0        0        0     9487 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/popen_fork.data.json
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json
+-rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json
+-rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json
+-rw-r--r--   0        0        0    18525 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/process.data.json
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/process.meta.json
+-rw-r--r--   0        0        0    28704 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/queues.data.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/queues.meta.json
+-rw-r--r--   0        0        0    30366 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/reduction.data.json
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/reduction.meta.json
+-rw-r--r--   0        0        0    36116 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/shared_memory.data.json
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json
+-rw-r--r--   0        0        0    98077 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json
+-rw-r--r--   0        0        0    10102 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/spawn.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/spawn.meta.json
+-rw-r--r--   0        0        0    28435 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/synchronize.data.json
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/synchronize.meta.json
+-rw-r--r--   0        0        0    24570 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/util.data.json
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/util.meta.json
+-rw-r--r--   0        0        0   397801 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     4908 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/packaging/__init__.data.json
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/packaging/__init__.meta.json
+-rw-r--r--   0        0        0    15520 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/packaging/_elffile.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/packaging/_elffile.meta.json
+-rw-r--r--   0        0        0    29325 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/packaging/_manylinux.data.json
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/packaging/_manylinux.meta.json
+-rw-r--r--   0        0        0    20376 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/packaging/_musllinux.data.json
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/packaging/_musllinux.meta.json
+-rw-r--r--   0        0        0    48580 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/packaging/_parser.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/packaging/_parser.meta.json
+-rw-r--r--   0        0        0    14958 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/packaging/_structures.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/packaging/_structures.meta.json
+-rw-r--r--   0        0        0    20540 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/packaging/_tokenizer.data.json
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/packaging/_tokenizer.meta.json
+-rw-r--r--   0        0        0    19513 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/packaging/markers.data.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/packaging/markers.meta.json
+-rw-r--r--   0        0        0    10512 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/packaging/requirements.data.json
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/packaging/requirements.meta.json
+-rw-r--r--   0        0        0    60559 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/packaging/specifiers.data.json
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/packaging/specifiers.meta.json
+-rw-r--r--   0        0        0    29671 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/packaging/tags.data.json
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/packaging/tags.meta.json
+-rw-r--r--   0        0        0    13225 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/packaging/utils.data.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/packaging/utils.meta.json
+-rw-r--r--   0        0        0    80955 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/packaging/version.data.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/packaging/version.meta.json
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pathspec/__init__.data.json
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pathspec/__init__.meta.json
+-rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pathspec/_meta.data.json
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pathspec/_meta.meta.json
+-rw-r--r--   0        0        0    29494 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pathspec/gitignore.data.json
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pathspec/gitignore.meta.json
+-rw-r--r--   0        0        0    29872 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pathspec/pathspec.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pathspec/pathspec.meta.json
+-rw-r--r--   0        0        0    19851 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pathspec/pattern.data.json
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pathspec/pattern.meta.json
+-rw-r--r--   0        0        0    55592 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pathspec/util.data.json
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pathspec/util.meta.json
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pathspec/patterns/__init__.data.json
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pathspec/patterns/__init__.meta.json
+-rw-r--r--   0        0        0    18510 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.meta.json
+-rw-r--r--   0        0        0    32503 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/platformdirs/__init__.data.json
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/platformdirs/__init__.meta.json
+-rw-r--r--   0        0        0    52590 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/platformdirs/api.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/platformdirs/api.meta.json
+-rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/platformdirs/version.data.json
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/platformdirs/version.meta.json
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pluggy/__init__.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pluggy/__init__.meta.json
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pluggy/_callers.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pluggy/_callers.meta.json
+-rw-r--r--   0        0        0   102996 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pluggy/_hooks.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pluggy/_hooks.meta.json
+-rw-r--r--   0        0        0    39554 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pluggy/_manager.data.json
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pluggy/_manager.meta.json
+-rw-r--r--   0        0        0    22344 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pluggy/_result.data.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pluggy/_result.meta.json
+-rw-r--r--   0        0        0    13570 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pluggy/_tracing.data.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pluggy/_tracing.meta.json
+-rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pluggy/_version.data.json
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pluggy/_version.meta.json
+-rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/__init__.data.json
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/__init__.meta.json
+-rw-r--r--   0        0        0    26890 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/auto_suggest.data.json
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/auto_suggest.meta.json
+-rw-r--r--   0        0        0   115432 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/buffer.data.json
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/buffer.meta.json
+-rw-r--r--   0        0        0    25920 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/cache.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/cache.meta.json
+-rw-r--r--   0        0        0    20835 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/cursor_shapes.data.json
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/cursor_shapes.meta.json
+-rw-r--r--   0        0        0    31349 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/data_structures.data.json
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/data_structures.meta.json
+-rw-r--r--   0        0        0    87520 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/document.data.json
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/document.meta.json
+-rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/enums.data.json
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/enums.meta.json
+-rw-r--r--   0        0        0    28526 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/history.data.json
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/history.meta.json
+-rw-r--r--   0        0        0    65848 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/keys.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/keys.meta.json
+-rw-r--r--   0        0        0    14425 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/mouse_events.data.json
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/mouse_events.meta.json
+-rw-r--r--   0        0        0    23629 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/patch_stdout.data.json
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/patch_stdout.meta.json
+-rw-r--r--   0        0        0    42743 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/renderer.data.json
+-rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/renderer.meta.json
+-rw-r--r--   0        0        0    13657 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/search.data.json
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/search.meta.json
+-rw-r--r--   0        0        0    10289 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/selection.data.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/selection.meta.json
+-rw-r--r--   0        0        0    35717 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/utils.data.json
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/utils.meta.json
+-rw-r--r--   0        0        0    30382 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/validation.data.json
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/validation.meta.json
+-rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/application/__init__.data.json
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/application/__init__.meta.json
+-rw-r--r--   0        0        0   116580 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/application/application.data.json
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/application/application.meta.json
+-rw-r--r--   0        0        0    17411 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/application/current.data.json
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/application/current.meta.json
+-rw-r--r--   0        0        0     9568 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/application/dummy.data.json
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/application/dummy.meta.json
+-rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/application/run_in_terminal.data.json
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/application/run_in_terminal.meta.json
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/clipboard/__init__.data.json
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/clipboard/__init__.meta.json
+-rw-r--r--   0        0        0    20695 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/clipboard/base.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/clipboard/base.meta.json
+-rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/clipboard/in_memory.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/clipboard/in_memory.meta.json
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/completion/__init__.data.json
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/completion/__init__.meta.json
+-rw-r--r--   0        0        0    49069 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/completion/base.data.json
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/completion/base.meta.json
+-rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/completion/deduplicate.data.json
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/completion/deduplicate.meta.json
+-rw-r--r--   0        0        0    10866 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/completion/filesystem.data.json
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/completion/filesystem.meta.json
+-rw-r--r--   0        0        0    34018 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/completion/fuzzy_completer.data.json
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/completion/fuzzy_completer.meta.json
+-rw-r--r--   0        0        0    10210 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/completion/nested.data.json
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/completion/nested.meta.json
+-rw-r--r--   0        0        0    10571 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/completion/word_completer.data.json
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/completion/word_completer.meta.json
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/eventloop/__init__.data.json
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/eventloop/__init__.meta.json
+-rw-r--r--   0        0        0    15354 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/eventloop/async_context_manager.data.json
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/eventloop/async_context_manager.meta.json
+-rw-r--r--   0        0        0    12774 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/eventloop/async_generator.data.json
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/eventloop/async_generator.meta.json
+-rw-r--r--   0        0        0    22342 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/eventloop/dummy_contextvars.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/eventloop/dummy_contextvars.meta.json
+-rw-r--r--   0        0        0    19676 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/eventloop/inputhook.data.json
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/eventloop/inputhook.meta.json
+-rw-r--r--   0        0        0     8541 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/eventloop/utils.data.json
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/eventloop/utils.meta.json
+-rw-r--r--   0        0        0     9943 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/filters/__init__.data.json
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/filters/__init__.meta.json
+-rw-r--r--   0        0        0    31137 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/filters/app.data.json
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/filters/app.meta.json
+-rw-r--r--   0        0        0    35307 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/filters/base.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/filters/base.meta.json
+-rw-r--r--   0        0        0    20205 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/filters/cli.data.json
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/filters/cli.meta.json
+-rw-r--r--   0        0        0     4798 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/filters/utils.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/filters/utils.meta.json
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/formatted_text/__init__.data.json
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/formatted_text/__init__.meta.json
+-rw-r--r--   0        0        0    17680 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/formatted_text/ansi.data.json
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/formatted_text/ansi.meta.json
+-rw-r--r--   0        0        0    16203 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/formatted_text/base.data.json
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/formatted_text/base.meta.json
+-rw-r--r--   0        0        0    10955 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/formatted_text/html.data.json
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/formatted_text/html.meta.json
+-rw-r--r--   0        0        0     6736 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/formatted_text/pygments.data.json
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/formatted_text/pygments.meta.json
+-rw-r--r--   0        0        0     6887 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/formatted_text/utils.data.json
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/formatted_text/utils.meta.json
+-rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/input/__init__.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/input/__init__.meta.json
+-rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/input/ansi_escape_sequences.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/input/ansi_escape_sequences.meta.json
+-rw-r--r--   0        0        0    31531 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/input/base.data.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/input/base.meta.json
+-rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/input/defaults.data.json
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/input/defaults.meta.json
+-rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/input/typeahead.data.json
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/input/typeahead.meta.json
+-rw-r--r--   0        0        0    18000 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/input/vt100_parser.data.json
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/input/vt100_parser.meta.json
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/__init__.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/__init__.meta.json
+-rw-r--r--   0        0        0     4744 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/defaults.data.json
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/defaults.meta.json
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/digraphs.data.json
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/digraphs.meta.json
+-rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/emacs_state.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/emacs_state.meta.json
+-rw-r--r--   0        0        0    65935 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/key_bindings.data.json
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/key_bindings.meta.json
+-rw-r--r--   0        0        0    41736 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/key_processor.data.json
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/key_processor.meta.json
+-rw-r--r--   0        0        0    18379 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/vi_state.data.json
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/vi_state.meta.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/__init__.data.json
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/__init__.meta.json
+-rw-r--r--   0        0        0     3880 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/auto_suggest.data.json
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/auto_suggest.meta.json
+-rw-r--r--   0        0        0     5505 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/basic.data.json
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/basic.meta.json
+-rw-r--r--   0        0        0     7918 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/completion.data.json
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/completion.meta.json
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/cpr.data.json
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/cpr.meta.json
+-rw-r--r--   0        0        0     8255 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/emacs.data.json
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/emacs.meta.json
+-rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/focus.data.json
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/focus.meta.json
+-rw-r--r--   0        0        0    12947 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/mouse.data.json
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/mouse.meta.json
+-rw-r--r--   0        0        0    77971 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/named_commands.data.json
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/named_commands.meta.json
+-rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/open_in_editor.data.json
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/open_in_editor.meta.json
+-rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/page_navigation.data.json
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/page_navigation.meta.json
+-rw-r--r--   0        0        0     8280 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/scroll.data.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/scroll.meta.json
+-rw-r--r--   0        0        0    32939 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/vi.data.json
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/vi.meta.json
+-rw-r--r--   0        0        0     6953 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/__init__.data.json
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/__init__.meta.json
+-rw-r--r--   0        0        0   191072 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/containers.data.json
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/containers.meta.json
+-rw-r--r--   0        0        0   103397 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/controls.data.json
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/controls.meta.json
+-rw-r--r--   0        0        0    15289 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/dimension.data.json
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/dimension.meta.json
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/dummy.data.json
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/dummy.meta.json
+-rw-r--r--   0        0        0    35473 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/layout.data.json
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/layout.meta.json
+-rw-r--r--   0        0        0    29041 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/margins.data.json
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/margins.meta.json
+-rw-r--r--   0        0        0    43226 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/menus.data.json
+-rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/menus.meta.json
+-rw-r--r--   0        0        0     6979 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/mouse_handlers.data.json
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/mouse_handlers.meta.json
+-rw-r--r--   0        0        0    85872 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/processors.data.json
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/processors.meta.json
+-rw-r--r--   0        0        0    27012 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/screen.data.json
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/screen.meta.json
+-rw-r--r--   0        0        0    25956 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/scrollable_pane.data.json
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/scrollable_pane.meta.json
+-rw-r--r--   0        0        0    45237 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/utils.data.json
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/utils.meta.json
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/lexers/__init__.data.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/lexers/__init__.meta.json
+-rw-r--r--   0        0        0    14816 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/lexers/base.data.json
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/lexers/base.meta.json
+-rw-r--r--   0        0        0    25563 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/lexers/pygments.data.json
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/lexers/pygments.meta.json
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/output/__init__.data.json
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/output/__init__.meta.json
+-rw-r--r--   0        0        0    78123 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/output/base.data.json
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/output/base.meta.json
+-rw-r--r--   0        0        0    10015 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/output/color_depth.data.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/output/color_depth.meta.json
+-rw-r--r--   0        0        0     4215 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/output/defaults.data.json
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/output/defaults.meta.json
+-rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/output/flush_stdout.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/output/flush_stdout.meta.json
+-rw-r--r--   0        0        0    31685 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/output/plain_text.data.json
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/output/plain_text.meta.json
+-rw-r--r--   0        0        0    56262 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/output/vt100.data.json
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/output/vt100.meta.json
+-rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/shortcuts/__init__.data.json
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/shortcuts/__init__.meta.json
+-rw-r--r--   0        0        0    22835 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/shortcuts/dialogs.data.json
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/shortcuts/dialogs.meta.json
+-rw-r--r--   0        0        0   114712 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/shortcuts/prompt.data.json
+-rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/shortcuts/prompt.meta.json
+-rw-r--r--   0        0        0    11079 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/shortcuts/utils.data.json
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/shortcuts/utils.meta.json
+-rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/shortcuts/progress_bar/__init__.data.json
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/shortcuts/progress_bar/__init__.meta.json
+-rw-r--r--   0        0        0    57362 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/shortcuts/progress_bar/base.data.json
+-rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/shortcuts/progress_bar/base.meta.json
+-rw-r--r--   0        0        0    53097 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/shortcuts/progress_bar/formatters.data.json
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/shortcuts/progress_bar/formatters.meta.json
+-rw-r--r--   0        0        0     5348 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/styles/__init__.data.json
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/styles/__init__.meta.json
+-rw-r--r--   0        0        0    52925 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/styles/base.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/styles/base.meta.json
+-rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/styles/defaults.data.json
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/styles/defaults.meta.json
+-rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/styles/named_colors.data.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/styles/named_colors.meta.json
+-rw-r--r--   0        0        0     5665 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/styles/pygments.data.json
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/styles/pygments.meta.json
+-rw-r--r--   0        0        0    28725 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/styles/style.data.json
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/styles/style.meta.json
+-rw-r--r--   0        0        0    45971 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/styles/style_transformation.data.json
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/styles/style_transformation.meta.json
+-rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/widgets/__init__.data.json
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/widgets/__init__.meta.json
+-rw-r--r--   0        0        0    97873 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/widgets/base.data.json
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/widgets/base.meta.json
+-rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/widgets/dialogs.data.json
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/widgets/dialogs.meta.json
+-rw-r--r--   0        0        0    20613 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/widgets/menus.data.json
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/widgets/menus.meta.json
+-rw-r--r--   0        0        0    31768 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/widgets/toolbars.data.json
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/widgets/toolbars.meta.json
+-rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pydal2sql/__init__.data.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pydal2sql/__init__.meta.json
+-rw-r--r--   0        0        0    41445 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pydal2sql/typer_support.data.json
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pydal2sql/typer_support.meta.json
+-rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pydal2sql/types.data.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pydal2sql/types.meta.json
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pydal2sql_core/__init__.data.json
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pydal2sql_core/__init__.meta.json
+-rw-r--r--   0        0        0    33442 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pydal2sql_core/cli_support.data.json
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pydal2sql_core/cli_support.meta.json
+-rw-r--r--   0        0        0    11990 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pydal2sql_core/core.data.json
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pydal2sql_core/core.meta.json
+-rw-r--r--   0        0        0    14843 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pydal2sql_core/helpers.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pydal2sql_core/helpers.meta.json
+-rw-r--r--   0        0        0    17244 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pydal2sql_core/types.data.json
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pydal2sql_core/types.meta.json
+-rw-r--r--   0        0        0    37406 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pyexpat/__init__.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pyexpat/__init__.meta.json
+-rw-r--r--   0        0        0    11760 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pyexpat/errors.data.json
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pyexpat/errors.meta.json
+-rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pyexpat/model.data.json
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pyexpat/model.meta.json
+-rw-r--r--   0        0        0    11300 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pytest/__init__.data.json
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/pytest/__init__.meta.json
+-rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/__init__.data.json
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/__init__.meta.json
+-rw-r--r--   0        0        0     4346 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/constants.data.json
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/constants.meta.json
+-rw-r--r--   0        0        0    23428 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/form.data.json
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/form.meta.json
+-rw-r--r--   0        0        0     8188 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompt.data.json
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompt.meta.json
+-rw-r--r--   0        0        0     9442 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/question.data.json
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/question.meta.json
+-rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/styles.data.json
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/styles.meta.json
+-rw-r--r--   0        0        0    10514 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/utils.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/utils.meta.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/version.data.json
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/version.meta.json
+-rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/__init__.data.json
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/__init__.meta.json
+-rw-r--r--   0        0        0    14644 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/autocomplete.data.json
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/autocomplete.meta.json
+-rw-r--r--   0        0        0     7096 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/checkbox.data.json
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/checkbox.meta.json
+-rw-r--r--   0        0        0    34906 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/common.data.json
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/common.meta.json
+-rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/confirm.data.json
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/confirm.meta.json
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/password.data.json
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/password.meta.json
+-rw-r--r--   0        0        0    10875 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/path.data.json
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/path.meta.json
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/press_any_key_to_continue.data.json
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/press_any_key_to_continue.meta.json
+-rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/rawselect.data.json
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/rawselect.meta.json
+-rw-r--r--   0        0        0     5962 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/select.data.json
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/select.meta.json
+-rw-r--r--   0        0        0     4730 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/text.data.json
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/text.meta.json
+-rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/__init__.data.json
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/__init__.meta.json
+-rw-r--r--   0        0        0    16999 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/backoff.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/backoff.meta.json
+-rw-r--r--   0        0        0    85848 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/client.data.json
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/client.meta.json
+-rw-r--r--   0        0        0    93397 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/cluster.data.json
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/cluster.meta.json
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/compat.data.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/compat.meta.json
+-rw-r--r--   0        0        0    66520 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/connection.data.json
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/connection.meta.json
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/crc.data.json
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/crc.meta.json
+-rw-r--r--   0        0        0     6763 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/credentials.data.json
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/credentials.meta.json
+-rw-r--r--   0        0        0    38204 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/exceptions.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/exceptions.meta.json
+-rw-r--r--   0        0        0    17826 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/lock.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/lock.meta.json
+-rw-r--r--   0        0        0    10756 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/ocsp.data.json
+-rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/ocsp.meta.json
+-rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/retry.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/retry.meta.json
+-rw-r--r--   0        0        0    25650 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/sentinel.data.json
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/sentinel.meta.json
+-rw-r--r--   0        0        0    14572 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/typing.data.json
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/typing.meta.json
+-rw-r--r--   0        0        0     8733 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/utils.data.json
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/utils.meta.json
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/__init__.data.json
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/__init__.meta.json
+-rw-r--r--   0        0        0    25974 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/base.data.json
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/base.meta.json
+-rw-r--r--   0        0        0    13625 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/commands.data.json
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/commands.meta.json
+-rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/encoders.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/encoders.meta.json
+-rw-r--r--   0        0        0    19890 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/helpers.data.json
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/helpers.meta.json
+-rw-r--r--   0        0        0    16424 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/hiredis.data.json
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/hiredis.meta.json
+-rw-r--r--   0        0        0     7715 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/resp2.data.json
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/resp2.meta.json
+-rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/resp3.data.json
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/resp3.meta.json
+-rw-r--r--   0        0        0    13926 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/socket.data.json
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/socket.meta.json
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/asyncio/__init__.data.json
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/asyncio/__init__.meta.json
+-rw-r--r--   0        0        0   110856 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/asyncio/client.data.json
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/asyncio/client.meta.json
+-rw-r--r--   0        0        0   103724 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/asyncio/cluster.data.json
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/asyncio/cluster.meta.json
+-rw-r--r--   0        0        0    95161 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/asyncio/connection.data.json
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/asyncio/connection.meta.json
+-rw-r--r--   0        0        0    18737 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/asyncio/lock.data.json
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/asyncio/lock.meta.json
+-rw-r--r--   0        0        0     9741 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/asyncio/retry.data.json
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/asyncio/retry.meta.json
+-rw-r--r--   0        0        0    28762 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/asyncio/sentinel.data.json
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/asyncio/sentinel.meta.json
+-rw-r--r--   0        0        0     5149 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/asyncio/utils.data.json
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/asyncio/utils.meta.json
+-rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/__init__.data.json
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/__init__.meta.json
+-rw-r--r--   0        0        0    93587 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/cluster.data.json
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/cluster.meta.json
+-rw-r--r--   0        0        0   401564 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/core.data.json
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/core.meta.json
+-rw-r--r--   0        0        0     6004 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/helpers.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/helpers.meta.json
+-rw-r--r--   0        0        0     6977 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/redismodules.data.json
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/redismodules.meta.json
+-rw-r--r--   0        0        0     8799 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/sentinel.data.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/sentinel.meta.json
+-rw-r--r--   0        0        0    36127 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/bf/__init__.data.json
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/bf/__init__.meta.json
+-rw-r--r--   0        0        0    35430 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/bf/commands.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/bf/commands.meta.json
+-rw-r--r--   0        0        0    20186 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/bf/info.data.json
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/bf/info.meta.json
+-rw-r--r--   0        0        0    16330 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/graph/__init__.data.json
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/graph/__init__.meta.json
+-rw-r--r--   0        0        0    12253 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/graph/commands.data.json
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/graph/commands.meta.json
+-rw-r--r--   0        0        0     5581 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/graph/edge.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/graph/edge.meta.json
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/graph/exceptions.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/graph/exceptions.meta.json
+-rw-r--r--   0        0        0    12629 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/graph/execution_plan.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/graph/execution_plan.meta.json
+-rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/graph/node.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/graph/node.meta.json
+-rw-r--r--   0        0        0     8795 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/graph/path.data.json
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/graph/path.meta.json
+-rw-r--r--   0        0        0    43138 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/graph/query_result.data.json
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/graph/query_result.meta.json
+-rw-r--r--   0        0        0    11069 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/json/__init__.data.json
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/json/__init__.meta.json
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/json/_util.data.json
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/json/_util.meta.json
+-rw-r--r--   0        0        0    31474 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/json/commands.data.json
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/json/commands.meta.json
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/json/decoders.data.json
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/json/decoders.meta.json
+-rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/json/path.data.json
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/json/path.meta.json
+-rw-r--r--   0        0        0    19740 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/search/__init__.data.json
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/search/__init__.meta.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/search/_util.data.json
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/search/_util.meta.json
+-rw-r--r--   0        0        0    34189 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/search/aggregation.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/search/aggregation.meta.json
+-rw-r--r--   0        0        0    55636 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/search/commands.data.json
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/search/commands.meta.json
+-rw-r--r--   0        0        0     3840 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/search/document.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/search/document.meta.json
+-rw-r--r--   0        0        0    38931 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/search/query.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/search/query.meta.json
+-rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/search/result.data.json
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/search/result.meta.json
+-rw-r--r--   0        0        0     8818 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/search/suggestion.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/search/suggestion.meta.json
+-rw-r--r--   0        0        0    12615 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/timeseries/__init__.data.json
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/timeseries/__init__.meta.json
+-rw-r--r--   0        0        0    68529 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/timeseries/commands.data.json
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/timeseries/commands.meta.json
+-rw-r--r--   0        0        0     8125 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/timeseries/info.data.json
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/timeseries/info.meta.json
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/timeseries/utils.data.json
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/timeseries/utils.meta.json
+-rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/__init__.data.json
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/__init__.meta.json
+-rw-r--r--   0        0        0     8768 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/__main__.data.json
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/__main__.meta.json
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_cell_widths.data.json
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_cell_widths.meta.json
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_emoji_codes.data.json
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_emoji_codes.meta.json
+-rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_emoji_replace.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_emoji_replace.meta.json
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_export_format.data.json
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_export_format.meta.json
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_extension.data.json
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_extension.meta.json
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_fileno.data.json
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_fileno.meta.json
+-rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_log_render.data.json
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_log_render.meta.json
+-rw-r--r--   0        0        0     6839 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_loop.data.json
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_loop.meta.json
+-rw-r--r--   0        0        0    16444 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_null_file.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_null_file.meta.json
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_palettes.data.json
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_palettes.meta.json
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_pick.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_pick.meta.json
+-rw-r--r--   0        0        0    12590 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_ratio.data.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_ratio.meta.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_spinners.data.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_spinners.meta.json
+-rw-r--r--   0        0        0     7101 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_stack.data.json
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_stack.meta.json
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_timer.data.json
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_timer.meta.json
+-rw-r--r--   0        0        0    53433 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_win32_console.data.json
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_win32_console.meta.json
+-rw-r--r--   0        0        0     8940 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_windows.data.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_windows.meta.json
+-rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_windows_renderer.data.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_windows_renderer.meta.json
+-rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_wrap.data.json
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/_wrap.meta.json
+-rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/abc.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/abc.meta.json
+-rw-r--r--   0        0        0    24347 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/align.data.json
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/align.meta.json
+-rw-r--r--   0        0        0    26848 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/ansi.data.json
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/ansi.meta.json
+-rw-r--r--   0        0        0    21129 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/box.data.json
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/box.meta.json
+-rw-r--r--   0        0        0     8887 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/cells.data.json
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/cells.meta.json
+-rw-r--r--   0        0        0    57697 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/color.data.json
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/color.meta.json
+-rw-r--r--   0        0        0    21972 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/color_triplet.data.json
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/color_triplet.meta.json
+-rw-r--r--   0        0        0    11427 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/columns.data.json
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/columns.meta.json
+-rw-r--r--   0        0        0   190779 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/console.data.json
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/console.meta.json
+-rw-r--r--   0        0        0     6421 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/constrain.data.json
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/constrain.meta.json
+-rw-r--r--   0        0        0    22261 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/containers.data.json
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/containers.meta.json
+-rw-r--r--   0        0        0    23326 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/control.data.json
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/control.meta.json
+-rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/default_styles.data.json
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/default_styles.meta.json
+-rw-r--r--   0        0        0    11746 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/emoji.data.json
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/emoji.meta.json
+-rw-r--r--   0        0        0    10354 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/errors.data.json
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/errors.meta.json
+-rw-r--r--   0        0        0     9209 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/file_proxy.data.json
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/file_proxy.meta.json
+-rw-r--r--   0        0        0    16680 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/highlighter.data.json
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/highlighter.meta.json
+-rw-r--r--   0        0        0    10622 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/json.data.json
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/json.meta.json
+-rw-r--r--   0        0        0    10805 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/jupyter.data.json
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/jupyter.meta.json
+-rw-r--r--   0        0        0    30064 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/live.data.json
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/live.meta.json
+-rw-r--r--   0        0        0     9936 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/live_render.data.json
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/live_render.meta.json
+-rw-r--r--   0        0        0    88816 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/markdown.data.json
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/markdown.meta.json
+-rw-r--r--   0        0        0    27404 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/markup.data.json
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/markup.meta.json
+-rw-r--r--   0        0        0    25218 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/measure.data.json
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/measure.meta.json
+-rw-r--r--   0        0        0    13374 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/padding.data.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/padding.meta.json
+-rw-r--r--   0        0        0     6681 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/pager.data.json
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/pager.meta.json
+-rw-r--r--   0        0        0    10046 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/palette.data.json
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/palette.meta.json
+-rw-r--r--   0        0        0    18539 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/panel.data.json
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/panel.meta.json
+-rw-r--r--   0        0        0   133658 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/pretty.data.json
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/pretty.meta.json
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/protocol.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/protocol.meta.json
+-rw-r--r--   0        0        0    16838 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/region.data.json
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/region.meta.json
+-rw-r--r--   0        0        0    29387 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/repr.data.json
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/repr.meta.json
+-rw-r--r--   0        0        0     9164 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/rule.data.json
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/rule.meta.json
+-rw-r--r--   0        0        0     4759 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/scope.data.json
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/scope.meta.json
+-rw-r--r--   0        0        0     6015 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/screen.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/screen.meta.json
+-rw-r--r--   0        0        0   100846 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/segment.data.json
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/segment.meta.json
+-rw-r--r--   0        0        0    11158 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/spinner.data.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/spinner.meta.json
+-rw-r--r--   0        0        0    13247 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/status.data.json
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/status.meta.json
+-rw-r--r--   0        0        0    58607 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/style.data.json
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/style.meta.json
+-rw-r--r--   0        0        0     6702 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/styled.data.json
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/styled.meta.json
+-rw-r--r--   0        0        0    81805 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/syntax.data.json
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/syntax.meta.json
+-rw-r--r--   0        0        0    86262 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/table.data.json
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/table.meta.json
+-rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/terminal_theme.data.json
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/terminal_theme.meta.json
+-rw-r--r--   0        0        0    92014 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/text.data.json
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/text.meta.json
+-rw-r--r--   0        0        0    15945 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/theme.data.json
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/theme.meta.json
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/themes.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/themes.meta.json
+-rw-r--r--   0        0        0    58612 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/traceback.data.json
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/rich/traceback.meta.json
+-rw-r--r--   0        0        0    22875 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/sqlite3/__init__.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/sqlite3/__init__.meta.json
+-rw-r--r--   0        0        0   185529 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/sqlite3/dbapi2.data.json
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/sqlite3/dbapi2.meta.json
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/src/__init__.data.json
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/src/__init__.meta.json
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/src/typedal/__about__.data.json
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/src/typedal/__about__.meta.json
+-rw-r--r--   0        0        0    13692 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/src/typedal/config.data.json
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/src/typedal/config.meta.json
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/su6/__about__.data.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/su6/__about__.meta.json
+-rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/su6/__init__.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/su6/__init__.meta.json
+-rw-r--r--   0        0        0    27733 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/su6/cli.data.json
+-rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/su6/cli.meta.json
+-rw-r--r--   0        0        0    67427 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/su6/core.data.json
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/su6/core.meta.json
+-rw-r--r--   0        0        0    63551 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/su6/plugins.data.json
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/su6/plugins.meta.json
+-rw-r--r--   0        0        0   155536 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/sys/__init__.data.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/sys/__init__.meta.json
+-rw-r--r--   0        0        0    93809 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tabulate/__init__.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tabulate/__init__.meta.json
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tabulate/version.data.json
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tabulate/version.meta.json
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tests/__init__.data.json
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tests/__init__.meta.json
+-rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomli/__init__.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomli/__init__.meta.json
+-rw-r--r--   0        0        0    55884 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomli/_parser.data.json
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomli/_parser.meta.json
+-rw-r--r--   0        0        0     7143 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomli/_re.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomli/_re.meta.json
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomli/_types.data.json
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomli/_types.meta.json
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomli_w/__init__.data.json
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomli_w/__init__.meta.json
+-rw-r--r--   0        0        0    34224 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomli_w/_writer.data.json
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomli_w/_writer.meta.json
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/__init__.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/__init__.meta.json
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/_compat.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/_compat.meta.json
+-rw-r--r--   0        0        0     9960 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/_types.data.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/_types.meta.json
+-rw-r--r--   0        0        0     8336 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/_utils.data.json
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/_utils.meta.json
+-rw-r--r--   0        0        0    24999 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/api.data.json
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/api.meta.json
+-rw-r--r--   0        0        0    50132 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/container.data.json
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/container.meta.json
+-rw-r--r--   0        0        0    38878 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/exceptions.data.json
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/exceptions.meta.json
+-rw-r--r--   0        0        0   287553 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/items.data.json
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/items.meta.json
+-rw-r--r--   0        0        0    36621 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/parser.data.json
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/parser.meta.json
+-rw-r--r--   0        0        0    24225 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/source.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/source.meta.json
+-rw-r--r--   0        0        0     8088 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/toml_char.data.json
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/toml_char.meta.json
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/toml_document.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/toml_document.meta.json
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typedal/__about__.data.json
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typedal/__about__.meta.json
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typedal/__init__.data.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typedal/__init__.meta.json
+-rw-r--r--   0        0        0    36289 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typedal/caching.data.json
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typedal/caching.meta.json
+-rw-r--r--   0        0        0    27838 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typedal/cli.data.json
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typedal/cli.meta.json
+-rw-r--r--   0        0        0    22466 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typedal/config.data.json
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typedal/config.meta.json
+-rw-r--r--   0        0        0   301190 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typedal/core.data.json
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typedal/core.meta.json
+-rw-r--r--   0        0        0    30719 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typedal/fields.data.json
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typedal/fields.meta.json
+-rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typedal/for_py4web.data.json
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typedal/for_py4web.meta.json
+-rw-r--r--   0        0        0    12836 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typedal/for_web2py.data.json
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typedal/for_web2py.meta.json
+-rw-r--r--   0        0        0    28464 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typedal/helpers.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typedal/helpers.meta.json
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typedal/serializers.data.json
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typedal/serializers.meta.json
+-rw-r--r--   0        0        0    24209 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typedal/types.data.json
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typedal/types.meta.json
+-rw-r--r--   0        0        0     9735 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typedal/web2py_py4web_shared.data.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typedal/web2py_py4web_shared.meta.json
+-rw-r--r--   0        0        0    10626 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typedal/serializers/as_json.data.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typedal/serializers/as_json.meta.json
+-rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typeguard/__init__.data.json
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typeguard/__init__.meta.json
+-rw-r--r--   0        0        0    40710 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_checkers.data.json
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_checkers.meta.json
+-rw-r--r--   0        0        0    15819 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_config.data.json
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_config.meta.json
+-rw-r--r--   0        0        0    35537 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_decorators.data.json
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_decorators.meta.json
+-rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_exceptions.data.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_exceptions.meta.json
+-rw-r--r--   0        0        0    23488 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_functions.data.json
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_functions.meta.json
+-rw-r--r--   0        0        0    23369 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_importhook.data.json
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_importhook.meta.json
+-rw-r--r--   0        0        0     5789 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_memo.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_memo.meta.json
+-rw-r--r--   0        0        0    21446 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_suppression.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_suppression.meta.json
+-rw-r--r--   0        0        0    85648 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_transformer.data.json
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_transformer.meta.json
+-rw-r--r--   0        0        0    11727 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_utils.data.json
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_utils.meta.json
+-rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typer/__init__.data.json
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typer/__init__.meta.json
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typer/_compat_utils.data.json
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typer/_compat_utils.meta.json
+-rw-r--r--   0        0        0    12325 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typer/_completion_shared.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typer/_completion_shared.meta.json
+-rw-r--r--   0        0        0    36460 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typer/_typing.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typer/_typing.meta.json
+-rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typer/colors.data.json
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typer/colors.meta.json
+-rw-r--r--   0        0        0     9694 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typer/completion.data.json
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typer/completion.meta.json
+-rw-r--r--   0        0        0    50878 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typer/core.data.json
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typer/core.meta.json
+-rw-r--r--   0        0        0    57396 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typer/main.data.json
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typer/main.meta.json
+-rw-r--r--   0        0        0    74258 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typer/models.data.json
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typer/models.meta.json
+-rw-r--r--   0        0        0    78838 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typer/params.data.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typer/params.meta.json
+-rw-r--r--   0        0        0    33649 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typer/rich_utils.data.json
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typer/rich_utils.meta.json
+-rw-r--r--   0        0        0    19703 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typer/utils.data.json
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/typer/utils.meta.json
+-rw-r--r--   0        0        0     6249 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/unittest/__init__.data.json
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/unittest/__init__.meta.json
+-rw-r--r--   0        0        0    27032 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/unittest/_log.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/unittest/_log.meta.json
+-rw-r--r--   0        0        0    11460 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/unittest/async_case.data.json
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/unittest/async_case.meta.json
+-rw-r--r--   0        0        0   286451 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/unittest/case.data.json
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/unittest/case.meta.json
+-rw-r--r--   0        0        0    15314 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/unittest/loader.data.json
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/unittest/loader.meta.json
+-rw-r--r--   0        0        0    12573 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/unittest/main.data.json
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/unittest/main.meta.json
+-rw-r--r--   0        0        0   193614 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/unittest/mock.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/unittest/mock.meta.json
+-rw-r--r--   0        0        0    22521 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/unittest/result.data.json
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/unittest/result.meta.json
+-rw-r--r--   0        0        0    13338 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/unittest/runner.data.json
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/unittest/runner.meta.json
+-rw-r--r--   0        0        0    17553 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/unittest/signals.data.json
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/unittest/signals.meta.json
+-rw-r--r--   0        0        0    12052 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/unittest/suite.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/unittest/suite.meta.json
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/urllib/__init__.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/urllib/__init__.meta.json
+-rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/urllib/error.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/urllib/error.meta.json
+-rw-r--r--   0        0        0   235720 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/urllib/parse.data.json
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/urllib/parse.meta.json
+-rw-r--r--   0        0        0   169451 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/urllib/request.data.json
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/urllib/request.meta.json
+-rw-r--r--   0        0        0    30659 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/urllib/response.data.json
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/urllib/response.meta.json
+-rw-r--r--   0        0        0    31341 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/witchery/__init__.data.json
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/witchery/__init__.meta.json
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/xml/__init__.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/xml/__init__.meta.json
+-rw-r--r--   0        0        0    30071 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/xml/dom/__init__.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/xml/dom/__init__.meta.json
+-rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/xml/dom/domreg.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/xml/dom/domreg.meta.json
+-rw-r--r--   0        0        0    67176 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/xml/dom/expatbuilder.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/xml/dom/expatbuilder.meta.json
+-rw-r--r--   0        0        0    15865 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/xml/dom/minicompat.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/xml/dom/minicompat.meta.json
+-rw-r--r--   0        0        0   173371 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/xml/dom/minidom.data.json
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/xml/dom/minidom.meta.json
+-rw-r--r--   0        0        0    36037 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/xml/dom/xmlbuilder.data.json
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/xml/dom/xmlbuilder.meta.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/xml/parsers/__init__.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/xml/parsers/__init__.meta.json
+-rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/xml/parsers/expat/__init__.data.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/xml/parsers/expat/__init__.meta.json
+-rw-r--r--   0        0        0    20645 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/xml/sax/__init__.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/xml/sax/__init__.meta.json
+-rw-r--r--   0        0        0    26771 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/xml/sax/handler.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/xml/sax/handler.meta.json
+-rw-r--r--   0        0        0    53739 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/xml/sax/xmlreader.data.json
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/xml/sax/xmlreader.meta.json
+-rw-r--r--   0        0        0   188224 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/__init__.data.json
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/__init__.meta.json
+-rw-r--r--   0        0        0    23798 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/_yaml.data.json
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/_yaml.meta.json
+-rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/composer.data.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/composer.meta.json
+-rw-r--r--   0        0        0    48721 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/constructor.data.json
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/constructor.meta.json
+-rw-r--r--   0        0        0    21570 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/cyaml.data.json
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/cyaml.meta.json
+-rw-r--r--   0        0        0    13642 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/dumper.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/dumper.meta.json
+-rw-r--r--   0        0        0    63025 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/emitter.data.json
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/emitter.meta.json
+-rw-r--r--   0        0        0     9518 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/error.data.json
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/error.meta.json
+-rw-r--r--   0        0        0    31137 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/events.data.json
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/events.meta.json
+-rw-r--r--   0        0        0    13347 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/loader.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/loader.meta.json
+-rw-r--r--   0        0        0    11844 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/nodes.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/nodes.meta.json
+-rw-r--r--   0        0        0    15083 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/parser.data.json
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/parser.meta.json
+-rw-r--r--   0        0        0    13189 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/reader.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/reader.meta.json
+-rw-r--r--   0        0        0    46065 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/representer.data.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/representer.meta.json
+-rw-r--r--   0        0        0    11331 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/resolver.data.json
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/resolver.meta.json
+-rw-r--r--   0        0        0    31183 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/scanner.data.json
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/scanner.meta.json
+-rw-r--r--   0        0        0    10682 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/serializer.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/serializer.meta.json
+-rw-r--r--   0        0        0    40449 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/tokens.data.json
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.mypy_cache/3.11/yaml/tokens.meta.json
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.pytest_cache/README.md
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     4398 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/0.1.14/15432600919105507093
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/0.1.14/7801493945118068108
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/0.1.6/2759713849472344579
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/0.1.7/14298551053547083375
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/0.1.7/3401287376304810316
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/1215429078721865123
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/121ed75fe9fe5f8e
+-rw-r--r--   0        0        0    23412 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/14855161046259211094
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/19309938546e93ab
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/197f3188bc94f91f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/1aa1390b5bde1004
+-rw-r--r--   0        0        0     8089 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/1b34455c399f0006
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/1bd1a229a4f4ee7f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/1c46d1f378d28fbb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/1ca71ee291d82018
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/1d6bb777df44b8ec
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/1dc8423cfb79eaa4
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/20585cf790eae81e
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/217892307344966949
+-rw-r--r--   0        0        0    12122 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/221af82ae72a7f27
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/2282e801459c52a4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/248c4e1a32c704cb
+-rw-r--r--   0        0        0    10858 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/24e1b4aab386ebc8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/28b1d8ac7e2aab6b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/2b7f7d266c8efaad
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/2bb6610cadf18e18
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/2dac345be8527adf
+-rw-r--r--   0        0        0    11525 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/2f3396c610fd7095
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/31731f8e74291475
+-rw-r--r--   0        0        0    13342 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/322af04e6d059ce5
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/3826106cf4494de8
+-rw-r--r--   0        0        0    11210 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/38d5fd55b14a9d6c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/3afc55a04b8f8bb2
+-rw-r--r--   0        0        0    12129 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/4022ee8774ccd98a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/42f9a2406e74c24f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/4696b157ff786f22
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/46a88ce266f1ad94
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/4a6edd5010cb9700
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/4d0230e9a81a468
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/52018ba3989fcaf7
+-rw-r--r--   0        0        0    13679 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/5491563776466765346
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/54e6ba8c25a22ffc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/566d94db91d23339
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/5a67aed8f6b70cd5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/5b076d769fa5cacd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/5ceb1580c62ee794
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/6bc90dbb56504f96
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/6c52d14716eee431
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/6f0c8f98e4da1d48
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/74e52af774eebdbd
+-rw-r--r--   0        0        0    11023 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/75bd1769f6e29ed7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/815ba2cfea236769
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/876d9a8d302e1c46
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/8891791100357482236
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/88e2927df9448936
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/8c4d3f5ef14b0167
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/8f8ec552e76f3eab
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/95c82d8566c6704c
+-rw-r--r--   0        0        0     8349 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/a0739889bf9412e8
+-rw-r--r--   0        0        0     5692 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/a225e4df39be9b29
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/a2340fd4c9aa1141
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/a513d558646cd439
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/b121e2b70fd66eb8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/b218ff88bc22b626
+-rw-r--r--   0        0        0    10964 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/b419496fa9e72887
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/b886c97e4d4117f0
+-rw-r--r--   0        0        0     8238 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/bdcdf5c7bbc1d738
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/c06de16f3c7a64cc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/c635f255374598c5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/c671ae94ff3d3e2e
+-rw-r--r--   0        0        0     8042 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/cdfecbca581311ee
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/ce44121ca4091b64
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/ced49ec87d10bcb0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/cfc06a1f13c8ab47
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/d16c5d29763a704e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/d225ad4c14b8ca60
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/d379b35d5e80b789
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/d3a95555c0919160
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/d655bee8ff0a59f2
+-rw-r--r--   0        0        0    11315 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/da4811a7730a562a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/dca573767bc8be7e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/e3e29f9eacb7027f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/e46ab4b61bb5d446
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/e5e0cc178d5c9df5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/eb564f7989641958
+-rw-r--r--   0        0        0    11467 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/eee2f3c667de6c7a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/f04d0d78a00adfd6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/f2ddc22a4b221f54
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/f879e8c947a6b7a4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/fa45ef3c3166e02d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.ruff_cache/content/faa51a5044a3c279
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 typedal-3.0.0b4/docs/1_getting_started.md
+-rw-r--r--   0        0        0     6509 2020-02-02 00:00:00.000000 typedal-3.0.0b4/docs/2_defining_tables.md
+-rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 typedal-3.0.0b4/docs/3_building_queries.md
+-rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 typedal-3.0.0b4/docs/4_relationships.md
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 typedal-3.0.0b4/docs/5_py4web.md
+-rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 typedal-3.0.0b4/docs/6_migrations.md
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 typedal-3.0.0b4/docs/index.md
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 typedal-3.0.0b4/docs/requirements.txt
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 typedal-3.0.0b4/docs/css/code_blocks.css
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 typedal-3.0.0b4/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 typedal-3.0.0b4/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     5891 2020-02-02 00:00:00.000000 typedal-3.0.0b4/htmlcov/d_0ccc93afd6526b6c___about___py.html
+-rw-r--r--   0        0        0     7907 2020-02-02 00:00:00.000000 typedal-3.0.0b4/htmlcov/d_0ccc93afd6526b6c___init___py.html
+-rw-r--r--   0        0        0   119633 2020-02-02 00:00:00.000000 typedal-3.0.0b4/htmlcov/d_0ccc93afd6526b6c_caching_py.html
+-rw-r--r--   0        0        0   146640 2020-02-02 00:00:00.000000 typedal-3.0.0b4/htmlcov/d_0ccc93afd6526b6c_cli_py.html
+-rw-r--r--   0        0        0   104666 2020-02-02 00:00:00.000000 typedal-3.0.0b4/htmlcov/d_0ccc93afd6526b6c_config_py.html
+-rw-r--r--   0        0        0   778432 2020-02-02 00:00:00.000000 typedal-3.0.0b4/htmlcov/d_0ccc93afd6526b6c_core_py.html
+-rw-r--r--   0        0        0    61614 2020-02-02 00:00:00.000000 typedal-3.0.0b4/htmlcov/d_0ccc93afd6526b6c_fields_py.html
+-rw-r--r--   0        0        0    17238 2020-02-02 00:00:00.000000 typedal-3.0.0b4/htmlcov/d_0ccc93afd6526b6c_for_py4web_py.html
+-rw-r--r--   0        0        0    22550 2020-02-02 00:00:00.000000 typedal-3.0.0b4/htmlcov/d_0ccc93afd6526b6c_for_web2py_py.html
+-rw-r--r--   0        0        0    69134 2020-02-02 00:00:00.000000 typedal-3.0.0b4/htmlcov/d_0ccc93afd6526b6c_helpers_py.html
+-rw-r--r--   0        0        0    42239 2020-02-02 00:00:00.000000 typedal-3.0.0b4/htmlcov/d_0ccc93afd6526b6c_types_py.html
+-rw-r--r--   0        0        0    17336 2020-02-02 00:00:00.000000 typedal-3.0.0b4/htmlcov/d_0ccc93afd6526b6c_web2py_py4web_shared_py.html
+-rw-r--r--   0        0        0    25828 2020-02-02 00:00:00.000000 typedal-3.0.0b4/htmlcov/d_18c616467159315a_as_json_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 typedal-3.0.0b4/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     7664 2020-02-02 00:00:00.000000 typedal-3.0.0b4/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 typedal-3.0.0b4/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 typedal-3.0.0b4/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 typedal-3.0.0b4/htmlcov/status.json
+-rw-r--r--   0        0        0    12406 2020-02-02 00:00:00.000000 typedal-3.0.0b4/htmlcov/style.css
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 typedal-3.0.0b4/src/typedal/__about__.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 typedal-3.0.0b4/src/typedal/__init__.py
+-rw-r--r--   0        0        0    11818 2020-02-02 00:00:00.000000 typedal-3.0.0b4/src/typedal/caching.py
+-rw-r--r--   0        0        0    18427 2020-02-02 00:00:00.000000 typedal-3.0.0b4/src/typedal/cli.py
+-rw-r--r--   0        0        0    11626 2020-02-02 00:00:00.000000 typedal-3.0.0b4/src/typedal/config.py
+-rw-r--r--   0        0        0    95038 2020-02-02 00:00:00.000000 typedal-3.0.0b4/src/typedal/core.py
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 typedal-3.0.0b4/src/typedal/fields.py
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 typedal-3.0.0b4/src/typedal/for_py4web.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 typedal-3.0.0b4/src/typedal/for_web2py.py
+-rw-r--r--   0        0        0     6509 2020-02-02 00:00:00.000000 typedal-3.0.0b4/src/typedal/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typedal-3.0.0b4/src/typedal/py.typed
+-rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 typedal-3.0.0b4/src/typedal/types.py
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 typedal-3.0.0b4/src/typedal/web2py_py4web_shared.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 typedal-3.0.0b4/src/typedal/serializers/as_json.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typedal-3.0.0b4/tests/__init__.py
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 typedal-3.0.0b4/tests/test_cli.py
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 typedal-3.0.0b4/tests/test_config.py
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 typedal-3.0.0b4/tests/test_docs_examples.py
+-rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 typedal-3.0.0b4/tests/test_helpers.py
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 typedal-3.0.0b4/tests/test_json.py
+-rw-r--r--   0        0        0    13197 2020-02-02 00:00:00.000000 typedal-3.0.0b4/tests/test_main.py
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 typedal-3.0.0b4/tests/test_mypy.py
+-rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 typedal-3.0.0b4/tests/test_orm.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 typedal-3.0.0b4/tests/test_py4web.py
+-rw-r--r--   0        0        0    11355 2020-02-02 00:00:00.000000 typedal-3.0.0b4/tests/test_query_builder.py
+-rw-r--r--   0        0        0    15716 2020-02-02 00:00:00.000000 typedal-3.0.0b4/tests/test_relationships.py
+-rw-r--r--   0        0        0     7012 2020-02-02 00:00:00.000000 typedal-3.0.0b4/tests/test_row.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 typedal-3.0.0b4/tests/test_stats.py
+-rw-r--r--   0        0        0     8365 2020-02-02 00:00:00.000000 typedal-3.0.0b4/tests/test_table.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 typedal-3.0.0b4/tests/test_web2py.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 typedal-3.0.0b4/tests/test_xx_others.py
+-rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 typedal-3.0.0b4/tests/timings.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 typedal-3.0.0b4/tests/configs/simple.toml
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 typedal-3.0.0b4/tests/configs/valid.env
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 typedal-3.0.0b4/tests/configs/valid.toml
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 typedal-3.0.0b4/.gitignore
+-rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 typedal-3.0.0b4/README.md
+-rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 typedal-3.0.0b4/pyproject.toml
+-rw-r--r--   0        0        0     7784 2020-02-02 00:00:00.000000 typedal-3.0.0b4/PKG-INFO
```

### Comparing `typedal-3.0.0b3/CHANGELOG.md` & `typedal-3.0.0b4/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v3.0.0-beta.4 (2024-03-20)
+
+### Fix
+
+* Bump pydal2sql dependency ([`33ba73e`](https://github.com/trialandsuccess/TypeDAL/commit/33ba73edbba4d0cf807a9a99846fb0b79d608262))
+
 ## v3.0.0-beta.3 (2024-03-20)
 
 ### Fix
 
 * Swap out black's implementation of find_pyproject_toml to configuraptor's ([`82676cc`](https://github.com/trialandsuccess/TypeDAL/commit/82676cc41f8734bc4e317b8f2b17f749024884ac))
 
 ## v3.0.0-beta.2 (2024-03-20)
```

### Comparing `typedal-3.0.0b3/coverage.svg` & `typedal-3.0.0b4/coverage.svg`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/example_new.py` & `typedal-3.0.0b4/example_new.py`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/example_old.py` & `typedal-3.0.0b4/example_old.py`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/mkdocs.yml` & `typedal-3.0.0b4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/_ast.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/_ast.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/_ast.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/_codecs.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/_codecs.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/_collections_abc.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/_collections_abc.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/_ctypes.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/_ctypes.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/_decimal.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/_decimal.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/_decimal.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/_decimal.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/abc.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/abc.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/array.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/array.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/array.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/array.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/builtins.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/builtins.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/builtins.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/codecs.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/codecs.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/codecs.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/contextlib.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/contextlib.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/dataclasses.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/dataclasses.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/datetime.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/datetime.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/datetime.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/decimal.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/decimal.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/decimal.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/decimal.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/enum.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/enum.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/enum.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/enum.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/genericpath.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/genericpath.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/io.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/io.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/io.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/io.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/mmap.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/mmap.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/mmap.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/numbers.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/numbers.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/numbers.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/numbers.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/pathlib.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/pathlib.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/pickle.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/pickle.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/pickle.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/posixpath.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/posixpath.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/re.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/re.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/re.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/re.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/sre_compile.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/sre_compile.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/sre_constants.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/sre_constants.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/sre_parse.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/sre_parse.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/subprocess.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/subprocess.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/sys.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/sys.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/sys.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/sys.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/time.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/time.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/time.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/time.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/types.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/types.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/types.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/types.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/typing.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/typing.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/typing.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/typing.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/typing_extensions.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/typing_extensions.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/_typeshed/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/_typeshed/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/collections/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/collections/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/collections/abc.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/collections/abc.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/ctypes/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/ctypes/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/email/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/email/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/email/charset.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/email/charset.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/email/contentmanager.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/email/contentmanager.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/email/errors.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/email/errors.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/email/header.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/email/header.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/email/header.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/email/message.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/email/message.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/email/message.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/email/policy.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/email/policy.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/importlib/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/importlib/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/importlib/abc.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/importlib/abc.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/importlib/machinery.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/importlib/machinery.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/importlib/metadata/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/importlib/metadata/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/importlib/metadata/_meta.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/importlib/metadata/_meta.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/os/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/os/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/os/path.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/os/path.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/os/path.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/src/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/src/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/src/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/src/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/src/typedal/__about__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/src/typedal/__about__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/src/typedal/__about__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/src/typedal/__about__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/src/typedal/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/src/typedal/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/src/typedal/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/src/typedal/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/src/typedal/core.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/src/typedal/core.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/src/typedal/core.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/src/typedal/core.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/src/typedal/fields.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/src/typedal/fields.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/src/typedal/fields.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/src/typedal/fields.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/src/typedal/pydal_objects.data.json` & `typedal-3.0.0b4/.mypy_cache/3.10/src/typedal/pydal_objects.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.10/src/typedal/pydal_objects.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.10/src/typedal/pydal_objects.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/__future__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/__future__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/__future__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/__future__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_ast.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_ast.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_bisect.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_bisect.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_bisect.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_bisect.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_codecs.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_codecs.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_collections_abc.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_collections_abc.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_compression.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_compression.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_compression.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_compression.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_csv.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_csv.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_csv.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_csv.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_ctypes.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_ctypes.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_decimal.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_decimal.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_decimal.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_decimal.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_json.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_json.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_json.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_json.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_locale.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_locale.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_locale.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_locale.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_operator.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_operator.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_operator.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_operator.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_random.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_random.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_random.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_random.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_socket.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_socket.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_socket.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_socket.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_stat.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_stat.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_stat.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_stat.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_thread.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_thread.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_thread.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_thread.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_tracemalloc.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_tracemalloc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_tracemalloc.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_tracemalloc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_warnings.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_warnings.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_warnings.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_warnings.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_weakref.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_weakref.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_weakref.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_weakref.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_weakrefset.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_weakrefset.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_weakrefset.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_weakrefset.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/abc.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/abc.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/argparse.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/argparse.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/argparse.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/argparse.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/array.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/array.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/array.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/array.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/ast.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/ast.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/ast.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/ast.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/atexit.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/atexit.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/atexit.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/atexit.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/base64.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/base64.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/base64.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/base64.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/bdb.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/bdb.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/bdb.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/bdb.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/binascii.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/binascii.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/binascii.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/binascii.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/bisect.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/bisect.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/bisect.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/bisect.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/builtins.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/builtins.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/bz2.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/bz2.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/bz2.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/bz2.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/calendar.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/calendar.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/calendar.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/calendar.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cmd.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cmd.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cmd.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cmd.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/codecs.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/codecs.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/colorsys.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/colorsys.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/colorsys.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/colorsys.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configparser.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configparser.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configparser.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configparser.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/contextlib.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/contextlib.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/contextvars.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/contextvars.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/contextvars.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/contextvars.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/copy.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/copy.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/copy.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/copy.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/copyreg.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/copyreg.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/copyreg.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/copyreg.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/csv.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/csv.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/csv.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/csv.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/dataclasses.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/dataclasses.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/datetime.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/datetime.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/datetime.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/decimal.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/decimal.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/decimal.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/decimal.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/difflib.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/difflib.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/difflib.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/difflib.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/dis.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/dis.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/dis.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/dis.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/doctest.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/doctest.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/doctest.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/doctest.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/enum.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/enum.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/enum.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/errno.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/errno.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/errno.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/errno.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/example_new.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/example_new.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/example_new.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/example_new.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/fnmatch.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/fnmatch.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/fnmatch.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/fnmatch.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/fractions.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/fractions.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/fractions.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/fractions.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/functools.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/functools.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/functools.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/functools.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/gc.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/gc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/gc.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/gc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/genericpath.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/genericpath.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/getpass.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/getpass.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/getpass.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/getpass.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/gettext.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/gettext.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/gettext.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/gettext.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/glob.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/glob.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/glob.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/glob.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/gzip.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/gzip.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/gzip.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/gzip.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/hashlib.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/hashlib.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/hashlib.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/hashlib.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/hmac.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/hmac.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/hmac.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/hmac.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/inspect.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/inspect.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/inspect.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/inspect.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/io.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/io.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/io.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/ipaddress.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/ipaddress.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/ipaddress.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/ipaddress.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/itertools.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/itertools.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/itertools.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/itertools.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/linecache.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/linecache.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/linecache.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/linecache.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/locale.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/locale.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/locale.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/locale.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/marshal.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/marshal.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/marshal.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/marshal.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/math.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/math.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/math.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/math.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/mimetypes.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/mimetypes.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/mimetypes.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/mimetypes.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/mmap.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/mmap.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/mmap.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/msvcrt.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/msvcrt.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/msvcrt.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/msvcrt.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/mypy_extensions.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/mypy_extensions.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/mypy_extensions.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/mypy_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/numbers.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/numbers.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/numbers.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/numbers.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/opcode.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/opcode.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/opcode.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/opcode.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/operator.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/operator.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/operator.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/operator.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pathlib.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pathlib.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pdb.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pdb.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pdb.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pdb.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pickle.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pickle.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pickle.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pkgutil.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pkgutil.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pkgutil.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pkgutil.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/platform.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/platform.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/platform.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/platform.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/posixpath.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/posixpath.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pprint.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pprint.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pprint.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pprint.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pty.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pty.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pty.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pty.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pydoc.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pydoc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pydoc.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pydoc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/queue.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/queue.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/queue.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/queue.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/random.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/random.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/random.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/random.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/re.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/re.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/re.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/reprlib.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/reprlib.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/reprlib.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/reprlib.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/secrets.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/secrets.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/secrets.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/secrets.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/select.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/select.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/select.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/select.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/selectors.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/selectors.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/selectors.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/selectors.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/shlex.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/shlex.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/shlex.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/shlex.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/shutil.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/shutil.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/shutil.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/shutil.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/signal.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/signal.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/signal.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/signal.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/socket.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/socket.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/socket.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/socket.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/src.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/src.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/src.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/src.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/sre_compile.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/sre_compile.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/sre_constants.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/sre_constants.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/sre_parse.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/sre_parse.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/ssl.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/ssl.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/ssl.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/ssl.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/stat.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/stat.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/stat.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/stat.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/string.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/string.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/string.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/string.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/struct.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/struct.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/struct.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/struct.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/subprocess.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/subprocess.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/sys.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/sys.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/sys.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/sys.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/sysconfig.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/sysconfig.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/sysconfig.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/sysconfig.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tarfile.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tarfile.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tarfile.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tarfile.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tempfile.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tempfile.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tempfile.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tempfile.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/termios.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/termios.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/termios.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/termios.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/textwrap.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/textwrap.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/textwrap.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/textwrap.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/threading.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/threading.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/threading.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/threading.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/time.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/time.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/time.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/time.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/token.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/token.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/token.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/token.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tokenize.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tokenize.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tokenize.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tokenize.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomllib.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomllib.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomllib.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomllib.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/traceback.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/traceback.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/traceback.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/traceback.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tracemalloc.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tracemalloc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tracemalloc.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tracemalloc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tty.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tty.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tty.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tty.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/types.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/types.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/types.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typing.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typing.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typing.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typing.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typing_extensions.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typing_extensions.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/unicodedata.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/unicodedata.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/unicodedata.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/unicodedata.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/uuid.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/uuid.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/uuid.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/uuid.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/warnings.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/warnings.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/warnings.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/warnings.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/weakref.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/weakref.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/weakref.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/weakref.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/zipfile.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/zipfile.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/zipfile.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/zipfile.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/zlib.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/zlib.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/zlib.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/zlib.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_argcomplete.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_argcomplete.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_argcomplete.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_argcomplete.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_version.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_version.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_version.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_version.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/cacheprovider.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/cacheprovider.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/cacheprovider.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/cacheprovider.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/capture.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/capture.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/capture.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/capture.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/compat.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/compat.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/compat.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/compat.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/debugging.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/debugging.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/debugging.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/debugging.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/deprecated.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/deprecated.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/deprecated.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/deprecated.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/doctest.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/doctest.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/doctest.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/doctest.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/fixtures.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/fixtures.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/fixtures.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/fixtures.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/freeze_support.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/freeze_support.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/freeze_support.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/freeze_support.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/helpconfig.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/helpconfig.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/helpconfig.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/helpconfig.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/hookspec.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/hookspec.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/hookspec.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/hookspec.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/legacypath.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/legacypath.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/legacypath.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/legacypath.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/logging.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/logging.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/logging.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/logging.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/main.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/main.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/main.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/main.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/monkeypatch.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/monkeypatch.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/monkeypatch.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/monkeypatch.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/nodes.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/nodes.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/nodes.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/nodes.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/outcomes.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/outcomes.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/outcomes.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/outcomes.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/pathlib.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/pathlib.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/pytester.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/pytester.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/pytester.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/pytester.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/pytester_assertions.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/pytester_assertions.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/pytester_assertions.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/pytester_assertions.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/python.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/python.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/python.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/python.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/python_api.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/python_api.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/python_api.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/python_api.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/recwarn.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/recwarn.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/recwarn.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/recwarn.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/reports.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/reports.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/reports.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/reports.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/runner.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/runner.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/runner.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/runner.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/scope.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/scope.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/scope.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/scope.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/stash.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/stash.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/stash.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/stash.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/terminal.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/terminal.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/terminal.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/terminal.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/timing.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/timing.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/timing.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/timing.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/tmpdir.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/tmpdir.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/tmpdir.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/tmpdir.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/warning_types.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/warning_types.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/warning_types.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/warning_types.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/warnings.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/warnings.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/warnings.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/warnings.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_code/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_code/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_code/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_code/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_code/code.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_code/code.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_code/code.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_code/code.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_code/source.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_code/source.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_code/source.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_code/source.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_io/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_io/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_io/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_io/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_io/saferepr.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_io/saferepr.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_io/saferepr.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_io/saferepr.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_io/terminalwriter.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_io/terminalwriter.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_io/terminalwriter.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_io/terminalwriter.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_io/wcwidth.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_io/wcwidth.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/_io/wcwidth.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/_io/wcwidth.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/assertion/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/assertion/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/assertion/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/assertion/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/assertion/rewrite.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/assertion/rewrite.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/assertion/rewrite.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/assertion/rewrite.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/assertion/truncate.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/assertion/truncate.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/assertion/truncate.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/assertion/truncate.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/assertion/util.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/assertion/util.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/assertion/util.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/assertion/util.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/config/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/config/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/config/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/config/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/config/argparsing.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/config/argparsing.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/config/argparsing.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/config/argparsing.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/config/compat.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/config/compat.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/config/compat.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/config/compat.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/config/exceptions.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/config/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/config/exceptions.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/config/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/config/findpaths.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/config/findpaths.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/config/findpaths.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/config/findpaths.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/mark/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/mark/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/mark/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/mark/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/mark/expression.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/mark/expression.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/mark/expression.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/mark/expression.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/mark/structures.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/mark/structures.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_pytest/mark/structures.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_pytest/mark/structures.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_typeshed/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_typeshed/xml.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_typeshed/xml.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/_typeshed/xml.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/_typeshed/xml.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/async_timeout/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/async_timeout/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/async_timeout/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/async_timeout/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/base_events.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/base_events.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/base_events.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/base_events.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/coroutines.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/coroutines.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/coroutines.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/coroutines.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/events.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/events.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/events.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/events.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/exceptions.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/exceptions.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/futures.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/futures.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/futures.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/futures.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/locks.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/locks.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/locks.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/locks.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/mixins.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/mixins.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/mixins.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/mixins.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/protocols.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/protocols.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/protocols.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/protocols.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/queues.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/queues.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/queues.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/queues.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/runners.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/runners.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/runners.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/runners.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/selector_events.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/selector_events.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/selector_events.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/selector_events.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/streams.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/streams.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/streams.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/streams.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/subprocess.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/subprocess.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/taskgroups.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/taskgroups.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/taskgroups.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/taskgroups.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/tasks.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/tasks.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/tasks.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/tasks.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/threads.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/threads.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/threads.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/threads.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/timeouts.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/timeouts.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/timeouts.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/timeouts.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/transports.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/transports.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/transports.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/transports.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/unix_events.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/unix_events.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/asyncio/unix_events.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/asyncio/unix_events.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/_width_table.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/_width_table.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/_width_table.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/_width_table.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/brackets.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/brackets.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/brackets.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/brackets.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/cache.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/cache.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/cache.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/cache.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/comments.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/comments.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/comments.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/comments.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/const.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/const.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/const.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/const.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/files.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/files.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/files.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/files.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/handle_ipynb_magics.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/handle_ipynb_magics.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/handle_ipynb_magics.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/handle_ipynb_magics.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/linegen.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/linegen.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/linegen.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/linegen.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/lines.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/lines.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/lines.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/lines.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/mode.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/mode.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/mode.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/mode.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/nodes.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/nodes.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/nodes.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/nodes.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/numerics.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/numerics.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/numerics.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/numerics.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/output.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/output.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/output.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/output.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/parsing.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/parsing.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/parsing.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/parsing.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/ranges.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/ranges.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/ranges.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/ranges.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/report.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/report.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/report.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/report.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/rusty.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/rusty.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/rusty.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/rusty.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/strings.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/strings.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/strings.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/strings.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/trans.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/trans.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/black/trans.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/black/trans.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/click/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/click/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/click/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/click/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/click/_compat.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/click/_compat.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/click/_compat.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/click/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/click/_termui_impl.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/click/_termui_impl.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/click/_termui_impl.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/click/_termui_impl.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/click/core.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/click/core.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/click/core.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/click/core.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/click/decorators.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/click/decorators.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/click/decorators.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/click/decorators.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/click/exceptions.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/click/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/click/exceptions.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/click/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/click/formatting.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/click/formatting.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/click/formatting.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/click/formatting.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/click/globals.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/click/globals.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/click/globals.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/click/globals.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/click/parser.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/click/parser.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/click/parser.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/click/parser.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/click/shell_completion.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/click/shell_completion.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/click/shell_completion.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/click/shell_completion.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/click/termui.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/click/termui.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/click/termui.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/click/termui.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/click/types.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/click/types.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/click/types.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/click/types.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/click/utils.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/click/utils.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/click/utils.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/click/utils.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/collections/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/collections/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/collections/abc.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/collections/abc.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/concurrent/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/concurrent/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/concurrent/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/concurrent/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/concurrent/futures/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/concurrent/futures/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/concurrent/futures/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/concurrent/futures/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/concurrent/futures/_base.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/concurrent/futures/_base.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/concurrent/futures/_base.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/concurrent/futures/_base.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/concurrent/futures/process.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/concurrent/futures/process.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/concurrent/futures/process.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/concurrent/futures/process.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/concurrent/futures/thread.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/concurrent/futures/thread.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/concurrent/futures/thread.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/concurrent/futures/thread.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configurablejson/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configurablejson/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configurablejson/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configurablejson/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configurablejson/_internals.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configurablejson/_internals.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configurablejson/_internals.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configurablejson/_internals.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configurablejson/encode.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configurablejson/encode.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configurablejson/encode.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configurablejson/encode.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/abs.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/abs.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/abs.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/abs.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/alias.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/alias.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/alias.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/alias.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/beautify.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/beautify.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/beautify.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/beautify.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/binary_config.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/binary_config.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/binary_config.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/binary_config.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/cls.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/cls.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/cls.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/cls.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/core.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/core.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/core.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/core.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/dump.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/dump.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/dump.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/dump.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/errors.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/errors.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/errors.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/errors.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/helpers.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/helpers.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/helpers.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/helpers.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/postpone.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/postpone.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/postpone.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/postpone.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/singleton.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/singleton.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/singleton.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/singleton.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/type_converters.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/type_converters.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/type_converters.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/type_converters.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/loaders/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/loaders/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/loaders/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/loaders/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/loaders/_types.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/loaders/_types.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/loaders/_types.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/loaders/_types.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/loaders/loaders_shared.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/loaders/loaders_shared.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/loaders/loaders_shared.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/loaders/loaders_shared.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/loaders/register.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/loaders/register.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/configuraptor/loaders/register.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/configuraptor/loaders/register.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/__about__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/__about__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/__about__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/__about__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/exceptions.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/exceptions.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/utils.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/utils.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/utils.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/utils.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/_oid.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/_oid.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/_oid.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/_oid.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/aead.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/aead.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/aead.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/aead.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/backend.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/backend.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/backend.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/backend.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/ciphers.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/ciphers.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/ciphers.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/ciphers.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/cmac.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/cmac.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/cmac.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/cmac.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/ec.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/ec.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/ec.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/ec.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/rsa.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/rsa.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/rsa.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/rsa.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/utils.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/utils.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/utils.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/backends/openssl/utils.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/_openssl.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/_openssl.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/_openssl.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/_openssl.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/asn1.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/asn1.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/asn1.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/asn1.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/exceptions.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/exceptions.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/ocsp.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/ocsp.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/ocsp.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/ocsp.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/x509.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/x509.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/x509.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/x509.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/aead.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/aead.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/aead.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/aead.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/cmac.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/cmac.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/cmac.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/cmac.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/dh.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/dh.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/dh.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/dh.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/dsa.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/dsa.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/dsa.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/dsa.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/ec.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/ec.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/ec.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/ec.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/ed25519.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/ed25519.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/ed25519.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/ed25519.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/ed448.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/ed448.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/ed448.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/ed448.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/hashes.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/hashes.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/hashes.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/hashes.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/hmac.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/hmac.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/hmac.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/hmac.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/kdf.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/kdf.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/kdf.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/kdf.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/keys.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/keys.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/keys.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/keys.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/poly1305.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/poly1305.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/poly1305.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/poly1305.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/rsa.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/rsa.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/rsa.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/rsa.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/x25519.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/x25519.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/x25519.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/x25519.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/x448.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/x448.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/x448.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/_rust/openssl/x448.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/openssl/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/openssl/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/openssl/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/openssl/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/openssl/_conditional.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/openssl/_conditional.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/openssl/_conditional.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/openssl/_conditional.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/openssl/binding.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/openssl/binding.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/bindings/openssl/binding.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/bindings/openssl/binding.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/_asymmetric.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/_asymmetric.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/_asymmetric.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/_asymmetric.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/_cipheralgorithm.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/_cipheralgorithm.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/_cipheralgorithm.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/_cipheralgorithm.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/_serialization.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/_serialization.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/_serialization.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/_serialization.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/constant_time.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/constant_time.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/constant_time.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/constant_time.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/hashes.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/hashes.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/hashes.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/hashes.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/dh.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/dh.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/dh.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/dh.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/dsa.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/dsa.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/dsa.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/dsa.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/ec.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/ec.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/ec.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/ec.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/ed25519.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/ed25519.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/ed25519.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/ed25519.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/ed448.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/ed448.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/ed448.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/ed448.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/padding.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/padding.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/padding.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/padding.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/rsa.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/rsa.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/rsa.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/rsa.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/types.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/types.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/types.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/types.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/utils.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/utils.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/utils.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/utils.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/x25519.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/x25519.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/x25519.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/x25519.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/x448.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/x448.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/x448.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/asymmetric/x448.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/aead.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/aead.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/aead.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/aead.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/algorithms.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/algorithms.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/algorithms.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/algorithms.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/base.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/base.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/base.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/base.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/modes.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/modes.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/modes.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/ciphers/modes.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/serialization/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/serialization/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/serialization/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/serialization/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/serialization/base.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/serialization/base.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/serialization/base.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/serialization/base.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/serialization/pkcs12.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/serialization/pkcs12.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/serialization/pkcs12.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/serialization/pkcs12.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/serialization/ssh.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/serialization/ssh.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/hazmat/primitives/serialization/ssh.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/hazmat/primitives/serialization/ssh.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/base.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/base.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/base.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/base.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/certificate_transparency.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/certificate_transparency.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/certificate_transparency.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/certificate_transparency.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/extensions.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/extensions.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/extensions.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/extensions.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/general_name.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/general_name.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/general_name.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/general_name.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/name.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/name.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/name.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/name.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/ocsp.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/ocsp.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/ocsp.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/ocsp.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/oid.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/oid.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/oid.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/oid.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/verification.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/verification.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/cryptography/x509/verification.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/cryptography/x509/verification.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/ctypes/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/ctypes/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/ctypes/wintypes.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/ctypes/wintypes.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/ctypes/wintypes.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/ctypes/wintypes.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/distutils/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/distutils/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/distutils/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/distutils/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/distutils/util.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/distutils/util.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/distutils/util.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/distutils/util.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/dotenv/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/dotenv/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/dotenv/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/dotenv/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/dotenv/main.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/dotenv/main.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/dotenv/main.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/dotenv/main.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/dotenv/parser.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/dotenv/parser.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/dotenv/parser.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/dotenv/parser.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/dotenv/variables.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/dotenv/variables.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/dotenv/variables.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/dotenv/variables.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/edwh_migrate/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/edwh_migrate/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/edwh_migrate/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/edwh_migrate/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/edwh_migrate/migrate.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/edwh_migrate/migrate.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/edwh_migrate/migrate.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/edwh_migrate/migrate.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/email/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/email/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/email/charset.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/email/charset.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/email/contentmanager.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/email/contentmanager.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/email/errors.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/email/errors.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/email/header.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/email/header.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/email/message.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/email/message.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/email/message.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/email/policy.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/email/policy.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/email/utils.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/email/utils.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/email/utils.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/email/utils.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/cmd.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/cmd.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/cmd.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/cmd.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/compat.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/compat.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/compat.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/compat.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/config.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/config.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/config.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/config.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/db.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/db.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/db.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/db.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/diff.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/diff.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/diff.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/diff.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/exc.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/exc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/exc.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/exc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/remote.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/remote.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/remote.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/remote.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/types.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/types.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/types.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/types.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/util.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/util.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/util.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/util.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/index/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/index/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/index/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/index/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/index/base.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/index/base.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/index/base.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/index/base.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/index/fun.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/index/fun.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/index/fun.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/index/fun.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/index/typ.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/index/typ.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/index/typ.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/index/typ.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/index/util.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/index/util.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/index/util.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/index/util.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/objects/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/objects/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/objects/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/objects/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/objects/base.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/objects/base.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/objects/base.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/objects/base.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/objects/blob.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/objects/blob.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/objects/blob.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/objects/blob.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/objects/commit.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/objects/commit.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/objects/commit.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/objects/commit.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/objects/fun.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/objects/fun.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/objects/fun.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/objects/fun.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/objects/tag.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/objects/tag.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/objects/tag.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/objects/tag.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/objects/tree.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/objects/tree.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/objects/tree.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/objects/tree.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/objects/util.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/objects/util.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/objects/util.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/objects/util.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/objects/submodule/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/objects/submodule/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/objects/submodule/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/objects/submodule/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/objects/submodule/base.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/objects/submodule/base.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/objects/submodule/base.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/objects/submodule/base.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/objects/submodule/root.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/objects/submodule/root.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/objects/submodule/root.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/objects/submodule/root.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/objects/submodule/util.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/objects/submodule/util.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/objects/submodule/util.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/objects/submodule/util.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/refs/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/refs/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/refs/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/refs/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/refs/head.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/refs/head.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/refs/head.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/refs/head.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/refs/log.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/refs/log.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/refs/log.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/refs/log.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/refs/reference.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/refs/reference.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/refs/reference.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/refs/reference.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/refs/remote.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/refs/remote.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/refs/remote.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/refs/remote.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/refs/symbolic.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/refs/symbolic.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/refs/symbolic.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/refs/symbolic.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/refs/tag.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/refs/tag.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/refs/tag.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/refs/tag.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/repo/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/repo/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/repo/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/repo/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/repo/base.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/repo/base.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/repo/base.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/repo/base.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/repo/fun.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/repo/fun.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/git/repo/fun.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/git/repo/fun.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/html/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/html/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/html/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/html/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/html/entities.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/html/entities.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/html/entities.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/html/entities.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/http/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/http/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/http/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/http/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/http/client.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/http/client.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/http/client.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/http/client.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/http/cookiejar.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/http/cookiejar.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/http/cookiejar.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/http/cookiejar.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/importlib/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/importlib/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/importlib/abc.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/importlib/abc.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/importlib/machinery.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/importlib/machinery.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/importlib/readers.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/importlib/readers.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/importlib/readers.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/importlib/readers.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/importlib/util.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/importlib/util.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/importlib/util.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/importlib/util.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/importlib/resources/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/importlib/resources/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/importlib/resources/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/importlib/resources/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/importlib/resources/abc.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/importlib/resources/abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/importlib/resources/abc.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/importlib/resources/abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/iniconfig/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/iniconfig/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/iniconfig/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/iniconfig/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/iniconfig/_parse.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/iniconfig/_parse.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/iniconfig/_parse.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/iniconfig/_parse.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/iniconfig/exceptions.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/iniconfig/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/iniconfig/exceptions.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/iniconfig/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/json/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/json/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/json/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/json/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/json/decoder.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/json/decoder.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/json/decoder.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/json/decoder.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/json/encoder.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/json/encoder.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/json/encoder.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/json/encoder.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/logging/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/logging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/logging/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/logging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/_compat.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/_compat.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/_compat.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/_punycode.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/_punycode.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/_punycode.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/_punycode.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/main.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/main.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/main.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/main.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/parser_block.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/parser_block.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/parser_block.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/parser_block.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/parser_core.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/parser_core.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/parser_core.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/parser_core.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/parser_inline.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/parser_inline.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/parser_inline.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/parser_inline.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/renderer.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/renderer.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/renderer.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/renderer.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/ruler.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/ruler.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/ruler.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/ruler.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/token.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/token.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/token.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/token.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/utils.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/utils.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/utils.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/utils.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/common/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/common/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/common/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/common/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/common/entities.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/common/entities.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/common/entities.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/common/entities.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/common/html_re.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/common/html_re.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/common/html_re.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/common/html_re.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/common/utils.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/common/utils.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/common/utils.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/common/utils.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/presets/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/presets/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/presets/default.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/presets/default.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/presets/default.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/presets/default.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/presets/zero.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/presets/zero.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/presets/zero.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/presets/zero.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/code.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/code.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/list.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/list.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/table.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/table.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/block.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/block.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/text_join.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/text_join.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_core/text_join.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_core/text_join.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/fragments_join.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/fragments_join.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/fragments_join.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/fragments_join.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/linkify.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/linkify.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/linkify.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/linkify.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/mdurl/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/mdurl/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/mdurl/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/mdurl/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/mdurl/_decode.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/mdurl/_decode.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/mdurl/_decode.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/mdurl/_decode.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/mdurl/_encode.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/mdurl/_encode.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/mdurl/_encode.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/mdurl/_encode.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/mdurl/_format.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/mdurl/_format.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/mdurl/_format.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/mdurl/_format.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/mdurl/_parse.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/mdurl/_parse.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/mdurl/_parse.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/mdurl/_parse.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/mdurl/_url.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/mdurl/_url.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/mdurl/_url.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/mdurl/_url.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/connection.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/connection.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/connection.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/connection.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/context.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/context.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/context.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/context.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/managers.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/managers.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/managers.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/managers.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/pool.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/pool.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/pool.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/pool.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/popen_fork.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/popen_fork.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/process.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/process.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/process.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/process.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/queues.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/queues.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/queues.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/queues.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/reduction.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/reduction.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/reduction.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/reduction.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/shared_memory.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/shared_memory.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/spawn.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/spawn.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/spawn.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/spawn.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/synchronize.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/synchronize.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/synchronize.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/synchronize.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/util.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/util.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/multiprocessing/util.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/multiprocessing/util.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/os/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/os/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/os/path.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/os/path.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/packaging/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/packaging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/packaging/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/packaging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/packaging/_elffile.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/packaging/_elffile.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/packaging/_elffile.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/packaging/_elffile.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/packaging/_manylinux.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/packaging/_manylinux.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/packaging/_manylinux.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/packaging/_manylinux.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/packaging/_musllinux.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/packaging/_musllinux.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/packaging/_musllinux.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/packaging/_musllinux.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/packaging/_parser.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/packaging/_parser.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/packaging/_parser.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/packaging/_parser.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/packaging/_structures.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/packaging/_structures.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/packaging/_structures.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/packaging/_structures.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/packaging/_tokenizer.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/packaging/_tokenizer.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/packaging/_tokenizer.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/packaging/_tokenizer.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/packaging/markers.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/packaging/markers.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/packaging/markers.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/packaging/markers.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/packaging/requirements.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/packaging/requirements.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/packaging/requirements.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/packaging/requirements.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/packaging/specifiers.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/packaging/specifiers.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/packaging/specifiers.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/packaging/specifiers.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/packaging/tags.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/packaging/tags.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/packaging/tags.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/packaging/tags.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/packaging/utils.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/packaging/utils.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/packaging/utils.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/packaging/utils.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/packaging/version.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/packaging/version.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/packaging/version.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/packaging/version.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pathspec/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pathspec/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pathspec/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pathspec/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pathspec/_meta.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pathspec/_meta.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pathspec/_meta.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pathspec/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pathspec/gitignore.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pathspec/gitignore.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pathspec/gitignore.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pathspec/gitignore.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pathspec/pathspec.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pathspec/pathspec.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pathspec/pathspec.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pathspec/pathspec.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pathspec/pattern.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pathspec/pattern.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pathspec/pattern.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pathspec/pattern.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pathspec/util.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pathspec/util.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pathspec/util.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pathspec/util.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pathspec/patterns/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pathspec/patterns/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pathspec/patterns/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pathspec/patterns/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/platformdirs/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/platformdirs/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/platformdirs/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/platformdirs/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/platformdirs/api.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/platformdirs/api.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/platformdirs/api.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/platformdirs/api.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/platformdirs/version.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/platformdirs/version.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/platformdirs/version.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/platformdirs/version.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pluggy/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pluggy/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pluggy/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pluggy/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pluggy/_callers.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pluggy/_callers.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pluggy/_callers.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pluggy/_callers.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pluggy/_hooks.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pluggy/_hooks.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pluggy/_hooks.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pluggy/_hooks.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pluggy/_manager.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pluggy/_manager.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pluggy/_manager.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pluggy/_manager.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pluggy/_result.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pluggy/_result.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pluggy/_result.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pluggy/_result.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pluggy/_tracing.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pluggy/_tracing.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pluggy/_tracing.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pluggy/_tracing.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pluggy/_version.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pluggy/_version.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pluggy/_version.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pluggy/_version.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/auto_suggest.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/auto_suggest.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/auto_suggest.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/auto_suggest.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/buffer.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/buffer.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/buffer.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/buffer.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/cache.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/cache.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/cache.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/cache.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/cursor_shapes.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/cursor_shapes.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/cursor_shapes.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/cursor_shapes.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/data_structures.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/data_structures.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/data_structures.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/data_structures.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/document.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/document.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/document.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/document.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/enums.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/enums.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/enums.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/enums.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/history.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/history.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/history.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/history.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/keys.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/keys.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/keys.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/keys.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/mouse_events.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/mouse_events.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/mouse_events.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/mouse_events.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/patch_stdout.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/patch_stdout.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/patch_stdout.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/patch_stdout.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/renderer.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/renderer.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/renderer.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/renderer.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/search.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/search.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/search.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/search.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/selection.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/selection.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/selection.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/selection.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/utils.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/utils.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/utils.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/utils.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/validation.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/validation.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/validation.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/validation.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/application/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/application/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/application/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/application/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/application/application.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/application/application.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/application/application.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/application/application.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/application/current.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/application/current.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/application/current.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/application/current.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/application/dummy.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/application/dummy.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/application/dummy.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/application/dummy.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/application/run_in_terminal.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/application/run_in_terminal.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/application/run_in_terminal.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/application/run_in_terminal.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/clipboard/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/clipboard/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/clipboard/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/clipboard/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/clipboard/base.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/clipboard/base.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/clipboard/base.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/clipboard/base.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/clipboard/in_memory.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/clipboard/in_memory.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/clipboard/in_memory.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/clipboard/in_memory.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/completion/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/completion/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/completion/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/completion/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/completion/base.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/completion/base.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/completion/base.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/completion/base.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/completion/deduplicate.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/completion/deduplicate.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/completion/deduplicate.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/completion/deduplicate.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/completion/filesystem.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/completion/filesystem.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/completion/filesystem.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/completion/filesystem.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/completion/fuzzy_completer.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/completion/fuzzy_completer.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/completion/fuzzy_completer.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/completion/fuzzy_completer.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/completion/nested.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/completion/nested.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/completion/nested.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/completion/nested.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/completion/word_completer.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/completion/word_completer.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/completion/word_completer.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/completion/word_completer.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/eventloop/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/eventloop/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/eventloop/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/eventloop/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/eventloop/async_context_manager.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/eventloop/async_context_manager.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/eventloop/async_context_manager.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/eventloop/async_context_manager.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/eventloop/async_generator.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/eventloop/async_generator.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/eventloop/async_generator.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/eventloop/async_generator.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/eventloop/dummy_contextvars.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/eventloop/dummy_contextvars.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/eventloop/dummy_contextvars.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/eventloop/dummy_contextvars.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/eventloop/inputhook.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/eventloop/inputhook.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/eventloop/inputhook.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/eventloop/inputhook.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/eventloop/utils.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/eventloop/utils.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/eventloop/utils.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/eventloop/utils.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/filters/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/filters/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/filters/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/filters/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/filters/app.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/filters/app.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/filters/app.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/filters/app.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/filters/base.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/filters/base.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/filters/base.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/filters/base.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/filters/cli.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/filters/cli.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/filters/cli.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/filters/cli.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/filters/utils.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/filters/utils.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/filters/utils.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/filters/utils.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/formatted_text/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/formatted_text/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/formatted_text/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/formatted_text/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/formatted_text/ansi.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/formatted_text/ansi.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/formatted_text/ansi.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/formatted_text/ansi.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/formatted_text/base.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/formatted_text/base.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/formatted_text/base.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/formatted_text/base.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/formatted_text/html.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/formatted_text/html.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/formatted_text/html.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/formatted_text/html.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/formatted_text/pygments.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/formatted_text/pygments.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/formatted_text/pygments.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/formatted_text/pygments.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/formatted_text/utils.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/formatted_text/utils.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/formatted_text/utils.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/formatted_text/utils.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/input/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/input/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/input/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/input/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/input/ansi_escape_sequences.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/input/ansi_escape_sequences.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/input/ansi_escape_sequences.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/input/ansi_escape_sequences.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/input/base.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/input/base.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/input/base.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/input/base.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/input/defaults.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/input/defaults.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/input/defaults.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/input/defaults.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/input/typeahead.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/input/typeahead.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/input/typeahead.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/input/typeahead.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/input/vt100_parser.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/input/vt100_parser.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/input/vt100_parser.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/input/vt100_parser.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/defaults.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/defaults.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/defaults.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/defaults.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/digraphs.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/digraphs.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/digraphs.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/digraphs.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/emacs_state.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/emacs_state.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/emacs_state.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/emacs_state.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/key_bindings.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/key_bindings.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/key_bindings.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/key_bindings.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/key_processor.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/key_processor.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/key_processor.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/key_processor.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/vi_state.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/vi_state.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/vi_state.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/vi_state.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/auto_suggest.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/auto_suggest.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/auto_suggest.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/auto_suggest.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/basic.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/basic.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/basic.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/basic.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/completion.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/completion.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/completion.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/completion.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/cpr.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/cpr.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/cpr.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/cpr.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/emacs.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/emacs.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/emacs.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/emacs.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/focus.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/focus.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/focus.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/focus.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/mouse.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/mouse.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/mouse.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/mouse.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/named_commands.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/named_commands.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/named_commands.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/named_commands.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/open_in_editor.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/open_in_editor.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/open_in_editor.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/open_in_editor.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/page_navigation.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/page_navigation.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/page_navigation.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/page_navigation.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/scroll.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/scroll.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/scroll.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/scroll.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/vi.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/vi.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/vi.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/key_binding/bindings/vi.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/containers.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/containers.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/containers.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/containers.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/controls.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/controls.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/controls.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/controls.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/dimension.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/dimension.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/dimension.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/dimension.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/dummy.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/dummy.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/dummy.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/dummy.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/layout.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/layout.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/layout.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/layout.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/margins.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/margins.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/margins.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/margins.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/menus.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/menus.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/menus.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/menus.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/mouse_handlers.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/mouse_handlers.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/mouse_handlers.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/mouse_handlers.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/processors.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/processors.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/processors.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/processors.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/screen.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/screen.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/screen.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/screen.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/scrollable_pane.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/scrollable_pane.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/scrollable_pane.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/scrollable_pane.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/utils.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/utils.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/layout/utils.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/layout/utils.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/lexers/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/lexers/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/lexers/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/lexers/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/lexers/base.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/lexers/base.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/lexers/base.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/lexers/base.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/lexers/pygments.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/lexers/pygments.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/lexers/pygments.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/lexers/pygments.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/output/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/output/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/output/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/output/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/output/base.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/output/base.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/output/base.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/output/base.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/output/color_depth.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/output/color_depth.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/output/color_depth.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/output/color_depth.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/output/defaults.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/output/defaults.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/output/defaults.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/output/defaults.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/output/flush_stdout.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/output/flush_stdout.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/output/flush_stdout.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/output/flush_stdout.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/output/plain_text.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/output/plain_text.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/output/plain_text.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/output/plain_text.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/output/vt100.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/output/vt100.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/output/vt100.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/output/vt100.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/shortcuts/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/shortcuts/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/shortcuts/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/shortcuts/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/shortcuts/dialogs.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/shortcuts/dialogs.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/shortcuts/dialogs.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/shortcuts/dialogs.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/shortcuts/prompt.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/shortcuts/prompt.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/shortcuts/prompt.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/shortcuts/prompt.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/shortcuts/utils.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/shortcuts/utils.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/shortcuts/utils.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/shortcuts/utils.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/shortcuts/progress_bar/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/shortcuts/progress_bar/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/shortcuts/progress_bar/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/shortcuts/progress_bar/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/shortcuts/progress_bar/base.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/shortcuts/progress_bar/base.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/shortcuts/progress_bar/base.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/shortcuts/progress_bar/base.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/shortcuts/progress_bar/formatters.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/shortcuts/progress_bar/formatters.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/shortcuts/progress_bar/formatters.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/shortcuts/progress_bar/formatters.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/styles/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/styles/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/styles/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/styles/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/styles/base.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/styles/base.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/styles/base.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/styles/base.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/styles/defaults.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/styles/defaults.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/styles/defaults.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/styles/defaults.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/styles/named_colors.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/styles/named_colors.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/styles/named_colors.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/styles/named_colors.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/styles/pygments.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/styles/pygments.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/styles/pygments.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/styles/pygments.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/styles/style.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/styles/style.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/styles/style.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/styles/style.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/styles/style_transformation.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/styles/style_transformation.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/styles/style_transformation.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/styles/style_transformation.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/widgets/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/widgets/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/widgets/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/widgets/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/widgets/base.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/widgets/base.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/widgets/base.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/widgets/base.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/widgets/dialogs.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/widgets/dialogs.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/widgets/dialogs.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/widgets/dialogs.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/widgets/menus.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/widgets/menus.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/widgets/menus.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/widgets/menus.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/widgets/toolbars.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/widgets/toolbars.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/prompt_toolkit/widgets/toolbars.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/prompt_toolkit/widgets/toolbars.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pydal2sql/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pydal2sql/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pydal2sql/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pydal2sql/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pydal2sql/typer_support.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pydal2sql/typer_support.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pydal2sql/typer_support.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pydal2sql/typer_support.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pydal2sql/types.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pydal2sql/types.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pydal2sql/types.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pydal2sql/types.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pydal2sql_core/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pydal2sql_core/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pydal2sql_core/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pydal2sql_core/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pydal2sql_core/cli_support.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pydal2sql_core/cli_support.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pydal2sql_core/cli_support.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pydal2sql_core/cli_support.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pydal2sql_core/core.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pydal2sql_core/core.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pydal2sql_core/core.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pydal2sql_core/core.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pydal2sql_core/helpers.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pydal2sql_core/helpers.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pydal2sql_core/helpers.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pydal2sql_core/helpers.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pydal2sql_core/types.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pydal2sql_core/types.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pydal2sql_core/types.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pydal2sql_core/types.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pyexpat/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pyexpat/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pyexpat/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pyexpat/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pyexpat/errors.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pyexpat/errors.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pyexpat/errors.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pyexpat/errors.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pyexpat/model.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pyexpat/model.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pyexpat/model.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pyexpat/model.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pytest/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pytest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/pytest/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/pytest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/constants.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/constants.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/constants.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/constants.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/form.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/form.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/form.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/form.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompt.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompt.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompt.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompt.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/question.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/question.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/question.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/question.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/styles.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/styles.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/styles.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/styles.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/utils.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/utils.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/utils.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/utils.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/version.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/version.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/version.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/version.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/autocomplete.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/autocomplete.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/autocomplete.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/autocomplete.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/checkbox.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/checkbox.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/checkbox.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/checkbox.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/common.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/common.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/common.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/common.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/confirm.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/confirm.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/confirm.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/confirm.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/password.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/password.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/password.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/password.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/path.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/path.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/path.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/path.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/press_any_key_to_continue.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/press_any_key_to_continue.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/press_any_key_to_continue.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/press_any_key_to_continue.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/rawselect.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/rawselect.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/rawselect.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/rawselect.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/select.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/select.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/select.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/select.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/text.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/text.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/questionary/prompts/text.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/questionary/prompts/text.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/backoff.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/backoff.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/backoff.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/backoff.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/client.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/client.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/client.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/client.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/cluster.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/cluster.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/cluster.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/cluster.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/compat.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/compat.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/compat.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/compat.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/connection.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/connection.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/connection.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/connection.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/crc.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/crc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/crc.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/crc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/credentials.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/credentials.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/credentials.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/credentials.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/exceptions.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/exceptions.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/lock.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/lock.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/lock.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/lock.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/ocsp.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/ocsp.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/ocsp.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/ocsp.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/retry.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/retry.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/retry.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/retry.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/sentinel.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/sentinel.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/sentinel.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/sentinel.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/typing.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/typing.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/typing.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/typing.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/utils.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/utils.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/utils.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/utils.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/base.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/base.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/base.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/base.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/commands.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/commands.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/commands.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/commands.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/encoders.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/encoders.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/encoders.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/encoders.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/helpers.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/helpers.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/helpers.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/helpers.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/hiredis.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/hiredis.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/hiredis.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/hiredis.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/resp2.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/resp2.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/resp2.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/resp2.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/resp3.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/resp3.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/resp3.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/resp3.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/socket.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/socket.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/_parsers/socket.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/_parsers/socket.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/asyncio/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/asyncio/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/asyncio/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/asyncio/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/asyncio/client.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/asyncio/client.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/asyncio/client.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/asyncio/client.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/asyncio/cluster.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/asyncio/cluster.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/asyncio/cluster.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/asyncio/cluster.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/asyncio/connection.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/asyncio/connection.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/asyncio/connection.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/asyncio/connection.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/asyncio/lock.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/asyncio/lock.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/asyncio/lock.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/asyncio/lock.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/asyncio/retry.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/asyncio/retry.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/asyncio/retry.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/asyncio/retry.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/asyncio/sentinel.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/asyncio/sentinel.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/asyncio/sentinel.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/asyncio/sentinel.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/asyncio/utils.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/asyncio/utils.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/asyncio/utils.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/asyncio/utils.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/cluster.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/cluster.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/cluster.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/cluster.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/core.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/core.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/core.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/core.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/helpers.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/helpers.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/helpers.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/helpers.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/redismodules.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/redismodules.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/redismodules.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/redismodules.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/sentinel.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/sentinel.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/sentinel.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/sentinel.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/bf/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/bf/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/bf/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/bf/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/bf/commands.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/bf/commands.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/bf/commands.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/bf/commands.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/bf/info.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/bf/info.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/bf/info.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/bf/info.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/graph/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/graph/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/graph/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/graph/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/graph/commands.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/graph/commands.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/graph/commands.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/graph/commands.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/graph/edge.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/graph/edge.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/graph/edge.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/graph/edge.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/graph/exceptions.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/graph/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/graph/exceptions.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/graph/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/graph/execution_plan.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/graph/execution_plan.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/graph/execution_plan.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/graph/execution_plan.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/graph/node.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/graph/node.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/graph/node.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/graph/node.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/graph/path.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/graph/path.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/graph/path.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/graph/path.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/graph/query_result.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/graph/query_result.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/graph/query_result.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/graph/query_result.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/json/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/json/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/json/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/json/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/json/_util.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/json/_util.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/json/_util.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/json/_util.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/json/commands.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/json/commands.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/json/commands.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/json/commands.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/json/decoders.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/json/decoders.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/json/decoders.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/json/decoders.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/json/path.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/json/path.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/json/path.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/json/path.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/search/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/search/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/search/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/search/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/search/_util.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/search/_util.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/search/_util.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/search/_util.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/search/aggregation.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/search/aggregation.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/search/aggregation.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/search/aggregation.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/search/commands.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/search/commands.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/search/commands.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/search/commands.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/search/document.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/search/document.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/search/document.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/search/document.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/search/query.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/search/query.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/search/query.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/search/query.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/search/result.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/search/result.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/search/result.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/search/result.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/search/suggestion.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/search/suggestion.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/search/suggestion.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/search/suggestion.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/timeseries/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/timeseries/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/timeseries/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/timeseries/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/timeseries/commands.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/timeseries/commands.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/timeseries/commands.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/timeseries/commands.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/timeseries/info.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/timeseries/info.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/timeseries/info.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/timeseries/info.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/timeseries/utils.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/timeseries/utils.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/redis/commands/timeseries/utils.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/redis/commands/timeseries/utils.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/__main__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/__main__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/__main__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/__main__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_cell_widths.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_cell_widths.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_cell_widths.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_cell_widths.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_emoji_codes.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_emoji_codes.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_emoji_codes.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_emoji_codes.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_emoji_replace.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_emoji_replace.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_emoji_replace.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_emoji_replace.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_export_format.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_export_format.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_export_format.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_export_format.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_extension.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_extension.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_extension.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_extension.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_fileno.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_fileno.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_fileno.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_fileno.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_log_render.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_log_render.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_log_render.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_log_render.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_loop.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_loop.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_loop.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_loop.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_null_file.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_null_file.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_null_file.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_null_file.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_palettes.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_palettes.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_palettes.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_palettes.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_pick.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_pick.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_pick.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_pick.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_ratio.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_ratio.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_ratio.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_ratio.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_spinners.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_spinners.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_spinners.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_spinners.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_stack.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_stack.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_stack.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_stack.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_timer.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_timer.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_timer.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_timer.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_win32_console.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_win32_console.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_win32_console.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_win32_console.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_windows.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_windows.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_windows.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_windows.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_windows_renderer.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_windows_renderer.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_windows_renderer.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_windows_renderer.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_wrap.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_wrap.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/_wrap.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/_wrap.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/abc.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/abc.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/align.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/align.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/align.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/align.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/ansi.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/ansi.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/ansi.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/ansi.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/box.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/box.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/box.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/box.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/cells.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/cells.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/cells.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/cells.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/color.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/color.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/color.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/color.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/color_triplet.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/color_triplet.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/color_triplet.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/color_triplet.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/columns.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/columns.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/columns.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/columns.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/console.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/console.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/console.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/console.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/constrain.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/constrain.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/constrain.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/constrain.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/containers.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/containers.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/containers.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/containers.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/control.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/control.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/control.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/control.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/default_styles.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/default_styles.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/default_styles.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/default_styles.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/emoji.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/emoji.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/emoji.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/emoji.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/errors.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/errors.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/errors.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/errors.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/file_proxy.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/file_proxy.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/file_proxy.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/file_proxy.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/highlighter.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/highlighter.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/highlighter.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/highlighter.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/json.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/json.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/json.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/json.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/jupyter.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/jupyter.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/jupyter.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/jupyter.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/live.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/live.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/live.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/live.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/live_render.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/live_render.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/live_render.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/live_render.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/markdown.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/markdown.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/markdown.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/markdown.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/markup.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/markup.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/markup.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/markup.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/measure.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/measure.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/measure.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/measure.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/padding.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/padding.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/padding.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/padding.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/pager.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/pager.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/pager.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/pager.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/palette.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/palette.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/palette.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/palette.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/panel.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/panel.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/panel.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/panel.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/pretty.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/pretty.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/pretty.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/pretty.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/protocol.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/protocol.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/protocol.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/protocol.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/region.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/region.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/region.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/region.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/repr.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/repr.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/repr.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/repr.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/rule.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/rule.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/rule.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/rule.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/scope.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/scope.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/scope.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/scope.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/screen.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/screen.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/screen.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/screen.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/segment.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/segment.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/segment.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/segment.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/spinner.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/spinner.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/spinner.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/spinner.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/status.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/status.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/status.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/status.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/style.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/style.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/style.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/style.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/styled.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/styled.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/styled.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/styled.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/syntax.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/syntax.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/syntax.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/syntax.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/table.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/table.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/table.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/table.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/terminal_theme.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/terminal_theme.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/terminal_theme.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/terminal_theme.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/text.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/text.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/text.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/text.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/theme.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/theme.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/theme.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/theme.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/themes.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/themes.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/themes.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/themes.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/traceback.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/traceback.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/rich/traceback.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/rich/traceback.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/sqlite3/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/sqlite3/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/sqlite3/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/sqlite3/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/sqlite3/dbapi2.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/sqlite3/dbapi2.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/sqlite3/dbapi2.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/sqlite3/dbapi2.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/src/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/src/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/src/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/src/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/src/typedal/__about__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/src/typedal/__about__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/src/typedal/__about__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/src/typedal/__about__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/src/typedal/config.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/src/typedal/config.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/src/typedal/config.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/src/typedal/config.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/su6/__about__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/su6/__about__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/su6/__about__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/su6/__about__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/su6/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/su6/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/su6/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/su6/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/su6/cli.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/su6/cli.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/su6/cli.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/su6/cli.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/su6/core.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/su6/core.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/su6/core.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/su6/core.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/su6/plugins.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/su6/plugins.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/su6/plugins.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/su6/plugins.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/sys/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/sys/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/sys/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/sys/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tabulate/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tabulate/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tabulate/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tabulate/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tabulate/version.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tabulate/version.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tabulate/version.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tabulate/version.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tests/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tests/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tests/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tests/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomli/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomli/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomli/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomli/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomli/_parser.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomli/_parser.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomli/_parser.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomli/_parser.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomli/_re.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomli/_re.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomli/_re.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomli/_re.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomli/_types.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomli/_types.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomli/_types.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomli/_types.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomli_w/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomli_w/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomli_w/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomli_w/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomli_w/_writer.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomli_w/_writer.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomli_w/_writer.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomli_w/_writer.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/_compat.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/_compat.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/_compat.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/_types.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/_types.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/_types.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/_types.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/_utils.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/_utils.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/_utils.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/_utils.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/api.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/api.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/api.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/api.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/container.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/container.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/container.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/container.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/exceptions.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/exceptions.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/items.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/items.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/items.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/items.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/parser.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/parser.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/parser.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/parser.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/source.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/source.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/source.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/source.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/toml_char.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/toml_char.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/toml_char.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/toml_char.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/toml_document.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/toml_document.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/tomlkit/toml_document.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/tomlkit/toml_document.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typedal/__about__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typedal/__about__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typedal/__about__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typedal/__about__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typedal/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typedal/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typedal/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typedal/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typedal/caching.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typedal/caching.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typedal/caching.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typedal/caching.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typedal/cli.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typedal/cli.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typedal/cli.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typedal/cli.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typedal/config.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typedal/config.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typedal/config.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typedal/config.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typedal/core.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typedal/core.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typedal/core.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typedal/core.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typedal/fields.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typedal/fields.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typedal/fields.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typedal/fields.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typedal/for_py4web.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typedal/for_py4web.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typedal/for_py4web.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typedal/for_py4web.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typedal/for_web2py.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typedal/for_web2py.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typedal/for_web2py.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typedal/for_web2py.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typedal/helpers.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typedal/helpers.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typedal/helpers.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typedal/helpers.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typedal/serializers.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typedal/serializers.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typedal/serializers.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typedal/serializers.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typedal/types.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typedal/types.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typedal/types.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typedal/types.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typedal/web2py_py4web_shared.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typedal/web2py_py4web_shared.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typedal/web2py_py4web_shared.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typedal/web2py_py4web_shared.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typedal/serializers/as_json.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typedal/serializers/as_json.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typedal/serializers/as_json.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typedal/serializers/as_json.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typeguard/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typeguard/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typeguard/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typeguard/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_checkers.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_checkers.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_checkers.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_checkers.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_config.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_config.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_config.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_config.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_decorators.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_decorators.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_decorators.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_decorators.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_exceptions.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_exceptions.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_exceptions.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_functions.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_functions.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_functions.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_functions.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_importhook.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_importhook.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_importhook.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_importhook.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_memo.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_memo.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_memo.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_memo.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_suppression.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_suppression.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_suppression.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_suppression.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_transformer.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_transformer.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_transformer.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_transformer.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_utils.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_utils.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typeguard/_utils.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typeguard/_utils.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typer/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typer/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typer/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typer/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typer/_compat_utils.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typer/_compat_utils.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typer/_compat_utils.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typer/_compat_utils.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typer/_completion_shared.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typer/_completion_shared.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typer/_completion_shared.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typer/_completion_shared.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typer/_typing.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typer/_typing.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typer/_typing.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typer/_typing.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typer/colors.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typer/colors.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typer/colors.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typer/colors.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typer/completion.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typer/completion.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typer/completion.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typer/completion.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typer/core.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typer/core.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typer/core.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typer/core.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typer/main.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typer/main.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typer/main.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typer/main.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typer/models.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typer/models.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typer/models.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typer/models.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typer/params.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typer/params.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typer/params.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typer/params.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typer/rich_utils.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typer/rich_utils.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typer/rich_utils.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typer/rich_utils.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typer/utils.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typer/utils.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/typer/utils.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/typer/utils.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/unittest/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/unittest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/unittest/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/unittest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/unittest/_log.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/unittest/_log.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/unittest/_log.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/unittest/_log.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/unittest/async_case.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/unittest/async_case.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/unittest/async_case.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/unittest/async_case.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/unittest/case.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/unittest/case.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/unittest/case.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/unittest/case.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/unittest/loader.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/unittest/loader.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/unittest/loader.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/unittest/loader.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/unittest/main.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/unittest/main.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/unittest/main.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/unittest/main.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/unittest/mock.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/unittest/mock.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/unittest/mock.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/unittest/mock.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/unittest/result.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/unittest/result.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/unittest/result.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/unittest/result.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/unittest/runner.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/unittest/runner.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/unittest/runner.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/unittest/runner.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/unittest/signals.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/unittest/signals.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/unittest/signals.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/unittest/signals.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/unittest/suite.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/unittest/suite.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/unittest/suite.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/unittest/suite.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/urllib/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/urllib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/urllib/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/urllib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/urllib/error.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/urllib/error.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/urllib/error.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/urllib/error.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/urllib/parse.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/urllib/parse.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/urllib/parse.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/urllib/parse.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/urllib/request.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/urllib/request.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/urllib/request.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/urllib/request.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/urllib/response.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/urllib/response.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/urllib/response.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/urllib/response.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/witchery/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/witchery/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/witchery/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/witchery/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/xml/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/xml/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/xml/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/xml/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/xml/dom/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/xml/dom/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/xml/dom/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/xml/dom/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/xml/dom/domreg.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/xml/dom/domreg.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/xml/dom/domreg.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/xml/dom/domreg.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/xml/dom/expatbuilder.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/xml/dom/expatbuilder.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/xml/dom/expatbuilder.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/xml/dom/expatbuilder.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/xml/dom/minicompat.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/xml/dom/minicompat.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/xml/dom/minicompat.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/xml/dom/minicompat.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/xml/dom/minidom.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/xml/dom/minidom.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/xml/dom/minidom.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/xml/dom/minidom.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/xml/dom/xmlbuilder.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/xml/dom/xmlbuilder.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/xml/dom/xmlbuilder.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/xml/dom/xmlbuilder.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/xml/parsers/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/xml/parsers/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/xml/parsers/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/xml/parsers/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/xml/parsers/expat/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/xml/parsers/expat/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/xml/parsers/expat/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/xml/parsers/expat/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/xml/sax/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/xml/sax/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/xml/sax/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/xml/sax/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/xml/sax/handler.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/xml/sax/handler.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/xml/sax/handler.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/xml/sax/handler.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/xml/sax/xmlreader.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/xml/sax/xmlreader.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/xml/sax/xmlreader.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/xml/sax/xmlreader.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/__init__.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/__init__.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/_yaml.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/_yaml.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/_yaml.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/_yaml.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/composer.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/composer.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/composer.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/composer.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/constructor.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/constructor.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/constructor.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/constructor.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/cyaml.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/cyaml.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/cyaml.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/cyaml.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/dumper.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/dumper.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/dumper.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/dumper.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/emitter.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/emitter.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/emitter.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/emitter.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/error.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/error.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/error.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/error.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/events.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/events.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/events.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/events.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/loader.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/loader.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/loader.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/loader.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/nodes.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/nodes.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/nodes.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/nodes.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/parser.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/parser.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/parser.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/parser.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/reader.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/reader.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/reader.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/reader.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/representer.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/representer.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/representer.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/representer.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/resolver.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/resolver.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/resolver.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/resolver.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/scanner.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/scanner.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/scanner.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/scanner.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/serializer.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/serializer.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/serializer.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/serializer.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/tokens.data.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/tokens.data.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.mypy_cache/3.11/yaml/tokens.meta.json` & `typedal-3.0.0b4/.mypy_cache/3.11/yaml/tokens.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.pytest_cache/v/cache/nodeids` & `typedal-3.0.0b4/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.ruff_cache/0.1.14/15432600919105507093` & `typedal-3.0.0b4/.ruff_cache/0.1.14/15432600919105507093`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.ruff_cache/0.1.6/2759713849472344579` & `typedal-3.0.0b4/.ruff_cache/0.1.6/2759713849472344579`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.ruff_cache/0.1.7/3401287376304810316` & `typedal-3.0.0b4/.ruff_cache/0.1.7/3401287376304810316`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.ruff_cache/content/14855161046259211094` & `typedal-3.0.0b4/.ruff_cache/content/14855161046259211094`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.ruff_cache/content/1b34455c399f0006` & `typedal-3.0.0b4/.ruff_cache/content/1b34455c399f0006`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.ruff_cache/content/20585cf790eae81e` & `typedal-3.0.0b4/.ruff_cache/content/20585cf790eae81e`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.ruff_cache/content/217892307344966949` & `typedal-3.0.0b4/.ruff_cache/content/217892307344966949`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.ruff_cache/content/221af82ae72a7f27` & `typedal-3.0.0b4/.ruff_cache/content/221af82ae72a7f27`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.ruff_cache/content/24e1b4aab386ebc8` & `typedal-3.0.0b4/.ruff_cache/content/24e1b4aab386ebc8`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.ruff_cache/content/2f3396c610fd7095` & `typedal-3.0.0b4/.ruff_cache/content/2f3396c610fd7095`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.ruff_cache/content/322af04e6d059ce5` & `typedal-3.0.0b4/.ruff_cache/content/322af04e6d059ce5`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.ruff_cache/content/3826106cf4494de8` & `typedal-3.0.0b4/.ruff_cache/content/3826106cf4494de8`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.ruff_cache/content/38d5fd55b14a9d6c` & `typedal-3.0.0b4/.ruff_cache/content/38d5fd55b14a9d6c`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.ruff_cache/content/4022ee8774ccd98a` & `typedal-3.0.0b4/.ruff_cache/content/4022ee8774ccd98a`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.ruff_cache/content/5491563776466765346` & `typedal-3.0.0b4/.ruff_cache/content/5491563776466765346`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.ruff_cache/content/75bd1769f6e29ed7` & `typedal-3.0.0b4/.ruff_cache/content/75bd1769f6e29ed7`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.ruff_cache/content/a0739889bf9412e8` & `typedal-3.0.0b4/.ruff_cache/content/a0739889bf9412e8`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.ruff_cache/content/a225e4df39be9b29` & `typedal-3.0.0b4/.ruff_cache/content/a225e4df39be9b29`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.ruff_cache/content/b419496fa9e72887` & `typedal-3.0.0b4/.ruff_cache/content/b419496fa9e72887`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.ruff_cache/content/bdcdf5c7bbc1d738` & `typedal-3.0.0b4/.ruff_cache/content/bdcdf5c7bbc1d738`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.ruff_cache/content/c06de16f3c7a64cc` & `typedal-3.0.0b4/.ruff_cache/content/c06de16f3c7a64cc`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.ruff_cache/content/cdfecbca581311ee` & `typedal-3.0.0b4/.ruff_cache/content/cdfecbca581311ee`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.ruff_cache/content/da4811a7730a562a` & `typedal-3.0.0b4/.ruff_cache/content/da4811a7730a562a`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/.ruff_cache/content/eee2f3c667de6c7a` & `typedal-3.0.0b4/.ruff_cache/content/eee2f3c667de6c7a`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/docs/1_getting_started.md` & `typedal-3.0.0b4/docs/1_getting_started.md`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/docs/2_defining_tables.md` & `typedal-3.0.0b4/docs/2_defining_tables.md`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/docs/3_building_queries.md` & `typedal-3.0.0b4/docs/3_building_queries.md`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/docs/4_relationships.md` & `typedal-3.0.0b4/docs/4_relationships.md`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/docs/5_py4web.md` & `typedal-3.0.0b4/docs/5_py4web.md`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/docs/6_migrations.md` & `typedal-3.0.0b4/docs/6_migrations.md`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/htmlcov/coverage_html.js` & `typedal-3.0.0b4/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/htmlcov/d_0ccc93afd6526b6c___about___py.html` & `typedal-3.0.0b4/htmlcov/d_0ccc93afd6526b6c___about___py.html`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/htmlcov/d_0ccc93afd6526b6c___init___py.html` & `typedal-3.0.0b4/htmlcov/d_0ccc93afd6526b6c___init___py.html`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/htmlcov/d_0ccc93afd6526b6c_caching_py.html` & `typedal-3.0.0b4/htmlcov/d_0ccc93afd6526b6c_caching_py.html`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/htmlcov/d_0ccc93afd6526b6c_cli_py.html` & `typedal-3.0.0b4/htmlcov/d_0ccc93afd6526b6c_cli_py.html`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/htmlcov/d_0ccc93afd6526b6c_config_py.html` & `typedal-3.0.0b4/htmlcov/d_0ccc93afd6526b6c_config_py.html`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/htmlcov/d_0ccc93afd6526b6c_core_py.html` & `typedal-3.0.0b4/htmlcov/d_0ccc93afd6526b6c_core_py.html`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/htmlcov/d_0ccc93afd6526b6c_fields_py.html` & `typedal-3.0.0b4/htmlcov/d_0ccc93afd6526b6c_fields_py.html`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/htmlcov/d_0ccc93afd6526b6c_for_py4web_py.html` & `typedal-3.0.0b4/htmlcov/d_0ccc93afd6526b6c_for_py4web_py.html`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/htmlcov/d_0ccc93afd6526b6c_for_web2py_py.html` & `typedal-3.0.0b4/htmlcov/d_0ccc93afd6526b6c_for_web2py_py.html`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/htmlcov/d_0ccc93afd6526b6c_helpers_py.html` & `typedal-3.0.0b4/htmlcov/d_0ccc93afd6526b6c_helpers_py.html`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/htmlcov/d_0ccc93afd6526b6c_types_py.html` & `typedal-3.0.0b4/htmlcov/d_0ccc93afd6526b6c_types_py.html`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/htmlcov/d_0ccc93afd6526b6c_web2py_py4web_shared_py.html` & `typedal-3.0.0b4/htmlcov/d_0ccc93afd6526b6c_web2py_py4web_shared_py.html`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/htmlcov/d_18c616467159315a_as_json_py.html` & `typedal-3.0.0b4/htmlcov/d_18c616467159315a_as_json_py.html`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/htmlcov/favicon_32.png` & `typedal-3.0.0b4/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/htmlcov/index.html` & `typedal-3.0.0b4/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/htmlcov/keybd_closed.png` & `typedal-3.0.0b4/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/htmlcov/keybd_open.png` & `typedal-3.0.0b4/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/htmlcov/status.json` & `typedal-3.0.0b4/htmlcov/status.json`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/htmlcov/style.css` & `typedal-3.0.0b4/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/src/typedal/caching.py` & `typedal-3.0.0b4/src/typedal/caching.py`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/src/typedal/cli.py` & `typedal-3.0.0b4/src/typedal/cli.py`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/src/typedal/config.py` & `typedal-3.0.0b4/src/typedal/config.py`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/src/typedal/core.py` & `typedal-3.0.0b4/src/typedal/core.py`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/src/typedal/fields.py` & `typedal-3.0.0b4/src/typedal/fields.py`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/src/typedal/for_py4web.py` & `typedal-3.0.0b4/src/typedal/for_py4web.py`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/src/typedal/for_web2py.py` & `typedal-3.0.0b4/src/typedal/for_web2py.py`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/src/typedal/helpers.py` & `typedal-3.0.0b4/src/typedal/helpers.py`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/src/typedal/types.py` & `typedal-3.0.0b4/src/typedal/types.py`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/src/typedal/web2py_py4web_shared.py` & `typedal-3.0.0b4/src/typedal/web2py_py4web_shared.py`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/src/typedal/serializers/as_json.py` & `typedal-3.0.0b4/src/typedal/serializers/as_json.py`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/tests/test_cli.py` & `typedal-3.0.0b4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/tests/test_config.py` & `typedal-3.0.0b4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/tests/test_docs_examples.py` & `typedal-3.0.0b4/tests/test_docs_examples.py`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/tests/test_helpers.py` & `typedal-3.0.0b4/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/tests/test_json.py` & `typedal-3.0.0b4/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/tests/test_main.py` & `typedal-3.0.0b4/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/tests/test_mypy.py` & `typedal-3.0.0b4/tests/test_mypy.py`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/tests/test_orm.py` & `typedal-3.0.0b4/tests/test_orm.py`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/tests/test_py4web.py` & `typedal-3.0.0b4/tests/test_py4web.py`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/tests/test_query_builder.py` & `typedal-3.0.0b4/tests/test_query_builder.py`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/tests/test_relationships.py` & `typedal-3.0.0b4/tests/test_relationships.py`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/tests/test_row.py` & `typedal-3.0.0b4/tests/test_row.py`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/tests/test_stats.py` & `typedal-3.0.0b4/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/tests/test_table.py` & `typedal-3.0.0b4/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/tests/test_web2py.py` & `typedal-3.0.0b4/tests/test_web2py.py`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/tests/test_xx_others.py` & `typedal-3.0.0b4/tests/test_xx_others.py`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/tests/timings.py` & `typedal-3.0.0b4/tests/timings.py`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/tests/configs/valid.toml` & `typedal-3.0.0b4/tests/configs/valid.toml`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/README.md` & `typedal-3.0.0b4/README.md`

 * *Files identical despite different names*

### Comparing `typedal-3.0.0b3/pyproject.toml` & `typedal-3.0.0b4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -33,25 +33,25 @@
 py4web = [
     "py4web",
 ]
 
 migrations = [
     "typer",
     "tabulate",
-    "pydal2sql",
-    "edwh-migrate",
+    "pydal2sql>=1.1.3",
+    "edwh-migrate>=0.8.0b1",
     "questionary",
     "tomlkit",
 ]
 
 all = [
     "py4web",
     "typer",
     "tabulate",
-    "pydal2sql[all]",
+    "pydal2sql[all]>=1.1.3",
     "edwh-migrate>=0.8.0b1",
     "questionary",
     "tomlkit",
 ]
 
 dev = [
     # build:
```

### Comparing `typedal-3.0.0b3/PKG-INFO` & `typedal-3.0.0b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TypeDAL
-Version: 3.0.0b3
+Version: 3.0.0b4
 Summary: Typing support for PyDAL
 Project-URL: Documentation, https://typedal.readthedocs.io/
 Project-URL: Issues, https://github.com/trialandsuccess/TypeDAL/issues
 Project-URL: Source, https://github.com/trialandsuccess/TypeDAL
 Author-email: Robin van der Noord <contact@trialandsuccess.nl>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
@@ -18,31 +18,31 @@
 Requires-Dist: configurable-json
 Requires-Dist: configuraptor>=1.26.2
 Requires-Dist: dill
 Requires-Dist: pydal
 Provides-Extra: all
 Requires-Dist: edwh-migrate>=0.8.0b1; extra == 'all'
 Requires-Dist: py4web; extra == 'all'
-Requires-Dist: pydal2sql[all]; extra == 'all'
+Requires-Dist: pydal2sql[all]>=1.1.3; extra == 'all'
 Requires-Dist: questionary; extra == 'all'
 Requires-Dist: tabulate; extra == 'all'
 Requires-Dist: tomlkit; extra == 'all'
 Requires-Dist: typer; extra == 'all'
 Provides-Extra: dev
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: mkdocs; extra == 'dev'
 Requires-Dist: mkdocs-dracula-theme; extra == 'dev'
 Requires-Dist: pytest-mypy-testing; extra == 'dev'
 Requires-Dist: python-semantic-release<8; extra == 'dev'
 Requires-Dist: su6[all]; extra == 'dev'
 Requires-Dist: types-pyyaml; extra == 'dev'
 Requires-Dist: types-tabulate; extra == 'dev'
 Provides-Extra: migrations
-Requires-Dist: edwh-migrate; extra == 'migrations'
-Requires-Dist: pydal2sql; extra == 'migrations'
+Requires-Dist: edwh-migrate>=0.8.0b1; extra == 'migrations'
+Requires-Dist: pydal2sql>=1.1.3; extra == 'migrations'
 Requires-Dist: questionary; extra == 'migrations'
 Requires-Dist: tabulate; extra == 'migrations'
 Requires-Dist: tomlkit; extra == 'migrations'
 Requires-Dist: typer; extra == 'migrations'
 Provides-Extra: py4web
 Requires-Dist: py4web; extra == 'py4web'
 Description-Content-Type: text/markdown
```

