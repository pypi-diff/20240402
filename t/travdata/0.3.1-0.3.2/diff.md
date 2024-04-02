# Comparing `tmp/travdata-0.3.1.tar.gz` & `tmp/travdata-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "travdata-0.3.1.tar", max compression
+gzip compressed data, was "travdata-0.3.2.tar", max compression
```

## Comparing `travdata-0.3.1.tar` & `travdata-0.3.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1095 2024-04-01 19:18:47.673696 travdata-0.3.1/LICENSE
--rw-r--r--   0        0        0     6682 2024-04-01 19:18:47.673696 travdata-0.3.1/README.rst
--rw-r--r--   0        0        0     1296 2024-04-01 19:18:47.677696 travdata-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      129 2024-04-01 19:18:47.677696 travdata-0.3.1/src/travdata/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 19:18:47.677696 travdata-0.3.1/src/travdata/cli/__init__.py
--rwxr-xr-x   0        0        0     1277 2024-04-01 19:18:47.677696 travdata-0.3.1/src/travdata/cli/cli.py
--rw-r--r--   0        0        0        0 2024-04-01 19:18:47.677696 travdata-0.3.1/src/travdata/cli/cmds/__init__.py
--rw-r--r--   0        0        0     1937 2024-04-01 19:18:47.677696 travdata-0.3.1/src/travdata/cli/cmds/csvtoyaml.py
--rw-r--r--   0        0        0     4207 2024-04-01 19:18:47.677696 travdata-0.3.1/src/travdata/cli/cmds/extractcsvtables.py
--rw-r--r--   0        0        0     2617 2024-04-01 19:18:47.677696 travdata-0.3.1/src/travdata/cli/cmds/licenses.py
--rw-r--r--   0        0        0      646 2024-04-01 19:18:47.677696 travdata-0.3.1/src/travdata/cli/cmds/listbooks.py
--rw-r--r--   0        0        0    22253 2024-04-01 19:18:47.677696 travdata-0.3.1/src/travdata/cli/cmds/tradetable.py
--rw-r--r--   0        0        0      521 2024-04-01 19:18:47.677696 travdata-0.3.1/src/travdata/commontext.py
--rw-r--r--   0        0        0    10245 2024-04-01 19:18:47.677696 travdata-0.3.1/src/travdata/config.py
--rw-r--r--   0        0        0      616 2024-04-01 19:18:47.677696 travdata-0.3.1/src/travdata/csvutil.py
--rw-r--r--   0        0        0      705 2024-04-01 19:18:47.677696 travdata-0.3.1/src/travdata/dataclassutil.py
--rw-r--r--   0        0        0        0 2024-04-01 19:18:47.677696 travdata-0.3.1/src/travdata/datatypes/__init__.py
--rw-r--r--   0        0        0     3914 2024-04-01 19:18:47.677696 travdata-0.3.1/src/travdata/datatypes/basic.py
--rw-r--r--   0        0        0        0 2024-04-01 19:18:47.677696 travdata-0.3.1/src/travdata/datatypes/core/__init__.py
--rw-r--r--   0        0        0      685 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/datatypes/core/trade.py
--rw-r--r--   0        0        0     3156 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/datatypes/core/worldcreation.py
--rw-r--r--   0        0        0      483 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/datatypes/yamlcodec.py
--rw-r--r--   0        0        0        0 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/extraction/__init__.py
--rw-r--r--   0        0        0     2357 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/extraction/parseutil.py
--rw-r--r--   0        0        0     8517 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/extraction/pdfextract.py
--rw-r--r--   0        0        0     4006 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/extraction/tabulautil.py
--rw-r--r--   0        0        0        0 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/gui/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/gui/extraction/__init__.py
--rw-r--r--   0        0        0    12253 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/gui/extraction/cfgwin.py
--rw-r--r--   0        0        0     4804 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/gui/extraction/runnerwin.py
--rw-r--r--   0        0        0      862 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/gui/gui.py
--rw-r--r--   0        0        0      766 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/gui/qtutil.py
--rw-r--r--   0        0        0        0 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/py.typed
--rw-r--r--   0        0        0        0 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/tableconverters/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/tableconverters/core/__init__.py
--rw-r--r--   0        0        0      550 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/tableconverters/core/registry.py
--rw-r--r--   0        0        0     2079 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/tableconverters/core/trade.py
--rw-r--r--   0        0        0     3802 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/tableconverters/core/worldcreation.py
--rw-r--r--   0        0        0     1093 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/tableconverters/registry.py
--rw-r--r--   0        0        0        0 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/travellermap/__init__.py
--rw-r--r--   0        0        0     3686 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/travellermap/apiurls.py
--rw-r--r--   0        0        0     2397 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/travellermap/sectorparse.py
--rw-r--r--   0        0        0     4879 2024-04-01 19:18:47.681696 travdata-0.3.1/src/travdata/travellermap/world.py
--rw-r--r--   0        0        0     7647 1970-01-01 00:00:00.000000 travdata-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-04-02 19:56:56.951187 travdata-0.3.2/LICENSE
+-rw-r--r--   0        0        0     6682 2024-04-02 19:56:56.951187 travdata-0.3.2/README.rst
+-rw-r--r--   0        0        0     1342 2024-04-02 19:56:56.959186 travdata-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      129 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/cli/__init__.py
+-rwxr-xr-x   0        0        0     1277 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/cli/cli.py
+-rw-r--r--   0        0        0        0 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/cli/cmds/__init__.py
+-rw-r--r--   0        0        0     1937 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/cli/cmds/csvtoyaml.py
+-rw-r--r--   0        0        0     4207 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/cli/cmds/extractcsvtables.py
+-rw-r--r--   0        0        0     2617 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/cli/cmds/licenses.py
+-rw-r--r--   0        0        0      646 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/cli/cmds/listbooks.py
+-rw-r--r--   0        0        0    22253 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/cli/cmds/tradetable.py
+-rw-r--r--   0        0        0      521 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/commontext.py
+-rw-r--r--   0        0        0    12409 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/config.py
+-rw-r--r--   0        0        0      616 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/csvutil.py
+-rw-r--r--   0        0        0     1046 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/dataclassutil.py
+-rw-r--r--   0        0        0        0 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/datatypes/__init__.py
+-rw-r--r--   0        0        0     3914 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/datatypes/basic.py
+-rw-r--r--   0        0        0        0 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/datatypes/core/__init__.py
+-rw-r--r--   0        0        0      685 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/datatypes/core/trade.py
+-rw-r--r--   0        0        0     3156 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/datatypes/core/worldcreation.py
+-rw-r--r--   0        0        0      483 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/datatypes/yamlcodec.py
+-rw-r--r--   0        0        0        0 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/extraction/__init__.py
+-rw-r--r--   0        0        0     2357 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/extraction/parseutil.py
+-rw-r--r--   0        0        0     8517 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/extraction/pdfextract.py
+-rw-r--r--   0        0        0     4006 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/extraction/tabulautil.py
+-rw-r--r--   0        0        0        0 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/gui/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/gui/extraction/__init__.py
+-rw-r--r--   0        0        0    12253 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/gui/extraction/cfgwin.py
+-rw-r--r--   0        0        0     4804 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/gui/extraction/runnerwin.py
+-rw-r--r--   0        0        0      862 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/gui/gui.py
+-rw-r--r--   0        0        0      766 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/gui/qtutil.py
+-rw-r--r--   0        0        0        0 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/py.typed
+-rw-r--r--   0        0        0        0 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/tableconverters/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/tableconverters/core/__init__.py
+-rw-r--r--   0        0        0      550 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/tableconverters/core/registry.py
+-rw-r--r--   0        0        0     2079 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/tableconverters/core/trade.py
+-rw-r--r--   0        0        0     3802 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/tableconverters/core/worldcreation.py
+-rw-r--r--   0        0        0     1093 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/tableconverters/registry.py
+-rw-r--r--   0        0        0        0 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/travellermap/__init__.py
+-rw-r--r--   0        0        0     3686 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/travellermap/apiurls.py
+-rw-r--r--   0        0        0     2397 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/travellermap/sectorparse.py
+-rw-r--r--   0        0        0     4879 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/travellermap/world.py
+-rw-r--r--   0        0        0     7647 1970-01-01 00:00:00.000000 travdata-0.3.2/PKG-INFO
```

### Comparing `travdata-0.3.1/LICENSE` & `travdata-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `travdata-0.3.1/README.rst` & `travdata-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `travdata-0.3.1/pyproject.toml` & `travdata-0.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "travdata"
-version = "0.3.1"
+version = "0.3.2"
 description = "Data utility code for Mongoose Traveller TTRPG."
 authors = ["John Beisley <johnbeisleyuk@gmail.com>"]
 keywords = ["traveller", "ttrpg"]
 license = "MIT"
 readme = "README.rst"  # rebuilt from README.adoc
 repository = "https://github.com/huin/travdata"
 packages = [
@@ -47,7 +47,10 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 exclude = '''(?x)(
     travdata/gui/.*  # QtCore.pyi syntax error.
 )'''
+
+[tool.pylint.main]
+ignore-paths = ["oneoff"]
```

### Comparing `travdata-0.3.1/src/travdata/cli/cli.py` & `travdata-0.3.2/src/travdata/cli/cli.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.1/src/travdata/cli/cmds/csvtoyaml.py` & `travdata-0.3.2/src/travdata/cli/cmds/csvtoyaml.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.1/src/travdata/cli/cmds/extractcsvtables.py` & `travdata-0.3.2/src/travdata/cli/cmds/extractcsvtables.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.1/src/travdata/cli/cmds/licenses.py` & `travdata-0.3.2/src/travdata/cli/cmds/licenses.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.1/src/travdata/cli/cmds/listbooks.py` & `travdata-0.3.2/src/travdata/cli/cmds/listbooks.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.1/src/travdata/cli/cmds/tradetable.py` & `travdata-0.3.2/src/travdata/cli/cmds/tradetable.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.1/src/travdata/commontext.py` & `travdata-0.3.2/src/travdata/commontext.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.1/src/travdata/config.py` & `travdata-0.3.2/src/travdata/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,30 +5,40 @@
 
 * ``config.yaml`` top-level configuration for multiple books.
 * ``book.yaml`` relating to a single input PDF.
 
 See development.adoc for more information in how this is used.
 """
 
+from __future__ import annotations
+
 import abc
 import argparse
 import dataclasses
 import pathlib
 import sys
 import textwrap
-from typing import Any, ClassVar, Iterator, Optional
+from typing import Any, ClassVar, Iterator, Optional, cast, TYPE_CHECKING
 
 from ruamel import yaml
 from travdata import dataclassutil
 
+if TYPE_CHECKING:
+    from _typeshed import DataclassInstance
+
 _YAML = yaml.YAML(typ="safe")
+# Retain the original ordering in mappings.
+_YAML.representer.sort_base_mapping_type_on_output = False
 
 __executable_environment__ = "development"
 
 
+_SET_METADATA = {"to_yaml": sorted, "from_yaml": set}
+
+
 class UserError(Exception):
     """Exception raised for user errors."""
 
 
 class YamlDataclassMixin:
     """Mixin for dataclasses created by YAML parsing.
 
@@ -46,14 +56,49 @@
     def __setstate__(self, state):
         try:
             self.__init__(**state)
         except Exception as e:
             e.add_note(f"processing {self.yaml_tag} with {state=}")
             raise
 
+    @classmethod
+    def to_yaml(cls, representer, node):
+        """Implements serialising the node as basic YAML types."""
+        mapping = {}
+        for field in dataclasses.fields(cast(type["DataclassInstance"], cls)):
+            value = getattr(node, field.name)
+            if not value and dataclassutil.has_default(field):
+                continue
+            if fn := field.metadata.get("to_yaml"):
+                value = fn(value)
+            mapping[field.name] = value
+        return representer.represent_mapping(cls.yaml_tag, mapping)
+
+    @classmethod
+    def from_yaml(cls, constructor, node):
+        """Implements deserialising the node from basic YAML types."""
+        data = constructor.construct_mapping(node)
+        if not isinstance(data, dict):
+            raise TypeError(data)
+        kwargs = {}
+        for field in dataclasses.fields(cast(type["DataclassInstance"], cls)):
+            try:
+                value = data.pop(field.name)
+            except KeyError:
+                if dataclassutil.has_default(field):
+                    continue
+                raise
+            if fn := field.metadata.get("from_yaml"):
+                value = fn(value)
+            kwargs[field.name] = value
+        if data:
+            names = ", ".join(sorted(data))
+            raise TypeError(f"unexpected fields {names} in {cls.yaml_tag}")
+        return cls(**kwargs)
+
 
 class RowFolder(abc.ABC):
     """Abstract base marker for configuring row grouping."""
 
 
 @dataclasses.dataclass
 @_YAML.register_class
@@ -90,27 +135,29 @@
     The "path" of group names and the table name form the path for both the
     ``.tabula-template.json`` file within the configuration directory and the
     output ``.csv`` file in the output directory.
     """
 
     file_stem: pathlib.Path
     type: str
+    tags: set[str] = dataclasses.field(default_factory=set)
     extraction: Optional[TableExtraction] = dataclasses.field(default_factory=TableExtraction)
 
 
 @dataclasses.dataclass
 class Group:
     """Group of items to extract from the PDF.
 
     A top-level group within a book is often aligned with a book chapter.
 
     The table items have Tabula templates in ``.directory``.
     """
 
     directory: pathlib.Path
+    tags: set[str] = dataclasses.field(default_factory=set)
     tables: dict[str, Table] = dataclasses.field(default_factory=dict)
     groups: dict[str, "Group"] = dataclasses.field(default_factory=dict)
 
     def all_tables(self) -> Iterator[Table]:
         """Iterates over all tables in this group and its child groups.
 
         :yield: Descendent tables.
@@ -123,14 +170,15 @@
 @dataclasses.dataclass
 class Book(YamlDataclassMixin):
     """Top level information about a book."""
 
     id_: str
     name: str
     default_filename: str
+    tags: set[str] = dataclasses.field(default_factory=set)
     group: Optional[Group] = None
 
 
 @dataclasses.dataclass
 class Config:
     """Top-level configuration."""
 
@@ -139,14 +187,15 @@
 
 
 @dataclasses.dataclass
 @_YAML.register_class
 class _YamlTable(YamlDataclassMixin):
     yaml_tag: ClassVar = "!Table"
     type: Optional[str] = None
+    tags: set[str] = dataclasses.field(default_factory=set, metadata=_SET_METADATA)
     extraction: Optional[TableExtraction] = None
 
     def prepare(self, name: str, directory: pathlib.Path) -> Table:
         """Creates a ``Table`` from self.
 
         :param name: Name of the table within its ``Group.groups``.
         :param directory: Path to the directory of the parent ``Group``,
@@ -157,27 +206,29 @@
         return Table(file_stem=directory / name, **kw)
 
 
 @dataclasses.dataclass
 @_YAML.register_class
 class _YamlGroup(YamlDataclassMixin):
     yaml_tag: ClassVar = "!Group"
+    tags: set[str] = dataclasses.field(default_factory=set, metadata=_SET_METADATA)
     groups: dict[str, "_YamlGroup"] = dataclasses.field(default_factory=dict)
     tables: dict[str, _YamlTable] = dataclasses.field(default_factory=dict)
     extraction_templates: Optional[list[TableExtraction]] = None
 
     def prepare(self, rel_group_dir: pathlib.Path) -> Group:
         """Creates a ``Group`` from self.
 
         :param rel_group_dir: Path to the directory of this group's directory,
         relative to the top-level config directory.
         :return: Prepared ``Group``.
         """
         return Group(
             directory=rel_group_dir,
+            tags=self.tags,
             tables={
                 name: table.prepare(name, rel_group_dir) for name, table in self.tables.items()
             },
             groups={
                 name: group.prepare(rel_group_dir / name) for name, group in self.groups.items()
             },
             # extraction_templates not included, as it is only for use in
@@ -188,14 +239,15 @@
 
 @dataclasses.dataclass
 @_YAML.register_class
 class _YamlBook(YamlDataclassMixin):
     yaml_tag: ClassVar = "!Book"
     name: str
     default_filename: str
+    tags: set[str] = dataclasses.field(default_factory=set, metadata=_SET_METADATA)
 
     def prepare(
         self,
         cfg_dir: pathlib.Path,
         book_id: str,
         limit_books: list[str],
     ) -> Book:
@@ -206,14 +258,15 @@
         :param limit_books: Allowlist of book names to load configuration for.
         :return: Prepared ``Book``.
         """
         book = Book(
             id_=book_id,
             name=self.name,
             default_filename=self.default_filename,
+            tags=self.tags,
         )
         if book_id in limit_books:
             rel_book_dir = pathlib.Path(book_id)
             cfg = _YAML.load(cfg_dir / rel_book_dir / "book.yaml")
             book.group = _prepare_group(cfg, rel_book_dir)
         return book
```

### Comparing `travdata-0.3.1/src/travdata/csvutil.py` & `travdata-0.3.2/src/travdata/csvutil.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.1/src/travdata/datatypes/basic.py` & `travdata-0.3.2/src/travdata/datatypes/basic.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.1/src/travdata/datatypes/core/trade.py` & `travdata-0.3.2/src/travdata/datatypes/core/trade.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.1/src/travdata/datatypes/core/worldcreation.py` & `travdata-0.3.2/src/travdata/datatypes/core/worldcreation.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.1/src/travdata/extraction/parseutil.py` & `travdata-0.3.2/src/travdata/extraction/parseutil.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.1/src/travdata/extraction/pdfextract.py` & `travdata-0.3.2/src/travdata/extraction/pdfextract.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.1/src/travdata/extraction/tabulautil.py` & `travdata-0.3.2/src/travdata/extraction/tabulautil.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.1/src/travdata/gui/extraction/cfgwin.py` & `travdata-0.3.2/src/travdata/gui/extraction/cfgwin.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.1/src/travdata/gui/extraction/runnerwin.py` & `travdata-0.3.2/src/travdata/gui/extraction/runnerwin.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.1/src/travdata/gui/gui.py` & `travdata-0.3.2/src/travdata/gui/gui.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.1/src/travdata/gui/qtutil.py` & `travdata-0.3.2/src/travdata/gui/qtutil.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.1/src/travdata/tableconverters/core/registry.py` & `travdata-0.3.2/src/travdata/tableconverters/core/registry.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.1/src/travdata/tableconverters/core/trade.py` & `travdata-0.3.2/src/travdata/tableconverters/core/trade.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.1/src/travdata/tableconverters/core/worldcreation.py` & `travdata-0.3.2/src/travdata/tableconverters/core/worldcreation.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.1/src/travdata/tableconverters/registry.py` & `travdata-0.3.2/src/travdata/tableconverters/registry.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.1/src/travdata/travellermap/apiurls.py` & `travdata-0.3.2/src/travdata/travellermap/apiurls.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.1/src/travdata/travellermap/sectorparse.py` & `travdata-0.3.2/src/travdata/travellermap/sectorparse.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.1/src/travdata/travellermap/world.py` & `travdata-0.3.2/src/travdata/travellermap/world.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.1/PKG-INFO` & `travdata-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: travdata
-Version: 0.3.1
+Version: 0.3.2
 Summary: Data utility code for Mongoose Traveller TTRPG.
 Home-page: https://github.com/huin/travdata
 License: MIT
 Keywords: traveller,ttrpg
 Author: John Beisley
 Author-email: johnbeisleyuk@gmail.com
 Requires-Python: >=3.11,<4.0
```

