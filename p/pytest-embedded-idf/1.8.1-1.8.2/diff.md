# Comparing `tmp/pytest_embedded_idf-1.8.1.tar.gz` & `tmp/pytest_embedded_idf-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_embedded_idf-1.8.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pytest_embedded_idf-1.8.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest_embedded_idf-1.8.1.tar` & `pytest_embedded_idf-1.8.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1094 2024-03-01 10:19:36.927475 pytest_embedded_idf-1.8.1/LICENSE
--rw-r--r--   0        0        0      520 2024-03-01 10:19:36.927475 pytest_embedded_idf-1.8.1/README.md
--rw-r--r--   0        0        0     3061 2024-03-01 10:19:36.927475 pytest_embedded_idf-1.8.1/pyproject.toml
--rw-r--r--   0        0        0      675 2024-03-01 10:19:36.927475 pytest_embedded_idf-1.8.1/pytest_embedded_idf/__init__.py
--rw-r--r--   0        0        0     9180 2024-03-01 10:19:36.927475 pytest_embedded_idf-1.8.1/pytest_embedded_idf/app.py
--rw-r--r--   0        0        0    11153 2024-03-01 10:19:36.927475 pytest_embedded_idf-1.8.1/pytest_embedded_idf/dut.py
--rw-r--r--   0        0        0     1233 2024-03-01 10:19:36.927475 pytest_embedded_idf-1.8.1/pytest_embedded_idf/linux.py
--rw-r--r--   0        0        0     9853 2024-03-01 10:19:36.927475 pytest_embedded_idf-1.8.1/pytest_embedded_idf/serial.py
--rw-r--r--   0        0        0    33058 2024-03-01 10:19:36.927475 pytest_embedded_idf-1.8.1/pytest_embedded_idf/unity_tester.py
--rw-r--r--   0        0        0    21859 2024-03-01 10:19:36.927475 pytest_embedded_idf-1.8.1/tests/test_idf.py
--rw-r--r--   0        0        0     2025 1970-01-01 00:00:00.000000 pytest_embedded_idf-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1094 2024-04-02 08:52:22.108840 pytest_embedded_idf-1.8.2/LICENSE
+-rw-r--r--   0        0        0      520 2024-04-02 08:52:22.108840 pytest_embedded_idf-1.8.2/README.md
+-rw-r--r--   0        0        0     3410 2024-04-02 08:52:22.108840 pytest_embedded_idf-1.8.2/pyproject.toml
+-rw-r--r--   0        0        0      675 2024-04-02 08:52:22.108840 pytest_embedded_idf-1.8.2/pytest_embedded_idf/__init__.py
+-rw-r--r--   0        0        0     9254 2024-04-02 08:52:22.108840 pytest_embedded_idf-1.8.2/pytest_embedded_idf/app.py
+-rw-r--r--   0        0        0    11146 2024-04-02 08:52:22.108840 pytest_embedded_idf-1.8.2/pytest_embedded_idf/dut.py
+-rw-r--r--   0        0        0     1232 2024-04-02 08:52:22.108840 pytest_embedded_idf-1.8.2/pytest_embedded_idf/linux.py
+-rw-r--r--   0        0        0     9930 2024-04-02 08:52:22.108840 pytest_embedded_idf-1.8.2/pytest_embedded_idf/serial.py
+-rw-r--r--   0        0        0    33073 2024-04-02 08:52:22.108840 pytest_embedded_idf-1.8.2/pytest_embedded_idf/unity_tester.py
+-rw-r--r--   0        0        0    22581 2024-04-02 08:52:22.108840 pytest_embedded_idf-1.8.2/tests/test_idf.py
+-rw-r--r--   0        0        0     2025 1970-01-01 00:00:00.000000 pytest_embedded_idf-1.8.2/PKG-INFO
```

### Comparing `pytest_embedded_idf-1.8.1/LICENSE` & `pytest_embedded_idf-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_embedded_idf-1.8.1/README.md` & `pytest_embedded_idf-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `pytest_embedded_idf-1.8.1/pyproject.toml` & `pytest_embedded_idf-1.8.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -26,83 +26,97 @@
     "Programming Language :: Python",
     "Topic :: Software Development :: Testing",
 ]
 dynamic = ["version", "description"]
 requires-python = ">=3.7"
 
 dependencies = [
-    "pytest-embedded~=1.8.1",
+    "pytest-embedded~=1.8.2",
     "esp-idf-panic-decoder",
 ]
 
 [project.optional-dependencies]
 serial = [
-    "pytest-embedded-serial-esp~=1.8.1",
+    "pytest-embedded-serial-esp~=1.8.2",
     "esp-coredump~=1.0",
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

### Comparing `pytest_embedded_idf-1.8.1/pytest_embedded_idf/__init__.py` & `pytest_embedded_idf-1.8.2/pytest_embedded_idf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,17 +20,17 @@
         'IdfSerial': '.serial',
         'IdfDut': '.dut',
     },
 )
 
 
 __all__ = [
+    'CaseTester',
     'IdfApp',
-    'IdfSerial',
     'IdfDut',
-    'CaseTester',
-    'LinuxSerial',
+    'IdfSerial',
     'LinuxDut',
+    'LinuxSerial',
     'UnittestMenuCase',
 ]
 
