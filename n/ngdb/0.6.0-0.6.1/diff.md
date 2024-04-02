# Comparing `tmp/ngdb-0.6.0.tar.gz` & `tmp/ngdb-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngdb-0.6.0.tar", last modified: Sat Mar 30 18:25:12 2024, max compression
+gzip compressed data, was "ngdb-0.6.1.tar", last modified: Tue Apr  2 07:05:22 2024, max compression
```

## Comparing `ngdb-0.6.0.tar` & `ngdb-0.6.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-03-30 18:25:12.886076 ngdb-0.6.0/
--rw-r--r--   0 davep      (501) staff       (20)     6449 2024-03-30 18:25:12.885999 ngdb-0.6.0/PKG-INFO
--rw-r--r--   0 davep      (501) staff       (20)     5137 2024-03-30 16:24:04.000000 ngdb-0.6.0/README.md
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-03-30 18:25:12.883965 ngdb-0.6.0/ngdb/
--rw-r--r--   0 davep      (501) staff       (20)     1035 2024-03-30 17:59:28.000000 ngdb-0.6.0/ngdb/__init__.py
--rw-r--r--   0 davep      (501) staff       (20)     4359 2024-03-30 18:01:10.000000 ngdb-0.6.0/ngdb/dosify.py
--rw-r--r--   0 davep      (501) staff       (20)    10252 2024-03-30 18:05:02.000000 ngdb-0.6.0/ngdb/entry.py
--rw-r--r--   0 davep      (501) staff       (20)     8637 2024-03-30 18:18:15.000000 ngdb-0.6.0/ngdb/guide.py
--rw-r--r--   0 davep      (501) staff       (20)     1195 2024-03-30 18:07:24.000000 ngdb-0.6.0/ngdb/link.py
--rw-r--r--   0 davep      (501) staff       (20)     2269 2024-03-30 18:07:43.000000 ngdb-0.6.0/ngdb/menu.py
--rw-r--r--   0 davep      (501) staff       (20)    12400 2024-03-30 18:10:14.000000 ngdb-0.6.0/ngdb/parser.py
--rw-r--r--   0 davep      (501) staff       (20)     1955 2024-03-30 18:10:37.000000 ngdb-0.6.0/ngdb/prompts.py
--rw-r--r--   0 davep      (501) staff       (20)        0 2024-03-30 16:24:04.000000 ngdb-0.6.0/ngdb/py.typed
--rw-r--r--   0 davep      (501) staff       (20)     7629 2024-03-30 18:18:26.000000 ngdb-0.6.0/ngdb/reader.py
--rw-r--r--   0 davep      (501) staff       (20)     2130 2024-03-30 18:13:05.000000 ngdb-0.6.0/ngdb/seealso.py
--rw-r--r--   0 davep      (501) staff       (20)     1963 2024-03-30 18:13:27.000000 ngdb-0.6.0/ngdb/types.py
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-03-30 18:25:12.885765 ngdb-0.6.0/ngdb.egg-info/
--rw-r--r--   0 davep      (501) staff       (20)     6449 2024-03-30 18:25:12.000000 ngdb-0.6.0/ngdb.egg-info/PKG-INFO
--rw-r--r--   0 davep      (501) staff       (20)      510 2024-03-30 18:25:12.000000 ngdb-0.6.0/ngdb.egg-info/SOURCES.txt
--rw-r--r--   0 davep      (501) staff       (20)        1 2024-03-30 18:25:12.000000 ngdb-0.6.0/ngdb.egg-info/dependency_links.txt
--rw-r--r--   0 davep      (501) staff       (20)       11 2024-03-30 18:25:12.000000 ngdb-0.6.0/ngdb.egg-info/top_level.txt
--rw-r--r--   0 davep      (501) staff       (20)      124 2024-03-30 18:19:59.000000 ngdb-0.6.0/pyproject.toml
--rw-r--r--   0 davep      (501) staff       (20)     1400 2024-03-30 18:25:12.886368 ngdb-0.6.0/setup.cfg
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-03-30 18:25:12.885587 ngdb-0.6.0/tests/
--rw-r--r--   0 davep      (501) staff       (20)      459 2024-03-30 16:24:04.000000 ngdb-0.6.0/tests/__init__.py
--rw-r--r--   0 davep      (501) staff       (20)     1049 2024-03-30 16:24:04.000000 ngdb-0.6.0/tests/test_dosify.py
--rw-r--r--   0 davep      (501) staff       (20)     1715 2024-03-30 16:24:04.000000 ngdb-0.6.0/tests/test_guide_base.py
--rw-r--r--   0 davep      (501) staff       (20)     7544 2024-03-30 16:24:04.000000 ngdb-0.6.0/tests/test_guide_entry.py
--rw-r--r--   0 davep      (501) staff       (20)     1817 2024-03-30 16:24:04.000000 ngdb-0.6.0/tests/test_guide_header.py
--rw-r--r--   0 davep      (501) staff       (20)     2364 2024-03-30 16:24:04.000000 ngdb-0.6.0/tests/test_guide_menu.py
--rw-r--r--   0 davep      (501) staff       (20)     3578 2024-03-30 16:24:04.000000 ngdb-0.6.0/tests/test_navigation.py
--rw-r--r--   0 davep      (501) staff       (20)     8471 2024-03-30 16:24:21.000000 ngdb-0.6.0/tests/test_parser.py
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-02 07:05:22.014285 ngdb-0.6.1/
+-rw-r--r--   0 davep      (501) staff       (20)     6449 2024-04-02 07:05:22.014230 ngdb-0.6.1/PKG-INFO
+-rw-r--r--   0 davep      (501) staff       (20)     5137 2024-03-30 16:24:04.000000 ngdb-0.6.1/README.md
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-02 07:05:22.012427 ngdb-0.6.1/ngdb/
+-rw-r--r--   0 davep      (501) staff       (20)     1035 2024-04-02 07:04:23.000000 ngdb-0.6.1/ngdb/__init__.py
+-rw-r--r--   0 davep      (501) staff       (20)     4522 2024-03-31 11:45:51.000000 ngdb-0.6.1/ngdb/dosify.py
+-rw-r--r--   0 davep      (501) staff       (20)    10257 2024-03-31 11:45:51.000000 ngdb-0.6.1/ngdb/entry.py
+-rw-r--r--   0 davep      (501) staff       (20)     8647 2024-03-31 11:45:51.000000 ngdb-0.6.1/ngdb/guide.py
+-rw-r--r--   0 davep      (501) staff       (20)     1195 2024-03-30 19:13:27.000000 ngdb-0.6.1/ngdb/link.py
+-rw-r--r--   0 davep      (501) staff       (20)     2269 2024-03-30 19:13:27.000000 ngdb-0.6.1/ngdb/menu.py
+-rw-r--r--   0 davep      (501) staff       (20)    12639 2024-03-31 11:45:51.000000 ngdb-0.6.1/ngdb/parser.py
+-rw-r--r--   0 davep      (501) staff       (20)     2107 2024-03-31 11:45:51.000000 ngdb-0.6.1/ngdb/prompts.py
+-rw-r--r--   0 davep      (501) staff       (20)        0 2024-03-30 16:24:04.000000 ngdb-0.6.1/ngdb/py.typed
+-rw-r--r--   0 davep      (501) staff       (20)     7634 2024-03-31 11:45:51.000000 ngdb-0.6.1/ngdb/reader.py
+-rw-r--r--   0 davep      (501) staff       (20)     2135 2024-03-31 11:45:51.000000 ngdb-0.6.1/ngdb/seealso.py
+-rw-r--r--   0 davep      (501) staff       (20)     1963 2024-03-30 19:13:27.000000 ngdb-0.6.1/ngdb/types.py
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-02 07:05:22.014015 ngdb-0.6.1/ngdb.egg-info/
+-rw-r--r--   0 davep      (501) staff       (20)     6449 2024-04-02 07:05:22.000000 ngdb-0.6.1/ngdb.egg-info/PKG-INFO
+-rw-r--r--   0 davep      (501) staff       (20)      510 2024-04-02 07:05:22.000000 ngdb-0.6.1/ngdb.egg-info/SOURCES.txt
+-rw-r--r--   0 davep      (501) staff       (20)        1 2024-04-02 07:05:22.000000 ngdb-0.6.1/ngdb.egg-info/dependency_links.txt
+-rw-r--r--   0 davep      (501) staff       (20)       11 2024-04-02 07:05:22.000000 ngdb-0.6.1/ngdb.egg-info/top_level.txt
+-rw-r--r--   0 davep      (501) staff       (20)      124 2024-03-30 19:13:27.000000 ngdb-0.6.1/pyproject.toml
+-rw-r--r--   0 davep      (501) staff       (20)     1400 2024-04-02 07:05:22.014539 ngdb-0.6.1/setup.cfg
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-02 07:05:22.013834 ngdb-0.6.1/tests/
+-rw-r--r--   0 davep      (501) staff       (20)      448 2024-03-30 19:13:27.000000 ngdb-0.6.1/tests/__init__.py
+-rw-r--r--   0 davep      (501) staff       (20)     1031 2024-03-30 19:13:27.000000 ngdb-0.6.1/tests/test_dosify.py
+-rw-r--r--   0 davep      (501) staff       (20)     1684 2024-03-30 19:13:27.000000 ngdb-0.6.1/tests/test_guide_base.py
+-rw-r--r--   0 davep      (501) staff       (20)     7411 2024-03-30 19:13:27.000000 ngdb-0.6.1/tests/test_guide_entry.py
+-rw-r--r--   0 davep      (501) staff       (20)     1795 2024-03-30 19:13:27.000000 ngdb-0.6.1/tests/test_guide_header.py
+-rw-r--r--   0 davep      (501) staff       (20)     2265 2024-03-30 19:13:27.000000 ngdb-0.6.1/tests/test_guide_menu.py
+-rw-r--r--   0 davep      (501) staff       (20)     3496 2024-03-30 19:13:27.000000 ngdb-0.6.1/tests/test_navigation.py
+-rw-r--r--   0 davep      (501) staff       (20)     7838 2024-03-30 19:13:27.000000 ngdb-0.6.1/tests/test_parser.py
```

### Comparing `ngdb-0.6.0/PKG-INFO` & `ngdb-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngdb
-Version: 0.6.0
+Version: 0.6.1
 Summary: Norton Guide database reading library
 Home-page: https://github.com/davep/ngdb.py
 Author: Dave Pearson
 Author-email: davep@davep.org
 Maintainer: Dave Pearson
 Maintainer-email: davep@davep.org
 License: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `ngdb-0.6.0/README.md` & `ngdb-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `ngdb-0.6.0/ngdb/__init__.py` & `ngdb-0.6.1/ngdb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """ngdb - Norton Guide database reading library."""
 
 ######################################################################
 # Main library information.
 __author__ = "Dave Pearson"
