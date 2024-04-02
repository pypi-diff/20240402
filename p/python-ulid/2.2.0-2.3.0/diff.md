# Comparing `tmp/python_ulid-2.2.0.tar.gz` & `tmp/python_ulid-2.3.0.tar.gz`

## Comparing `python_ulid-2.2.0.tar` & `python_ulid-2.3.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 python_ulid-2.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 python_ulid-2.2.0/.readthedocs.yml
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 python_ulid-2.2.0/CHANGELOG.rst
--rw-r--r--   0        0        0     4314 2020-02-02 00:00:00.000000 python_ulid-2.2.0/README.rst
--rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 python_ulid-2.2.0/logo.png
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 python_ulid-2.2.0/.github/workflows/lint-and-test.yml
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 python_ulid-2.2.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 python_ulid-2.2.0/docs/Makefile
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 python_ulid-2.2.0/docs/api.rst
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 python_ulid-2.2.0/docs/changelog.rst
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 python_ulid-2.2.0/docs/conf.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 python_ulid-2.2.0/docs/index.rst
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 python_ulid-2.2.0/docs/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_ulid-2.2.0/tests/__init__.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 python_ulid-2.2.0/tests/test_base32.py
--rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 python_ulid-2.2.0/tests/test_ulid.py
--rw-r--r--   0        0        0     7516 2020-02-02 00:00:00.000000 python_ulid-2.2.0/ulid/__init__.py
--rw-r--r--   0        0        0     5290 2020-02-02 00:00:00.000000 python_ulid-2.2.0/ulid/__main__.py
--rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 python_ulid-2.2.0/ulid/base32.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 python_ulid-2.2.0/ulid/constants.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_ulid-2.2.0/ulid/py.typed
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 python_ulid-2.2.0/.gitignore
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 python_ulid-2.2.0/LICENSE
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 python_ulid-2.2.0/hatch.toml
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 python_ulid-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 python_ulid-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 python_ulid-2.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 python_ulid-2.3.0/.readthedocs.yml
+-rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 python_ulid-2.3.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     5677 2020-02-02 00:00:00.000000 python_ulid-2.3.0/README.rst
+-rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 python_ulid-2.3.0/logo.png
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 python_ulid-2.3.0/.github/workflows/lint-and-test.yml
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 python_ulid-2.3.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 python_ulid-2.3.0/docs/Makefile
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_ulid-2.3.0/docs/requirements.txt
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 python_ulid-2.3.0/docs/source/api.rst
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 python_ulid-2.3.0/docs/source/changelog.rst
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 python_ulid-2.3.0/docs/source/conf.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 python_ulid-2.3.0/docs/source/index.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_ulid-2.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 python_ulid-2.3.0/tests/test_base32.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 python_ulid-2.3.0/tests/test_cli.py
+-rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 python_ulid-2.3.0/tests/test_ulid.py
+-rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 python_ulid-2.3.0/ulid/__init__.py
+-rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 python_ulid-2.3.0/ulid/__main__.py
+-rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 python_ulid-2.3.0/ulid/base32.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 python_ulid-2.3.0/ulid/constants.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_ulid-2.3.0/ulid/py.typed
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 python_ulid-2.3.0/.gitignore
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 python_ulid-2.3.0/LICENSE
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 python_ulid-2.3.0/hatch.toml
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 python_ulid-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 python_ulid-2.3.0/PKG-INFO
```

### Comparing `python_ulid-2.2.0/CHANGELOG.rst` & `python_ulid-2.3.0/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,29 @@
 .. _changelog:
 
 Changelog
 =========
 
 Versions follow `Semantic Versioning <http://www.semver.org>`_
 
+`2.3.0`_ - 2023-09-21
+---------------------
+
+Added
+~~~~~
+* :class:`.ULID` objects can now be converted to bytes with ``bytes(ulid)``.
+* The Pydantic v2 protocol is now supported, so that the :class:`.ULID` class can be directly used
+  as type annotations in `Pydantic models <https://docs.pydantic.dev/latest/concepts/models/#basic-model-usage>`_
+
+Changed
+~~~~~~~
+* The type annotations have been adapted, so that the classmethod constructors properly reflect the
+  type for :class:`.ULID` subclasses. Thanks to `@johnpaulett <https://github.com/johnpaulett>`_
+
+
 `2.2.0`_ - 2023-09-21
 ---------------------
 
 Added
 ~~~~~
 * Added a new flag ``--uuid4`` to the CLI ``show`` command, that converts the provided ``ULID``
   into an RFC 4122 compliant ``UUID``.
@@ -124,14 +139,15 @@
     >>> ULID().hex
     '0171caa5459a8631a6894d072c8550a8'
 
 * Equality checks and ordering now also work with ``str``-instances.
 * The package now has no external dependencies.
 * The test-coverage has been raised to 100%.
 
+.. _2.3.0: https://github.com/mdomke/python-ulid/compare/2.2.0...2.3.0
 .. _2.2.0: https://github.com/mdomke/python-ulid/compare/2.1.0...2.2.0
 .. _2.1.0: https://github.com/mdomke/python-ulid/compare/2.0.0...2.1.0
 .. _2.0.0: https://github.com/mdomke/python-ulid/compare/1.1.0...2.0.0
 .. _1.1.0: https://github.com/mdomke/python-ulid/compare/1.0.3...1.1.0
 .. _1.0.3: https://github.com/mdomke/python-ulid/compare/1.0.2...1.0.3
 .. _1.0.0: https://github.com/mdomke/python-ulid/compare/0.2.0...1.0.0
