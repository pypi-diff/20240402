# Comparing `tmp/pytest_embedded-1.8.1.tar.gz` & `tmp/pytest_embedded-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_embedded-1.8.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pytest_embedded-1.8.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest_embedded-1.8.1.tar` & `pytest_embedded-1.8.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1094 2024-03-01 10:19:36.931475 pytest_embedded-1.8.1/LICENSE
--rw-r--r--   0        0        0      120 2024-03-01 10:19:36.931475 pytest_embedded-1.8.1/README.md
--rw-r--r--   0        0        0     2996 2024-03-01 10:19:36.931475 pytest_embedded-1.8.1/pyproject.toml
--rw-r--r--   0        0        0      150 2024-03-01 10:19:36.931475 pytest_embedded-1.8.1/pytest_embedded/__init__.py
--rw-r--r--   0        0        0     1095 2024-03-01 10:19:36.931475 pytest_embedded-1.8.1/pytest_embedded/app.py
--rw-r--r--   0        0        0     7615 2024-03-01 10:19:36.931475 pytest_embedded-1.8.1/pytest_embedded/dut.py
--rw-r--r--   0        0        0     6886 2024-03-01 10:19:36.931475 pytest_embedded-1.8.1/pytest_embedded/log.py
--rw-r--r--   0        0        0    55918 2024-03-01 10:19:36.931475 pytest_embedded-1.8.1/pytest_embedded/plugin.py
--rw-r--r--   0        0        0    10803 2024-03-01 10:19:36.931475 pytest_embedded-1.8.1/pytest_embedded/unity.py
--rw-r--r--   0        0        0    10022 2024-03-01 10:19:36.931475 pytest_embedded-1.8.1/pytest_embedded/utils.py
--rw-r--r--   0        0        0    20794 2024-03-01 10:19:36.931475 pytest_embedded-1.8.1/tests/test_base.py
--rw-r--r--   0        0        0     1461 1970-01-01 00:00:00.000000 pytest_embedded-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1094 2024-04-02 08:52:22.108840 pytest_embedded-1.8.2/LICENSE
+-rw-r--r--   0        0        0      120 2024-04-02 08:52:22.108840 pytest_embedded-1.8.2/README.md
+-rw-r--r--   0        0        0     3345 2024-04-02 08:52:22.108840 pytest_embedded-1.8.2/pyproject.toml
+-rw-r--r--   0        0        0      150 2024-04-02 08:52:22.108840 pytest_embedded-1.8.2/pytest_embedded/__init__.py
+-rw-r--r--   0        0        0     1487 2024-04-02 08:52:22.108840 pytest_embedded-1.8.2/pytest_embedded/app.py
+-rw-r--r--   0        0        0     7556 2024-04-02 08:52:22.108840 pytest_embedded-1.8.2/pytest_embedded/dut.py
+-rw-r--r--   0        0        0     6852 2024-04-02 08:52:22.108840 pytest_embedded-1.8.2/pytest_embedded/log.py
+-rw-r--r--   0        0        0    55320 2024-04-02 08:52:22.108840 pytest_embedded-1.8.2/pytest_embedded/plugin.py
+-rw-r--r--   0        0        0    10807 2024-04-02 08:52:22.108840 pytest_embedded-1.8.2/pytest_embedded/unity.py
+-rw-r--r--   0        0        0    10022 2024-04-02 08:52:22.108840 pytest_embedded-1.8.2/pytest_embedded/utils.py
+-rw-r--r--   0        0        0    20777 2024-04-02 08:52:22.108840 pytest_embedded-1.8.2/tests/test_base.py
+-rw-r--r--   0        0        0     1461 1970-01-01 00:00:00.000000 pytest_embedded-1.8.2/PKG-INFO
```

### Comparing `pytest_embedded-1.8.1/LICENSE` & `pytest_embedded-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_embedded-1.8.1/pyproject.toml` & `pytest_embedded-1.8.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -37,67 +37,81 @@
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
 
 [project.entry-points."pytest11"]
 pytest_embedded = "pytest_embedded.plugin"
