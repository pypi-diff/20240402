# Comparing `tmp/pytest_embedded_serial-1.8.1.tar.gz` & `tmp/pytest_embedded_serial-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_embedded_serial-1.8.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pytest_embedded_serial-1.8.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest_embedded_serial-1.8.1.tar` & `pytest_embedded_serial-1.8.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1094 2024-03-01 10:19:36.927475 pytest_embedded_serial-1.8.1/LICENSE
--rw-r--r--   0        0        0      195 2024-03-01 10:19:36.927475 pytest_embedded_serial-1.8.1/README.md
--rw-r--r--   0        0        0     2944 2024-03-01 10:19:36.927475 pytest_embedded_serial-1.8.1/pyproject.toml
--rw-r--r--   0        0        0      176 2024-03-01 10:19:36.927475 pytest_embedded_serial-1.8.1/pytest_embedded_serial/__init__.py
--rw-r--r--   0        0        0     1271 2024-03-01 10:19:36.931475 pytest_embedded_serial-1.8.1/pytest_embedded_serial/dut.py
--rw-r--r--   0        0        0     6113 2024-03-01 10:19:36.931475 pytest_embedded_serial-1.8.1/pytest_embedded_serial/serial.py
--rw-r--r--   0        0        0     3164 2024-03-01 10:19:36.931475 pytest_embedded_serial-1.8.1/tests/test_serial.py
--rw-r--r--   0        0        0     1549 1970-01-01 00:00:00.000000 pytest_embedded_serial-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1094 2024-04-02 08:52:22.108840 pytest_embedded_serial-1.8.2/LICENSE
+-rw-r--r--   0        0        0      195 2024-04-02 08:52:22.108840 pytest_embedded_serial-1.8.2/README.md
+-rw-r--r--   0        0        0     3293 2024-04-02 08:52:22.108840 pytest_embedded_serial-1.8.2/pyproject.toml
+-rw-r--r--   0        0        0      176 2024-04-02 08:52:22.108840 pytest_embedded_serial-1.8.2/pytest_embedded_serial/__init__.py
+-rw-r--r--   0        0        0     1271 2024-04-02 08:52:22.108840 pytest_embedded_serial-1.8.2/pytest_embedded_serial/dut.py
+-rw-r--r--   0        0        0     6184 2024-04-02 08:52:22.108840 pytest_embedded_serial-1.8.2/pytest_embedded_serial/serial.py
+-rw-r--r--   0        0        0     1653 2024-04-02 08:52:22.108840 pytest_embedded_serial-1.8.2/tests/test_serial.py
+-rw-r--r--   0        0        0     1549 1970-01-01 00:00:00.000000 pytest_embedded_serial-1.8.2/PKG-INFO
```

### Comparing `pytest_embedded_serial-1.8.1/LICENSE` & `pytest_embedded_serial-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_embedded_serial-1.8.1/pyproject.toml` & `pytest_embedded_serial-1.8.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -26,77 +26,91 @@
     "Programming Language :: Python",
     "Topic :: Software Development :: Testing",
 ]
 dynamic = ["version", "description"]
 requires-python = ">=3.7"
 
 dependencies = [
-    "pytest-embedded~=1.8.1",
+    "pytest-embedded~=1.8.2",
     "pyserial~=3.0",
 ]
 
 [project.urls]
 homepage = "https://github.com/espressif/pytest-embedded"
 repository = "https://github.com/espressif/pytest-embedded"
 documentation = "https://docs.espressif.com/projects/pytest-embedded/en/latest/"
 changelog = "https://github.com/espressif/pytest-embedded/blob/main/CHANGELOG.md"
 
 [tool.isort]
 profile = 'black'
 
-[tool.black]
+[tool.ruff]
 line-length = 120
-target-version = ['py37']
-force-exclude = '/tests/'
-skip-string-normalization = true
+target-version = "py37"
 