```

### Comparing `python_ulid-2.2.0/README.rst` & `python_ulid-2.3.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -65,14 +65,20 @@
 
 Use ``pip`` to install the library
 
 .. code-block:: bash
 
   $ pip install python-ulid
 
+to include Pydantic support install the optional dependency like so
+
+.. code-block:: bash
+
+  $ pip install python-ulid[pydantic]
+
 .. installation-end
 
 .. usage-begin
 
 Basic Usage
 -----------
 
@@ -90,32 +96,64 @@
 
    >>> import time, datetime
    >>> ULID.from_timestamp(time.time())
    ULID(01E75J1MKKWMGG0N5MBHFMRC84)
    >>> ULID.from_datetime(datetime.datetime.now())
    ULID(01E75J2XBK390V2XRH44EHC10X)
 
-There are several options for encoding the ``ULID`` object (e.g. string, hex, int),
-as well as to access the timestamp attribute in different formats:
+There are several options for encoding the ``ULID`` object
+(e.g. string, hex, int, bytes, UUID):
 
 .. code-block:: pycon
 
    >>> str(ulid)
    '01BTGNYV6HRNK8K8VKZASZCFPE'
    >>> ulid.hex
    '015ea15f6cd1c56689a373fab3f63ece'
+   >>> int(ulid)
+   1820576928786795198723644692628913870
+   >>> bytes(ulid)
+   b'\x01^\xa1_l\xd1\xc5f\x89\xa3s\xfa\xb3\xf6>\xce'
+   >>> ulid.to_uuid()
+   UUID('015ea15f-6cd1-c566-89a3-73fab3f63ece')
+
+It is also possible to directly access the timestamp component of a ``ULID``,
+either in UNIX epoch or as ``datetime.datetime``
+
+.. code-block:: pycon
+
    >>> ulid.timestamp
    1505945939.153
    >>> ulid.datetime
    datetime.datetime(2017, 9, 20, 22, 18, 59, 153000, tzinfo=datetime.timezone.utc)
-   >>> ulid.to_uuid()
-   UUID('015ea15f-6cd1-c566-89a3-73fab3f63ece')
 
 .. usage-end
 
+.. pydantic-begin
+
+Pydantic integration
+---------------------
+
+The ``ULID`` class can be directly used for the popular data validation library
+`Pydantic <https://docs.pydantic.dev/latest/>`_ like so
+
+.. code-block:: python
+
+  from pydantic import BaseModel
+  from ulid import ULID
+
+
+  class Model(BaseModel):
+    ulid: ULID
+
+  model = Model(ulid="DX89370400440532013000")  # OK
+  model = Model(ulid="not-a-ulid")  # Raises ValidationError
+
+.. pydantic-end
+
 .. cli-begin
 
 Command line interface
 -----------------------
 
 The package comes with a CLI interface that can be invoked either by the script name
 ``ulid`` or as python module ``python -m ulid``. The CLI allows you to generate, inspect
@@ -132,25 +170,40 @@
    $ ulid show 01HASFKBN8SKZTSVVS03K5AMMS
    ULID:      01HASFKBN8SKZTSVVS03K5AMMS
    Hex:       018ab2f9aea8ccffacef7900e6555299
    Int:       2049395013039097460549394558635823769
    Timestamp: 1695219822.248
    Datetime:  2023-09-20 14:23:42.248000+00:00
 
+There are several flags to select specific output formats for the ``show`` command, e.g.
+
+
+.. code-block:: bash
+
+   $ ulid show --datetime 01HASFKBN8SKZTSVVS03K5AMMS
+   2023-09-20 14:23:42.248000+00:00
+
 The special character ``-`` allows to read values from ``stdin`` so that they can be piped. E.g.
 
 .. code-block:: bash
 
    $ echo 01HASFKBN8SKZTSVVS03K5AMMS | ulid show --uuid -
    018ab2f9-aea8-4cff-acef-7900e6555299
 
    $ date --iso-8601 | python -m ulid build --from-datetime -
    01HAT9PVR02T3S13XB48S7GEHE
 
+For a full overview of flags for the ``build`` and ``show`` commands use the ``--help`` option
+(e.g. ``ulid show --help``).
+
 .. cli-end
 
 Other implementations
 ---------------------
 
 * `ahawker/ulid <https://github.com/ahawker/ulid>`_
 * `valohai/ulid2 <https://github.com/valohai/ulid2>`_
 * `mdipierro/ulid <https://github.com/mdipierro/ulid>`_
+* `oklog/ulid <https://github.com/oklog/ulid>`_
+* `ulid/javascript <https://github.com/ulid/javascript>`_
+* `RobThree/NUlid <https://github.com/RobThree/NUlid>`_
+* `imdario/go-ulid <https://github.com/imdario/go-ulid>`_
```

#### html2text {}

```diff
@@ -16,36 +16,55 @@
 UUID * Uses Crockford's base32 for better efficiency and readability (5 bits
 per character) * Case insensitive * No special characters (URL safe) In general
 the structure of a ULID is as follows: .. code-block:: text 01AN4Z07BY
 79KA1307SR9X4MV3 |----------| |----------------| Timestamp Randomness 48bits
 80bits For more information have a look at the original `specification
 github.com/alizain/ulid#specification>`_. .. teaser-end .. installation-begin
 Installation ------------ Use ``pip`` to install the library .. code-block::
