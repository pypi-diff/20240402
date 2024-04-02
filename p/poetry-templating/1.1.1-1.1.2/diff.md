# Comparing `tmp/poetry_templating-1.1.1.tar.gz` & `tmp/poetry_templating-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_templating-1.1.1.tar", max compression
+gzip compressed data, was "poetry_templating-1.1.2.tar", max compression
```

## Comparing `poetry_templating-1.1.1.tar` & `poetry_templating-1.1.2.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      945 2024-02-05 12:57:06.681234 poetry_templating-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     4562 2024-01-09 18:45:40.644342 poetry_templating-1.1.1/README.md
--rw-r--r--   0        0        0      167 2024-02-05 12:59:54.665219 poetry_templating-1.1.1/src/poetry_templating/__init__.py
--rw-r--r--   0        0        0     7421 2024-01-09 18:29:02.346885 poetry_templating-1.1.1/src/poetry_templating/engine.py
--rw-r--r--   0        0        0      564 2024-02-05 12:59:54.660703 poetry_templating-1.1.1/src/poetry_templating/error.py
--rw-r--r--   0        0        0     3891 2024-02-05 12:59:54.662204 poetry_templating-1.1.1/src/poetry_templating/plugin.py
--rw-r--r--   0        0        0     6219 2024-02-05 12:59:54.663715 poetry_templating-1.1.1/src/poetry_templating/util.py
--rw-r--r--   0        0        0     5218 1970-01-01 00:00:00.000000 poetry_templating-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-02 13:15:30.083359 poetry_templating-1.1.2/LICENCE
+-rw-r--r--   0        0        0     4411 2024-04-02 13:15:30.083359 poetry_templating-1.1.2/README.md
+-rw-r--r--   0        0        0      910 2024-04-02 13:15:30.087359 poetry_templating-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      160 2024-04-02 13:15:30.863363 poetry_templating-1.1.2/src/poetry_templating/__init__.py
+-rw-r--r--   0        0        0     7192 2024-04-02 13:15:30.087359 poetry_templating-1.1.2/src/poetry_templating/engine.py
+-rw-r--r--   0        0        0      544 2024-04-02 13:15:30.867363 poetry_templating-1.1.2/src/poetry_templating/error.py
+-rw-r--r--   0        0        0     4113 2024-04-02 13:15:30.863363 poetry_templating-1.1.2/src/poetry_templating/plugin.py
+-rw-r--r--   0        0        0     6009 2024-04-02 13:15:30.863363 poetry_templating-1.1.2/src/poetry_templating/util.py
+-rw-r--r--   0        0        0     5218 1970-01-01 00:00:00.000000 poetry_templating-1.1.2/PKG-INFO
```

### Comparing `poetry_templating-1.1.1/pyproject.toml` & `poetry_templating-1.1.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-[tool.poetry]
-name = "poetry-templating"
-version = "1.1.1"
-description = "A plugin for poetry which lets you substitute text on build."
-authors = ["NimajnebEC <nimajnebec@users.noreply.github.com>"]
-repository = "https://github.com/NimajnebEC/poetry-templating"
-packages = [{ include = "poetry_templating", from = "src" }]
-readme = "README.md"
-license = "MIT"
-
-[tool.poetry.dependencies]
-python = ">= 3.8, < 3.13"
-poetry = "^1.7.1"
-
-[tool.poetry.group.dev.dependencies]
-coveralls = "^3.3.1"
-pytest = "^7.4.3"
-ruff = "^0.1.7"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.poetry.plugins."poetry.application.plugin"]
-templating = "poetry_templating.plugin:TemplatingPlugin"
-
-[tool.poetry-templating]
-exclude = ["src/poetry_templating/engine.py", "tests/*"]
-
-[tool.ruff]
-line-length = 92
-
-[tool.coverage.run]
-source = ["poetry_templating"]
-command_line = "-m pytest"
+[tool.poetry]
+name = "poetry-templating"
+version = "1.1.2"
+description = "A plugin for poetry which lets you substitute text on build."
+authors = ["NimajnebEC <nimajnebec@users.noreply.github.com>"]
+repository = "https://github.com/NimajnebEC/poetry-templating"
+packages = [{ include = "poetry_templating", from = "src" }]
+readme = "README.md"
+license = "MIT"
+
+[tool.poetry.dependencies]
+python = ">= 3.8, < 3.13"
+poetry = "^1.8.0"
+
+[tool.poetry.group.dev.dependencies]
+coveralls = "^3.3.1"
+pytest = "^7.4.3"
+ruff = "^0.1.7"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.poetry.plugins."poetry.application.plugin"]
+templating = "poetry_templating.plugin:TemplatingPlugin"
+
+[tool.poetry-templating]
+exclude = ["src/poetry_templating/engine.py", "tests/*"]
+
+[tool.ruff]
+line-length = 92
+
+[tool.coverage.run]
+source = ["poetry_templating"]
+command_line = "-m pytest"
```

### Comparing `poetry_templating-1.1.1/README.md` & `poetry_templating-1.1.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,151 +1,172 @@
-# Templating Poetry Plugin
-
-[![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
-[![PyPI - Version](https://img.shields.io/pypi/v/poetry-templating)
-](https://pypi.org/project/poetry-templating/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/poetry-templating)](https://pypi.org/project/poetry-templating/)
-[![Coverage Status](https://img.shields.io/coverallsCoverage/github/NimajnebEC/poetry-templating)](https://coveralls.io/github/NimajnebEC/poetry-templating?branch=main)
-[![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/nimajnebec/poetry-templating/test.yml)
-](https://github.com/NimajnebEC/poetry-templating/actions)
-
-A plugin for [Poetry](https://python-poetry.org/) which lets you substitute text on build. This plugin was created to allow you to keep a single source of truth for package wide properties such as version and author.
-
-## Installation
-
-The easiest way to install the plugin is via the [`self add`](https://python-poetry.org/docs/cli/#self-add) command of Poetry.
-
-```
-poetry self add poetry-templating
-```
-
-If you used `pipx` to install Poetry you can add the plugin via the `pipx inject` command.
-
-```
-pipx inject poetry poetry-templating
-```
-
-Otherwise, if you used `pip` to install Poetry you can add the plugin packages via the `pip install` command.
-
-```
-pip install poetry-templating
-```
-
-## Usage
-
-Poetry Templating uses 'template slots' as placeholders and definitions for what they should be replaced with. Consider the following file:
-
-```py
-__version__ = "${pyproject.tool.poetry.version}"
-```
-
-When evaluated, the slot will be replaced with the `tool.poetry.version` property from `pyproject.toml`, for example:
-
-```py
-__version__ = "1.2.3"
-```
-
-Slots can also be used in conjunction with comments to add entire lines only present in the built package. This can be used with `# templating: delete` to significantly change functionality in the built package, for example:
-
-```py
-production = false # templating: delete
-# ${"production = true"}
-
-becomes
-
-production = true
-```
-
-## Evaluating Templates
-
-Poetry Templating will automatically evaluate template slots when building the package distributables with the `poetry build` command. You can also evaluate the project in-place by running the `poetry templating evaluate` command.
-
-## Constructs
-
-Poetry Templating features a number of constructs which can be used in template slots.
-
-### Literal Construct
-
-Denoted by quotes or double quotes, literal constructs simply replace the slot with the text within.
-
-```
-${"Hello World"}
-
-becomes
-
-Hello World
-```
-
-Template slots within literal constructs are also evaluated, allowing for basic string concatenation, for example:
-
-```py
-# ${"__version__ = ${pyproject.tool.poetry.version}"}
-
-becomes
-
-__version__ = "1.2.3"
-
-```
-
-### PyProject Construct
-
-Allows you to refernce values from the package's `pyproject.toml` file.
-
-```
-${pyproject.tool.poetry.version}
-${pyproject.tool.poetry.authors.0}
-
-becomes
-
-1.2.3
-John Doe <john.doe@example.com
-```
-
-### Environment Variable Construct
-
-Allows you to reference the buildtime environment variables.
-
-```
-${env.HOME}
-
-becomes
-
-/home/example/
-```
-
-### File Construct
-
-Denoted with a forward slash, or `./` for relative files, the file construct gets the entire content of an arbitrary file.
-
-```
-${/LICENCE}
-
-becomes
-
-MIT License
-
-Permission is hereby granted ...
-```
-
-## Configuration
-
-Poetry Templating can be configured in your `pyproject.toml` file under the `tool.poetry-templating` table.
-
-| key      | default   | description                                                                    |
-| -------- | --------- | ------------------------------------------------------------------------------ |
-| encoding | "utf-8"   | The text encoding to use when processing files.                                |
-| include  | ["\*.py"] | A list of glob patterns for files to process.                                  |
-| exclude  | []        | A list of glob patterns for files not to process, has priority over `include`. |
-
-Poetry Templating can also be enabled and disabled within a single file:
-
-```py
-# templating: off
-example = "${'will NOT get evaluated'}"
-# templating: on
-evaluated = "${'WILL get evaluated'}"
-
-becomes
-
-example = "${'will NOT get evaluated'}"
-evaluated = "WILL get evaluated"
-```
+Metadata-Version: 2.1
+Name: poetry-templating
+Version: 1.1.2
+Summary: A plugin for poetry which lets you substitute text on build.
+Home-page: https://github.com/NimajnebEC/poetry-templating
+License: MIT
+Author: NimajnebEC
+Author-email: nimajnebec@users.noreply.github.com
+Requires-Python: >=3.8,<3.13
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: poetry (>=1.8.0,<2.0.0)
+Project-URL: Repository, https://github.com/NimajnebEC/poetry-templating
+Description-Content-Type: text/markdown
+
+# Templating Poetry Plugin
+
+[![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
+[![PyPI - Version](https://img.shields.io/pypi/v/poetry-templating)
+](https://pypi.org/project/poetry-templating/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/poetry-templating)](https://pypi.org/project/poetry-templating/)
+[![Coverage Status](https://img.shields.io/coverallsCoverage/github/NimajnebEC/poetry-templating)](https://coveralls.io/github/NimajnebEC/poetry-templating?branch=main)
+[![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/nimajnebec/poetry-templating/test.yml)
+](https://github.com/NimajnebEC/poetry-templating/actions)
+
+A plugin for [Poetry](https://python-poetry.org/) which lets you substitute text on build. This plugin was created to allow you to keep a single source of truth for package wide properties such as version and author.
+
+## Installation
+
+The easiest way to install the plugin is via the [`self add`](https://python-poetry.org/docs/cli/#self-add) command of Poetry.
+
+```
+poetry self add poetry-templating
+```
+
+If you used `pipx` to install Poetry you can add the plugin via the `pipx inject` command.
+
+```
+pipx inject poetry poetry-templating
+```
+
+Otherwise, if you used `pip` to install Poetry you can add the plugin packages via the `pip install` command.
+
+```
+pip install poetry-templating
+```
+
+## Usage
+
+Poetry Templating uses 'template slots' as placeholders and definitions for what they should be replaced with. Consider the following file:
+
+```py
+__version__ = "${pyproject.tool.poetry.version}"
+```
+
+When evaluated, the slot will be replaced with the `tool.poetry.version` property from `pyproject.toml`, for example:
+
+```py
+__version__ = "1.2.3"
+```
+
+Slots can also be used in conjunction with comments to add entire lines only present in the built package. This can be used with `# templating: delete` to significantly change functionality in the built package, for example:
+
+```py
+production = false # templating: delete
+# ${"production = true"}
+
+becomes
+
+production = true
+```
+
+## Evaluating Templates
+
+Poetry Templating will automatically evaluate template slots when building the package distributables with the `poetry build` command. You can also evaluate the project in-place by running the `poetry templating evaluate` command.
+
+## Constructs
+
+Poetry Templating features a number of constructs which can be used in template slots.
+
+### Literal Construct
+
+Denoted by quotes or double quotes, literal constructs simply replace the slot with the text within.
+
+```
+${"Hello World"}
+
+becomes
+
+Hello World
+```
+
+Template slots within literal constructs are also evaluated, allowing for basic string concatenation, for example:
+
+```py
+# ${"__version__ = ${pyproject.tool.poetry.version}"}
+
+becomes
+
+__version__ = "1.2.3"
+
+```
+
+### PyProject Construct
+
+Allows you to refernce values from the package's `pyproject.toml` file.
+
+```
+${pyproject.tool.poetry.version}
+${pyproject.tool.poetry.authors.0}
+
+becomes
+
+1.2.3
+John Doe <john.doe@example.com
+```
+
+### Environment Variable Construct
+
+Allows you to reference the buildtime environment variables.
+
+```
+${env.HOME}
+
+becomes
+
+/home/example/
+```
+
+### File Construct
+
+Denoted with a forward slash, or `./` for relative files, the file construct gets the entire content of an arbitrary file.
+
+```
+${/LICENCE}
+
+becomes
+
+MIT License
+
+Permission is hereby granted ...
+```
+
+## Configuration
+
+Poetry Templating can be configured in your `pyproject.toml` file under the `tool.poetry-templating` table.
+
+| key      | default   | description                                                                    |
+| -------- | --------- | ------------------------------------------------------------------------------ |
+| encoding | "utf-8"   | The text encoding to use when processing files.                                |
+| include  | ["\*.py"] | A list of glob patterns for files to process.                                  |
+| exclude  | []        | A list of glob patterns for files not to process, has priority over `include`. |
+
+Poetry Templating can also be enabled and disabled within a single file:
+
+```py
+# templating: off
+example = "${'will NOT get evaluated'}"
+# templating: on
+evaluated = "${'WILL get evaluated'}"
+
+becomes
+
+example = "${'will NOT get evaluated'}"
+evaluated = "WILL get evaluated"
+```
+
```

### Comparing `poetry_templating-1.1.1/src/poetry_templating/engine.py` & `poetry_templating-1.1.2/src/poetry_templating/engine.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,229 +1,229 @@
-from __future__ import annotations
-
-import logging
-import os
-import re
-from pathlib import Path
-from re import Match, Pattern
-from typing import Callable, List, Optional, Union
-
-from poetry.core.pyproject.toml import PyProjectTOML
-
-from poetry_templating import DEFAULT_ENCODING, DEFAULT_EXCLUDE, DEFAULT_INCLUDE
-from poetry_templating.error import EvaluationError
-from poetry_templating.util import (
-    StrPath,
-    get_configuration,
-    get_listable,
-    matches_any,
-    relative,
-    traverse,
-)
-
-RE_TEMPLATE_SLOT = re.compile(r"(?:#\s*)?\${(.+)}")
-
-RE_DISABLE = re.compile(r"^\s*#\s*templating: off\s*$", re.IGNORECASE)
-RE_ENABLE = re.compile(r"^\s*#\s*templating: on\s*$", re.IGNORECASE)
-RE_DELETE = re.compile(r"#\s*templating: delete", re.IGNORECASE)
-
-_log = logging.getLogger(__name__)
-
-
-class TemplatingEngine:
-    """The Templating Engine class is responsible for processing strings and substituting template slots with their evaluated values."""
-
-    def __init__(self, pyproject: PyProjectTOML) -> None:
-        """The Templating Engine class is responsible for processing strings and substituting template slots with their evaluated values.
-
-        Parameters
-        ----------
-        pyproject : PyProjectTOML
-            The pyproject.toml of the parent package.
-        """
-        self.processed: List[str] = []
-        self.pyproject: PyProjectTOML = pyproject
-        self.root = os.path.dirname(pyproject.path)
-
-        # Get configuration
-        configuration = get_configuration(pyproject)
-        self.encoding = configuration.get("encoding", DEFAULT_ENCODING)
-        self.include = get_listable(configuration, "include", DEFAULT_INCLUDE)
-        self.exclude = get_listable(configuration, "exclude", DEFAULT_EXCLUDE)
-
-    def relative(self, path: StrPath) -> Path:
-        return relative(path, self.root)
-
-    def set_processed(self, path: StrPath) -> None:
-        rel = self.relative(path)
-        self.processed.append(rel.as_posix())
-
-    def should_process(self, path: StrPath) -> bool:
-        rel = self.relative(path)
-        return (
-            rel.as_posix() not in self.processed
-            and matches_any(rel, self.include)
-            and not matches_any(rel, self.exclude)
-        )
-
-    def evaluate_and_replace(self) -> int:
-        count = 0
-        for path in (os.path.join(p, f) for p, _, fs in os.walk(self.root) for f in fs):
-            if self.should_process(path):
-                count += 1
-                result = ""
-                ctx = EvaluationContext(path, self)
-                with open(path, "r+") as file:
-                    for line in file:
-                        evaluated = ctx.evaluate_line(line)
-                        if evaluated is not None:
-                            result += evaluated
-                    file.seek(0)
-                    file.write(result)
-                    file.truncate()
-                self.set_processed(path)
-
-        return count
-
-    def evaluate_string(
-        self,
-        data: str,
-        location: Optional[StrPath] = None,
-    ) -> str:
-        result: List[str] = []
-        ctx = EvaluationContext(location, self)
-        for line in data.split("\n"):
-            evaluated = ctx.evaluate_line(line)
-            if evaluated is not None:
-                result.append(evaluated)
-
-        if location is not None:
-            self.set_processed(location)
-
-        return "\n".join(result)
-
-
-class EvaluationContext:
-    def __init__(
-        self,
-        location: Optional[StrPath],
-        engine: TemplatingEngine,
-    ) -> None:
-        self.location = location and engine.relative(location)
-        self.engine = engine
-        self.enabled = True
-        self.line = -1
-
-    def evaluate_line(self, data: str) -> Union[str, None]:
-        self.line += 1
-
-        # Check for on/off comment
-        if RE_DISABLE.match(data):
-            self.enabled = False
-            return None
-        if RE_ENABLE.match(data):
-            self.enabled = True
-            return None
-
-        # Process line
-        if self.enabled:
-            # Skip if ends with delete comment
-            if RE_DELETE.search(data):
-                return None
-
-            return self.evaluate_string(data)
-        else:
-            return data
-
-    def evaluate_string(self, data: str) -> str:
-        return RE_TEMPLATE_SLOT.sub(self._evaluate_slot, data)
-
-    def _evaluate_slot(self, match: re.Match) -> str:
-        content = match.group(1)
-        for construct in Construct.constructs:
-            check = construct.pattern.match(content)
-            if check is not None:
-                try:
-                    return construct.handler(check, self)
-                except Exception as e:
-                    if isinstance(e, EvaluationError):
-                        raise
-                    raise EvaluationError(self, e) from e  # pragma: no cover
-        raise EvaluationError(self, "Unknown Construct")
-
-
-class Construct:
-    constructs: List["Construct"] = []
-
-    def __init__(
-        self,
-        pattern: Pattern,
-        handler: Callable[[Match, EvaluationContext], str],
-    ) -> None:
-        Construct.constructs.append(self)
-        self.handler = handler
-        self.pattern = pattern
-
-    @staticmethod
-    def construct(
-        pattern: Union[Pattern, str],
-    ) -> Callable[[Callable[[Match, EvaluationContext], str]], Construct]:
-        if isinstance(pattern, str):
-            pattern = re.compile(pattern)
-
-        def wrapper(func: Callable[[Match, EvaluationContext], str]) -> Construct:
-            return Construct(pattern, func)
-
-        return wrapper
-
-
-# Define Constructs
-
-
-@Construct.construct("^[\"'](.+)[\"']$")
-def literal_construct(match: Match, ctx: EvaluationContext) -> str:
-    return ctx.evaluate_string(match.group(1))
-
-
-@Construct.construct(r"^pyproject((?:\.[^.]+)+)?$")
-def pyproject_construct(match: Match, ctx: EvaluationContext) -> str:
-    path = match.group(1)
-
-    if path is None:
-        return str(ctx.engine.pyproject.data)
-
-    result = traverse(ctx.engine.pyproject.data, path[1:])
-    return str(result)
-
-
-@Construct.construct(r"^(\.?(?:\/.+)+)$")
-def file_construct(match: Match, ctx: EvaluationContext) -> str:
-    path: str = match.group(1)
-
-    if path.startswith("/"):
-        path = os.path.join(ctx.engine.root, path[1:])
-    else:
-        if ctx.location is None:
-            raise EvaluationError(ctx, "Relative paths are not permitted in this context")
-        path = os.path.join(ctx.engine.root, os.path.dirname(ctx.location), path)
-
-    if not os.path.isfile(path):
-        raise EvaluationError(ctx, f'No such file "{os.path.abspath(path)}"')
-
-    with open(path, "r", encoding=ctx.engine.encoding) as f:
-        content = f.read()
-        if ctx.engine.should_process(path):
-            content = ctx.engine.evaluate_string(content, path)
-        return content
-
-
-@Construct.construct(r"^env(?:\.([^\.\s]+))?$")
-def environ_construct(match: Match, ctx: EvaluationContext) -> str:
-    key = match.group(1)
-
-    if key is None:
-        return str(dict(os.environ))
-
-    if key not in os.environ:
-        raise EvaluationError(ctx, f"No environment variable '{key}'")
-
-    return os.environ[key]
+from __future__ import annotations
+
+import logging
+import os
+import re
+from pathlib import Path
+from re import Match, Pattern
+from typing import Callable, List, Optional, Union
+
+from poetry.core.pyproject.toml import PyProjectTOML
+
+from poetry_templating import DEFAULT_ENCODING, DEFAULT_EXCLUDE, DEFAULT_INCLUDE
+from poetry_templating.error import EvaluationError
+from poetry_templating.util import (
+    StrPath,
+    get_configuration,
+    get_listable,
+    matches_any,
+    relative,
+    traverse,
+)
+
+RE_TEMPLATE_SLOT = re.compile(r"(?:#\s*)?\${(.+)}")
+
+RE_DISABLE = re.compile(r"^\s*#\s*templating: off\s*$", re.IGNORECASE)
+RE_ENABLE = re.compile(r"^\s*#\s*templating: on\s*$", re.IGNORECASE)
+RE_DELETE = re.compile(r"#\s*templating: delete", re.IGNORECASE)
+
+_log = logging.getLogger(__name__)
+
+
+class TemplatingEngine:
+    """The Templating Engine class is responsible for processing strings and substituting template slots with their evaluated values."""
+
+    def __init__(self, pyproject: PyProjectTOML) -> None:
+        """The Templating Engine class is responsible for processing strings and substituting template slots with their evaluated values.
+
+        Parameters
+        ----------
+        pyproject : PyProjectTOML
+            The pyproject.toml of the parent package.
+        """
+        self.processed: List[str] = []
+        self.pyproject: PyProjectTOML = pyproject
+        self.root = os.path.dirname(pyproject.path)
+
+        # Get configuration
+        configuration = get_configuration(pyproject)
+        self.encoding = configuration.get("encoding", DEFAULT_ENCODING)
+        self.include = get_listable(configuration, "include", DEFAULT_INCLUDE)
+        self.exclude = get_listable(configuration, "exclude", DEFAULT_EXCLUDE)
+
+    def relative(self, path: StrPath) -> Path:
+        return relative(path, self.root)
+
+    def set_processed(self, path: StrPath) -> None:
+        rel = self.relative(path)
+        self.processed.append(rel.as_posix())
+
+    def should_process(self, path: StrPath) -> bool:
+        rel = self.relative(path)
+        return (
+            rel.as_posix() not in self.processed
+            and matches_any(rel, self.include)
+            and not matches_any(rel, self.exclude)
+        )
+
+    def evaluate_and_replace(self) -> int:
+        count = 0
+        for path in (os.path.join(p, f) for p, _, fs in os.walk(self.root) for f in fs):
+            if self.should_process(path):
+                count += 1
+                result = ""
+                ctx = EvaluationContext(path, self)
+                with open(path, "r+") as file:
+                    for line in file:
+                        evaluated = ctx.evaluate_line(line)
+                        if evaluated is not None:
+                            result += evaluated
+                    file.seek(0)
+                    file.write(result)
+                    file.truncate()
+                self.set_processed(path)
+
+        return count
+
+    def evaluate_string(
+        self,
+        data: str,
+        location: Optional[StrPath] = None,
+    ) -> str:
+        result: List[str] = []
+        ctx = EvaluationContext(location, self)
+        for line in data.split("\n"):
+            evaluated = ctx.evaluate_line(line)
+            if evaluated is not None:
+                result.append(evaluated)
+
+        if location is not None:
+            self.set_processed(location)
+
+        return "\n".join(result)
+
+
+class EvaluationContext:
+    def __init__(
+        self,
+        location: Optional[StrPath],
+        engine: TemplatingEngine,
+    ) -> None:
+        self.location = location and engine.relative(location)
+        self.engine = engine
+        self.enabled = True
+        self.line = -1
+
+    def evaluate_line(self, data: str) -> Union[str, None]:
+        self.line += 1
+
+        # Check for on/off comment
+        if RE_DISABLE.match(data):
+            self.enabled = False
+            return None
+        if RE_ENABLE.match(data):
+            self.enabled = True
+            return None
+
+        # Process line
+        if self.enabled:
+            # Skip if ends with delete comment
+            if RE_DELETE.search(data):
+                return None
+
+            return self.evaluate_string(data)
+        else:
+            return data
+
+    def evaluate_string(self, data: str) -> str:
+        return RE_TEMPLATE_SLOT.sub(self._evaluate_slot, data)
+
+    def _evaluate_slot(self, match: re.Match) -> str:
+        content = match.group(1)
+        for construct in Construct.constructs:
+            check = construct.pattern.match(content)
+            if check is not None:
+                try:
+                    return construct.handler(check, self)
+                except Exception as e:
+                    if isinstance(e, EvaluationError):
+                        raise
+                    raise EvaluationError(self, e) from e  # pragma: no cover
+        raise EvaluationError(self, "Unknown Construct")
+
+
+class Construct:
+    constructs: List["Construct"] = []
+
+    def __init__(
+        self,
+        pattern: Pattern,
+        handler: Callable[[Match, EvaluationContext], str],
+    ) -> None:
+        Construct.constructs.append(self)
+        self.handler = handler
+        self.pattern = pattern
+
+    @staticmethod
+    def construct(
+        pattern: Union[Pattern, str],
+    ) -> Callable[[Callable[[Match, EvaluationContext], str]], Construct]:
+        if isinstance(pattern, str):
+            pattern = re.compile(pattern)
+
+        def wrapper(func: Callable[[Match, EvaluationContext], str]) -> Construct:
+            return Construct(pattern, func)
+
+        return wrapper
+
+
+# Define Constructs
+
+
+@Construct.construct("^[\"'](.+)[\"']$")
+def literal_construct(match: Match, ctx: EvaluationContext) -> str:
+    return ctx.evaluate_string(match.group(1))
+
+
+@Construct.construct(r"^pyproject((?:\.[^.]+)+)?$")
+def pyproject_construct(match: Match, ctx: EvaluationContext) -> str:
+    path = match.group(1)
+
+    if path is None:
+        return str(ctx.engine.pyproject.data)
+
+    result = traverse(ctx.engine.pyproject.data, path[1:])
+    return str(result)
+
+
+@Construct.construct(r"^(\.?(?:\/.+)+)$")
+def file_construct(match: Match, ctx: EvaluationContext) -> str:
+    path: str = match.group(1)
+
+    if path.startswith("/"):
+        path = os.path.join(ctx.engine.root, path[1:])
+    else:
+        if ctx.location is None:
+            raise EvaluationError(ctx, "Relative paths are not permitted in this context")
+        path = os.path.join(ctx.engine.root, os.path.dirname(ctx.location), path)
+
+    if not os.path.isfile(path):
+        raise EvaluationError(ctx, f'No such file "{os.path.abspath(path)}"')
+
+    with open(path, "r", encoding=ctx.engine.encoding) as f:
+        content = f.read()
+        if ctx.engine.should_process(path):
+            content = ctx.engine.evaluate_string(content, path)
+        return content
+
+
+@Construct.construct(r"^env(?:\.([^\.\s]+))?$")
+def environ_construct(match: Match, ctx: EvaluationContext) -> str:
+    key = match.group(1)
+
+    if key is None:
+        return str(dict(os.environ))
+
+    if key not in os.environ:
+        raise EvaluationError(ctx, f"No environment variable '{key}'")
+
+    return os.environ[key]
```

### Comparing `poetry_templating-1.1.1/src/poetry_templating/error.py` & `poetry_templating-1.1.2/src/poetry_templating/error.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:  # pragma: no cover
-    from poetry_templating.engine import EvaluationContext
-
-
-class TemplatingError(Exception):
-    ...
-
-
-class EvaluationError(TemplatingError):
-    def __init__(self, ctx: "EvaluationContext", message) -> None:
-        super().__init__(
-            f"Error evaluating template: {message}\n  "
-            + (
-                f"Line {ctx.line}"
-                if ctx.location is None
-                else f'File "{ctx.location}", line {ctx.line}'
-            )
-        )
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:  # pragma: no cover
+    from poetry_templating.engine import EvaluationContext
+
+
+class TemplatingError(Exception):
+    ...
+
+
+class EvaluationError(TemplatingError):
+    def __init__(self, ctx: "EvaluationContext", message) -> None:
+        super().__init__(
+            f"Error evaluating template: {message}\n  "
+            + (
+                f"Line {ctx.line}"
+                if ctx.location is None
+                else f'File "{ctx.location}", line {ctx.line}'
+            )
+        )
```

### Comparing `poetry_templating-1.1.1/src/poetry_templating/plugin.py` & `poetry_templating-1.1.2/src/poetry_templating/plugin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,103 +1,110 @@
-import os
-import shutil
-import tempfile
-from contextlib import contextmanager
-from pathlib import Path
-from typing import Iterator, List, Type
-
-from cleo.events.console_command_event import ConsoleCommandEvent
-from cleo.events.console_events import COMMAND
-from cleo.io.io import IO
-from poetry.console.application import Application
-from poetry.console.commands.build import BuildCommand
-from poetry.console.commands.command import Command
-from poetry.factory import Factory
-from poetry.plugins.application_plugin import ApplicationPlugin
-from poetry.poetry import Poetry
-from poetry.puzzle.provider import Indicator
-
-from poetry_templating import DEFAULT_BUILD_DIR
-from poetry_templating.util import Mixin
-
-
-@contextmanager
-def progress(io: IO, message: str) -> Iterator[None]:
-    if not io.output.is_decorated():
-        io.write_line(message)
-        yield
-    else:
-        indicator = Indicator(io, "{message}{context}<debug>({elapsed:2s})</debug>")
-
-        with indicator.auto(message, message):
-            yield
-
-
-class EvaluateCommand(Command):
-    name: str = "templating evaluate"
-    description = "Evaluate templates in the current directory."
-
-    def handle(self) -> int:
-        from poetry_templating.engine import TemplatingEngine
-
-        engine = TemplatingEngine(self.poetry.pyproject)
-        with progress(self.io, "<info>Evaluating templates...</info>"):
-            count = engine.evaluate_and_replace()
-        self.line(f"<info>Evaluated templates in {count} files!</info>")
-        return 0
-
-
-class TemplatingPlugin(ApplicationPlugin):
-    @property
-    def commands(self) -> List[Type[Command]]:
-        return [EvaluateCommand]
-
-    def activate(self, application: Application):
-        super().activate(application)
-
-        try:
-            self.poetry = application.poetry
-        except RuntimeError:
-            pass  # Disable build hook if pyproject could not be found
-        else:
-            self.root = Path(os.path.dirname(application.poetry.pyproject.path))
-            application.event_dispatcher.add_listener(COMMAND, self.on_command)  # type: ignore
-
-    def on_command(self, event: ConsoleCommandEvent, *_) -> None:
-        # If command is build command, set up build templating
-        command = event.command
-        if isinstance(command, BuildCommand):
-            self.setup_build(command)
-
-    def setup_build(self, command: BuildCommand):
-        from poetry.core.masonry.builder import Builder
-
-        # Mixin to point builders to evaluated clone project
-        @Mixin.mixin(command, "handle")
-        def handler_mixin() -> int:
-            with builder_mixin, self.evaluated_clone(command.io) as poetry:
-                command._poetry = poetry
-                return handler_mixin.original()
-
-        # Mixin to set the "target_dir" parameter back to the original project
-        @Mixin.mixin(Builder, "build")
-        def builder_mixin(*args, target_dir=None, **kwargs) -> None:
-            target_dir = self.root / DEFAULT_BUILD_DIR
-            builder_mixin.original(*args, **kwargs, target_dir=target_dir)
-
-        handler_mixin.inject()  # Inject handler mixin to this instance of BuildCommand
-
-    @contextmanager
-    def evaluated_clone(self, io: IO) -> Iterator[Poetry]:
-        from poetry_templating.engine import TemplatingEngine
-
-        with tempfile.TemporaryDirectory() as tmpdir:
-            with progress(io, "Evaluating templates..."):
-                shutil.copytree(self.root, tmpdir, symlinks=False, dirs_exist_ok=True)
-
-                # Create clone poetry instance
-                poetry = Factory().create_poetry(Path(tmpdir), io=io)
-
-                # Evaluate clone
-                engine = TemplatingEngine(poetry.pyproject)
-                engine.evaluate_and_replace()
-            yield poetry
+import contextlib
+import os
+import shutil
+import tempfile
+from contextlib import contextmanager
+from pathlib import Path
+from typing import Iterator, List, Optional, Type
+
+from cleo.events.console_command_event import ConsoleCommandEvent
+from cleo.events.console_events import COMMAND
+from cleo.io.io import IO
+from poetry.console.application import Application
+from poetry.console.commands.build import BuildCommand
+from poetry.console.commands.command import Command
+from poetry.factory import Factory
+from poetry.plugins.application_plugin import ApplicationPlugin
+from poetry.poetry import Poetry
+from poetry.puzzle.provider import Indicator
+
+from poetry_templating import DEFAULT_BUILD_DIR
+from poetry_templating.util import Mixin
+
+
+@contextmanager
+def progress(io: IO, message: str) -> Iterator[None]:
+    if not io.output.is_decorated():
+        io.write_line(message)
+        yield
+    else:
+        indicator = Indicator(io, "{message}{context}<debug>({elapsed:2s})</debug>")
+
+        with indicator.auto(message, message):
+            yield
+
+
+class EvaluateCommand(Command):
+    name: str = "templating evaluate"
+    description = "Evaluate templates in the current directory."
+
+    def handle(self) -> int:
+        from poetry_templating.engine import TemplatingEngine
+
+        engine = TemplatingEngine(self.poetry.pyproject)
+        with progress(self.io, "<info>Evaluating templates...</info>"):
+            count = engine.evaluate_and_replace()
+        self.line(f"<info>Evaluated templates in {count} files!</info>")
+        return 0
+
+
+class TemplatingPlugin(ApplicationPlugin):
+    @property
+    def commands(self) -> List[Type[Command]]:
+        return [EvaluateCommand]
+
+    def activate(self, application: Application):
+        super().activate(application)
+
+        try:
+            self.poetry = application.poetry
+        except RuntimeError:
+            pass  # Disable build hook if pyproject could not be found
+        else:
+            self.root = Path(os.path.dirname(application.poetry.pyproject.path))
+            application.event_dispatcher.add_listener(COMMAND, self.on_command)  # type: ignore
+
+    def on_command(self, event: ConsoleCommandEvent, *_) -> None:
+        # If command is build command, set up build templating
+        command = event.command
+        if isinstance(command, BuildCommand):
+            self.setup_build(command)
+
+    def setup_build(self, command: BuildCommand):
+        # Mixin to point builders to evaluated clone project
+        @Mixin.mixin(command, "handle")
+        def handler_mixin() -> int:
+            with build_mixin, self.evaluated_clone(command.io) as poetry:
+                command._poetry = poetry
+                return handler_mixin.original()
+
+        # Mixin to set the "target_dir" parameter back to the original project
+        @Mixin.mixin(command, "_build")
+        def build_mixin(*args, target_dir: Optional[Path] = None, **kwargs) -> None:
+            if target_dir is None:  # pragma: no cover
+                # Function is always called with a value
+                target_dir = self.root / DEFAULT_BUILD_DIR
+            else:
+                with contextlib.suppress(ValueError):
+                    target_dir = self.root / target_dir.relative_to(
+                        command.poetry.pyproject_path.parent
+                    )
+
+            build_mixin.original(*args, **kwargs, target_dir=target_dir)
+
+        handler_mixin.inject()  # Inject handler mixin to this instance of BuildCommand
+
+    @contextmanager
+    def evaluated_clone(self, io: IO) -> Iterator[Poetry]:
+        from poetry_templating.engine import TemplatingEngine
+
+        with tempfile.TemporaryDirectory() as tmpdir:
+            with progress(io, "Evaluating templates..."):
+                shutil.copytree(self.root, tmpdir, symlinks=False, dirs_exist_ok=True)
+
+                # Create clone poetry instance
+                poetry = Factory().create_poetry(Path(tmpdir), io=io)
+
+                # Evaluate clone
+                engine = TemplatingEngine(poetry.pyproject)
+                engine.evaluate_and_replace()
+            yield poetry
```

### Comparing `poetry_templating-1.1.1/src/poetry_templating/util.py` & `poetry_templating-1.1.2/src/poetry_templating/util.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,210 +1,210 @@
-from __future__ import annotations
-
-import os
-from pathlib import Path
-from typing import Any, Callable, Dict, List, Optional, Union
-
-from poetry.core.pyproject.toml import PyProjectTOML
-
-from poetry_templating import CONFIG_TABLE
-
-StrPath = Union[Path, str]
-
-
-class Mixin:
-    """Represents a replacement action for an attribute of an object."""
-
-    def __init__(self, obj: object, name: str, repl: Any) -> None:
-        """Represents a replacement action for an attribute of an object.
-
-        Parameters
-        ----------
-        obj : object
-            The object the attribute belongs to.
-        name : str
-            The name of the attribute to replace.
-        repl : Any
-            The replacement.
-        """
-        self.replacement: Any = repl
-        self.original: Any = None
-        self.obj: object = obj
-        self.name: str = name
-
-    def __enter__(self) -> None:
-        self.inject()
-
-    def __exit__(self, *_) -> None:
-        self.restore()
-
-    def inject(self) -> None:
-        """Inject the replacement into the object's attribute."""
-        self.original = getattr(self.obj, self.name)
-        setattr(self.obj, self.name, self.replacement)
-
-    def restore(self) -> None:
-        """Restore the attribute back to its original value"""
-        setattr(self.obj, self.name, self.original)
-
-    @staticmethod
-    def mixin(
-        obj: object, name: Optional[str] = None
-    ) -> Callable[[Callable[..., Any]], Mixin]:
-        """Decorator to generate a mixin from a function.
-
-        Parameters
-        ----------
-        obj : object
-            The object the attribute belongs to.
-        name : str, optional
-            The name of the attribute to replace, the name of the fucntion by default.
-        """
-
-        def wrapper(func: Callable[..., Any]) -> Mixin:
-            return Mixin(obj, name or func.__name__, func)
-
-        return wrapper
-
-
-def matches_any(path: StrPath, patterns: list[str]) -> bool:
-    """Checks if the specified path matches any of the provided patterns.
-
-    Parameters
-    ----------
-    path : Path
-        The path to check against.
-    patterns : list[str]
-        A list of glob patterns to check against the path.
-
-    Returns
-    -------
-    bool
-        True if any of the patterns matched against the path.
-    """
-    normalized = Path(Path(path).as_posix().lower())
-    return any(normalized.match(p.lower().strip("/")) for p in patterns)
-
-
-def get_configuration(pyproject: PyProjectTOML) -> dict:
-    """Get the poetry templating configuration dictionary.
-
-    Parameters
-    ----------
-    pyproject : PyProjectTOML
-        The pyproject.toml file which contains the configuration.
-
-    Returns
-    -------
-    dict
-        The dictionary containing the poetry templating configuration.
-    """
-    tool_table = pyproject.data.get("tool")
-    if not isinstance(tool_table, dict):
-        raise TypeError("Could not find table 'tool'")
-
-    config_table = tool_table.get(CONFIG_TABLE, {})
-    if not isinstance(config_table, dict):
-        raise TypeError(f"Could not find table 'tool.{CONFIG_TABLE}'")
-
-    return config_table
-
-
-def get_listable(dict: dict, key: str, default: list = []) -> list:
-    """Gets a list from the specified dictionary and key. If the value is not a list, it will be wrapped in one.
-
-    Parameters
-    ----------
-    dict : dict
-        The dictionary in which the desired key resides.
-    key : str
-        The key of the value to get.
-    default : list, optional
-        The default value to return if the key is not found. Empty list by default.
-
-    Returns
-    -------
-    list
-        The value in list form.
-    """
-    value = dict.get(key, default)
-    if not isinstance(value, list):
-        value = [value]
-    return value
-
-
-def relative(path: StrPath, root: StrPath) -> Path:
-    """Attempts to generate a relative path from the provided root. An absolute path will be returned if `path` is not a subpath of `root`.
-
-    Parameters
-    ----------
-    path : Path
-        The path to attempt to make relative.
-    root : str
-        The root directory to make the path relative to.
-
-    Returns
-    -------
-    Path
-        The resolved, relative path.
-    """
-    resolved = Path(os.path.realpath(path))
-    try:
-        return resolved.relative_to(root)
-    except ValueError:
-        return resolved
-
-
-def traverse(
-    structure: Union[Dict[str, Any], List[Any]],
-    path: Union[str, List[str]],
-) -> Any:
-    """Gets value at the provided path from the given dictionary or list.
-
-    Paths should be a list of keys/indexes as either a list or string, separated by dots.
-
-    Parameters
-    ----------
-    structure : dict | list
-        The structure to traverse through.
-    path : str | list[str]
-        The path to the value to return.
-
-    Returns
-    -------
-    Any
-        The value at the provided path
-
-    Raises
-    ------
-    KeyError
-        Raised when attempting to access a dictionary key that does not exist.
-    ValueError
-        Raised when an unexpected value is found while traversing.
-    IndexError
-        Raised when attempting to access a list item that does not exist.
-    """
-    if isinstance(path, str):
-        path = path.split(".")
-
-    current = structure
-    for i, step in enumerate(path):
-        if isinstance(current, dict):  # Handle dictionaries
-            if step not in current:
-                raise KeyError(f"{'.'.join(path[:i + 1])} does not exist")
-            current = current[step]
-        elif isinstance(current, list):  # Handle lists
-            try:
-                index = int(step)
-            except ValueError:
-                raise ValueError(f"'{step}' is not a valid list index")
-
-            if index >= len(current):
-                raise IndexError(
-                    f"{index} is out of range for list at {'.'.join(path[:i])}"
-                )
-
-            current = current[index]
-        else:
-            raise ValueError(f"Expected list or dictionary at {'.'.join(path[:i])}")
-
-    return current
+from __future__ import annotations
+
+import os
+from pathlib import Path
+from typing import Any, Callable, Dict, List, Optional, Union
+
+from poetry.core.pyproject.toml import PyProjectTOML
+
+from poetry_templating import CONFIG_TABLE
+
+StrPath = Union[Path, str]
+
+
+class Mixin:
+    """Represents a replacement action for an attribute of an object."""
+
+    def __init__(self, obj: object, name: str, repl: Any) -> None:
+        """Represents a replacement action for an attribute of an object.
+
+        Parameters
+        ----------
+        obj : object
+            The object the attribute belongs to.
+        name : str
+            The name of the attribute to replace.
+        repl : Any
+            The replacement.
+        """
+        self.replacement: Any = repl
+        self.original: Any = None
+        self.obj: object = obj
+        self.name: str = name
+
+    def __enter__(self) -> None:
+        self.inject()
+
+    def __exit__(self, *_) -> None:
+        self.restore()
+
+    def inject(self) -> None:
+        """Inject the replacement into the object's attribute."""
+        self.original = getattr(self.obj, self.name)
+        setattr(self.obj, self.name, self.replacement)
+
+    def restore(self) -> None:
+        """Restore the attribute back to its original value"""
+        setattr(self.obj, self.name, self.original)
+
+    @staticmethod
+    def mixin(
+        obj: object, name: Optional[str] = None
+    ) -> Callable[[Callable[..., Any]], Mixin]:
+        """Decorator to generate a mixin from a function.
+
+        Parameters
+        ----------
+        obj : object
+            The object the attribute belongs to.
+        name : str, optional
+            The name of the attribute to replace, the name of the fucntion by default.
+        """
+
+        def wrapper(func: Callable[..., Any]) -> Mixin:
+            return Mixin(obj, name or func.__name__, func)
+
+        return wrapper
+
+
+def matches_any(path: StrPath, patterns: list[str]) -> bool:
+    """Checks if the specified path matches any of the provided patterns.
+
+    Parameters
+    ----------
+    path : Path
+        The path to check against.
+    patterns : list[str]
+        A list of glob patterns to check against the path.
+
+    Returns
+    -------
+    bool
+        True if any of the patterns matched against the path.
+    """
+    normalized = Path(Path(path).as_posix().lower())
+    return any(normalized.match(p.lower().strip("/")) for p in patterns)
+
+
+def get_configuration(pyproject: PyProjectTOML) -> dict:
+    """Get the poetry templating configuration dictionary.
+
+    Parameters
+    ----------
+    pyproject : PyProjectTOML
+        The pyproject.toml file which contains the configuration.
+
+    Returns
+    -------
+    dict
+        The dictionary containing the poetry templating configuration.
+    """
+    tool_table = pyproject.data.get("tool")
+    if not isinstance(tool_table, dict):
+        raise TypeError("Could not find table 'tool'")
+
+    config_table = tool_table.get(CONFIG_TABLE, {})
+    if not isinstance(config_table, dict):
+        raise TypeError(f"Could not find table 'tool.{CONFIG_TABLE}'")
+
+    return config_table
+
+
+def get_listable(dict: dict, key: str, default: list = []) -> list:
+    """Gets a list from the specified dictionary and key. If the value is not a list, it will be wrapped in one.
+
+    Parameters
+    ----------
+    dict : dict
+        The dictionary in which the desired key resides.
+    key : str
+        The key of the value to get.
+    default : list, optional
+        The default value to return if the key is not found. Empty list by default.
+
+    Returns
+    -------
+    list
+        The value in list form.
+    """
+    value = dict.get(key, default)
+    if not isinstance(value, list):
+        value = [value]
+    return value
+
+
+def relative(path: StrPath, root: StrPath) -> Path:
+    """Attempts to generate a relative path from the provided root. An absolute path will be returned if `path` is not a subpath of `root`.
+
+    Parameters
+    ----------
+    path : Path
+        The path to attempt to make relative.
+    root : str
+        The root directory to make the path relative to.
+
+    Returns
+    -------
+    Path
+        The resolved, relative path.
+    """
+    resolved = Path(os.path.realpath(path))
+    try:
+        return resolved.relative_to(root)
+    except ValueError:
+        return resolved
+
+
+def traverse(
+    structure: Union[Dict[str, Any], List[Any]],
+    path: Union[str, List[str]],
+) -> Any:
+    """Gets value at the provided path from the given dictionary or list.
+
+    Paths should be a list of keys/indexes as either a list or string, separated by dots.
+
+    Parameters
+    ----------
+    structure : dict | list
+        The structure to traverse through.
+    path : str | list[str]
+        The path to the value to return.
+
+    Returns
+    -------
+    Any
+        The value at the provided path
+
+    Raises
+    ------
+    KeyError
+        Raised when attempting to access a dictionary key that does not exist.
+    ValueError
+        Raised when an unexpected value is found while traversing.
+    IndexError
+        Raised when attempting to access a list item that does not exist.
+    """
+    if isinstance(path, str):
+        path = path.split(".")
+
+    current = structure
+    for i, step in enumerate(path):
+        if isinstance(current, dict):  # Handle dictionaries
+            if step not in current:
+                raise KeyError(f"{'.'.join(path[:i + 1])} does not exist")
+            current = current[step]
+        elif isinstance(current, list):  # Handle lists
+            try:
+                index = int(step)
+            except ValueError:
+                raise ValueError(f"'{step}' is not a valid list index")
+
+            if index >= len(current):
+                raise IndexError(
+                    f"{index} is out of range for list at {'.'.join(path[:i])}"
+                )
+
+            current = current[index]
+        else:
+            raise ValueError(f"Expected list or dictionary at {'.'.join(path[:i])}")
+
+    return current
```