```

### Comparing `pytest_embedded-1.8.1/pytest_embedded/app.py` & `pytest_embedded-1.8.2/pytest_embedded/app.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,26 +18,34 @@
         build_dir: Optional[str] = None,
         **kwargs,
     ):
         if app_path is None:
             app_path = os.getcwd()
 
         self.app_path = os.path.realpath(app_path)
-        self.binary_path = self._get_binary_path(build_dir)
+        self.binary_path = self._get_binary_path(build_dir or 'build')
 
         for k, v in kwargs.items():
             setattr(self, k, v)
 
     def _get_binary_path(self, build_dir: Optional[str] = None) -> Optional[str]:
         if not build_dir:
             return None
 
-        if os.path.isdir(build_dir):
+        # if build_dir is an absolute path, use it directly
+        logging.debug(f'checking if {build_dir} is an absolute path...')
+        if os.path.isabs(build_dir):
             return os.path.realpath(build_dir)
 
-        logging.debug(f'{build_dir} doesn\'t exist. Treat it as a relative path...')
+        # try relative path based on app_path first
+        logging.debug(f'checking if {build_dir} exists in {self.app_path}...')
         path = os.path.join(self.app_path, build_dir)
         if os.path.isdir(path):
             return path
 
-        logging.debug(f'{path} doesn\'t exist.')
+        # try relative path based on cwd
+        logging.debug(f'checking if {build_dir} exists in {os.getcwd()}...')
+        if os.path.isdir(build_dir):
+            return os.path.realpath(build_dir)
+
+        logging.debug(f"{path} doesn't exist.")
         return None
```

### Comparing `pytest_embedded-1.8.1/pytest_embedded/dut.py` & `pytest_embedded-1.8.2/pytest_embedded/dut.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,27 +60,27 @@
 
     def write(self, s: AnyStr) -> None:
         """
         Write to the `MessageQueue` instance
         """
         self._q.put(to_bytes(s))
 
-    def _pexpect_func(func) -> Callable[..., Union[Match, AnyStr]]:  # noqa
-        @functools.wraps(func)  # noqa
+    def _pexpect_func(func) -> Callable[..., Union[Match, AnyStr]]:
+        @functools.wraps(func)
         def wrapper(
             self, pattern, *args, expect_all: bool = False, not_matching: List[Union[str, re.Pattern]] = (), **kwargs
         ) -> Union[Union[Match, AnyStr], List[Union[Match, AnyStr]]]:
             patterns = to_list(pattern)
             res = []
             while patterns:
                 try:
-                    index = func(self, pattern, *args, **kwargs)  # noqa
+                    index = func(self, pattern, *args, **kwargs)
                 except (pexpect.EOF, pexpect.TIMEOUT) as e:
                     debug_str = (
-                        f'Not found "{str(pattern)}"\n'
+                        f'Not found "{pattern!s}"\n'
                         f'Bytes in current buffer (color code eliminated): {self.pexpect_proc.buffer_debug_str}\n'
                         f'Please check the full log here: {self.logfile}'
                     )
                     raise e.__class__(debug_str) from e
 
                 if self.pexpect_proc.match in [pexpect.EOF, pexpect.TIMEOUT]:
                     res.append(self.pexpect_proc.before.rstrip())
@@ -104,16 +104,16 @@
             if len(res) == 1:
                 return res[0]
 
             return res
 
         return wrapper
 
-    @_pexpect_func  # noqa
-    def expect(self, pattern, **kwargs) -> Match:  # noqa
+    @_pexpect_func
+    def expect(self, pattern, **kwargs) -> Match:
         """
         Expect the `pattern` from the internal buffer. All the arguments will be passed to `pexpect.expect()`.
 
         Args:
             pattern: string, or compiled regex, or a list of string and compiled regex.
 
         Keyword Args:
@@ -126,16 +126,16 @@
             `AnyStr` or `re.Match`
 
             - `AnyStr`: if you're matching `pexpect.EOF` or `pexpect.TIMEOUT` to get all the current buffers.
             - `re.Match`: if matched given string.
         """
         return self.pexpect_proc.expect(pattern, **kwargs)
 