-bash $ pip install python-ulid .. installation-end .. usage-begin Basic Usage -
----------- Create a new ``ULID`` object from the current timestamp .. code-
-block:: pycon >>> from ulid import ULID >>> ULID() ULID
-(01E75HZVW36EAZKMF1W7XNMSB4) or use one of the named constructors .. code-
-block:: pycon >>> import time, datetime >>> ULID.from_timestamp(time.time())
-ULID(01E75J1MKKWMGG0N5MBHFMRC84) >>> ULID.from_datetime(datetime.datetime.now
-()) ULID(01E75J2XBK390V2XRH44EHC10X) There are several options for encoding the
-``ULID`` object (e.g. string, hex, int), as well as to access the timestamp
-attribute in different formats: .. code-block:: pycon >>> str(ulid)
+bash $ pip install python-ulid to include Pydantic support install the optional
+dependency like so .. code-block:: bash $ pip install python-ulid[pydantic] ..
+installation-end .. usage-begin Basic Usage ----------- Create a new ``ULID``
+object from the current timestamp .. code-block:: pycon >>> from ulid import
+ULID >>> ULID() ULID(01E75HZVW36EAZKMF1W7XNMSB4) or use one of the named
+constructors .. code-block:: pycon >>> import time, datetime >>>
+ULID.from_timestamp(time.time()) ULID(01E75J1MKKWMGG0N5MBHFMRC84) >>>
+ULID.from_datetime(datetime.datetime.now()) ULID(01E75J2XBK390V2XRH44EHC10X)
+There are several options for encoding the ``ULID`` object (e.g. string, hex,
+int, bytes, UUID): .. code-block:: pycon >>> str(ulid)
 '01BTGNYV6HRNK8K8VKZASZCFPE' >>> ulid.hex '015ea15f6cd1c56689a373fab3f63ece'
->>> ulid.timestamp 1505945939.153 >>> ulid.datetime datetime.datetime(2017, 9,
-20, 22, 18, 59, 153000, tzinfo=datetime.timezone.utc) >>> ulid.to_uuid() UUID
-('015ea15f-6cd1-c566-89a3-73fab3f63ece') .. usage-end .. cli-begin Command line
-interface ----------------------- The package comes with a CLI interface that
-can be invoked either by the script name ``ulid`` or as python module ``python
--m ulid``. The CLI allows you to generate, inspect and convert ULIDs, e.g. ..
-code-block:: bash $ ulid build 01HASFKBN8SKZTSVVS03K5AMMS $ ulid build --from-
-datetime=2023-09-23T10:20:30 01HB0J0F5GCKEXNSWVAD5PEAC1 $ ulid show
+>>> int(ulid) 1820576928786795198723644692628913870 >>> bytes(ulid)
+b'\x01^\xa1_l\xd1\xc5f\x89\xa3s\xfa\xb3\xf6>\xce' >>> ulid.to_uuid() UUID
+('015ea15f-6cd1-c566-89a3-73fab3f63ece') It is also possible to directly access
+the timestamp component of a ``ULID``, either in UNIX epoch or as
+``datetime.datetime`` .. code-block:: pycon >>> ulid.timestamp 1505945939.153
+>>> ulid.datetime datetime.datetime(2017, 9, 20, 22, 18, 59, 153000,
+tzinfo=datetime.timezone.utc) .. usage-end .. pydantic-begin Pydantic
+integration --------------------- The ``ULID`` class can be directly used for
+the popular data validation library `Pydantic
+docs.pydantic.dev/latest/>`_ like so .. code-block:: python from pydantic
+import BaseModel from ulid import ULID class Model(BaseModel): ulid: ULID model
+= Model(ulid="DX89370400440532013000") # OK model = Model(ulid="not-a-ulid") #
+Raises ValidationError .. pydantic-end .. cli-begin Command line interface ----
+------------------- The package comes with a CLI interface that can be invoked
+either by the script name ``ulid`` or as python module ``python -m ulid``. The
+CLI allows you to generate, inspect and convert ULIDs, e.g. .. code-block::
+bash $ ulid build 01HASFKBN8SKZTSVVS03K5AMMS $ ulid build --from-datetime=2023-
+09-23T10:20:30 01HB0J0F5GCKEXNSWVAD5PEAC1 $ ulid show
 01HASFKBN8SKZTSVVS03K5AMMS ULID: 01HASFKBN8SKZTSVVS03K5AMMS Hex:
 018ab2f9aea8ccffacef7900e6555299 Int: 2049395013039097460549394558635823769