-__version__ = '1.8.1'
+__version__ = '1.8.2'
```

### Comparing `pytest_embedded_idf-1.8.1/pytest_embedded_idf/app.py` & `pytest_embedded_idf-1.8.2/pytest_embedded_idf/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import logging
 import os
 import shlex
 import subprocess
 import sys
-from typing import Any, Dict, List, NamedTuple, Optional, Tuple
+from typing import Any, ClassVar, Dict, List, NamedTuple, Optional, Tuple
 
 from pytest_embedded.app import App
 
 
 class FlashFile(NamedTuple):
     offset: int
     file_path: str
@@ -22,27 +22,28 @@
     Attributes:
         elf_file (str): elf file path
         flash_args (dict[str, Any]): dict of flasher_args.json
         flash_files (list[FlashFile]): list of (offset, file path, encrypted) of files need to be flashed in
         flash_settings (dict[str, Any]): dict of flash settings
     """
 
-    XTENSA_TARGETS = ['esp32', 'esp32s2', 'esp32s3']
-    RISCV32_TARGETS = ['esp32c3', 'esp32h2', 'esp32c2', 'esp32c6']
+    XTENSA_TARGETS: ClassVar[List[str]] = ['esp32', 'esp32s2', 'esp32s3']
+    RISCV32_TARGETS: ClassVar[List[str]] = ['esp32c3', 'esp32h2', 'esp32c2', 'esp32c6']
 
     FLASH_ARGS_FILENAME = 'flash_args'
     FLASH_PROJECT_ARGS_FILENAME = 'flash_project_args'
     FLASH_ARGS_JSON_FILENAME = 'flasher_args.json'
 
     def __init__(
         self,
+        *args,
         part_tool: Optional[str] = None,
         **kwargs,
     ):
-        super().__init__(**kwargs)
+        super().__init__(*args, **kwargs)
 
         # Optional info
         self._sdkconfig = None
         self._target = None
         # the partition table is used for nvs
         self._parttool = part_tool
         self._partition_table = None
@@ -90,17 +91,17 @@
         """
         Returns:
             dict contains all k-v pairs from the sdkconfig file
         """
         if self._sdkconfig is not None:
             return self._sdkconfig
 
-        sdkconfig_json_path = os.path.join(self.binary_path, 'config', 'sdkconfig.json')
+        sdkconfig_json_path = os.path.join(self.binary_path or '', 'config', 'sdkconfig.json')
         if not os.path.isfile(sdkconfig_json_path):
-            logging.warning(f'{sdkconfig_json_path} doesn\'t exist. Skipping...')
+            logging.warning(f"{sdkconfig_json_path} doesn't exist. Skipping...")
             self._sdkconfig = {}
         else:
             self._sdkconfig = json.load(open(sdkconfig_json_path))
         return self._sdkconfig
 
     @property
     def target(self) -> str:
@@ -147,15 +148,15 @@
             self.flash_args.get('partition_table', self.flash_args.get('partition-table', {})).get('file', ''),
         )
         process = subprocess.Popen(
             [sys.executable, self.parttool_path, partition_file],
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         )
-        stdout, stderr = process.communicate()
+        stdout, _ = process.communicate()
         raw_data = stdout.decode() if isinstance(stdout, bytes) else stdout
 
         partition_table = {}
         for line in raw_data.splitlines():
             if line[0] != '#':
                 try:
                     _name, _type, _subtype, _offset, _size, _flags = line.split(',')
```

### Comparing `pytest_embedded_idf-1.8.1/pytest_embedded_idf/dut.py` & `pytest_embedded_idf-1.8.2/pytest_embedded_idf/dut.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,18 @@
 from contextlib import redirect_stdout
 
 from pytest_embedded.utils import UserHint, to_str
 from pytest_embedded_serial.dut import SerialDut
 from pytest_embedded_serial_esp import EspSerial
 
 from .app import IdfApp
-from .unity_tester import UnittestMenuCase  # noqa # keep backward compatibility
-from .unity_tester import IdfUnityDutMixin
+from .unity_tester import (
+    IdfUnityDutMixin,
+    UnittestMenuCase,  # noqa # keep backward compatibility
+)
 
 
 class IdfDut(IdfUnityDutMixin, SerialDut):
     """
     Dut class for serial ports connect to Espressif boards which are flashed with ESP-IDF apps
 
     Attributes:
