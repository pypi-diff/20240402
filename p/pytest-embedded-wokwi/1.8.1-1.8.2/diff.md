# Comparing `tmp/pytest_embedded_wokwi-1.8.1.tar.gz` & `tmp/pytest_embedded_wokwi-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_embedded_wokwi-1.8.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pytest_embedded_wokwi-1.8.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest_embedded_wokwi-1.8.1.tar` & `pytest_embedded_wokwi-1.8.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1094 2024-03-01 10:19:36.931475 pytest_embedded_wokwi-1.8.1/LICENSE
--rw-r--r--   0        0        0     1911 2024-03-01 10:19:36.931475 pytest_embedded_wokwi-1.8.1/README.md
--rw-r--r--   0        0        0     3071 2024-03-01 10:19:36.931475 pytest_embedded_wokwi-1.8.1/pyproject.toml
--rw-r--r--   0        0        0      204 2024-03-01 10:19:36.931475 pytest_embedded_wokwi-1.8.1/pytest_embedded_wokwi/__init__.py
--rw-r--r--   0        0        0      434 2024-03-01 10:19:36.931475 pytest_embedded_wokwi-1.8.1/pytest_embedded_wokwi/dut.py
--rw-r--r--   0        0        0      293 2024-03-01 10:19:36.931475 pytest_embedded_wokwi-1.8.1/pytest_embedded_wokwi/idf.py
--rw-r--r--   0        0        0     4126 2024-03-01 10:19:36.931475 pytest_embedded_wokwi-1.8.1/pytest_embedded_wokwi/wokwi_cli.py
--rw-r--r--   0        0        0     1086 2024-03-01 10:19:36.931475 pytest_embedded_wokwi-1.8.1/tests/test_wokwi.py
--rw-r--r--   0        0        0     3377 1970-01-01 00:00:00.000000 pytest_embedded_wokwi-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1094 2024-04-02 08:52:22.108840 pytest_embedded_wokwi-1.8.2/LICENSE
+-rw-r--r--   0        0        0     1911 2024-04-02 08:52:22.108840 pytest_embedded_wokwi-1.8.2/README.md
+-rw-r--r--   0        0        0     3420 2024-04-02 08:52:22.108840 pytest_embedded_wokwi-1.8.2/pyproject.toml
+-rw-r--r--   0        0        0      188 2024-04-02 08:52:22.108840 pytest_embedded_wokwi-1.8.2/pytest_embedded_wokwi/__init__.py
+-rw-r--r--   0        0        0      434 2024-04-02 08:52:22.108840 pytest_embedded_wokwi-1.8.2/pytest_embedded_wokwi/dut.py
+-rw-r--r--   0        0        0      293 2024-04-02 08:52:22.108840 pytest_embedded_wokwi-1.8.2/pytest_embedded_wokwi/idf.py
+-rw-r--r--   0        0        0     4112 2024-04-02 08:52:22.108840 pytest_embedded_wokwi-1.8.2/pytest_embedded_wokwi/wokwi_cli.py
+-rw-r--r--   0        0        0     1086 2024-04-02 08:52:22.108840 pytest_embedded_wokwi-1.8.2/tests/test_wokwi.py
+-rw-r--r--   0        0        0     3377 1970-01-01 00:00:00.000000 pytest_embedded_wokwi-1.8.2/PKG-INFO
```

### Comparing `pytest_embedded_wokwi-1.8.1/LICENSE` & `pytest_embedded_wokwi-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_embedded_wokwi-1.8.1/README.md` & `pytest_embedded_wokwi-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `pytest_embedded_wokwi-1.8.1/pyproject.toml` & `pytest_embedded_wokwi-1.8.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -27,82 +27,96 @@
     "Programming Language :: Python",
     "Topic :: Software Development :: Testing",
 ]
 dynamic = ["version", "description"]
 requires-python = ">=3.7"
 
 dependencies = [
-    "pytest-embedded~=1.8.1",
+    "pytest-embedded~=1.8.2",
     "toml~=0.10.2",
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

### Comparing `pytest_embedded_wokwi-1.8.1/pytest_embedded_wokwi/wokwi_cli.py` & `pytest_embedded_wokwi-1.8.2/pytest_embedded_wokwi/wokwi_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         app = self.app
         flasher_args = self.firmware_resolver.resolve_firmware(app)
         wokwi_toml_path = os.path.join(app.app_path, 'wokwi.toml')
         firmware_path = Path(flasher_args).relative_to(app.app_path).as_posix()
         elf_path = Path(app.elf_file).relative_to(app.app_path).as_posix()
 
         if os.path.exists(wokwi_toml_path):