-Timestamp: 1695219822.248 Datetime: 2023-09-20 14:23:42.248000+00:00 The
-special character ``-`` allows to read values from ``stdin`` so that they can
-be piped. E.g. .. code-block:: bash $ echo 01HASFKBN8SKZTSVVS03K5AMMS | ulid
-show --uuid - 018ab2f9-aea8-4cff-acef-7900e6555299 $ date --iso-8601 | python -
-m ulid build --from-datetime - 01HAT9PVR02T3S13XB48S7GEHE .. cli-end Other
-implementations --------------------- * `ahawker/ulid
+Timestamp: 1695219822.248 Datetime: 2023-09-20 14:23:42.248000+00:00 There are
+several flags to select specific output formats for the ``show`` command, e.g.
+.. code-block:: bash $ ulid show --datetime 01HASFKBN8SKZTSVVS03K5AMMS 2023-09-
+20 14:23:42.248000+00:00 The special character ``-`` allows to read values from
+``stdin`` so that they can be piped. E.g. .. code-block:: bash $ echo
+01HASFKBN8SKZTSVVS03K5AMMS | ulid show --uuid - 018ab2f9-aea8-4cff-acef-
+7900e6555299 $ date --iso-8601 | python -m ulid build --from-datetime -
+01HAT9PVR02T3S13XB48S7GEHE For a full overview of flags for the ``build`` and
+``show`` commands use the ``--help`` option (e.g. ``ulid show --help``). ..
+cli-end Other implementations --------------------- * `ahawker/ulid
 github.com/ahawker/ulid>`_ * `valohai/ulid2
 github.com/valohai/ulid2>`_ * `mdipierro/ulid
-github.com/mdipierro/ulid>`_
+github.com/mdipierro/ulid>`_ * `oklog/ulid
+github.com/oklog/ulid>`_ * `ulid/javascript
+github.com/ulid/javascript>`_ * `RobThree/NUlid
+github.com/RobThree/NUlid>`_ * `imdario/go-ulid
+github.com/imdario/go-ulid>`_
```

### Comparing `python_ulid-2.2.0/logo.png` & `python_ulid-2.3.0/logo.png`

 * *Files identical despite different names*

### Comparing `python_ulid-2.2.0/.github/workflows/lint-and-test.yml` & `python_ulid-2.3.0/.github/workflows/lint-and-test.yml`

 * *Files 19% similar despite different names*

```diff
@@ -5,55 +5,68 @@
     branches: [main]
   pull_request:
     branches: [main]
 
 jobs:
   lint-code:
     runs-on: ubuntu-latest
+    name: Lint code
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
-          python-version: "3.11"
+          python-version: "3.12"
       - name: Install dependencies
         run: |
           pip install hatch
           pip install hatch-vcs
           pip install hatch-fancy-pypi-readme
       - name: Lint code
         run: hatch run lint:style
 
   lint-typing:
     runs-on: ubuntu-latest
+    name: Lint type annotations
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
-          python-version: "3.11"
+          python-version: "3.12"
       - name: Install dependencies
         run: |
           pip install hatch
           pip install hatch-vcs
           pip install hatch-fancy-pypi-readme
       - name: Lint typing
         run: hatch run lint:typing
 
   test:
     runs-on: ubuntu-latest
+    name: Run tests
     strategy:
       matrix:
-        python-version: ["3.9", "3.10", "3.11"]
+        python-version: ["3.9", "3.10", "3.11", "3.12"]
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           pip install hatch
           pip install hatch-vcs
           pip install hatch-fancy-pypi-readme
       - name: Test
         run: hatch run cov-test
+      - uses: codecov/codecov-action@v4
+        with:
+          token: ${{ secrets.CODECOV_TOKEN }}
+
+  package:
+    name: Build & verify package
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v4
+      - uses: hynek/build-and-inspect-python-package@v2
```

### Comparing `python_ulid-2.2.0/.github/workflows/publish.yml` & `python_ulid-2.3.0/.github/workflows/publish.yml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 jobs:
   deploy:
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.x"
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install hatch
           pip install hatch-vcs
```

### Comparing `python_ulid-2.2.0/docs/Makefile` & `python_ulid-2.3.0/docs/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Minimal makefile for Sphinx documentation
 #
 
 # You can set these variables from the command line, and also
 # from the environment for the first two.
 SPHINXOPTS    ?=
 SPHINXBUILD   ?= sphinx-build
-SOURCEDIR     = .
-BUILDDIR      = _build
+SOURCEDIR     = source
+BUILDDIR      = build
 
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
 .PHONY: help Makefile
```

### Comparing `python_ulid-2.2.0/docs/conf.py` & `python_ulid-2.3.0/docs/source/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 from datetime import datetime
 
 
-sys.path.insert(0, os.path.abspath(".."))
+sys.path.insert(0, os.path.abspath("../.."))
 
-import ulid  # noqa
+import ulid
 
 
 copyright = f"{datetime.now().year}, Martin Domke"
 author = "Martin Domke"
 master_doc = "index"
 source_suffix = [".rst", ".md"]
 
@@ -20,39 +20,33 @@
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.napoleon",
     "sphinx.ext.viewcode",
+    "sphinx_copybutton",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
-exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
+exclude_patterns = []
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_logo = "../logo.png"
+html_logo = "../../logo.png"
 html_theme = "furo"
-html_theme_options = {
-    "github_user": "mdomke",
-    "github_repo": "python-ulid",
-    "description": "A library for working with ULIDs",
-    "sidebar_collapse": False,
-    "logo_text_align": "center",
-}
 
 html_title = "Python ULID docs"
 
 # If false, no index is generated.
 html_use_index = True
 
 # If true, the index is split into individual pages for each letter.
```

### Comparing `python_ulid-2.2.0/docs/index.rst` & `python_ulid-2.3.0/docs/source/index.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Python ULID
 ===========
 
 Release v\ |release| (:ref:`What's new <changelog>`)
 
 
-.. include:: ../README.rst
+.. include:: ../../README.rst
    :start-after: teaser-begin
    :end-before: teaser-end
 
-.. include:: ../README.rst
+.. include:: ../../README.rst
    :start-after: installation-begin
    :end-before: installation-end
 