@@ -41,15 +43,15 @@
     app: IdfApp
     serial: EspSerial
 
     def __init__(
         self,
         app: IdfApp,
         skip_check_coredump: bool = False,
-        panic_output_decode_script: str = None,
+        panic_output_decode_script: t.Optional[str] = None,
         **kwargs,
     ) -> None:
         self.target = app.target
         self.skip_check_coredump = skip_check_coredump
         self._panic_output_decode_script = panic_output_decode_script
 
         super().__init__(app=app, **kwargs)
@@ -113,35 +115,35 @@
                 f'{self.toolchain_prefix}-gdb',
                 '--command',
                 f'{self.app.app_path}/build/prefix_map_gdbinit',
                 '--batch',
                 '-n',
                 self.app.elf_file,
                 '-ex',
-                "target remote | \"{python}\" \"{script}\" --target {target} \"{output_file}\"".format(
+                'target remote | "{python}" "{script}" --target {target} "{output_file}"'.format(
                     python=sys.executable,
                     script=self.panic_output_decode_script,
                     target=self.target,
                     output_file=panic_output_file.name,
                 ),
                 '-ex',
                 'bt',
             ]
             output = subprocess.check_output(cmd, stderr=subprocess.STDOUT)
             logging.info('\n\nBacktrace:\n')
-            logging.info(output.decode())  # noqa: E999
+            logging.info(output.decode())
         except subprocess.CalledProcessError as e:
             logging.debug(f'Failed to run gdb_panic_server.py script: {e}\n{e.output}\n\n')
             logging.info(panic_output.decode())
         finally:
             if panic_output_file is not None:
                 try:
                     os.unlink(panic_output_file.name)
                 except OSError as e:
