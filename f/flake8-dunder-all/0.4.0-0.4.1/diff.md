# Comparing `tmp/flake8_dunder_all-0.4.0.tar.gz` & `tmp/flake8_dunder_all-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_dunder_all-0.4.0.tar", last modified: Thu Mar 28 18:50:01 2024, max compression
+gzip compressed data, was "flake8_dunder_all-0.4.1.tar", last modified: Tue Apr  2 15:58:21 2024, max compression
```

## Comparing `flake8_dunder_all-0.4.0.tar` & `flake8_dunder_all-0.4.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-03-28 18:50:01.530026 flake8_dunder_all-0.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-03-28 18:50:01.522026 flake8_dunder_all-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-28 18:50:01.530026 flake8_dunder_all-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-03-28 18:50:01.530026 flake8_dunder_all-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-03-28 18:50:01.530026 flake8_dunder_all-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-03-28 18:49:33.605756 flake8_dunder_all-0.4.0/flake8_dunder_all/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-03-28 18:49:33.605756 flake8_dunder_all-0.4.0/flake8_dunder_all/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 18:49:33.605756 flake8_dunder_all-0.4.0/flake8_dunder_all/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9140 2024-03-28 18:49:33.605756 flake8_dunder_all-0.4.0/flake8_dunder_all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-04-02 15:58:21.355108 flake8_dunder_all-0.4.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-02 15:58:21.351108 flake8_dunder_all-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-02 15:58:21.355108 flake8_dunder_all-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-04-02 15:58:21.355108 flake8_dunder_all-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-04-02 15:58:21.359108 flake8_dunder_all-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-02 15:57:49.231186 flake8_dunder_all-0.4.1/flake8_dunder_all/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-02 15:57:49.231186 flake8_dunder_all-0.4.1/flake8_dunder_all/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 15:57:49.231186 flake8_dunder_all-0.4.1/flake8_dunder_all/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10303 2024-04-02 15:57:49.231186 flake8_dunder_all-0.4.1/flake8_dunder_all/__init__.py
```

### Comparing `flake8_dunder_all-0.4.0/README.rst` & `flake8_dunder_all-0.4.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 .. |license| image:: https://img.shields.io/github/license/python-formate/flake8-dunder-all
 	:target: https://github.com/python-formate/flake8-dunder-all/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/python-formate/flake8-dunder-all
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/python-formate/flake8-dunder-all/v0.4.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/python-formate/flake8-dunder-all/v0.4.1
 	:target: https://github.com/python-formate/flake8-dunder-all/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/python-formate/flake8-dunder-all
 	:target: https://github.com/python-formate/flake8-dunder-all/commit/master
 	:alt: GitHub last commit
 
@@ -169,15 +169,15 @@
 
 .. code-block:: yaml
 
 	 - repo: https://gitlab.com/pycqa/flake8
 	   rev: 3.8.1
 	   hooks:
 	    - id: flake8
-	      additional_dependencies: [flake8-dunder-all==0.4.0]
+	      additional_dependencies: [flake8-dunder-all==0.4.1]
 
 ``ensure-dunder-all`` script
 
 There is also a script which will automatically add __all__ for files which don't have it.
 
 See `the documentation <https://flake8-dunder-all.readthedocs.io/en/latest/usage.html#ensure-dunder-all-script>`_
 for details.
```

### Comparing `flake8_dunder_all-0.4.0/LICENSE` & `flake8_dunder_all-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_dunder_all-0.4.0/pyproject.toml` & `flake8_dunder_all-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "flake8-dunder-all"
-version = "0.4.0"
+version = "0.4.1"
 description = "A Flake8 plugin and pre-commit hook which checks to ensure modules have defined '__all__'."
 readme = "README.rst"
 keywords = [ "flake8",]
 dynamic = []
 dependencies = [
     "astatine>=0.3.1",
     "click>=7.1.2",
@@ -151,15 +151,15 @@
     "__new__",
     "__getnewargs__",
     "__abstractmethods__",
     "__hash__",
 ]
 
 [tool.mypy]
-python_version = "3.6"
+python_version = "3.8"
 namespace_packages = true
 check_untyped_defs = true
 warn_unused_ignores = true
 no_implicit_optional = true
 show_error_codes = true
 
 [tool.snippet-fmt]
```

### Comparing `flake8_dunder_all-0.4.0/PKG-INFO` & `flake8_dunder_all-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.2
 Name: flake8-dunder-all
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Flake8 plugin and pre-commit hook which checks to ensure modules have defined '__all__'.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Keywords: flake8
 Home-page: https://github.com/python-formate/flake8-dunder-all
 Project-URL: Issue Tracker, https://github.com/python-formate/flake8-dunder-all/issues
 Project-URL: Source Code, https://github.com/python-formate/flake8-dunder-all
@@ -138,15 +138,15 @@
 .. |license| image:: https://img.shields.io/github/license/python-formate/flake8-dunder-all
 	:target: https://github.com/python-formate/flake8-dunder-all/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/python-formate/flake8-dunder-all
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/python-formate/flake8-dunder-all/v0.4.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/python-formate/flake8-dunder-all/v0.4.1
 	:target: https://github.com/python-formate/flake8-dunder-all/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/python-formate/flake8-dunder-all
 	:target: https://github.com/python-formate/flake8-dunder-all/commit/master
 	:alt: GitHub last commit
 
@@ -210,15 +210,15 @@
 
 .. code-block:: yaml
 
 	 - repo: https://gitlab.com/pycqa/flake8
 	   rev: 3.8.1
 	   hooks:
 	    - id: flake8