-.. include:: ../README.rst
+.. include:: ../../README.rst
    :start-after: usage-begin
    :end-before: usage-end
 
-.. include:: ../README.rst
+.. include:: ../../README.rst
+   :start-after: pydantic-begin
+   :end-before: pydantic-end
+
+.. include:: ../../README.rst
    :start-after: cli-begin
    :end-before: cli-end
 
 API documentation
 -----------------
 
 .. toctree::
```

### Comparing `python_ulid-2.2.0/tests/test_base32.py` & `python_ulid-2.3.0/tests/test_base32.py`

 * *Files identical despite different names*

### Comparing `python_ulid-2.2.0/tests/test_ulid.py` & `python_ulid-2.3.0/tests/test_ulid.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from datetime import datetime
 from datetime import timedelta
 from datetime import timezone
 from typing import Union
 
 import pytest
 from freezegun import freeze_time
+from pydantic import BaseModel
+from pydantic import ValidationError
 
 from ulid import base32
 from ulid import constants
 from ulid import ULID
 
 
 def utcnow() -> datetime:
@@ -111,25 +113,29 @@
     assert hash(ulid1) == hash(ULID.from_bytes(ulid1.bytes))
     assert hash(ulid1) != hash(ulid2)
 
 
 @freeze_time()
 def test_ulid_from_time() -> None:
     ulid1 = ULID.from_timestamp(time.time())
-    ulid2 = ULID.from_datetime(utcnow())
+    ulid2 = ULID.from_timestamp(time.time_ns() // 1000000)
+    ulid3 = ULID.from_datetime(utcnow())
 
     now = utcnow()
     t = time.time()
 
     assert ulid1.timestamp == pytest.approx(t)
     datetimes_almost_equal(ulid1.datetime, now)
 
     assert ulid2.timestamp == pytest.approx(t)
     datetimes_almost_equal(ulid2.datetime, now)
 
+    assert ulid2.timestamp == pytest.approx(t)
+    datetimes_almost_equal(ulid3.datetime, now)
+
 
 @freeze_time()
 def test_ulid_from_timestamp() -> None:
     t = time.time()
     ulid1 = ULID.from_timestamp(t)
     ulid2 = ULID.from_timestamp(int(t * constants.MILLISECS_IN_SECS))
     assert ulid1.timestamp == ulid2.timestamp
@@ -151,7 +157,23 @@
         (ULID.from_int, "not-an-int"),
         (ULID.from_uuid, "not-a-uuid"),
     ],
 )
 def test_ulid_invalid_input(constructor: Callable[[Params], ULID], value: Params) -> None:
     with pytest.raises(ValueError):  # noqa: PT011
         constructor(value)
+
+
+def test_pydantic_protocol() -> None:
+    ulid = ULID()
+
+    class Model(BaseModel):
+        ulid: ULID
+
+    for value in [ulid, str(ulid), int(ulid), bytes(ulid)]:
+        model = Model(ulid=value)
+        assert isinstance(model.ulid, ULID)
+        assert model.ulid == ulid
+
+    for value in [b"not-enough", "not-enough"]:
+        with pytest.raises(ValidationError):
+            Model(ulid=value)
```

### Comparing `python_ulid-2.2.0/ulid/__init__.py` & `python_ulid-2.3.0/ulid/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,23 +5,29 @@
 import time
 import uuid
 from collections.abc import Callable
 from datetime import datetime
 from datetime import timezone
 from typing import Any
 from typing import Generic
+from typing import TYPE_CHECKING
 from typing import TypeVar
 
 from ulid import base32
 from ulid import constants
 
 
+if TYPE_CHECKING:  # pragma: no cover
+    from pydantic import GetCoreSchemaHandler
+    from pydantic import ValidatorFunctionWrapHandler
+    from pydantic_core import CoreSchema
+
 try:
     from importlib.metadata import version
-except ImportError:
+except ImportError:  # pragma: no cover
     from importlib_metadata import version  # type: ignore
 
 
 __version__ = version("python-ulid")
 
 
 T = TypeVar("T", bound=type)
@@ -40,14 +46,17 @@
                 message += " or ".join([t.__name__ for t in self.types])
                 raise ValueError(message)
             return func(cls, value)
 
         return wrapped
 
 
+U = TypeVar("U", bound="ULID")
+
+
 @functools.total_ordering
 class ULID:
     """The :class:`ULID` object consists of a timestamp part of 48 bits and of 80 random bits.
 
     .. code-block:: text
 
        01AN4Z07BY      79KA1307SR9X4MV3
@@ -63,33 +72,35 @@
         >>> str(ulid)
         '01E75PVKXA3GFABX1M1J9NZZNF'
     """
 
     def __init__(self, value: bytes | None = None) -> None:
         if value is not None and len(value) != constants.BYTES_LEN:
             raise ValueError("ULID has to be exactly 16 bytes long.")