-                    logging.debug(f'Couldn\'t remove temporary panic output file ({e})')
+                    logging.debug(f"Couldn't remove temporary panic output file ({e})")
 
     def _check_coredump(self) -> None:
         """
         Handle errors by panic_handler_script or check core dumps via UART or partition table.
         Write the decoded or read core dumps into separated files.
 
         For UART and panic output, would read the `_pexpect_logfile` file.
@@ -263,27 +265,27 @@
             run_flash = False
 
         if run_flash:
             self.flash_via_jtag()
 
     def flash_via_jtag(self):
         if not self.openocd:
-            logging.warning('no openocd instance created. can\'t flash via openocd `program_esp`')
+            logging.warning("no openocd instance created. can't flash via openocd `program_esp`")
             return
 
         if self.app.is_loadable_elf:
             # loadable elf flash to ram. no cache.
             # load via test script.
             # For example:
-            # self.gdb.write('mon reset halt')
-            # self.gdb.write('thb *0x40007d54')
-            # self.gdb.write('c')
-            # self.gdb.write('load')
+            # >>> self.gdb.write('mon reset halt')
+            # >>> self.gdb.write('thb *0x40007d54')
+            # >>> self.gdb.write('c')
+            # >>> self.gdb.write('load')
             return
 
         for _f in self.app.flash_files:
             if _f.encrypted:
-                raise ValueError('Encrypted files can\'t be flashed in via JTAG')
+                raise ValueError("Encrypted files can't be flashed in via JTAG")
             self.openocd.write(f'program_esp {_f.file_path} {hex(_f.offset)} verify')
 
         if self._meta:
             self._meta.set_port_app_cache(self.serial.port, self.app)
```

### Comparing `pytest_embedded_idf-1.8.1/pytest_embedded_idf/linux.py` & `pytest_embedded_idf-1.8.2/pytest_embedded_idf/linux.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         self,
         app: IdfApp,
         **kwargs,
     ) -> None:
         self.app = app
 
         if not hasattr(self.app, 'target'):
-            raise ValueError(f'Idf app not parsable. Please check if it\'s valid: {self.app.binary_path}')
+            raise ValueError(f"Idf app not parsable. Please check if it's valid: {self.app.binary_path}")
 
         if self.app.target != 'linux':
             raise ValueError(f'Targets do not match. App target: {self.app.target}, Cmd target: "linux".')
 
         super().__init__(cmd=[self.app.elf_file], **kwargs)
 
     def hard_reset(self) -> None:
```

### Comparing `pytest_embedded_idf-1.8.1/pytest_embedded_idf/serial.py` & `pytest_embedded_idf-1.8.2/pytest_embedded_idf/serial.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         **kwargs,
     ) -> None:
         self.app = app
         self.confirm_target_elf_sha256 = confirm_target_elf_sha256
         self.erase_nvs = erase_nvs
 
         if not hasattr(self.app, 'target'):
-            raise ValueError(f'Idf app not parsable. Please check if it\'s valid: {self.app.binary_path}')
+            raise ValueError(f"Idf app not parsable. Please check if it's valid: {self.app.binary_path}")
 
         if target and self.app.target and self.app.target != target:
             raise ValueError(f'Targets do not match. App target: {self.app.target}, Cmd target: {target}.')
 
         super().__init__(
             target=target or app.target,
             **kwargs,
@@ -104,50 +104,54 @@
                     '--no-stub',
                     'load_ram',
                     bin_file,
                 ],
                 esp=self.esp,
             )
 
-    def _force_flag(self):
+    def _force_flag(self, app: Optional[IdfApp] = None):
         if self.esp_flash_force:
             return ['--force']
 
-        if any(
-            (
-                self.app.sdkconfig.get('SECURE_FLASH_ENC_ENABLED', False),
-                self.app.sdkconfig.get('SECURE_BOOT', False),
-            )
-        ):
+        if app is None:
+            app = self.app
+
+        if any((
+            app.sdkconfig.get('SECURE_FLASH_ENC_ENABLED', False),
+            app.sdkconfig.get('SECURE_BOOT', False),
+        )):
             return ['--force']
 
         return []
 
     @EspSerial.use_esptool()
     def erase_flash(self, force: bool = False):
         if self._force_flag() or force:
             super().erase_flash(force=True)
         else:
             super().erase_flash()
 
     @EspSerial.use_esptool()
-    def flash(self) -> None:
+    def flash(self, app: Optional[IdfApp] = None) -> None:
         """
         Flash the `app.flash_files` to the dut
         """
-        if not self.app.flash_files:
+        if not app:
+            app = self.app
+
+        if not app.flash_files:
             logging.error('No flash files detected. Skipping auto flash...')
             return
 
-        if not self.app.flash_settings:
+        if not app.flash_settings:
             logging.error('No flash settings detected. Skipping auto flash...')
             return
 
         _args = []
-        for k, v in self.app.flash_args['extra_esptool_args'].items():
+        for k, v in app.flash_args['extra_esptool_args'].items():
             if isinstance(v, bool):
                 if k == 'stub':
                     if v is False:
                         _args.append('--no-stub')
                 elif v:
                     _args.append(f'--{k}')
             else:
@@ -159,43 +163,43 @@
 
         _args.append('write_flash')
 
         if self.erase_nvs:
             esptool.main(
                 [
                     'erase_region',
-                    str(self.app.partition_table['nvs']['offset']),
-                    str(self.app.partition_table['nvs']['size']),
+                    str(app.partition_table['nvs']['offset']),
+                    str(app.partition_table['nvs']['size']),
                 ],
                 esp=self.esp,
             )
             self.esp.connect()
 
         encrypt_files = []
         flash_files = []
-        for file in self.app.flash_files:
+        for file in app.flash_files:
             if file.encrypted:
                 encrypt_files.extend([hex(file.offset), str(file.file_path)])
             else:
                 flash_files.extend([hex(file.offset), str(file.file_path)])
 
         if flash_files and encrypt_files:
             _args.extend([*flash_files, '--encrypt-files', *encrypt_files])
         else:
             if flash_files:
                 _args.extend(flash_files)
             else:
                 _args.extend(['--encrypt', *encrypt_files])
 
-        _args.extend([*self.app.flash_args['write_flash_args'], *self._force_flag()])
+        _args.extend([*app.flash_args['write_flash_args'], *self._force_flag(app)])
 
         esptool.main(_args, esp=self.esp)
 
         if self._meta:
-            self._meta.set_port_app_cache(self.port, self.app)
+            self._meta.set_port_app_cache(self.port, app)
 
     @EspSerial.use_esptool()
     def dump_flash(
         self,
         partition: Optional[str] = None,
         address: Optional[str] = None,
         size: Optional[str] = None,
@@ -280,15 +284,15 @@
         """
         Check if the sha256 values are matched between the flashed target and the `self.app.elf_file`
 
         Returns:
             True if the sha256 values are matched
         """
         if not self.app.elf_file:
-            logging.info('no elf file. Can\'t tell if the target flashed the same elf file or not. Assume as False')
+            logging.info("no elf file. Can't tell if the target flashed the same elf file or not. Assume as False")
             return False
 
         flash_elf_sha256 = self.read_flash_elf_sha256()
         elf_sha256 = hashlib.sha256()
         with open(self.app.elf_file, 'rb') as fr:
             elf_sha256.update(fr.read())
```

### Comparing `pytest_embedded_idf-1.8.1/pytest_embedded_idf/unity_tester.py` & `pytest_embedded_idf-1.8.2/pytest_embedded_idf/unity_tester.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 DEFAULT_START_RETRY = 3
 DEFAULT_TIMEOUT = 90
 WAIT_FOR_MENU_TIMEOUT = 10
 
 READY_PATTERN_LIST = [
     'Press ENTER to see the list of tests',
     'Enter test for running',
-    'Enter next test, or \'enter\' to see menu',
+    "Enter next test, or 'enter' to see menu",
 ]
 
 
 @dataclass
 class UnittestMenuCase:
     """
     Dataclass of esp-idf unit test cases parsed from test menu