-	      additional_dependencies: [flake8-dunder-all==0.4.0]
+	      additional_dependencies: [flake8-dunder-all==0.4.1]
 
 ``ensure-dunder-all`` script
 
 There is also a script which will automatically add __all__ for files which don't have it.
 
 See `the documentation <https://flake8-dunder-all.readthedocs.io/en/latest/usage.html#ensure-dunder-all-script>`_
 for details.
```

### Comparing `flake8_dunder_all-0.4.0/flake8_dunder_all/utils.py` & `flake8_dunder_all-0.4.1/flake8_dunder_all/utils.py`

 * *Files identical despite different names*

### Comparing `flake8_dunder_all-0.4.0/flake8_dunder_all/__main__.py` & `flake8_dunder_all-0.4.1/flake8_dunder_all/__main__.py`

 * *Files identical despite different names*

### Comparing `flake8_dunder_all-0.4.0/flake8_dunder_all/__init__.py` & `flake8_dunder_all-0.4.1/flake8_dunder_all/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,29 +28,29 @@
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 #  THE SOFTWARE.
 #
 
 # stdlib
 import ast
 import sys
-from typing import Any, Generator, List, Set, Tuple, Type, Union
+from typing import Any, Generator, Iterator, List, Set, Tuple, Type, Union
 
 # 3rd party
 from consolekit.terminal_colours import Fore
 from domdf_python_tools.paths import PathPlus
 from domdf_python_tools.typing import PathLike
 from domdf_python_tools.utils import stderr_writer
 
 # this package
 from flake8_dunder_all.utils import find_noqa, get_docstring_lineno, mark_text_ranges
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020 Dominic Davis-Foster"
 __license__: str = "MIT"
-__version__: str = "0.4.0"
+__version__: str = "0.4.1"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = ("Visitor", "Plugin", "check_and_add_all", "DALL000")
 
 DALL000 = "DALL000 Module lacks __all__."
 
 
@@ -154,20 +154,18 @@
 	def handle_import(self, node: Union[ast.Import, ast.ImportFrom]) -> None:
 		"""
 		Handles ``import foo`` and ``from foo import bar``.
 
 		:param node: The node being visited
 		"""
 
-		if self.use_endlineno:
-			if node.end_lineno > self.last_import:  # type: ignore[union-attr]
-				self.last_import = node.end_lineno  # type: ignore[union-attr]
+		if self.use_endlineno and node.end_lineno is not None:
+			self.last_import = max(self.last_import, node.end_lineno)
 		else:
-			if node.lineno > self.last_import:
-				self.last_import = node.lineno
+			self.last_import = max(self.last_import, node.lineno)
 
 	def visit_Import(self, node: ast.Import) -> None:
 		"""
 		Visit ``import foo``.
 
 		:param node: The node being visited
 		"""
@@ -187,24 +185,68 @@
 
 	def visit_If(self, node: ast.If) -> None:
 		"""
 		Visit an if statement and check if it's for `TYPE_CHECKING`.
 
 		:param node: The node being visited.
 		"""
-		# Check if the condition is checking for TYPE_CHECKING
-		if isinstance(node.test, ast.Name) and node.test.id == "TYPE_CHECKING":
-			# Process the body of the if statement for any import statements
-			for body_node in node.body:
-				if isinstance(body_node, (ast.Import, ast.ImportFrom)):
-					self.handle_import(body_node)
-		# Continue visiting other nodes
+
+		if _is_type_checking(node.test):
+			if self.use_endlineno and node.end_lineno is not None:
+				self.last_import = max(self.last_import, node.end_lineno)
+			else:
+				self.last_import = max(self.last_import, max(_descend_node(node)))
+
+		self.generic_visit(node)
+
+	def visit_Try(self, node: ast.Try) -> None:
+		"""
+		Visit a Try statement.
+
+		:param node: The node being visited.
+		"""
+
+		if any(isinstance(n, (ast.Import, ast.ImportFrom)) for n in node.body):
+			if self.use_endlineno and node.end_lineno is not None and sys.implementation.name != "pypy":  # pragma: no cover (pypy)
+				self.last_import = max(self.last_import, node.end_lineno)
+			else:  # pragma: no cover (!pypy)
+				end_lineno = max(
+						*_descend_node(node),
+						*_descend_node(node, "handlers"),
+						*_descend_node(node, "orelse"),
+						*_descend_node(node, "finalbody"),
+						)
+				self.last_import = max(self.last_import, end_lineno)
+
 		self.generic_visit(node)
 
 
+def _descend_node(node: ast.AST, attr: str = "body") -> Iterator[int]:
+	for child in getattr(node, attr, []):
+		yield child.lineno
+		yield from _descend_node(child)
+
+
+_nameconstant = ast.Constant if sys.version_info >= (3, 8) else ast.NameConstant
+
+
+def _is_type_checking(node: ast.AST) -> bool:
+	"""
+	Does the given ``if`` node indicate a `TYPE_CHECKING` block?
+	"""  # noqa: D400
+
+	if isinstance(node, ast.Name) and node.id == "TYPE_CHECKING":
+		return True
+	elif isinstance(node, _nameconstant) and node.value is False:
+		return True
+	elif isinstance(node, ast.BoolOp):
+		return any(_is_type_checking(value) for value in node.values)
+	return False
+
+
 class Plugin:
 	"""
 	A Flake8 plugin which checks to ensure modules have defined ``__all__``.
 
 	:param tree: The abstract syntax tree (AST) to check.
 	"""
```

