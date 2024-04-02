# Comparing `tmp/pytest_embedded_qemu-1.8.1.tar.gz` & `tmp/pytest_embedded_qemu-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_embedded_qemu-1.8.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pytest_embedded_qemu-1.8.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest_embedded_qemu-1.8.1.tar` & `pytest_embedded_qemu-1.8.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1094 2024-03-01 10:19:36.927475 pytest_embedded_qemu-1.8.1/LICENSE
--rw-r--r--   0        0        0      552 2024-03-01 10:19:36.927475 pytest_embedded_qemu-1.8.1/README.md
--rw-r--r--   0        0        0     3020 2024-03-01 10:19:36.927475 pytest_embedded_qemu-1.8.1/pyproject.toml
--rw-r--r--   0        0        0      369 2024-03-01 10:19:36.927475 pytest_embedded_qemu-1.8.1/pytest_embedded_qemu/__init__.py
--rw-r--r--   0        0        0     6374 2024-03-01 10:19:36.927475 pytest_embedded_qemu-1.8.1/pytest_embedded_qemu/app.py
--rw-r--r--   0        0        0      473 2024-03-01 10:19:36.927475 pytest_embedded_qemu-1.8.1/pytest_embedded_qemu/dut.py
--rw-r--r--   0        0        0     4119 2024-03-01 10:19:36.927475 pytest_embedded_qemu-1.8.1/pytest_embedded_qemu/qemu.py
--rw-r--r--   0        0        0     4479 2024-03-01 10:19:36.927475 pytest_embedded_qemu-1.8.1/tests/test_qemu.py
--rw-r--r--   0        0        0     1983 1970-01-01 00:00:00.000000 pytest_embedded_qemu-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1094 2024-04-02 08:52:22.108840 pytest_embedded_qemu-1.8.2/LICENSE
+-rw-r--r--   0        0        0      552 2024-04-02 08:52:22.108840 pytest_embedded_qemu-1.8.2/README.md
+-rw-r--r--   0        0        0     3369 2024-04-02 08:52:22.108840 pytest_embedded_qemu-1.8.2/pyproject.toml
+-rw-r--r--   0        0        0      369 2024-04-02 08:52:22.108840 pytest_embedded_qemu-1.8.2/pytest_embedded_qemu/__init__.py
+-rw-r--r--   0        0        0     6452 2024-04-02 08:52:22.108840 pytest_embedded_qemu-1.8.2/pytest_embedded_qemu/app.py
+-rw-r--r--   0        0        0      473 2024-04-02 08:52:22.108840 pytest_embedded_qemu-1.8.2/pytest_embedded_qemu/dut.py
+-rw-r--r--   0        0        0     4113 2024-04-02 08:52:22.108840 pytest_embedded_qemu-1.8.2/pytest_embedded_qemu/qemu.py
+-rw-r--r--   0        0        0     4481 2024-04-02 08:52:22.108840 pytest_embedded_qemu-1.8.2/tests/test_qemu.py
+-rw-r--r--   0        0        0     1983 1970-01-01 00:00:00.000000 pytest_embedded_qemu-1.8.2/PKG-INFO
```

### Comparing `pytest_embedded_qemu-1.8.1/LICENSE` & `pytest_embedded_qemu-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_embedded_qemu-1.8.1/README.md` & `pytest_embedded_qemu-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `pytest_embedded_qemu-1.8.1/pyproject.toml` & `pytest_embedded_qemu-1.8.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -26,82 +26,96 @@
     "Programming Language :: Python",
     "Topic :: Software Development :: Testing",
 ]
 dynamic = ["version", "description"]
 requires-python = ">=3.7"
 
 dependencies = [
-    "pytest-embedded~=1.8.1",
+    "pytest-embedded~=1.8.2",
     "qemu.qmp==0.0.3"
 ]
 
 [project.optional-dependencies]
 idf = [
-    "pytest-embedded-idf~=1.8.1",
+    "pytest-embedded-idf~=1.8.2",
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

### Comparing `pytest_embedded_qemu-1.8.1/pytest_embedded_qemu/app.py` & `pytest_embedded_qemu-1.8.2/pytest_embedded_qemu/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 
 
 class IdfFlashImageMaker:
     """
     Create a single image for QEMU based on the `IdfApp`'s partition table and all the flash files.
     """
 