@@ -258,15 +258,15 @@
         @functools.wraps(func)
         def wrapper(self, *args, **kwargs):
             _start_at = time.perf_counter()  # declare here in case hard reset failed
             _timeout = kwargs.get('timeout', 30)
             _case = args[0]
 
             if _case.type not in func.__name__:
-                logging.warning('The %s case can\'t be executed with %s function.', _case.type, func.__name__)
+                logging.warning("The %s case can't be executed with %s function.", _case.type, func.__name__)
                 return
 
             try:
                 # do it here since the first hard reset before test case shouldn't be counted in duration time
                 if 'reset' in kwargs:
                     if kwargs.get('reset'):
                         self._hard_reset()
@@ -277,15 +277,15 @@
                 _timestamp = time.perf_counter()
                 _log = ''
                 try:
                     _timeout = _timeout - _timestamp + _start_at
                     if _timeout < 0:  # pexpect process would expect 30s if < 0
                         _timeout = 0
                     self.expect(UNITY_SUMMARY_LINE_REGEX, timeout=_timeout)
-                except Exception:  # result block missing # noqa
+                except Exception:  # result block missing
                     pass
                 else:  # result block exists
                     _log = remove_asci_color_code(self.pexpect_proc.before)
                 finally:
                     _end_at = time.perf_counter()
                     self._add_single_unity_test_case(
                         _case, _log, additional_attrs={'time': round(_end_at - _start_at, 3)}
@@ -447,15 +447,15 @@
     """
 
     # The signal pattens come from 'test_utils.c'
     SEND_SIGNAL_PREFIX = 'Send signal: '
     WAIT_SIGNAL_PREFIX = 'Waiting for signal: '
     UNITY_SEND_SIGNAL_REGEX = SEND_SIGNAL_PREFIX + r'\[(.*?)\]!'
     UNITY_WAIT_SIGNAL_REGEX = WAIT_SIGNAL_PREFIX + r'\[(.*?)\]!'
-    signal_pattern_list = [
+    signal_pattern_list: t.ClassVar[t.List[str]] = [
         UNITY_SEND_SIGNAL_REGEX,  # The dut send a signal
         UNITY_WAIT_SIGNAL_REGEX,  # The dut is blocked and waiting for a signal
         UNITY_SUMMARY_LINE_REGEX,  # Means the case finished
     ]
 
     DevResponse = namedtuple('DevResponse', ['completed', 'data'])
```

### Comparing `pytest_embedded_idf-1.8.1/tests/test_idf.py` & `pytest_embedded_idf-1.8.2/tests/test_idf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import platform
 import re
 import tempfile
 import xml.etree.ElementTree as ET
 
 import pytest
+
 from pytest_embedded_idf.dut import IdfDut
 
 toolchain_required = pytest.mark.skipif(
     os.getenv('PATH') is None or os.path.join('riscv32-esp-elf-gdb', 'bin') not in os.getenv('PATH'),
     reason="'riscv32-esp-elf-gdb' is not found in $PATH. The test execution will be skipped",
 )
 
@@ -387,15 +388,38 @@
         '--embedded-services', 'esp,idf',
         '--part-tool', os.path.join(testdir.tmpdir, 'gen_esp32part.py'),
     )
 
     result.assert_outcomes(passed=1)
 
 
-def test_no_elf_file(testdir):
+def test_flash_another_app(testdir):
+    testdir.makepyfile(r"""
+        import pytest
+        import pexpect
+
+        from pytest_embedded_idf import IdfApp
+
+        def test_flash_another_app(dut):
+            dut.serial.flash(IdfApp('{}'))
+            dut.expect('Hash of data verified.', timeout=5)
+            dut.expect_exact('Hello world!', timeout=5)
+    """.format(os.path.join(testdir.tmpdir, 'hello_world_esp32')))
+
+    result = testdir.runpytest(
+        '-s',
+        '--app-path', os.path.join(testdir.tmpdir, 'unit_test_app_esp32'),
+        '--embedded-services', 'esp,idf',
+        '--part-tool', os.path.join(testdir.tmpdir, 'gen_esp32part.py'),
+    )
+
+    result.assert_outcomes(passed=1)
+
+
+def test_flash_with_no_elf_file(testdir):
     testdir.makepyfile(r"""
          import pytest
          import pexpect
 
          def test_flash_with_no_elf_file(dut):
              dut.expect('Hash of data verified.', timeout=5)
              dut.expect_exact('Hello world!', timeout=5)
@@ -470,14 +494,15 @@
         '--embedded-services', 'idf',
         '--app-path', f'{os.path.join(testdir.tmpdir, "hello_world_linux")}',
         '--target', 'linux',
     )
 
     result.assert_outcomes(passed=1)
 
+
 @pytest.mark.skipif(platform.machine() != 'x86_64', reason='The test is intended to be run on an x86_64 machine.')
 def test_unity_tester_with_linux(testdir):
     testdir.makepyfile(r"""
 
     def test_unity_tester_with_linux(dut):
         dut.run_all_single_board_cases()
     """
```

### Comparing `pytest_embedded_idf-1.8.1/PKG-INFO` & `pytest_embedded_idf-1.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-idf
-Version: 1.8.1
+Version: 1.8.2
 Summary: Make pytest-embedded plugin work with ESP-IDF.
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
 Requires-Dist: esp-idf-panic-decoder
-Requires-Dist: pytest-embedded-serial-esp~=1.8.1 ; extra == "serial"
+Requires-Dist: pytest-embedded-serial-esp~=1.8.2 ; extra == "serial"
 Requires-Dist: esp-coredump~=1.0 ; extra == "serial"
 Project-URL: changelog, https://github.com/espressif/pytest-embedded/blob/main/CHANGELOG.md
 Project-URL: documentation, https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Project-URL: homepage, https://github.com/espressif/pytest-embedded
 Project-URL: repository, https://github.com/espressif/pytest-embedded
 Provides-Extra: serial
```