-            with open(wokwi_toml_path, 'rt') as f:
+            with open(wokwi_toml_path) as f:
                 toml_data = toml.load(f)
 
             if 'wokwi' not in toml_data:
                 toml_data['wokwi'] = {'version': 1}
 
             wokwi_table = toml_data['wokwi']
             if wokwi_table.get('firmware') == firmware_path and wokwi_table.get('elf') == elf_path:
@@ -92,24 +92,24 @@
                     'version': 1,
                     'generatedBy': f'pytest-embedded-wokwi {__version__}',
                     'firmware': firmware_path,
                     'elf': elf_path,
                 }
             }
 
-        with open(wokwi_toml_path, 'wt') as f:
+        with open(wokwi_toml_path, 'w') as f:
             toml.dump(toml_data, f)
 
     def create_diagram_json(self):
         app = self.app
         diagram_json_path = os.path.join(app.app_path, 'diagram.json')
         target_board = target_to_board[app.target]
 
         if os.path.exists(diagram_json_path):
-            with open(diagram_json_path, 'rt') as f:
+            with open(diagram_json_path) as f:
                 json_data = json.load(f)
             if not any(part['type'] == target_board for part in json_data['parts']):
                 logging.warning(
                     f'diagram.json exists, no part with type "{target_board}" found. '
                     + 'You may need to update the diagram.json file manually to match the target board.'
                 )
             return
@@ -120,15 +120,15 @@
             'editor': 'wokwi',
             'parts': [{'type': target_board, 'id': 'esp'}],
             'connections': [
                 ['esp:TX', '$serialMonitor:RX', ''],
                 ['esp:RX', '$serialMonitor:TX', ''],
             ],
         }
-        with open(diagram_json_path, 'wt') as f:
+        with open(diagram_json_path, 'w') as f:
             f.write(json.dumps(diagram, indent=2))
 
     def _hard_reset(self):
         """
         This is a fake hard_reset. Keep this API to keep the consistency.
         """
         raise NotImplementedError
```

### Comparing `pytest_embedded_wokwi-1.8.1/tests/test_wokwi.py` & `pytest_embedded_wokwi-1.8.2/tests/test_wokwi.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_wokwi-1.8.1/PKG-INFO` & `pytest_embedded_wokwi-1.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-wokwi
-Version: 1.8.1
+Version: 1.8.2
 Summary: Make pytest-embedded plugin work with the Wokwi CLI.
 Author-email: Fu Hanxi <fuhanxi@espressif.com>, Uri Shaked <uri@wokwi.com>
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
 Requires-Dist: toml~=0.10.2
-Requires-Dist: pytest-embedded-idf~=1.8.1 ; extra == "idf"
+Requires-Dist: pytest-embedded-idf~=1.8.2 ; extra == "idf"
 Project-URL: changelog, https://github.com/espressif/pytest-embedded/blob/main/CHANGELOG.md
 Project-URL: documentation, https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Project-URL: homepage, https://github.com/espressif/pytest-embedded
 Project-URL: repository, https://github.com/espressif/pytest-embedded
 Provides-Extra: idf
 
 ### pytest-embedded-wokwi
```

