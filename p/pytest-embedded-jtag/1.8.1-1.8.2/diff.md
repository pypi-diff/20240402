# Comparing `tmp/pytest_embedded_jtag-1.8.1.tar.gz` & `tmp/pytest_embedded_jtag-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_embedded_jtag-1.8.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pytest_embedded_jtag-1.8.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest_embedded_jtag-1.8.1.tar` & `pytest_embedded_jtag-1.8.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1094 2024-03-01 10:19:36.927475 pytest_embedded_jtag-1.8.1/LICENSE
--rw-r--r--   0        0        0      245 2024-03-01 10:19:36.927475 pytest_embedded_jtag-1.8.1/README.md
--rw-r--r--   0        0        0     2928 2024-03-01 10:19:36.927475 pytest_embedded_jtag-1.8.1/pyproject.toml
--rw-r--r--   0        0        0      165 2024-03-01 10:19:36.927475 pytest_embedded_jtag-1.8.1/pytest_embedded_jtag/__init__.py
--rw-r--r--   0        0        0     1845 2024-03-01 10:19:36.927475 pytest_embedded_jtag-1.8.1/pytest_embedded_jtag/gdb.py
--rw-r--r--   0        0        0     2359 2024-03-01 10:19:36.927475 pytest_embedded_jtag-1.8.1/pytest_embedded_jtag/openocd.py
--rw-r--r--   0        0        0      930 2024-03-01 10:19:36.927475 pytest_embedded_jtag-1.8.1/tests/test_jtag.py
--rw-r--r--   0        0        0     1573 1970-01-01 00:00:00.000000 pytest_embedded_jtag-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1094 2024-04-02 08:52:22.108840 pytest_embedded_jtag-1.8.2/LICENSE
+-rw-r--r--   0        0        0      245 2024-04-02 08:52:22.108840 pytest_embedded_jtag-1.8.2/README.md
+-rw-r--r--   0        0        0     3277 2024-04-02 08:52:22.108840 pytest_embedded_jtag-1.8.2/pyproject.toml
+-rw-r--r--   0        0        0      165 2024-04-02 08:52:22.108840 pytest_embedded_jtag-1.8.2/pytest_embedded_jtag/__init__.py
+-rw-r--r--   0        0        0     1845 2024-04-02 08:52:22.108840 pytest_embedded_jtag-1.8.2/pytest_embedded_jtag/gdb.py
+-rw-r--r--   0        0        0     2309 2024-04-02 08:52:22.108840 pytest_embedded_jtag-1.8.2/pytest_embedded_jtag/openocd.py
+-rw-r--r--   0        0        0      930 2024-04-02 08:52:22.108840 pytest_embedded_jtag-1.8.2/tests/test_jtag.py
+-rw-r--r--   0        0        0     1573 1970-01-01 00:00:00.000000 pytest_embedded_jtag-1.8.2/PKG-INFO
```

### Comparing `pytest_embedded_jtag-1.8.1/LICENSE` & `pytest_embedded_jtag-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_embedded_jtag-1.8.1/pyproject.toml` & `pytest_embedded_jtag-1.8.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -26,76 +26,90 @@
     "Programming Language :: Python",
     "Topic :: Software Development :: Testing",
 ]
 dynamic = ["version", "description"]
 requires-python = ">=3.7"
 
 dependencies = [
-    "pytest-embedded-serial~=1.8.1",
+    "pytest-embedded-serial~=1.8.2",
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

### Comparing `pytest_embedded_jtag-1.8.1/pytest_embedded_jtag/gdb.py` & `pytest_embedded_jtag-1.8.2/pytest_embedded_jtag/gdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     def __init__(self, gdb_prog_path: Optional[str] = None, gdb_cli_args: Optional[str] = None, **kwargs):
         gdb_prog_path = gdb_prog_path or self.GDB_PROG_PATH
         gdb_cli_args = shlex.split(gdb_cli_args or self.GDB_DEFAULT_ARGS)
 
         self._gdb_first_prompt_matched = False
 
-        super().__init__(cmd=[gdb_prog_path] + gdb_cli_args, **kwargs)
+        super().__init__(cmd=[gdb_prog_path, *gdb_cli_args], **kwargs)
 
     def write(self, s: AnyStr, non_blocking: bool = False, timeout: float = 30) -> Optional[str]:
         super().write(s)
         _buffer = ''
         _t_start = time.time()
 
         with open(self._logfile) as fr:
```

### Comparing `pytest_embedded_jtag-1.8.1/pytest_embedded_jtag/openocd.py` & `pytest_embedded_jtag-1.8.2/pytest_embedded_jtag/openocd.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,26 +38,24 @@
         if openocd_scripts_path:
             openocd_cli_args.extend(['-s', openocd_scripts_path])
 
         self.tcl_port = self.TCL_BASE_PORT + port_offset
         self.telnet_port = self.TELNET_BASE_PORT + port_offset
         self.gdb_port = self.GDB_BASE_PORT + port_offset
 
-        openocd_cli_args.extend(
-            [
-                '-c',
-                f'tcl_port {self.tcl_port}',
-                '-c',
-                f'telnet_port {self.telnet_port}',
-                '-c',
-                f'gdb_port {self.gdb_port}',
-            ]
-        )
+        openocd_cli_args.extend([
+            '-c',
+            f'tcl_port {self.tcl_port}',
+            '-c',
+            f'telnet_port {self.telnet_port}',
+            '-c',
+            f'gdb_port {self.gdb_port}',
+        ])
 
-        super().__init__(cmd=[openocd_prog_path] + openocd_cli_args, **kwargs)
+        super().__init__(cmd=[openocd_prog_path, *openocd_cli_args], **kwargs)
 
         # open telnet port to interact with openocd
         for i in range(30):
             try:
                 self.telnet = telnetlib.Telnet('127.0.0.1', self.telnet_port, 5)
                 break
             except ConnectionRefusedError:
```

### Comparing `pytest_embedded_jtag-1.8.1/tests/test_jtag.py` & `pytest_embedded_jtag-1.8.2/tests/test_jtag.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_jtag-1.8.1/PKG-INFO` & `pytest_embedded_jtag-1.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-jtag
-Version: 1.8.1
+Version: 1.8.2
 Summary: Make pytest-embedded plugin work with JTAG.
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
 Project-URL: changelog, https://github.com/espressif/pytest-embedded/blob/main/CHANGELOG.md
 Project-URL: documentation, https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Project-URL: homepage, https://github.com/espressif/pytest-embedded
 Project-URL: repository, https://github.com/espressif/pytest-embedded
 
 ### pytest-embedded-jtag
```