-[tool.ruff]
+[tool.ruff.lint]
 select = [
     'F',  # Pyflakes
     'E',  # pycodestyle
     'W',  # pycodestyle
 #    'C90',  # mccabe
-#    'I',  # isort
+    'I',  # isort
 #    'N',  # pep8-naming
 #    'D',  # pydocstyle
-#    'UP',  #  pyupgrade
-#    'YTT',  # flake8-2020
+    'UP',  # pyupgrade
+    'YTT',  # flake8-2020
 #    'ANN',  # flake8-annotations
+#    'ASYNC',  # flake8-async
+#    'TRIO',  # flake8-trio
 #    'S',  # flake8-bandit
 #    'BLE',  # flake8-blind-except
 #    'FBT',  # flake8-boolean-trap
 #    'B',  # flake8-bugbear
-#    'A',  # flake8-builtins
+    'A',  # flake8-builtins
 #    'COM',  # flake8-commas
-#    'C4',  #  flake8-comprehensions
+#    'CPY',  # flake8-copyright
+#    'C4',  # flake8-comprehensions
 #    'DTZ',  # flake8-datetimez
 #    'T10',  # flake8-debugger
-#    'DJ',  #  flake8-django
-#    'EM',  #  flake8-errmsg
+#    'DJ',  # flake8-django
+#    'EM',  # flake8-errmsg
 #    'EXE',  # flake8-executable
+#    'FA',  # flake8-future-annotations
 #    'ISC',  # flake8-implicit-str-concat
 #    'ICN',  # flake8-import-conventions
 #    'G',  # flake8-logging-format
 #    'INP',  # flake8-no-pep420
 #    'PIE',  # flake8-pie
 #    'T20',  # flake8-print
 #    'PYI',  # flake8-pyi
-#    'PT',  #  flake8-pytest-style
+#    'PT',  # flake8-pytest-style
 #    'Q',  # flake8-quotes
 #    'RSE',  # flake8-raise
 #    'RET',  # flake8-return
 #    'SLF',  # flake8-self
+#    'SLOT',  # flake8-slots
 #    'SIM',  # flake8-simplify
 #    'TID',  # flake8-tidy-imports
 #    'TCH',  # flake8-type-checking
-#    'ARG',  # flake8-unused-arguments
+#    'INT',  # flake8-gettext
+    'ARG',  # flake8-unused-arguments
 #    'PTH',  # flake8-use-pathlib
-#    'ERA',  # eradicate
-#    'PD',  #  pandas-vet
+#    'TD',  # flake8-todos
+#    'FIX',  # flake8-fixme
+    'ERA',  # eradicate
+#    'PD',  # pandas-vet
 #    'PGH',  # pygrep-hooks
-#    'PL',  #  Pylint
+#    'PL',  # Pylint
 #    'TRY',  # tryceratops
+#    'FLY',  # flynt
 #    'NPY',  # NumPy-specific rules
-#    'RUF',  # Ruff-specific rules
+#    'AIR',  # Airflow
+#    'PERF',  # Perflint
+#    'FURB',  # refurb
+    'LOG',  # flake8-logging
+    'RUF',  # Ruff-specific rules
 ]
-line-length = 120
-target-version = "py37"
+
+[tool.ruff.format]
+quote-style = "single"
+exclude = ["**/tests/*"]
+docstring-code-format = true
```

### Comparing `pytest_embedded_serial-1.8.1/pytest_embedded_serial/dut.py` & `pytest_embedded_serial-1.8.2/pytest_embedded_serial/dut.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_serial-1.8.1/pytest_embedded_serial/serial.py` & `pytest_embedded_serial-1.8.2/pytest_embedded_serial/serial.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import contextlib
 import copy
 import logging
 import multiprocessing
 import queue
 import threading
 import time
-from typing import Dict, Optional
+from typing import Any, ClassVar, Dict, Optional
 
 import serial as pyserial
 from pytest_embedded.log import MessageQueue
 from pytest_embedded.utils import Meta
 from serial.tools import list_ports
 
 
@@ -24,31 +24,31 @@
 
     Warning:
         - make sure this `Serial.__init__()` run the last in MRO, it would create and start the redirect serial process
     """
 
     DEFAULT_BAUDRATE = 115200
 
-    DEFAULT_PORT_CONFIG = {
+    DEFAULT_PORT_CONFIG: ClassVar[Dict[str, Any]] = {
         'baudrate': DEFAULT_BAUDRATE,
         'bytesize': pyserial.EIGHTBITS,
         'parity': pyserial.PARITY_NONE,
         'stopbits': pyserial.STOPBITS_ONE,
         'timeout': 0.05,  # read timeout
         'xonxoff': False,
         'rtscts': False,
     }
 
-    occupied_ports: Dict[str, None] = dict()
+    occupied_ports: ClassVar[Dict[str, None]] = dict()
 
     def __init__(
         self,
         msg_queue: MessageQueue,
-        port: str = None,
-        port_location: str = None,
+        port: Optional[str] = None,
+        port_location: Optional[str] = None,
         baud: int = DEFAULT_BAUDRATE,
         meta: Optional[Meta] = None,
         **kwargs,
     ):
         self._q = msg_queue
         self._meta = meta
         self._redirect_thread: _SerialRedirectThread = None  # type: ignore
```

### Comparing `pytest_embedded_serial-1.8.1/PKG-INFO` & `pytest_embedded_serial-1.8.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-serial
-Version: 1.8.1
+Version: 1.8.2
 Summary: Make pytest-embedded plugin work with Serial.
 Author-email: Fu Hanxi <fuhanxi@espressif.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Testing
-Requires-Dist: pytest-embedded~=1.8.1
+Requires-Dist: pytest-embedded~=1.8.2
 Requires-Dist: pyserial~=3.0
 Project-URL: changelog, https://github.com/espressif/pytest-embedded/blob/main/CHANGELOG.md
 Project-URL: documentation, https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Project-URL: homepage, https://github.com/espressif/pytest-embedded
 Project-URL: repository, https://github.com/espressif/pytest-embedded
 
 ### pytest-embedded-serial
```