-        self.bytes: bytes = value or ULID.from_timestamp(time.time()).bytes
+        self.bytes: bytes = (
+            value or ULID.from_timestamp(time.time_ns() // constants.NANOSECS_IN_MILLISECS).bytes
+        )
 
     @classmethod
     @validate_type(datetime)
-    def from_datetime(cls, value: datetime) -> ULID:
+    def from_datetime(cls: type[U], value: datetime) -> U:
         """Create a new :class:`ULID`-object from a :class:`datetime`. The timestamp part of the
         `ULID` will be set to the corresponding timestamp of the datetime.
 
         Examples:
 
             >>> from datetime import datetime
             >>> ULID.from_datetime(datetime.now())
             ULID(01E75QRYCAMM1MKQ9NYMYT6SAV)
         """
         return cls.from_timestamp(value.timestamp())
 
     @classmethod
     @validate_type(int, float)
-    def from_timestamp(cls, value: int | float) -> ULID:
+    def from_timestamp(cls: type[U], value: int | float) -> U:
         """Create a new :class:`ULID`-object from a timestamp. The timestamp can be either a
         `float` representing the time in seconds (as it would be returned by :func:`time.time()`)
         or an `int` in milliseconds.
 
         Examples:
 
             >>> import time
@@ -100,47 +111,47 @@
             value = int(value * constants.MILLISECS_IN_SECS)
         timestamp = int.to_bytes(value, constants.TIMESTAMP_LEN, "big")
         randomness = os.urandom(constants.RANDOMNESS_LEN)
         return cls.from_bytes(timestamp + randomness)
 
     @classmethod
     @validate_type(uuid.UUID)
-    def from_uuid(cls, value: uuid.UUID) -> ULID:
+    def from_uuid(cls: type[U], value: uuid.UUID) -> U:
         """Create a new :class:`ULID`-object from a :class:`uuid.UUID`. The timestamp part will be
         random in that case.
 
         Examples:
 
             >>> from uuid import uuid4
             >>> ULID.from_uuid(uuid4())
             ULID(27Q506DP7E9YNRXA0XVD8Z5YSG)
         """
         return cls(value.bytes)
 
     @classmethod
     @validate_type(bytes)
-    def from_bytes(cls, bytes_: bytes) -> ULID:
+    def from_bytes(cls: type[U], bytes_: bytes) -> U:
         """Create a new :class:`ULID`-object from sequence of 16 bytes."""
         return cls(bytes_)
 
     @classmethod
     @validate_type(str)
-    def from_hex(cls, value: str) -> ULID:
+    def from_hex(cls: type[U], value: str) -> U:
         """Create a new :class:`ULID`-object from 32 character string of hex values."""
         return cls.from_bytes(bytes.fromhex(value))
 
     @classmethod
     @validate_type(str)
-    def from_str(cls, string: str) -> ULID:
+    def from_str(cls: type[U], string: str) -> U:
         """Create a new :class:`ULID`-object from a 26 char long string representation."""
         return cls(base32.decode(string))
 
     @classmethod
     @validate_type(int)
-    def from_int(cls, value: int) -> ULID:
+    def from_int(cls: type[U], value: int) -> U:
         """Create a new :class:`ULID`-object from an `int`."""
         return cls(int.to_bytes(value, constants.BYTES_LEN, "big"))
 
     @property
     def milliseconds(self) -> int:
         """The timestamp part as epoch time in milliseconds.
 
@@ -205,14 +216,18 @@
         """Encode this object as a 26 character string sequence."""
         return base32.encode(self.bytes)
 
     def __int__(self) -> int:
         """Encode this object as an integer."""
         return int.from_bytes(self.bytes, byteorder="big")
 
+    def __bytes__(self) -> bytes:
+        """Encode this object as byte sequence."""
+        return self.bytes
+
     def __lt__(self, other: Any) -> bool:
         if isinstance(other, ULID):
             return self.bytes < other.bytes
         elif isinstance(other, int):
             return int(self) < other
         elif isinstance(other, bytes):
             return self.bytes < other
@@ -229,7 +244,38 @@
             return self.bytes == other
         elif isinstance(other, str):
             return str(self) == other
         return NotImplemented
 
     def __hash__(self) -> int:
         return hash(self.bytes)
+
+    @classmethod
+    def __get_pydantic_core_schema__(cls, source: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+        from pydantic_core import core_schema
+
+        return core_schema.no_info_wrap_validator_function(
+            cls._pydantic_validate,
+            core_schema.union_schema(
+                [
+                    core_schema.is_instance_schema(ULID),
+                    core_schema.no_info_plain_validator_function(ULID),
+                ]
+            ),
+        )
+
+    @classmethod
+    def _pydantic_validate(cls, value: Any, handler: ValidatorFunctionWrapHandler) -> Any:
+        from pydantic_core import PydanticCustomError
+
+        try:
+            if isinstance(value, int):
+                ulid = cls.from_int(value)
+            elif isinstance(value, str):
+                ulid = cls.from_str(value)
+            elif isinstance(value, ULID):
+                ulid = value
+            else:
+                ulid = cls.from_bytes(value)
+        except ValueError as err:
+            raise PydanticCustomError("ulid_format", "Unrecognized format") from err
+        return handler(ulid)
```

### Comparing `python_ulid-2.2.0/ulid/__main__.py` & `python_ulid-2.3.0/ulid/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+from __future__ import annotations
+
 import argparse
 import shutil
 import sys
 import textwrap
 from collections.abc import Callable
 from collections.abc import Sequence
 from datetime import datetime
 from functools import partial
 from typing import Any
-from typing import Optional
 from uuid import UUID
 
 import ulid
 from ulid import ULID
 
 
 def make_parser(prog: str | None = None) -> argparse.ArgumentParser:
@@ -88,34 +89,34 @@
     s.add_argument("--int", action="store_true", help="convert to int")
     s.add_argument("--timestamp", "--ts", action="store_true", help="show timestamp")
     s.add_argument("--datetime", "--dt", action="store_true", help="show datetime")
     s.set_defaults(func=show)
     return parser
 
 
-def main(argv: Sequence[str], prog: str | None = None) -> None:
+def main(argv: Sequence[str], prog: str | None = None) -> str:
     args = make_parser(prog).parse_args(argv)
-    args.func(args)
+    return args.func(args)
 
 
-def from_value_or_stdin(value: str, convert: Optional[Callable[[str], Any]] = None) -> Any:
+def from_value_or_stdin(value: str, convert: Callable[[str], Any] | None = None) -> Any:
     value = sys.stdin.readline().strip() if value == "-" else value
     if convert is not None:
         return convert(value)
     return value
 
 
 def parse_numeric(s: str) -> int | float:
     try:
         return int(s)
     except ValueError:
         return float(s)
 
 
-def build(args: argparse.Namespace) -> None:
+def build(args: argparse.Namespace) -> str:
     ulid: ULID
     if args.from_int is not None:
         ulid = ULID.from_int(from_value_or_stdin(args.from_int, int))
     elif args.from_hex is not None:
         ulid = ULID.from_hex(from_value_or_stdin(args.from_hex))
     elif args.from_str is not None:
         ulid = ULID.from_str(from_value_or_stdin(args.from_str))
@@ -123,44 +124,42 @@
         ulid = ULID.from_timestamp(from_value_or_stdin(args.from_timestamp, parse_numeric))
     elif args.from_datetime is not None:
         ulid = ULID.from_datetime(from_value_or_stdin(args.from_datetime, datetime.fromisoformat))
     elif args.from_uuid is not None:
         ulid = ULID.from_uuid(from_value_or_stdin(args.from_uuid, UUID))
     else:
         ulid = ULID()
-    print(ulid)
+    return str(ulid)
 
 
-def show(args: argparse.Namespace) -> None:
+def show(args: argparse.Namespace) -> str:
     ulid: ULID = ULID.from_str(from_value_or_stdin(args.ulid))
     if args.uuid:
-        print(ulid.to_uuid())
+        return str(ulid.to_uuid())
     elif args.uuid4:
-        print(ulid.to_uuid4())
+        return str(ulid.to_uuid4())
     elif args.hex:
-        print(ulid.hex)
+        return ulid.hex
     elif args.int:
-        print(int(ulid))
+        return str(int(ulid))
     elif args.timestamp:
-        print(ulid.timestamp)
+        return str(ulid.timestamp)
     elif args.datetime:
-        print(ulid.datetime)
+        return ulid.datetime.isoformat()
     else:
-        print(
-            textwrap.dedent(
-                f"""
-                ULID:      {ulid!s}
-                Hex:       {ulid.hex}
-                Int:       {int(ulid)}
-                Timestamp: {ulid.timestamp}
-                Datetime:  {ulid.datetime}
-                """
-            ).strip()
-        )
+        return textwrap.dedent(
+            f"""
+            ULID:      {ulid!s}
+            Hex:       {ulid.hex}
+            Int:       {int(ulid)}
+            Timestamp: {ulid.timestamp}
+            Datetime:  {ulid.datetime.isoformat()}
+            """
+        ).strip()
 
 
-def entrypoint() -> None:
-    main(sys.argv[1:])
+def entrypoint() -> None:  # pragma: no cover
+    print(main(sys.argv[1:]))
 
 
-if __name__ == "__main__":
+if __name__ == "__main__":  # pragma: no cover
     main(sys.argv[1:], "python -m ulid")
```

### Comparing `python_ulid-2.2.0/ulid/base32.py` & `python_ulid-2.3.0/ulid/base32.py`

 * *Files identical despite different names*

### Comparing `python_ulid-2.2.0/LICENSE` & `python_ulid-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_ulid-2.2.0/pyproject.toml` & `python_ulid-2.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -18,17 +18,23 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS :: MacOS X",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Software Development :: Libraries",
 ]
 
+[project.optional-dependencies]
+pydantic = [
+    "pydantic>=2.0"
+]
+
 [project.scripts]
 ulid = "ulid.__main__:entrypoint"
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.build.targets.wheel]
@@ -38,44 +44,39 @@
 
 [tool.black]
 line-length = 100
 
 [tool.ruff]
 target-version = "py39"
 line-length = 100