-    @_pexpect_func  # noqa
-    def expect_exact(self, pattern, **kwargs) -> Match:  # noqa
+    @_pexpect_func
+    def expect_exact(self, pattern, **kwargs) -> Match:
         """
         Expect the `pattern` from the internal buffer. All the arguments will be passed to `pexpect.expect_exact()`.
 
         Args:
             pattern: string, or a list of string
 
         Keyword Args:
```

### Comparing `pytest_embedded-1.8.1/pytest_embedded/log.py` & `pytest_embedded-1.8.2/pytest_embedded/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
                 raise EOF('Bad File Descriptor')
             raise
 
         s = self._decoder.decode(s, final=False)
         self._log(s, 'read')
         return s
 
-    def terminate(self, force=False):
+    def terminate(self, force=False):  # noqa
         """
         Close the temporary file stream and itself.
         """
         self.close()
 
 
 def live_print_call(*args, msg_queue: Optional[MessageQueue] = None, expect_returncode: int = 0, **kwargs):
@@ -173,22 +173,20 @@
         # we use real log file to record output, pipe-like file object won't be non-blocking.
         _log_file = os.path.join(logdir, f'{self.SOURCE.lower()}-{uuid.uuid4()}{logfile_extension}')
         self._fw = open(_log_file, 'w')
         self._logfile = _log_file
         self._logfile_offset = 0
         logging.debug(f'temp log file: {_log_file}')
 
-        kwargs.update(
-            {
-                'bufsize': 0,
-                'stdin': subprocess.PIPE,
-                'stdout': self._fw,
-                'stderr': self._fw,
-            }
-        )
+        kwargs.update({
+            'bufsize': 0,
+            'stdin': subprocess.PIPE,
+            'stdout': self._fw,
+            'stderr': self._fw,
+        })
 
         self._cmd = cmd
         logging.info('Executing %s', ' '.join(cmd) if isinstance(cmd, list) else cmd)
         super().__init__(cmd, **kwargs)
 
         # some sub classes does not need to redirect to the message queue, they use blocking-IO instead and
         # return the response immediately in `write()`
```

### Comparing `pytest_embedded-1.8.1/pytest_embedded/plugin.py` & `pytest_embedded-1.8.2/pytest_embedded/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,15 +267,15 @@
 ###########
 _COUNT = 1
 
 
 def _gte_one_int(v) -> int:
     try:
         v = int(v)
-    except Exception:  # noqa
+    except Exception:
         pass  # deal with it later
     else:
         if v >= 1:
             return v
 
     print('"count" value should be a integer greater or equal to 1')
     sys.exit(1)
@@ -394,15 +394,15 @@
                     current_kwargs[k] = getter(v)
                 else:
                     current_kwargs[k] = v
 
             if func.__name__ == 'dut_index':
                 current_kwargs['count'] = i
 
-            res = tuple(list(res) + [func(*args, **current_kwargs)])
+            res = tuple([*list(res), func(*args, **current_kwargs)])
 
         return res
 
     return wrapper
 
 
 def multi_dut_generator_fixture(
@@ -480,15 +480,15 @@
                         current_kwargs[k] = getter(v)
                     else:
                         current_kwargs[k] = v
 
                 try:
                     i_res = func(*args, **current_kwargs)
                     res.append(i_res)
-                except Exception:  # noqa
+                except Exception:
                     for item in res:  # close the earlier succeeded set up items
                         _close_or_terminate(item)
 
                     raise
 
             try:
                 yield res
@@ -1018,15 +1018,15 @@
             raise UnknownServiceError(s)
 
         try:
             importlib.import_module(SERVICE_LIB_NAMES[s].replace('-', '_'))
         except ModuleNotFoundError:
             raise PackageNotInstalledError(s)
 
-    return ['base'] + services
+    return ['base', *services]
 
 
 @dataclass
 class ClassCliOptions:
     classes: t.Dict[str, type]
     mixins: t.Dict[str, t.List[type]]
     kwargs: t.Dict[str, t.Dict[str, t.Any]]
@@ -1102,34 +1102,30 @@
         if fixture == 'app':
             kwargs['app'] = {'app_path': app_path, 'build_dir': build_dir}
             if 'idf' in _services:
                 if 'qemu' in _services:
                     from pytest_embedded_qemu import DEFAULT_IMAGE_FN, QemuApp
 
                     classes[fixture] = QemuApp
-                    kwargs[fixture].update(
-                        {
-                            'msg_queue': msg_queue,
-                            'part_tool': part_tool,
-                            'qemu_image_path': qemu_image_path,
-                            'skip_regenerate_image': skip_regenerate_image,
-                            'encrypt': encrypt,
-                            'keyfile': keyfile,
-                            'qemu_prog_path': qemu_prog_path,
-                        }
-                    )
+                    kwargs[fixture].update({
+                        'msg_queue': msg_queue,
+                        'part_tool': part_tool,
+                        'qemu_image_path': qemu_image_path,
+                        'skip_regenerate_image': skip_regenerate_image,
+                        'encrypt': encrypt,
+                        'keyfile': keyfile,
+                        'qemu_prog_path': qemu_prog_path,
+                    })
                 else:
                     from pytest_embedded_idf import IdfApp
 
                     classes[fixture] = IdfApp
-                    kwargs[fixture].update(
-                        {
-                            'part_tool': part_tool,
-                        }
-                    )
+                    kwargs[fixture].update({
+                        'part_tool': part_tool,
+                    })
             elif 'arduino' in _services:
                 from pytest_embedded_arduino import ArduinoApp
 
                 classes[fixture] = ArduinoApp
             else:
                 from .app import App
 
@@ -1153,30 +1149,26 @@
                     'erase_all': erase_all,
                     'meta': _meta,
                 }
                 if 'idf' in _services:
                     from pytest_embedded_idf import IdfSerial
 
                     classes[fixture] = IdfSerial
-                    kwargs[fixture].update(
-                        {
-                            'app': None,
-                            'confirm_target_elf_sha256': confirm_target_elf_sha256,
-                            'erase_nvs': erase_nvs,
-                        }
-                    )
+                    kwargs[fixture].update({
+                        'app': None,
+                        'confirm_target_elf_sha256': confirm_target_elf_sha256,
+                        'erase_nvs': erase_nvs,
+                    })
                 elif 'arduino' in _services:
                     from pytest_embedded_arduino import ArduinoSerial
 
                     classes[fixture] = ArduinoSerial
-                    kwargs[fixture].update(
-                        {
-                            'app': None,
-                        }
-                    )
+                    kwargs[fixture].update({
+                        'app': None,
+                    })
                 else:
                     from pytest_embedded_serial_esp import EspSerial
 
                     classes[fixture] = EspSerial
             elif 'serial' in _services or 'jtag' in _services:
                 from pytest_embedded_serial.serial import Serial
 
@@ -1235,23 +1227,21 @@
                     'dut_index': dut_index,
                 }
         elif fixture == 'wokwi':
             if 'wokwi' in _services:
                 from pytest_embedded_wokwi import WokwiCLI
 
                 classes[fixture] = WokwiCLI
-                kwargs[fixture].update(
-                    {
-                        'wokwi_cli_path': wokwi_cli_path,
-                        'wokwi_timeout': wokwi_timeout,
-                        'msg_queue': msg_queue,
-                        'app': None,
-                        'meta': _meta,
-                    }
-                )
+                kwargs[fixture].update({
+                    'wokwi_cli_path': wokwi_cli_path,
+                    'wokwi_timeout': wokwi_timeout,
+                    'msg_queue': msg_queue,
+                    'app': None,
+                    'meta': _meta,
+                })
         elif fixture == 'dut':
             classes[fixture] = Dut
             kwargs[fixture] = {
                 'pexpect_proc': pexpect_proc,
                 'msg_queue': msg_queue,
                 'app': None,
                 'pexpect_logfile': _pexpect_logfile,
@@ -1264,73 +1254,63 @@
 
                 mixins[fixture].append(IdfUnityDutMixin)
 
             if 'wokwi' in _services:
                 from pytest_embedded_wokwi import WokwiDut
 
                 classes[fixture] = WokwiDut
-                kwargs[fixture].update(
-                    {
-                        'wokwi': None,
-                    }
-                )
+                kwargs[fixture].update({
+                    'wokwi': None,
+                })
 
                 if 'idf' in _services:
                     from pytest_embedded_wokwi.idf import IDFFirmwareResolver
 
                     kwargs['wokwi'].update({'firmware_resolver': IDFFirmwareResolver()})
                 else:
                     raise SystemExit('wokwi service should be used together with idf service')
             elif 'qemu' in _services:
                 from pytest_embedded_qemu import QemuDut
 
                 classes[fixture] = QemuDut
-                kwargs[fixture].update(
-                    {
-                        'qemu': None,
-                    }
-                )
+                kwargs[fixture].update({
+                    'qemu': None,
+                })
             elif 'jtag' in _services:
                 if 'idf' in _services:
                     from pytest_embedded_idf import IdfDut
 
                     classes[fixture] = IdfDut
                 else:
                     from pytest_embedded_serial import SerialDut
 
                     classes[fixture] = SerialDut
 
-                kwargs[fixture].update(
-                    {
-                        'serial': None,
-                        'openocd': None,
-                        'gdb': None,
-                    }
-                )
+                kwargs[fixture].update({
+                    'serial': None,
+                    'openocd': None,
+                    'gdb': None,
+                })
             elif 'serial' in _services or 'esp' in _services:
                 if 'esp' in _services and 'idf' in _services:
                     from pytest_embedded_idf import IdfDut
 
                     classes[fixture] = IdfDut
-                    kwargs[fixture].update(
-                        {
-                            'skip_check_coredump': skip_check_coredump,
-                            'panic_output_decode_script': panic_output_decode_script,
-                        }
-                    )
+                    kwargs[fixture].update({
+                        'skip_check_coredump': skip_check_coredump,
+                        'panic_output_decode_script': panic_output_decode_script,
+                    })
                 else:
                     from pytest_embedded_serial import SerialDut
 
                     classes[fixture] = SerialDut
 
-                kwargs[fixture].update(
-                    {
-                        'serial': None,
-                    }
-                )
+                kwargs[fixture].update({
+                    'serial': None,
+                })
 
     return ClassCliOptions(classes, mixins, kwargs)
 
 
 ####################
 # Derived Fixtures #
 ####################
@@ -1539,15 +1519,15 @@
 
     @staticmethod
     def _pytest_fixturedef_get_kwargs(fixturedef: FixtureDef[t.Any], request: SubRequest) -> t.Dict[str, t.Any]:
         kwargs = {}
         for argname in fixturedef.argnames:
             fixdef = request._get_active_fixturedef(argname)
             assert fixdef.cached_result is not None
-            result, arg_cache_key, exc = fixdef.cached_result
+            result, _, _ = fixdef.cached_result
             request._check_scope(argname, request._scope, fixdef._scope)
             kwargs[argname] = result
 
         return kwargs
 
     @staticmethod
     def _pytest_fixturedef_exec(fixturedef: FixtureDef[t.Any], request: SubRequest, kwargs: t.Dict[str, t.Any]):
@@ -1585,17 +1565,17 @@
     @pytest.hookimpl(trylast=True)
     def pytest_collection_modifyitems(self, items: t.List[Function]):
         if self.check_duplicates:
             duplicated_test_cases = self._duplicate_items([test.name for test in items])
             if duplicated_test_cases:
                 raise ValueError(f'Duplicated test function names: {duplicated_test_cases}')
 
-            duplicated_test_script_paths = self._duplicate_items(
-                [os.path.basename(name) for name in set([str(test.path.absolute()) for test in items])]
-            )
+            duplicated_test_script_paths = self._duplicate_items([
+                os.path.basename(name) for name in set([str(test.path.absolute()) for test in items])
+            ])
             if duplicated_test_script_paths:
                 raise ValueError(f'Duplicated test scripts: {duplicated_test_script_paths}')
 
         if self.parallel_index == 1 and self.parallel_count == 1:
             return
 
         current_job_index = self.parallel_index - 1  # convert to 0-based index
@@ -1621,15 +1601,15 @@
     def pytest_runtest_call(self, item: Function):
         # raise dut failed cases
         if 'dut' in item.funcargs:
             duts = [dut for dut in to_list(item.funcargs['dut']) if isinstance(dut, Dut)]
             self._raise_dut_failed_cases_if_exists(duts)  # type: ignore
 
     @pytest.hookimpl(trylast=True)  # combine all possible junit reports should be the last step
-    def pytest_sessionfinish(self, session: Session, exitstatus: int) -> None:  # noqa
+    def pytest_sessionfinish(self, session: Session, exitstatus: int) -> None:
         modifier: JunitMerger = session.config.stash[_junit_merger_key]
         _stash_session_tempdir = session.config.stash.get(_session_tempdir_key, None)
         _stash_junit_report_path = session.config.stash.get(_junit_report_path_key, None)
         if _stash_session_tempdir is not None:
             modifier.merge(find_by_suffix('.xml', _stash_session_tempdir))
 
         if _stash_junit_report_path:
```

### Comparing `pytest_embedded-1.8.1/pytest_embedded/unity.py` & `pytest_embedded-1.8.2/pytest_embedded/unity.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     # TEST (        group_name,         case_name )             stdout
     r'TEST\((?P<group>[^\s,]+), (?P<name>[^\r\n)]+)\)(?P<stdout>[\S\s]*?)'
     #           foo.c:          100::                  FAIL           : Expected 2 was 1
     r'(?:(?P<file>.+):(?P<line>\d+)::)?(?P<result>PASS|FAIL|IGNORE)(?::(?P<message>.+))?'
 )
 
 UNITY_SUMMARY_LINE_REGEX = re.compile(
-    br'^[-]+\s*(\d+) Tests (\d+) Failures (\d+) Ignored\s*(?P<result>OK|FAIL)',
+    rb'^[-]+\s*(\d+) Tests (\d+) Failures (\d+) Ignored\s*(?P<result>OK|FAIL)',
     re.MULTILINE,
 )
 
 # https://www.w3.org/TR/xml11/#NT-Char
 # https://www.w3.org/TR/xml11/#NT-RestrictedChar
 _avoid_compatibility_chars = [
     (0x00, 0x08),
@@ -241,15 +241,15 @@
         for _dir, _junit_files in test_case_dir_sub_junit_files.items():
             merged_dut_junit_filepath = os.path.join(_dir, self.SUB_JUNIT_FILENAME)
 
             # multi-dut, multi junit files
             if len(_junit_files) > 1:
                 _data = None
                 for _junit_file in _junit_files:
-                    logging.info(f'Merging {_junit_file} to {merged_dut_junit_filepath}')
+                    logging.debug(f'Merging {_junit_file} to {merged_dut_junit_filepath}')
                     _junit = ET.parse(_junit_file)
                     _root = _junit.getroot()
 
                     if _data is None:
                         _data = _junit
                     else:
                         _data.getroot().extend(_root)
@@ -266,22 +266,22 @@
                             _data.getroot().attrib['tests'],
                             _root.attrib['tests'],
                         )
                 _data.write(merged_dut_junit_filepath)
             # multi-dut, single junit file
             elif _junit_files[0] != merged_dut_junit_filepath:
                 _junit_file = _junit_files[0]
-                logging.info(f'Rename {_junit_file} to {merged_dut_junit_filepath}')
+                logging.debug(f'Rename {_junit_file} to {merged_dut_junit_filepath}')
                 os.rename(_junit_file, merged_dut_junit_filepath)
 
             _merged_multi_dut_junit_files.append(merged_dut_junit_filepath)
 
         # second round, merge the test case junit report back to the main junit report
         for file in _merged_multi_dut_junit_files:
-            logging.info(f'Merging {file} to {self.junit_path}')
+            logging.debug(f'Merging {file} to {self.junit_path}')
             merging_xml = ET.parse(file)
             merging_cases = merging_xml.findall('testcase')
             merging_parent = merging_xml.getroot()
 
             # a normal file path should be /tmp/pytest-embedded/<test_case_name>/dut.xml
             test_case_name = os.path.basename(os.path.dirname(file))
             junit_parent = self.junit.find(f'.//testcase[@name="{test_case_name}"]...')
@@ -311,8 +311,8 @@
                 junit_parent.attrib['tests'], merging_parent.attrib['tests'], -1
             )
 
             if int(junit_parent.attrib['failures']) > 0:
                 self.failed = True
 
         self.junit.write(self.junit_path)
-        logging.info(f'Merged junit report dumped to {os.path.realpath(self.junit_path)}')
+        logging.debug(f'Merged junit report dumped to {os.path.realpath(self.junit_path)}')
```

### Comparing `pytest_embedded-1.8.1/pytest_embedded/utils.py` & `pytest_embedded-1.8.2/pytest_embedded/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,25 +144,25 @@
             if file.endswith(suffix):
                 res.append(os.path.join(root, file))
 
     return res
 
 
 _ANSI_COLOR_CODE_RE = re.compile(
-    r'''
+    r"""
     \x1B  # ESC
     (?:   # 7-bit C1 Fe (except CSI)
         [@-Z\\-_]
     |     # or [ for CSI, followed by a control sequence
         \[
         [0-?]*  # Parameter bytes
         [ -/]*  # Intermediate bytes
         [@-~]   # Final byte
     )
-''',
+""",
     re.VERBOSE,
 )
 
 
 def remove_asci_color_code(s: t.AnyStr) -> str:
     if isinstance(s, bytes):
         s = s.decode('utf-8', errors='ignore')
```

### Comparing `pytest_embedded-1.8.1/tests/test_base.py` & `pytest_embedded-1.8.2/tests/test_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
         name: str
         path = Path('.')
 
     # _Fake instances are used in order to pass `pytest_collection_modifyitems` hook
     fake_items = [_FakeItem(name='1'), _FakeItem(name='2'), _FakeItem(name='3'),
                   _FakeItem(name='4'), _FakeItem(name='5')]
     fake_plugin = PytestEmbedded(parallel_count, parallel_index)
-    fake_plugin.pytest_collection_modifyitems(fake_items)  # noqa
+    fake_plugin.pytest_collection_modifyitems(fake_items)
     assert len(fake_items) == res
 
 
 def test_expect(testdir):
     testdir.makepyfile(r"""
         import re
         import pexpect
@@ -487,15 +487,14 @@
 
     assert junit_report[0].get('name') == 'test_case'
     assert junit_report[0].find('failure') is not None
     assert junit_report[1].get('name') == 'test_case'
     assert junit_report[1].find('failure') is not None
 
 
-
 def test_duplicate_stdout_popen(testdir):
     testdir.makepyfile(r"""
         import pytest
         import pexpect
         import sys
         from pytest_embedded.log import DuplicateStdoutPopen
 
@@ -570,15 +569,15 @@
 
     assert "ValueError: Duplicated test scripts: ['test_duplicate_module.py']" in capsys.readouterr().out
 
 
 @pytest.mark.temp_disable_packages('pytest_embedded_serial', 'pytest_embedded_idf')
 def test_temp_disable_packages():
     with pytest.raises(ImportError):
-        import pytest_embedded_serial.serial  # noqa
+        import pytest_embedded_serial.serial
 
     with pytest.raises(ImportError):
         import pytest_embedded_serial  # noqa
 
     with pytest.raises(ImportError):
         import pytest_embedded_idf  # noqa
```

### Comparing `pytest_embedded-1.8.1/PKG-INFO` & `pytest_embedded-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-embedded
-Version: 1.8.1
+Version: 1.8.2
 Summary: A pytest plugin that designed for embedded testing.
 Author-email: Fu Hanxi <fuhanxi@espressif.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
```

