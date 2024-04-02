# Comparing `tmp/pytest_embedded_arduino-1.8.1.tar.gz` & `tmp/pytest_embedded_arduino-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_embedded_arduino-1.8.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pytest_embedded_arduino-1.8.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest_embedded_arduino-1.8.1.tar` & `pytest_embedded_arduino-1.8.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1094 2024-03-01 10:19:36.927475 pytest_embedded_arduino-1.8.1/LICENSE
--rw-r--r--   0        0        0      516 2024-03-01 10:19:36.927475 pytest_embedded_arduino-1.8.1/README.md
--rw-r--r--   0        0        0     3093 2024-03-01 10:19:36.927475 pytest_embedded_arduino-1.8.1/pyproject.toml
--rw-r--r--   0        0        0      193 2024-03-01 10:19:36.927475 pytest_embedded_arduino-1.8.1/pytest_embedded_arduino/__init__.py
--rw-r--r--   0        0        0     2426 2024-03-01 10:19:36.927475 pytest_embedded_arduino-1.8.1/pytest_embedded_arduino/app.py
--rw-r--r--   0        0        0     1530 2024-03-01 10:19:36.927475 pytest_embedded_arduino-1.8.1/pytest_embedded_arduino/serial.py
--rw-r--r--   0        0        0      747 2024-03-01 10:19:36.927475 pytest_embedded_arduino-1.8.1/tests/test_arduino.py
--rw-r--r--   0        0        0     1994 1970-01-01 00:00:00.000000 pytest_embedded_arduino-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1094 2024-04-02 08:52:22.104840 pytest_embedded_arduino-1.8.2/LICENSE
+-rw-r--r--   0        0        0      516 2024-04-02 08:52:22.104840 pytest_embedded_arduino-1.8.2/README.md
+-rw-r--r--   0        0        0     3442 2024-04-02 08:52:22.104840 pytest_embedded_arduino-1.8.2/pyproject.toml
+-rw-r--r--   0        0        0      193 2024-04-02 08:52:22.104840 pytest_embedded_arduino-1.8.2/pytest_embedded_arduino/__init__.py
+-rw-r--r--   0        0        0     2511 2024-04-02 08:52:22.104840 pytest_embedded_arduino-1.8.2/pytest_embedded_arduino/app.py
+-rw-r--r--   0        0        0     1530 2024-04-02 08:52:22.104840 pytest_embedded_arduino-1.8.2/pytest_embedded_arduino/serial.py
+-rw-r--r--   0        0        0      747 2024-04-02 08:52:22.108840 pytest_embedded_arduino-1.8.2/tests/test_arduino.py
+-rw-r--r--   0        0        0     1994 1970-01-01 00:00:00.000000 pytest_embedded_arduino-1.8.2/PKG-INFO
```

### Comparing `pytest_embedded_arduino-1.8.1/LICENSE` & `pytest_embedded_arduino-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_embedded_arduino-1.8.1/README.md` & `pytest_embedded_arduino-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `pytest_embedded_arduino-1.8.1/pyproject.toml` & `pytest_embedded_arduino-1.8.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -27,81 +27,95 @@
     "Programming Language :: Python",
     "Topic :: Software Development :: Testing",
 ]
 dynamic = ["version", "description"]
 requires-python = ">=3.7"
 
 dependencies = [
-    "pytest-embedded~=1.8.1",
+    "pytest-embedded~=1.8.2",
 ]
 
 [project.optional-dependencies]
 serial = [
-    "pytest-embedded-serial-esp~=1.8.1"
+    "pytest-embedded-serial-esp~=1.8.2"
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

### Comparing `pytest_embedded_arduino-1.8.1/pytest_embedded_arduino/app.py` & `pytest_embedded_arduino-1.8.2/pytest_embedded_arduino/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 import os
-from typing import List, Tuple
+from typing import ClassVar, Dict, List, Tuple
 
 from pytest_embedded.app import App
 
 
 class ArduinoApp(App):
     """
     Arduino App class
@@ -13,25 +13,25 @@
         sketch (str): Sketch name.
         fqbn (str): Fully Qualified Board Name.
         target (str) : ESPxx chip.
         flash_files (List[Tuple[int, str, str]]): List of (offset, file path, encrypted) of files need to be flashed in.
     """
 
     #: dict of flash settings
-    flash_settings = {
+    flash_settings: ClassVar[Dict[str, Dict[str, str]]] = {
         'esp32': {'flash_mode': 'dio', 'flash_size': 'detect', 'flash_freq': '80m'},
         'esp32s2': {'flash_mode': 'dio', 'flash_size': 'detect', 'flash_freq': '80m'},
         'esp32c3': {'flash_mode': 'dio', 'flash_size': 'detect', 'flash_freq': '80m'},
         'esp32s3': {'flash_mode': 'dio', 'flash_size': 'detect', 'flash_freq': '80m'},
         'esp32c6': {'flash_mode': 'dio', 'flash_size': 'detect', 'flash_freq': '80m'},
         'esp32h2': {'flash_mode': 'dio', 'flash_size': 'detect', 'flash_freq': '48m'},
     }
 
     #: dict of binaries' offset.
-    binary_offsets = {
+    binary_offsets: ClassVar[Dict[str, List[int]]] = {
         'esp32': [0x1000, 0x8000, 0x10000],
         'esp32s2': [0x1000, 0x8000, 0x10000],
         'esp32c3': [0x0, 0x8000, 0x10000],
         'esp32s3': [0x0, 0x8000, 0x10000],
         'esp32c6': [0x0, 0x8000, 0x10000],
         'esp32h2': [0x0, 0x8000, 0x10000],
     }
```

### Comparing `pytest_embedded_arduino-1.8.1/pytest_embedded_arduino/serial.py` & `pytest_embedded_arduino-1.8.2/pytest_embedded_arduino/serial.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_arduino-1.8.1/tests/test_arduino.py` & `pytest_embedded_arduino-1.8.2/tests/test_arduino.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_arduino-1.8.1/PKG-INFO` & `pytest_embedded_arduino-1.8.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-arduino
-Version: 1.8.1
+Version: 1.8.2
 Summary: Make pytest-embedded plugin work with Arduino.
 Author-email: Abdelatif Guettouche <abdelatif.guettouche@espressif.com>, Fu Hanxi <fuhanxi@espressif.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
@@ -16,16 +16,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Testing
-Requires-Dist: pytest-embedded~=1.8.1
-Requires-Dist: pytest-embedded-serial-esp~=1.8.1 ; extra == "serial"
+Requires-Dist: pytest-embedded~=1.8.2
+Requires-Dist: pytest-embedded-serial-esp~=1.8.2 ; extra == "serial"
 Project-URL: changelog, https://github.com/espressif/pytest-embedded/blob/main/CHANGELOG.md
 Project-URL: documentation, https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Project-URL: homepage, https://github.com/espressif/pytest-embedded
 Project-URL: repository, https://github.com/espressif/pytest-embedded
 Provides-Extra: serial
 
 ### pytest-embedded-arduino
```