+
+[tool.ruff.lint]
 select = ["A", "B", "C", "C4", "E", "F", "I", "N", "PT", "Q", "RUF", "S", "SIM", "T10", "UP", "W", "YTT"]
 fixable = ["RUF100", "I001"]
 ignore = [
     "S101",   # Allow usage of asserts
     "A001",   # Allow shadowing bultins 
     "A003",   # Allow shadowing bultins on classes
 ]
 
-[tool.ruff.mccabe]
+[tool.ruff.lint.mccabe]
 max-complexity = 15
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 force-single-line = true
 lines-after-imports = 2
 order-by-type = false
 
-[tool.isort]
-profile = "black"
-force_alphabetical_sort_within_sections = true
-force_single_line = true
-lines_after_imports = 2
-line_length = 100
-
 [tool.coverage.run]
 branch = true
 parallel = true
 source = ["ulid"]
 
 [tool.doc8]
 max-line-length = 100
 
 [tool.hatch.metadata.hooks.fancy-pypi-readme]
 content-type = "text/x-rst"
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 path = "README.rst"
-start-after = ".. teaser-begin"
+start-after = ".. teaser-begin"
```

### Comparing `python_ulid-2.2.0/PKG-INFO` & `python_ulid-2.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,29 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: python-ulid
-Version: 2.2.0
+Version: 2.3.0
 Summary: Universally unique lexicographically sortable identifier
 Author-email: Martin Domke <mail@martindomke.net>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.9