-    XTENSA_FLASH_BIN_SIZES = [
+    XTENSA_FLASH_BIN_SIZES: t.ClassVar[t.List[t.Tuple[int, str]]] = [
         (2 * 1024 * 1024, '2MB'),
         (4 * 1024 * 1024, '4MB'),
         (8 * 1024 * 1024, '8MB'),
         (16 * 1024 * 1024, '16MB'),
     ]
 
-    RISCV_FLASH_BIN_SIZES = [
+    RISCV_FLASH_BIN_SIZES: t.ClassVar[t.List[t.Tuple[int, str]]] = [
         (256 * 1024, '256KB'),
         (512 * 1024, '512KB'),
         (1 * 1024 * 1024, '1MB'),
         (2 * 1024 * 1024, '2MB'),
         (4 * 1024 * 1024, '4MB'),
         (8 * 1024 * 1024, '8MB'),
         (16 * 1024 * 1024, '16MB'),
```

### Comparing `pytest_embedded_qemu-1.8.1/pytest_embedded_qemu/qemu.py` & `pytest_embedded_qemu-1.8.2/pytest_embedded_qemu/qemu.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,20 +47,20 @@
             qemu_cli_args: QEMU CLI arguments
             qemu_extra_args: QEMU CLI extra arguments, will be appended to `qemu_cli_args`
         """
         self.app = app
 
         image_path = qemu_image_path or DEFAULT_IMAGE_FN
         if not os.path.exists(image_path):
-            raise ValueError(f'QEMU image path doesn\'t exist: {image_path}')
+            raise ValueError(f"QEMU image path doesn't exist: {image_path}")
 
         qemu_prog_path = qemu_prog_path or self.qemu_prog_name
 
         if qemu_cli_args:
-            qemu_cli_args = qemu_cli_args.strip("\"").strip("\'")
+            qemu_cli_args = qemu_cli_args.strip('"').strip("'")
         qemu_cli_args = shlex.split(qemu_cli_args or self.qemu_default_args)
         qemu_extra_args = shlex.split(qemu_extra_args or '')
 
         self.qmp_addr = None
         self.qmp_port = None
 
         dut_index = int(kwargs.pop('dut_index', 0))
@@ -79,15 +79,15 @@
             self.qmp_addr = '127.0.0.1'
             with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
                 s.bind((self.qmp_addr, 0))
                 _, self.qmp_port = s.getsockname()
             qemu_cli_args += shlex.split(self.QEMU_DEFAULT_QMP_FMT.format(self.qmp_port))
 
         super().__init__(
-            cmd=[qemu_prog_path, *qemu_cli_args, *qemu_extra_args] + ['-drive', f'file={image_path},if=mtd,format=raw'],
+            cmd=[qemu_prog_path, *qemu_cli_args, *qemu_extra_args, '-drive', f'file={image_path},if=mtd,format=raw'],
             **kwargs,
         )
 
     @property
     def qemu_prog_name(self):
         if self.app:
             try:
```

### Comparing `pytest_embedded_qemu-1.8.1/tests/test_qemu.py` & `pytest_embedded_qemu-1.8.2/tests/test_qemu.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,22 +120,23 @@
     keyfile_path = os.path.join(app_path, 'pre_encryption_key.bin')
     efuses_path = os.path.join(app_path, 'pre_encryption_efuses.bin')
 
     result = testdir.runpytest(
         '-s',
         '--embedded-services', 'idf,qemu',
         '--app-path', app_path,
-        '--qemu-extra-args',f'-drive file={efuses_path},if=none,format=raw,id=efuse'
+        '--qemu-extra-args', f'-drive file={efuses_path},if=none,format=raw,id=efuse'
         ' -global driver=nvram.esp32.efuse,property=drive,value=efuse',
         '--encrypt', 'true',
         '--keyfile', keyfile_path,
     )
 
     result.assert_outcomes(passed=1)
 
+
 @qemu_bin_required
 def test_qemu_use_idf_mixin_methods(testdir):
     testdir.makepyfile("""
         import pexpect
         import pytest
 
         def test_qemu_use_idf_mixin_methods(dut):
```

### Comparing `pytest_embedded_qemu-1.8.1/PKG-INFO` & `pytest_embedded_qemu-1.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-qemu
-Version: 1.8.1
+Version: 1.8.2
 Summary: Make pytest-embedded plugin work with QEMU.
 Author-email: Fu Hanxi <fuhanxi@espressif.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
@@ -16,17 +16,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Testing
-Requires-Dist: pytest-embedded~=1.8.1
+Requires-Dist: pytest-embedded~=1.8.2
 Requires-Dist: qemu.qmp==0.0.3
-Requires-Dist: pytest-embedded-idf~=1.8.1 ; extra == "idf"
+Requires-Dist: pytest-embedded-idf~=1.8.2 ; extra == "idf"
 Project-URL: changelog, https://github.com/espressif/pytest-embedded/blob/main/CHANGELOG.md
 Project-URL: documentation, https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Project-URL: homepage, https://github.com/espressif/pytest-embedded
 Project-URL: repository, https://github.com/espressif/pytest-embedded
 Provides-Extra: idf
 
 ### pytest-embedded-qemu
```