-__copyright__ = "Copyright 2021-2022, Dave Pearson"
+__copyright__ = "Copyright 2021-2024, Dave Pearson"
 __credits__ = ["Dave Pearson"]
 __maintainer__ = "Dave Pearson"
 __email__ = "davep@davep.org"
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 __licence__ = "GPLv3+"
 
 ##############################################################################
 # Import things for easier access.
 from .dosify import make_dos_like
 from .entry import Entry, Long, Short
 from .guide import NortonGuide
```

### Comparing `ngdb-0.6.0/ngdb/dosify.py` & `ngdb-0.6.1/ngdb/dosify.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 """Code to support the DOS heritage of most Norton Guide databases."""
 
 ##############################################################################
+# Python compatibility hackage.
+from __future__ import annotations
+
+##############################################################################
 # Python imports.
 from typing import Final
 
 ##############################################################################
-DOS_MAP: Final = str.maketrans(
+DOS_MAP: Final[dict[int, str]] = str.maketrans(
     {
         0: " ",
         1: "\u263A",
         2: "\u263B",
         3: "\u2665",
         4: "\u2666",
         5: "\u2663",
```

### Comparing `ngdb-0.6.0/ngdb/entry.py` & `ngdb-0.6.1/ngdb/entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
 
 ##############################################################################
 TEntry = Type["Entry"]
 """Type of the type of an entry."""
 
 ##############################################################################
-MAX_LINE_LENGTH: Final = 1024
+MAX_LINE_LENGTH: Final[int] = 1024
 """Maximum size of a line we'll look for in a guide."""
 
 
 ##############################################################################
 class Entry:
     """Norton Guide database entry class."""
```

### Comparing `ngdb-0.6.0/ngdb/guide.py` & `ngdb-0.6.1/ngdb/guide.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,18 +50,18 @@
     Attributes:
         path: The path of the database.
     """
 
     MAGIC: Final = {"EH": "Expert Help", "NG": "Norton Guide"}
     """Lookup for valid database magic markers."""
 
-    TITLE_LENGTH: Final = 40
+    TITLE_LENGTH: Final[int] = 40
     """The length of a title in the header."""
 
-    CREDIT_LENGTH: Final = 66
+    CREDIT_LENGTH: Final[int] = 66
     """The length of a line in the credits."""
 
     def __init__(self, guide: str | Path) -> None:
         """Constructor.
 
         Args:
             guide: The guide to open.
```

### Comparing `ngdb-0.6.0/ngdb/link.py` & `ngdb-0.6.1/ngdb/link.py`

 * *Files identical despite different names*

### Comparing `ngdb-0.6.0/ngdb/menu.py` & `ngdb-0.6.1/ngdb/menu.py`

 * *Files identical despite different names*

### Comparing `ngdb-0.6.0/ngdb/parser.py` & `ngdb-0.6.1/ngdb/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 """Norton Guide parser for the text inside a guide."""
 
 ##############################################################################
+# Python compatibility hackage.
+from __future__ import annotations
+
+##############################################################################
 # Python imports.
 from abc import ABC, abstractmethod
 from enum import Enum, auto
 from typing import Final
 
 ##############################################################################
 # Local imports.
@@ -19,15 +23,15 @@
     BOLD = auto()
     UNDERLINE = auto()
     REVERSE = auto()
     ATTR = auto()
 
 
 ##############################################################################
-CTRL_CHAR: Final = "^"
+CTRL_CHAR: Final[str] = "^"
 """The control character that marks an upcoming attribute."""
 
 
 ##############################################################################
 class ParseState:
     """Raw text parsing state tracking class.
 
@@ -380,15 +384,24 @@
     def open_markup(self, cls: str) -> str:
         return f"[{cls}]"
 
     def close_markup(self, cls: str) -> str:
         del cls
         return "[/]"
 
-    COLOUR_MAP: Final = {1: 4, 3: 6, 4: 1, 6: 3, 9: 21, 11: 14, 12: 196, 14: 11}
+    COLOUR_MAP: Final[dict[int, int]] = {
+        1: 4,
+        3: 6,
+        4: 1,
+        6: 3,
+        9: 21,
+        11: 14,
+        12: 196,
+        14: 11,
+    }
     """DOS to Rich colour mapping. This is just the exceptions."""
 
     @classmethod
     def map_colour(cls, colour: int) -> int:
         """Map a DOS colour into a similar colour from Rich.
 
         Args:
```

### Comparing `ngdb-0.6.0/ngdb/prompts.py` & `ngdb-0.6.1/ngdb/prompts.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 """Provides a class that is the base for a prompt collection."""
 
 ##############################################################################
+# Python compatibility hackage.
+from __future__ import annotations
+
+##############################################################################
 # Python imports.
 from typing import Final, Iterator
 
 ##############################################################################
 # Local imports.
 from .link import Link
 
 
 ##############################################################################
 class PromptCollection:
     """Base class for classes that contain prompt/offset collections."""
 
-    MAX_PROMPT_LENGTH: Final = 128
+    MAX_PROMPT_LENGTH: Final[int] = 128
     """The maximum length of a prompt in a guide."""
 
     def __init__(self) -> None:
         """Constructor."""
         self._count = 0
         self._prompts: tuple[str, ...] = ()
         self._offsets: tuple[int, ...] = ()
```

### Comparing `ngdb-0.6.0/ngdb/reader.py` & `ngdb-0.6.1/ngdb/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
         Once the rest of the library is done and working well this extra bit
         if docstring will likely be removed because work to improve the
         speed of this class will finally take place.
     """
 
     #: The value that marks run-length-encoded spaces.
-    RLE_MARKER: Final = "\xFF"
+    RLE_MARKER: Final[str] = "\xFF"
 
     @classmethod
     def unrle(cls, rle_text: str) -> str:
         """Un-run-length-encode the given string.
 
         Args:
             rle_text: The text that needs expanding.
```

### Comparing `ngdb-0.6.0/ngdb/seealso.py` & `ngdb-0.6.1/ngdb/seealso.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .reader import GuideReader
 
 
 ##############################################################################
 class SeeAlso(PromptCollection):
     """Class to load and hold all the see alsos for a long entry."""
 
-    MAX_SEE_ALSO: Final = 20
+    MAX_SEE_ALSO: Final[int] = 20
     """Max number of see also items we'll handle.
 
     This is the limit published in the Expert Help Compiler manual and,
     while this limit isn't really needed in this code, it does help guard
     against corrupt guides.
     """
```

### Comparing `ngdb-0.6.0/ngdb/types.py` & `ngdb-0.6.1/ngdb/types.py`

 * *Files identical despite different names*

### Comparing `ngdb-0.6.0/ngdb.egg-info/PKG-INFO` & `ngdb-0.6.1/ngdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngdb
-Version: 0.6.0
+Version: 0.6.1
 Summary: Norton Guide database reading library
 Home-page: https://github.com/davep/ngdb.py
 Author: Dave Pearson
 Author-email: davep@davep.org
 Maintainer: Dave Pearson
 Maintainer-email: davep@davep.org
 License: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `ngdb-0.6.0/setup.cfg` & `ngdb-0.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ngdb-0.6.0/tests/test_dosify.py` & `ngdb-0.6.1/tests/test_dosify.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 # Python imports.
 from unittest import TestCase
 
 ##############################################################################
 # Library imports.
 from ngdb import make_dos_like
 
+
 ##############################################################################
 # DOS-a-like text conversion unit tests.
-class TestMakeDOSLike( TestCase ):
+class TestMakeDOSLike(TestCase):
     """Test the utility function that helps with DOS character conversion."""
 
-    def test_empty_string( self ) -> None:
+    def test_empty_string(self) -> None:
         """It can handle an empty string."""
-        self.assertEqual( make_dos_like( "" ), "" )
+        self.assertEqual(make_dos_like(""), "")
 
-    def test_plain_string( self ) -> None:
+    def test_plain_string(self) -> None:
         """It can handle some plain text."""
-        self.assertEqual( make_dos_like( "Hello, World!" ), "Hello, World!" )
+        self.assertEqual(make_dos_like("Hello, World!"), "Hello, World!")
 
-    def test_graphical( self ) -> None:
+    def test_graphical(self) -> None:
         """It can handle some \"graphical\" characters."""
-        self.assertEqual( make_dos_like( "Ä" * 100 ), "─" * 100 )
+        self.assertEqual(make_dos_like("Ä" * 100), "─" * 100)
+
 
 ### test_dosify.py ends here
```

### Comparing `ngdb-0.6.0/tests/test_guide_base.py` & `ngdb-0.6.1/tests/test_guide_header.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,55 @@
-"""Base Norton Guide interaction unit tests."""
+"""Test the main header reading code."""
 
 ##############################################################################
 # Python imports.
 from unittest import TestCase
 
 ##############################################################################
 # Library imports.
 from ngdb import NortonGuide
 
 ##############################################################################
 # Local imports.
-from . import GOOD_GUIDE, MISSING_GUIDE
+from . import GOOD_GUIDE
 
-##############################################################################
-# Test various forms of opening a guide.
-class TestOpen( TestCase ):
-    """Norton Guide opening tests."""
-
-    def test_open_good( self ) -> None:
-        """It should be possible to open a good guide that exists."""
-        guide = NortonGuide( GOOD_GUIDE )
-        self.assertTrue( guide.is_open )
-        guide.close()
-
-    def test_open_missing_guide( self ) -> None:
-        """Opening a missing guide show throw the correct exception."""
-        with self.assertRaises( FileNotFoundError ):
-            _ = NortonGuide( MISSING_GUIDE )
-
-    def test_with_guide( self ) -> None:
-        """It should be possible to open a guide using with."""
-        with NortonGuide( GOOD_GUIDE ) as guide:
-            self.assertTrue( guide.is_open )
-        self.assertFalse( guide.is_open )
 
 ##############################################################################
-# Test str()ing the guide object.
-class TestStr( TestCase ):
-    """Test applying str() to a guide object."""
-
-    def test_str( self ) -> None:
-        """The str() of the object should be the path to the file."""
-        self.assertEqual( str( NortonGuide( GOOD_GUIDE ) ), str( GOOD_GUIDE ) )
+# Test various attributes of a Norton Guide database header.
+class TestGoodHeader(TestCase):
+    """Good Norton Guide database header tests."""
+
+    def setUp(self) -> None:
+        """Set up for the tests."""
+        self.guide = NortonGuide(GOOD_GUIDE)
+
+    def test_is_ng(self) -> None:
+        """It should be possible to test for a valid database."""
+        self.assertTrue(self.guide.is_a)
+
+    def test_menu_count(self) -> None:
+        """The menu count should read correctly."""
+        self.assertEqual(self.guide.menu_count, 1)
+
+    def test_title(self) -> None:
+        """The title should read correctly."""
+        self.assertEqual(self.guide.title, "Expert Guide")
+
+    def test_credits(self) -> None:
+        """The credits should read correctly."""
+        self.assertCountEqual(
+            self.guide.credits,
+            (
+                "Expert Guide",
+                "Copyright (c) 1997-2015 David A. Pearson",
+                "",
+                "email: davep@davep.org",
+                "  web: http://www.davep.org/",
+            ),
+        )
+
+    def test_made_with(self) -> None:
+        """The test guide should be made with the Norton Guide compiler."""
+        self.assertEqual(self.guide.made_with, NortonGuide.MAGIC["NG"])
+
 
-### test_guide_base.py ends here
+### test_guide_header.py ends here
```

### Comparing `ngdb-0.6.0/tests/test_guide_entry.py` & `ngdb-0.6.1/tests/test_guide_entry.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,186 +2,196 @@
 
 ##############################################################################
 # Python imports.
 from unittest import TestCase
 
 ##############################################################################
 # Library imports.
-from ngdb       import NortonGuide, Short, Long, UnknownEntryType
+from ngdb import Long, NortonGuide, Short, UnknownEntryType
 from ngdb.types import EntryType
 
 ##############################################################################
 # Local imports.
 from . import BIG_GUIDE
 
+
 ##############################################################################
 # Unknown entry type tests.
-class TestUnknown( TestCase ):
+class TestUnknown(TestCase):
     """Test picking up on an unknown entry type."""
 
-    def test_unknown( self ) -> None:
+    def test_unknown(self) -> None:
         """Attempting to load an unknown entry type should result in an exception."""
-        with self.assertRaises( UnknownEntryType ):
-            NortonGuide( BIG_GUIDE ).goto( 0 ).load()
+        with self.assertRaises(UnknownEntryType):
+            NortonGuide(BIG_GUIDE).goto(0).load()
+
 
 ##############################################################################
 # Test loading up a short entry.
-class TestShort( TestCase ):
+class TestShort(TestCase):
     """Short entry loading unit tests."""
 
-    def setUp( self ) -> None:
+    def setUp(self) -> None:
         """Set up for testing the short entry."""
-        self.entry = NortonGuide( BIG_GUIDE ).goto_first().load()
+        self.entry = NortonGuide(BIG_GUIDE).goto_first().load()
 
-    def test_load_correct_type( self ) -> None:
+    def test_load_correct_type(self) -> None:
         """A short entry should load as the correct type."""
-        self.assertIsInstance( self.entry, Short )
+        self.assertIsInstance(self.entry, Short)
 
-    def test_correct_id( self ) -> None:
+    def test_correct_id(self) -> None:
         """It should have a short entry ID."""
-        self.assertEqual( self.entry.type_id, 0 )
-        self.assertTrue( EntryType.is_short( self.entry.type_id ) )
-        self.assertFalse( EntryType.is_long( self.entry.type_id ) )
+        self.assertEqual(self.entry.type_id, 0)
+        self.assertTrue(EntryType.is_short(self.entry.type_id))
+        self.assertFalse(EntryType.is_long(self.entry.type_id))
 
-    def test_entry_size( self ) -> None:
+    def test_entry_size(self) -> None:
         """It should have the correct size."""
-        self.assertEqual( self.entry.size, 838 )
+        self.assertEqual(self.entry.size, 838)
 
-    def test_parent( self ) -> None:
+    def test_parent(self) -> None:
         """It should not have a parent."""
-        self.assertFalse( bool( self.entry.parent ) )
+        self.assertFalse(bool(self.entry.parent))
 
-    def test_parent_line( self ) -> None:
+    def test_parent_line(self) -> None:
         """It should not have a parent line."""
-        self.assertFalse( self.entry.parent.has_line )
+        self.assertFalse(self.entry.parent.has_line)
 
-    def test_parent_menu( self ) -> None:
+    def test_parent_menu(self) -> None:
         """The test short entry should have a parent menu."""
-        self.assertTrue( self.entry.parent.has_menu )
+        self.assertTrue(self.entry.parent.has_menu)
 
-    def test_parent_prompt( self ) -> None:
+    def test_parent_prompt(self) -> None:
         """The test short entry should have a parent menu prompt."""
-        self.assertTrue( self.entry.parent.has_prompt )
+        self.assertTrue(self.entry.parent.has_prompt)
 
-    def test_previous( self ) -> None:
+    def test_previous(self) -> None:
         """It should not have a previous entry."""
-        self.assertFalse( self.entry.has_previous )
+        self.assertFalse(self.entry.has_previous)
 
-    def test_next( self ) -> None:
+    def test_next(self) -> None:
         """It should not have a next entry."""
-        self.assertFalse( self.entry.has_next )
+        self.assertFalse(self.entry.has_next)
 
-    def test_str_entry( self ) -> None:
+    def test_str_entry(self) -> None:
         """The str() of the entry should be the main text."""
-        str_entry = str( self.entry )
-        self.assertEqual( len( str_entry.split( "\n" ) ), len( self.entry ) )
+        str_entry = str(self.entry)
+        self.assertEqual(len(str_entry.split("\n")), len(self.entry))
 
-    def test_lines_and_offsets( self ) -> None:
+    def test_lines_and_offsets(self) -> None:
         """There should be equal numbers of lines and offsets."""
-        self.assertEqual( len( self.entry.lines ), len( self.entry.offsets ) )
+        self.assertEqual(len(self.entry.lines), len(self.entry.offsets))
 
-    def test_list_like( self ) -> None:
+    def test_list_like(self) -> None:
         """It should be possible to treat a short entry like a list."""
         self.assertEqual(
-            self.entry[ 0 ],
-            ( " OL_95AppTitle()          Set/get the Windows 95 application title.", 1389 )
+            self.entry[0],
+            (
+                " OL_95AppTitle()          Set/get the Windows 95 application title.",
+                1389,
+            ),
         )
         self.assertEqual(
-            self.entry[ 0 ].text,
-            " OL_95AppTitle()          Set/get the Windows 95 application title."
+            self.entry[0].text,
+            " OL_95AppTitle()          Set/get the Windows 95 application title.",
         )
-        self.assertEqual( self.entry[ 0 ].offset, 1389 )
-        self.assertTrue( self.entry[ 0 ].has_offset )
+        self.assertEqual(self.entry[0].offset, 1389)
+        self.assertTrue(self.entry[0].has_offset)
 
-    def test_iter_iter( self ) -> None:
+    def test_iter_iter(self) -> None:
         """It should be possible to treat a short entry like an iterator."""
         self.assertEqual(
-            next( iter( self.entry ) ),
-            ( " OL_95AppTitle()          Set/get the Windows 95 application title.", 1389 )
+            next(iter(self.entry)),
+            (
+                " OL_95AppTitle()          Set/get the Windows 95 application title.",
+                1389,
+            ),
         )
 
+
 ##############################################################################
 # Test loading up a long entry.
-class TestLong( TestCase ):
+class TestLong(TestCase):
     """Long entry loading unit tests."""
 
-    def setUp( self ) -> None:
+    def setUp(self) -> None:
         """Set up for testing the long entry."""
-        self.entry = NortonGuide( BIG_GUIDE ).goto_first().skip().load()
+        self.entry = NortonGuide(BIG_GUIDE).goto_first().skip().load()
 
-    def test_load_correct_type( self ) -> None:
+    def test_load_correct_type(self) -> None:
         """A long entry should load as the correct type."""
-        self.assertIsInstance( self.entry, Long )
+        self.assertIsInstance(self.entry, Long)
 
-    def test_correct_id( self ) -> None:
+    def test_correct_id(self) -> None:
         """It should have a long entry ID."""
-        self.assertEqual( self.entry.type_id, 1 )
-        self.assertFalse( EntryType.is_short( self.entry.type_id ) )
-        self.assertTrue( EntryType.is_long( self.entry.type_id ) )
+        self.assertEqual(self.entry.type_id, 1)
+        self.assertFalse(EntryType.is_short(self.entry.type_id))
+        self.assertTrue(EntryType.is_long(self.entry.type_id))
 
-    def test_entry_size( self ) -> None:
+    def test_entry_size(self) -> None:
         """It should have the correct size."""
-        self.assertEqual( self.entry.size, 940 )
+        self.assertEqual(self.entry.size, 940)
 
-    def test_parent( self ) -> None:
+    def test_parent(self) -> None:
         """It should have a parent."""
-        self.assertTrue( bool( self.entry.parent ) )
+        self.assertTrue(bool(self.entry.parent))
 
-    def test_parent_line( self ) -> None:
+    def test_parent_line(self) -> None:
         """It should have a parent line."""
-        self.assertTrue( self.entry.parent.has_line )
-        self.assertEqual( self.entry.parent.line, 0 )
+        self.assertTrue(self.entry.parent.has_line)
+        self.assertEqual(self.entry.parent.line, 0)
 
-    def test_parent_menu( self ) -> None:
+    def test_parent_menu(self) -> None:
         """The test long entry should have a parent menu."""
-        self.assertTrue( self.entry.parent.has_menu )
+        self.assertTrue(self.entry.parent.has_menu)
 
-    def test_parent_prompt( self ) -> None:
+    def test_parent_prompt(self) -> None:
         """The test long entry should have a parent menu prompt."""
-        self.assertTrue( self.entry.parent.has_prompt )
+        self.assertTrue(self.entry.parent.has_prompt)
 
-    def test_previous( self ) -> None:
+    def test_previous(self) -> None:
         """It should not have a previous entry."""
-        self.assertFalse( self.entry.has_previous )
+        self.assertFalse(self.entry.has_previous)
 
-    def test_next( self ) -> None:
+    def test_next(self) -> None:
         """It should have a next entry."""
-        self.assertTrue( self.entry.has_next )
+        self.assertTrue(self.entry.has_next)
 
-    def test_str_entry( self ) -> None:
+    def test_str_entry(self) -> None:
         """The str() of the entry should be the main text."""
-        str_entry = str( self.entry )
-        self.assertEqual( len( str_entry.split( "\n" ) ), len( self.entry ) )
+        str_entry = str(self.entry)
+        self.assertEqual(len(str_entry.split("\n")), len(self.entry))
 
-    def test_list_like( self ) -> None:
+    def test_list_like(self) -> None:
         """It should be possible to treat a long entry like a list."""
-        self.assertEqual( self.entry[ 0 ], " ^bOL_95AppTitle()" )
+        self.assertEqual(self.entry[0], " ^bOL_95AppTitle()")
 
-    def test_iter_like( self ) -> None:
+    def test_iter_like(self) -> None:
         """It should be possible to treat a long entry like an iterator."""
-        self.assertEqual( next( iter( self.entry ) ), " ^bOL_95AppTitle()" )
+        self.assertEqual(next(iter(self.entry)), " ^bOL_95AppTitle()")
 
-    def test_see_also( self ) -> None:
+    def test_see_also(self) -> None:
         """The test long entry should have a see-also menu."""
-        self.assertTrue( bool( self.entry.see_also ) )
+        self.assertTrue(bool(self.entry.see_also))
 
-    def test_see_also_count( self ) -> None:
+    def test_see_also_count(self) -> None:
         """The test long entry should have the correct number of see-also items."""
-        self.assertEqual( len( self.entry.see_also ), 1 )
+        self.assertEqual(len(self.entry.see_also), 1)
 
-    def test_see_also_text( self ) -> None:
+    def test_see_also_text(self) -> None:
         """The test long entry should have the correct see-also prompt."""
-        self.assertEqual( self.entry.see_also.prompts[ 0 ], "OL_95VMTitle()" )
+        self.assertEqual(self.entry.see_also.prompts[0], "OL_95VMTitle()")
 
-    def test_see_also_offset( self ) -> None:
+    def test_see_also_offset(self) -> None:
         """The test long entry should have the correct see-also offset."""
-        self.assertEqual( self.entry.see_also.offsets[ 0 ], 2355 )
+        self.assertEqual(self.entry.see_also.offsets[0], 2355)
 
-    def test_see_also_list_like( self ) -> None:
+    def test_see_also_list_like(self) -> None:
         """It should be possible to treat the see-also object like a list."""
-        self.assertEqual( self.entry.see_also[ 0 ], ( "OL_95VMTitle()", 2355 ) )
+        self.assertEqual(self.entry.see_also[0], ("OL_95VMTitle()", 2355))
 
-    def test_see_also_iter_like( self ) -> None:
+    def test_see_also_iter_like(self) -> None:
         """It should be possible to treat the see-also object like an iterator."""
-        self.assertEqual( next( iter( self.entry.see_also ) ), ( "OL_95VMTitle()", 2355 ) )
+        self.assertEqual(next(iter(self.entry.see_also)), ("OL_95VMTitle()", 2355))
+
 
 ### test_guide_entry.py ends here
```

### Comparing `ngdb-0.6.0/tests/test_navigation.py` & `ngdb-0.6.1/tests/test_navigation.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,90 +2,94 @@
 
 ##############################################################################
 # Python imports.
 from unittest import TestCase
 
 ##############################################################################
 # Library imports.
-from ngdb import NortonGuide, Short, Long, NGEOF
+from ngdb import NGEOF, Long, NortonGuide, Short
 
 ##############################################################################
 # Local imports.
-from . import GOOD_GUIDE, BIG_GUIDE
+from . import BIG_GUIDE, GOOD_GUIDE
+
 
 ##############################################################################
 # Guide navigation unit tests.
-class TestBasicNavigation( TestCase ):
+class TestBasicNavigation(TestCase):
     """Basic guide navigation unit tests."""
 
-    def setUp( self ) -> None:
+    def setUp(self) -> None:
         """Set up for the tests."""
-        self.guide = NortonGuide( BIG_GUIDE )
+        self.guide = NortonGuide(BIG_GUIDE)
 
-    def test_go_first( self ) -> None:
+    def test_go_first(self) -> None:
         """It should be possible to go to the first entry."""
-        self.assertIsInstance( NortonGuide( BIG_GUIDE ).goto_first().load(), Short )
+        self.assertIsInstance(NortonGuide(BIG_GUIDE).goto_first().load(), Short)
 
-    def test_skip( self ) -> None:
+    def test_skip(self) -> None:
         """It should be possible to skip an entry without reading it."""
-        self.assertIsInstance( NortonGuide( BIG_GUIDE ).goto_first().skip().load(), Long )
+        self.assertIsInstance(NortonGuide(BIG_GUIDE).goto_first().skip().load(), Long)
+
 
 ##############################################################################
 # EOF detection tests.
-class TestEOF( TestCase ):
+class TestEOF(TestCase):
     """Unit tests relating to detecting EOF in a guide."""
 
-    def test_small_eof_skip( self ) -> None:
+    def test_small_eof_skip(self) -> None:
         """A guide with one entry should EOF when skipping."""
-        guide = NortonGuide( GOOD_GUIDE )
+        guide = NortonGuide(GOOD_GUIDE)
         guide.skip()
-        self.assertTrue( guide.eof )
+        self.assertTrue(guide.eof)
 
-    def test_small_eof_load( self ) -> None:
+    def test_small_eof_load(self) -> None:
         """A guide with one entry should not EOF when loading."""
-        guide = NortonGuide( GOOD_GUIDE )
+        guide = NortonGuide(GOOD_GUIDE)
         guide.load()
-        self.assertFalse( guide.eof )
+        self.assertFalse(guide.eof)
 
-    def test_big_eof_skip( self ) -> None:
+    def test_big_eof_skip(self) -> None:
         """A guide with multiple entries should not be EOF early on during skips."""
-        guide = NortonGuide( BIG_GUIDE ).goto_first()
-        for _ in range( 5 ):
+        guide = NortonGuide(BIG_GUIDE).goto_first()
+        for _ in range(5):
             guide.skip()
-            self.assertFalse( guide.eof )
+            self.assertFalse(guide.eof)
 
-    def test_big_eof_load( self ) -> None:
+    def test_big_eof_load(self) -> None:
         """A guide with multiple entries should not be EOF early on during loads."""
-        guide = NortonGuide( BIG_GUIDE ).goto_first()
-        for _ in range( 5 ):
+        guide = NortonGuide(BIG_GUIDE).goto_first()
+        for _ in range(5):
             guide.load()
             guide.skip()
-            self.assertFalse( guide.eof )
+            self.assertFalse(guide.eof)
 
-    def test_small_eof_guard_skip( self ) -> None:
+    def test_small_eof_guard_skip(self) -> None:
         """Attempting to skip past the end of single-entry guide should throw an error."""
-        guide = NortonGuide( GOOD_GUIDE ).goto_first()
-        with self.assertRaises( NGEOF ):
-            for _ in range( 100 ):
+        guide = NortonGuide(GOOD_GUIDE).goto_first()
+        with self.assertRaises(NGEOF):
+            for _ in range(100):
                 guide.skip()
 
-    def test_big_eof_guard_skip( self ) -> None:
+    def test_big_eof_guard_skip(self) -> None:
         """Attempting to skip past the end of multiple-entry guide should throw an error."""
-        guide = NortonGuide( BIG_GUIDE ).goto_first()
-        with self.assertRaises( NGEOF ):
-            for _ in range( 100 ):
+        guide = NortonGuide(BIG_GUIDE).goto_first()
+        with self.assertRaises(NGEOF):
+            for _ in range(100):
                 guide.skip()
 
+
 ##############################################################################
 # Guide iteration tests.
-class TestIter( TestCase ):
+class TestIter(TestCase):
     """Unit tests relating to iterating through a guide."""
 
-    def test_iter_small( self ) -> None:
+    def test_iter_small(self) -> None:
         """It should be possible to iterate through a guide with one entry."""
-        self.assertEqual( len( list( NortonGuide( GOOD_GUIDE ) ) ), 1 )
+        self.assertEqual(len(list(NortonGuide(GOOD_GUIDE))), 1)
 
-    def test_iter_big( self ) -> None:
+    def test_iter_big(self) -> None:
         """It should be possible to iterate through a guide with more than one entry."""
-        self.assertEqual( len( list( NortonGuide( BIG_GUIDE ) ) ), 28 )
+        self.assertEqual(len(list(NortonGuide(BIG_GUIDE))), 28)
+
 
 ### test_navigation.py ends here
```

### Comparing `ngdb-0.6.0/tests/test_parser.py` & `ngdb-0.6.1/tests/test_parser.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,245 +1,224 @@
 """Norton Guide entry content markup unit tests."""
 
 ##############################################################################
+# Python compatibility hackage.
+from __future__ import annotations
+
+##############################################################################
 # Python imports.
-from typing   import Any, Iterator, Union
+from typing import Any, Iterator, List, Tuple, Union
 from unittest import TestCase
 
 ##############################################################################
+# Backward compatibility.
+from typing_extensions import TypeAlias
+
+##############################################################################
 # Library imports.
-from ngdb        import BaseParser, PlainText
+from ngdb import BaseParser, PlainText
 from ngdb.parser import RichText
 
+
 ##############################################################################
 # Plain text parser tests.
-class TestPlainText( TestCase ):
+class TestPlainText(TestCase):
     """Perform parser tests against the plain text parser."""
 
-    def test_empty_string( self ) -> None:
+    def test_empty_string(self) -> None:
         """It can handle an empty line."""
-        self.assertEqual( str( PlainText( "" ) ), "" )
+        self.assertEqual(str(PlainText("")), "")
 
-    def test_no_markup( self ) -> None:
+    def test_no_markup(self) -> None:
         """It can handle a line with no markup."""
-        self.assertEqual( str( PlainText( "Test" ) ), "Test" )
+        self.assertEqual(str(PlainText("Test")), "Test")
 
-    def test_strips_non_text_markup( self ) -> None:
+    def test_strips_non_text_markup(self) -> None:
         """It should strip all non-text markup without issue."""
         self.assertEqual(
-            str( PlainText( "^A10This ^Bis ^Na ^Rtest, ^Ureally it is." ) ),
-            "This is a test, really it is."
+            str(PlainText("^A10This ^Bis ^Na ^Rtest, ^Ureally it is.")),
+            "This is a test, really it is.",
         )
 
-    def test_strips_only_non_text_markup( self ) -> None:
+    def test_strips_only_non_text_markup(self) -> None:
         """It should turn non-text markup only into an empty string."""
-        self.assertEqual( str( PlainText( "^A10^B^N^R^U" ) ), "" )
+        self.assertEqual(str(PlainText("^A10^B^N^R^U")), "")
 
-    def test_ctrl_ctrl( self ) -> None:
+    def test_ctrl_ctrl(self) -> None:
         """^^ should become ^."""
-        self.assertEqual( str( PlainText( "^^" * 10 ) ), "^" * 10 )
+        self.assertEqual(str(PlainText("^^" * 10)), "^" * 10)
 
-    def test_char_code( self ) -> None:
+    def test_char_code(self) -> None:
         """It should be able to handle character codes."""
-        self.assertEqual( str( PlainText( "^C20^C21" ) ), " !" )
+        self.assertEqual(str(PlainText("^C20^C21")), " !")
 
-    def test_truncated_markup( self ) -> None:
+    def test_truncated_markup(self) -> None:
         """It should handle truncated markup."""
-        self.assertEqual( str( PlainText( "^" ) ), "" )
+        self.assertEqual(str(PlainText("^")), "")
 
-##############################################################################
-#: Type of a single event that the TestParser will catch.
-TEvent = Union[ str, tuple[ str, Any ] ]
 
-##############################################################################
-#: Type of the collection of events in the TestParser.
-TEvents = list[ TEvent ]
+TEvent: TypeAlias = Union[str, Tuple[str, Any]]
+"""Type of a single event that the TestParser will catch."""
+
+TEvents: TypeAlias = List[TEvent]
+"""Type of the collection of events in the TestParser."""
+
 
 ##############################################################################
 # Unit-test-oriented Norton Guide line parser.
-class TestParser( BaseParser ):
+class TestParser(BaseParser):
     """Parser class for working with unit tests."""
 
-    def __init__( self, line: str ) -> None:
-
+    def __init__(self, line: str) -> None:
         # First off, we're going to collect all the different events that
         # happen, so start a list for doing that.
         self._events: TEvents = []
 
         # Then call the super.
-        super().__init__( line )
+        super().__init__(line)
 
-    def text( self, text: str ) -> None:
-        self._events.append( ( "T", text ) )
+    def text(self, text: str) -> None:
+        self._events.append(("T", text))
 
-    def colour( self, colour: int ) -> None:
-        self._events.append( ( "A", colour ) )
+    def colour(self, colour: int) -> None:
+        self._events.append(("A", colour))
 
-    def normal( self ) -> None:
-        self._events.append( "N" )
+    def normal(self) -> None:
+        self._events.append("N")
 
-    def bold( self ) -> None:
-        self._events.append( "B" )
+    def bold(self) -> None:
+        self._events.append("B")
 
-    def unbold( self ) -> None:
-        self._events.append( "b" )
+    def unbold(self) -> None:
+        self._events.append("b")
 
-    def reverse( self ) -> None:
-        self._events.append( "R" )
+    def reverse(self) -> None:
+        self._events.append("R")
 
-    def unreverse( self ) -> None:
-        self._events.append( "r" )
+    def unreverse(self) -> None:
+        self._events.append("r")
 
-    def underline( self ) -> None:
-        self._events.append( "U" )
+    def underline(self) -> None:
+        self._events.append("U")
 
-    def ununderline( self ) -> None:
-        self._events.append( "u" )
+    def ununderline(self) -> None:
+        self._events.append("u")
 
-    def char( self, char: int ) -> None:
-        self._events.append( ( "C", char ) )
+    def char(self, char: int) -> None:
+        self._events.append(("C", char))
 
-    def __iter__( self ) -> Iterator[ TEvent ]:
+    def __iter__(self) -> Iterator[TEvent]:
         """The collection of events caught by the parser."""
-        return iter( self._events )
+        return iter(self._events)
+
 
 ##############################################################################
 # Parser event unit tests.
-class TestParseEvents( TestCase ):
+class TestParseEvents(TestCase):
     """Test the various events that happen within a parser."""
 
-    def test_empty_line( self ) -> None:
+    def test_empty_line(self) -> None:
         """There should be no events in an empty line."""
-        self.assertListEqual( list( TestParser( "" ) ), [] )
+        self.assertListEqual(list(TestParser("")), [])
 
-    def test_no_markup( self ) -> None:
+    def test_no_markup(self) -> None:
         """There should be a single text event for a non-markup line."""
-        self.assertListEqual( list( TestParser( "Hello, World!" ) ), [ ( "T", "Hello, World!" ) ] )
+        self.assertListEqual(
+            list(TestParser("Hello, World!")), [("T", "Hello, World!")]
+        )
 
-    def test_colour( self ) -> None:
+    def test_colour(self) -> None:
         """There should be a colour event when there's a ^A."""
         self.assertListEqual(
-            list( TestParser( "Hello, ^A20World!" ) ),
-            [
-                ( "T", "Hello, " ),
-                ( "A", 0x20 ),
-                ( "T", "World!" )
-            ]
+            list(TestParser("Hello, ^A20World!")),
+            [("T", "Hello, "), ("A", 0x20), ("T", "World!")],
         )
 
-    def test_multi_colour( self ) -> None:
+    def test_multi_colour(self) -> None:
         """Multiple there should be multiple colour events with multiple ^A."""
         self.assertListEqual(
-            list( TestParser( "Hello, ^A20World^A64!" ) ),
-            [
-                ( "T", "Hello, " ),
-                ( "A", 0x20 ),
-                ( "T", "World" ),
-                ( "A", 0x64 ),
-                ( "T", "!" )
-            ]
+            list(TestParser("Hello, ^A20World^A64!")),
+            [("T", "Hello, "), ("A", 0x20), ("T", "World"), ("A", 0x64), ("T", "!")],
         )
 
-    def test_same_colour( self ) -> None:
+    def test_same_colour(self) -> None:
         """Two consecutive ^A of the same colour should cause a ^N."""
         self.assertListEqual(
-            list( TestParser( "Hello, ^A20World^A20!" ) ),
-            [
-                ( "T", "Hello, " ),
-                ( "A", 0x20 ),
-                ( "T", "World" ),
-                "N",
-                ( "T", "!" )
-            ]
+            list(TestParser("Hello, ^A20World^A20!")),
+            [("T", "Hello, "), ("A", 0x20), ("T", "World"), "N", ("T", "!")],
         )
 
-    def test_bold( self ) -> None:
+    def test_bold(self) -> None:
         """It should be possible to turn bold on and off with ^B."""
         self.assertListEqual(
-            list( TestParser( "Hello, ^BWorld^B!" ) ),
-            [
-                ( "T", "Hello, " ),
-                "B",
-                ( "T", "World" ),
-                "b",
-                ( "T", "!" )
-            ]
+            list(TestParser("Hello, ^BWorld^B!")),
+            [("T", "Hello, "), "B", ("T", "World"), "b", ("T", "!")],
         )
 
-    def test_char( self ) -> None:
+    def test_char(self) -> None:
         """It should be possible to generate characters with ^C."""
         self.assertListEqual(
-            list( TestParser( "".join( f"^C{n:02x}" for n in range( 256 ) ) ) ),
-            [ ( "C", n ) for n in range( 256 ) ]
+            list(TestParser("".join(f"^C{n:02x}" for n in range(256)))),
+            [("C", n) for n in range(256)],
         )
 
-    def test_normal( self ) -> None:
+    def test_normal(self) -> None:
         """A ^N markup should result in a back-to-normal event."""
         self.assertListEqual(
-            list( TestParser( "Hello, ^NWorld!" ) ),
+            list(TestParser("Hello, ^NWorld!")),
             [
-                ( "T", "Hello, " ),
+                ("T", "Hello, "),
                 "N",
-                ( "T", "World!" ),
-            ]
+                ("T", "World!"),
+            ],
         )
 
-    def test_reverse( self ) -> None:
+    def test_reverse(self) -> None:
         """It should be possible to turn reverse on and off with ^R."""
         self.assertListEqual(
-            list( TestParser( "Hello, ^RWorld^R!" ) ),
-            [
-                ( "T", "Hello, " ),
-                "R",
-                ( "T", "World" ),
-                "r",
-                ( "T", "!" )
-            ]
+            list(TestParser("Hello, ^RWorld^R!")),
+            [("T", "Hello, "), "R", ("T", "World"), "r", ("T", "!")],
         )
 
-    def test_underline( self ) -> None:
+    def test_underline(self) -> None:
         """It should be possible to turn underline on and off with ^U."""
         self.assertListEqual(
-            list( TestParser( "Hello, ^UWorld^U!" ) ),
-            [
-                ( "T", "Hello, " ),
-                "U",
-                ( "T", "World" ),
-                "u",
-                ( "T", "!" )
-            ]
+            list(TestParser("Hello, ^UWorld^U!")),
+            [("T", "Hello, "), "U", ("T", "World"), "u", ("T", "!")],
         )
 
+
 ##############################################################################
 # Test the Rich parser.
-class TestRichParser( TestCase ):
+class TestRichParser(TestCase):
     """Test the Rich-friendly parser."""
 
-    def test_empty_line( self ) -> None:
+    def test_empty_line(self) -> None:
         """An empty line should parse fine."""
-        self.assertEqual( str( RichText( "" ) ), "" )
+        self.assertEqual(str(RichText("")), "")
 
-    def test_no_markup( self ) -> None:
+    def test_no_markup(self) -> None:
         """A line with no markup should parse fine."""
-        self.assertEqual( str( RichText( "Hello, World!" ) ), "Hello, World!" )
+        self.assertEqual(str(RichText("Hello, World!")), "Hello, World!")
 
-    def test_escape_markup( self ) -> None:
+    def test_escape_markup(self) -> None:
         """Text that looks like Rich markup should get escaped."""
-        self.assertEqual( str( RichText( "Hello, [W]orld!" ) ), "Hello, \\[W]orld!" )
+        self.assertEqual(str(RichText("Hello, [W]orld!")), "Hello, \\[W]orld!")
 
-    def test_colour( self ) -> None:
+    def test_colour(self) -> None:
         """A colour attribute should come out as the expected markup."""
-        self.assertEqual( str( RichText( "^A02Hello" ) ), "[color(2) on color(0)]Hello[/]" )
+        self.assertEqual(str(RichText("^A02Hello")), "[color(2) on color(0)]Hello[/]")
 
-    def test_bold( self ) -> None:
+    def test_bold(self) -> None:
         """A bold attribute should turn into the Rich version."""
-        self.assertEqual( str( RichText( "^BHello^b" ) ), "[bold]Hello[/]" )
+        self.assertEqual(str(RichText("^BHello^b")), "[bold]Hello[/]")
 
-    def test_reverse( self ) -> None:
+    def test_reverse(self) -> None:
         """A reverse attribute should turn into the Rich version."""
-        self.assertEqual( str( RichText( "^RHello^r" ) ), "[reverse]Hello[/]" )
+        self.assertEqual(str(RichText("^RHello^r")), "[reverse]Hello[/]")
 
-    def test_underline( self ) -> None:
+    def test_underline(self) -> None:
         """An underline attribute should turn into the Rich version."""
-        self.assertEqual( str( RichText( "^UHello^u" ) ), "[underline]Hello[/]" )
+        self.assertEqual(str(RichText("^UHello^u")), "[underline]Hello[/]")
+
 
 ### test_parser.py ends here
```