+Provides-Extra: pydantic
+Requires-Dist: pydantic>=2.0; extra == 'pydantic'
 Description-Content-Type: text/x-rst
 
 
 
 A ``ULID`` is a *universally unique lexicographically sortable identifier*. It is
 
 * 128-bit compatible with ``UUID``
@@ -53,14 +56,20 @@
 
 Use ``pip`` to install the library
 
 .. code-block:: bash
 
   $ pip install python-ulid
 
+to include Pydantic support install the optional dependency like so
+
+.. code-block:: bash
+
+  $ pip install python-ulid[pydantic]
+
 .. installation-end
 
 .. usage-begin
 
 Basic Usage
 -----------
 
@@ -78,32 +87,64 @@
 
    >>> import time, datetime
    >>> ULID.from_timestamp(time.time())
    ULID(01E75J1MKKWMGG0N5MBHFMRC84)
    >>> ULID.from_datetime(datetime.datetime.now())
    ULID(01E75J2XBK390V2XRH44EHC10X)
 
-There are several options for encoding the ``ULID`` object (e.g. string, hex, int),
-as well as to access the timestamp attribute in different formats:
+There are several options for encoding the ``ULID`` object
+(e.g. string, hex, int, bytes, UUID):
 
 .. code-block:: pycon
 
    >>> str(ulid)
    '01BTGNYV6HRNK8K8VKZASZCFPE'
    >>> ulid.hex
    '015ea15f6cd1c56689a373fab3f63ece'
+   >>> int(ulid)
+   1820576928786795198723644692628913870
+   >>> bytes(ulid)
+   b'\x01^\xa1_l\xd1\xc5f\x89\xa3s\xfa\xb3\xf6>\xce'
+   >>> ulid.to_uuid()
+   UUID('015ea15f-6cd1-c566-89a3-73fab3f63ece')
+
+It is also possible to directly access the timestamp component of a ``ULID``,
+either in UNIX epoch or as ``datetime.datetime``
+
+.. code-block:: pycon
+
    >>> ulid.timestamp
    1505945939.153
    >>> ulid.datetime
    datetime.datetime(2017, 9, 20, 22, 18, 59, 153000, tzinfo=datetime.timezone.utc)
-   >>> ulid.to_uuid()
-   UUID('015ea15f-6cd1-c566-89a3-73fab3f63ece')
 
 .. usage-end
 
+.. pydantic-begin
+
+Pydantic integration
+---------------------
+
+The ``ULID`` class can be directly used for the popular data validation library
+`Pydantic <https://docs.pydantic.dev/latest/>`_ like so
+
+.. code-block:: python
+
+  from pydantic import BaseModel
+  from ulid import ULID
+
+
+  class Model(BaseModel):
+    ulid: ULID
+
+  model = Model(ulid="DX89370400440532013000")  # OK
+  model = Model(ulid="not-a-ulid")  # Raises ValidationError
+
+.. pydantic-end
+
 .. cli-begin
 
 Command line interface
 -----------------------
 
 The package comes with a CLI interface that can be invoked either by the script name
 ``ulid`` or as python module ``python -m ulid``. The CLI allows you to generate, inspect
@@ -120,25 +161,40 @@
    $ ulid show 01HASFKBN8SKZTSVVS03K5AMMS
    ULID:      01HASFKBN8SKZTSVVS03K5AMMS
    Hex:       018ab2f9aea8ccffacef7900e6555299
    Int:       2049395013039097460549394558635823769
    Timestamp: 1695219822.248
    Datetime:  2023-09-20 14:23:42.248000+00:00
 
+There are several flags to select specific output formats for the ``show`` command, e.g.
+
+
+.. code-block:: bash
+
+   $ ulid show --datetime 01HASFKBN8SKZTSVVS03K5AMMS
+   2023-09-20 14:23:42.248000+00:00
+
 The special character ``-`` allows to read values from ``stdin`` so that they can be piped. E.g.
 
 .. code-block:: bash
 
    $ echo 01HASFKBN8SKZTSVVS03K5AMMS | ulid show --uuid -
    018ab2f9-aea8-4cff-acef-7900e6555299
 
    $ date --iso-8601 | python -m ulid build --from-datetime -
    01HAT9PVR02T3S13XB48S7GEHE
 
+For a full overview of flags for the ``build`` and ``show`` commands use the ``--help`` option
+(e.g. ``ulid show --help``).
+
 .. cli-end
 
 Other implementations
 ---------------------
 
 * `ahawker/ulid <https://github.com/ahawker/ulid>`_
 * `valohai/ulid2 <https://github.com/valohai/ulid2>`_
 * `mdipierro/ulid <https://github.com/mdipierro/ulid>`_
+* `oklog/ulid <https://github.com/oklog/ulid>`_
+* `ulid/javascript <https://github.com/ulid/javascript>`_
+* `RobThree/NUlid <https://github.com/RobThree/NUlid>`_
+* `imdario/go-ulid <https://github.com/imdario/go-ulid>`_
```

