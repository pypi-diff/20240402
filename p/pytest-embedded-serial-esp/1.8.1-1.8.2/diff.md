# Comparing `tmp/pytest_embedded_serial_esp-1.8.1.tar.gz` & `tmp/pytest_embedded_serial_esp-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_embedded_serial_esp-1.8.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pytest_embedded_serial_esp-1.8.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest_embedded_serial_esp-1.8.1.tar` & `pytest_embedded_serial_esp-1.8.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1094 2024-03-01 10:19:36.927475 pytest_embedded_serial_esp-1.8.1/LICENSE
--rw-r--r--   0        0        0      202 2024-03-01 10:19:36.927475 pytest_embedded_serial_esp-1.8.1/README.md
--rw-r--r--   0        0        0     2954 2024-03-01 10:19:36.927475 pytest_embedded_serial_esp-1.8.1/pyproject.toml
--rw-r--r--   0        0        0      155 2024-03-01 10:19:36.927475 pytest_embedded_serial_esp-1.8.1/pytest_embedded_serial_esp/__init__.py
--rw-r--r--   0        0        0     6597 2024-03-01 10:19:36.927475 pytest_embedded_serial_esp-1.8.1/pytest_embedded_serial_esp/serial.py
--rw-r--r--   0        0        0     2906 2024-03-01 10:19:36.927475 pytest_embedded_serial_esp-1.8.1/tests/test_esp.py
--rw-r--r--   0        0        0     1583 1970-01-01 00:00:00.000000 pytest_embedded_serial_esp-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1094 2024-04-02 08:52:22.108840 pytest_embedded_serial_esp-1.8.2/LICENSE
+-rw-r--r--   0        0        0      202 2024-04-02 08:52:22.108840 pytest_embedded_serial_esp-1.8.2/README.md
+-rw-r--r--   0        0        0     3303 2024-04-02 08:52:22.108840 pytest_embedded_serial_esp-1.8.2/pyproject.toml
+-rw-r--r--   0        0        0      155 2024-04-02 08:52:22.108840 pytest_embedded_serial_esp-1.8.2/pytest_embedded_serial_esp/__init__.py
+-rw-r--r--   0        0        0     7036 2024-04-02 08:52:22.108840 pytest_embedded_serial_esp-1.8.2/pytest_embedded_serial_esp/serial.py
+-rw-r--r--   0        0        0     2906 2024-04-02 08:52:22.108840 pytest_embedded_serial_esp-1.8.2/tests/test_esp.py
+-rw-r--r--   0        0        0     1583 1970-01-01 00:00:00.000000 pytest_embedded_serial_esp-1.8.2/PKG-INFO
```

### Comparing `pytest_embedded_serial_esp-1.8.1/LICENSE` & `pytest_embedded_serial_esp-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_embedded_serial_esp-1.8.1/pyproject.toml` & `pytest_embedded_serial_esp-1.8.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -26,77 +26,91 @@
     "Programming Language :: Python",
     "Topic :: Software Development :: Testing",
 ]
 dynamic = ["version", "description"]
 requires-python = ">=3.7"
 
 dependencies = [
-    "pytest-embedded-serial~=1.8.1",
+    "pytest-embedded-serial~=1.8.2",
     "esptool~=4.5",
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

### Comparing `pytest_embedded_serial_esp-1.8.1/pytest_embedded_serial_esp/serial.py` & `pytest_embedded_serial_esp-1.8.2/pytest_embedded_serial_esp/serial.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import contextlib
 import functools
 import logging
 import subprocess
+import warnings
 from typing import Optional
 from warnings import warn
 
 import esptool
 from esptool import __version__ as ESPTOOL_VERSION
 from esptool.targets import CHIP_LIST as ESPTOOL_CHIPS
 from pexpect import TIMEOUT
@@ -24,20 +25,22 @@
             pexpect_proc.expect(f'MAC: {port_mac.lower()}', timeout=0.1)
         except TIMEOUT:
             return False
         else:
             return True
 
 
-class EsptoolArgs(object):
+class EsptoolArgs:
     """
     fake args object, this is a hack until esptool Python API is improved
     """
 
     def __init__(self, **kwargs):
+        warnings.warn('EsptoolArgs is deprecated and will be removed in 2.0 release.', DeprecationWarning)
+
         for key, value in kwargs.items():
             self.__setattr__(key, value)
 
 
 class EspSerial(Serial):
     """
     Serial class for ports connected to espressif products
@@ -48,15 +51,15 @@
     def __init__(
         self,
         pexpect_proc: PexpectProcess,
         msg_queue: MessageQueue,
         target: Optional[str] = None,
         beta_target: Optional[str] = None,
         port: Optional[str] = None,
-        port_mac: str = None,
+        port_mac: Optional[str] = None,
         baud: int = Serial.DEFAULT_BAUDRATE,
         esptool_baud: int = ESPTOOL_DEFAULT_BAUDRATE,
         esp_flash_force: bool = False,
         skip_autoflash: bool = False,
         erase_all: bool = False,
         meta: Optional[Meta] = None,
         **kwargs,
@@ -90,15 +93,15 @@
                     ports = [port]
                 else:
                     raise ValueError(f'The specified MAC address {port_mac} binds with different port, not with {port}')
             else:
                 ports = [port]
 
         # normal loader
-        if esptool_target not in (['auto'] + ESPTOOL_CHIPS):
+        if esptool_target not in ['auto', *ESPTOOL_CHIPS]:
             raise ValueError(
                 f'esptool version {ESPTOOL_VERSION} not support target {esptool_target}\n'
                 f'Supported targets: {ESPTOOL_CHIPS}'
             )
 
         with contextlib.redirect_stdout(msg_queue):
             self.esp = esptool.get_default_connected_device(
@@ -129,31 +132,37 @@
             self._meta.set_port_target_cache(self.port, self.target)
 
         if self.erase_all:
             esptool.main(['erase_flash'], esp=self.esp)
 
         super()._post_init()
 
-    def use_esptool(hard_reset_after: bool = True, no_stub: bool = False):
+    def use_esptool(hard_reset_after: Optional[bool] = None, no_stub: Optional[bool] = None):
         """
         1. tell the redirect serial thread to stop reading from the `pyserial` instance
-        2. esptool reuse the `pyserial` instance and call `run_stub()`
-        3. call to the decorated function, could use `self.stub` inside the function as the stubbed loader
-        4. call `hard_reset()`, if `hard_reset_after` is True
-        5. tell the redirect serial thread to continue reading from serial
+        2. esptool reuse the `pyserial` instance and call `esptool.main()` to do the actual work
+        3. tell the redirect serial thread to continue reading from serial
 
         Args:
-            hard_reset_after: run hard reset after
-            no_stub: disable launching the flasher stub
+            hard_reset_after: run hard reset after (deprecated)
+            no_stub: disable launching the flasher stub (deprecated)
         """
-        warn(
-            "The 'no_stub' parameter is now read directly from `flasher_args.json` "
-            'and does not need to be explicitly set.',
-            DeprecationWarning,
-        )
+        if hard_reset_after is not None:
+            warn(
+                "The 'hard_reset_after' parameter is now read directly from `flasher_args.json` "
+                'and does not need to be explicitly set. This parameter will be removed in 2.0 release.',
+                DeprecationWarning,
+            )
+
+        if no_stub is not None:
+            warn(
+                "The 'no_stub' parameter is now read directly from `flasher_args.json` "
+                'and does not need to be explicitly set. This parameter will be removed in 2.0 release.',
+                DeprecationWarning,
+            )
 
         def decorator(func):
             @functools.wraps(func)
             def wrapper(self, *args, **kwargs):
                 with self.disable_redirect_thread():
                     with contextlib.redirect_stdout(self._q):
                         settings = self.proc.get_settings()
```

### Comparing `pytest_embedded_serial_esp-1.8.1/tests/test_esp.py` & `pytest_embedded_serial_esp-1.8.2/tests/test_esp.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_serial_esp-1.8.1/PKG-INFO` & `pytest_embedded_serial_esp-1.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-serial-esp
-Version: 1.8.1
+Version: 1.8.2
 Summary: Make pytest-embedded plugin work with Espressif target boards.
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
-Requires-Dist: pytest-embedded-serial~=1.8.1
+Requires-Dist: pytest-embedded-serial~=1.8.2
 Requires-Dist: esptool~=4.5
 Project-URL: changelog, https://github.com/espressif/pytest-embedded/blob/main/CHANGELOG.md
 Project-URL: documentation, https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Project-URL: homepage, https://github.com/espressif/pytest-embedded
 Project-URL: repository, https://github.com/espressif/pytest-embedded
 
 ### pytest-embedded-serial-esp
```

